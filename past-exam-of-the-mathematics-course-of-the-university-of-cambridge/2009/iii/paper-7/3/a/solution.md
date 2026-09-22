<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The improper integral is assumed to have a finite limit. Fix $\lambda>1$ and put $I(U,V)=\int_U^V(\beta(x)-x)x^{-2}dx$. Convergence implies $I(X,\lambda X)\to0$ and $I(X/\lambda,X)\to0$ as $X\to\infty$. By monotonicity,

$$
I(X,\lambda X)\ge\beta(X)\int_X^{\lambda X}x^{-2}dx-\log\lambda
=(1-\lambda^{-1})\frac{\beta(X)}X-\log\lambda,
$$

and

$$
I(X/\lambda,X)\le(\lambda-1)\frac{\beta(X)}X-\log\lambda.
$$

Thus

$$
\frac{\log\lambda}{\lambda-1}\le\liminf_{X\to\infty}\frac{\beta(X)}X
\le\limsup_{X\to\infty}\frac{\beta(X)}X\le\frac{\log\lambda}{1-\lambda^{-1}}.
$$

Both outer bounds tend to one as $\lambda\downarrow1$, giving $\boxed{\beta(X)/X\to1}$. This [monotone integral Tauberian lemma](../../../../../../monotone-integral-tauberian-lemma.md) uses monotonicity to control the value at a point from integral averages on adjacent multiplicative intervals; convergence of the integral alone would not control arbitrary local spikes.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
