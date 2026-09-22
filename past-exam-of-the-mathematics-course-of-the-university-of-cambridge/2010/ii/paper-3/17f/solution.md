<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

Take a uniformly random ordering of the vertices and select each vertex that precedes every neighbor. The selected set is [independent](../../../../../independent-random-variables.md): if two adjacent vertices were both selected, each would have to precede the other. Among the $d(v)+1$ vertices consisting of $v$ and its neighbors, each is equally likely to come first, so the selection probability is $1/(d(v)+1)$. Linearity of [expectation](../../../../../expected-value.md) gives expected size $\sum_v1/(d(v)+1)$. At least one ordering attains at least this average; its [integer](../../../../../integer.md) size is therefore at least the ceiling. This proves the [Caro-Wei bound](../../../../../caro-wei-bound.md)

$$
\boxed{\alpha(G)\ge\left\lceil\sum_v\frac1{d(v)+1}\right\rceil.}
$$

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
