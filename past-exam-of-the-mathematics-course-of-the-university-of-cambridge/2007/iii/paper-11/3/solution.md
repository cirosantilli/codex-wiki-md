<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Blaschke product](../../../../../blaschke-product.md) here is taken over distinct points of the orbit; its existence is part of the hypothesis. It is not necessary to assert that every discrete orbit satisfies the [Blaschke condition](../../../../../blaschke-condition.md).

The modulus of a [Blaschke factor](../../../../../blaschke-factor.md) is the [pseudohyperbolic distance](../../../../../pseudohyperbolic-distance.md). Thus, away from the orbit,

$$
|B(z)|=\prod_{a\in G(0)}\left|\frac{z-a}{1-\overline az}\right|=\prod_{a\in G(0)}\tanh\frac{\rho(z,a)}2.
$$

The logarithms converge absolutely at such a point, by the compact convergence estimate for the [Blaschke product](../../../../../blaschke-product.md). Every $T\in G$ preserves the [hyperbolic metric](../../../../../hyperbolic-metric.md) and permutes the orbit. Reindexing this convergent product yields $|B(Tz)|=|B(z)|$.

The functions $B\circ T$ and $B$ have the same simple zero set, since $T$ is a [biholomorphism](../../../../../biholomorphism.md). Their quotient therefore extends holomorphically and without zeros across the orbit. It has modulus one everywhere. The [open mapping theorem](../../../../../open-mapping-theorem-complex-analysis.md) makes it a constant, denoted $\chi(T)$. Finally

$$
B(STz)=\chi(S)B(Tz)=\chi(S)\chi(T)B(z).
$$

Since $B$ is not identically zero, cancellation gives

$$
\boxed{\chi(ST)=\chi(S)\chi(T),\qquad |\chi(T)|=1,\qquad B(Tz)=\chi(T)B(z).}
$$

This is the [automorphy character of an orbit Blaschke product](../../../../../automorphy-character-of-an-orbit-blaschke-product.md). The equal-modulus argument is essential: equality of zero sets alone would not make the quotient of two bounded [holomorphic functions](../../../../../holomorphic-function.md) constant.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
