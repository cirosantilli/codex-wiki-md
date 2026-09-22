<h1 id="8b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [phase plane](../../../../../../phase-plane.md) system is $\dot x=y$, $\dot y=-cy-\sin x$. Its [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) are **$(k\pi,0)$ for every integer $k$**. At such a point the [Jacobian matrix](../../../../../../jacobian-matrix.md) and characteristic equation are

$$
J=\begin{pmatrix}0&1\\-(-1)^k&-c\end{pmatrix},\qquad r^2+cr+(-1)^k=0.
$$

For even $k$, the [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) is a **[stable focus](../../../../../../stable-spiral.md) for $0<c<2$**, with [eigenvalues](../../../../../../eigenvalue.md) $-c/2\pm i\sqrt{1-c^2/4}$; it is a **[stable node](../../../../../../stable-node.md) for $c>2$**, with two distinct negative real [eigenvalues](../../../../../../eigenvalue.md). The excluded value $c=2$ gives the repeated critical case.

For odd $k$, the [eigenvalues](../../../../../../eigenvalue.md) are $(-c\pm\sqrt{c^2+4})/2$. One is positive and one negative, so each is a **[saddle equilibrium](../../../../../../saddle-equilibrium.md) for every $c>0$**. These classifications follow from the [linearization of a dynamical system](../../../../../../linearization-of-a-dynamical-system.md), since all the relevant [eigenvalues](../../../../../../eigenvalue.md) have nonzero real part for $c>0$. The even equilibria remain hyperbolic at $c=2$ too, although their [linearization](../../../../../../linearization.md) then has a repeated eigenvalue; that critical case is excluded from the requested classification.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [8B](../../8b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
