# Lecture03. Locally Weighted & Logistic Regression

* Topic
  - Locally Weighted Regression<br>
  - Probabilistic interpretation of linear regression<br>
  - Logistic regression (Classfication Algorihtm)<br>
  - Newton's method (for linear regression) <br>
<hr>

### Locally weighted Regression<br>

Locally weighted Regression is a way to modify linear regressions and make it fit very non-linear functions.
It depends on what I learned in linear regression.

Q. Fitting models to data is what are the features I want.

Feature selection algorithm is a type of algorithm for automatically deciding.

- Parametic learning algorithms : Fix some fixed set of parameters such as theta. 
The thing what I have to do is just fitting parameters like theta to minimize the cost functions.
It doesn't matter the size/amount of data.
Focusing on the training examples that are close to where I want to make a prediction. The values are similar on the x axis.
To make a prediction, I will use the line that just fit to make a prediction at that value of x
What i wound do is focus on the local area and use the straight line.
Fit theta to minimize a modified cost function.
W(i) is the weighting function makes a value between 0 and 1 that tells me how much should I pay attention to the values of xi,yi. Cost Function, Not Gaussian bell curve(density)
ex)linear regression

- Non-parametic learning algorithms : The amount of data/parameters keep grow with the size of training set.
The amount of stuff grows linearly as a function of the training set size.
It is not good for the massive dataset because I need to keep all of data in my computer memory/disk to make predictions.
ex) locally weighted regression



* tau
* Overfitting, Underfitting

*The reason why we use a squared error

A probabilistic interpretation of linear regression

Why Least squares?
Epsilon i E(i) is distrubted Gaussian would mean 0 and co-variance sigma squared.(Normal distrubution)

* IID (Independently and Identically Distributed)

; semicolon..theta is not a random variable..

* MLE (Maximum Likelihood Estimation) :  The theta to maximize the likelikehood
i.e. choose theta to minimize the likelihood (J(theta)) + sigma squared

* Classification
- Binary Classification 

Linear Regression isn't a good algorithm for classification. Because it fits very bad...

Logistic Regression needs sigmoid function.
There are a lot of loss functions but the reason why picking sigmoid up is there's a broader class of algorithms called generalized linear models.

* Log likelihood
Try to choose value of theta to maximize l(theta) :  gradient descent

Q. Is there a equivalent of normal equations to logistic regression? No.


* Newton's method (big jump) : very fast algorithm
Bigger but more expensive than gradient descent

L prime.. F(theta) Tangent.. Delta..
f of theta is same to l prime of theta (f(theta) = l'(theta)
