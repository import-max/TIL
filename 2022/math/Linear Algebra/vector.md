## Vector

[참고 영상1](https://youtu.be/br7tS1t2SFE)
[참고 영상2](https://youtu.be/CytxrmaUY98)

* Vector = 크기(Magnitude) + Direction(방향)<br> = List(리스트)

예를 들어 어떤 물체가 5km/h로 움직인다는 것은 벡터가 아니다. 크기일뿐, 어느 방향으로 움직이는 지 알 수 없다. <br>즉, 속력이라고 말할 수 있다. 다른 말로는 스칼라(Scalar)라고 한다.
<br>이것에 '동쪽으로' 움직인다는 정보가 더해진다면 '벡터'가 되고, 속도라고도 부른다. 즉, **_속도(Velocity)는 벡터(Vector)다._**

벡터의 정보를 표현할 때 **2차원**을 통해 표현할 수 있다. <br>선형대수의 장점은 이처럼 _2차원뿐만 아니라 수학적으로 3차원을 넘어서까지 다룰 수 있다는 점이다._<br><br>
![image](https://user-images.githubusercontent.com/68390559/149089371-cbab2561-6ebc-4610-9a03-30a70a8f314a.png)<br>
크기는 화살표를 그려서 표현할 수 있다. <br> 크기는 단위마다 시간당 속력을 나타내고, 오른쪽 방향을 향한다. 길이는 속력을 나타낸다.
<br><br>

![image](https://user-images.githubusercontent.com/68390559/149089118-f063ab50-450e-426a-a25f-b28c91a2509a.png)<br>
벡터는 시작점에 관계없이 **크기**와 **방향**만 신경쓰면 된다.<br>
따라서 두 벡터는 크기(길이)도 같고, 방향도 같기 때문에 같은 벡터라고 볼 수 있다.<br><br>
<br>
![image](https://user-images.githubusercontent.com/68390559/149139186-6c33054a-1258-4581-be20-613a8c0049cf.png)<br>
벡터를 매번 이렇게 그려줄 수는 없기 때문에 일반적으로 표현을 한다면, 알파벳 v와 화살표를 사용하여 표현할 수 있다.<br>
벡터를 나타낼 때는 스칼라(일반 숫자)와 비교하기 위해 굵은(bold) 알파벳으로 표현하고 위에 화살표를 그리(거나 생략하)는 편이다.<br>
(5,0) 처럼 나열하여 표현하는 것은 Raw Vector, 2차원 배열로 표현한 것은 Column Vector의 표현방식이다.<br>
대부분 따로 언급이 없으면 Column Vector의 형태를 뜻한다. 이는 수평으로 5만큼, 수직으로 0만큼 이동했다는 뜻이다.<br><br>


![image](https://user-images.githubusercontent.com/68390559/149139568-a4a2367a-e7bb-4e9f-b266-a26935d19662.png)<br>
만약 수평으로 3, 수직으로 4로 이동한 벡터가 있다면 위와같이 표기롤 하며 피타고라스 정리를 통해 벡터의 길이가 5임을 알 수 있다.



<hr>

* Vector Space = 벡터(선형)공간으로, 원소를 벡터라고 한다. 덧셈에 대해 닫혀있는 집합.
* Linear Combination = 선형 결합, Vector를 활용하여 각 항에 상수를 곱할 수 있다. 같은 공간상에 존재하는 벡터들 사이에 가능하다.

![image](https://user-images.githubusercontent.com/68390559/149790948-733ecf90-5923-4b69-b322-2b2be27e69dd.png)<br>
R의 지수 부분의 숫자는 차원을 의미하며, 2차원 공간상에 존재하는 모든 실수(real number)벡터들의 집합을 의미한다.<br>
즉, 어떠한 평면위의 점도 임의의 값을 활용하여 연립방정식을 통해 풀 수 있고 표현할 수 있다. Span R2라고 표현하기도 한다.


* Operation with vectors (벡터의 연산자)
1) Vector addition(덧셈) : 두 개의 벡터는 같은 인덱스끼리 더한다. (component wise)
2) Scalar multiplication(곱셈) : 두 개의 벡터를 활용한 연산이 아닌 1개의 스칼라와 1개의 벡터를 활용한 연산이다.








