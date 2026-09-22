<h1 id="6h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
N(\theta)=\#\{i:X_i<\theta\}.
$$

Ignoring the immaterial choice of density values at the sample points, the [likelihood function](../../../../../../likelihood-function.md) is

$$
\boxed{
L(\theta)
=2^{-n}\left(1+\frac1\theta\right)^{N(\theta)}}.
$$

Between consecutive [order statistics](../../../../../../order-statistic.md), $N(\theta)$ is constant while $(1+1/\theta)^{N(\theta)}$ decreases with $\theta$. A maximum can therefore be moved to the left endpoint of one of these intervals. With an equivalent version using $\mathbf1_{\{x\leq\theta\}}$, the maximum is attained at a sample order statistic. Thus the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) coincides with one of $X_1,\ldots,X_n$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6H](../../6h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
