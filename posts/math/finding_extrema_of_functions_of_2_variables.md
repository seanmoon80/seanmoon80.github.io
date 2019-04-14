---
title: "Finding Extrema of Functions of 2 Variables"
date: 2019-04-12T21:59:28-04:00
---

## Extrema of function
* Relative Max is a peak of a _Curve_
* Relative Max is a Pek of a _Surface_
* Relative Max, Relative Min >= 1

## Single variable
* $f\prime(x) = 0\text{ or undefined}$ gives critical points
* Critical points could be inflection points

## 2 Variables
* Both partial derivatives $f_x, f_y = 0$ _AT THE SAME POINT_
* Cricital points could be _undefined(within domain of the function)_ or _saddle point_
* Relative Max - Both $f_x, f_y$ goes to positive to negative (Increasing to Decreasing)
* Relative Min - Both $f_x, f_y$ goes to negative to positive (Decreasing to Increasing)
* Saddle point - One is decreasing to increasing, other one is increasing to decreasing

## Second Derivative Test
* $ D(x,y) = f\_{xx}(x,y) \cdot f\_{yy} - (f\_{xy})^2$
* $f\_{xx}$ is giving concavity in x-direction
* $f\_{yy}$ is giving concavity in y-direction
* $f\_{xx} \cdot f\_{yy}$ is only positive when $x$ and $y$ directions agree on concavity direction.
* $f\_{xy}^2$ is always positive.
* $D(a,b) > 0,\ f\_{xx}(a,b) > 0 \rightarrow Relative Min$
* $D(a,b) > 0,\ f\_{xx}(a,b) < 0 \rightarrow Relative Max$
* $D(a,b) < 0 \rightarrow \text{Saddle point}$
* $D(a,b) = 0 \rightarrow \text{Inconclusive}$
* $f\_x = 0, f\_y = 0 \rightarrow \text{Find critical point} \rightarrow D(x,y) \rightarrow \text{Pulg in critical point}$

### Example 1
$$\begin{align}
f(x,y) &= 2x^2+y^2-2xy-8x-2y+2 \newline
f\_x &= 4x - 2y - 8 = 0 \newline
f\_y &= 2y - 2x - 2 = 0 \newline
2x &= 10, x = 5, y = 6 \newline
&\text{Critical Point: } (5,6) \newline
f\_{xx} &= 4,\ f\_{yy} = 2,\ f\_{xy} = -2 \newline
D(x,y) = 4 \cdot 2 - 4 = 4
\end{align}$$

### Example 2
$$\begin{align}
f\_x = 2x - 6 - \sqrt y = 0,\ f\_y = \frac{-x}{2\sqrt{y}} + 1 = 0 \newline
1 = \frac{x}{2\sqrt{y}} \rightarrow \sqrt{y} = \frac{x}{2} \newline
f\_x = 2x - 6 - \frac{x}{2} \rightarrow x = 4, y = 4 \newline
\end{align}$$

### Example 3
$$\begin{align}
f(x,y) = x^2 + 5y^2 + x^2y + 2y^3 \newline
f\_x = 2x + 2xy, f\_y = 10y + x^2 + 6y^2 \newline
2x(1+y) = 0 \rightarrow x = 0, y = -1 \newline
\text{When x = 0} \newline
2y(3y + 5) = 0 \rightarrow y = 0, y = \frac{-5}{3} \newline
\text{Critical Point: } (0,0), (0, \frac{-5}{3})
\text{When y = -1} \newline
x^2 - 4 = 0 \rightarrow x = 2, -2 \newline
\text{Critical Point: } (2, -1), (-2, -1) \newline
D(x,y) = (2+2y) \cdot (10+12y) - (2x)^2
\end{align}$$

## Absolute Max and Min
* Closed Region, Absolute max and min must exist
* They must occur at either a critical point or on the boundary

### Example 1
$$\begin{align}
f(x,y) = x^2 + xy + y^2,\ R: \\{(x,y) | -2 \ge x \ge 2, -1 \ge y \ge 1 \\} \newline
f\_x = 2x + y, f\_y = x + 2y \newline
3x = 0 \rightarrow x = 0, y = 0 \newline
f(0,0) = 0 \newline
x = -2, y = y \newline
f(-2,y) = 4 - 2y + y^2 \newline
f\prime(-2,y) = 2y - 2 = 0 \rightarrow y = 1
f(-2,1) = 3 \rightarrow \text{Critical point} \newline
f(-2,-1) = 7 \rightarrow \text{End point} \newline\newline
x = 2, y = y \newline
f(2,y) = 4 + 2y + y^2 \newline
f\prime(2,y) = 2y + 2 = 0 \rightarrow y = -1
f(2, -1) = 3 \rightarrow \text{Critical point} \newline
f(2, 1) = 7 \rightarrow \text{End point} \newline\newline
x = x , y = -1 \newline
f(x, -1) = x^2 - x + 1 \newline
f\prime(x, -1) = 2x -1 = 0 \rightarrow x = \frac{1}{2} \newline
f(\frac{1}{2}, -1) = \frac{3}{4} \newline
f(-2, -1) = 7, f(2, -1) = 3
\end{align}$$
