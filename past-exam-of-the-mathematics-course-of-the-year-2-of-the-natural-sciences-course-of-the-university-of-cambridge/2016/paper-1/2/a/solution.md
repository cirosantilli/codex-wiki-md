<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $y(x,t)=X(x)T(t)$ in the [wave equation](../../../../../wave-equation-split.md). A nonzero product obtained by [separation of variables](../../../../../separation-of-variables.md) obeys

$$
\frac{X''}{X}=\frac{T''}{c^2T}=-k^2.
$$

The fixed-end [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) require $X(0)=X(L)=0$. The zero and negative spatial [eigenvalue](../../../../../eigenvalue.md) cases produce only the trivial solution; the nontrivial [eigenfunctions](../../../../../eigenfunction.md) are

$$
X_n(x)=\sin\frac{n\pi x}{L},\qquad k_n=\frac{n\pi}{L},\qquad\omega_n=ck_n,\qquad n=1,2,\ldots.
$$

For each [normal mode](../../../../../normal-mode.md), $T_n''+\omega_n^2T_n=0$. By [superposition](../../../../../superposition-principle.md) and completeness of the [Fourier sine basis](../../../../../fourier-sine-basis.md), the general finite-energy solution has the expansion

$$
\boxed{y(x,t)=\sum_{n=1}^{\infty}\left[A_n\cos\omega_nt+B_n\sin\omega_nt\right]\sin\frac{n\pi x}{L}.}
$$

If $f(x)=y(x,0)$ and $g(x)=y_t(x,0)$, [orthogonality](../../../../../orthogonal-vectors.md) gives $A_n=(2/L)\int_0^Lf(x)\sin(k_nx)\,dx$ and $B_n=2\int_0^Lg(x)\sin(k_nx)\,dx/(L\omega_n)$. Individual products are separable; their sum is the general solution.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
