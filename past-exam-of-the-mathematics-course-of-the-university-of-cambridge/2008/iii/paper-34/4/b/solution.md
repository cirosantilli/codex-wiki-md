<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here $X_1\leq1$, so for every $\tau>0$,

$$
0<e^{\tau X_1}\leq e^\tau,\qquad M(\tau)=\mathbb E e^{\tau X_1}\leq e^\tau<\infty.
$$

The [Jensen inequality](../../../../../../jensen-s-inequality.md) for the strictly convex [exponential function](../../../../../../exponential-function.md) gives

$$
M(\tau)\geq e^{\tau\mathbb E X_1}=1.
$$

In fact the inequality is strict: $\mathbb P(X_1=1)>0$ and $\mathbb E X_1=0$ exclude a constant [random variable](../../../../../../random-variable-split.md). In particular, $\boxed{1\leq M(\tau)<\infty}$ as required.

For $Z_n=e^{\tau S_n}/M(\tau)^n$, independence and identical distribution give

$$
\mathbb E e^{\tau S_n}=\prod_{i=1}^n\mathbb E e^{\tau X_i}=M(\tau)^n.
$$

Thus $Z_n$ is positive, integrable with mean one, and adapted to the [natural filtration](../../../../../../natural-filtration.md). Conditioning on the next increment gives

$$
\mathbb E[Z_{n+1}\mid\mathcal F_n]
=\frac{e^{\tau S_n}}{M(\tau)^{n+1}}\mathbb E[e^{\tau X_{n+1}}\mid\mathcal F_n]
=\frac{e^{\tau S_n}}{M(\tau)^n}=Z_n.
$$

Consequently $\boxed{(Z_n)\text{ is a martingale}.}$ This is the [exponential martingale of a random walk](../../../../../../exponential-martingale-of-a-random-walk.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
