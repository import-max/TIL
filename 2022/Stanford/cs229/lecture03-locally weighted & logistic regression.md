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

