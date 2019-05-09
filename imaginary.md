
# Multiplication vs. Exponents 


![](https://betterexplained.com/wp-content/uploads/2018/08/imaginary-multiplication-exponents.png)

곱은 축을 옮기는 것이다. 그림처럼 $1$과 $\cdot 1$을 생각해보면 된다. 지수화는 벡터의 방향을 $\frac{\pi}{2}$만큼 트는 것을 의미한다. 이는 현재의 방향에서  $\frac{\pi}{2}$ 회전이다. 

## 72 Rules 

- 1이 있다고 하자. 여기에 적정한 수를 곱하면 되니, 단위 수로 나쁘지 않다. 
- 녀석이 2가 되어야 한다. 즉 두 배가 된다. 
- 복리(compound rate)로 어느 정도의 성장률이 필요한가? 

$$
\begin{aligned}
2 &= e^{x}\\\\
\ln 2 &= \ln e^{x} = x
\end{aligned}
$$

즉, $x = \ln 2 = 0.693$이다. 만일 성장률을 백분률로 나타낸다면, $100 x = 69.3$. 그리고 $e$의 특성상  $100x = rt$로 분리할 수 있다. 즉, $r$은 백분율로 나타낸 연간 성장률이고 $t$는 연차를 나타낸다. 즉, 어떤 상태가 두 개가 되기 위해 필요한 연간 성장률 및 연차를 나타낸다. 그런데, 69.3이라는 숫자는 구구단에 등장하지 않는다. 구구단에 등장하는 가장 가까운 숫자가 72이다. 그래서 72의 법칙이라고 불린다. 

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
eyJoaXN0b3J5IjpbMjA1OTkyMTU2MSwtMTQ1NjIzNTcwNSwxNj
g0OTg5NjE0LC02NDg3NjA2MTJdfQ==
-->