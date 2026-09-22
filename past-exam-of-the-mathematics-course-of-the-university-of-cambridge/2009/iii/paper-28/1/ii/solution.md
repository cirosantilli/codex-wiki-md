<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First reduce the [polynomial](../../../../../../polynomial-split.md) modulo seven. At residues $0,1,\ldots,6$, its values are respectively $4,2,6,1,0,2,6$. Its only residue root is therefore $4$, and $f'(4)=45\equiv3\pmod7$ is a [unit](../../../../../../unit-in-a-ring.md). By [Hensel lemma](../../../../../../hensel-s-lemma.md), this residue root lifts uniquely to the [7-adic integers](../../../../../../7-adic-integer.md); any other root would have to reduce to the same residue root. Thus **there is exactly one root in $\mathbb Z_7$, congruent to $4$ modulo seven.**

Modulo five the values at $0,1,\ldots,4$ are $4,2,1,2,1$, so there is no residue root and hence **no root in $\mathbb Z_5$.** Modulo three the only possible residue root is $-1$. But writing $x=-1+3t$ gives

$$
f(-1+3t)=6-27t^2+27t^3\equiv6\pmod9.
$$

Thus that residue root cannot lift even modulo nine, and **there is no root in $\mathbb Z_3$.** A repeated residue root alone would not establish this obstruction; the second congruence is needed.

Modulo two both residues are roots. The even residue is simple because $f'(0)=-3$ is a [2-adic unit](../../../../../../2-adic-unit.md), so [Hensel lemma](../../../../../../hensel-s-lemma.md) gives exactly one even root. For any odd [2-adic integer](../../../../../../2-adic-integer.md), $x^3\equiv x\pmod4$, whence $f(x)\equiv-2x\equiv2\pmod4$. No odd root can exist. Consequently the full answer is

$$
\boxed{\#\{x\in\mathbb Z_2:f(x)=0\}=1.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
