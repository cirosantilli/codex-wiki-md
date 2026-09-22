<h1 id="26k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $S_n=\sum_{j=1}^nY_j$ for the [partial sum](../../../../../../partial-sum.md). Fix an integer $M\geq1$. The [tail-sum formula for expectation](../../../../../../tail-sum-formula-for-expectation.md), applied to the nonnegative [random variable](../../../../../../random-variable-split.md) $|Y_1|$, gives

$$
\sum_{n=1}^{\infty}\mathbb P(|Y_n|>Mn)
=\sum_{n=1}^{\infty}\mathbb P(|Y_1|>Mn)
=\infty,
$$

because $\mathbb E|Y_1|=\infty$. The events $\{|Y_n|>Mn\}$ are [independent](../../../../../../independent-random-variables.md), so the second [Borel--Cantelli lemma](../../../../../../borel-cantelli-lemmas.md) shows that $|Y_n|/n>M$ infinitely often with probability one. Taking the countable intersection over $M\in\mathbb N$ yields

$$
\limsup_{n\to\infty}\frac{|Y_n|}{n}=\infty
$$

[almost surely](../../../../../../almost-sure-convergence.md).

Now $Y_n=S_n-S_{n-1}$, and the [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\frac{|Y_n|}{n}
\leq \frac{|S_n|}{n}
+\frac{n-1}{n}\frac{|S_{n-1}|}{n-1}.
$$

If the [limit superior](../../../../../../limit-superior.md) of $|S_n|/n$ were finite, the right-hand side would have finite limit superior, contradicting the preceding conclusion. Therefore

$$
\limsup_{n\to\infty}\frac{|Y_1+\cdots+Y_n|}{n}=\infty
$$

almost surely.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26K](../../26k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
