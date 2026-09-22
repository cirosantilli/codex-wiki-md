<h1 id="4g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix an effective enumeration $f_{e,n}$ of the $n$-ary [partial recursive functions](../../../../../../computable-function.md).

The [S-m-n theorem](../../../../../../smn-theorem.md) says that program inputs can be compiled into an index: for every $m,n\geq1$ there is a total recursive $s_n^m$ such that

$$
f_{s_n^m(e,x_1,\ldots,x_m),n}(y_1,\ldots,y_n)
\simeq f_{e,m+n}(x_1,\ldots,x_m,y_1,\ldots,y_n).
$$

Here $\simeq$ means that either both sides are undefined or both are defined and equal.

The [recursion theorem](../../../../../../kleene-s-recursion-theorem.md) says that every total recursive transformation $h$ of program indices has a semantic fixed point: some $e$ satisfies

$$
f_{e,1}\simeq f_{h(e),1}.
$$

The [Rice theorem](../../../../../../rice-s-theorem.md) says that every nontrivial [extensional property of programs](../../../../../../extensional-property-of-programs.md) computed by partial recursive functions is undecidable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4G](../../4g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
