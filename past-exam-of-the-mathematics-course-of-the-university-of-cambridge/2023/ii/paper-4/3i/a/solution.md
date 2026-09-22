<h1 id="3i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the standard dot product on $\mathbb F_2^n$, the [dual code](../../../../../../dual-code.md) is

$$
\boxed{
C^\perp=\{y\in\mathbb F_2^n:y\cdot c=0
\text{ for every }c\in C\}.}
$$

It is an intersection of kernels of [linear functions](../../../../../../linear-function.md), and is therefore a [linear code](../../../../../../linear-code.md).

Let $\sigma$ denote cyclic right shift. If $y\in C^\perp$ and $c\in C$, then

$$
(\sigma y)\cdot c=y\cdot(\sigma^{-1}c).
$$

A [cyclic code](../../../../../../cyclic-code.md) is closed under both $\sigma$ and $\sigma^{-1}$, so $\sigma^{-1}c\in C$ and the right-hand side vanishes. Hence $\sigma y\in C^\perp$, proving directly that the [dual of a cyclic code](../../../../../../dual-of-a-cyclic-code.md) is cyclic.

Identify words with polynomials in $\mathbb F_2[X]/(X^n-1)$. If the [generator polynomial of a cyclic code](../../../../../../generator-polynomial-of-a-cyclic-code.md) is the monic divisor $g(X)$ and

$$
g(X)h(X)=X^n-1,
$$

then the generator polynomial of $C^\perp$ is the monic reciprocal

$$
\boxed{g^\perp(X)=h^*(X)
=X^{\deg h}h(X^{-1})/h(0).}
$$

Equivalently, the parity-check polynomial of one code becomes, after reversal, the generator polynomial of its dual.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3I](../../3i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
