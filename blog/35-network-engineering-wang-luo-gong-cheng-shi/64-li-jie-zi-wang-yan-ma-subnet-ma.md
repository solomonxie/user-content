# ❖ 理解子网掩码 Subnet Mask

**网络掩码的唯一目的是：在一串IP中，区分哪部分是`网络号`，哪部分是`主机号`。**

一般在家里局域网中，假设我自己的电脑IP是`192.168.1.123`：
- 网络号就是`192.168.1`，即一台路由器所负责的“区域”，这片区域**最多**能有253台机器。
- 主机号就是`123`，就是253台机器中的一台。

如果要达到通过IP传输，就必须先找到`网络`，再找到`主机`。
然而，光是一串数字`192.168.1.123`，完全看不出哪部分是网络哪部分是主机。
这时候就必须要借助子网掩码。如果没有子网掩码，就不能实现通讯。

可以想象子网掩码是一个真的Mask面具：
假设IP写在一张纸上，而Mask是另一张用剪刀挖出一个窟窿的纸，然后把它盖在IP纸上，透过窟窿漏出来的那部分就是`主机名`。

那么，通过编程怎么实现这个"面具"呢？
这是一个非常精妙的实现：把`Mask`也设置为一串看似IP地址的数字，然后通过`IP`和`Mask`转换成二进制，并进行`逐位OR计算`。

计算过程：
- 假设IP地址是：`192.168.199.123`, 子网掩码是`255.255.255.0`
- 那么Mask中的255二进制化后变为`1111 1111`，那么IP中所有二进制数与它`按位OR`计算的结果，都是原数本身
- 但是Mask中的0转换为二进制后是`0000 0000`，那么IP中的所有二进制数与它`按位OR`计算的结果，都是0.
- 全部计算完毕后，结果再转换回十进制后是：`192.168.199.0`。
- 因为IP地址中，不能有主机名为`0`，所以这个结果中所有标记为`0`的部分，就指代为主机号范围了。

