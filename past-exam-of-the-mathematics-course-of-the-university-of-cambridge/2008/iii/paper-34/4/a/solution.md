<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $S_0=0$ and take $\mathcal F_0$ to be the trivial [sigma-algebra](../../../../../../sigma-algebra.md). Each $S_n$ is measurable with respect to the [natural filtration](../../../../../../natural-filtration.md) $\mathcal F_n=\sigma(X_1,\ldots,X_n)$, and

$$
\mathbb E|S_n|\leq\sum_{i=1}^n\mathbb E|X_i|<\infty.
$$

Independence of $X_{n+1}$ from $\mathcal F_n$ makes its [conditional expectation](../../../../../../conditional-expectation.md) equal to its [expected value](../../../../../../expected-value.md), which is zero. Hence

$$
\mathbb E[S_{n+1}\mid\mathcal F_n]
=S_n+\mathbb E[X_{n+1}\mid\mathcal F_n]
=S_n+\mathbb E X_{n+1}=S_n.
$$

The measurability, integrability and [conditional expectation](../../../../../../conditional-expectation.md) conditions are all verified, so $\boxed{(S_n)\text{ is a martingale for }(\mathcal F_n).}$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
