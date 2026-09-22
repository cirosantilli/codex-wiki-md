<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First expand the variational integrand:

$$
\mathcal L=f'^2+(3f-x)f'+2f^2-2x^2.
$$

Its needed partial [derivatives](../../../../../derivative.md) are $\mathcal L_f=3f'+4f$ and $\mathcal L_{f'}=2f'+3f-x$. The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is therefore

$$
\frac d{dx}(2f'+3f-x)-(3f'+4f)=0,\qquad\boxed{f''-2f=\frac12.}
$$

The general solution is $f=A\cosh(\sqrt2x)+B\sinh(\sqrt2x)-1/4$. Subtracting the two endpoint equations gives $B=0$; adding them gives $A=1/[4\cosh\sqrt2]$. Hence

$$
\boxed{f(x)=\frac14\left[\frac{\cosh(\sqrt2x)}{\cosh\sqrt2}-1\right].}
$$

This is the unique stationary solution. It is also the unique [global minimizer](../../../../../global-minimizer.md): after discarding the fixed [boundary terms](../../../../../boundary-term.md), [integration by parts](../../../../../integration-by-parts.md) rewrites $I$ as $\int_{-1}^1[f'^2+2f^2+f-2x^2]dx$. For an endpoint-zero [variation](../../../../../variation.md) $\eta$, the linear part vanishes at the displayed solution and

$$
I[f+\eta]-I[f]=\int_{-1}^1[\eta'^2+2\eta^2]dx\geq0,
$$

with equality only for $\eta=0$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [9](../../9.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
