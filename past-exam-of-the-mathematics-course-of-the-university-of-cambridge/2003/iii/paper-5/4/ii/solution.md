<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take an integer $K\ge1$ bounding synchronous distances at integer times. Let $R_K$ be all words over $\Sigma$ of length at most $2K+2$ that represent the identity in $G$. This is a finite set. We claim that $\langle\Sigma\mid R_K\rangle$ presents $G$, interpreting inverse letters in the usual way.

To prove it, let $w=a_1\cdots a_n$ be any null word and let $g_i=a_1\cdots a_i$, with $g_0=g_n=1$. Draw the [combing](../../../../../../combing-of-a-group.md) [paths](../../../../../../continuous-path.md) $\sigma(g_i)$ as vertical columns, completed [paths](../../../../../../continuous-path.md) being padded by stationary steps. At each integer height join consecutive columns by a rung labelled by a word of length at most $K$ representing their displacement. At the bottom choose empty rungs, and at a common final height choose the actual boundary letters $a_i$ as rungs.

Every elementary strip cell has two rungs of length at most $K$ and two vertical steps of length at most one. Its boundary word has length at most $2K+2$ and is null in $G$, because the four [paths](../../../../../../continuous-path.md) close in the actual [Cayley graph](../../../../../../cayley-graph.md). It is therefore a [relator](../../../../../../relator.md) in $R_K$. Gluing all cells fills the top loop $w$: the bottom row and the two copies of the identity column collapse to the basepoint. Thus every null word is a product of conjugates of these finitely many short [relators](../../../../../../relator.md). The reverse containment holds because each [relator](../../../../../../relator.md) is already an identity in $G$.

Hence the [finite presentation from a synchronous combing](../../../../../../finite-presentation-from-a-synchronous-combing.md) proves

$$
\boxed{G\text{ is finitely presented}.}
$$

This is an existence proof of a finite [relator](../../../../../../relator.md) set. It does not assume an [algorithm](../../../../../../algorithm.md) for identifying identities in an arbitrary [group presentation](../../../../../../group-presentation.md) before establishing decidability.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
