<h1 id="30k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $H_k$ is [previsible](../../../../../../predictable-process.md), $H_k$ is $\mathcal F_{k-1}$-measurable. The finite sum $\widehat X_n$ is therefore $\mathcal F_n$-measurable. Boundedness of $H$ and integrability of the martingale increments imply

$$
\mathbb E|\widehat X_n|<\infty.
$$

Finally,

$$
\begin{aligned}
\mathbb E[\widehat X_n-\widehat X_{n-1}\mid\mathcal F_{n-1}]
&=\mathbb E[H_n(X_n-X_{n-1})\mid\mathcal F_{n-1}]\\
&=H_n\mathbb E[X_n-X_{n-1}\mid\mathcal F_{n-1}]\\
&=0.
\end{aligned}
$$

Thus

$$
\mathbb E[\widehat X_n\mid\mathcal F_{n-1}]
=\widehat X_{n-1},
$$

so $\widehat X$ is a martingale. It is the [martingale transform](../../../../../../martingale-transform.md) of $X$ by $H$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
