<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the [Snake lemma](../../../../../../snake-lemma.md) degree by degree to a short exact sequence of complexes

$$
0\to A_\bullet\to B_\bullet\to C_\bullet\to0.
$$

If $[c]\in H_n(C)$, lift a cycle $c$ to $b\in B_n$. Its boundary maps to zero in $C_{n-1}$, so it comes from a cycle $a\in A_{n-1}$; define $\partial[c]=[a]$. The Snake-lemma exactness and independence checks yield

$$
\cdots\to H_n(A)\to H_n(B)\to H_n(C)
\xrightarrow{\partial}H_{n-1}(A)\to H_{n-1}(B)\to\cdots.
$$

This is the algebraic [Mayer–Vietoris theorem](../../../../../../mayer-vietoris-sequence.md) for homology objects.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
