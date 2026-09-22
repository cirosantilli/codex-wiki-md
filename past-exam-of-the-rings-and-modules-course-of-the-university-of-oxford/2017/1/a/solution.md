<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [ring](../../../../ring.md) $R$, its [ring characteristic](../../../../characteristic-of-a-ring.md) is the least positive [integer](../../../../integer-split.md) $n$ with $n1_R=0$, or zero if no positive such integer exists. Equivalently it is the least positive integer satisfying $nr=0$ for every $r\in R$, because $nr=(n1_R)r$. This additive formulation also defines the [characteristic of a rng](../../../../characteristic-of-a-rng.md) when an identity is not assumed.

Let $R$ be an [integral domain](../../../../integral-domain.md). Since $1_R\ne0$, its characteristic is not one. If its positive characteristic were a composite integer $n=ab$ with $1<a,b<n$, minimality would give $a1_R\ne0$ and $b1_R\ne0$, but

$$
(a1_R)(b1_R)=n1_R=0.
$$

This contradicts the absence of [zero divisors](../../../../zero-divisor.md). Therefore

$$
\boxed{\operatorname{char}R=0\quad\text{or a prime number}.}
$$

This is the [characteristic of an integral domain](../../../../characteristic-of-an-integral-domain.md) theorem. If an integral domain is defined without requiring an identity, the same conclusion follows from the additive definition: for a hypothetical composite characteristic $n=ab$, choose $r$ with $ar\ne0$, which exists by minimality of $n$. Then $(ar)(bs)=n(rs)=0$ for every $s$, forcing $bs=0$ for every $s$ and contradicting minimality again.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the rings and modules course of the University of Oxford](../../../split.md)
5. [Rings and modules course of the University of Oxford](../../../../rings-and-modules-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
