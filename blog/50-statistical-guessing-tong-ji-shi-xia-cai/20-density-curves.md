# Density Curves

Some times `histograms` aren't good enough to visualize large amount of dataset. And `Density Curve` plot will solve the problem, as it can take on **any** value in a **continuum**, they're not just thrown into some buckets.

![image](https://user-images.githubusercontent.com/14041622/43827044-72d905a8-9b2b-11e8-81ad-1bdbddfef4a7.png)

Axes (Tricky):
- `X-axis` represents the values of data points
- `Y-axis` represents the **proportion** of certain **interval**, which is up to 1 (or 100%).


## Area

The entire **AREA** under the curve is **100%**, which represent all the data points.

The **percentage** of a interval of data points, is the **AREA** under the curve over the interval. NOT the height of a point.

## Parameters of Density Curves

### Median
For **Symmetric distribution**, the **Median** is right at the middle, which is at 50th percentile.

For **Skewed distribution**, the **[Left side area] = [Right side area] = 50%**.

### Mean
For **Symmetric distribution**, the **Mean** is right at the middle:

![image](https://user-images.githubusercontent.com/14041622/43822845-ec32c44a-9b1f-11e8-8e8f-13f74084ecfe.png)

For **Skewed distribution**, the **Mean** is at the right or left of the **Median**:

![image](https://user-images.githubusercontent.com/14041622/43822931-24963268-9b20-11e8-906f-8e00ebf65047.png)


### Example
![image](https://user-images.githubusercontent.com/14041622/43829010-8cf08754-9b30-11e8-9fd7-c089bc167aec.png)
What is the height of median?

Solve:
- The median is at 50th percentile, which both left & right area are **50%**.
- But we **CAN'T** know exactly where the median is.
- By eyeballing it, the point divide the shape to TWO EQUAL areas is around 5.5,
- But without further information we can't tell the height.


### Example


Solve:
- The **whole area** under the curve is `100%`
- The base is 4, so:
![image](https://user-images.githubusercontent.com/14041622/43828492-3bec938a-9b2f-11e8-971d-d2c423d506f8.png)


### Example
![image](https://user-images.githubusercontent.com/14041622/43829689-223e1cee-9b32-11e8-88bb-6d91fff931ab.png)

Solve:
- The area under the density curve when x>3 is the **whole area**
- Hence the area is 100%


### Example
![image](https://user-images.githubusercontent.com/14041622/43829807-6d860e46-9b32-11e8-94b1-79d7f533f49c.png)

Solve:
- Area over interval `[3,5]` is a triangle.
- Apply the area formula: `1/2 * (5-3)*0.6 = 0.6 = 60%`
