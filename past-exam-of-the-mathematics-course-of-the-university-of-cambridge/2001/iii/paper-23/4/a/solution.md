<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a continuous strictly increasing [cumulative distribution function](../../../../../../cumulative-distribution-function.md) $F$ and a [uniform distribution](../../../../../../continuous-uniform-distribution.md) $U$ on $(0,1)$, monotonicity gives

$$
\Pr(F^{-1}(U)\le y)=\Pr(U\le F(y))=F(y).
$$

Thus **each transformed draw has distribution function $F$**. This is [inverse transform sampling](../../../../../../inverse-transform-sampling.md). The conclusion extends to discontinuous or non-strictly increasing $F$ by its [quantile function](../../../../../../quantile-function.md) $Q(u)=\inf\{x:F(x)\ge u\}$: right continuity gives $Q(u)\le y$ exactly when $u\le F(y)$. Independent uniforms produce independent transformed draws, but marginal uniformity alone does not establish [independence](../../../../../../independent-random-variables.md).

If “uniformly distributed sequence” instead means deterministic equidistribution, the empirical fraction of $\eta_i\le y$ is the empirical fraction of $\xi_i\le F(y)$ and tends to $F(y)$. That is an empirical distribution statement, not a claim that the deterministic sequence consists of independent [random variables](../../../../../../random-variable-split.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
