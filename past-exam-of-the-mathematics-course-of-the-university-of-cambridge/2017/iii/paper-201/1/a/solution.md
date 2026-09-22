<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Relative to a [probability space](../../../../../../probability-space.md) $(\Omega,\mathcal F,\mathbb P)$ and a [filtration](../../../../../../filtration-probability-theory.md) $(\mathcal F_n)$, the real [stochastic process](../../../../../../stochastic-process-split.md) $(M_n)$ is a [martingale](../../../../../../martingale-split.md) if it is [adapted](../../../../../../adapted-process.md), each $M_n$ is an [integrable random variable](../../../../../../integrable-random-variable.md), and

$$
\boxed{\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n\quad\text{almost surely for every }n\geq0.}
$$

Here [adapted](../../../../../../adapted-process.md) means $M_n$ is $\mathcal F_n$-measurable, and integrability means $\mathbb E|M_n|<\infty$. By the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md), the equivalent multi-step condition is $\mathbb E[M_j\mid\mathcal F_i]=M_i$ for all $i\leq j$. The [filtration](../../../../../../filtration-probability-theory.md) is part of the definition; specifying only the marginal means is insufficient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
