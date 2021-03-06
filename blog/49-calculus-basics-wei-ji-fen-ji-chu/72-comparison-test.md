#  ❖ Comparison Test

> You can understand `Comparison Test` intuitively as a `Sandwich Test`.

**THIS TEST IS GOOD FOR `RATIONAL EXPRESSIONS`.**

## 「Direct Comparison Test」

Assume that we have a series `a_n`, and we're to make up a similar series to it as `b_n`:

The logic is:
- If `b > a` & `b` **converges**, then `a` **converges** as well.
- If `a > b` & `b` **diverges**, then `a` **diverges** as well.

It's so much easier if you think it graphically.

[▼Refer to video: Comparison Test (KristaKingMath)](https://www.youtube.com/watch?v=ctJGrBzGoss&index=22&list=PLJ8OrXpbC-BPaXEPecIAS_ddViV2_gcYL&t=0s)
![image](https://user-images.githubusercontent.com/14041622/41836071-335c1832-788c-11e8-8370-883596b34704.png)
![image](https://user-images.githubusercontent.com/14041622/41839502-fbe6ede6-7895-11e8-994d-cba3b1663e4b.png)

[▼Refer to xaktly: Comparison Test](http://www.xaktly.com/ComparisonTest.html)
![image](https://user-images.githubusercontent.com/14041622/41899041-01c26114-795e-11e8-99c5-10db043f4e49.png)


### Example
![image](https://user-images.githubusercontent.com/14041622/41838143-27c14d48-7892-11e8-914b-3e656d97a16d.png)
Solve:
- Assume the asked series as `a_n`, and we make up a very similar series bigger than it, as `b_n`:
![image](https://user-images.githubusercontent.com/14041622/41838411-f6f774e8-7892-11e8-9063-45c2a9285b83.png)
- Apply the `p-series test` we get that the `b_n` **converges**.
- Since `a_n < b_n`, so according to the `Sandwich test (Direct comparison test)`, `a_n` **converges** as well.

## 「Limit Comparison Test」

`Limit comparison test` is like an extension when the `Direct comparison test` **won't** work. 
etc., when we compare `a` with `b`, although `b` converges but `a > b`, so we can't make any conclusion.
And that's where the `limit comparison test` comes in place.

The logic is:
- Take the limit of the division `a/b`.
- If the `Limit > 0`, then they **both converges** or **both diverges**.
- If the `Limit ≤ 0`, then there's no conclusion.

[►`Jump over to Khan academy for practice: Limit comparison test`](https://www.khanacademy.org/math/ap-calculus-bc/bc-series/modal/e/limit-comparison-test)

[▼Refer to video: Limit Comparison Test (KristaKingMath)](https://www.youtube.com/watch?v=PPTLtFhAp6c&list=PLJ8OrXpbC-BPaXEPecIAS_ddViV2_gcYL&index=22)
![image](https://user-images.githubusercontent.com/14041622/41836745-3b72364e-788e-11e8-9404-8f862092c188.png)

[▼Refer to xaktly: Limit Comparison Test](http://www.xaktly.com/LimitComparisonTest.html)
![image](https://user-images.githubusercontent.com/14041622/41899002-e801b784-795d-11e8-8b03-9470d5322a47.png)



### Example
![image](https://user-images.githubusercontent.com/14041622/41841203-43c74a30-789a-11e8-807e-8a03986e9276.png)
Solve:
![image](https://user-images.githubusercontent.com/14041622/41841366-ab22aada-789a-11e8-9852-3a781fb63934.png)

### Example
![image](https://user-images.githubusercontent.com/14041622/41842613-e09c44ca-789d-11e8-894b-f12153b03232.png)
Solve:
- We can't easily tell in the comparison who's greater, so we decide to apply the `limit comparison test`:
![image](https://user-images.githubusercontent.com/14041622/41842732-37c91160-789e-11e8-9352-d6cc241e898c.png)

