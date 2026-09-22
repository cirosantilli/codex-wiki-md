<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [martingale](../../../../../../martingale-split.md) property gives $\mathbb E[X_n\mid\mathcal F_m]=X_m$. Both $X_m$ and $X_n$ are [square-integrable](../../../../../../square-integrable-function.md), so their product is integrable by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Using the $\mathcal F_m$-measurability of $X_m$ in [conditional expectation](../../../../../../conditional-expectation.md) gives

$$
\mathbb E[X_nX_m]=\mathbb E\!\left[X_m\mathbb E[X_n\mid\mathcal F_m]\right]=\mathbb E[X_m^2].
$$

The pull-out step for the possibly unbounded $X_m$ can be justified by first truncating it, then passing to the limit in the [L2 norm](../../../../../../l2-norm.md) and using the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Expanding the square now yields

$$
\boxed{\mathbb E[(X_n-X_m)^2]=\mathbb E[X_n^2]-\mathbb E[X_m^2]\qquad(m\leq n).}
$$

The left side is nonnegative. Thus $a_n=\mathbb E[X_n^2]$ is nondecreasing and bounded above by $M$, and so $a_n\to a\leq M$. For $m\leq n$,

$$
\|X_n-X_m\|_2^2=a_n-a_m\leq a-a_m\longrightarrow0.
$$

By symmetry of the [norm](../../../../../../norm.md) difference this proves that $(X_n)$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md) in the [L2 space](../../../../../../l2-space-is-a-hilbert-space.md). The completeness established in part (a) gives an $X_\infty\in L^2$ with

$$
\boxed{X_n\longrightarrow X_\infty\text{ in }L^2.}
$$

This is the [L2-bounded martingale convergence theorem](../../../../../../l2-bounded-martingale-convergence-theorem.md), derived from [martingale-difference orthogonality](../../../../../../martingale-difference-orthogonality.md) and completeness. The same sequence also converges [almost surely](../../../../../../almost-sure-convergence.md) by part (b), since $\mathbb E|X_n|\leq\sqrt M$; uniqueness of a limit in [probability](../../../../../../probability.md) identifies that limit with this $X_\infty$.

## ↑ Ancestors (11)

1. [C](../c.md)
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
