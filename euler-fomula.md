
# Source 

- [https://betterexplained.com/articles/intuitive-understanding-of-eulers-formula/](https://betterexplained.com/articles/intuitive-understanding-of-eulers-formula/)
- [https://betterexplained.com/articles/easy-trig-identities-with-eulers-formula/](https://betterexplained.com/articles/easy-trig-identities-with-eulers-formula/)
- [https://www.dsprelated.com/showarticle/754.php](https://www.dsprelated.com/showarticle/754.php)

# Euler Equation or Formula 

$$
e^{i \theta} = \cos \theta + i \cdot \sin \theta 
$$

# Proof 

## Using taylor series expansion 

$$
\sin x \xrightarrow{\text{derivative}} 
\cos x \xrightarrow{\text{derivative}} 
-\sin x \xrightarrow{\text{derivative}} 
-\cos x \xrightarrow{\text{derivative}} 
\sin x 
$$

With T.S.E. around $x = 0$

$$
\begin{aligned}
\sin x  & = x - \dfrac{x^3}{3!} + \dfrac{x^5}{5!}  - \dotsb \\\\
\cos x & = 1 - \dfrac{x^2}{2!} + \dfrac{x^4}{4!}  - \dotsb \\
\end{aligned}
$$

From the definition of $e^x$

$$
e^x = 1 + x + \dfrac{x^2}{2!} +  \dfrac{x^3}{3!} + \dotsb
$$

$$
\begin{aligned}
e^{i \cdot x}  & =  1 + i \cdot  x - \dfrac{x^2}{2!}  -  \dfrac{i \cdot x^3}{3!}  +  \dfrac{x^4}{4!}  + \dfrac{i \cdot x^5}{5!} -  \dfrac{x^6}{6!}  -  \dfrac{i \cdot x^7}{7!}  +   \dfrac{x^8}{8!}  + \dotsb \\\\
&= \left( 1- - \dfrac{x^2}{2!} +  \dfrac{x^4}{4!} - \dfrac{x^6}{6!}  +   \dfrac{x^8}{8!}  \right) + 
i \left( x  -  \dfrac{x^3}{3!}  + \dfrac{ x^5}{5!}   -  \dfrac{x^7}{7!}  \right) \\\\
& = \cos x + i \cdot \sin x
\end{aligned}
$$

## Visually (really amazing) 

[http://slesinsky.org/brian/misc/eulers_identity.html](http://slesinsky.org/brian/misc/eulers_identity.html)

$e$의 정의를 떠올려보자. 

$$
e^x = \lim_{n \to \infty} \left( 1 + \dfrac{x}{n} \right)^n
$$

$x = x \cdot i$로 두고 이를 기하학적으로 이해하면 아래와 같다. 

![https://raw.githubusercontent.com/anarinsk/public_writing/master/assets/images/iproduct.png](https://raw.githubusercontent.com/anarinsk/public_writing/master/assets/images/iproduct.png)

### Facts 

1. 복소계에서 곱은 두 개의 비슷한 삼각형을 붙여서 그려나가는 형태로 진행된다. 특히 제곱의 경우에는 한변을 공유한 상태에서 앞 삼각형과 비슷한 크기의 삼각형을 계속 붙여나가는 형태다. 
2. $a + b \cdot i$는 복소계 좌표에서 $x$축으로 $a$ 만큼 이동하고 $y$축으로 직각으로 $b$ 만큼 이동하는 형태로 진행된다. 

1의 특별한 경우로 같은 크기의 이등변 삼각형을 계속 붙여 나가는 경우를 생각할 수 있다. 이 경우 복소수 제곱은 단위 원을 벗어나지 않는다. 2의 경우는 직각 삼각형의 이동으로 정식화할 수 있다. 

$$
(1 + \dfrac{\pi \cdot i}{n})^n
$$

을 시각화한다고 생각해보자. $\pi$ 만큼의 라디언을 $n$번 잘라서 계속 붙여 나가게 된다. $\pi$는 복소 좌표계에서 $(-1.0)$에서 끝나게 되니, 반원형태로 생각할 수 있다. 이때 $n \to \infty$를 하면, 접하는 삼각형들의 변의 길이는 동일해지고 fact 1에 따라서 이등변 삼각형이 되므로 원을 벗어나지 않게 된다. 

$$
\lim_{n \to \infty} (1 + \dfrac{\pi \cdot i}{n})^n = e^{\pi \cdot i}
$$

그리고 복소 좌표계에서 해당 제곱은 $(-1,0)$에서 끝나게 된다. 

### A special case 

복소 좌표계에서 $x = \pi \cdot i$는 특별한 가정이다. $x$에 다른 라디언을 넣으면 이는 좌표계에서 $(1,0)$에서 해당 라디언 만큼 움직인 좌표를 나타내게 된다. 즉, $e^{x \cdot i}$는 복소 좌표계의 단위원 위에서의 움직임을 나타내게 된다. 



# Basic 

## Pi 

* Definition: The ratio between the length of circumference and diameter 
* diameter is same as $2 \times$ radius 
* Thus, length of circumference is $2\times r \times \pi$

## Radian 

* radius(반지름)에서 온 말임을 쉽게 알 수 있다. 
* 즉, 특정한 원호의 길이를 반지름으로 나눈 것을 radian이라고 정의한다. 이에 따르면, 
	* 원주가 $2r\pi$이므로, 360도를 나타내는 radian은 $2\pi$가 된다. 
* 따라서 이 관계로부터, 360도의 1/2인 180도는 $pi$, 1/4인 90도는 $\frac{\pi}{2}$등과 같이 정의된다. 
* 360단위로 표기된 각도를 실수로 치환하는 테크닉으로 이해하면 좋겠다. 
* 더구나 360도라는 것은 아무런 베이스가 없는 표기법이다. Radian을 쓰게 될 경우 각도가 실수로 치환되는 장점이 있고, 단위에 의존하지 않게 된다. 

# Euler Identity 

$$
e^{i \pi} = -1
$$

On ciricle, $\cos x + i \sin x$. Thus, $x = \pi$ ,  Euler indenity is derived. 

# Imaginary Growth 

![imaginary growth](https://betterexplained.com/wp-content/uploads/euler/imaginary_growth.png)

- $e^{xi}$, 즉, exponential에서 순수하게 $i$만 갖는 경우는 실수 라인($x$ 축)과 직교한 움직임이라고 볼 수 있다. 
- 그렇다면, $x$가 커지만 커질수록 계속해서 Im 쪽으로 뻗어나가야 하지 않을까? 
	- $x$에 아무리 큰 숫자가 와도 원 주위를 돌 뿐 원을 벗어나지 않는다! 
- 직관적으로 이해해보자. 

# Some Properties of Imaginary 

## The unit circle 

* 실수와 허수를 각기 cartesian space에 $x$, $y$ 축에 두자. 그러면, 

$$
\vert a + b \cdot i \vert = \sqrt{a^2 + b^2}
$$

이 값으로 허수를 나누면 모든 허수의 길이는 $\sqrt{a^2 + b^2}$ 단위원 안에 들어온다.

## Powers 

### Integers 

$i^0 = 1$, $i^1 = i$, $i^2 = -1$

단위 원 주위를 돌게 된다는 점을 쉽게 알 수 있다. 

## Fractional 

$i^{1/2}$을 생각해보자. 일단 $i^{1/2} = a + b\cdot i$ 라고 가정해보자. 양변을 제곱하고 문제를 풀면, 

$$
\left( a, b \right) = \left( \dfrac{\sqrt{2}}{2}, \dfrac{\sqrt{2}}{2} \right)~\text{or}~\left( -\dfrac{\sqrt{2}}{2}, -\dfrac{\sqrt{2}}{2} \right)
$$

심심하면, $z^3 = 1$을 풀어보기 바란다. 

## Exponential behavior 

$i$의 승수의 경우 고유값을 갖지 않고 순환하는 특성을 지니고 있다. 

$$
z = i^p = i(p + 4\cdot n)
$$

이는 $i$ 축을 가진 허수계가 단위 원에서 돌아가는 이유이기도 하다. 즉, 어떤 $z$라도 임의의 fraction을 곱해서 얻을 수 있으며, 녀석은 항상 단위원 위에 있게 된다. 
더불어 곱이 합으로 처리되는 특징을 지니고 있다. 즉, 

$$
z_1 z_2 = i^{p_1} i^{p_2} = i^{p_1 + p_2} = z_3
$$

이 특성 때문에 단위에 종속되지 않는다. 즉, radian을 하나 잡고 이를 fractional power를 통해서 적당히 돌리면 해당 위치를 찾을 수 있는 것이다. 

## Radian scale 

- 1 radian, 단위원 위에서는 그냥 그대로 1의 각을 $u$라고 하자. 이 경우, 

$$
u = \cos (1) + i \cdot \sin (1) 
$$

앞서 본 것처럼 파워 스케일이 몇 개의 radian을 가졌는지와 일치하므로, 

$$
u^{\theta} =  \cos \theta + i \cdot \sin \theta
$$ 

그런데, 식의 우변은 Euler formula의 우변과 같다. 따라서, 

$$
u^{\theta} = e^{i \cdot \theta} = \left( e^i \right)^\theta
$$

즉, 오일러 방정식은 복소 공간의 어떤 점을 단위 원 둘레의 어떤 위치로 옮기는 역할을 한다. 이 경우 고려해야 하는 변수는 2개에서 1개로 줄어든다. 





<!--stackedit_data:
eyJoaXN0b3J5IjpbMTg1ODQwOTMwNiwtNjg3OTY4MTEzLC0xMz
Y0NjQ3ODkyLC0xMDgxMjYwNDE0LC0xNjkyNjAxNTI2XX0=
-->