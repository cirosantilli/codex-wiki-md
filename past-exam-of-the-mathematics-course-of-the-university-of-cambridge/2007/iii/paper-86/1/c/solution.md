<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Dirichlet spectral formula for half-line constant drift](../../../../../../dirichlet-spectral-formula-for-half-line-constant-drift.md) can be checked both spectrally and through its [heat kernel](../../../../../../heat-kernel.md). For $x>0,t>0$, each factor $e^{ikx-\omega t}$ solves the differential equation, since $-\omega=(ik)^2+\alpha ik$. Differentiating the upper limit in $G_0$ introduces only

$$
-\frac{g_0(t)}{2\pi}\int_L e^{ikx}(2ik+\alpha)dk=0.
$$

This vanishes by closing upward for $x>0$, or by recognizing the polynomial Fourier multiplier as a distribution supported at $x=0$. Thus differentiation under regularized contours, followed by the smooth interior limit, proves the PDE. At $t=0$ the boundary transform vanishes and the reflected initial-data integral is zero by part (a), leaving [Fourier inversion](../../../../../../fourier-inversion-theorem.md) of $q_0$.

For a direct verification of the boundary limit, evaluate the contour integrals. Let

$$
K(s,t)=\frac1{\sqrt{4\pi t}}\exp\left[-\frac{(s+\alpha t)^2}{4t}\right].
$$

The real-axis [Gaussian Fourier transform](../../../../../../fourier-transform-of-a-gaussian.md) gives this kernel. In the reflected initial term, $e^{-i\nu(k)\xi}=e^{ik\xi+\alpha\xi}$, so a valid contour deformation gives $e^{\alpha\xi}K(x+\xi,t)$. The boundary integral gives $-(2\partial_x+\alpha)K(x,t)=xK(x,t)/t$. Consequently the same solution is

$$
\boxed{q(x,t)=\int_0^\infty\left[K(x-\xi,t)-e^{\alpha\xi}K(x+\xi,t)\right]q_0(\xi)d\xi+\int_0^t P(x,t-s)g_0(s)ds,}
$$

where

$$
P(x,u)=\frac{x}{2\sqrt\pi\,u^{3/2}}\exp\left[-\frac{(x+\alpha u)^2}{4u}\right],\qquad u>0.
$$

Interchange of the space or time integrals with the spectral integral can first be performed with cutoffs; the displayed Gaussian kernels justify their removal for the stated smooth decaying data. The possible exponential $e^{\alpha\xi}$ is compensated by Gaussian decay, so exponential decay of $q_0$ is not an extra assumption.

At $x=0$, $K(-\xi,t)=e^{\alpha\xi}K(\xi,t)$, so the initial-data contribution has zero boundary trace. The kernel $P$ is a time [approximate identity](../../../../../../approximate-identity.md) as $x\downarrow0$. Indeed it is the standard positive heat boundary kernel multiplied by $e^{-\alpha x/2-\alpha^2u/4}$. The standard kernel has total mass one on $u>0$, as the substitution $r=x/(2\sqrt u)$ shows; its mass on $u\geq\delta$ is $O(x/\sqrt\delta)$. The additional factor tends to one uniformly on sufficiently short time intervals as $x\downarrow0$, so $\int_0^t P(x,u)du\to1$ for fixed $t>0$. Continuity of $g_0$ and the vanishing tail then give

$$
\boxed{\lim_{x\downarrow0}q(x,t)=g_0(t),\qquad0<t<T.}
$$

For fixed $x>0$, the first kernel tends to a point mass at $\xi=x$, the reflected kernel is exponentially small as $t\downarrow0$, and the boundary-forcing integral is also exponentially small. This independently proves $q(x,t)\to q_0(x)$. The compatibility $q_0(0)=g_0(0)$ supplies continuity at the initial corner.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
