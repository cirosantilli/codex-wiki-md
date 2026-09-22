<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $Y=\mathbb E[X\mid\mathcal G]$. The [conditional expectation](../../../../../../conditional-expectation.md) is an $L^2$ contraction by the [conditional Jensen inequality](../../../../../../conditional-jensen-inequality.md), so $X,Y$ are square-integrable. The defining integral identity for [conditional expectation](../../../../../../conditional-expectation.md), first with bounded [measurable](../../../../../../measurability.md) truncations of $Y$ and then with their $L^2$ limit, gives

$$
\mathbb E[XY]=\mathbb E[Y\mathbb E[X\mid\mathcal G]]=\mathbb E[Y^2].
$$

For clarity, if $Y^{(K)}=\max(-K,\min(Y,K))$, then $\mathbb E[XY^{(K)}]=\mathbb E[YY^{(K)}]$, and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) permits the limit $K\to\infty$. Expanding the square now proves the [equality case for conditional second moments](../../../../../../equality-case-for-conditional-second-moments.md):

$$
\mathbb E[(X-Y)^2]=\mathbb E[X^2]-\mathbb E[Y^2]=0.
$$

A nonnegative [random variable](../../../../../../random-variable-split.md) of zero [expected value](../../../../../../expected-value.md) vanishes [almost surely](../../../../../../almost-sure-convergence.md). Therefore $\boxed{X=Y\text{ almost surely}.}$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
