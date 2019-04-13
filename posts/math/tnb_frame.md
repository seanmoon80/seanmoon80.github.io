---
title: "TNB Frame(Frenet-Serret Frame)"
date: 2019-02-02T09:38:47-05:00
---

## Definition
Unlikely IJK frame, it is moving through the curve.  
To descirbe motion of particles travling along the curve  
T - $\vec{T}$ Unit Tangent Vector. Direction particle is heading.  
N - $\vec{N}$ Normal Vector. Direction particle is turning.  
B - $\vec{B}$ Binormal Vector. Direction of particle's twisting  

## How to find TNB
$\vec{T}$: Unit Tangent
$$\begin{align}&\vec{T}(s) = \vec{r}\prime(s) \text{ or } \vec{T}(t) = \frac{\vec{r}\prime(t)}{||\vec{r}\prime(t)||}\end{align}$$
$\vec{N}$: Unit Normal
$$\begin{align}
&\vec{N}(t) = \frac{\vec{T}\prime(t)}{||\vec{T}\prime(t)||} \newline 
&\text{Every vector with a constant length is perpendicular to it's Tangent vector} \newline
&\text{Proof: Let } \vec{v} \text{ have constant length} \newline
&\vec{v}\cdot\vec{v} = |\vec{v}|^2 = C^2 \newline
&\dfrac{d}{dt}(\vec{v}\cdot\vec{v}) = \dfrac{d}{dt}(C^2) \newline
&\vec{v}\prime\cdot\vec{v} + \vec{v}\cdot\vec{v}\prime = 2(\vec{v}\prime\cdot\vec{v}) = 0 \newline
&\text{So } \vec{T}(t) \perp \vec{T}\prime(t)
\end{align}$$
$\vec{B}$: Unit Binormal
$$\vec{B} = \vec{T} \times \vec{N}$$

## Curvature(곡률)
Curvature is Arc Length compared to Heading($\vec{T}$).  
How $\vec{T}$ is changing with respect to arc length.

### Arc length reparameterized vector function
$$
\vec{r}\prime(s) = \vec{T}(s)  
$$
$$
\kappa = \left|\left|\dfrac{d\vec{T}}{ds}\right|\right| = \left|\left|\vec{T}\prime(s)\right|\right|$$

### Original vector function
$$\begin{align}
\vec{T}\prime(t) = \dfrac{d\vec{T}}{dt} \rightarrow &\dfrac{d\vec{T}}{dt} = \dfrac{d\vec{T}}{ds}\cdot\dfrac{ds}{dt} \newline
&\dfrac{d\vec{T}}{ds} = \frac{\dfrac{d\vec{T}}{dt}}{\dfrac{ds}{dt}} \rightarrow ||\dfrac{d\vec{T}}{ds}|| = \frac{\||\dfrac{d\vec{T}}{dt}\||}{\||\dfrac{ds}{dt}\||}\tag 1 \newline
S(t) = \int \||r\prime\||\, dt \rightarrow & \dfrac{d}{dt}(S(t)) = \dfrac{d}{dt}\int \||r\prime\(t)||\, dt \newline
&\dfrac{ds}{dt} = ||r\prime(t)|| \tag 2 \newline
&\kappa = \frac{||\vec{T}\prime(t)||}{||\vec{r}\prime(t)||}
\end{align}$$

### With Polynomial
$$
\kappa = \frac{||\vec{r}\prime\times\vec{r}\prime\prime||}{||\vec{r}\prime||^3}
$$

## Torsion(곡선 비틀림)
A measure of a curves "Failure to be contained in plane"
$$\begin{align}
\tau &= \frac{(\vec{r}\prime\times\vec{r}\prime\prime)\cdot\vec{r}\prime\prime\prime}{\||\vec{r}\prime\times\vec{r}\prime\prime\||^2} \newline
\tau &= \dfrac{-d\vec{B}}{ds}\cdot\vec{N}
\end{align}$$

## Osculating Circle
At any point on a curve, There will be a circle that fits that curve "BEST"  
At the ponit, A circle and a curve have Same tangent, Same curvature.  
Unit Normal($\vec{N}$) will pass throuogh or point center of circle.  
The Plane that contains circle(osculating plane) must contain $\vec{T}\text{ and }\vec{N}$  
The radius of osc circle is called "Radius of Curvature" and  
$$
\rho = \frac{1}{\kappa}
$$

## Example 1
Find $\vec{T}\, \vec{N}\, \vec{B}\, \kappa\, \rho$, EQ of OSC plane and EQ of Normal plane at $t = \frac{\pi}{2}$  
For $\vec{r}(t) = \cos{t}\hat i + \sin{t}\hat j + t\hat k$

### Tangent vector
$$\begin{align}
\vec{r}\prime(t) &= -\sin{t}\hat i + \cos{t}\hat j + \hat k \tag 1 \newline
||\vec{r}\prime(t)|| &= \sqrt{\sin^2 t + \cos^2 t + 1} \newline &= \sqrt{2} \tag 2 \newline
\vec{T}(t) &= \frac{-\sin{t}\hat i + \cos{t}\hat j + \hat k}{\sqrt{2}} \newline
&= \frac{2}{\sqrt{2}}(-\sin{t}\hat i + \cos{t}\hat j + \hat k) \tag 3 \newline
\end{align}$$

### Normal vector
$$\begin{align}
\vec{T}\prime(t) &= \frac{\sqrt{2}}{2}(-\cos{t}\hat i + -\sin{t}\hat j) \tag 4 \newline
||\vec{T}\prime(t)|| &= \frac{\sqrt{2}}{2}\sqrt{\cos^2 t + \sin^2 t} \newline
&= \frac{\sqrt{2}}{2} \tag 5 \newline
\vec{N}(t) &= \frac{\vec{T}\prime(t)}{||\vec{T}\prime(t)||} \newline
&= \frac{\frac{\sqrt{2}}{2}(-\cos{t}\hat i + -\sin{t}\hat j)}{\frac{\sqrt{2}}{2}} \newline
&= -\cos{t}\hat i - \sin{t}\hat j \tag 6 \newline
\end{align}$$

### Binormal vector
$$\begin{align}
\vec{N} &= \vec{T}\times\vec{N} \newline
&= \frac{\sqrt{2}}{2}\begin{bmatrix}-\sin{t} & \cos{t} & 1 \newline -\cos{t} & -\sin{t} & 0\end{bmatrix} \newline
&= \frac{\sqrt{2}}{2}(\sin{t}\hat i + \cos{t}\hat j + \hat k) \newline
\end{align}$$

### Curvature
$$\begin{align}
\kappa &= \frac{||\vec{T}\prime(t)||}{||\vec{r}\prime(t)||} \newline
&= \frac{\frac{\sqrt{2}}{2}}{\sqrt{2}} = \frac{1}{2} \tag 7 \newline
\end{align}$$

### Radius of curvature
$$\begin{align}
\rho &= \frac{1}{\kappa}  = 2 \tag 8
\end{align}$$

### Point at given t
$$\begin{align}
\vec{r}(\frac{\pi}{2}) &= 0\hat i + 1\hat j + \frac{\pi}{2}\hat k \newline
\vec{T}(\frac{\pi}{2}) &= \frac{\sqrt{2}}{2}(-\hat i + 0\hat j + \hat k) \newline
\vec{N}(\frac{\pi}{2}) &= -\hat j \newline
\vec{B}(\frac{\pi}{2}) &= \frac{\sqrt{2}}{2}(\hat i + \hat k)
\end{align}$$

### Osculating Plane
Contains $\vec{T} \text{ and } \vec{N}\, \vec{B}$ is the normal vector
$$\begin{align}
P(0,1,\frac{\pi}{2}),\  \vec{B} = \frac{\sqrt{2}}{2}(\hat i + \hat k),\ \vec{n} = \hat i + \hat k \newline
\text{Plane} \rightarrow 1(x-0)+0(y-1)+1(z-\frac{\pi}{2}) = 0 \newline
x + z = \frac{\pi}{2}
\end{align}$$

### Normal Plane
Contains $\vec{N} \text{ and } \vec{B},\ \vec{T}$ is the normal
$$\begin{align}
P(0,1,\frac{\pi}{2}), \ \vec{T} = \frac{\sqrt{2}}{2}(-\hat i + \hat k),\ \vec{n} = -\hat i + \hat k \newline
\text{Plane} \rightarrow -1(x - 0)+0(y-1)+1(z-\frac{\pi}{2}) = 0  \newline
-x + z = \frac{\pi}{2}
\end{align}$$

## Encapsulation
Find curvature of $y = x^3 + 1$  
Apply one of below formulars for given polinomial  

$$\begin{align}
y = f(x) &\rightarrow \left\< t, f(t), 0\right>,\ t\hat i + f(t)\hat j\newline
x = g(y) &\rightarrow \left\< g(t), t, 0\right>,\ g(t)\hat i + t\hat j\newline
x = f(t), y=g(t) &\rightarrow \left\< f(t), g(t), 0\right>, f(t)\hat i + g(t)\hat j \newline
r = f(\theta) &\rightarrow \left\< f(t)\cos{t}, f(t)\sin{t},0\right>
\end{align}$$  
  
$$\begin{align}
y = x^3 + 1 &\rightarrow t\hat i + (t^3 + 1)\hat j \newline
\vec{r}\prime(t) &= \hat i + 3t^2\hat j \newline
||\vec{r}\prime(t)|| = \sqrt{1 + 9t^4} \newline
\vec{r}\prime\prime(t) = 6t\hat j \newline
\kappa = \frac{6t}{(\sqrt{1+9t^4})^3}
\end{align}$$