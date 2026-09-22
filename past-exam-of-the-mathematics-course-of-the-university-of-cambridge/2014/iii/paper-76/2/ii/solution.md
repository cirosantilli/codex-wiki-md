<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

To find the [threefold phase-locked equilibria](../../../../../../threefold-phase-locked-equilibria.md), write $C=Re^{i\theta}$ with $R>0$; separating real and imaginary parts gives

$$
\boxed{R_T=R(\mu-R^2)+R^2\cos3\theta,\qquad
\theta_T=-\omega-R\sin3\theta.}
$$

A steady state satisfies

$$
\cos3\theta_0=\frac{R_0^2-\mu}{R_0},\qquad
\sin3\theta_0=-\frac{\omega}{R_0},
$$

so

$$
\boxed{(\mu-R_0^2)^2+\omega^2=R_0^2.}
$$

Writing $y=R_0^2$ and $D=1+4\mu-4\omega^2$, the amplitude branches are

$$
\boxed{y_\pm=\mu+\frac12\pm\frac12\sqrt D.}
$$

There are two distinct positive roots for **$\mu>\omega^2-1/4$**, except at $(\mu,\omega)=(0,0)$, where $y_-=0$ and only the upper root is nonzero. Indeed their sum is positive in this range and their product is $\mu^2+\omega^2$. Below the fold condition there are none. At equality, there is one positive repeated root $y=\omega^2+1/4$, the [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md) limit.

For each positive amplitude, the sine and cosine determine $3\theta_0$ modulo $2\pi$, giving three phases separated by $2\pi/3$. Thus the source's “two states” means **two amplitude branches modulo the threefold spatial symmetry**. Generically there are six nonzero complex equilibria, three on each branch, not literally two.

The polar [Jacobian matrix](../../../../../../jacobian-matrix.md) at an equilibrium is

$$
J=\begin{pmatrix}
-\mu-y&3\omega R_0\\
\omega/R_0&3\mu-3y
\end{pmatrix},
\quad
\operatorname{tr}J=2\mu-4y,\quad
\det J=3y(2y-2\mu-1).
$$

On the lower branch, $\det J=-3y_-\sqrt D<0$, so it is a [saddle equilibrium](../../../../../../saddle-equilibrium.md) and unstable. On the upper branch, $\det J=3y_+\sqrt D>0$ and

$$
\operatorname{tr}J=-2(\mu+1+\sqrt D)<0,
$$

because existence implies $\mu>-1/4$. Therefore **every upper-branch equilibrium is [asymptotically stable](../../../../../../asymptotic-stability.md), and every lower-branch equilibrium is a [saddle equilibrium](../../../../../../saddle-equilibrium.md)**, away from the degenerate endpoints. The [eigenvalues](../../../../../../eigenvalue.md) are unchanged by the smooth polar coordinate transformation at $R_0>0$. The origin, not covered by those coordinates, has [eigenvalues](../../../../../../eigenvalue.md) $\mu\pm i\omega$ and is stable for $\mu<0$ and unstable for $\mu>0$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
