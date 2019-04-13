---
title: "Finding differentials of multivariable functions"
date: 2019-03-15T22:03:19-04:00
---

## Differentials
* $\Delta y$ Gives the total change in height from $x$ to $x + \Delta x$
* $dy$ Gives the change in height from "p" to a point on the tangent line at $ x + \Delta x$  
* $\Delta y \ne dy$ But As $\Delta x$ Gets really small($\Delta x$ to 0) then $\Delta y \approx dy$

$\Delta{y} = $ Increment  
$dy = $ Differential  
$\Delta{x} = dx,\ \Delta{y} \ne dy$  
$f\prime(x) = \frac{dy}{dx}$  
$dy = f\prime(x)dx$

### For R-3 Surface
* Given a surface from "P" to "Q" and a Tangent Plane at "p"
* $\Delta z$ is the Actual change from "P" to "Q" (x,y) to ($x + \Delta{x},\ y + \Delta{y}$)
* $dz$ is the change in height from "P" to a point on the tangent plane at ($x + \Delta{x},\ y + \Delta{y}$)

$\Delta{z} = \Delta{z_x} + \Delta{z_y}$  
$\Delta{z_x} \approx dz_x = f_xdx$  
$\Delta{z_y} \approx dz_y = f_ydy$  
$\Delta{z} \approx dz_x + dz_y = f_xdx + f_ydy$  
$\Delta{z} \approx dz = f_xdx + f_ydy$

### Example 1
Find diff of $z = ye^{x^2-y^2}$  
$f_x = 2xye^{x^2-y^2}$  
$f_y = e^{x^2-y^2} - 2y^2e^{x^2-y^2} = (1-2y^2)e^{x^2-y^2}$  
$dz = 2xye^{x^2-y^2}dx + (1-2y^2)e^{x^2-y^2}dy$

### Example 2
$f(x,y,z) = \ln(2x-y)+e^{2xz}$, Find df  
$f_x = \frac{2}{2x-y} + 2ze^{2xz}$  
$f_y = \frac{-1}{2x-y}$  
$f_z = 2xe^{2xz}$  
$df = (\frac{2}{2x-y} + 2ze^{2xz})dx - \frac{1}{2x-y}dy + 2xe^{2xz}dz$  
  
Approx  change from (2,3,0) -> (2.01,2.97,0.04)    

$df = (\frac{2}{2\cdot2 - 3} + 2\cdot0e^{2x0})(0.01) - \frac{1}{2\cdot2 - 3}(-0.03) + 2\cdot2e^{2\cdot2\cdot0}(0.04)$  
$\Delta{f} \approx 0.21$
