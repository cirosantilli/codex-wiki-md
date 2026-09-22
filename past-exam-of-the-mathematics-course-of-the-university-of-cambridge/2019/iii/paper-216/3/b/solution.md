<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The summand intended in the question is $d,h(X(t))/S(X(t))$. Under stationarity,

$$
\mathbb E_\pi\left[\frac{d,h(X)}{S(X)}\right]
=\int\frac{d,h(x)}{S(x)}\frac{S(x)}d\nu(dx)
=\int h\,d\nu=H.
$$

Moreover $S(x)\geq dc_1$, so the summand is bounded by $1/c_1$. A stationary geometrically ergodic Markov chain satisfies the [Markov-chain law of large numbers](../../../../../../markov-chain-law-of-large-numbers.md); hence

$$
\widehat H_n=\frac1n\sum_{t=1}^n
\frac{d,h(X(t))}{S(X(t))}
\longrightarrow H
$$

almost surely, and therefore in probability. In particular,

$$
\boxed{\Pr(|\widehat H_n-H|>\epsilon)\to0.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
