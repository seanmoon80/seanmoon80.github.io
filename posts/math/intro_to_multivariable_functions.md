---
title: "Intro to Multivariable Functions"
date: 2019-02-20T13:54:16-05:00
---

* You must have 1 dimension more than the number of independent variables.(Number of independent variables + 1)  
    * $f(x) = x + 1 \rightarrow y = x + 1 \rightarrow \text{2-D}$  
    * $g(x,y) = x^2 + y^2 \rightarrow z = x^2 + y^2 \rightarrow \text{3-D}$  
    * $h(x,y,z) = \frac{x^2 + y^2}{z - 3} \rightarrow w = \frac{x^2 + y^2}{z - 3}$
* You must have the same dimension as number of independent variables.
    * $f(x) = x + 1 \rightarrow y = x + 1 \rightarrow \text{1-D}$  
    * $g(x,y) = x^2 + y^2 \rightarrow z = x^2 + y^2 \rightarrow \text{2-D}$  
    * $h(x,y,z) = \frac{x^2 + y^2}{z - 3} \rightarrow w = \frac{x^2 + y^2}{z - 3} \rightarrow \text{3-D}$

### Example 1
$$\begin{align}
f(x, y, z) &= \sqrt{x^2 + 2y^2 + 3z^2} \newline
f(0, 2, -1) &= \sqrt{0^2 + 2\cdot2^2 + 3\cdot(-1)^2} = \sqrt{11} \newline
f(u, u-1, u+1) &= \sqrt{u^2 + 2(u-1)^2 + 3(u+1)^2} \newline
&= \sqrt{u^2 + 2u^2 - 4u + 2 + 3u^2 + 6u + 3} \newline
&= \sqrt{6u^2 + 2u + 5}
\end{align}$$

### Example 2
$$\begin{align}
&f(x,y) = \frac{xy}{x-y} \rightarrow x - y \neq 0 \newline
&Domain: \\{ (x,y)\ |\ x \neq y \\} \newline
&Range: \\{ z\ |\ -\infty \lt z \lt \infty \\}
\end{align}$$

### Example 3
$$\begin{align}
&g(x, y) = \sqrt{4 - x^2 - y^2} \newline
&Domain: \\{ (x,y)\ |\ 0 \le x^2 + y^2 \le 4 \\} \newline
&Range: \\{ z\ |\ 0 \le z \le 2 \\}
\end{align}$$

* To graph domain, You must have an Axis for each Independent variable  

### Example 4
$$\begin{align}
&f(x, y) = \frac{xy}{x^2 - y^2} \newline
&Domain: \\{ (x, y)\ |\ y \ne \pm x \\}
\end{align}$$

### Example 5
$$\begin{align}
&f(x, y, z) = \sqrt{9-x^2-y^2-z^2} \newline
&Domain: \\{ (x,y,z)\ |\ x^2+y^2+z^2 \le 9 \\}
\end{align}$$

### Example 6
$$\begin{align}
&f(x,y,z) = \frac{\sqrt{4 - x^2 - y^2}}{z - 3} \newline
&Domain: \\{ (x,y,z)\ |\ x^2 + y^2 \le 4,\ z \ne 3 \\}
\end{align}$$

## Level Curves
The shape we get when a plane intersects our surface at different levels along the axis of the dependent variable  
A map of level curves is a contour plot  
To find level curves Set $f = "k"$

### Exmaple 1
$$\begin{align}
f(x,y) &= \sqrt{16 - x^2 - y^2} \newline
k &= \sqrt{16 - x^2 - y^2} \newline
k^2 &= 16 - x^2 - y^2 \newline
x^2 + y^2 &= 16 - k^2 \newline
\end{align}$$