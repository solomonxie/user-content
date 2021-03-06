# LU Decomposition [DRAFT]

For a Matrix A, we could factor it out as `A = LU`, just like we factor a number to two numbers.

[`Online LU Decomposition Calculator`](https://www.wolframalpha.com/input/?i=LU+decomposition+of+%7B%7B7,3,-11%7D,%7B-6,7,10%7D,%7B-11,2,-2%7D%7D&lk=3)

![image](https://user-images.githubusercontent.com/14041622/39573271-176de746-4f05-11e8-9309-26d7d0f664ac.png)

## 「Upper Triangular Matrix」

The factor matrix `U` represents the `Upper Triangular Matrix`, which we're already familiar with: the matrix we've got after `Gauss Elimination`.

Refer to video:[ LU Decomposition using Gaussian Elimination](https://www.youtube.com/watch?v=jbeX2HCW6OE)

![image](https://user-images.githubusercontent.com/14041622/39575064-d1531996-4f0b-11e8-995e-239df4d1214a.png)


## 「Lower Triangular Matrix」

The factor matrix `L` is not hard to get as well: 
**All the numbers in this matrix are `factor numbers` we used in each elimination step.**

![image](https://user-images.githubusercontent.com/14041622/39574447-d81f9198-4f09-11e8-946d-1f1274111884.png)

### How to get the 「Lower Triangular Matrix」

[Refer to this video: LU Decomposition - Shortcut Method by Math is power](https://www.youtube.com/watch?v=UlWcofkUDDU)





## Solve 「System of equations」 using 「LU Decomposition」

> The final **goal** of learning `LU Decomposition` is to **solve Linear systems**.

[Refer to this video: Solve a System of Linear Equations Using LU Decomposition](https://www.youtube.com/watch?v=m3EojSAgIao&feature=youtu.be)

Assume there's equation `AX = B` as below, and we're to solve for `X`: 
![image](https://user-images.githubusercontent.com/14041622/39588763-ffebdd56-4f2e-11e8-8a07-891176ba45e8.png)

Steps to apply the `LU Decomposition` to solve the Linear System:
- Decompose LU, and represent `AX = B` as `LUX = B`
![image](https://user-images.githubusercontent.com/14041622/39590029-47d16bf6-4f32-11e8-9fec-3c8b8f69b577.png)
- Let `Y = UX`, then solve `LY = B` for `Y`
![image](https://user-images.githubusercontent.com/14041622/39589780-b2228144-4f31-11e8-93f7-29aecf55d008.png)
- Solve `Y = UX` for `X`
![image](https://user-images.githubusercontent.com/14041622/39589848-e32dfdf4-4f31-11e8-8856-20deeb25fc7b.png)




