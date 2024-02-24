
 <!--  ![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/Einstein%20and%20machine%20learning1.jfif)) -->
 
 ![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/Einstein%20teaching%20machine%20learning.jfif)

# **Machine Learning Full Course**
# Day 1
## Introduction: 

Arthur Samuel popularized the term `Machine Learning`. Machine Learning is the field of study that gives computers the ability to learn without being explicitly programmed. It is a branch of artificial intelligence (AI) and computer science that focuses on the use of data and algorithms to imitate the way humans learn, gradually improving their accuracy.

There are two main types of Machine Learning algorithms. They are:
1. Supervised learning
2. Unsupervised learning

The other types of machine learning algorithms are:
- Recommender system
- Reinforcement learning

# 1. Supervised Learning

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
# 2. Unsupervised Learning

Unsupervised learning is a type of machine learning algorithm that models its data from the unlabelled data and finds something interesting in it. Unsupervised learning might decide to make group or cluster as we aren't supposed to give `right answer` and angorithm has to find structure in the data.

The few examples of unsupervised learning algorithm are:
- Clustering Google News,
- Clustering DNA microarray,
- Clustering or Grouping Customers
- Clustering similar kind of data

![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/unsupervised-learning.webp)

# Day 3
## Cost Function
Cost Function is a mathematical function that quantifies the difference between the predicted values of a model and the actual observed values. Cost Function in machine learning contains parameters w and b. While performing with the large number of training data, the cost function might get higher as a result a recipocal of 2m is taken. The goal is to get minimum cost function to measures how well the model's predictions align with the actual target values.

When the cost function is minimum or close to zero, it means that the model fits better than the other choices for parameters w and b.

![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/cost%20function.png)

# Day 4
# Gradient Descent Algorithm
Today, I learned about the gradient descent algorithm, which plays a significant role in decreasing the cost function. In this algorithm, the value of 'w' is changed with respect to the derivative of the cost function or the learning rate. The learning rate is typically taken positive and in between 0 and 1. When we use a very low learning rate, the descent steps will be very slow, taking only baby steps. However, using too high a learning rate number can lead to overshooting the gradient descent and failing to converge.

> [!Note] :
> When updating 'w' and 'b' simultaneously, update 'w' and 'b' first in a temporary variable, and then copy the temporary variable to 'w' and 'b'. Otherwise, the changed value of 'w' will be in the new updating 'b', leading to incorrect final output values.

![](https://github.com/Sudippdn/Machine-Learning-From-the-begining/blob/main/Image/gradient%20descent%20algorithm.png)

