<h1 id="30k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because $X$ is a martingale,

$$
\mathbb E[\xi_n\mid\mathcal F_{n-1}]=0.
$$

Writing

$$
p_n=\mathbb P(\xi_n=1\mid\mathcal F_{n-1}),
$$

and using $\xi_n\in\{-1,1\}$ gives

$$
0=p_n-(1-p_n)=2p_n-1.
$$

Thus

$$
\mathbb P(\xi_n=1\mid\mathcal F_{n-1})
=\mathbb P(\xi_n=-1\mid\mathcal F_{n-1})
=\frac12.
$$

For signs $e_1,\ldots,e_m\in\{-1,1\}$, repeated use of the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives

$$
\begin{aligned}
\mathbb P(\xi_1=e_1,\ldots,\xi_m=e_m)
&=\mathbb E\left[
\mathbf1_{\{\xi_1=e_1,\ldots,\xi_{m-1}=e_{m-1}\}}
\mathbb P(\xi_m=e_m\mid\mathcal F_{m-1})
\right]\\
&=\frac12\mathbb P(\xi_1=e_1,\ldots,\xi_{m-1}=e_{m-1})\\
&=2^{-m}.
\end{aligned}
$$

**Hence the increments are [IID](../../../../../../independent-and-identically-distributed-random-variables.md) symmetric signs, proving the [symmetric signs forced by the martingale property](../../../../../../symmetric-signs-forced-by-the-martingale-property.md) result. Thus $X_n-X_0$ is a [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
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
