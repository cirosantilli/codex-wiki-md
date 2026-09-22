<h1 id="26k/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose first that

$$
\mathbb E[(X_{\mu_n}-X_\nu)^2]\longrightarrow0.
$$

This is [convergence in L2](../../../../../../../convergence-in-l2.md), hence [convergence in probability](../../../../../../../convergence-in-probability.md), which implies [convergence in distribution](../../../../../../../convergence-in-distribution.md). By part (i), the respective laws are $\mu_n$ and $\nu$, so $\mu_n$ converges [weakly](../../../../../../../weak-convergence-of-probability-measures.md) to $\nu$. Part (a)(i) also gives

$$
\int_{\mathbb R}x^2\,d\mu_n(x)
=\mathbb E[X_{\mu_n}^2]
\longrightarrow
\mathbb E[X_\nu^2]
=\int_{\mathbb R}x^2\,d\nu(x).
$$

Conversely, suppose that $\mu_n$ converges weakly to $\nu$ and the displayed second moments converge. By the stated [quantile coupling for convergence in distribution](../../../../../../../quantile-coupling-for-convergence-in-distribution.md),

$$
X_{\mu_n}\longrightarrow X_\nu
\qquad\text{almost surely}.
$$

Part (i) identifies their second moments with those of the measures, so part (a)(ii) applies and gives convergence in $L^2$. Therefore

$$
\boxed{
\mathbb E[(X_{\mu_n}-X_\nu)^2]\to0
\iff
\left(\mu_n\Rightarrow\nu
\text{ and }
\int x^2\,d\mu_n\to\int x^2\,d\nu\right).}
$$

This is the [one-dimensional second-Wasserstein convergence criterion](../../../../../../../one-dimensional-second-wasserstein-convergence-criterion.md) realized by the common-quantile coupling.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [26K](../../../26k.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
