
# Exponential 

## Definition 

$$
\exp {(x)} = \sum_{k=0}^\infty \dfrac{x^k}{k!} = 1 + x + \dfrac{x^2}{2!} + + \dfrac{x^3}{3!} + \dotsb
$$

* or Euler number 

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

경제성장율 같은 경우 많아야 10% 정도에 불과하다. 따라서 로그 디퍼런스를 그대로 성장율처럼 써도 되겠다. 
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM3Mjc4NTk0NiwxNDM3MDIwMDA3LDE2ND
E0MDMyNzUsLTExMTQ5NzA5MjksLTIxNDIxMDQwMDMsMTcwNDc2
ODY5MywtODMxMDU2NjUwLDE0NDY0OTc5MzhdfQ==
-->