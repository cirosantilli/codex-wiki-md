<h1 id="b/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [degree of a field extension](../../../../degree-of-a-field-extension.md) $[K:F]$ is the dimension of $K$ as a [vector space](../../../../vector-space-split.md) over $F$. The [tower law](../../../../tower-law.md) states that for finite extensions $F\subseteq E\subseteq K$,

$$
[K:F]=[K:E][E:F].
$$

If the left side is prime, one factor is one. Degree one forces equality of the corresponding fields, so **there is no proper intermediate field**.

Let $K$ have 32 elements. Its [prime field](../../../../prime-field.md) is $\mathbb F_2$, and its dimension over that field is five, since a dimension-$d$ [vector space](../../../../vector-space-split.md) over $\mathbb F_2$ has $2^d$ elements. Every element outside $\mathbb F_2$ has [minimal polynomial](../../../../minimal-polynomial.md) of degree five: its generated intermediate field has degree greater than one and dividing five.

Every element of $K$ satisfies $x^{32}=x$, by the [multiplicative group of a field](../../../../multiplicative-group-of-a-field.md) of order 31 for nonzero elements. Hence $X^{32}-X$ splits completely over $K$ and has no repeated roots, since its derivative is minus one. Conversely any [irreducible polynomial](../../../../irreducible-polynomial.md) $q$ over $\mathbb F_2$ gives a [quotient ring](../../../../quotient-ring.md) $\mathbb F_2[X]/(q)$ with 32 elements. Its defining element satisfies $X^{32}-X$, so $q$ divides that [polynomial](../../../../polynomial-split.md) and therefore has all five distinct roots in $K$.

The 30 elements of $K\setminus\mathbb F_2$ are thus partitioned into disjoint five-element root sets of the [irreducible polynomials](../../../../irreducible-polynomial.md). Their number is

$$
\boxed{\frac{32-2}{5}=6.}
$$

No classification of the six individual [polynomials](../../../../polynomial-split.md) is needed; the tower degree and separability already count them all.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
