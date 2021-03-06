#  ❖ Geometric Random Variables


[Refer to wiki: Geometric distribution](https://www.wikiwand.com/en/Geometric_distribution)
[Refer to Khan academy: Geometric random variables introduction](https://www.khanacademy.org/math/ap-statistics/random-variables-ap/modal/v/geometric-random-variables-introduction)

## 「Geometric Random Variable」 vs. 「Binomial Random Variable」

![image](https://user-images.githubusercontent.com/14041622/44519111-9f574200-a6fe-11e8-8853-bb97da651ec3.png)

- A `binomial setting` has a set number of trials, and the variable in question is the number of successes that occur in those trials.
- A `geometric setting` DOES NOT have a set number of trials, and the variable in question is the number of trials it takes to get the first success.

In both settings, the trials are independent and the probability of success remains the same on each trial.

The only difference between `Geometric R.V.` and `Binomial R.V.` is that, 
**The Geometric R.V. DOES NOT have a certain number of trails.**

Requirements of Geometric R.V.:
- `p`: Same probability p on each trail.
- `Yes-no question`: Each trail's outcome is either success or failure.
- `Independent`: Each trail is independent to each other.


## Understanding「Geometric Probability」

The geometric distribution gives the probability that the first occurrence of success requires k independent trials, each with success probability p.


![image](https://user-images.githubusercontent.com/14041622/44646195-cff3f000-aa0c-11e8-879f-d154367fb2b9.png)


If it's asking for `Number of Trails`, then the number `Trails = failures + success = (n-1) + 1`.
If it's asking for `Number of failures`, then the number `Trails = Failures+1 = n+1`.
**And that's why the formula is slightly different.**

Assume `p` is the probability of success on each trail, `n` is the number of trails or failures:
- `Number of Trials` until the first success:
![image](https://user-images.githubusercontent.com/14041622/44616098-372e6a80-a87c-11e8-8ce6-a6c2f6a42c46.png)
- `Number of Failures` until the first success:
![image](https://user-images.githubusercontent.com/14041622/44616095-309ff300-a87c-11e8-85d5-ee4a2c7a6cc7.png)


### Example
![image](https://user-images.githubusercontent.com/14041622/44615924-08ae9080-a878-11e8-8c36-9bbe1d53e88e.png)
Solve:
![image](https://user-images.githubusercontent.com/14041622/44616241-c2a8fb00-a87e-11e8-80f5-f9311adb2f5b.png)


## 「Mean & Variance」 of Geometric Probability

![image](https://user-images.githubusercontent.com/14041622/44578538-78fcd980-a7c6-11e8-9843-6d1a493afe92.png)



## 「Cumulative Geometric Probability」

We know how to calculate Geometric Probability at each value, but `Cumulative G.P.` would be bit tricky.

![image](https://user-images.githubusercontent.com/14041622/44647029-7ccf6c80-aa0f-11e8-8b52-46a3a8ed1f26.png)

**The formula literally means: FAIL a TIMES IN A ROW.**


This formula is good for `X>a`, and with a bit twist you can get most out of it.
etc., 
- `P(X≥4)` is the same with `P(X>3)`
- `P(X≤5)` is the same with `1 - P(X>5)`
- `P(X<7)` is the same with `1 - P(X>6)`


### Example
![image](https://user-images.githubusercontent.com/14041622/44616397-84f9a180-a881-11e8-921d-c23810a9415c.png)
Solve:
- The easiest way is to apply the cumulative geometric probability formula:
- `P(X<5) = 1 - P(X>4) = 1 - Failure⁴ = 1-0.9^4 = 0.34`
- Another way is to calculate each item in the sequence:
`P(C≤4) = P(C=1) + P(C=2) + P(C=3) + P(C=4)`
- which we expand it to:
`P(C≤4) = 0.9⁰*0.1 + 0.9*0.1 + 0.9²*0.1 + 0.9³*0.1`
- We could easily recognize it as a standard `Geometric Series`, so we can apply the formula:
`P(C≤4) = 0.1 * (1-0.9⁴) / (1-0.9) = 0.34`


### Example
![image](https://user-images.githubusercontent.com/14041622/44616505-bc694d80-a883-11e8-855a-33f0c0bd8517.png)
Solve:
- It's the same as "the probability of 5 failures in a row."
![image](https://user-images.githubusercontent.com/14041622/44616525-10743200-a884-11e8-83f4-6bbaa83e99a7.png)


### Example
![image](https://user-images.githubusercontent.com/14041622/44644301-30336380-aa06-11e8-9f26-73f20abfb177.png)
Solve:
![image](https://user-images.githubusercontent.com/14041622/44644334-4e00c880-aa06-11e8-9794-f2b698bb62f2.png)


