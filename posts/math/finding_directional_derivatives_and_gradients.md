---
title: "Finding Directional Derivatives And Gradients"
date: 2019-03-29T21:28:27-04:00
---

Graph https://www.geogebra.org/m/gwajt8rk

## Directional Derivatives
* To give a direction, There must be a _Vector_(Unit Vector $\vec u$) on the   
  Plane of the _Independent Variables_.  
* Need Point "P" on _XY-Plane_ for specific _Rate Of Change_  
* Make line through "P" parallel to $\vec u$  
* Create a plane parallel to $\vec u$z-plane  
* Move $\Delta x$ and $\Delta y$ to 0  
* $\vec{PQ}$ parallel $\vec u \rightarrow \vec{PQ} = h\cdot\vec u \rightarrow h\cdot(u_1\hat i + u_2\hat j)$  
* $\vec{PQ} = \Delta x\hat i + \Delta y\hat j = hu_1\hat i + hu_2\hat j \rightarrow \Delta x = hu_1,\ \Delta y = hu_2$  

$$\begin{align}
&\lim_{h \to 0}\frac{f(x + hu_1, y + hu_2) - f(x,y)}{\sqrt{h^2u_1^2 + h^2u_2^2} \rightarrow h\sqrt{u_1^2 + u_2^2}} \newline
D\_\vec{u}f(x,y) &= \lim\_{h \to 0}\frac{f(x + hu\_1, y + hu\_2) - f(x,y)}{h} \newline
D\_\vec{u}f(x,y) &= f\_x\cdot u\_1 + f\_y\cdot u\_2
\end{align}$$

### Example 1
$$\begin{align}
f(x,y) &= x^3 - 2x^2 + y^3, \text{Point(1,2)}, \text{Vector } \theta = \frac{\pi}{6} \newline
\vec u &= \cos\theta\hat i + \sin\theta\hat j = \cos\frac{\pi}{6}\hat i + \sin\frac{\pi}{6}\hat j = \frac{\sqrt{3}}{2}\hat i + \frac{1}{2}\hat j \newline
f_x &= 3x^2-4x, f_y = 3y^2 \newline
D\_\vec{u}f(x,y) &= (3x^2-4x)\frac{\sqrt{3}}{2} + 3y^2\cdot\frac{1}{2} \newline
D\_\vec{u}f(1,2) &= -\frac{\sqrt{3}}{2} + 6 
\end{align}$$
It is slope of tangent line to the surface(f(x,y)) at the point "P" in the direction "u"

## Gradient
$$\begin{align}
D\_\vec{u}f(x,y) &= f\_x\cdot u\_1 + f\_y\cdot u\_2 \newline
&= (f\_x\hat i + f\_y\hat j)\cdot(u\_1\hat i + u\_2\hat j) \newline
f\_x\hat i + f\_y\hat j &\rightarrow \text{Gradient} \newline
\nabla f(x,y) &= f\_x\hat i + f\_y\hat j \newline
D\_\vec{u}f(x,y) &= \nabla f(x,y) \cdot \vec u
\end{align}$$

* $D\_\vec u$ is a _SLOPE_, A _SCALAR_ not a vector  
* $\nabla f$ is A _VECTOR_(Part of $D\_\vec u$)  
* $\nabla f$ relates to the "Grade" of the surface  
* If $\nabla f = \vec 0$, then $D\_\vec u f = 0$ for any point
* $D\_\vec u f(x,y)$ Has its _MAX_ value of $||\nabla f(x,y)||$ when $\vec u || C\cdot\nabla f$ 'C' is a Scalar

$$\begin{align}
D\_\vec u f(x,y) &= \nabla f\cdot\vec u = |\nabla f|\cdot|\vec u|\cdot\cos\theta = |\nabla f|\cdot\cos\theta \newline
&1 \le \cos\theta \le -1
\begin{cases}
\cos\theta = 1, \theta = 0 \newline
\cos\theta = -1, \theta = {\pi} \newline
\end{cases} \newline
\theta \le 1 &\rightarrow D\_\vec u\ \text{Becomes less steep} \newline
\theta = 0 &\rightarrow D\_\vec u f(x,y) = -|\nabla f(x,y)|
\end{align}$$

* $\nabla f$ gives the _VECTOR_ for the _STEEPEST_ grade of a surface at a point

### Example 1
Find $\nabla f(x,y)$ for $f(x,y) = \frac{1}{x^2+y^2}$ at (1,2)  
$$\begin{align}
&f_x = \frac{-2x}{x^2+y^2},\ f_y = \frac{-2y}{x^2+y^2} \newline
&\nabla f(x,y) = \frac{-2x}{(x^2+y^2)^2}\hat i - \frac{2y}{(x^2+y^2)^2}\hat j \rightarrow \text{The vector for Max slope of surface at any point} \newline
&P(1,2) \rightarrow \nabla f(1,2) = \frac{-2}{25}\hat i + \frac{4}{25}\hat j
\end{align}$$

### Example 2
$$\begin{align}
f(x,y,z) &= \frac{x+y}{x+z},\ \nabla f(1,2,3) \newline
f\_x &= \frac{z-y}{(x+z)^2} \newline
f\_y &= \frac{1}{x+} \newline
f\_z &= \frac{-(x+y)}{(x+z)^2} \newline
\nabla f(x,y,z) &= \frac{z-y}{(x+z)^2}\hat i + \frac{1}{x+}\hat j - \frac{-(x+y)}{(x+z)^2} \hat k \newline
\nabla f(1,2,3) &= \frac{1}{16}\hat i + \frac{1}{4}\hat j - \frac{3}{16}\hat k
\end{align}$$

### Example 3
$$\begin{align}
\text{Find }D\_\vec u f(x,y)\ \text{for } f(x,y) = (x^2+y^2+1)^\frac{1}{2}\ \text{at } P(2,2)\ \text{in the direction of } \vec v = 3\hat i + 4\hat j
\end{align}$$

$$\begin{align}
f\_x &= \frac{x}{\sqrt{x^2+y^2+1}},\ f\_y = \frac{y}{\sqrt{x^2+y^2+1}} \newline
\nabla f(x,y) &= \frac{x}{\sqrt{x^2+y^2+1}}\hat i + \frac{y}{\sqrt{x^2+y^2+1}}\hat j \newline
\nabla f(2,2) &= \frac{2}{3}\hat i + \frac{2}{3}\hat j \newline
\vec u &= \frac{\vec v}{|\vec v|} = \frac{3\hat i + 4\hat j}{\sqrt{9 + 16}} = \frac{3}{5}\hat i + \frac{4}{5}\hat j \newline
D\_\vec u f(x,y) &= \nabla f\cdot\vec u \newline
D\_\vec u f(2,2) &= (\frac{2}{3}\hat i + \frac{2}{3}\hat j)\cdot(\frac{3}{5}\hat i + \frac{4}{5}\hat j) = \frac{14}{15}
\end{align}$$