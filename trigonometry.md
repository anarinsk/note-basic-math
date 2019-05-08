
# Source 

* Hack trigonometry
[https://betterexplained.com/articles/intuitive-trigonometry/](https://betterexplained.com/articles/intuitive-trigonometry/)

* Binary operation on trigonometry 
[https://betterexplained.com/articles/easy-trig-identities-with-eulers-formula/](https://betterexplained.com/articles/easy-trig-identities-with-eulers-formula/) 

* Derivatives of trigonometry 
[https://betterexplained.com/articles/easy-trig-identities-with-eulers-formula/](https://betterexplained.com/articles/easy-trig-identities-with-eulers-formula/) 


# Hack Trig 

- 그냥 대단하다! 이렇게 외울 걸... 
![Trig all functions in a single diagram](https://betterexplained.com/wp-content/uploads/trig/trig-overall.png)
<br>
![Trig identities from similar triangles and pythagorean theorem](https://betterexplained.com/wp-content/uploads/trig/trig-identities.png)


## Origin of word tagent 

![Tangent](https://betterexplained.com/wp-content/uploads/trig/tangent.png)

- 파란색 기준의 $\tan \theta$와 빨간색 기준의 $\tan \theta$는 동일하다. 
- 따라서 녹색선의 길이는 같다. 
- 적색과 녹색은 서로 직교(orthogonal)함으로 녹색선은 원에 접해야 한다. 


# Binary Operation of Trigonometry 

![euler's formula multiplication](https://betterexplained.com/wp-content/uploads/trig/euler-trig-1.png?t=2)

## Derivation 

위 그림에서 $a$ 라디언 만큼 움직인 것과 $b$ 라디언 만큼 움직인 것을 더한 즉, $(a+b)$ 라디언 만큼 움직인 것의 삼각함수 값을 나타내보자. 

$$
e^{i \cdot (a+b)} = cos(a+b) + i \cdot sin(a+b)
$$

also, 

$$
\begin{aligned}
e^{i \cdot (a+b)} & = e^{i \cdot a} e^{i \cdot b} \\\\
 & = (\cos a + i \cdot \sin a)(\cos b + i \cdot \sin b)
 & = (\cos a \cos b - \sin a \sin b) + i \cdot (\cos a \sin b + \cos b \sin a) 
\end{aligned}
$$

![sine addition formula combined height](https://betterexplained.com/wp-content/uploads/trig/combined-height-1.png)
![cosine addition formula combined width](https://betterexplained.com/wp-content/uploads/trig/combined-width-1.png)

그림에서 보는 것처럼, $a+b$ 라디언의 높이는 $\sin (a+b)$를 정의하고 이는 허수계이다. 앞의 식에서 

$$
\sin (a+b) = \cos a \sin b + \cos b \sin a
$$

그리고 실수계의 정의에 따라서 

$$
\cos (a+b) = \cos a \cos b - \sin a \sin b
$$

이를 재미있게 해석해볼 수 있다. 그림에서 보듯이, 각각의 높이는 각각의 삼각형대로 반영되지 않고 그에 가중치를 곱해지는 형태로 반영된다. 

# Derivative of Trigonometry 

## Approximation for small radian 

![](https://betterexplained.com/wp-content/uploads/trig/add-small-angles.png)

만일 합해지는 두 각이 아주 작다고 해보자. 이 경우 각각 움직이는 각이 크지 않으므로 사실상 각을 이루는 선분의 길이가 얼추 비슷할 것이다. 따라서, $\cos a, \cos b \approx 1$이 성립한다. 즉, 

$\sin (a+b) \approx \sin a + \sin b$

그리고 $a$, $b$가 이미 라디언값이기 때문에 $\sin x \approx x$가 성립함으로 

$\sin (a+b) \approx a + b$

## Derivative of $\sin$

이제 이 사실은 $\sin x$의 도함수를 도출하는 데 활용해보자. 

$$
\begin{aligned} 
\dfrac{d (\sin x)}{ dx} & =  \lim_{dx \to 0}  \dfrac{\sin (x + dx) - \sin x}{dx}  \\\\
& =  \lim_{dx \to 0}  \dfrac{\sin x \cos dx + \sin dx \cos x - \sin x}{dx} \\\\
& =  \lim_{dx \to 0}  \dfrac{\sin x \cdot 1 + \sin dx \cos x - \sin x}{dx} \\\\
& =  \lim_{dx \to 0}  \dfrac{\sin dx \cos x }{dx} \\
& =  \lim_{dx \to 0}  \dfrac{dx \cdot \cos x }{dx} \\
& = \cos x
\end{aligned}
$$

$\cos x$의 미분도 같은 방식으로 구현해보자. 

$$
\dfrac{d (\cos x)}{dx} = -\sin x
$$ 

# Some Practices 

$$
\sin (a-b) = \cos a \sin (-b) + \cos(-b) \sin a
$$

$$
\sin (2a) = \sin (a+a) = \cos a \sin a + \cos a \sin a = 2 \cos a \sin a 
$$

# Why radian 

[https://betterexplained.com/articles/intuitive-guide-to-angles-degrees-and-radians/](https://betterexplained.com/articles/intuitive-guide-to-angles-degrees-and-radians/)

각도는 사실 이상한 표기법이다. 

- 360도의 근거는 무엇인가? (1년을 빗대서 365일에서 온 단위) 
- 그리고 일종의 절대 단위다. 

각도를 상대화해서 실수로 만들 수는 없을까? 
- $\pi$에 착안하자. 즉, $\pi$란 원주와 지름(diameter)의 일정한 비율을 나



<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEyMjMwODQwNDksLTEwMTU3MzExNjUsLT
YzMTY3ODI2NF19
-->