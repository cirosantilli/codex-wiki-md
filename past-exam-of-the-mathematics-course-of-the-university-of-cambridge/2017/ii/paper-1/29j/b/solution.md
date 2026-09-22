<h1 id="29j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Inductively, $X_0,\ldots,X_n$ are [functions](../../../../../../function-split.md) of $\Delta_0,\ldots,\Delta_n$, so $\mathcal F_n\subseteq\sigma(\Delta_0,\ldots,\Delta_n)$. The average $f_n(X_0,\ldots,X_n)$ is therefore $\mathcal F_n$-measurable and independent of $\Delta_{n+1}$. If $X_0,\ldots,X_n$ are integrable, then

$$
\mathbb E|f_n|\le\frac1{n+1}\sum_{j=0}^n\mathbb E|X_j|<\infty,
\quad
\mathbb E|\Delta_{n+1}f_n|=\mathbb E|\Delta_{n+1}|\,\mathbb E|f_n|<\infty.
$$

Starting with $X_0=\Delta_0$, induction proves integrability of every $X_n$. Adaptation holds by definition of the natural [filtration](../../../../../../filtration-probability-theory.md). [Independence](../../../../../../independent-random-variables.md) and zero mean now legitimately give

$$
\mathbb E[X_{n+1}\mid\mathcal F_n]
=X_n+f_n\mathbb E[\Delta_{n+1}\mid\mathcal F_n]=X_n.
$$

Hence **the process is a [martingale](../../../../../../martingale-split.md)**. Only first moments are used; no second-moment or boundedness assumption on the increments is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29J](../../29j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
