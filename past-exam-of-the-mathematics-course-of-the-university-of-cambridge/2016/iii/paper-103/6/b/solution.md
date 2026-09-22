<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [generalised permutation](../../../../../../generalised-permutation.md) is a finite multiset of pairs $(a,b)$ from two ordered alphabets, written as a two-row array, or biword. It may equivalently be specified by a finite-support matrix of nonnegative integer multiplicities $m_{a,b}$. The condition that no column is repeated means $m_{a,b}\in\{0,1\}$: each ordered pair occurs at most once. It does not forbid repeated entries in either individual row.

For this class use the [dual Robinson–Schensted–Knuth correspondence](../../../../../../dual-robinson-schensted-knuth-correspondence.md). Order the columns by nondecreasing top entry $a$, and by **strictly decreasing bottom entry $b$ when the top entries agree**. Insert the bottom entries in that order by ordinary semistandard [row insertion](../../../../../../row-insertion.md), which bumps the leftmost entry strictly greater than the incoming entry. Record the corresponding top entry in each newly created cell. Let $T$ be the insertion tableau and $U$ the recording tableau.

Ordinary [row insertion](../../../../../../row-insertion.md) permits repeated entries, preserving weak increase along rows and strict increase down columns; therefore $T$ is a [semistandard Young tableau](../../../../../../semistandard-young-tableau.md). The recording entries are inserted in nondecreasing order, so $U$ weakly increases along both rows and columns before considering strictness. Within one block of equal top entries, the bottom entries are strictly decreasing. The standard row-bumping comparison lemma says that a later, smaller input creates a new box strictly below the box created by the preceding input. Thus the boxes carrying one repeated top entry form a vertical strip, with at most one in each row. Consequently $U$ has strictly increasing rows and weakly increasing columns, so **$U^t$ is semistandard**.

Knuth's generalized insertion theorem, in this dual ordering, makes the map a bijection between finite $0$-$1$ matrices and these pairs. Its reverse description is also transparent: remove the largest recording entry, choosing its lowest box when it repeats, and reverse [row insertion](../../../../../../row-insertion.md) in $T$. Repeating recovers bottom entries in the reverse of the specified ordering. Equal top entries recover distinct bottom entries, which is exactly the no-repeated-column condition. Thus

$$
\boxed{\pi\longleftrightarrow(T,U),\qquad
\operatorname{shape}(T)=\operatorname{shape}(U),\quad
T\text{ and }U^t\text{ semistandard}}.
$$

The descending tie rule matters; the usual ascending tie rule would instead give two ordinary [Semistandard Young tableaux](../../../../../../semistandard-young-tableau.md).

Finally, the type of a tableau means its entry-multiplicity vector. [Row insertion](../../../../../../row-insertion.md) rearranges and bumps entries without changing their multiplicities. Hence

$$
\boxed{\operatorname{type}(T)_b=\sum_a m_{a,b},\qquad
\operatorname{type}(U)_a=\sum_b m_{a,b}}.
$$

Thus the bottom-row multiplicities of the generalised permutation give the type of $T$, while the top-row multiplicities give the type of $U$; transposing $U$ does not change its type.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
