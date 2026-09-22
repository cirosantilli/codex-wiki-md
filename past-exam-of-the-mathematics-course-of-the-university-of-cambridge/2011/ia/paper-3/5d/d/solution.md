<h1 id="5d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Extend $\sigma\in S_n$ to a [permutation](../../../../../../permutation.md) $\widehat\sigma$ of $n+2$ letters that fixes the last two letters. Let $t=(n+1\ n+2)$, and let $\epsilon(\sigma)$ be $0$ or $1$ according as $\sigma$ is even or odd. Define

$$
\iota(\sigma)=\widehat\sigma\,t^{\epsilon(\sigma)}.
$$

The two factors have disjoint supports and commute. Their signs cancel, so $\iota(\sigma)\in A_{n+2}$. Additivity of [parity of a permutation](../../../../../../parity-of-a-permutation.md) modulo two gives

$$
\iota(\sigma\tau)=\widehat\sigma\widehat\tau\,t^{\epsilon(\sigma)+\epsilon(\tau)}
=\iota(\sigma)\iota(\tau).
$$

Thus $\iota$ is a [group homomorphism](../../../../../../group-homomorphism.md). Its restriction to the first $n$ letters recovers $\sigma$, making it injective. Its image is therefore a [subgroup](../../../../../../subgroup.md) isomorphic to $S_n$:

$$
\boxed{S_n\cong\iota(S_n)\leq A_{n+2}.}
$$

This [group embedding](../../../../../../group-embedding.md) works for every positive $n$, including the trivial case $n=1$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5D](../../5d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
