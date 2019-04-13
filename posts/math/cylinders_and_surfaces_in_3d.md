---
title: "Cylinders and surfaces in 3d"
date: 2019-01-04T15:33:31-05:00
---

## Cylinders
1. 어떤 방정식에서 변수가 2개만 주어졌을 경우 (주어진 변수를 통한 삼차원상의 평면과 그 평면위에서의 궤적을 알수있음)
2. 주어진 방정식에 의한 평면상의 궤적을 주어지지 않은 변수축(Axis)로 이동.
3. 이동축으로 이동하더라도 평면상의 궤적이 모양은 변하지 않음


### Example
$$z = 4 - x^2$$
$$z = -x^2 + 4$$
xz평면에 z축(Axis)로 +4만큼 이동한 $x^2$의 궤적을 y축으로 이동  

{{< geogebra id="ab22acnp" width="800" height="600" >}}

---
## Surfaces
1. 어떤 방정식에서 변수가 3개인 경우.
2. 이동축으로 이동함에 따라 궤적이 변화

### Steps
1. Surface 형태
2. 이동축과 평면축
3. 최소 두개이상의 평면상의 궤적

### Ellipsoids
$$\frac{x^2}{a^2} + \frac{y^2}{b^2} + \frac{z^2}{c^2} = 1$$
1. All positive  
2. All power '2'  
3. has constant  

#### Intercepts
표준형을 통한 교차점
$$\begin{align}x = \pm a \newline y = \pm b\newline z = \pm c\end{align}$$

#### Example
$$\begin{align}9x^2 + 4y^2 + z^2 = 36 \newline
\frac{x^2}{4} + \frac{y^2}{9} + \frac{z^2}{36} = 1 \newline
\frac{x^2}{2^2} + \frac{y^2}{3^2} + \frac{z^2}{6^2} = 1 \newline
x = \pm 2,\ y = \pm 3,\ z = \pm 6 \end{align}$$

### 1-Sheet Hyperboloid
$$\frac{x^2}{a^2} + \frac{y^2}{b^2} - \frac{z^2}{c^2} = 1$$
1. has 1 negative  
2. All power '2'  
3. has constant  

#### Notes
* Negative(-) 변수축(Axis)로 이동
* Negative 변수를 0을 대입
* $\sqrt{분모}$를 대입해서 3좌표축의 값의 궤적을 구함

#### Example
$$\begin{align}
9x^2 + 9z^2 - 4y^2 = 36 \newline\newline
\frac{x^2}{4} + \frac{z^2}{4} - \frac{y^2}{9} = 1 \newline\newline
y = 0 \implies \frac{x^2}{4} + \frac{z^2}{4} = 1 \newline
x = \pm 2,\ y = \pm 2 \newline\newline
y = \pm 3 \implies \frac{x^2}{4} + \frac{z^2}{4} = 2 \newline
\frac{x^2}{8} + \frac{z^2}{8} = 1 \newline
x = \pm 2\sqrt{2},\ y = \pm 2\sqrt{2}
\end{align}$$

### 2-sheet Hyperboloid
$$\frac{x^2}{a^2} - \frac{y^2}{b^2} - \frac{z^2}{c^2} = 1$$
1. has 1 positive

#### Notes
* Positive(+) 변수축으로 이동
* Negative(-) 두변수에 0을 대입
* Positive 변수에 분모로 약분가능한 값 대입

#### Example
$$\begin{align}
-y^2 + x^2 + 9z^2 + 9 = 0 \newline
-x^2 - 9z^2 + y^2 = 9 \newline
-\frac{x^2}{9} - z^2 + \frac{y^2}{9} = 1 \newline\newline
x = z = 0 \implies \frac{y^2}{9} = 1 \newline
y = \pm 3 \newline\newline
y = \pm 6 \implies -\frac{x^2}{9} + 4 - z^2 = 1 \newline
-\frac{x^2}{9} -z^2 = -3 \newline
\frac{x^2}{27} + \frac{z^2}{3} = 1 \newline
x = \pm 3\sqrt{3},\ y = \pm\sqrt{3}
\end{align}$$

### Cones
$$\frac{x^2}{a^2} + \frac{y^2}{b^2} - \frac{z^2}{c^2} = 0$$
1. Has one Negative  
2. All Power '2'  
3. No Constant  

#### Notes
* Negative(-) 변수축으로 이동
* Negative 변수에 0 대입해서 원점표시
* Negative 변수에 분모로 약분가능한 값 대입해서 원이나 타원의 방정식으로 변형

#### Example
$$\begin{align}
z^2 - 9x^2 - 4y^2 = 0 \newline
9x^2 + 4y^2 - z^2 = 0 \newline
z = x = y = 0 \newline
z = \pm6 \implies 9x^2 + 4y^2 = 36 \newline
\frac{x^2}{4} + \frac{y^2}{9} = 1 \newline
x = \pm2,\ z = \pm3
\end{align}$$

### Paraboloid
$$\frac{x^2}{a^2} + \frac{y^2}{b^2} = CZ$$
1. 변수 3개 그중 거듭제곱 2개  
2. 거듭제곱으로 표현된 변수는 반드시 양의 기호(Positive)

#### Notes
* 차수가 낮은 변수축으로 열린 형태 (+,-에 따라 방향 결정)
* 낮은차수 변수에 0 대입

#### Example
$$\begin{align}
z = x^2 + 4y^2 - 4 \newline
x^2 + 4y^2 = z + 4 \newline\newline
z = 0 \implies x^2 + 4y^2 = 4 \newline
\frac{x^2}{4} + y^2 = 1 \newline
x = \pm2,\ y = \pm1
\end{align}$$

### Hyperbolic Paraboloid
$$\frac{x^2}{a^2} - \frac{y^2}{b^2} = CZ$$
1. 거듭제곱으로 표현된 변수중 하나가 음의 기호

#### Notes
* 낮은차수 변수 방향축
* 양수와 음수를 낮은차수 변수에 대입(쌍곡선에서의 대칭축의 변화)

#### Example
$$\begin{align}
x^2 - y^2 - z = 0 \newline
x^2 - y^2 = z \newline\newline
z = 1 \implies x^2 - y^2 = 1 \newline\newline
z = -1 \implies y^2 - x^2 = 1 
\end{align}$$

{{< geogebra id="spzcwtr2" width="800" height="600" >}}