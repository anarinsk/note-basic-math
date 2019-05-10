
# Exponential 

## Definition 

$$
\exp {(x)} = \sum_{k=0}^\infty = 1 + x + \dfrac{x^2}{2!} + + \dfrac{x^3}{3!} + \dotsb
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
\dfrac{d}{dx}\ln (x) & = \lim_{h \to 0} \dfrac{\ln (x+h) - \ln (x)}{h} \\ \\
&=  \lim_{h \to 0} \dfrac{1}{h} \ln \left( 1+\frac{h}{x} \right) \\ \\
& =  \lim_{h \to 0} \ln 
\left( 1+\frac{h}{x} \right)^{\frac{1}{h}} \\ \\
& =  \lim_{h \to 0} \ln \left( 1+\frac{1}{t} \right)^{\frac{t}{x}} \\ \\
& = \dfrac{1}{x} \ln \left( \lim_{t \to 0} \left( 1+\frac{1}{t} \right)^t \right) \\ \\
& = \dfrac{1}{x} \ln (e) \\ \\
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

자연로그 값의 차이를 어떻게 이해해야 하는가? 

Let $x_t$, $x_{t+1}$ be money values of two consecutive times. Return can be written by 

$$
\dfrac{x_{t+1} - x_t}{x_t}  = r
$$

$$
x_{t+1} = (1+r) x_t
$$

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQ4NjE3NDg0MSwxNDQ2NDk3OTM4XX0=
-->