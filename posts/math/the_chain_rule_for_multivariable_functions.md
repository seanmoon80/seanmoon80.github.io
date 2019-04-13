---
title: "The Chain Rule for Multivariable Functions"
date: 2019-03-22T19:30:55-04:00
draft: true
---

## Chain rule for singlevariable function
$$\begin{align}
\frac{dy}{dt} &= \frac{dy}{dx}\cdot\frac{dx}{dt} \newline
(f \circ g)\prime &= (f\prime \circ g)\cdot g\prime \newline
f(g(x)) &= f\prime(g(x))\cdot g\prime(x) \newline\newline
\end{align}$$
$$\begin{align}
y &= (3x)^4,\ u = 3x,\ y = u^4 \newline
y &= f(u),\ f(u) = u^4,\ u = g(x) = 3x \newline
\frac{dy}{dx} &= 4u^3\cdot 3 = 12\cdot(3x)^3 = 324x^3
\end{align}$$
* Even though there are 3-variables (x,y,t), only __1 Independent variable__ exist.  
* In above example, Variable __$u$__ is __Intermediate Variable__

## Multivariable function
$$\begin{align}
w = x^2 - y^2,\ x = t^2+1,\ y = t^3 + t \newline
\end{align}$$
* "x" and "y" are __Intermediate variables__ "t" is the __Independant variable__  
* Therefore, It has two paths from "w" to "t" to find $\frac{dw}{dt}$  
* $\Delta{t} \rightarrow \Delta{x},\ \Delta{y} \rightarrow \Delta{w}$
$$\begin{align}
\Delta{w} &= \text{The amount "x" changes "w"} + \text{The amount "y" changes "w"}\newline
&= \underbrace{\text{Rate of change in x-direction}}\_{\frac{\partial{w}}{\partial{x}}}\cdot\Delta{x} + \underbrace{\text{Rate of change in y-direction}}\_{\frac{\partial{w}}{\partial{y}}}\cdot\Delta{y} \newline
\Delta{w} &= \frac{\partial w}{\partial x}\cdot\Delta x + \frac{\partial w}{\partial y}\cdot\Delta y \newline
\frac{\Delta w}{\Delta t} &= \frac{\partial w}{\partial x}\cdot\frac{\Delta x}{\Delta t} + \frac{\partial w}{\partial y}\cdot\frac{\Delta y}{\Delta t} \newline
\underbrace{\lim_{\Delta{t} \to 0}\frac{\Delta w}{\Delta t}}\_{\frac{dw}{dt}} &= \frac{\partial w}{\partial x}\cdot\underbrace{\lim\_{\Delta{t} \to 0}\frac{\Delta x}{\Delta t}}\_{\frac{dx}{dt}} + \frac{\partial w}{\partial y}\cdot\underbrace{\lim\_{\Delta{t} \to 0}\frac{\Delta y}{\Delta t}}\_{\frac{dy}{dt}} \newline
\frac{dw}{dt} &= \frac{\partial w}{\partial x}\cdot\frac{dx}{dt} + \frac{\partial w}{\partial y}\cdot\frac{dy}{dt}
\end{align}$$

### Example 1
$$\begin{align}
w = x^2y - xy^3,\ x = \cos t,\ y = e^t \newline
\frac{dw}{dt} &= \frac{\partial w}{\partial x}\cdot\frac{dx}{dt} + \frac{\partial w}{\partial y}\cdot\frac{dy}{dt} \newline
&= (2xy - y^3)\cdot(-\sin t) + (x^2 - 3xy^2)\cdot e^t
\end{align}$$

## Multi Independent variables
* It has to be partial derivative for each Independent variables.  
$$\begin{align}
w 
\begin{cases}
x
\begin{cases}
u \newline
v
\end{cases}
\newline
y
\begin{cases}
u \newline
v
\end{cases}
\end{cases}
\frac{\partial w}{\partial u},\ \frac{\partial w}{\partial v} \newline
\frac{\partial w}{\partial u} = \frac{\partial w}{\partial x}\cdot\frac{\partial x}{\partial u} + \frac{\partial w}{\partial y}\cdot\frac{\partial y}{\partial u} \newline
\frac{\partial w}{\partial v} = \frac{\partial w}{\partial x}\cdot\frac{\partial x}{\partial v} + \frac{\partial w}{\partial y}\cdot\frac{\partial y}{\partial v}
\end{align}$$

### Example 2
$$
w = x^3 + y^3,\ x = u^2 + v^2,\ y = 2uv \\\\  
\begin{align}
\frac{\partial w}{\partial u} &= 3x^2\cdot 2u + 3y^2\cdot 2v \newline
\frac{\partial w}{\partial v} &= 3x^2\cdot 2v + 3y^2\cdot 2u \newline
\end{align}$$

### Example 3
$$
w = x\tan^{-1}(yz),\ x = u^{\frac{1}{2}},\ y = e^{-2v},\ z = v\cos{u}\\\\  
\begin{align}
\frac{\partial w}{\partial u} &= \frac{\partial w}{\partial x}\cdot\frac{\partial x}{\partial u} + \frac{\partial w}{\partial z}\cdot\frac{\partial z}{\partial u} \newline
\frac{\partial w}{\partial v} &= \frac{\partial w}{\partial y}\cdot\frac{\partial y}{\partial v} + \frac{\partial w}{\partial z}\cdot\frac{\partial z}{\partial v} \newline
\frac{\partial w}{\partial u} &= \tan^{-1}(yz)\cdot\frac{1}{2\sqrt{u}} + x\cdot\frac{1}{1 + y^2z^2}\cdot{y}\cdot (-v\sin u) \newline
\frac{\partial w}{\partial v} &= x\cdot\frac{1}{1 + y^2z^2}\cdot{z}\cdot(-2e^{-2v}) + x\cdot\frac{1}{1+y^2z^2}\cdot{y}\cdot\cos{u}
\end{align}$$

## Implicit Form
$$
w = f(x,y)\, y = g(x)\\\\  
\begin{align}
\frac{\partial w}{\partial x} &= \frac{\partial w}{\partial x} + \frac{\partial w}{\partial y}\cdot\frac{dy}{dx} = 0 \newline
\frac{\partial w}{\partial y}\cdot\frac{dy}{dx} &= -\frac{\partial w}{\partial x} \newline
\frac{dy}{dx} &= -\frac{f_x}{f_y}
\end{align}
$$

### Example 4
$$
2x^2 + 3(xy)^{\frac{1}{2}} - 2y - 4 = 0,\ y = g(x)\ \text{Find } \frac{dy}{dx}\\\\  
\frac{dy}{dx} = -\frac{4x + \frac{3}{2}(xy)^{-\frac{1}{2}}\cdot y}{\frac{3}{2}(xy)^{-\frac{1}{2}}\cdot x - 2}
$$