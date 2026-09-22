<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The equation as printed requires $v\ne0$; its sign does not affect the result. Seek separated solutions $\psi=X(x)T(t)$. Substitution into the [wave equation](../../../../../wave-equation-split.md) gives

$$
\frac{X''}{X}=\frac{T''}{v^2T}=-\lambda,
\qquad X''+\lambda X=0,\qquad T''+v^2\lambda T=0.
$$

The [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) impose $X'(0)=X'(\pi)=0$. Multiplying the spatial equation by $X$ and [integration by parts](../../../../../integration-by-parts.md) gives $\int_0^\pi(X')^2dx=\lambda\int_0^\pi X^2dx$, so nontrivial spatial [eigenfunctions](../../../../../eigenfunction.md) require $\lambda\geq0$.

For $\lambda=0$, $X$ is constant and $T=A_0+B_0t$. For $\lambda=k^2>0$, $X=C\cos kx+D\sin kx$. The first [boundary condition](../../../../../boundary-condition.md) gives $D=0$, and the second gives $\sin k\pi=0$. Thus $k=n$ is a positive integer and the spatial [eigenfunctions](../../../../../eigenfunction.md) are $\cos nx$. Their time dependence is $A_n\cos(nvt)+B_n\sin(nvt)$. By [superposition](../../../../../superposition-principle.md),

$$
\psi=A_0+B_0t+\sum_{n\geq1}\bigl[A_n\cos(nvt)+B_n\sin(nvt)\bigr]\cos nx.
$$

The zero initial [velocity](../../../../../velocity.md) sets $B_0=B_n=0$. The [trigonometric identity](../../../../../trigonometric-identity.md) gives the initial profile $\cos^2(x/2)=(1+\cos x)/2$, so only the constant mode and the first cosine mode occur. Hence

$$
\boxed{\psi(x,t)=\frac12+\frac12\cos x\cos(vt)}.
$$

Its spatial [derivative](../../../../../derivative.md) is $-\tfrac12\sin x\cos(vt)$, which vanishes at both boundaries, and its time [derivative](../../../../../derivative.md) vanishes initially. Thus it satisfies all the required data.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
