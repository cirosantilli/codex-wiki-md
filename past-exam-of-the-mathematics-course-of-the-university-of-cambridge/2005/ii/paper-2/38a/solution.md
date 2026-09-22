<h1 id="38a/solution">Solution</h1>

↑ **Parent:** [38A](../38a.md)

For a finite-dimensional linear operator $A$, the [Krylov subspace](../../../../../krylov-subspace.md) is

$$
\mathcal K_m(A,v)=\operatorname{span}\{v,Av,\ldots,A^{m-1}v\}.
$$

These spaces are nested, so their dimensions are nondecreasing and can rise by at most one at each step. If $v\ne0$, let $k$ be the first index for which $A^kv$ is a [linear combination](../../../../../linear-combination.md) of $v,\ldots,A^{k-1}v$. The preceding $k$ vectors are [independent](../../../../../independent-random-variables.md). Multiplying that dependence by $A$ and repeatedly substituting shows every higher power also lies in their span. Thus

$$
\boxed{d_m=m\ (1\leq m\leq k),\qquad d_m=k\ (m\geq k).}
$$

Such an index exists because the ambient space is finite-dimensional. If $v=0$, the separate answer is $d_m=0$ for every $m$, with $k=0$.

For [Krylov dimension from spectral components](../../../../../krylov-dimension-from-spectral-components.md), when $A$ is [diagonalizable](../../../../../diagonalizable-matrix.md), group the [eigenvector](../../../../../eigenvector.md) expansion by distinct [eigenvalues](../../../../../eigenvalue.md):

$$
v=u_1+\cdots+u_k,\qquad Au_j=\lambda_ju_j,
$$

where each $u_j$ is its nonzero component in a distinct [eigenspace](../../../../../eigenspace.md). Then $A^rv=\sum_j\lambda_j^ru_j$. The vectors $u_j$ are [independent](../../../../../independent-random-variables.md), and the [Vandermonde matrix](../../../../../vandermonde-matrix.md) $(\lambda_j^r)_{0\leq r<k}$ is invertible because the [eigenvalues](../../../../../eigenvalue.md) are distinct. Hence the first $k$ powers span exactly $\operatorname{span}\{u_j\}$, proving **the stabilized dimension equals the number of distinct [eigenspaces](../../../../../eigenspace.md) with nonzero component in $v$**. These $u_j$ themselves are [eigenvectors](../../../../../eigenvector.md), so this is also the minimum number of [eigenvectors](../../../../../eigenvector.md) needed to represent $v$ when the [eigenvectors](../../../../../eigenvector.md) may be chosen freely.

If the printed phrase instead means the count of nonzero coefficients in an arbitrary fixed eigenbasis, it is false with repeated [eigenvalues](../../../../../eigenvalue.md). For example $A=I$ and $v=e_1+e_2$ use two vectors of that [basis](../../../../../basis.md) but have $\dim\mathcal K_m=1$; the vector $v$ itself is an [eigenvector](../../../../../eigenvector.md). For a simple [spectrum](../../../../../spectrum-functional-analysis.md) there is no distinction. This qualification resolves the claim without assuming an unstated simple [spectrum](../../../../../spectrum-functional-analysis.md).

## ↑ Ancestors (10)

1. [38A](../38a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
