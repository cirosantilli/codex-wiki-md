<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [continuous semimartingale](../../../../../../continuous-semimartingale.md) $X$, its [quadratic variation](../../../../../../quadratic-variation.md) is the continuous increasing zero-starting process obtained as the limit, uniformly on compact time intervals in probability, of sums of squared increments along deterministic partitions whose mesh tends to zero. If $X=X_0+N+V$ is its continuous local-martingale/finite-variation decomposition, then $[X]=[N]$; finite-variation terms and their cross sums vanish.

Write $D=d\mathbb Q/d\mathbb P$. If $\mathbb P(E_n)\to0$, then for every $R>0$,

$$
\mathbb Q(E_n)\leq R\mathbb P(E_n)+\mathbb E_{\mathbb P}[D\mathbf1_{\{D>R\}}].
$$

First send $n$ to infinity and then $R$ to infinity. Thus convergence in probability under $\mathbb P$ implies convergence in probability under $\mathbb Q$, also for a supremum on a compact time interval. The same squared-increment sums converge under $\mathbb Q$ to the $\mathbb P$ version of $[X]$. Since $X$ is also a [semimartingale](../../../../../../semimartingale.md) under $\mathbb Q$, these sums converge to its $\mathbb Q$ [quadratic variation](../../../../../../quadratic-variation.md). Uniqueness of limits in probability gives equality at every fixed time; continuity and countably many rational times give

$$
\boxed{[X]^{\mathbb Q}=[X]^{\mathbb P}\quad\mathbb Q\text{-indistinguishably}.}
$$

Absolute continuity suffices; equivalence is not required. This is [quadratic variation under an absolutely continuous measure change](../../../../../../quadratic-variation-under-an-absolutely-continuous-measure-change.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
