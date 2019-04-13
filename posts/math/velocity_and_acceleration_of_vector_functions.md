---
title: "Velocity and Acceleration of Vector functions"
date: 2019-02-12T22:45:44-05:00
---

## Velocity and Acceleration
$$\begin{align}
\text{Given vector funciton }&\vec{r}(t) \newline
\text{Velocity: }&\vec{v}(t) = \vec{r}\prime(t) \newline
\text{Acceleration: }&\vec{a}(t) = \vec{v}\prime(t) = \vec{r}\prime\prime(t) \newline
\text{Speed: }&||\vec{v}(t)||
\end{align}$$

### Example 1
Find Velocity, Accel and speed of a particle described by $\vec{r}(t) = \left< t, t^2, t^3 \right>$ at t = 1
$$\begin{align}
\text{Velocity: } &\vec{r}\prime(t) = \left< 1, 2t, 3t^2 \right> \rightarrow \vec{v}(1) = \left< 1, 2, 3 \right> \newline
\text{Speed: } &||\vec{v}(1)|| = \sqrt{1+4+9} = \sqrt{14} \newline
\text{Acceleration: } &\vec{r}\prime\prime(t) = \left< 0, 2, 6t \right> \rightarrow \vec{a}(1) = \left< 0, 2, 6 \right> \newline
\end{align}$$

### Example 2 (Integral)
$\underbrace{\vec{a}(t) = e^t\hat i + e^{-t}\hat k}_{\vec{r}\prime\prime(t)},\ \ \underbrace{\vec{v}(0) = \hat i + 2\hat j}\_{\vec{r}\prime(0)},\ \ \vec{r}(0) = 3\hat i + \hat j + 2\hat k$
$$\begin{align}
&\vec{v}(t) = \int{\vec{a}(t)}\, dt \rightarrow \int{e^t\hat i + e^{-t}\hat k}\, dt = e^t\hat i - e^t\hat k + C\_{1} \newline
&\vec{v}(0) = \hat i + 2\hat j = \hat i - \hat k + C\_{1} \newline
&C\_{1} = 2\hat j + \hat k \newline
&\vec{v}(t) = e^t\hat i - e^{-t}\hat k + 2\hat j + \hat k = e^t\hat i - 2\hat j +(1 - e^{-t})\hat k \newline
&\int{\vec{v}(t)}\, dt = e^t\hat i + 2t\hat j + (t + e^{-t})\hat k + C\_{2} \newline
&\vec{r}(0) = \hat i + \hat k + C\_{2} = 3\hat i + \hat j + 2\hat k \newline
&C\_{2} = 2\hat i + \hat j + \hat k \newline
&\vec{r}(t) = (e^t + 2)\hat i + (1 + 2t)\hat j + (1 + t + e^{-t})\hat k
\end{align}$$

### Note
We can define Accel as a vector with $\vec{T} and \vec{N}$ (Let $||\vec{v}(t)|| = v$ Speed)  
$$\begin{align}
\vec{a} = v\prime\vec{T} + \kappa v^2\vec{N} \text{ or } \newline
\vec{a} = \frac{\vec{r}\prime \cdot \vec{r}\prime\prime}{||\vec{r}\prime||}\vec{T} + \frac{||\vec{r}\prime \times \vec{r}\prime\prime||}{||\vec{r}\prime||}\vec{N}
\end{align}$$

### Example 3
$$\begin{align}
&\vec{r}(t) = (\vec{v}_{0}\cos\alpha)t\hat i + \left\[ h + (\vec{v}\_{0}\sin\alpha)t - \frac{1}{2}gt^2 \right\]\hat j \newline
&\vec{v}\_{0} = \text{Initial Velocity} \newline
&\alpha = \text{Angle of horizontal inclination} \newline
&h = \text{Height} \newline
&g = \text{Acceleration Gravity}
\end{align}$$

Qestion: You shoot a rifle from a 200 FT cliff with angle of 30 degrees form parallel and muzzle velocity of 1500 ft/sec

$$\begin{align}
&\vec{v}_{0} = 1500 FT/sec \newline
&\alpha = \frac{\pi}{6} \newline
&h = 200 FT \newline 
&g = 32 FT/s^2 \newline
\end{align}$$
$$\begin{align}
\vec{r}(t) &= (1500\cdot\cos(\frac{\pi}{6}))t\hat i + \left\[200 + (1500\cdot\sin(\frac{\pi}{6}))t - 16t^2\right\]\hat j \newline
&= \underbrace{750\sqrt{3}t\hat i}\_{x: Range} + \underbrace{(200 + 750t - 16t^2)\hat j}\_{y: Height} \newline
\end{align}$$
Q1 When Bullet Hit ground?  
$$\begin{align}
&y = 0 \rightarrow 200+750t-16t^2 = 0 \rightarrow t = 47.1 sec \newline
\end{align}$$
Q2 Max Range?  
$$
x = 750\sqrt{3}(47.1)
$$