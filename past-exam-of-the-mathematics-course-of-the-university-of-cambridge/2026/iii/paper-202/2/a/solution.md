<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $(X_n)$ be [Cauchy](../../../../../../cauchy-sequence.md) in the norm

$$
\lVert X\rVert=\mathbb E\sup_{t\geq0}|X_t|.
$$

Choose a subsequence $(X_{n_k})$ for which

$$
\sum_{k=1}^{\infty}\lVert X_{n_{k+1}}-X_{n_k}\rVert<\infty.
$$

[Tonelli theorem](../../../../../../tonelli-theorem.md) implies

$$
\sum_k\sup_{t\geq0}|X_{n_{k+1}}(t)-X_{n_k}(t)|<\infty
$$

almost surely. The subsequence therefore converges uniformly on $[0,\infty)$, outside one null event, to a continuous process $X$. For each $t$, $X_t$ is the almost-sure limit of $\mathcal F_t$-measurable variables; completeness of the filtration makes the chosen version adapted. The same summable bound and [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) show that $\mathbb E\sup_t|X_t|<\infty$ and that $X_{n_k}\to X$ in norm.

Since the original sequence is Cauchy, the usual triangle argument upgrades convergence of the subsequence to $X_n\to X$ in norm. Thus the space of indistinguishability classes is a [Banach space](../../../../../../banach-space-split.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
