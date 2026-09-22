<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [weighted inner product](../../../../weighted-inner-product.md) $\langle f,g\rangle_w=\int_a^bw(x)\overline{f(x)}g(x)\,dx$ with positive weight $w$. For a [self-adjoint operator](../../../../self-adjoint-operator.md) $L$ and nonzero [eigenfunction](../../../../eigenfunction.md) $Ly=\lambda y$, self-adjointness gives $\lambda\langle y,y\rangle_w=\langle y,Ly\rangle_w=\langle Ly,y\rangle_w=\overline\lambda\langle y,y\rangle_w$. The positive norm therefore forces $\lambda$ to be real. For two [eigenfunctions](../../../../eigenfunction.md) of distinct [eigenvalues](../../../../eigenvalue.md), the same calculation gives $(\lambda_2-\lambda_1)\langle y_1,y_2\rangle_w=0$, proving their [orthogonality](../../../../orthogonal-vectors.md).

The [Chebyshev differential equation](../../../../chebyshev-differential-equation.md) takes the [Sturm-Liouville form](../../../../sturm-liouville-form.md)

$$
-\frac d{dx}\left(\sqrt{1-x^2}\,y'\right)=n^2\frac{y}{\sqrt{1-x^2}},\qquad
\boxed{p=\sqrt{1-x^2},\quad w=(1-x^2)^{-1/2},\quad q=0.}
$$

Its operator is $Ly=-(1-x^2)y''+xy'$, so $Lx=x$ as required. For $y=x^3+Bx$, direct substitution gives $Ly=9x^3+(B-6)x$. Comparing coefficients yields

$$
\boxed{y_3=x^3-\frac34x,\qquad n^2=9.}
$$

Explicitly, using $x=\cos\theta$,

$$
\langle y_1,y_3\rangle_w=\int_{-1}^1\frac{x^4-3x^2/4}{\sqrt{1-x^2}}dx=\frac{3\pi}8-\frac34\frac\pi2=0.
$$

The endpoints are singular because $p$ vanishes and $w$ diverges there. The polynomial solutions use the natural condition $py'\to0$ at each end; under $x=\cos\theta$ these are the [Neumann eigenfunctions of the Chebyshev differential operator](../../../../neumann-eigenfunctions-of-the-chebyshev-differential-operator.md), proportional to $\cos(n\theta)$. They differ from the zero-value endpoint realization of the same differential expression.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
