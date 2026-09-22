<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $X,Y$ be [prey](../../../../../prey.md) and [predator](../../../../../predator.md) abundances. With constant positive demographic and [predation](../../../../../predation.md) coefficients, the [Lotka-Volterra equations](../../../../../lotka-volterra-equations.md) are

$$
\dot X=X(\alpha-\beta Y),\qquad
\dot Y=Y(\delta X-\gamma).
$$

Their positive [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) is $X_* =\gamma/\delta$, $Y_* =\alpha/\beta$. Its [Jacobian matrix](../../../../../jacobian-matrix.md) and [eigenvalues](../../../../../eigenvalue.md) are

$$
\boxed{J_*=
\begin{pmatrix}0&-\beta\gamma/\delta\\\delta\alpha/\beta&0\end{pmatrix},
\qquad \lambda_\pm=\pm i\sqrt{\alpha\gamma}.}
$$

The linearized populations oscillate with period $2\pi/\sqrt{\alpha\gamma}$, with the [predator](../../../../../predator.md) peak following the [prey](../../../../../prey.md) peak. This is a [center equilibrium](../../../../../center-equilibrium.md), not an attracting [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md). The conclusion is supported beyond [linearization](../../../../../linearization.md) by the [Logarithmic first integral of the Lotka-Volterra equations](../../../../../logarithmic-first-integral-of-the-lotka-volterra-equations.md): in these units one may use

$$
V=\delta X-\gamma\log X+\beta Y-\alpha\log Y.
$$

Direct differentiation gives $\dot V=0$. Its [Hessian matrix](../../../../../hessian-matrix.md) is a [positive-definite matrix](../../../../../positive-definite-matrix.md) in the [positive quadrant](../../../../../positive-quadrant.md), and its minimum is at $(X_*,Y_*)$. Nearby level curves are closed [periodic orbits](../../../../../periodic-orbit.md), so there is no damping toward a preferred oscillation amplitude.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
