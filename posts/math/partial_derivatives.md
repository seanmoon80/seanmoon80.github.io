---
title: "Partial Derivatives(Derivatives of Multivariable Functions)"
date: 2019-03-03T22:24:53-05:00
---

## Derivative
$f(x,y)$ is a surface in $\mathbb{R}- 3$  

* it is the slope of surface at a point -> $\infty$ number of lines
* Find the slope of the tangent line to a surface at a point. we
  must give the tangent line a Direction
    * For now, we restrict our direction to in the 'X-Direction(Axis)' or
      in the 'y-Direction'
* To find the slope of tangent line in 'X-Direction', we must contain the tangent line in a plane parallel to teh xz-Plane
* Requires "y" to be constant

### Notation
$$\begin{align}
f(x,y) =& z \newline 
\frac{\partial f}{\partial x}, \frac{\partial z}{\partial x}, f\_{x}, z\_{x}:\ &\text{Holds 'y' constant} \newline
&\text{Slope of tangent line ot the surface at a point in x-direction} \\newline
\frac{\partial f}{\partial y}, \frac{\partial z}{\partial y}, f\_{y}, z\_{y}:\ &\text{Holds 'x' constant} \newline
&\text{Slope of tangent line of the surface at apoint in y-direction}
\end{align}$$

### Ex1
$$\begin{align}
f(x,y) &= 2x^2y^3-3x^2y+2x^2+3y^2+1 \newline
\frac{\partial f}{\partial x} &= 4xy^3 - 6xy + 4x \newline
\frac{\partial f}{\partial y} &= 6x^2y^2-3x^2+6y
\end{align}$$

### Ex2
$$\begin{align}
f(x,y) &= xe^{xy^2} \newline
f_{x} &= \frac{\partial}{\partial x}\[x\]e^{xy^2} + x\cdot\frac{\partial}{\partial x}\left[e^{xy^2}\right] \newline
&= e^{xy^2} + x\cdot e^{xy^2}\cdot\frac{\partial}{\partial x}[xy^2] \newline
&= e^{xy^2} + x\cdot e^{xy^2}\cdot y^2 \newline
&= e^{xy^2}(1+xy^2) \newline
f\_{y} &= x\cdot\frac{\partial}{\partial y}\left[e^{xy^2}\right] \newline
&= x\cdot e^{xy^2}\cdot\frac{\partial}{\partial y}\left[xy^2\right] \newline
&= x\cdot e^{xy^2}\cdot 2xy \newline
&= 2x^2ye^{xy^2}
\end{align}$$

### Ex3
$$\begin{align}
g(x,y) &= x^2 \cosh{\frac{x}{y}} \newline
g\_{x} &= 2x\cosh{\frac{x}{y}}+x^2\sinh{\frac{x}{y}}\cdot\frac{1}{y} \newline
g\_{y} &= x^2\sinh{\frac{x}{y}}\cdot(-\frac{x}{y^2})
\end{align}$$

### Ex4
[Quotient Rule](http://tutorial.math.lamar.edu/Classes/CalcI/ProductQuotientRule.aspx)
$$
\left(\frac{f}{g}\right)\prime = \frac{f\prime{g} - fg\prime}{g^2}
$$
$$\begin{align}
f(x,y,z,w) &= \frac{xw^2}{y+\sin{(zw)}} \newline
f\_{x} &= \frac{w^2}{y+\sin{zw}} \newline
f\_{w} &= \frac{2xw\cdot(y+\sin{zw}) - xw^2\cdot\cos{(zw)}\cdot{z}}{(y+sin{(zw)})^2}
\end{align}$$

## Implicit Derivatives(음함수의 미분)

* Take derivative for both sides
* $x\cdot{z}, y\cdot{z}$ - apply product rule

$$\begin{align}
x^2+xz+yz^2 &= 8 \newline
\frac{\partial}{\partial x}\left[x^2y+xz+yz^2\right] &= \frac{\partial}{\partial x}\left[8\right] \newline
2xy + \frac{\partial}{\partial x}[x]\cdot{z} + x\cdot\frac{\partial}{\partial x}[z] + 2y\cdot{z}\cdot\frac{\partial}{\partial x}[z] &= 0 \newline
2xy+z+x\cdot\frac{\partial z}{\partial x} + 2y\cdot z\cdot \frac{\partial z}{\partial x} &= 0 \newline
\frac{\partial z}{\partial x}(x + 2yz) &= -2xy - z \newline
\frac{\partial z}{\partial x} &= \frac{-2xy - z}{x+2yz}
\end{align}$$

## Higher Derivative
$$
f(x,y)
\begin{cases} \displaystyle
\frac{\partial z}{\partial x}
\begin{cases} \displaystyle
\frac{\partial ^2 f}{\partial x^2},\ f\_{xx},\ z\_{xx} \\\\  \\\\  
\displaystyle
\frac{\partial ^2 f}{\partial y \partial x},\ f\_{xy}, z\_{xy}
\end{cases} \\\\ \\\\   
\displaystyle
\frac{\partial z}{\partial y}
\begin{cases} \displaystyle
\frac{\partial ^2 f}{\partial y^2},\ f\_{yy},\ z\_{yy} \\\\ \\\\   
\displaystyle
\frac{\partial ^2 f}{\partial x \partial y},\ f\_{yx},\ z\_{yx}
\end{cases} \\\\
\end{cases}$$

### Ex 1
$$\begin{align}
f(x,y) &= x\sin^2 y+y^2\cos{x}\ f\_{xy},f\_{yx} \newline
f\_{x} &= \sin^2 y - y^2\sin{x} \newline
f\_{xy} &= 2\sin{y}\cdot\cos{y} - 2y\sin{x} \newline
f\_{y} &= 2x\sin{y}\cdot\cos{y}+2y\cos{x} \newline
f\_{yx} &= 2\sin{y}\cdot\cos{y} - 2y\sin{x}
\end{align}$$

* Any function that is continuous on a region, Mixed partial derivatives are Equal

## Laplace Equation
$$\begin{align}
h(x,y) \rightarrow h\_{xx} + h\_{yy} = 0
\end{align}$$
