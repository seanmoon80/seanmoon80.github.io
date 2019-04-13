---
title: "Finding Tangent Planes and Normal Lines to Surfaces"
date: 2019-04-05T22:32:08-04:00
---

## Tangent Plane
* GeoGebra - https://www.geogebra.org/classic/f2u7jjsb
* In 2-d, We can find tangent line at a point
* In 3-d, We can find tangent plane at a point
* Let's say we have $f(x,y) = z$ surface. It will have a level curve at $f(x,y) = C
* Level curve is always 1 dimension less (3D -> 2D, 4D -> 3D)
* It can redefine to vector function $\vec r(t) = x(t)\hat i + y(t)\hat j \rightarrow$ Level curve
* Function for level curve is $f(x(t),y(t)) = C
* Take derivative with respect to variable "t" $\rightarrow f\prime(x(t),y(t)) = 0$
$$\begin{align}
\frac{\partial f}{\partial y}\cdot\frac{dy}{dt} + \frac{\partial f}{\partial x}\cdot\frac{dx}{dt} &= 0\\\\  
(\frac{\partial f}{\partial x}\hat i + \frac{\partial f}{\partial y}\hat j)\cdot(\frac{dx}{dt}\hat i + \frac{dy}{dt}\hat j) &= 0\\\\  
(f_x\hat i + f_y\hat j)\cdot(\frac{dx}{dt}\hat i + \frac{dy}{dt}\hat j) &= 0\\\\  
\nabla f(x,y)\cdot\vec r\prime(t) &= 0
\end{align}$$

* $\nabla f(x,y)\cdot\vec r\prime(t) = 0$  
* $\vec r\prime(t)$ gives a _slope of tangent vector of level curve_  
* dot product = 0, the two vectors are _orthogonal_ $\rightarrow |\vec v_1|\cdot|\vec v_2|\cdot\cos\theta$
* $\nabla f(x,y)$ is the normal to a level curve $f(x,y) = C$
* $\nabla f(x,y,z)$ is the normal to a level surface $(x,y,z) = C$
* tangent planes and normal lines

### Examples 1
Find the tangent line and normal line to $x^2-y^2 = 16$ at point(5,3)  
* $x^2-y^2 = 16$ is 2-D, to get gradient we need to pretend $x^2-y^2=16$ is a level curve to some serface in 3D  

$$\begin{align}
x^2 - y^2 = 16 \rightarrow \text{3-D: } f(x,y) = x^2 - y^2 \newline  
\nabla f(x,y) = 2x\hat i - 2y\hat j \rightarrow \text{Normal vector to any level curve } x^2 - y^2 = C \newline  
\nabla f(5,3) = 10\hat i - 6\hat j \newline
m_N = \frac{-6}{10} = \frac{-3}{5} \rightarrow \text{Slope of Normal line} \newline
y - y_1 = m(x-x_1) \rightarrow \text{Equation of the Normal line}\newline
y - 3 = \frac{-3}{5}(x - 5) \rightarrow y = \frac{-3}{5}x + 6\newline
m_T = \frac{-1}{m_N} = \frac{5}{3}\newline
y - 3 = \frac{5}{3}(x - 5) \rightarrow y = \frac{5}{3}x - \frac{16}{3}
\end{align}$$

### Examples 2
Find Normal vector to $-x^2+y^2-z^2=4$ at point (1,3,2)  
$$\begin{align}
f(x,y,z) = -x^2+y^2-z^2 \rightarrow 4-D\newline
\nabla f(x,y,z) = -2x\hat i + 2y\hat j -2z\hat k
\end{align}$$

## Planes
$\vec n = a\hat i + b\hat j + c\hat k$ and $P(x_0,y_0,z_0)$  
$a(x-x_0) + b(y-y_0) + c(z-z_0) = 0$  

## Normal lines
$\frac{x-x_0}{a}a = \frac{y-y_0}{b} = \frac{z-z_0}{c}$  
$x = x_0+at, y = y_0+bt, z = z_0+ct$
