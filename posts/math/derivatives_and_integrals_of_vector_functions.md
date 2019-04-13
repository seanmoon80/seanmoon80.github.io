---
title: "Derivatives and Integrals of Vector Functions"
date: 2019-01-25T14:22:59-05:00
---

## Derivatives
$$\begin{align} 
f\prime(x) &= \lim_{\Delta x \to 0}\frac{f(x + \Delta x) - f(x)}{\Delta x} \newline\newline
\vec{r}\prime(t) &= \lim\_{\Delta t \to 0}\frac{\vec{r}(t + \Delta t) - \vec{r}(t)}{\Delta t} \newline
&= \lim\_{\Delta t \to 0}\frac{(f(t + \Delta t)\hat i + g(t + \Delta t)\hat j + h(t + \Delta t)\hat k) - (f(t)\hat i + g(t)\hat j + h(t)\hat k)}{\Delta t} \newline
&= \lim\_{\Delta t \to 0}\frac{f(t + \Delta t) - f(t)}{\Delta t}\hat i + \lim\_{\Delta t \to 0}\frac{g(t + \Delta t) - g(t)}{\Delta t}\hat j + \lim\_{\Delta t \to 0}\frac{h(t + \Delta t) - h(t)}{\Delta t}\hat k \newline
&= f\prime(t)\hat i + g\prime(t)\hat j + h\prime(t)\hat k
\end{align}$$ 

* 접선벡터(Tagent vector) - 접선(Tangent line)의 방향벡터
* 주어진 t에 대한 접선벡터
* 주어진 t에 대한 접선(Tangent Line)
* 접선벡터를 통해 곡선(Curve)의 방향

### Example 1.
{{< geogebra id="qr4v4xxa" width="800" height="600" >}}
$$\begin{align}
&\vec{r}(t) = \left< 4\cos{t}, 2\sin{t} \right>\ 0 \lt t \lt 2\pi \newline\newline
&\text{Find Point of tangency(P.O.T) at } t = \frac{\pi}{3} \newline
&\text{Find Tangent Vector at P.O.T} \newline
&x = 4\cos t \rightarrow \cos t = \frac{x}{4} \newline
&y = 2\sin t \rightarrow \sin t = \frac{x}{2} \newline
&\frac{x^2}{16} + \frac{y^2}{4} = 1 \newline
&\vec{r}(\frac{\pi}{3}) = (4\frac{1}{2})\hat i + (2\frac{\sqrt{3}}{2})\hat j = 2\hat i + \sqrt{3}\hat j \newline
&P.O.T\ (2, \sqrt{3}) \newline\newline
&\vec{r}\prime(t) = \left<-4\sin t, 2\cos t \right> \newline\newline
&\text{Tangent Vector at P.O.T }\newline
&\vec{r}\prime(\frac{\pi}{3}) = \left<-2\sqrt{3}, 1 \right>
\end{align}$$

### Unit Tangent Vectors
$$ \vec{T}(t) = \frac{\vec{r}\prime(t)}{|| \vec{r}\prime(t) ||} $$
$$\begin{align}
\vec{T}(t) &= \frac{-4\sin t\hat i + 2\cos t\hat j}{\sqrt{(-4\sin{t})^2 + (2\cos{t})^2}} \newline
\vec{T}(\frac{\pi}{3}) &= \frac{-2\sqrt{3}\hat i + \hat j}{\sqrt{13}}
\end{align}$$

### Tangent Lines
$$\begin{align}
&\text{Point} = (x\_0,y\_0,z\_0),\ \text{Direction Vector } \vec{v} = \left< a, b, c \right> \newline\newline
&x = x\_0 + at,\ y = y\_0 + bt,\ z = z\_0 + ct \newline\newline
&x = 2 - 2\sqrt{3}t,\ y = \sqrt{3} + t
\end{align}$$

-----------
## Integrals
$$\begin{align}
&\displaystyle\int_0^1(t\hat i + t^2\hat j + t^3\hat k) \, dt \newline
&= \left. \frac{1}{2}t^2\hat i + \frac{1}{3}t^3\hat j + \frac{1}{4}t^4\hat k\ \right|_0^1 \newline
&= \frac{1}{2}(1-0)^2\hat i + \frac{1}{3}(1-0)^3\hat j + \frac{1}{4}(1-0)^4\hat k \newline
&= \frac{1}{2}\hat i + \frac{1}{3}\hat j + \frac{1}{4}\hat k
\end{align}$$

### Indefinite Integral of vector function
$$\begin{align}
&\displaystyle\int (t\hat i + t^2\hat j + t^3\hat k) \, dt \newline
&\displaystyle\int t \, dt = \frac{1}{2}t^2\hat i + C_1\hat i \newline
&\displaystyle\int t^2 \, dt = \frac{1}{3}t^3\hat j + C_2\hat j \newline
&\displaystyle\int t^2 \, dt = \frac{1}{4}t^4\hat k + C_3\hat k \newline
&= \frac{1}{2}t^2\hat i + \frac{1}{3}t^3\hat j + \frac{1}{4}\hat k + \underbrace{C_1\hat i + C_2\hat j + C_3\hat k}\_{C\text{(Constant Vector)}}
\end{align}$$

### Example
$$\begin{align}
&\vec{r}\prime(t) = 2\hat i + 4t\hat j + 6t^2\hat k \newline
&\vec{r}(0) = \hat i + \hat k \newline
&\vec{r}(t) = \int 2\hat i + 4t\hat j + 6t^2\hat k \, dt \newline
&= 2t\hat i + 2t^2\hat j + 2t^3\hat k + C \newline\newline
&\vec{r}(0) = C = \hat i + \hat k
\end{align}$$