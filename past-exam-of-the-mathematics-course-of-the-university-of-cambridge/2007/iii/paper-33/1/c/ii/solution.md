<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $Z_n=\mathbb E[X_\infty\mid\mathcal F_n]$. It is a [conditional-expectation martingale](../../../../../../../conditional-expectation-martingale.md). We justify why its limit is $X_\infty$, rather than just quoting convergence to an unspecified random variable.

First the family is [uniformly integrable](../../../../../../../uniform-integrability.md). For $A=\{Z_n>K\}\in\mathcal F_n$, nonnegativity and the [conditional expectation](../../../../../../../conditional-expectation.md) identity give

$$
\begin{aligned}
\mathbb E[Z_n\mathbf1_A]
&=\mathbb E[X_\infty\mathbf1_A]\\
&\leq\mathbb E[X_\infty\mathbf1_{\{X_\infty>K/2\}}]+\frac K2\mathbb P(A)
\leq\mathbb E[X_\infty\mathbf1_{\{X_\infty>K/2\}}]+\frac12\mathbb E[Z_n\mathbf1_A].
\end{aligned}
$$

Thus its tail [expectations](../../../../../../../expected-value.md) are at most twice the integrable tail of $X_\infty$, uniformly in $n$. The [uniformly integrable martingale convergence theorem](../../../../../../../uniformly-integrable-martingale-convergence-theorem.md) gives a limit $Z$ almost surely and in $L^1$. For any $A\in\mathcal F_m$ and $n\geq m$,

$$
\mathbb E[Z_n\mathbf1_A]=\mathbb E[X_\infty\mathbf1_A].
$$

Pass to the $L^1$ limit and extend from $\mathcal A$ to all Borel sets by the [Monotone class theorem](../../../../../../../monotone-class-theorem.md). The equality of these integrals forces $Z=X_\infty$ almost surely. Combining this with the preceding convergence of $X_n$ proves

$$
\boxed{Y_n=X_n-Z_n\longrightarrow0\quad\lambda\text{-almost surely}.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
