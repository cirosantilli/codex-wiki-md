<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $(X_k)_{k=0}^n$ be a nonnegative [submartingale](../../../../../../submartingale.md) and assume $X_n\in L^p$. Set $X^*=\max_{0\leq k\leq n}X_k$. For $a>0$, let $A_k$ be the event that $k$ is the first index with $X_k>a$. These events are disjoint, $A_k\in\mathcal F_k$, and their union is $\{X^*>a\}$.

The [submartingale](../../../../../../submartingale.md) property gives $\mathbb E[X_n\mid\mathcal F_k]\geq X_k$. Hence

$$
a\mathbb P\{X^*>a\}\leq\sum_k\mathbb E[X_k1_{A_k}]\leq\sum_k\mathbb E[X_n1_{A_k}]=\mathbb E[X_n;X^*>a].
$$

Thus part (ii) applies on the probability space with $F=X^*$ and $g=X_n$, giving the [Doob Lp maximal inequality](../../../../../../doob-lp-maximal-inequality.md)

$$
\boxed{\mathbb E(X^*)^p\leq q^p\mathbb E X_n^p}.
$$

The same split at $a/2$ makes $X^*/2$ satisfy part (i), recovering the preliminary constant $2^p q$. Probability spaces automatically have finite superlevel measures. For a right-continuous nonnegative [submartingale](../../../../../../submartingale.md) on $[0,T]$, apply these finite-time bounds to increasing finite grids containing $T$ and a dense set of times; right continuity and [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) extend the estimate to $\sup_{t\leq T}X_t$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
