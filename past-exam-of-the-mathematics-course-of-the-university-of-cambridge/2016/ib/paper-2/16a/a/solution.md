<h1 id="16a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md) select the spatial [eigenfunctions](../../../../../../eigenfunction.md) $\cos nx$, $n=0,1,\ldots$, of the separated [wave equation](../../../../../../wave-equation-split.md). Indeed separation gives $X''+\lambda X=0$ with $X'(0)=X'(\pi)=0$. Integration by parts gives $\lambda\int X^2=\int X'^2\ge0$. The zero value yields the constant mode; for positive $\lambda$, the first boundary condition removes the sine term and the second requires $\sqrt\lambda=n\in\mathbb N$. For $n>0$, the temporal factor is $\cos nct$: the sine factor vanishes because the initial velocity is zero. The zero mode has constant displacement, with no term linear in time for the same reason.

The constant [Fourier cosine series](../../../../../../fourier-cosine-series.md) coefficient is the mean $\pi^{-1}\int_0^\pi bx\,dx=b\pi/2$. The remaining coefficients are

$$
a_n=\frac{2b}{\pi}\int_0^\pi x\cos nx\,dx
=\frac{2b}{\pi n^2}\bigl((-1)^n-1\bigr).
$$

Only odd modes survive. Thus **the displacement is**

$$
\boxed{y(x,t)=\frac{b\pi}{2}-\frac{4b}{\pi}\sum_{k=0}^{\infty}
\frac{\cos((2k+1)x)\cos((2k+1)ct)}{(2k+1)^2}.}
$$

The series for displacement converges absolutely and uniformly. The initial velocity is zero in the finite-energy sense, and the initial displacement is $bx$. There is an endpoint compatibility qualification: when $b\ne0$, the initial slope does not satisfy the [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md) at $t=0$. The answer is therefore a finite-energy [weak solution](../../../../../../weak-solution.md), piecewise classical between the propagating corners, rather than a globally twice continuously differentiable solution up to the initial endpoints. The mode expansion implements reflection at those endpoints.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16A](../../16a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
