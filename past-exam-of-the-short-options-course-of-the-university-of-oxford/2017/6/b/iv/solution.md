<h1 id="6/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $y=\pm\sqrt{2/\pi}\sin x$, both the constraint and endpoint values hold, the extremal equation has $\lambda=1$, and direct integration gives $J[y]=1$.

For any admissible function, its derivative has [Fourier cosine series](../../../../../fourier-cosine-series.md) coefficients $na_n$ and zero constant coefficient. This follows by [integration by parts](../../../../../integration-by-parts.md): $\int_0^\pi y'\cos(nx)dx=n\int_0^\pi y\sin(nx)dx$, and $\int_0^\pi y'=0$. Thus the [Parseval identity](../../../../../parseval-identity.md) gives

$$
J[y]=\frac\pi2\sum_{n\geq1}n^2a_n^2
\geq\frac\pi2\sum_{n\geq1}a_n^2=1.
$$

For finite sums the same identity follows directly from the cosine product formula in the hint; the $L^2$ identity justifies the general case. Equality holds only if $a_n=0$ for all $n\geq2$, and normalization then fixes $a_1=\pm\sqrt{2/\pi}$. Therefore

$$
\boxed{J_{\min}=1,\qquad y_{\min}(x)=\pm\sqrt{\frac2\pi}\sin x.}
$$

This is the [minimum Dirichlet energy at fixed L2 norm on an interval](../../../../../minimum-dirichlet-energy-at-fixed-l2-norm-on-an-interval.md), equivalently the sharp [Wirtinger inequality](../../../../../wirtinger-inequality.md) for this interval.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
