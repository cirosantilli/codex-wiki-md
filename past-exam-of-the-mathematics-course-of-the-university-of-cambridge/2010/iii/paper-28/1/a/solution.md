<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $0<p<1$, so the ratio defining $Z_n$ is meaningful. Extend the [random walk](../../../../../../random-walk.md) by $S_0=0$, the [filtration](../../../../../../filtration-probability-theory.md) by a trivial $\mathcal F_0$, and the process by $Z_0=1$. Write $r=q/p$. Each $Z_n=r^{S_n}$ is $\mathcal F_n$-measurable and integrable, since $|S_n|\leq n$. The next increment is independent of $\mathcal F_n$, so

$$
\mathbb E[Z_{n+1}\mid\mathcal F_n]
=Z_n\mathbb E[r^{X_{n+1}}]
=Z_n(pr+qr^{-1})
=Z_n(q+p)=Z_n.
$$

Therefore $\boxed{(Z_n)_{n\geq0}\text{ is a nonnegative martingale},\quad\mathbb EZ_n=1}$. This is the [exponential martingale of a biased simple random walk](../../../../../../exponential-martingale-of-a-biased-simple-random-walk.md), with exponent $\log(q/p)$. At $p=q=1/2$, it is the constant process one. The endpoint cases $p=0$ or $p=1$ require separate definitions and are not covered by the printed ratio.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
