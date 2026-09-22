<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The gradient bound makes $f$ a [Lipschitz function](../../../../../../lipschitz-continuity.md), with $|f(x)|\le|f(0)|+K\lVert x\rVert$, so its value at a [Gaussian random variable](../../../../../../gaussian-random-variable.md) is integrable and square integrable. The future [Brownian increment](../../../../../../brownian-increment.md) $X_1-X_t$ is independent of $\mathcal F_t$ and has distribution $N(0,(1-t)I_d)$. Conditioning on the current location therefore gives

$$
\boxed{M_t=\mathbb E[f(X_t+(X_1-X_t))\mid\mathcal F_t]=P_{1-t}f(X_t).}
$$

This is the [Markov property](../../../../../../markov-property.md) expressed through the [Brownian transition semigroup](../../../../../../brownian-transition-semigroup.md). In particular $M_0=\mu$ and $M_1=f(X_1)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
