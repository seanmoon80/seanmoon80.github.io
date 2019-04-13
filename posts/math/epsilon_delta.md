---
title: "Epsilon Delta"
date: 2018-12-29T16:58:16-05:00
---

## Epsilon-delta definition
$\lim_{x\to{a}}f(x) = L$

x가 a에 한없이 가까워질때 함수 f(x)는 L에 수렴한다.
한없이 가까이? 얼마만큼이 한없이 가깝지? 

$x$에 대한 함수 $f(x)$가 있을때,  
임의의 양수 $\epsilon$에 적당한 양수 $\delta$가 존재하여 $0 < |x - a| < \delta$이면 $|f(x) - L| < \epsilon$이 될때  
$x \rightarrow a$일때 함수 $f(x)$의 극한값을 L이라고 정의한다.  이때, 함수 $f(x)$는 $x \rightarrow a$에서 L에 수렴한다고 하며  
$\lim_{x\to{a}}f(x) = L$이라고 한다.


![alt text](https://ds055uzetaobb.cloudfront.net/image_optimizer/ff3edcfc564cc64e74e090606aa07b35aef6660a.png "Epsilon-delta geometric")

## Example
1. $\lim_{x\to{-2}}2x+1 = -3$  

$$\begin{align}|x - a| < \delta &= |x -(-2)| < \delta$ \newline
&= |x + 2| < \delta
\end{align}$$
  
$$\begin{align}|f(x) - L| < \epsilon &= |2x + 1 -(-3)| < \epsilon \newline
&= |2x + 4| < \epsilon \newline
&= |2||x + 2| < \epsilon \newline
&= |x + 2| < \frac{\epsilon}{2}
\end{align}$$

$$|x+2| < \frac{\epsilon}{2}, \delta = \frac{\epsilon}{2}$$

2. $\lim_{x\to{2}}x^2 + x - 2 = 4$

$$\begin{align}|f(x) - L| < \epsilon &= |(x^2 + x - 2) - 4| < \epsilon \newline
&= |(x^2 + x - 6)| < \epsilon \newline
&= |(x + 3)(x - 2)| < \epsilon \newline
&= |x + 3||x - 2| < \epsilon \newline
&= |x - 2| < \frac{\epsilon}{|x + 3|}
\end{align}$$
**NOTE: In general $\delta$ must be in terms of $\epsilon$ only without any extra variables.**
We know that $x$ is close to a. So, let's say $|x - a| < 1$. Then, this means, $1 < x < 3, \text{or}\ 4 < x+3 < 6$
To get minimum, $x + 3\ \text{is}\ 6$
$$|x - 2| < \frac{\epsilon}{x + 3} < \frac{\epsilon}{6}$$
$$|x - 2| < 1\ \text{and}\ |x-2| < \frac{\epsilon}{6}$$
Given $\epsilon$, let $\delta = min\\{1, \frac{\epsilon}{6}\\}$  

$\delta = 1,\ 1 < \frac{\epsilon}{6} \implies \epsilon > 6$
$$\begin{align} |x - a| < \delta &= |x - 2| < 1 \newline
&= |x - 2||x + 3| < |x + 3| \newline
&= |x^2 + x - 6| < |x + 3| \newline
&= |x^2+x-6| < |x+3| < 6 < \epsilon \newline
&= |(x^2+x-2)-4| < \epsilon \newline
&= |f(x)-L| < \epsilon\end{align}$$

$\delta = \frac{\epsilon}{6}$
$$\begin{align}|x - 2| < \frac{\epsilon}{6} &= |x-2||x+3| < 6\frac{\epsilon}{6} \newline
&= |x^2 + x - 6| < \epsilon \newline
&= |(x^2 + x - 2) - 4| < \epsilon \newline
&= |f(x) - L| < \epsilon\end{align}$$

### Infinity
$$\lim_{x\to\infty}\sqrt{x} = \infty$$  
$|f(x) - \infty| = \infty$  
$|x - \infty| = \infty$  

1. 극한값이 무한대인 경우  
임의의 M > 0 에 대해, $0 < |x - c| < \delta$이며 f(x) > M을 만족하는 $\delta > 0$이 존재하면 $\lim_{x\to{c}}f(x) = \infty$로 정의한다.
2. x가 무한대로 가는경우  
임의의 $\epsilon > 0$에 대해 x > N이면 $|f(x) - L| < \epsilon$을 만족하는 N > 0이 존재하면 $\lim_{x\to\infty}f(x) = L$로 정의한다.
$$\begin{align} x > N &\implies f(x) > M \newline
f(x) > M &= \sqrt{x} > M \newline
&= x > M^2 \newline
x > N &= x > M^2 \newline &= \sqrt{x} > M \newline
&= f(x) > M\end{align}$$
