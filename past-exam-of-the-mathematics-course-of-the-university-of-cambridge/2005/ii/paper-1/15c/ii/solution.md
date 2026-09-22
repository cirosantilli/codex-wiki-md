<h1 id="15c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Measure $\theta$ from the downward vertical, so the bob is at $(x+l\sin\theta,-l\cos\theta)$. Its squared speed is $\dot x^2+2l\dot x\dot\theta\cos\theta+l^2\dot\theta^2$. Up to a constant potential term, the [Lagrangian](../../../../../../lagrangian.md) is

$$
\boxed{L=\tfrac12(M+m)\dot x^2+ml\dot x\dot\theta\cos\theta+\tfrac12ml^2\dot\theta^2+mgl\cos\theta.}
$$

The [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md) give

$$
(M+m)\ddot x+ml(\ddot\theta\cos\theta-\dot\theta^2\sin\theta)=0,\qquad l\ddot\theta+\ddot x\cos\theta+g\sin\theta=0.
$$

At the downward stable equilibrium, [linearization](../../../../../../linearization.md) gives $(M+m)\ddot x+ml\ddot\theta=0$ and $l\ddot\theta+\ddot x+g\theta=0$. Eliminating $\ddot x$ yields

$$
\boxed{\omega_{\rm small}^2=\frac{(M+m)g}{Ml}.}
$$

There is also a zero-frequency translational mode because the rail fixes no preferred pivot position.

If an external force imposes $\ddot x=A$ constantly, the bob's angular equation becomes $l\ddot\theta+A\cos\theta+g\sin\theta=0$. Its stable equilibrium therefore has

$$
\boxed{\theta_*=-\arctan(A/g)\pmod{2\pi}}
$$

on the branch near the downward vertical. The displaced bob leans opposite the acceleration. The solution differing by $\pi$ is unstable, corresponding to alignment opposite the effective gravitational field in the accelerating frame.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [15C](../../15c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
