# Basic 

함수를 다항식으로 근사하는 것 

$$
f(x) = c_0 + c_1 x + c_2 x^2 + c_3 x^3 + \dotsb
$$

- 어느 포인트 주변에서 근사할 것인가? $x=0$

$$
f(0) = c_0 
$$

- $c_1$은 어떻게 구할 것인가? 

$$
f^\prime (x) = c_1 + 2 c_2 x + 3 c_3 x^2 + \dotsb
$$

$$
f^\prime(0) = c_1
$$


Taylor series expansion around $x=0$ is: 

$$
f(x) = f(0) + f^\prime(0) x +  \dfrac{f^{\prime\prime} (0)}{2!} x^2 +  \dfrac{f^{\prime\prime\prime} (0)}{3!} x^3 + \dotsb
$$

Generally around point $a$

$$
f(x) = f(a) + f^\prime(a) (x-a) +  \dfrac{f^{\prime\prime} (a)}{2!} (x-a)^2 + \dfrac{f^{\prime\prime\prime} (a)}{3!} (x-a)^3 + \dotsb
$$

# Taylor Series Expansion for Trigonometry 

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
<br> 
$$
\begin{aligned}
e^{i \cdot x}  & =  1 + i \cdot  x - \dfrac{x^2}{2!}  -  \dfrac{i \cdot x^3}{3!}  +  \dfrac{x^4}{4!}  + \dfrac{i \cdot x^5}{5!} -  \dfrac{x^6}{6!}  -  \dfrac{i \cdot x^7}{7!}  +   \dfrac{x^8}{8!}  + \dotsb \\\\
&= \left( 1- - \dfrac{x^2}{2!} +  \dfrac{x^4}{4!} - \dfrac{x^6}{6!}  +   \dfrac{x^8}{8!}  \right) + 
i \left( x  -  \dfrac{x^3}{3!}  + \dfrac{ x^5}{5!}   -  \dfrac{x^7}{7!}  \right) \\\\
& = \cos x + i \cdot \sin x
\end{aligned}
$$
<!--stackedit_data:
eyJoaXN0b3J5IjpbNjM1NzUxNTgwXX0=
-->