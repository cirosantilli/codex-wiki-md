<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For every $\theta\geq0$, the [Markov inequality](../../../../../../markov-inequality.md) and [independence](../../../../../../independent-random-variables.md) give the [Chernoff bound](../../../../../../chernoff-bound.md)

$$
\mathbb P(S_n\geq na)
\leq e^{-n\theta a}\mathbb E e^{\theta S_n}
=\exp\{-n(\theta a-\psi(\theta))\}.
$$

Optimize over nonnegative $\theta$. For $a\geq\mu$, part (a) identifies this supremum with $I(a)$, yielding the finite-$n$ estimate

$$
\boxed{\mathbb P(S_n\geq na)\leq e^{-nI(a)}.}
$$

If $I(a)=\infty$, use parameters with arbitrarily large $\theta a-\psi(\theta)$; the probability must then be zero. Taking the logarithmic upper limit proves the upper bound in the [Cramér theorem](../../../../../../cramer-s-theorem.md):

$$
\boxed{\limsup_{n\to\infty}\frac1n\log\mathbb P(S_n\geq na)\leq-I(a).}
$$

For $a<\mu$, the nonnegative-parameter supremum is zero, giving the correct trivial tail-rate upper bound. **Exponential Markov bounds and the product moment-generating function supply the entire upper-bound argument.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
