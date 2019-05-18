
# Exponential 

## Definition 

$$
\begin{aligned}
\exp {(x)} & = \lim_{n \to \infty} \left( 1 + \dfrac{1}{n} \right)^n \\ 
& =\sum_{k=0}^\infty \dfrac{x^k}{k!} = 1 + x + \dfrac{x^2}{2!} + + \dfrac{x^3}{3!} + \dotsb
\end{aligned}
$$



* Also called Euler number 
* Expand limit expression:

$$
{n\choose 0} \dfrac{}{}
$$

## Narrative 

$$
\lim_{n \to \infty} (1 + \dfrac{1}{n})^n
$$

* 1의 이자율(100%)를 단위 기간 내에 무한번 컴파운딩(복리) 지급, 이라고 이해할 수 있다. 
	+ continuously compounded interest 

## rate of $x$

* 만일 이자율이 $x \times 100$ rate 라면? 

$$
\lim_{n \to \infty} (1 + \dfrac{x}{n})^n
$$

### Derivation 

$$
\begin{aligned}
\lim_{n \to \infty} (1 + \dfrac{x}{n})^n   & = \lim_{n \to \infty} \left( (1 + \dfrac{1}{n/x})^{n/x} \right)^x \\\\
& = \lim_{n \to \infty} \left( ( 1 + \dfrac{1}{t})^t \right)^x, ~\text{where $t \equiv n/x$} \\\\
& = \left( \lim_{t \to \infty} ( 1 + \dfrac{1}{t})^t \right)^x \\\\
& =  e ^x
\end{aligned}
$$

## Derivative 

$$
\begin{aligned}
\dfrac{d}{dx}\ln (x) & = \lim_{h \to 0} \dfrac{\ln (x+h) - \ln (x)}{h} \\\\
&=  \lim_{h \to 0} \dfrac{1}{h} \ln \left( 1+\frac{h}{x} \right) \\\\
& =  \lim_{h \to 0} \ln 
\left( 1+\frac{h}{x} \right)^{\frac{1}{h}} \\\\
& =  \lim_{h \to 0} \ln \left( 1+\frac{1}{t} \right)^{\frac{t}{x}} \\\\
& = \dfrac{1}{x} \ln \left( \lim_{t \to 0} \left( 1+\frac{1}{t} \right)^t \right) \\\\
& = \dfrac{1}{x} \ln (e) \\\\
& = \dfrac{1}{x}
\end{aligned}
$$

### Application 

$$
\dfrac{d}{dx}\log_a (x) = \dfrac{\ln (x)}{\ln (a)} = \dfrac{1}{\ln (a)} \cdot \ln (x) = \dfrac{1}{\ln (a) x}
$$

### Exponential 

#### First 

$$
\dfrac{d}{dx}\ln (e^x) = \dfrac{x}{dx} x = 1 
$$

#### Second 

$$
\dfrac{d}{dx}\ln (e^x) = \dfrac{1}{e^x}\left( \dfrac{d}{dx} e^x \right)
$$

Thus, 

$$
\dfrac{1}{e^x}\left( \dfrac{d}{dx} e^x \right) = 1
$$

$$
\dfrac{d}{dx} e^x = e^x
$$

# Log Difference 

두 자연로그 값의 차분을 어떻게 이해해야 하는가? 

Let $x_t$, $x_{t+1}$ be money values of two consecutive times. Return can be written by 

$$
\dfrac{x_{t+1} - x_t}{x_t}  = r
$$

$$
\begin{aligned}
x_{t+1} & = (1+r) x_t \\\\
\ln x_{t+1} &= \ln(1+r) + \ln x_t \\\\
\ln x_{t+1} - \ln x_t &= \ln(1+r) \\\\
\Delta \ln x_{t+1} & \approx r ~ \text{for $r$ is small}.
\end{aligned}
$$

왜 $\ln$이어야 하는가? $r=0$ 주위에서 TSE을 구해보자. 

$$
\ln (1+r) = \ln 1 + \dfrac{1}{1+r}|_{r=0} (r-0)  + \dotsb \approx r
$$

왜 $e$를 밑수로 써야 하는가? 10을 쓰면 안되나? 그렇다면, $\log_{10} (1+r)$을 $r$에 대해서 미분해보자. 우리가 아는 위의 로그 미분 결과는 자연 로그에만 해당함을 상기하자! 

$$
\frac{d}{dr} \log_{10} (1+r) = \dfrac{1}{\ln 10}\cdot \dfrac{1}{(1+r)} 
$$

즉, $r$ 텀에 들어가는 계수가 1이 아니라 $\frac{1}{\ln 10}$이 곱해진다. $\ln$이 왜 중요한지 다시 기억하기 바란다! 

경제성장율 같은 경우 많아야 10% 정도에 불과하다. 따라서 로그 디퍼런스를 그대로 성장율처럼 써도 되겠다. 게다가, $\ln (1+x) \leq x$가 성립한다. 즉 오차가 크게 나는 경우에도 값을 과장하게 되지는 않는다. 

# 72 Rules 

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
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIxMDI2MzY0MDksMzgwNTI2ODgwLC0xOT
MxODI2NTg0LDE0MzcwMjAwMDcsMTY0MTQwMzI3NSwtMTExNDk3
MDkyOSwtMjE0MjEwNDAwMywxNzA0NzY4NjkzLC04MzEwNTY2NT
AsMTQ0NjQ5NzkzOF19
-->