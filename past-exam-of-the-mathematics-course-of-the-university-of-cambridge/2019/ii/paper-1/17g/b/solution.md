<h1 id="17g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose the [strongly regular graph](../../../../../../strongly-regular-graph.md) has $n$ vertices, degree $d$, $r$ common neighbours for every adjacent pair and $s$ common neighbours for every nonadjacent pair. By the [walk count from powers of an adjacency matrix](../../../../../../walk-count-from-powers-of-an-adjacency-matrix.md), $(A^2)_{ij}$ counts common neighbours of $i$ and $j$, while $(A^2)_{ii}=d$. Hence the [adjacency-matrix relation for a strongly regular graph](../../../../../../adjacency-matrix-relation-for-a-strongly-regular-graph.md) is

$$
A^2=(d-s)I+(r-s)A+sJ,
$$

where $J$ is the [all-ones matrix](../../../../../../all-ones-matrix.md).

The [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) gives an orthonormal eigenbasis for $A$. Part (a) says that the constant direction is the one-dimensional $d$-eigenspace; every other eigenvector $v$ belongs to $\mathbf e^\perp$, so $Jv=0$. If $Av=\theta v$, the displayed identity gives

$$
\theta^2-(r-s)\theta-(d-s)=0.
$$

There are at most two possible roots $\theta$ in addition to $d$. Thus $G$ has at most three distinct eigenvalues.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17G](../../17g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
