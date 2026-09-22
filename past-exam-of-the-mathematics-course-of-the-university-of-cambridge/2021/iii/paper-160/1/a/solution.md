<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Expand the [Column antisymmetrizer of a Young tableau](../../../../../../column-antisymmetrizer-of-a-young-tableau.md):

$$
b_v\{w\}=\sum_{g\in C(v)}\operatorname{sgn}(g)\{gw\}.
$$

If two entries in one column of $v$ lie in the same row of $w$, their transposition belongs to both $C(v)$ and the row stabilizer of $w$, so the terms cancel in pairs. The assumption $b_v\{w\}\ne0$ therefore says that every row of $w$ meets every column of $v$ in at most one entry.

The first row of $w$ has $\lambda_1$ entries, while $v$ has exactly $\lambda_1$ nonempty columns. It must consequently contain exactly one entry from each column of $v$. Permuting within each column puts these entries in the first row positions of $v$. Delete the matched first rows and repeat the argument on the remaining [Young diagram](../../../../../../young-diagram.md). The product of the resulting column permutations is an element $h\in C(v)$ for which the row sets of $hv$ are those of $w$. Thus

$$
\boxed{h\{v\}=\{w\}}.
$$

This is the [nonzero column antisymmetrizer criterion](../../../../../../nonzero-column-antisymmetrizer-criterion.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 160](../../../paper-160-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
