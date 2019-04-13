---
title: "Limits and continuity of multivariable functions"
date: 2019-02-27T21:35:04-05:00
---

## Limits
In 2-D, There are only two path to approach to some point 'a'.  
Therefore, Limit does exist if thoes two path approaching to same
value  
  
2차원상에서 특정한 점 'a'로 접근하는 경로는 2개밖에 없으므로  
좌극한과 우극한의 값이 동일할 경우 극한값 존재

$$
\lim\_{x \to a}f(x) = L  \\\\  
\lim\_{a \to a^-}f(x) = \lim\_{a \to a^+}f(x)
$$

In 3-D, There are infinity number of path exist 
to apprach to some point 'a'  
  
3차원상에서 특정한 점 'a' 와 'b'로 접근하는 경로는 무한개 존재

### How to find Limit
1. Squeeze Theorem (샌드위치 정리)
2. Continuity of function (함수의 연속성)
3. Find 2 path to show limit doesn't exist

### DNE(Does Not Exist) Example
#### Step 1
Set $x = 0$. So, we can travel along the surface directly over
'y-Axis'
$$
\lim_{(x,y) \to (0,0)}\frac{x^2 - y^2}{2x^2+y^2} \\\\  
\text{when x = 0} \rightarrow \lim\_{y \to 0}\frac{0^2 - y^2}{0 + y^2} = -1 \\\\  
\text{when y = 0} \rightarrow \lim\_{x \to 0}\frac{x^2 - 0}{2x^2 - 0} = \frac{1}{2} \\\\  
-1 \ne \frac{1}{2}\ \text{Therefore, limit does not exist at } (0,0)
$$
#### Step 2
If Step1 doesn't work.  
1. Pick another path which contains the point (a, b)  
2. Try to substitute so degrees of numer and denom are equal.(분모분자 약분가능)  
3. Always use either x = 0 or y = 0 as 1 Path  
$$
\lim_{(x,y) \to (0,0)}\frac{3xy}{3x^2+y^2} \\\\  
x = 0 \rightarrow 0,\ y = 0 \rightarrow 0
$$

Set $y = f(x)$ or $x = f(y)$ Make it sure path contains the point (a,b)  
$$
y = x \rightarrow \lim_{x \to 0}\frac{3x^2}{4x^2} = \frac{3}{4} \\\\  
0 \ne \frac{3}{4}\, \text{Therefore, Limit does not exist.}
$$

$$
\lim_{(x,y) \to (1,0)}\frac{2xy - 2y}{x^2+y^2-2x+1} \\\\  
y = 0 \rightarrow \lim\_{x \to 1}\frac{0}{x^2-2x+1} = 0 \\\\  
x = 1 \rightarrow \lim\_{y \to 0}\frac{2y-2y}{y^2} = 0 \\\\  
\lim\_{(x,y) \to (1,0)}\frac{2y(x-1)}{y^2+(x-1)^2} \\\\
x-1 = y \rightarrow \lim\_{y \to 0}\frac{2y\cdot y}{y^2+y^2} = 1
$$

1. For 3-var, Paths are now Parametric "t"  
2. Always choose an AXIS as 1st path
$$
\lim\_{(x,y,z) \to (0,0,0)}\frac{xy+yz+xz}{x^2+y^2+z^2} \\\\  
\text{Along X-Axis} (y = 0, z = 0) \rightarrow \lim\_{x \to 0}\frac{0}{x^2} = 0 \\\\  
\text{Along C:} x = t, y = t, z = t \rightarrow \frac{3t^2}{3t^2} = 1
$$

### Continuity
a Function continuous at any point inside its domain  
1. Polynomial continuous everywhere  
2. Rational function continuous everywhere where denom $\ne 0$  
3. Continuity holds for compositions.  

#### Continuity Example
##### EX1
$$
f(x,y) = \frac{x^3+xy+y^3}{x^2+y^2} \\\\  
\text{Doman :}\\{ (x,y)|(x,y) \ne (0,0) \\} \\\\  
$$

##### EX2
$$
f(x,y,z) = \frac{xyz}{x^2+y^2+z^2+4} \\\\  
\text{Domain :}\\{ (x,y,z) | x^2+y^2+z^2 \ne 4 \\}
$$

##### EX3
$$\begin{align}
f(x,y) &= x^2 + xy + y^2 \\\\  
g(t) &= t\cos{t} + \sin{t} \\\\  
f(x) &\rightarrow \text{Continuous on All }(x,y) \\\\  
g(t) &\rightarrow \text{Continuous on All }'t' \\\\  
h(x,y) = g(f(x,y)) &\rightarrow \text{Continuous on everywhere}
\end{align}$$

##### EX4
$$\begin{align}
f(x,y) &= x-2y+3 \\\\  
g(t) &= \sqrt{t} + \frac{1}{t} \\\\  
f(x,y) &\rightarrow \text{Continuous on All }(x,y) \\\\  
g(t) &\rightarrow \text{Continuous on }\\{t|t > 0\\} \\\\  
h(x,y) = g(f(x,y)) &\rightarrow \text{Continuous on }\\{(x,y)|x-2y > -3\\}
\end{align}$$

### Squeeze theorem
$$\begin{align}
&\lim_{(x,y) \to (0,0)}\frac{5x^2y}{x^2+y^2} \\\\  
\frac{5x^2y}{x^2+y^2} &\rightarrow \left|\frac{5x^2y}{x^2+y^2}\right| = \frac{5x^2|y|}{x^2+y^2}\\\\  
\frac{5x^2}{x^2} = 5 &\rightarrow \frac{5x^2}{x^2+y^2} \le 5 \rightarrow \frac{5x^2|y|}{x^2+y^2} \le 5|y| \\\\  
0 \le \frac{5x^2|y|}{x^2+y^2} \le 5|y| &\rightarrow \lim\_{(x,y)\to (0,0)} 0 = 0 \le \lim\_{(x,y)\to (0,0)}\frac{5x^2|y|}{x^2+y^2} \le \lim\_{(x,y) \to (0,0)}5|y|
\end{align}$$