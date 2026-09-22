<h1 id="12g/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $K$ be the [diagonal halting set](../../../../../../../diagonal-halting-set.md) and put

$$
C=(\mathbb N\setminus K)\oplus K
=\{2n:n\notin K\}\cup\{2n+1:n\in K\}.
$$

If $C$ were a [computably enumerable set](../../../../../../../recursively-enumerable-set.md), then $n\mapsto2n$ would many-one reduce $\mathbb N\setminus K$ to $C$, making the complement of $K$ computably enumerable. Together with the computable enumerability of $K$, that would make $K$ a [computable set](../../../../../../../computable-set.md), a contradiction.

Moreover

$$
\mathbb N\setminus C=K\oplus(\mathbb N\setminus K).
$$

If this complement were computably enumerable, $n\mapsto2n+1$ would again make $\mathbb N\setminus K$ computably enumerable. **Thus neither $C$ nor its complement is computably enumerable.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [12G](../../../12g.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
