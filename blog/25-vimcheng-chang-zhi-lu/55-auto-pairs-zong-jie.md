#  ❖ Auto-pairs 总结

用过Sublime的都知道，写引号、括号之类配对的文字时，它都会智能的自动补全另一边括号。
同样，VIM也有很多实现它的插件。

其中比较轻量好用的有`autoclose`和`auto-pairs`，而auto-pairs更智能、更全面。

[参考官网：jiangmiao/auto-pairs](https://github.com/jiangmiao/auto-pairs)

官方Repo的介绍很清楚的解释了每种用法，扫一眼就都明白了。

这里记录一些高级的问题。


## `<M-e>`键的问题

初看，并不明白<M>在键盘上是什么？Google了很久也查不到。最后终于在查关键字`Vim Key Notation`发现了，原来`<M>`代表`Meta key`，在很多终端或平台是不支持的。偶尔有支持的，那就是Alt键。这个时候，它和`<A-..>`是同样的意思。

但是，自动补全括号中，有一个`fast wrap`功能，需要用到`<M-e>`键，即`Alt-e`键。可是不管怎么按，在insert还是normal模式按，都只会输出一个奇怪符号`´`，而不执行命令。

为什么？
因为`Alt`快捷键，在很多Terminal或平台都是不支持的，比如Mac的终端。

经过一番查询，Mac的iTerm2可以将Alt(Option)键映射为Meta键。
位置为：Preference -> Profiles -> Keys -> Left Option key -> `ESC+`.

![image](https://user-images.githubusercontent.com/14041622/50380545-6b3c5f80-06a5-11e9-8547-476db30dc966.png)

然后就能解决fast wrap的问题了，效果如官方解释一样非常方便：
```
input: |'hello' (press (<M-e> at |)
output: ('hello')

wrap string, only support c style string
input: |'h\\el\'lo' (press (<M-e> at |)
output ('h\\ello\'')

input: |[foo, bar()] (press (<M-e> at |)
output: ([foo, bar()])
```

除了`<M-e>`即`Alt-e`外，还有很多自动补全括号引号的按键：
```
System Shortcuts:
    <CR>  : Insert new indented line after return if cursor in blank brackets or quotes.
    <BS>  : Delete brackets in pair
    <M-p> : Toggle Autopairs (g:AutoPairsShortcutToggle)
    <M-e> : Fast Wrap (g:AutoPairsShortcutFastWrap)
    <M-n> : Jump to next closed pair (g:AutoPairsShortcutJump)
    <M-b> : BackInsert (g:AutoPairsShortcutBackInsert)

If <M-p> <M-e> or <M-n> conflict with another keys or want to bind to another keys, add

    let g:AutoPairsShortcutToggle = '<another key>'

to .vimrc, if the key is empty string '', then the shortcut will be disabled.
```

如果Alt键太难按，也可以设置mapping如：
- `imap <C-d>e <M-e>`，也就是按`Ctrl-d`，再按e即可。
- `imap <C-d>p <M-p>`，也就是按`Ctrl-d`，再按p即可。
或者：
- `imap <C-d> <Meta>`，那么之后就都一样了，只要按`Ctrl-d`，再按e/p/n/b/{等等

注意：设置映射时候，不能用`inoremap`了，实践中，只有`imap`才能生效。


## JSON自动补全问题

一开始非常奇怪，在我写一个`*.json`文件时候，每次输完一对引号，在其中输入数字时候，所有引号就全部消失。一开始以为是bug，结果发现是插件有意为之！
也就是说，`auto-pairs`等多种插件，都会为了**方便阅读**，自动帮你隐藏JSON中的引号，让它看起来更简介，更像YAML文件。
