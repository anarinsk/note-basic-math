

![](https://betterexplained.com/wp-content/uploads/2018/08/imaginary-multiplication-exponents.png)

# 복수 좌표계에서 움직임 

## 허수의 곱 

허수를 곱한다는 것은 복소 좌표계에서 축을 한번에 옮기는 것이다. 왼쪽 그림처럼 $1$과 $i \cdot 1$을 생각해보면 된다. 

## $e^{x \cdot i}$ 

그렇다면, exponential에서 허수의 승수는 어떻게 기하학적으로 이해할 수 있을까? 허수를 승수로 곱하면 어떻게 될까? $e$의 정의로 돌아가보는 게 좋다. 

$$
e^{xi} = \lim_{n \to \infty} \left( 1 + \dfrac{x}{n} i \right)^n
$$

$(1+\frac{1}{n}i)$는 실수계로 1만큼 그리고 허수계로 즉, 90도의 각도로 방향을 틀어 $1/n$만큼 이동한다는 의미다. 이제 $(1+\frac{1}{n}i)^2$은 무엇인가? 한번 이동한 상태에서 제곱이다. 사실상 허수의 곱과 같다. 90도 만큼 $1/n$ 만큼 이동하는 것을 의미한다. 그리고 $e^{ix}$의 정의를 보면, 1의 길이를 유지한 상태에서 $x$ 라디언 만큼 회전하는 것을 의미한다. 

![](https://betterexplained.com/wp-content/uploads/math-analogies/math-analogies-jpg.022.jpeg)

### More understanding 

$(1+\dfrac{i}{100})^{2}$ 따져보자. 

1. $(1+\dfrac{i}{100})$는 실수축으로 1, 허수축으로 $\frac{1}{100}$으로 이동한다. 
2. $(1+\dfrac{i}{100})(1+\dfrac{i}{100})$을 계산해보자. 

$$
1+\dfrac{2}{100}i -(\dfrac{1}{100})^{2} \approx 1+\dfrac{1}{50}i
$$

해당 삼각형의 등변의 길이를 구하면, 

$$
\sqrt{1^2 + (\dfrac{1}{50})^2} \approx 1
$$

$$
\lim_{n \to \infty} \sqrt{1^2 + (\dfrac{1}{n})^2} = 1
$$

NOT PROPERLY ENDED

## Examples

### Case $2^i$

$$
2^i = e^{\ln (2) \cdot i}
$$

$$
2^i = \cos 0.693 + i \cdot \sin 0.693 = .769 + .639 \cdot i
$$

### Case $i^i$

$i = e^{\frac{\pi}{2}\cdot i}$. 즉, $e^{x \cdot i}$의 특징에서 따라서 $x =\frac{\pi}{2}$로 원주 위에서 돌릴 수 있다.  

$$
i^i = \left[ e^{\frac{\pi}{2}\cdot i} \right]^i =  e^{\frac{\pi}{2}\cdot i \cdot i} = e^{-\frac{\pi}{2}}  = 0.207\dotsc
$$

흥미롭게도 그냥 실수가 되버린다. 

### Case $i \cdot i^i$

앞서 보았던 것처럼, $i$를 곱하면 축을 이동시키게 된다. 즉, 허수 축의 $(0, 0.207i)$로 옮겨가게 된다. 


### Velocity of $f(x) = e^{i x}$

$$
f^\prime (x) = \dfrac{d}{d x} e^{ix} = i e^{ix} = i \cdot f(x)
$$

즉, 현재의 포지션에서 직각의 가속도($i$)로 움직이게 된다. 



<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQyNTQ3OTEzLC02MDQxNTEzNjEsMTU1Mj
A1NzA2LDI5MzA0MDcwOSw4NzcwNDgwOTQsLTYyMDEwOTI0OCw2
MzI4MjA5MzYsMjA1OTkyMTU2MSwtMTQ1NjIzNTcwNSwxNjg0OT
g5NjE0LC02NDg3NjA2MTJdfQ==
-->