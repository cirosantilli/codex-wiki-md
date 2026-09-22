<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The real [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) on a [probability space](../../../../../../probability-space.md) consists of equivalence classes of [measurable functions](../../../../../../measurable-function.md) $X:\Omega\to\mathbb R$ satisfying $\mathbb E[X^2]<\infty$, where two [random variables](../../../../../../random-variable-split.md) represent the same element if they are equal [almost surely](../../../../../../almost-sure-convergence.md). Its [norm](../../../../../../norm.md) is

$$
\|X\|_2=(\mathbb E[X^2])^{1/2}.
$$

Passing to equivalence classes makes this a genuine [norm](../../../../../../norm.md): $\|X\|_2=0$ exactly when $X=0$ [almost surely](../../../../../../almost-sure-convergence.md). The [Minkowski inequality](../../../../../../minkowski-inequality.md) gives the [triangle inequality](../../../../../../triangle-inequality.md).

Let $(X_n)$ be a [Cauchy sequence](../../../../../../cauchy-sequence.md) in this [norm](../../../../../../norm.md). Choose an increasing sequence of indices $n_k$ such that

$$
\|X_{n_{k+1}}-X_{n_k}\|_2\leq2^{-k}\qquad(k\geq1).
$$

This is possible by choosing $n_k$ beyond a Cauchy threshold for tolerance $2^{-k}$. Set $D_k=X_{n_{k+1}}-X_{n_k}$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) on a [probability space](../../../../../../probability-space.md) gives $\mathbb E|D_k|\leq\|D_k\|_2$. By [Tonelli theorem](../../../../../../tonelli-theorem.md),

$$
\mathbb E\!\left[\sum_{k\geq1}|D_k|\right]
=\sum_{k\geq1}\mathbb E|D_k|\leq\sum_{k\geq1}2^{-k}<\infty.
$$

Thus the [series](../../../../../../series-mathematics.md) of absolute differences is finite [almost surely](../../../../../../almost-sure-convergence.md). Define $X=X_{n_1}+\sum_{k\geq1}D_k$ on this [probability](../../../../../../probability.md)-one [event](../../../../../../event.md), and give it the value zero on its complement. It is a [measurable function](../../../../../../measurable-function.md), and $X_{n_k}\to X$ [almost surely](../../../../../../almost-sure-convergence.md).

For $l>k$, the [Minkowski inequality](../../../../../../minkowski-inequality.md) gives

$$
\|X_{n_l}-X_{n_k}\|_2\leq\sum_{j=k}^{l-1}2^{-j}.
$$

Apply the [Fatou lemma](../../../../../../fatou-s-lemma.md) to the squared difference as $l\to\infty$. It follows that

$$
\|X-X_{n_k}\|_2\leq\sum_{j=k}^\infty2^{-j}=2^{1-k}.
$$

In particular $X-X_{n_1}\in L^2$, and therefore $X\in L^2$ by the [Minkowski inequality](../../../../../../minkowski-inequality.md). This proves [convergence in L2](../../../../../../convergence-in-l2.md) of the subsequence. To recover the entire sequence, for a prescribed $\varepsilon>0$ choose a Cauchy threshold $N$ for $\varepsilon/2$, then choose $k$ with $n_k\geq N$ and $\|X-X_{n_k}\|_2<\varepsilon/2$. For every $n\geq N$,

$$
\|X_n-X\|_2\leq\|X_n-X_{n_k}\|_2+\|X_{n_k}-X\|_2<\varepsilon.
$$

Hence $\boxed{X_n\to X\text{ in }L^2}$, proving [completeness of Lp spaces](../../../../../../completeness-of-lp-spaces.md) for $p=2$ without assuming the desired completeness in the argument.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
