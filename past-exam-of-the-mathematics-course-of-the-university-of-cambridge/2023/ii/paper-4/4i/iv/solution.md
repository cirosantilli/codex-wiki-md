<h1 id="4i/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

An accepting derivation in a right-linear grammar has the form

$$
S\Rightarrow w_1A_1\Rightarrow
w_1w_2A_2\Rightarrow\cdots
\Rightarrow w_1\cdots w_m,
$$

with one active variable until the final terminal production.

If no variable repeated on any accepting derivation, an accepting derivation could contain at most $|V|$ variable occurrences. Since the production set is finite, only finitely many such derivations and hence finitely many terminal words would exist. The hypothesis that $\mathcal L(G)$ is infinite therefore supplies an accepting derivation in which some variable $A$ occurs twice.

Split this derivation at the two occurrences:

$$
S\Rightarrow^*uA,\qquad
A\Rightarrow^*vA,\qquad
A\Rightarrow^*z,
$$

where $u,v,z\in\Sigma^*$. The first segment makes $A$ an [accessible variable of a regular grammar](../../../../../../accessible-variable-of-a-regular-grammar.md), the middle segment makes it a [looping variable of a regular grammar](../../../../../../looping-variable-of-a-regular-grammar.md), and the last makes it a [terminable variable of a regular grammar](../../../../../../terminable-variable-of-a-regular-grammar.md). Thus $A$ has all three properties, proving the [accessible looping terminable variable criterion](../../../../../../accessible-looping-terminable-variable-criterion.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4I](../../4i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
