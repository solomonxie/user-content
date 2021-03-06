#  ❖ Significant Difference Test (Proportions)

> "_Hypothesis Test for difference_", which sounds more intuitive with _significant different test_ because it's testing for a significant difference.

[Refer to Khan academy: Hypothesis test for difference in proportions](https://www.khanacademy.org/math/ap-statistics/two-sample-inference/modal/v/hypothesis-test-for-difference-in-proportions)

[`▶ Jump back to previous note on: One-sample Z Test`](https://github.com/solomonxie/solomonxie.github.io/issues/50#issuecomment-420189772)

> Reminder: One-sample Z Test
![image](https://user-images.githubusercontent.com/14041622/45408926-514fb180-b6a0-11e8-8174-1a360944483c.png)


## Formula for 「Two-Sample Z Test」

Combining the proportion of successes
In this type of test, it's useful to first calculate the pooled (or combined) proportion of successes in both samples:

![image](https://user-images.githubusercontent.com/14041622/45471111-a94eec80-b762-11e8-9de2-5c9bade7c136.png)

> We do significance tests assuming that the null hypothesis is true. In this test, our null hypothesis is that the two population proportions are equal, but we don't have a hypothesized value for their common proportion. Our best estimate for this value is Ṕc. We'll use this pooled (or combined) value in the standard error formula where we'd ideally use each population proportion.


![image](https://user-images.githubusercontent.com/14041622/45471171-ddc2a880-b762-11e8-8fdd-59dbd9a5e162.png)

The `Hypothesis difference` is 0 when `H₀: p1 - p2 = 0`.



## Z-value in 「Two-sample Z Test」

### Example
![image](https://user-images.githubusercontent.com/14041622/45471059-77d62100-b762-11e8-9ca1-38abd611aac4.png)
Solve:
- Combining the proportion of successes:
![image](https://user-images.githubusercontent.com/14041622/45471269-1cf0f980-b763-11e8-8f6b-0a217e216ddd.png)
- Input values to formula:
![image](https://user-images.githubusercontent.com/14041622/45471292-3134f680-b763-11e8-9414-d22415e9d0aa.png)



## P-value in a 「Two-sample Z Test」

### Example
![image](https://user-images.githubusercontent.com/14041622/45472166-fc766e80-b765-11e8-8ef0-b2d324717cf4.png)
Solve:
- Calculate `z-score`:
![image](https://user-images.githubusercontent.com/14041622/45472536-149abd80-b767-11e8-9405-051427dc3c44.png)
- Since the Alternative hypothesis is `Ha: p1 ≠ p2`, so we're to add up **both tails** of probabilities:
![image](https://user-images.githubusercontent.com/14041622/45472579-3136f580-b767-11e8-8251-0ca75d92a5a3.png)



