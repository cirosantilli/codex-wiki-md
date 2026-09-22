<h1 id="3i/solution">Solution</h1>

↑ **Parent:** [3I](../3i.md)

Write $\mathbf1_n$ for the all-one column vector. The [parity-check extension of a linear code](../../../../../parity-check-extension-of-a-linear-code.md) is

$$
C^+=\{(c_1,\ldots,c_n,c_1+\cdots+c_n):c\in C\}.
$$

The defining map $C\to\mathbb F_2^{n+1}$ is [linear](../../../../../linear-map.md), so $C^+$ is a binary [linear code](../../../../../linear-code.md). If $G$ is a [generator matrix](../../../../../generator-matrix.md) and $H$ a [parity-check matrix](../../../../../parity-check-matrix.md) for $C$, then one may take

$$
G^+=\begin{pmatrix}G&G\mathbf1_n\end{pmatrix},
\qquad
H^+=
\begin{pmatrix}
H&0\\
\mathbf1_n^T&1
\end{pmatrix}.
$$

The [punctured code](../../../../../punctured-code.md) in, say, the last coordinate is

$$
C^-=\{(c_1,\ldots,c_{n-1}):c\in C\}.
$$

Coordinate deletion is a [linear map](../../../../../linear-map.md), so $C^-$ is [linear](../../../../../linear-code.md). Its [generator matrix](../../../../../generator-matrix.md) $G^-$ is obtained by deleting the last column of $G$. If the [minimum distance](../../../../../minimum-hamming-distance-of-a-linear-code.md) is at least two, deletion is injective on $C$, and hence $C^-$ has the same dimension as $C$.

For its [parity-check matrix](../../../../../parity-check-matrix.md), first use invertible row operations on $H$ to make its nonzero last column a coordinate vector. The last column is nonzero because otherwise the weight-one word supported there would belong to $C$, contrary to $d\geq2$. Delete the pivot row and the last column; the resulting matrix $H^-$ is a [parity-check matrix](../../../../../parity-check-matrix.md) for $C^-$. Equivalently, $(C^-)^\perp$ is obtained by shortening the [dual code](../../../../../dual-code.md) $C^\perp$ at the deleted coordinate.

Finally, the [shortened code](../../../../../shortened-code.md) in the last coordinate is

$$
C'=\{(c_1,\ldots,c_{n-1}):(c_1,\ldots,c_{n-1},0)\in C\}.
$$

It is linear whenever $C$ is linear, because it is the puncture of the subspace $C\cap\{x_n=0\}$.

## ↑ Ancestors (10)

1. [3I](../3i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
