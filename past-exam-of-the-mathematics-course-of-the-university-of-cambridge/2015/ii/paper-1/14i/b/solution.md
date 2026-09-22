<h1 id="14i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $A$ be the [adjacency matrix of a graph](../../../../../../adjacency-matrix.md), $J$ the all-ones [matrix](../../../../../../matrix.md) and $\mathbf1$ the all-ones vector. Counting two-step walks gives

$$
A^2=(k-b)I+(a-b)A+bJ,\qquad A\mathbf1=k\mathbf1.
$$

Because $b\geq1$, any two nonadjacent vertices have a common neighbour, so the graph is connected. The [eigenvalue](../../../../../../eigenvalue.md) $k$ is simple: for a real [eigenvector](../../../../../../eigenvector.md) at $k$, a maximal entry and the averaging equation force its neighbours, and then every vertex, to have the same value. Since $A$ is real symmetric, its other [eigenvectors](../../../../../../eigenvector.md) lie in $\mathbf1^\perp$, where $J$ vanishes. Their [eigenvalues](../../../../../../eigenvalue.md) are therefore

$$
r,s=\frac{a-b\pm d}{2},\qquad d=\sqrt{(a-b)^2+4(k-b)}.
$$

Here $d>0$ for the present incomplete connected graph. Indeed $k\geq b$; if $d=0$, then $k=b=a$, which conflicts with $a\leq k-1$ for an edge. If $r,s$ have multiplicities $m_r,m_s$, dimension and zero trace give $m_r+m_s=n-1$ and $k+m_rr+m_ss=0$. Thus

$$
\boxed{m_r=\frac12\left(n-1+\frac{(n-1)(b-a)-2k}{d}\right),\qquad
m_s=\frac12\left(n-1-\frac{(n-1)(b-a)-2k}{d}\right)}.
$$

These are dimensions of [eigenspaces](../../../../../../eigenspace.md), hence integers. A multiplicity may be zero; that does not affect the conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14I](../../14i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
