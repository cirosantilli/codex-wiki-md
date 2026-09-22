<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use standard [Brownian motion](../../../../../../brownian-motion-split.md), started at $X_0=0$. Fix $0\leq\alpha<\beta$, and divide $[\alpha,\beta]$ into $N$ equal subintervals. Its Brownian increments are independent centred [normal random variables](../../../../../../gaussian-random-variable.md) with strictly positive variance, so each is nonnegative with [probability](../../../../../../probability.md) $1/2$. A nondecreasing path on the entire interval must have every one of these increments nonnegative. Hence

$$
\mathbb P(X\text{ is nondecreasing on }[\alpha,\beta])\leq2^{-N}
$$

for every $N$, and therefore this probability is zero.

There are only countably many pairs of rational endpoints $0\leq\alpha<\beta$. Take the union of the corresponding null events. Every interval of positive length, even one selected depending on the path, contains an interval with rational endpoints. Outside that single null event no such interval can be nondecreasing. Thus

$$
\boxed{\mathbb P(\exists\text{ a positive-length interval on which }X\text{ is nondecreasing})=0.}
$$

Applying the same argument to $-X$ also rules out nonincreasing intervals, the full [nowhere monotonicity of Brownian motion](../../../../../../nowhere-monotonicity-of-brownian-motion.md) property.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
