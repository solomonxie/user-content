# Book: Intro to Statistical Learning (ISL)


## Model selection: 「Prediction」 vs. 「Inference」

- If our goal is to **understand** the data, namely the `inference`, then it's better to choose the model with more **interpretability**.
- if our goal is to **predict**, then it's good to go with models that have more **flexibility** but less understandable, sometime it may refer to "non-linear" models.

## Model selection: 「Flexibility」 vs. 「Interpretability」

![snip20181018_5](https://user-images.githubusercontent.com/14041622/47135635-a6a46180-d2e3-11e8-82ad-ce78ab9d7607.png)


## 「Clustering」

`Cluster Analysis` is NOT to compare `input and output(x & y)`, but to compare `two variables (x1 & x2)`,
because in the case there's no clear associate for `x & y`, we have left no choice but to analyze variables themselves.

![image](https://user-images.githubusercontent.com/14041622/47136767-4dd6c800-d2e7-11e8-980f-a8c35dc0012c.png)


## Model selection: 「Quantitative」 vs. 「Qualitative」

- Numerical: Linear Regression
- Categorical: Logistic Regression, boosting, KNN


## Model selection: 「Train MAE」 vs. 「Test MAE」

> In general, we do not really care how well the method works training on the `Training data`.
Rather, we are interested in the accuracy of the predictions that we obtain when we apply our method to previously `Unseen Test data`.

**We’d like to select the model for which the average of this quantity—the `test MSE`—is as small as possible.**

> There is no guarantee that the method with the lowest training MSE will also have the lowest test MSE.

![image](https://user-images.githubusercontent.com/14041622/47139998-c04ba600-d2ef-11e8-8844-5cf29b614cf2.png)

> Regardless of whether overfitting has occurred, we almost always want the `Training MSE` to be SMALLER than the `Test MSE`, 
because most statistical learning methods either directly or indirectly seek to **minimize** the training MSE. Overfitting refers specifically to the case in which a less flexible model would have yielded a smaller test MSE. 


## 「Bias-Variance」 Trade-off

The relationship between `bias`, `Variance` and `Test MSE`

![image](https://user-images.githubusercontent.com/14041622/47142661-fe4bc880-d2f5-11e8-8172-0781bb7d7a5e.png)



## Evaluate Classification: 「Training Error Rate」 vs. 「Test error」

Training Error Rate:
![image](https://user-images.githubusercontent.com/14041622/47143778-88952c00-d2f8-11e8-8ae3-484c11320ff7.png)

Test Error:
![image](https://user-images.githubusercontent.com/14041622/47143791-8cc14980-d2f8-11e8-9a5f-5895d403406a.png)



## 「Bayes Classifier」

![image](https://user-images.githubusercontent.com/14041622/47144104-49b3a600-d2f9-11e8-97be-16cff2247b5d.png)

![image](https://user-images.githubusercontent.com/14041622/47144113-4f10f080-d2f9-11e8-98ca-b1ecf2202089.png)


**`Bayes decision boundary`**: The Bayes classifier’s prediction is determined by the Bayes decision boundary; an observation that falls on the orange side of the boundary will be assigned to the orange class, and similarly an observation on the blue side of the boundary will be assigned to the blue class.

`Bayes Error Rate`: The Bayes classifier produces the lowest possible test error rate, called the Bayes error rate. 
![image](https://user-images.githubusercontent.com/14041622/47144171-710a7300-d2f9-11e8-8166-1b6e951d8b2d.png)

> Note that: In theory we would always like to predict qualitative responses using the `Bayes classifier`. But for real data, we do not know the conditional distribution of Y given X, and so computing the `Bayes classifier` is **impossible**. Therefore, the Bayes classifier serves as an **unattainable gold standard** against which to compare other methods.


## 「K-Nearest Neighbors」 (KNN Classifier)

> Many approaches attempt to estimate the conditional distribution of Y given X, and then classify a given observation to the class with highest estimated probability. One such method is the K-nearest neighbors (KNN) classifier.

![image](https://user-images.githubusercontent.com/14041622/47144685-8f24a300-d2fa-11e8-9040-463ef50bcce7.png)

KNN applies `Bayes rule` and classifies the test observation x0 to the class with the largest probability.


![image](https://user-images.githubusercontent.com/14041622/47145113-91d3c800-d2fb-11e8-96eb-01b9114fa0cc.png)
> In the left-hand panel, we have plotted a small training data set consisting of six blue and six orange observations. Our goal is to make a prediction for the point labeled by the black cross. Suppose that we choose K = 3. Then KNN will first identify the three observations that are closest to the cross. This neighborhood is shown as a circle. It consists of two blue points and one orange point, resulting in estimated probabilities of 2/3 for the blue class and 1/3 for the orange class. Hence KNN will predict that the black cross belongs to the blue class. In the right-hand panel of Figure 2.14 we have applied the KNN approach with K = 3 at all of the possible values for X1 and X2, and have drawn in the corresponding KNN decision boundary.


