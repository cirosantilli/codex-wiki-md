<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At a [fixed point](../../../../fixed-point.md), the first equation gives $y=0$, the second then gives $x=0$, and the third gives $z=-\mu$. Thus there is exactly one [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) for every real $\mu$:

$$
\boxed{(x,y,z)=(0,0,-\mu).}
$$

The [Jacobian matrix](../../../../jacobian-matrix.md) there is

$$
J=\begin{pmatrix}0&1&0\\-1&5\epsilon\mu&0\\0&0&-1\end{pmatrix},\qquad
\det(\lambda I-J)=(\lambda+1)(\lambda^2-5\epsilon\mu\lambda+1).
$$

One [eigenvalue](../../../../eigenvalue.md) is $-1$. The other two have product one and sum $5\epsilon\mu$. For $\mu<0$ their real parts are negative, so the [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) is [asymptotically stable](../../../../asymptotic-stability.md); for $\mu>0$ both real parts are positive, leaving two unstable directions and one stable direction. At $\mu=0$ the [eigenvalues](../../../../eigenvalue.md) are $-1,i,-i$, with

$$
\left.\frac{d}{d\mu}\operatorname{Re}\lambda_\pm\right|_{\mu=0}=\frac{5\epsilon}{2}>0.
$$

Therefore **the only local [bifurcation](../../../../bifurcation.md) of this [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) is a [Hopf bifurcation](../../../../hopf-bifurcation.md) at $\mu=0$**. A repeated real [eigenvalue](../../../../eigenvalue.md) away from zero does not itself cause a [bifurcation](../../../../bifurcation.md): the [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) remains [hyperbolic](../../../../hyperbolic-equilibrium-point.md) there.

The cubic [centre manifold](../../../../center-manifold.md) calculation below gives the [Hopf normal form](../../../../hopf-normal-form.md) radial coefficient $-9\epsilon/8<0$, so this is a [supercritical Hopf bifurcation](../../../../supercritical-hopf-bifurcation.md). Small attracting [periodic orbits](../../../../periodic-orbit.md) occur on the $\mu>0$ side. In particular, at $\mu=0$ the leading cubic radial drift is inward, although [linear stability](../../../../linear-stability.md) alone cannot decide that boundary case.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the nonlinear systems course of the University of Oxford](../../../split.md)
5. [Nonlinear systems course of the University of Oxford](../../../../nonlinear-systems-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
