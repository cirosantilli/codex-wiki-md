<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Sample [Brownian motion](../../../../../../brownian-motion-split.md) at integer times and put $Z_n=B_n/\sqrt n$. Every $Z_n$ has [normal distribution](../../../../../../normal-distribution.md) $N(0,1)$, although the $Z_n$ are correlated. Let

$$
L=\limsup_{n\to\infty}Z_n.
$$

For every fixed integer $m$,

$$
L=\limsup_{n\to\infty}\frac{B_n-B_m}{\sqrt n},
$$

because $B_m/\sqrt n\to0$ [almost surely](../../../../../../almost-sure-convergence.md). The right-hand expression depends only on the future [independent increments](../../../../../../independent-increments.md) $B_{j}-B_{j-1}$ with $j>m$. Thus $\{L\geq a\}$ is, up to a [null set](../../../../../../null-set.md), a [tail event](../../../../../../tail-event.md) of those [independent increments](../../../../../../independent-increments.md), and its probability is zero or one by the [Kolmogorov zero-one law](../../../../../../kolmogorov-s-zero-one-law.md).

For any finite real $a$, every $Z_n$ exceeds $a$ with the same positive probability $p_a=\mathbb P(N(0,1)\geq a)$. For each $N$,

$$
\mathbb P\left(\bigcup_{n\geq N}\{Z_n\geq a\}\right)\geq p_a.
$$

Taking the decreasing intersection over $N$ shows that $Z_n\geq a$ infinitely often with probability at least $p_a$. This event implies $L\geq a$, so $\mathbb P(L\geq a)>0$. The zero-one law makes it one. Intersecting over positive integers $a$ gives $L=+\infty$ [almost surely](../../../../../../almost-sure-convergence.md). The continuous-time limit superior is at least the one along integers, hence

$$
\boxed{\limsup_{t\to\infty}\frac{B_t}{\sqrt t}=+\infty
\quad\text{almost surely}.}
$$

This proves that [Brownian fluctuations exceed the square-root scale](../../../../../../brownian-fluctuations-exceed-the-square-root-scale.md) without needing the lower bound in the law of the iterated logarithm.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
