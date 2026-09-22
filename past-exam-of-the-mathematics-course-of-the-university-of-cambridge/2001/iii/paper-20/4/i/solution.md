<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $M<N$ homogeneous equations $\sum_{j=1}^N a_{ij}z_j=0$ with integral coefficients $|a_{ij}|\le A$, $A\ge1$, [Siegel lemma](../../../../../../siegel-s-lemma.md) supplies a nonzero integral vector with

$$
0<\|z\|_\infty\le Q=\left\lfloor(2NA)^{M/(N-M)}\right\rfloor.
$$

Map the [integer](../../../../../../integer.md) box $\{0,\ldots,Q\}^N$ to the $M$ equation values. There are $(Q+1)^N$ inputs, while each output coordinate lies in $[-NAQ,NAQ]$, so there are at most $(2NAQ+1)^M$ outputs. Since $Q+1>(2NA)^{M/(N-M)}$ and $2NAQ+1\le2NA(Q+1)$, the input count is strictly larger. Two inputs have the same image; their nonzero difference solves every equation and has the stated norm bound. This proves the lemma by the [pigeonhole proof of integer Siegel lemma](../../../../../../pigeonhole-proof-of-integer-siegel-lemma.md).

Rational coefficients are handled by clearing denominators. For coefficients in a [number field](../../../../../../number-field.md) of degree $d$, expansion in a rational basis gives at most $dM$ rational equations; if $N>dM$ the same argument gives an [integer](../../../../../../integer.md) solution with the corresponding effective bound after clearing the basis denominators. The lemma concerns homogeneous equations; arbitrary inhomogeneous [integer](../../../../../../integer.md) equations need not be soluble.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
