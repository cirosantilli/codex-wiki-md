<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The transformation of the [uniform distribution](../../../../../../continuous-uniform-distribution.md) gives, for $x\geq1$,

$$
\mathbb P(X_1\geq x)=\mathbb P(U_1\leq x^{-2})=x^{-2}.
$$

Thus $X_1$ has a [Pareto distribution](../../../../../../pareto-distribution.md) with lower endpoint $1$ and shape $2$. It has mean $2$, but no positive exponential moments, so the preceding version of the [Cramér theorem](../../../../../../cramer-s-theorem.md) is unavailable.

At $a=0$, the event in question is certain. For every fixed $a>0$ and all sufficiently large $n$, positivity of the summands gives the [one-big-jump polynomial lower bound](../../../../../../one-big-jump-polynomial-lower-bound.md)

$$
1\geq\mathbb P(W_n\geq na)\geq\mathbb P(X_1\geq na)=(na)^{-2}.
$$

Taking logarithms and dividing by $n$ gives an upper bound $0$ and a lower bound $-2\log(na)/n\to0$. Hence

$$
\boxed{\lim_{n\to\infty}\frac1n\log\mathbb P(W_n\geq na)=0\quad\text{for every }a\geq0.}
$$

This covers thresholds below, at and above the mean. Above the mean it means decay is slower than exponential speed $n$, not that the tail [probability](../../../../../../probability.md) tends to $1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
