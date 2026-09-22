<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the convention that a [z-sieved number](../../../../../../rough-number.md) is a positive integer with no [prime factor](../../../../../../prime-factor.md) strictly below $z$; $1$ is included. Such integers are also called [rough numbers](../../../../../../rough-number.md). Using instead exclusion of [primes](../../../../../../prime-number.md) at most $z$ changes an endpoint convention, not the following fixed-$u$ asymptotic.

The [Buchstab function](../../../../../../buchstab-function.md) is the [continuous function](../../../../../../continuous-function.md) $w:[1,\infty)\to\mathbb R$ determined by

$$
\boxed{w(u)=\frac1u\quad(1\le u\le2),\qquad\frac{d}{du}(u w(u))=w(u-1)\quad(u>2).}
$$

Successive integration over intervals of length one determines the [Buchstab function](../../../../../../buchstab-function.md) uniquely from its initial values.

A standard fixed-$u$ form of [Buchstab theorem](../../../../../../buchstab-theorem.md) states that, for each fixed $u>1$, as $z\to\infty$,

$$
\boxed{\Phi(z^u,z)\sim\frac{z^u}{\log z}\,w(u).}
$$

For $1<u\le2$, this agrees with the [Prime number theorem](../../../../../../prime-number-theorem.md), since apart from an immaterial endpoint the [z-sieved numbers](../../../../../../rough-number.md) in this range are $1$ and the [primes](../../../../../../prime-number.md) from $z$ to $z^u$. The restriction $u>1$ matters: at $u=1$ the count is bounded, so the displayed asymptotic does not hold there.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
