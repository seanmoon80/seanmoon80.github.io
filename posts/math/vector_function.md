---
title: "Vector Function"
date: 2019-01-16T21:45:14-05:00
---

## Definition
1. 실수 집합을 정의역으로 가지며 벡터의 집합을 치역으로 가지는 함수
2. 그러한 함수를 $r$이라하고 $r$의 정의역의 어떤 수 $t$에 대한 유일한 벡터 $V_3$가 있을 경우 $r(t)$로 표기할수 있다.
$$\begin{align}
&A = \\{ t \mid t \in \mathbb{R} \\}, B = \\{\left< x,y,z \right> \mid x,y,z \in \mathbb{R} \\} \newline
&\vec r : A\rightarrow B
\end{align}$$
3. $r(t)$의 component가 $f(t),\ g(t), h(t)$로 표현될 경우 $f, g, h$는 $r$의 component functions이라 부를수 있고
$$r(t) = \left< f(t),g(t),h(t) \right> = f(t)i + g(t)j + h(t)k$$
4. $t$는 독립변수로서 일반적으로 시간을 나타냄
5. 치역의 벡터들의 종점은 삼차원상에서 Curve의 자취를 나타냄

### Example
$$\begin{align}
\vec r(t) = \left<\sqrt{t}, \frac{1}{t-1},\ln{t}\right> \newline
\underbrace{x = \sqrt{t}}_{t \ge 0},\ \underbrace{y = \frac{1}{t-1}}\_{t \ne 1},\ \underbrace{z = \ln{t}}\_{t \gt 0} \newline 
\text{Common Domain}: 0 \lt t \lt 1, 1 \lt t \newline\newline
t = 2: \vec r(2) = \left<\sqrt{2},1,\ln2\right>\newline
t = 4: \vec r(4) = \left<2, \frac{1}{3}, \ln4\right>
\end{align}$$

### Sketching
1. 'x', 'y', 'z' component를 구함
2. 하나이상의 component 함수를 이용(식을 t에 대해 정리) curve나 surface를 구함
    * component 함수 2개 이용시 평면에  
    * component 함수 3개 이용시 surface를 따라 curve 
3. 't'에 어떤값을 대입해서 방향과 점을 찾음.

{{< geogebra id="ntgmyyt4" width="800" height="600" >}}

#### Example 1
$$\begin{align}
&\vec r(t) = \underbrace{\sqrt{t}\hat\imath}_{x} + \underbrace{(4 - t)\hat\jmath}\_{y},\ t \ge 0 \newline
&x^2  = t \newline
&y = 4 - x^2 \newline
&t = 0: \vec r(0) = 4\hat\jmath \newline
&t = 4: \vec r(4) = 2\hat\imath
\end{align}$$

#### Example 2
$$\begin{align}
&\vec r(t) = \left< t, t^2, t^3 \right>,\ t \ge 0 \newline
&x = t, y = t^2, z = t^3 \newline
\end{align}$$

### Limit
$$\begin{align}
\lim_{t \to a} \vec r(t) = \left<\lim\_{t \to a}f(t), \lim\_{t \to a}g(t), \lim\_{t \to a}h(t)\right>
\end{align}$$

#### Example 1
$$\begin{align}
&\lim_{t \to 2} \Big[\sqrt{t}\hat\imath + (\frac{t^2-4}{t-2})\hat\jmath + (\frac{t}{t^2+1})\hat k\Big] \newline\newline
&\lim\_{t \to 2}\sqrt{2} = sqrt{2} \newline\newline
&\lim\_{t \to 2}\frac{t^2-4}{t-2} = \lim\_{t \to 2}\frac{(t-2)(t+2)}{t-2} = 4 \newline\newline
&\lim\_{t \to 2}\frac{t}{t^2+1} = \frac{2}{5} \newline\newline
&= \left\<\sqrt{2}, 4, \frac{2}{5} \right>
\end{align}$$