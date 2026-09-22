<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [norm](../../../../norm.md) on a [complex vector space](../../../../complex-vector-space.md) is a map $\|\cdot\|:X\to[0,\infty)$ that vanishes only at zero, satisfies $\|\lambda x\|=|\lambda|\|x\|$, and obeys the [triangle inequality](../../../../triangle-inequality.md). The space is Banach when every [Cauchy sequence](../../../../cauchy-sequence.md) in the resulting [metric](../../../../metric.md) converges in $X$.

If $X$ is Banach and $\sum_j\|x_j\|<\infty$, the estimate $\|\sum_{j=m}^nx_j\|\leq\sum_{j=m}^n\|x_j\|$ shows that its [partial sums](../../../../partial-sum.md) are Cauchy, hence converge. Conversely let every such [series](../../../../series-mathematics.md) converge and take a [Cauchy sequence](../../../../cauchy-sequence.md) $(y_n)$. Choose a subsequence with $\|y_{n_{k+1}}-y_{n_k}\|<2^{-k}$. The [series](../../../../series-mathematics.md) consisting of $y_{n_1}$ followed by these successive differences is absolutely summable in [norm](../../../../norm.md), so converges by hypothesis; its [partial sums](../../../../partial-sum.md) are exactly this subsequence. A [Cauchy sequence](../../../../cauchy-sequence.md) with a convergent subsequence converges to the same limit, proving **the [absolute-series criterion for completeness](../../../../absolute-series-criterion-for-completeness.md)**.

On the [absolutely summable sequence space](../../../../absolutely-summable-sequence-space.md) $\ell^1$, coordinatewise addition and scalar multiplication preserve membership, and summing the scalar [triangle inequality](../../../../triangle-inequality.md) verifies its [norm](../../../../norm.md) axioms. To prove [completeness](../../../../completeness.md) using the criterion, let $x^{(k)}=(x_j^{(k)})\in\ell^1$ with $\sum_k\|x^{(k)}\|_1<\infty$. For each $j$ the sum $x_j=\sum_kx_j^{(k)}$ converges absolutely, and the permitted interchange of nonnegative double sums gives

$$
\sum_j|x_j|\leq\sum_j\sum_k|x_j^{(k)}|=\sum_k\|x^{(k)}\|_1<\infty.
$$

Thus $x\in\ell^1$. Moreover

$$
\left\|x-\sum_{k=1}^Nx^{(k)}\right\|_1\leq\sum_{k>N}\|x^{(k)}\|_1\to0.
$$

Every absolutely [norm](../../../../norm.md)-summable [series](../../../../series-mathematics.md) therefore converges in $\ell^1$, proving **$\ell^1$ is a [Banach space](../../../../banach-space-split.md)**.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
