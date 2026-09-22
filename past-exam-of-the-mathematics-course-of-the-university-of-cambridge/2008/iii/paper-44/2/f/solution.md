<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Multiplying the likelihood in part (d) by the [Haldane prior](../../../../../../haldane-prior.md) gives $p(\phi\mid y)\propto\phi^{s-1}(1-\phi)^{n-1}$. Consequently

$$
\boxed{\phi\mid y\sim\operatorname{Beta}(s,n),\qquad s=\sum_i y_i>0.}
$$

For at least one hospital, $n>0$, this posterior is proper exactly when $s>0$. If every count is zero, the kernel diverges at $\phi=0$ and does not define a [posterior distribution](../../../../../../bayesian-posterior.md); the [improper prior](../../../../../../improper-prior.md) cannot then be used for the subsequent expectation.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
