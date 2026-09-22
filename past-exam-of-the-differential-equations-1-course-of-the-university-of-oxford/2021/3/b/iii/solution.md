<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

One suitable [autonomous planar system](../../../../../autonomous-planar-system.md) is

$$
\boxed{\dot x=y^2-1,\qquad \dot y=x^2-1.}
$$

Its [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md) are exactly the four combinations $(x,y)=(\pm1,\pm1)$. Its [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J(x,y)=\begin{pmatrix}0&2y\\2x&0\end{pmatrix},\qquad \lambda^2=4xy.
$$

Thus $(-1,-1)$ and $(1,1)$ have [eigenvalues](../../../../../eigenvalue.md) $\pm2$ and are [saddle equilibria](../../../../../saddle-equilibrium.md). At the other two points the [eigenvalues](../../../../../eigenvalue.md) are $\pm2i$. To establish the nonlinear [centre equilibrium](../../../../../center-equilibrium.md) classifications, use the [first integral](../../../../../first-integral.md)

$$
H(x,y)=\frac{x^3}{3}-x-\frac{y^3}{3}+y,\qquad
\dot H=(x^2-1)(y^2-1)-(y^2-1)(x^2-1)=0.
$$

Its [Hessian matrix](../../../../../hessian-matrix.md) is $\operatorname{diag}(2x,-2y)$, a [negative-definite matrix](../../../../../negative-definite-matrix.md) at $(-1,1)$ and a [positive-definite matrix](../../../../../positive-definite-matrix.md) at $(1,-1)$. Thus each is a strict [local extremum](../../../../../local-extremum.md), and nearby [regular level sets](../../../../../regular-level-set.md) are [closed curves](../../../../../closed-curve.md) supporting [periodic orbits](../../../../../periodic-orbit.md), by the [planar first integral criterion for a centre](../../../../../planar-first-integral-criterion-for-a-centre.md).

Immediately to the right of $(-1,1)$, the [vector field](../../../../../vector-field.md) points down because $x^2-1<0$, so that centre is clockwise. Immediately to the right of $(1,-1)$ it points up because $x^2-1>0$, so that centre is counterclockwise. This verifies both the nonlinear classifications and the prescribed orientations, with exactly four [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
