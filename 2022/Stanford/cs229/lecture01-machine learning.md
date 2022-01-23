# Lecture 01. Machine Learning

There are a lot of project of Machine Learning. It is getting much greater than the past.
The amount of being done in machine learning is very strongly up.

## Introduction
The pace of progress in machine learning has accelerated.

## Prerequisities (전제조건)
1. The students should have a knowledge of basic computer skills and principles.
Understand all of those concepts (i.e. Big O notation, queus, stacks, binary trees, etc).
2. The students should have a basic familiarity with probability and statics.
i.e. random variable, expected value of a random variable, variance of a random variable, etc.
3. You should know about the basic linear algebra.
i.e. what's a matrix, vector, multiply two matrices, multiplying matrices and a vector.

 ## Contents
 Class are rely on the convex optimization algorithms. There are another lectures.
 CS230 has a deep access of deep learning.  CS229 & CS229A are also helpful.
 
 ## Machine Learning
* Field of study that gives computers the ability to learn without being explicitly programmed. (Arthur Samuel,1959)
 i.e. finding patters
* Well-posed learning problem

## Supervised Learning
![image](https://user-images.githubusercontent.com/68390559/150683593-76237769-00fb-4866-931f-e90f41028b23.png)

Most widely used tool is supervised learning.
It finds the relationship in the datasets mapping from X(horizontal) to Y(vertical).

## Regression
![image](https://user-images.githubusercontent.com/68390559/150683769-5f1c1e45-d7ab-4c6a-8f3f-d9a1effa3389.png)<br>
Like this situation
It is called a clssification problem if we only have two values of possible output.(0,1)

![image](https://user-images.githubusercontent.com/68390559/150684103-d2a12f75-5a7d-4c62-9714-7dacf610e2e2.png)<br>
If we have two features, we can assume using two-dimensional vectors.

![image](https://user-images.githubusercontent.com/68390559/150684154-0c694813-1c2d-4ef0-aae4-d848e05cd184.png)<br>
Maybe we could seperate out the positive and negative examples using a straight line using learning algorithm.
It's the concept of logistic regression algorithm.



![image](https://user-images.githubusercontent.com/68390559/150684340-da574891-d596-4e5d-b36f-417a5a6823c0.png)<br>
The algorithm called the Support Vector Machine don't use a lot of features. It uses an infinite number of input features.
Support Vector Machine(SVM) is a model for classification to define the decision boundary.
It allows us to use an infinite-dimensional vector to represent a feature.

The effective way to think about computer memory using SVM is the technical method called kernels.
We learn how to build learning algorithms that work with so that the infinitely long lists of features, numbers.
It is one of the relatively effective learning algorithms to solve problems.

## Examples
The heart of supervised learning is that during training, we are given inputs X together with the labels Y.
And we give it both at the same time, and the task of our learning algorithm is to find a mapping so that given a new X.
We can map it to the most appropriate output Y.

In the cases of video about autonomous driving show the learning algorithms.
The algorithms learns using the back-propagation learning algorithms or gradient descents.
After the learning algorithms has learned, the neural networks drives itself through the trained neural networks.

## Machine Learning Strategy (Learning Theory)
We should be more professional about all fileds of effective engineering and all of algorithms.

## Deep Learning
It is the basics of how to train a neural network as well.

## Unsupervised Learning
![image](https://user-images.githubusercontent.com/68390559/150685940-44072621-089e-483d-bc46-17757508778c.png)

It is an unsupervised learning algorithm called K-means clustering.
It figures out and classifies things through same things.

![image](https://user-images.githubusercontent.com/68390559/150686353-2428ea7b-3f48-4b0c-b8fe-1eceecf03202.png)

These are another examples of clustering algorithms.<br>
Unsupervised learning isn't the same as learning clustering.
Unsupervised learning is the concept of using unlabeld data. There is no Y(target,answer) and just X(input). And we should find interesting things about the data.

![image](https://user-images.githubusercontent.com/68390559/150686493-f57f3234-2999-4d6a-80b5-6367a64d5ab1.png)
* Cocktail party problem
Cocktail party problem is another unsupervised learning problem.
It is a phonemenon that the participator could hear through the microphones even if they're in the noisy party room.
But, how can we have the algorithm seperate out the people's voices? That's an supervised learning problem.
Because there are no labels and just sticking microphones and have multiple users at the same time.

It is called ICA(Independent Component Analysis).

* Another example of Unsupervised learning problem
Internet has tons of unlabeled text data but we can learn interesting things about them and figure them out.


## Reinforcement Learning

![image](https://user-images.githubusercontent.com/68390559/150686789-042b878c-6974-4423-a9a5-e6917c0bc0ec.png)<br>
If we want to fly a helicopter, we have two control sticks that we're moving.
But no one know what's the optimal way to move the control stick.
The way we can get a helicopter fly itself is let the helicopter do whatever as training a dog.
We train a dog with repeat. 
We let the dog do whatever it wants, and whenever it behaves well, we say, "Oh, Good dog". But when it misbehaves we say, "Bad dog".
So we let the helicopter do whatever it wants and whenever it flies well.
It is the reinforcement learning algorithms to figure out how to control it over time.
So as to get more good results and fewer of bad things. It's also using for Robotics.
