
 <!--  ![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/Einstein%20and%20machine%20learning1.jfif)) -->
 
 ![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/Einstein%20teaching%20machine%20learning.jfif)

## **Machine Learning Full Course**

### **TABLE OF CONTENTS **
Days | Topic
-----|--------
 1   | <a href = "#supervised">Supervised Learning</a>
 2   | <a href = "#unsupervised">Unsupervised Learning</a>
 3   | <a href = "#costfun">Cost Function</a>
 4   | <a href = "#GDA">Gradient Descent Algorithm</a>
 5   | <a href = "#MLR">Multiple Linear Regression</a>
 6   | <a href = "#FSGD">Feature Scaling with Gradient Descent</a>
 7   | <a href = "#LR">Classification with Logistic Regression</a>

# Day 1
## Introduction: 

Arthur Samuel popularized the term `Machine Learning`. Machine Learning is the field of study that gives computers the ability to learn without being explicitly programmed. It is a branch of artificial intelligence (AI) and computer science that focuses on the use of data and algorithms to imitate the way humans learn, gradually improving their accuracy.

There are two main types of Machine Learning algorithms. They are:
1. Supervised learning
2. Unsupervised learning

The other types of machine learning algorithms are:
- Recommender system
- Reinforcement learning

## <section id = "supervised">1. Supervised Learning</section>

Supervised learning is a type of machine learning algorithm where the model learns from labeled data or right answer. In supervised learning, the algorithm is trained on a dataset that consists of input-output pairs, where the input data is accompanied by corresponding correct output labels. The goal of supervised learning is to learn a mapping function from input to output so that it can predict the output for new, unseen input data. 

There are two type of supervised learning which are:
i. Regression - Housing Price Prediction
ii. Classification - Finding out if lump is benign or malignant

Difference between Regression and Classification

a. - Regression tries to predict any number from infinitely mant no of possible numbers.
   - Classification Only tries to predict either 0 or 1

b. - Classification: Infinitely large no of possible output
   - Regression: Predict categories of small no of possible outputs

![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/supervised-learning.png)

# Day 2
## <section id = "unsupervised">2. Unsupervised Learning</section>

Unsupervised learning is a type of machine learning algorithm that models its data from the unlabelled data and finds something interesting in it. Unsupervised learning might decide to make group or cluster as we aren't supposed to give `right answer` and angorithm has to find structure in the data.

The few examples of unsupervised learning algorithm are:
- Clustering Google News,
- Clustering DNA microarray,
- Clustering or Grouping Customers
- Clustering similar kind of data

![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/unsupervised-learning.webp)

# Day 3
## <section id = "costfun">Cost Function</section>
Cost Function is a mathematical function that quantifies the difference between the predicted values of a model and the actual observed values. Cost Function in machine learning contains parameters w and b. While performing with the large number of training data, the cost function might get higher as a result a recipocal of 2m is taken. The goal is to get minimum cost function to measures how well the model's predictions align with the actual target values.

When the cost function is minimum or close to zero, it means that the model fits better than the other choices for parameters w and b.

![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/cost%20function.png)

# Day 4
## <section id = "GDA">Gradient Descent Algorithm</section>
Today, I learned about the gradient descent algorithm, which plays a significant role in decreasing the cost function. In this algorithm, the value of 'w' is changed with respect to the derivative of the cost function or the learning rate. The learning rate is typically taken positive and in between 0 and 1. When we use a very low learning rate, the descent steps will be very slow, taking only baby steps. However, using too high a learning rate number can lead to overshooting the gradient descent and failing to converge.

> [!Note]
> When updating 'w' and 'b' simultaneously, update 'w' and 'b' first in a temporary variable, and then copy the temporary variable to 'w' and 'b'. Otherwise, the changed value of 'w' will be in the new updating 'b', leading to incorrect final output values.

![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/gradient%20descent%20algorithm.png)

# Day 5
## <section id = "MLR">Multiple Linear Regression using vectorization</section>

Multiple Linear Regression is the method of perfoming gradient descent of dataset having multiple features or variables to make a prediction. 
For example: Suppose, there are other pieces of information, such as the area of land, number of bedrooms, floors, and age of the home, needed to predict the price of the home.

![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/Day%205/multiple%20feature%20of%20linear%20regression.png)

Gradient Descent can be find from various method. 
- Simple method i.e adding individual list of array
- Using For loop and add individual list of array
- Using mathematical summation function
- Using vectorization

  _Methods can be displays as:_
  
![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/Day%205/vectorization%20part%201.png)

Among among methods, we can use the `vectorization method`, which performs faster as it utilizes the Python library NumPy for the calculations. 

_It can be show as:_

![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/Day%205/efficiency%20of%20vectorization.png)


There are other alternatives to gradient descent called the [Normal Equation](https://towardsdatascience.com/normal-equation-a-matrix-approach-to-linear-regression-4162ee170243#:~:text=Limitations%3A,for%20more%20than%2010K%20features.), which is suitable only for linear equations. It solves for 'w' and 'b' without iteration but becomes slow when the number of features is large (> 10,000) 

![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/Day%205/Normal%20Equation.png)

# Day 6
### <section id = "FSGD">Feature Scaling for Gradient Descent</section>
Feature scaling is a method used to normalize the range of independent variables or features of data. Suppose, if you have multiple independent variables like age, salary, and height with the range of (18-60years), (NRS.10,000- to NRS.2,50,000) and (0.5m to 2m), then feature scaling will help them to be in same range (especially 0 - 1).

### Feature Scaling is importance for the following reasons: 
 - It helps to navigate the direct path to the global minimum.
 - Imagine the cost function like a landscape with hills and valleys. Feature scaling creates a smoother landscape for gradient descent to navigate. This smoother landscape allows the algorithm to take larger steps towards the minimum, making the optimization process more efficient.
 - Equal footing of the features, so that other features with large magnitude differences do not overshadow the smaller features.

### Following are the methods that can be utilized to perform scaling:
 - Feature Scaling
 - Mean Normalization
 - Z-score Normalization

_We can identify the problems of gradient descent by the following methods:_

![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/Day%206/learning%20rate%20and%20curve.png)

# Day 7
### <section id = "LR">Classification with Logistic Regression</section>

Today, I introduced myself with simoid function or logistic function and logistic regression and then performed classification using linear and non-linear decision boundaries.  The reason why we used logistic regression instead of linear regression for classification is, linear regression does not work properly for classification in every aspect where logistic regression can do most often. 

![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/Day%207/Logistic%20Regression.png)

We can categorises the decision boundaries in two types. Type are:
- Linear Decision Boundaries
- Non-Linear Decision Boundaries


![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/Day%207/decision%20boundaries.png)

 
