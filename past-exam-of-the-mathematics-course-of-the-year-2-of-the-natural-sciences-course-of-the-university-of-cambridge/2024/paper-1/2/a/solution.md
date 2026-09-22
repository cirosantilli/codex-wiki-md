<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [separation of variables](../../../../../separation-of-variables.md) with $\rho(x,t)=X(x)T(t)$ and temporal factor $T=e^{-\lambda t}$. The spatial [eigenvalue](../../../../../eigenvalue.md) equation is

$$
-DX''-\gamma X=\lambda X,\qquad X(0)=X(L)=0.
$$

The nontrivial solutions of these [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) are sine [eigenfunctions](../../../../../eigenfunction.md). Normalizing in the usual [inner product](../../../../../inner-product-split.md) on $(0,L)$ gives

$$
\boxed{\psi_n(x)=\sqrt{\frac2L}\sin\frac{n\pi x}{L},\qquad\lambda_n=D\left(\frac{n\pi}{L}\right)^2-\gamma,\qquad n=1,2,\ldots,}
$$

with $\int_0^L\psi_n\psi_m\,dx=\delta_{nm}$. The [superposition principle](../../../../../superposition-principle.md) and the [Fourier sine series](../../../../../fourier-sine-series.md) then give

$$
\boxed{\rho(x,t)=\sum_{n=1}^{\infty}a_n\sqrt{\frac2L}\sin\frac{n\pi x}{L}\exp\left[\left(\gamma-\frac{Dn^2\pi^2}{L^2}\right)t\right].}
$$

The constants are the initial-data coefficients $a_n=\int_0^L\rho(x,0)\psi_n(x)\,dx$. Here physical diffusion means $D>0$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
