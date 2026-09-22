<h1 id="6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**True.** Let $G=\langle X\mid R\rangle$ and $H=\langle Y\mid S\rangle$, using disjoint finite generating alphabets. The [direct product of groups](../../../../../../direct-product-of-groups.md) has finite presentation

$$
G\times H=\langle X,Y\mid R,S,[x,y]=1\ (x\in X,\ y\in Y)\rangle.
$$

The commuting relations let every word be reordered as a word in $X$ followed by a word in $Y$; the two projections then show that no additional relations within either factor are imposed. For an input word $w$, form its projections $w_X$ and $w_Y$ by deleting all letters from the other factor. Evaluate each projection with the given [word problem for a group](../../../../../../word-problem-for-groups.md) algorithm for that factor. The product coordinates give

$$
\boxed{w=1\text{ in }G\times H\quad\Longleftrightarrow\quad w_X=1\text{ in }G\ \text{and}\ w_Y=1\text{ in }H.}
$$

Both component algorithms halt, so this is a terminating algorithm. No subgroup-membership procedure or comparison between unknown presentations is required.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
