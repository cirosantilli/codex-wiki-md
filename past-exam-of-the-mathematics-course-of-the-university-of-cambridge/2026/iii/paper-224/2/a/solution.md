<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $P\ne Q$ be [probability mass functions](../../../../../../probability-mass-function.md) on a finite [alphabet](../../../../../../alphabet.md), with $P$ absolutely continuous with respect to $Q$. A decision region $B_n$ accepts the null law $P^{\otimes n}$. Write

$$
\alpha_n=P^{\otimes n}(B_n^c),\qquad
\beta_n=Q^{\otimes n}(B_n)
$$

for its type-I and type-II errors. [Stein's lemma](../../../../../../stein-s-lemma-information-theory.md) states that for every fixed $0<\varepsilon<1$,

$$
\lim_{n\to\infty}-\frac1n\log
\inf_{B_n:\,\alpha_n\leq\varepsilon}\beta_n
=D(P\Vert Q),
$$

where logarithms and [relative entropy](../../../../../../kullback-leibler-divergence.md) use base two.

For achievability, let

$$
B_n=\left\{x_1^n:\frac1n\log
\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}
\geq D(P\Vert Q)-\eta\right\}.
$$

Under $P^{\otimes n}$, the normalized log-likelihood ratio converges in probability to $D(P\Vert Q)$ by the [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md), so $alpha_n\to0$. On $B_n$, $Q^{\otimes n}\leq2^{-n(D(P\Vert Q)-\eta)}P^{\otimes n}$, whence $\beta_n\leq2^{-n(D(P\Vert Q)-\eta)}$.

For the converse, let

$$
A_n=\left\{x_1^n:\frac1n\log
\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}
\leq D(P\Vert Q)+\eta\right\}.
$$

Again $P^{\otimes n}(A_n)\to1$. If $alpha_n\leq\varepsilon$, then

$$
\beta_n\geq Q^{\otimes n}(B_n\cap A_n)
\geq2^{-n(D(P\Vert Q)+\eta)}P^{\otimes n}(B_n\cap A_n).
$$

The final factor has positive lower limit at least $1-\varepsilon$. Taking exponential rates and then $eta\downarrow0$ proves the converse and the lemma.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
