<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each $n\geq1$, choose the continuous [probability density functions](../../../../../../probability-density-function.md)

$$
f(u)=1,\qquad g_n(u)=1+\frac{u-1/2}{\sqrt n}.
$$

The second is at least $1/2$ and integrates to one. Their [expected values](../../../../../../expected-value.md) differ by

$$
\psi(g_n)-\psi(f)=\frac1{\sqrt n}\int_0^1u(u-1/2)\,du=\frac1{12\sqrt n}.
$$

Writing $g_n/f=1+\Delta_n$ gives

$$
P_f\Delta_n^2=\frac1n\int_0^1(u-1/2)^2\,du=\frac1{12n}.
$$

The supplied product bound, also obtained from the [chi-squared divergence of product measures](../../../../../../chi-squared-divergence-of-product-measures.md), implies

$$
\|P_f^{(n)}-P_{g_n}^{(n)}\|_1^2
\leq\left(1+\frac1{12n}\right)^n-1
\leq e^{1/12}-1\leq\frac1{11}<1.
$$

For the final elementary estimate, compare the exponential series with the geometric series: $e^x\leq(1-x)^{-1}$ for $0\leq x<1$. Thus the overlap of the product laws is at least $1/2$. Part (b) now gives the explicit [mean-estimation minimax lower bound for continuous densities](../../../../../../mean-estimation-minimax-lower-bound-for-continuous-densities.md)

$$
\boxed{R_n^*\geq\frac14\cdot\frac1{144n}\cdot\frac12=\frac1{1152n}.}
$$

So **one may take $C=1/1152$, uniformly for all $n\geq1$**. The alternatives are allowed to depend on $n$, because the [minimax risk](../../../../../../minimax-risk.md) takes a supremum over all continuous [probability density functions](../../../../../../probability-density-function.md) separately at each sample size.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
