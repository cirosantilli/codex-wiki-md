<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For every $\theta\geq0$, the [exponential Markov bound](../../../../../../exponential-markov-bound.md) and [independence](../../../../../../independent-random-variables.md) give

$$
\mathbb P(S_n/n\geq x)
=\mathbb P(e^{\theta S_n}\geq e^{n\theta x})
\leq e^{-n\theta x}\mathbb E e^{\theta S_n}
=\exp\{-n(\theta x-\psi(\theta))\}.
$$

Taking the [infimum](../../../../../../infimum.md) over $\theta\geq0$ yields

$$
\limsup_{n\to\infty}\frac1n\log\mathbb P(S_n/n\geq x)
\leq-\sup_{\theta\geq0}(\theta x-\psi(\theta)).
$$

For $x\geq m$, [convexity](../../../../../../convex-function.md) makes this supremum equal to $\psi^*(x)$, proving the upper bound in the stated tail form of [Cramér theorem](../../../../../../cramer-s-theorem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
