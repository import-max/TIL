# Lecture02.Linear Regression

Batch/Stochastic gradient descent is an algorithm for fitting linear regression models.<br>
Normal equation is a very efficient way to let you fit linear models.

To motivate linear regression, it is one of the most simplest algorithms.<br>
Self-driving car had a supervised learning peoblem. The way to put pictures with lens in, and output that you want. Maybe the ouput is a continuous value.
It was a regression problem.

The simplelest possible learning algorithm a supervised learning regression problem is linear regression.
가장 효율적인 알고리즘이 선형회귀이다.

The process of supervised learning is using training set and feed them to a learning algorithm.
The learning algorithm makes predictions about the task. This output is called a hypothesis.

When designing a learning algorithm, even though linear regression, the way about structing a machine learning algorithm is important.

## Designing a learning algorithm 알고리즘을 구축하는 방법

지도 학습에서는 왼쪽에 데이터 셋(훈련 데이터)을 가지고 알고리즘에 데이터를 공급하는 것
그리고 목표는 아웃풋(예상 결과)을 출력하는 것

기계학습 알고리즘을 구조화하는 건 중요하다.

알고리즘을 설계할 때 가장 중요한 것은 어떻게 가설 H를 표현하느냐? 이다.
보통 하나의 입력X만 있지만 여러 데이터가 입력값인 경우가 있을 수도 있다.

표기법을 단순화하기 위해
h(x) = 시그마 어쩌고 저쩌고로 표현..

* How do you represent the hypothesis? We represent as a letter, H(x).

![image](https://user-images.githubusercontent.com/68390559/151367633-423a4ab7-72bd-45c0-9fcf-ef9378ca46c0.png)

h(x)=θ0 + θ1x  (아핀 함수)

   θ0           X0   
[  θ1  ]  =  [  X1  ]
   θ2           X2
   
θ is called parameters.(매개변수)
The role of learning algorithm is to choose parameters to make good predictions about the task.

m = training examples  = rows in table above (훈련 수)
X = input, features, attirubutes 
Y = output,or target variable.

(x,y) is a training example. (훈련 예시)
x(i), y(i)를 나타내기 위해.. 훈련 예제 테이블에 인덱스를 쓰는 방법
x1(1), x1(2) 이런식으로 표현

n = features
x + 세타 = 차원..
두 개의 특징을 가진건 3차원

* 매개변수 theta를 어떻게 선택해서 가설을 출력할 것인가?
h(x)가 y에 가깝도록 선택하는 것.

선형 회귀 알고리즘에서 최소화를 하고 싶어
가설이 출력하는 것 (h theta(x) - y)2(제곱) > 최소화하는 세타값 찾기
(gaussian)

cost function of J > minimize
선형회귀가 모델 일반화라고 하는 더 일반적인 방법

Theta의 비용함수 j를 최소화하는 방법 gradient descent(경사하강법)
모든 0의 벡터와 같음 세타와 같음(3차원)
세타의 초기값과 우리는 세타를 계속 변경할 것이다. 

![image](https://user-images.githubusercontent.com/68390559/151634732-7b33b51f-8f8f-4fde-91cb-5bb98c1416d1.png)

j의 높이를 최소화하는 theta 0, 1찾기
가장 낮은 고도로 가는 것. 발걸음을 반복함.가장 가파른 방향
매개변수를 초기화하는 방법에 따라 도착한다.

theta를 조정하거나 수정하는 방법뿐
learning rate = 학습률(비용함수 J의 편도함수)

함수의 도함수가 가파른 기울기를 정한다.
학습률을 어떻게 결정합니까? 

제곱의 미분을 취해서 어찌저찌된다... X의 theta J에 편도함수를 곱함..
h 세타(x)-y * Xj

Theta J - lr(h theta(x)-y) * Xj
단일 훈련 예제를 사용했지만 실제로는 M개의 데이터가 있다. 도함수 = 도함수의 합

Gradient descent algorightm은 수렴할때까지 반복하고 업데이트를 한다.
각 반복에서 j=0,1,,,n까지 수행한다.

![image](https://user-images.githubusercontent.com/68390559/151635676-860b2290-586a-40c4-9c43-8d14bc80a264.png)
![image](https://user-images.githubusercontent.com/68390559/151635681-ddcb04f7-2c33-4f3e-85fb-6d303bdcdd45.png)

유일한 로컬 최적도 전역 최적
큰 그릇을 보고 수평 조각을 취하고 가장자리가 있는 곳 등을 최적화함
![image](https://user-images.githubusercontent.com/68390559/151635718-8ff6f441-e2a8-4781-8490-3f9effdffa8f.png)
x에서 초기화

항상 90도가 가장 가파르다. 전역 최소값이 하나만 있기 때문에 결국 최소값으로 수렴한다.
알파값을 매우 크게 설정하면 overshoot되어 최소값을 초과할 수 있다. 너무 작으면 반복횟수가 크다.
어떤 학습률이 가장 효율적일지 공부하는 건 좋다.
alpha의 여러 값을 시도하고 보통 지수 척도로 시도한다.(2의배수)

![image](https://user-images.githubusercontent.com/68390559/151635929-59da9e76-a9e2-4e30-b238-b32e1a674ad6.png)
![image](https://user-images.githubusercontent.com/68390559/151635895-47e02666-653f-4568-848b-b042e22d2f7f.png)
theta0 > 0, theta1 > 0 초기화한다면 잘 된다..
반복할때마다 theta의 다른값을 찾으려고 하는 것. 더 나은 데이터를 찾으려고 함.


2차함수. 기울기는 양의 방향이고 줄이기 원하는 것(theta)은 직접 예제를 통해 작업하는 것이 좋다. Theta를 계속 빼
Gradient descent, Linear regression : 가장 많이 쓰여
경사하강법은 각각을 합산하여 계산해. (일괄 경사하강법) batch gradient descent
batch = 전체 데이터를 살피고 모든 예제를 배치로 처리하기 때문에 그런 이름이 붙음. 단점은 큰 데이터 세트가 있는 경우..
ex) 수억개의 데이터가 있는 경우 데이터가 너무 커서 매개변수를 한 번 업데이트하려면 전체 데이터 세트를 검색해야 하기 때문에 계산 과정이 복잡하다는 것(시그마).
단계가 느려져(모든 데이터를 훑어보기 때문에). 그러면 비용이 비싸져.

그 대안법이 있어.
확률적 경사하강법(stochastic gradient)은 매개변수 세타를 업데이트하기 전에 루프를 1~m까지 gradient를 취함.
확률적 경사하강법을 사용하면 매개변수를 어딘가에서 초기화해. 매개변수를 수정해서 예측값을 높여.
가장 직접적인 방법으로 내려가는 건 아니고 확률적으로 계속해서 매개변수를 수정해가면서 내려가지만 최종적으로는 글로벌 최소값으로 하강해 가는것.
실제로 최소값으로 이동하지는 않음. 매개변수가 수렴하지 않기 때문에 앞의 것보다 더 나은 결과를 내려고 노력한다.
아주 큰 데이터가 큰 경우 알고리즘을 훨씬 더 빠르게 진행할 수 있다. 배치보다 stochastic이 실제로 더 많이 사용된다.

확률 > 미니배치로 바꿀수 있니? mini-batch
한번에 한가지 예..가 아님.
일괄 경사 하강법 > 
확률적 경사하강법의 절약 효과는 전역 최적이 아닌 글로벌 매개변수(기계학습에 사용하는 것 ) > 이거는 최소값에 도달하지 못해도 예측을 잘 할 것.
시간이 지남에 따라 학습률이 줄고 진동의 크기가 감소하게 된다. 따라서 어디를 가든 최소값이 아닐 수 있지만 점점 더 반복할수록 최소값에 가까워짐
그래서 lr을 줄이려고 한다.

ta(j)가 갈때까지 멈춰. 선형회귀는 지역 최적값이 없기 때문에 수렴 디버깅 문제가 덜 발생해

둘다 반복 알고리즘, 

## 정규방정식 Normal equation

세타를 같게 설정하는,,, 행렬 곱셈,,, 전역 최소값으로 수렴하게 하는 값,,
도함수... 행렬....f(a)... 2x2 ...
vector matrix  > column vector ...

행렬의 도함수에 대한 정의에 대한 개요는 theta of J > j(theta) = cost function
함수를 최소화하는 것은 세타에 대해 도함수를 취하고 0...으로 ...벡터...
세타의 도함수를 0,0하고 세타를 풀고 세타 공식으로 끝남. 

만약 a가 정방행렬이라면 행의수는 열의 수와 같다.
궤적을 대각선 항목의 합과 같도록 표기.
tr(A) 궤적... 45도 축을 따라 뒤집기 때문에 행렬을 전치할 때 대각선은 동일하게 유지되고 추적은 전치의 추적과 같다.
tr(a) = trAt
f(a) = trAB
삼각형(도함수)Af(a) = BT
tr AB = tr BA 
tr ABC = tr CAB 순환 속성...
A trA AtC = CAtctA x제곱의 도함수가 2_x

j(theta) > 행렬 vector로 표기 X = r
X를 가져와서 행렬에 훈련 예제를 행에 쌓아. X를 design matrix로 부를거야
X(theta) = [matrix][열벡터] 곱하는 것..

Y = 훈련 예제에서 모든 레이블을 가져와 큰 열 벡터에 쌓는 벡터x
x theta - y x1.. ...h(x)(m)- y(x)(m)
zTz = 시그마 z2

도함수(theta)J(theta) = 도함수(theta)1/2(X(theta)-y)T(X(theta)-y)
= 1/2도함수(theta)((theta)TXT-yT)(X(theta)-y)
= 1/2도함수(theta)[....ㅎㅎ]
= cf(ax-b(ax-b(a2x2-axb-bax+b2)))
도함수가 도함수를 전치한다..미분을 0으로 설정...
XtXtheta = XtY
X transpose X inverse = X trasnspose Y> 전역 최소값의 theta값을 얻을 수 있음.
x가 비가역적이라면.. ...반복x > normal equation

To find correct learning rate is empirical.




