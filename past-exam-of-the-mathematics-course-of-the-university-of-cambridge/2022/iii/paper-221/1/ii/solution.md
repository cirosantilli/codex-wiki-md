<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Among observed pretreatment variables, every sufficient set must contain $M_1$ to block

$$
Z_1\leftarrow M_1\to C\to Y
$$

and $Z_3$ to block

$$
Z_1\leftarrow S\to Z_3\to Y.
$$

Conditioning on $Z_3$ opens the [collider](../../../../../../collider.md) on

$$
Z_1\leftarrow S\to Z_3\leftarrow M_3\to C\to Y,
$$

so $M_3$ must also be included. The resulting minimal [sufficient adjustment set](../../../../../../sufficient-adjustment-set.md) is

$$
X_0=\{M_1,M_3,Z_3\}.
$$

It blocks every path from $Z_1$ to $Y$ that remains after removing $A\to Y$, while the open path

$$
Z_1\leftarrow S\to Z_2\to A
$$

preserves [instrument relevance](../../../../../../instrument-relevance.md). Adding $M_2$ blocks no required relevance path, so

$$
X_1=\{M_1,M_2,M_3,Z_3\}
$$

is also sufficient.

There are no others. In particular, adding $Z_2$ blocks the displayed relevance path. Without $M_2$, conditioning on $Z_2$ also opens

$$
Z_1\leftarrow S\to Z_2\leftarrow M_2\to C\to Y,
$$

which violates independence; adding $M_2$ closes that path but leaves no open path from $Z_1$ to $A$. Hence the complete list is $X_0$ and $X_1$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
