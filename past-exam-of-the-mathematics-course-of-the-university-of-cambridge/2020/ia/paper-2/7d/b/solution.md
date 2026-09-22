<h1 id="7d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Fermat-Euler theorem](../../../../../../euler-s-theorem.md) states that if $\gcd(a,n)=1$, then

$$
\boxed{a^{\phi(n)}\equiv1\pmod n}.
$$

Let $r_1,\ldots,r_{\phi(n)}$ be a reduced residue system modulo $n$. Multiplication by $a$ permutes these classes, because $ar_i\equiv ar_j\pmod n$ implies $r_i\equiv r_j\pmod n$. Hence

$$
\prod_i ar_i\equiv\prod_i r_i\pmod n.
$$

Every $r_i$ is invertible modulo $n$, so cancellation gives $a^{\phi(n)}\equiv1\pmod n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7D](../../7d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
