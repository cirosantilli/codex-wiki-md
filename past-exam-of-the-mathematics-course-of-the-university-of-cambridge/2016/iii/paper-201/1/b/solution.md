<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [almost sure submartingale convergence theorem](../../../../../../almost-sure-submartingale-convergence-theorem.md) says that if a [submartingale](../../../../../../submartingale.md) $(Y_n)$ satisfies

$$
\sup_n\mathbb E[Y_n^+]<\infty,
$$

then there is an [integrable random variable](../../../../../../integrable-random-variable.md) $Y_\infty$ such that

$$
\boxed{Y_n\longrightarrow Y_\infty\quad\text{almost surely}.}
$$

Indeed the positive-part bound also bounds the negative parts, since $\mathbb E Y_n\geq\mathbb E Y_0$; the theorem gives a finite limit. In particular, the [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) applies to any [martingale](../../../../../../martingale-split.md) with $\sup_n\mathbb E|M_n|<\infty$.

For a nonnegative [martingale](../../../../../../martingale-split.md), $\mathbb E M_n=\mathbb E M_0$ supplies this bound automatically. Its limit obeys $\mathbb E M_\infty\leq\mathbb E M_0$ by the [Fatou lemma](../../../../../../fatou-s-lemma.md). **[Almost sure convergence](../../../../../../almost-sure-convergence.md) alone need not preserve the [expectation](../../../../../../expected-value.md) or give convergence in L1.** [Uniform integrability](../../../../../../uniform-integrability.md) is the additional condition that supplies [convergence in L1](../../../../../../convergence-in-l1.md) and the identity $M_n=\mathbb E[M_\infty\mid\mathcal F_n]$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
