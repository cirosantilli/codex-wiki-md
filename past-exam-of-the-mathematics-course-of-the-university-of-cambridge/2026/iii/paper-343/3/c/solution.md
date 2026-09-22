<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Ignoring the common normalization $1/(2\sqrt2)$, direct multiplication gives

$$
|v(e_{00})\rangle
=|000\rangle+|001\rangle+|010\rangle-|011\rangle,
$$



$$
|v(e_{10})\rangle
=|000\rangle-|001\rangle+|010\rangle+|011\rangle,
$$



$$
|v(e_{01})\rangle
=|100\rangle+|101\rangle-|110\rangle+|111\rangle,
$$



$$
|v(e_{11})\rangle
=|100\rangle-|101\rangle-|110\rangle-|111\rangle.
$$

These four states span the positive eigenspace of $Z\otimes X\otimes Z$. The parent term annihilating that local MPS support is therefore the complementary projector

$$
\boxed{h=\frac12(I-Z\otimes X\otimes Z)}.
$$

Translated terms have stabilizers $K_j=Z_{j-1}X_jZ_{j+1}$. Two such Pauli strings either do not overlap nontrivially or have two X--Z anticommutations, so all $K_j$ commute. Their positive eigenspaces have a common state, making the parent Hamiltonian frustration free. Each alternating global X symmetry flips the two Z factors of every $K_j$ or neither, and therefore commutes with every local term.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
