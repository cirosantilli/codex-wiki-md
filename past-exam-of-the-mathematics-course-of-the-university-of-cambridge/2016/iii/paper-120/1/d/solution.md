<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [regular language](../../../../../../regular-language.md) $L$ is nonempty because it represents every element of the [group](../../../../../../group-split.md). Find any accepted word $t=a_1\cdots a_k$ using [Breadth-first search](../../../../../../breadth-first-search.md) in its [finite-state automaton](../../../../../../finite-state-machine.md). If $t$ is the [empty word](../../../../../../empty-word.md), it already represents the identity.

Otherwise begin with $t\in L$ and repeatedly apply the [linear-time multiplication in an automatic structure](../../../../../../linear-time-multiplication-in-an-automatic-structure.md) to the letters

$$
a_k^{-1},a_{k-1}^{-1},\ldots,a_1^{-1}.
$$

These letters belong to $A$ by symmetry of the [alphabet](../../../../../../alphabet.md). All intermediate words lie in $L$, and the final word $\gamma$ represents

$$
\overline t\,a_k^{-1}\cdots a_1^{-1}=1.
$$

Hence **an identity representative can be constructed effectively**:

$$
\boxed{\gamma\in L,\qquad\overline\gamma=1.}
$$

This is a finite preliminary computation depending only on the fixed [automatic structure for a group](../../../../../../automatic-structure-for-a-group.md); it uses no test for whether an arbitrary word represents the identity.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
