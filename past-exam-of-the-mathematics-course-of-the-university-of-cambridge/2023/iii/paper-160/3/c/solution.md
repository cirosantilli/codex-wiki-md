<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the [Murnaghan–Nakayama rule](../../../../../../murnaghan-nakayama-rule.md) successively to the $w$ disjoint $e$-cycles. A complete term requires a sequence of $w$ removable $e$-hooks. If $w>w_e(\lambda)$, no such sequence exists after the [Weight of a partition](../../../../../../weight-of-a-partition.md) is exhausted, so the character value is zero.

Suppose $w=w_e(\lambda)$. Every complete sequence ends at the [Core of a partition](../../../../../../core-of-a-partition.md) $C_e(\lambda)$. Under the [abacus divisible-hook correspondence](../../../../../../hooks-divisible-by-the-abacus-modulus.md), a removal chooses one cell from one component $\lambda^{(i)}$ of the [quotient of a partition](../../../../../../quotient-of-a-partition.md). The choices of which runner is used occur in

$$
\binom{w}{|\lambda^{(0)}|,\ldots,|\lambda^{(e-1)}|}
$$

orders. Within runner $i$, the signed complete removal sum is the degree $\chi^{\lambda^{(i)}}(1)$, and all inter-runner removal orders have the common [Sign of an abacus hook-removal sequence](../../../../../../sign-of-an-abacus-hook-removal-sequence.md) $\varepsilon\in\{1,-1\}$. The remaining permutation $\gamma$ acts on the core, giving

$$
\boxed{\chi^\lambda(\rho\gamma)
=\varepsilon
\binom{w}{|\lambda^{(0)}|,\ldots,|\lambda^{(e-1)}|}
\chi^{C_e(\lambda)}(\gamma)
\prod_{i=0}^{e-1}\chi^{\lambda^{(i)}}(1).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 160](../../../paper-160-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
