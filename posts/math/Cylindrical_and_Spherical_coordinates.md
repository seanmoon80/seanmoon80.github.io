---
title: "Cylindrical and Spherical coordinates"
date: 2019-01-08T17:12:06-05:00
---

## Polar coordinate system(극좌표계)
![polar coordinate](/CircularCoordinates.png)
* 평면위의 위치를 각도($\theta$)와 거리($r$)로 표현

---
## Cylindrical coordinate system(원통좌표계)
$$(x, y, z) \implies (r, \theta, z)$$
![cylindrical coordinate](/Cylindrical_coordinate.gif)  
* 'r'은 3차원 공간상에서 원점에서부터 점까지의 거리가 아님.  
* 'r'은 xy 평면에 투사된 점까지의 거리  
* xy평면에 투영시 팔분면에서의 위치를 사분면의 위치로 투영.

### Rectangular coordinate system(직교좌표계)과의 관계
$$\begin{align}
Cyl \xrightarrow\ Rec\ &\begin{cases}
\cos\theta = \frac{x}{r} \implies x = r\cos\theta \newline
\sin\theta = \frac{y}{r} \implies y = r\sin\theta \newline
z = z
\end{cases} \newline
Rec \xrightarrow\ Cyl\ &\begin{cases}
r^2 = x^2 + y^2 \implies r = \sqrt{x^2 + y^2} \newline
\tan\theta = \frac{y}{x} \newline
z = z
\end{cases}
\end{align}$$

### Example
#### Cylindrical to Rectagular
$$\begin{align}
&(3, -\frac\pi{6},2) \implies \text{Rectangular coordinate} \newline
&Oct = 4,\ Quad = 4 \newline
&r = 3,\ \theta = -\frac\pi{6},\ z = 2 \newline
&x = r\cos\theta \implies 3\cos({-\frac\pi{6}}) = \frac{3\sqrt{3}}{2} \newline
&y = r\sin\theta \implies 3\sin({-\frac\pi{6}}) = -\frac{3}{2} \newline
&(\frac{3\sqrt{3}}{2}, -\frac{3}{2}, 2)
\end{align}$$
#### Rectangular to Cylindrical
$$\begin{align}
&(\sqrt{2}, -\sqrt{2}, 4) \newline
&Oct = 4,\ Quad = 4 \newline
&z = 4 \newline
&r = \sqrt{x^2 + y^2} \implies r = \sqrt{(\sqrt{2})^2 + (-\sqrt{2})^2} = \pm 2 \newline
&\tan\theta = \frac{y}{x} \implies \tan\theta = -1 \newline
&\theta = \frac{3\pi}{4}\ or\ \frac{7\pi}{4}
\end{align}$$

---
## Spherical coordinate system(구면좌표계)
{{< geogebra id="usjmrzwq" width="800" height="600" >}}
$$(x, y, z) \implies (\rho, \theta, \phi)$$
* $\rho$ 원점에서부터 어떤 점 P까지의 거리  
* $\theta$ 원통좌표계와 동일  
* $\phi$  Z축으로부터 어떤 점 P까지의 양의 각도($0 <= \phi <= \pi$)
$$\begin{align}
&\sin\phi = \frac{r}{\rho} \implies r = \rho\sin\phi \newline
&\cos\phi = \frac{z}{\rho} \implies z = \rho\cos\phi \newline
Sph \xrightarrow\ Rec\ &\begin{cases}
x = r\cos\theta \implies x = \rho\sin\phi\cos\theta \newline
y = r\sin\theta \implies y = \rho\sin\phi\sin\theta \newline
z = \rho\cos\phi
\end{cases} \newline
Rec \xrightarrow\ Sph\ &\begin{cases}
\rho^2 = r^2 + z^2 \implies \rho = \sqrt{x^2 + y^2 + z^2} \newline
\tan\theta = \frac{y}{x} \newline
\cos\phi = \frac{z}{\rho}
\end{cases}
\end{align}$$

### Example
#### Spherical to Rectangular
$$ \\
Sph: (3, \frac{\pi}{4}, \frac{3\pi}{4})
$$
$$
\begin{align} \newline
x &= \rho\sin\phi\cos\theta = 3\sin\frac{3\pi}{4}\cos\frac{\pi}{4} = 3 \cdot \frac{\sqrt{2}}{2} \cdot \frac{\sqrt{2}}{2} \newline
&= \frac{3}{2} \newline\newline
y &= \rho\sin\phi\sin\theta = 3\sin\frac{3\pi}{4}\sin\frac{\pi}{4} = 3 \cdot \frac{\sqrt{2}}{2} \cdot \frac{\sqrt{2}}{2} \newline
&= \frac{3}{2} \newline\newline
z &= \rho\cos\phi = 3\cos\frac{3\pi}{4} = 3 \cdot (-\frac{\sqrt{2}}{2}) \newline
&= \frac{-3\sqrt{2}}{2}
\end{align}
$$

#### Rectangular to Spherical
$$ \\
Rec: (-2,2\sqrt{3},4)
$$
$$
\begin{align}
&Quad = 2,\ Oct = 2 \newline
\rho &= \sqrt{x^2 + y^2 + z^2} = \sqrt{(-2)^2 + (2\sqrt{3})^2 + 4^2} = \sqrt{32} \newline
&= 4\sqrt{2} \newline\newline
\tan\theta &= \frac{y}{x} = \frac{2\sqrt{3}}{-2} \newline
\theta &= \tan^{-1}-\sqrt{3} = \frac{2\pi}{3}\, \frac{5\pi}{3} \newline
\cos\phi &= \frac{z}{\rho} = \frac{4}{4\sqrt{2}} = \frac{\sqrt{2}}{2}
\phi = \frac{\pi}{4}
\end{align}
$$