# Notes on Coursera ML Andrew Ng

In general, any machine learning problem can be assigned to one of two broad classifications:
Supervised learning and Unsupervised learning.

> Tom Mitchell provides a more modern definition: "A computer program is said to learn from experience E with respect to some class of tasks T and performance measure P, if its performance at tasks in T, as measured by P, improves with experience E."


### Supervised learning: "Right answers" given.
- It can be a **Regression problem**, which `predict continuous valued output`,
- also can be a **Classification** problem, which `predict discrete valued output`.


### Unsupervised learning: 
is to find out some **structure** in a dataset, and find out **clusters** is a big part of the work. 
**With unsupervised learning there is NO feedback based on the prediction results.**

### There's also _Non-clustering_ problem for unsupervised learning
like the "cocktail party algorithm".

### _Octave_ 
Octave is much more faster to implement a prototype than other languages. We can first use Octave to test our ideas, models, and transfer it into other languages when it's success.


### Linear regression model
![image](https://user-images.githubusercontent.com/14041622/46943697-d0227a80-d0a2-11e8-9e0e-1d7b28f8b583.png)


### Cost function
![image](https://user-images.githubusercontent.com/14041622/46939279-77e67b00-d098-11e8-8d57-d6c341560ab2.png)


### Contour Plot
![image](https://user-images.githubusercontent.com/14041622/46940434-4c18c480-d09b-11e8-8617-62e1ddc10c91.png)


### Gradient Descent intuition
![image](https://user-images.githubusercontent.com/14041622/46941377-897e5180-d09d-11e8-81e5-d7fcb36f420d.png)

### Gradient descent algorithm
The gradient descent algorithm is: **repeat until convergence:**
![image](https://user-images.githubusercontent.com/14041622/46941457-be8aa400-d09d-11e8-915c-fc255ca27792.png)
where `j=0,1` represents the feature index number.

simultaneously update the parameters θ1, θ2...
![image](https://user-images.githubusercontent.com/14041622/46941394-8edb9c00-d09d-11e8-8d57-0f19d018da00.png)


### "Batch" Gradient descent
**"Batch": Each step of gradient descent computes ALL the training data.**
