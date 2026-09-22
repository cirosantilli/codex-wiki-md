<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A diameter-only bound also needs the normalization of a [Laplacian](../../../../../laplacian.md) stencil, beyond its coefficient signs. For example, a single interior row $L_he_p=\varepsilon(e_a-e_p)$ with $e_a=0$ allows $|L_he_p|=1$ and $|e_p|=1/\varepsilon$ on a domain of fixed diameter. Thus arbitrary rescaling of the printed coefficients rules out a universal diameter-only estimate.

For the intended normalized [Laplacian](../../../../../laplacian.md) stencil, assume $L_h1=0$ and $L_h\phi=4$ for $\phi_p=|x_p-x_0|^2$, with $x_0\in\Omega$, as holds for the standard two-dimensional central stencil. Let $D=\operatorname{diam}\Omega$. Then $0\leq\phi_p\leq D^2$. Use the [truncation error](../../../../../truncation-error.md) convention $T_p=L_hu_p-f_p$, so $L_he_p=T_p$; reversing the convention does not change the absolute-value argument.

The two functions $\psi_p^\pm=\pm e_p+(T/4)\phi_p$ satisfy $L_h\psi^\pm\geq-T+T=0$. On the prescribed boundary $e_a=0$, so their maximum boundary values are at most $TD^2/4$. Apply the [discrete maximum principle](../../../../../discrete-maximum-principle.md) from part (a), with its boundary-connectivity assumption. Since $\phi\geq0$,

$$
\boxed{E\leq\frac{D^2}{4}T.}
$$

This is the standard [quadratic-barrier error estimate for a discrete Laplacian](../../../../../quadratic-barrier-error-estimate-for-a-discrete-laplacian.md). The calculation identifies exactly the additional normalization needed for the bound intended by the question.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
