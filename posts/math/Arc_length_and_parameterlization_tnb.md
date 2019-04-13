---
title: "Arc Length and Parameterlization"
date: 2019-01-30T22:19:46-05:00
draft: true
---

## Arc Length
$$\begin{align}
L = \int_a^b \sqrt{(f'(t))^2 + (g'(t))^2}\, dt
\end{align}$$

* [Lectur 5.4](https://www.youtube.com/watch?v=5Yuw1jCBq-0&list=PLF797E961509B4EB5&index=32)  
* [Reference](http://tutorial.math.lamar.edu/Classes/CalcII/ArcLength.aspx)  
* Stewart Calculus 7th Edition Chapter 10.2(P645)

### For 3-D
$$\begin{align}
L &= \int_a^b \sqrt{(f'(t))^2 + (g'(t))^2 + (h'(t))^2}\, dt \newline\newline
\vec{r}(t) &= f(t)\hat i + g(t)\hat j + h(t)\hat k \newline\newline
\vec{r}'(t) &= f'(t)\hat i + g'(t)\hat j + h'(t)\hat k \newline\newline
\|\vec{r}'(t)\| &= \sqrt{(f'(t))^2 + (g'(t))^2 + (h'(t))^2} \newline\newline
L &= \int_a^b \|\vec{r}'(t)\|\, dt
\end{align}$$  

* This formula will give one of two things.  
* Actual arc length(definite integral) when $t \in [a, b]$ We call it 'L'  
* Arc length function(indefinite integral). Still has 't'. We call it $S(t)$

### Example 1
$$\begin{align}
\text{Find Arc Length }: \vec{r}(t) &= 4\sin{t}\hat i + 3t\hat j + 4\cos{t}\hat k\ (0 \le t \le 2\pi) \newline
\vec{r'}(t) &= 4\cos{t}\hat i + 3\hat j - 4\sin{t}\hat k \newline
||\vec{r'}(t)|| &= \sqrt{16\cos^2{t} + 9 + 16\sin^2{t}} \newline
&= \sqrt{16(\cos^2{t} + \sin^2{t}) + 9} = 5 \newline
L &= \int_0^{2\pi}5\, dt = 10\pi \newline\newline
\end{align}$$

#### Arc Length Function
* Replace 't' to 'u'(u-sub)
* Set interval from start point of 't' and to 't'
$$\begin{align}
S(t) &= \int_0^t 5\, du = \left| 5u \right|_0^t = 5t \newline
t &= \frac{S}{5} \newline
\end{align}$$

#### Reparameterize
* Replate 't' in vector function to arc length function
$$\begin{align}
\vec{r}(s) &= 4\sin{\frac{s}{5}}\hat i + 3{\frac{s}{5}}\hat j + 4\cos{\frac{s}{5}}\hat k
\end{align}$$
1. can walk through the curve.
2. could simplify the formular.
3. Easy to get Unit Tangent Vector

{{< geogebra id="wem2skrd" width="800" height="600" >}}