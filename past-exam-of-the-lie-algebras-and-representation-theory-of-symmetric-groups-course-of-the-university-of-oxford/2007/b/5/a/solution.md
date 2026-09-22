<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [tabloid](../../../../../tabloid.md) records the sets of entries in each row of a tableau. Let $C_t$ be the subgroup permuting entries independently within each column. The [polytabloid](../../../../../polytabloid.md) is

$$
e_t=\sum_{\pi\in C_t}\operatorname{sgn}(\pi)\{\pi t\},
$$

and the [Specht module](../../../../../specht-module.md) $S^\lambda$ is spanned by these [vectors](../../../../../vector.md). A [standard polytabloid](../../../../../standard-polytabloid.md) is one whose tableau increases along rows and down columns.

Order [tabloids](../../../../../tabloid.md) by first sorting each row increasingly, then comparing the resulting row-reading words lexicographically. For a standard tableau $t$, every nonidentity column [permutation](../../../../../permutation.md) produces a strictly larger word. In the first row affected by that [permutation](../../../../../permutation.md), each replacement comes from farther down the same column and is larger than the entry it replaces; all earlier rows remain unchanged. Sorting the affected row therefore increases its word. Also no nontrivial column [permutation](../../../../../permutation.md) fixes its row sets, since a cell is the unique intersection of its row and column. Hence the least [tabloid](../../../../../tabloid.md) in $e_t$ is $\{t\}$ with coefficient one.

Distinct standard tableaux have distinct row [tabloids](../../../../../tabloid.md). In a nonzero [linear relation](../../../../../linear-relation.md) among their [polytabloids](../../../../../polytabloid.md), choose the least leading [tabloid](../../../../../tabloid.md) with a nonzero coefficient. None of the [vectors](../../../../../vector.md) with larger leading [tabloids](../../../../../tabloid.md) can contribute to it, so its coefficient cannot cancel. This contradiction proves **[linear independence](../../../../../linear-independence.md) of the [standard polytabloids](../../../../../standard-polytabloid.md)**.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
