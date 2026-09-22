<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Necessity is a property of [standard Young tableaux](../../../../../../standard-young-tableau.md) alone. The first entry occupies $(1,1)$, with [Content of a Young-diagram cell](../../../../../../content-of-a-young-diagram-cell.md) zero. Every subsequent cell has a cell immediately above or to its left, of content one larger or one smaller, already present. If two entries occupy the same diagonal, the later cell lies strictly southeast of the earlier. The cells immediately right of and immediately below the earlier one exist and have contents $a+1,a-1$; their entries lie strictly between the two given entries. This proves all three conditions for [content vectors of standard Young tableaux](../../../../../../content-vector-of-a-standard-young-tableau.md).

For sufficiency, build the [Young diagram](../../../../../../young-diagram.md) one cell at a time. All coordinates are [integers](../../../../../../integer.md), because each new coordinate differs by one from an earlier coordinate, starting at zero. Cells of any fixed content $a$ are ordered northwest to southeast. For $a\geq0$ their positions are $(r,r+a)$, $r=1,2,\ldots$; for $a<0$ they are $(r-a,r)$.

At the first occurrence of a positive $a$, the candidate is $(1,a+1)$. The occurrence of $a+1$ earlier would already force a cell of content $a$ in its row, so the neighbor condition must instead supply the content $a-1$. This supplies the left predecessor. The negative case is symmetric, supplying the upper predecessor, and the first zero gives $(1,1)$.

At any later occurrence of $a$, take the next position on its diagonal. The preceding occurrence already supplied all but the next necessary predecessor on each neighboring diagonal. The repeated-entry condition supplies both $a-1$ and $a+1$ after that preceding occurrence, so those next predecessors are present. More explicitly, for $a>0$ and the $r$th occurrence, the left predecessor is the $r$th cell of content $a-1$, and the upper predecessor is the $(r-1)$st cell of content $a+1$. For $a=0$ both are the $(r-1)$st cells on their respective diagonals; for $a<0$ the roles are reversed. These are exactly the predecessors supplied by the two new neighboring occurrences.

The new cell is therefore an [addable node of a Young diagram](../../../../../../addable-node-of-a-young-diagram.md). Induction produces a [partition of an integer](../../../../../../partition-of-an-integer.md) at every stage, and filling the added cell by its insertion time gives a [standard Young tableau](../../../../../../standard-young-tableau.md). No choice was possible because [addable nodes of a Young diagram](../../../../../../addable-node-of-a-young-diagram.md) have distinct contents. Thus

$$
\boxed{\operatorname{Cont}(n)=\{a\in\mathbb C^n:a\text{ satisfies the three conditions}\},}
$$

and the construction also proves uniqueness of the tableau with a specified vector.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
