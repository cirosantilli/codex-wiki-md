<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [separation of variables](../../../../../separation-of-variables.md) in the form $u=X(x)T(t)$, with $T'/T=X''/X=-\lambda$. Then $T=e^{-\lambda t}$ and the spatial [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) is

$$
-X''=\lambda X,\qquad X'(0)=X(0),\qquad X'(1)=X(1).
$$

These real separated [Robin boundary conditions](../../../../../robin-boundary-condition.md) give a [self-adjoint differential operator](../../../../../self-adjoint-differential-operator.md), so the [eigenvalues](../../../../../eigenvalue.md) are real. All three sign cases must be considered.

If $\lambda=\mu^2>0$, write $X=A\cos\mu x+B\sin\mu x$. The first condition gives $B=A/\mu$, while the second reduces to

$$
-A\left(\mu+\frac1\mu\right)\sin\mu=0.
$$

Thus $\mu=n\pi$, and scaling the [eigenfunction](../../../../../eigenfunction.md) gives $V_n=n\pi\cos(n\pi x)+\sin(n\pi x)$.

If $\lambda=0$, then $X=A+Bx$. The first condition gives $B=A$, and the second gives $B=A+B$, so $A=B=0$; there is no zero [eigenvalue](../../../../../eigenvalue.md).

If $\lambda=-\kappa^2<0$, write $X=A\cosh\kappa x+B\sinh\kappa x$. The first condition gives $B=A/\kappa$, and the second becomes

$$
A\left(\kappa-\frac1\kappa\right)\sinh\kappa=0.
$$

Hence $\kappa=1$, giving the single negative [eigenvalue](../../../../../eigenvalue.md) $-1$ and spatial [eigenfunction](../../../../../eigenfunction.md) $e^x$. Completeness of this regular [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) now gives

$$
\boxed{u(x,t)=c_0e^{t+x}+\sum_{n=1}^{\infty}c_ne^{-n^2\pi^2t}\left[n\pi\cos(n\pi x)+\sin(n\pi x)\right].}
$$

This is [Robin diffusion with a growing mode](../../../../../robin-diffusion-with-a-growing-mode.md). The growth is compatible with the stated conditions: they prescribe the same coordinate [derivative](../../../../../derivative.md) at both ends, not identical dissipative outward-normal conditions.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
