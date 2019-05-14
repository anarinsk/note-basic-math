
# Source 

[https://dhruvp.netlify.com/2018/12/31/matrices/](https://dhruvp.netlify.com/2018/12/31/matrices/)

[https://dhruvp.netlify.com/2019/02/25/eigenvectors/](https://dhruvp.netlify.com/2019/02/25/eigenvectors/)

# Multiplication as Arithmetic 

매트릭스를 연산으로 보는 것에 익숙하다. 왜냐하면 이것으로 시험을 봤기 때문이지... 

![](https://upload.wikimedia.org/wikipedia/commons/thumb/e/eb/Matrix_multiplication_diagram_2.svg/313px-Matrix_multiplication_diagram_2.svg.png)

하지만 이러한 이해에는 어떤 직관도 수학적인 묘미도 없다. 

# Matrix as Function 

매트릭스를 함수로 이해할 수 있다. 다만 특별한 성격의 함수들만 가능한다. 이를 linear map이라고 부른다. 리니어 맵의 정의 두 개는 아래와 같다. $f(\cdot)$이 리니어 맵일 때, 

1.  $f(c \cdot x) = c f(x)$
2. $f(x+y) = f(x) + f(y)$

$f(x)=x^2$은 리니어 맵일까? 당연히 아니다. 1, 2 모두 성립하지 않는다. 

# Linear map as ratation and scaling 


![](https://upload.wikimedia.org/wikipedia/commons/thumb/8/87/Rotation_illustration2.svg/1920px-Rotation_illustration2.svg.png)

![scaling example](https://developer.apple.com/library/archive/documentation/Cocoa/Conceptual/CocoaDrawingGuide/Art/scaling_2x.png)

# Examples: Linear Map 

## 1-d

선형의 경우 간단하다. 우리가 아는 덧셈, 그리고 곱셈을 생각하면 되겠다. 

## 2-d
 
 2차원만 되도 사정이 복잡하다. 예를 들어보자. $f(x)$가 일종의 scaling function이라고 하자. $x$ 축으로 3배, $y$ 축으로 5배 이동한다. 이를 그림으로 나타내면 아래와 같다. 

 
![](https://dhruvp.netlify.com/public/images/scaling_f.png)

두 개의 베이시스 $[1,0]^{\rm T}$, $[0, 1]^{\rm T}$를 생각해보자. 이 함수는 다음과 같은 산출을 내놓을 것이다. 

$f\left(\left[ \begin{array}{l}{1} \\ {0}\end{array}\right]\right)=\left[ \begin{array}{l}{3} \\ {0}\end{array}\right]$

$f\left(\left[ \begin{array}{l}{0} \\ {1}\end{array}\right]\right)=\left[ \begin{array}{l}{0} \\ {5}\end{array}\right]$

$f([10, 9]^{\rm T})$는 어떻게 표현될까? 

$f\left(\left[ \begin{array}{l}{10} \\ {9}\end{array}\right]\right)=f\left(\left[ \begin{array}{c}{10} \\ {0}\end{array}\right]\right)+f\left(\left[ \begin{array}{l}{0} \\ {9}\end{array}\right]\right)$

$=10 \cdot f\left(\left[ \begin{array}{l}{1} \\ {0}\end{array}\right]\right)+9 \cdot f\left(\left[ \begin{array}{l}{0} \\ {1}\end{array}\right]\right)$

$=10 \cdot \left[ \begin{array}{l}{3} \\ {0}\end{array}\right]+9 \cdot \left[ \begin{array}{l}{0} \\ {5}\end{array}\right]$

$=\left[ \begin{array}{c}{30} \\ {0}\end{array}\right]+\left[ \begin{array}{c}{0} \\ {45}\end{array}\right]$

$=\left[ \begin{array}{l}{30} \\ {45}\end{array}\right]$

# Matrices 

$\left[f\left(\left[ \begin{array}{l}{1} \\ {0}\end{array}\right]\right) \quad f\left(\left[ \begin{array}{l}{0} \\ {1}\end{array}\right]\right)\right]$

$=\left[ \begin{array}{ll}{3} & {0} \\ {0} & {5}\end{array}\right]$

# Example of Creating a Matrix Representation 

$G=\left[ \begin{array}{cc}{0} & {-1} \\ {1} & {0}\end{array}\right]$ 

- 이 매트릭스는 어떤 변환을 나타내는가? 답부터 말하면, 반 시계 방향으로 $\pi/2$ 만큼 회전시키는 의미를 지닌다. 
- 우선, 앞서 봤던 것처럼 $G$의 첫번째 컬럼은 $[1,0]^{\rm T}$의 변환을 의미한다. 그 의미는 아래의 그림과 같다. 

![](https://dhruvp.netlify.com/public/images/rotation_1_0.png)

- 우선, 앞서 봤던 것처럼 $G$의 두번째 컬럼은 $[0,1]^{\rm T}$의 변환을 의미한다. 그 의미는 아래의 그림과 같다. 


![](https://dhruvp.netlify.com/public/images/rotation_0_1.png)

$G=\left[ \begin{array}{cc}{0} & {-1} \\ {1} & {0}\end{array}\right]$

$[1,0]^{\rm T}$에서 시작한다고 생각하면 $x$축을 $y축으로 반시계 방향으로 뒤집은 이후 다시 한번 반시계방향으로 $\pi/2$ 만큼 회전시키는 것을 의미한다. 

# Applying the Function 


1. The first column of the matrix tells us $g\left(\left[ \begin{array}{l}{1} \\ {0}\end{array}\right]\right)$
3. the second column tells us $g\left(\left[ \begin{array}{l}{0} \\ {1}\end{array}\right]\right)$

$\left[ \begin{array}{l}{x} \\ {y}\end{array}\right]=x \cdot \left[ \begin{array}{c}{1} \\ {0}\end{array}\right]+y \cdot \left[ \begin{array}{c}{0} \\ {1}\end{array}\right]$

$g\left(\left[ \begin{array}{l}{x} \\ {y}\end{array}\right]\right)=g\left(x \cdot \left[ \begin{array}{l}{1} \\ {0}\end{array}\right]+y \cdot \left[ \begin{array}{l}{0} \\ {1}\end{array}\right]\right)$

(by additivity of linear map)

$=g\left(x \cdot \left[ \begin{array}{l}{1} \\ {0}\end{array}\right]\right)+g\left(y \cdot \left[ \begin{array}{l}{0} \\ {1}\end{array}\right]\right)$

(by scalar multiplication of linear map)

$=x \cdot g\left(\left[ \begin{array}{l}{1} \\ {0}\end{array}\right]\right)+y \cdot g\left(\left[ \begin{array}{l}{0} \\ {1}\end{array}\right]\right)$

$=x \cdot \left[ \begin{array}{l}{0} \\ {1}\end{array}\right]+y \cdot \left[ \begin{array}{c}{-1} \\ {0}\end{array}\right]$

$g\left(\left[ \begin{array}{l}{x} \\ {y}\end{array}\right]\right)=\left[ \begin{array}{c}{0 x-1 y} \\ {x+0 y}\end{array}\right]$

$\left[ \begin{array}{cc}{0} & {-1} \\ {1} & {0}\end{array}\right] \cdot \left[ \begin{array}{l}{x} \\ {y}\end{array}\right]$

# Matrix Multiplication as Function Composition 

$H=\left[g\left(f\left(\left[ \begin{array}{l}{1} \\ {0}\end{array}\right]\right) \quad g\left(f\left(\left[ \begin{array}{l}{0} \\ {1}\end{array}\right]\right)\right)\right)\right]$

$H=\left[g\left(F_{c o l 1}\right) \quad g\left(F_{c o l 2}\right)\right]$

$H=\left[G \cdot F_{c o l 1} \quad G \cdot F_{c o l 2}\right]$
<!--stackedit_data:
eyJoaXN0b3J5IjpbNzA0MTY0MTQ4XX0=
-->