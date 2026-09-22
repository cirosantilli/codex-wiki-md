<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the ideal transverse-motion model of the question: constant [tension](../../../../../../tension.md), small slopes, no bending stiffness, and no transverse body-force term. On a short segment away from $x=0$, the vertical components of the endpoint tensions are, to first order in $y_x$, $Ty_x(x+\Delta x,t)$ and $-Ty_x(x,t)$. Its mass is $\rho\Delta x$, since $\rho$ is [linear mass density](../../../../../../linear-mass-density.md). [Newton's second law](../../../../../../newton-s-second-law.md) gives

$$
\rho\Delta x\,y_{tt}=T\bigl[y_x(x+\Delta x,t)-y_x(x,t)\bigr].
$$

Dividing by $\Delta x$ and taking its limit proves the [wave equation on a string](../../../../../../wave-equation-on-a-string.md) on each side of the mass:

$$
\boxed{y_{tt}=c^2y_{xx},\qquad c^2=\frac T\rho,\qquad -\ell<x<0\text{ or }0<x<\ell.}
$$

The string on the right pulls the [point mass](../../../../../../point-mass.md) with vertical component $Ty_x(0^+,t)$, while the string on the left contributes $-Ty_x(0^-,t)$. Hence

$$
\boxed{m\ddot Y(t)=T\bigl[y_x(0^+,t)-y_x(0^-,t)\bigr].}
$$

The fixed supports and attachment impose the [boundary conditions](../../../../../../boundary-condition.md)

$$
\boxed{y(-\ell,t)=y(\ell,t)=0,\qquad y(0^-,t)=y(0^+,t)=Y(t).}
$$

Together with the mass equation, these are the endpoint and matching conditions. The slope can jump at $x=0$: the jump supplies the mass's vertical [acceleration](../../../../../../acceleration.md). Requiring the slope to be continuous would incorrectly remove its dynamics.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
