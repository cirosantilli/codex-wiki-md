<h1 id="12f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [parse tree](../../../../../../parse-tree.md) has the start variable at its root; the ordered children of a variable spell the right side of the production used at that occurrence, and its leaves, read left to right, spell the derived word.

For a grammar in [Chomsky normal form](../../../../../../chomsky-normal-form.md) with $r$ variables, take pumping length $p=2^r$. A parse tree for a word of length at least $p$ has a root-to-leaf path containing one variable twice. The yield can therefore be written

$$
w=uvxyz,
$$

where $|vxy|\leq p$, $|vy|>0$, and replacing the subtree between the repeated variables zero, one, or several times proves

$$
uv^ixy^iz\in L\qquad(i\geq0).
$$

This is the [pumping lemma for context-free languages](../../../../../../pumping-lemma-for-context-free-languages.md). Without Chomsky normal form but with no epsilon or unit productions, use the maximum production length to choose a larger exponential $p$; bounded branching and the same repeated-variable argument apply.

The language $\{a^ib^ia^i:i\geq0\}$ is not context free. A pumped window of bounded length cannot alter all three long blocks equally, so pumping breaks one of the required equalities.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12F](../../12f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
