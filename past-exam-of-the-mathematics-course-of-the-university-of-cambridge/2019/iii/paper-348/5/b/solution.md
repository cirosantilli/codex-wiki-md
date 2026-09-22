<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $D=\operatorname{diam}(X)<\infty$, and first suppose $1\leq p\leq q<\infty$. On any [transport plan](../../../../../../transport-plan.md) $\pi$, which has total mass one, the [Holder inequality](../../../../../../holder-inequality.md) gives

$$
\left(\int|x-y|^p\,d\pi\right)^{1/p}
\leq\left(\int|x-y|^q\,d\pi\right)^{1/q}.
$$

Also, $|x-y|\leq D$ gives

$$
\int|x-y|^q\,d\pi\leq D^{q-p}\int|x-y|^p\,d\pi.
$$

Taking infima, or using arbitrarily close competitors if an infimum is not attained, yields

$$
\boxed{W_p(\mu,\nu)\leq W_q(\mu,\nu)
\leq D^{1-p/q}W_p(\mu,\nu)^{p/q}.}
$$

For $p=q$ the two distances coincide, and if $D=0$ there is only one [probability measure](../../../../../../probability-measure.md), so the conclusion is immediate. For $D>0$ and $p<q$, the displayed bounds imply both directions of

$$
\boxed{W_p(\mu_n,\mu)\to0\quad\Longleftrightarrow\quad W_q(\mu_n,\mu)\to0.}
$$

For $q<p$, exchange the exponents. Thus all finite-order [p-Wasserstein distances](../../../../../../p-wasserstein-distance.md) induce the same convergence on a bounded subset of $\mathbb R^d$. Closedness of $X$ is not required for these estimates.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
