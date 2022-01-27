# Lecture02.Linear Regression

Batch/Stochastic gradient descent is an algorithm for fitting linear regression models.<br>
Normal equation is a very efficient way to let you fit linear models.

To motivate linear regression, it is one of the most simplest algorithms.<br>
Self-driving car had a supervised learning peoblem. The way to put pictures with lens in, and output that you want. Maybe the ouput is a continuous value.
It was a regression problem.

The simplelest possible learning algorithm a supervised learning regression problem is linear regression.

The process of supervised learning is using training set and feed them to a learning algorithm.
The learning algorithm makes predictions about the task. This output is called a hypothesis.

When designing a learning algorithm, even though linear regression, the way about structing a machine learning algorithm is important.

## Designing a learning algorithm

* How do you represent the hypothesis? We represent as a letter, H(x).

![image](https://user-images.githubusercontent.com/68390559/151367633-423a4ab7-72bd-45c0-9fcf-ef9378ca46c0.png)

h(x)=θ0 + θ1x

   θ0           X0
[  θ1  ]  =  [  X1  ]
   θ2           X2
   
θ is called parameters.
The role of learning algorithm is to choose parameters to make good predictions about the task.

X = input, or features
Y = output,or target variable.

(x,y) is a training example.

