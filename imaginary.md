

![](https://betterexplained.com/wp-content/uploads/2018/08/imaginary-multiplication-exponents.png)

# 복수 좌표계에서 움직임 

## 허수의 곱 

허수를 곱한다는 것은 복소 좌표계에서 축을 한번에 옮기는 것이다. 왼쪽 그림처럼 $1$과 $i \cdot 1$을 생각해보면 된다. 

## $e^{x \cdot i}$ 

그렇다면, exponential에서 허수의 승수는 어떻게 기하학적으로 이해할 수 있을까? 허수를 승수로 곱하면 어떻게 될까? $e$의 정의로 돌아가보는 게 좋다. 

$$
e = \lim_{n \to \infty} \left( 1 + \dfra\right)
$$

![](https://betterexplained.com/wp-content/uploads/math-analogies/math-analogies-jpg.022.jpeg)


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
eyJoaXN0b3J5IjpbLTk0NzU3MjQwNiw4NzcwNDgwOTQsLTYyMD
EwOTI0OCw2MzI4MjA5MzYsMjA1OTkyMTU2MSwtMTQ1NjIzNTcw
NSwxNjg0OTg5NjE0LC02NDg3NjA2MTJdfQ==
-->