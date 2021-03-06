#  ❖ Function Area between curve & axes

[►Jump to Khan academy for some practice: Curve areas](https://www.khanacademy.org/math/ap-calculus-bc/bc-applications-definite-integrals/modal/quiz/bc-horizontal-area-quiz)

## Area Between 「X-axis」 & 「Curve」

Strategy:
- Figure out the interval (boundaries) for the definite integral.
- Directly Integrate the function: `ʃ f(x) dx` over the interval.

### Example
![image](https://user-images.githubusercontent.com/14041622/41593733-9cebe77a-73f3-11e8-91bf-8a8d9d6e89a6.png)
Solve:
- The interval is between `0 & x when f(x)=0`.
- Set `f(x) = 0 = 2 + 2cos(x)` -> `cos(x)=-1` -> `x = arccos(-1) = π`
- So the interval is `[0, π]`.
- The area then is `ʃ (2+2cosx) dx` over the interval `[0, π]`
- The result is `2π` from the definite integral .


## Area Between 「Y-axis」 & 「Curve」

Strategy:
- Inverse the function to make it in term of `y`.
- Instead of integrate in term of `x`, we need to integrate in term of `y`.
- Integrate: `ʃ f(y) dy`



### Example
![image](https://user-images.githubusercontent.com/14041622/41611868-c86d34b4-7423-11e8-9a0b-94d052cd9bb8.png)
Solve:
- Now we have the function `f(y) = 15/y`
- Integrate the function in term of `y`:
![image](https://user-images.githubusercontent.com/14041622/41612030-3d01b6f6-7424-11e8-9d98-a6e2beef690a.png)


### Example
![image](https://user-images.githubusercontent.com/14041622/41641168-f89115de-7496-11e8-808a-1094a9034dd5.png)
Solve:
- Integral the function in term of `y`:
![image](https://user-images.githubusercontent.com/14041622/41641800-0df347a6-7499-11e8-86d9-6c740140d81e.png)



## Area Between 「Two curves」
 

 
Strategy:
 
- Subtract smaller area from bigger area (must be positive): `ʃ |f(x)-g(x)| dx`
 

 

 
### Example
 
![image](https://user-images.githubusercontent.com/14041622/41597493-314bc514-7400-11e8-8f84-04ac08653266.png)
 
Solve:
 
![image](https://user-images.githubusercontent.com/14041622/41597717-d38df6da-7400-11e8-9224-06a2a4644cd2.png)
 

 

 
### Example
 
![image](https://user-images.githubusercontent.com/14041622/41599531-17b0a880-7406-11e8-882a-9f8d33632974.png)
 
Solve:
 
- The graph is as below:
 
![image](https://user-images.githubusercontent.com/14041622/41599539-1e41565e-7406-11e8-9fb8-45b2bcc20dd5.png)
 
- We can actually ignore the graph to calculate:
 
![image](https://user-images.githubusercontent.com/14041622/41599704-8e9d6e38-7406-11e8-90a6-a095e8d5a3e9.png)
 


## 「Horizontal areas」 between curves

### Example
![image](https://user-images.githubusercontent.com/14041622/41641877-477e6c4e-7499-11e8-95e2-46ff645b4429.png)
Solve:
- Clearly, it's bit harder to find the x-axis boundaries for the area.
- And the y-axis boundaries could be easily found where as the point two curves intersect.
- So let two equations equal to get two intersect points:
![image](https://user-images.githubusercontent.com/14041622/41642038-c1e4a0b6-7499-11e8-8332-3ee37c8c2415.png)
- And since it's area between two functions, we subtract one from another `f(y) - g(y)` to get:
![image](https://user-images.githubusercontent.com/14041622/41642128-07ba1b8e-749a-11e8-9fb4-412ef88537c4.png)
- So the result would be:
![image](https://user-images.githubusercontent.com/14041622/41642160-1c56d532-749a-11e8-9608-cf55bc24300b.png)

