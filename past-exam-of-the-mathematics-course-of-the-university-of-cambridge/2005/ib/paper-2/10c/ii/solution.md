<h1 id="10c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The cyclic [matrix](../../../../../../matrix.md) acts by $(v_1,v_2,v_3,v_4)\mapsto(v_2,v_3,v_4,v_1)$. For each fourth root of unity $\lambda$, the [vector](../../../../../../vector.md) $v_\lambda=(1,\lambda,\lambda^2,\lambda^3)^T$ satisfies $Av_\lambda=\lambda v_\lambda$, because $\lambda^4=1$. This supplies the four distinct [eigenvalues](../../../../../../eigenvalue.md) and nonzero [eigenvectors](../../../../../../eigenvector.md):

$$
\begin{array}{c|c}
\lambda&v_\lambda^T\\\hline
1&(1,1,1,1)\\
-1&(1,-1,1,-1)\\
i&(1,i,-1,-i)\\
-i&(1,-i,-1,i)
\end{array}
$$

[Eigenvectors](../../../../../../eigenvector.md) for distinct [eigenvalues](../../../../../../eigenvalue.md) are linearly independent. Thus, with these columns in the indicated order,

$$
P=\begin{pmatrix}1&1&1&1\\1&-1&i&-i\\1&1&-1&-1\\1&-1&-i&i\end{pmatrix},\qquad
\boxed{P^{-1}AP=\operatorname{diag}(1,-1,i,-i).}
$$

They form a [basis](../../../../../../basis.md) over $\mathbb C$, so there are no other [eigenvalues](../../../../../../eigenvalue.md). Equivalently the [characteristic polynomial](../../../../../../characteristic-polynomial.md) is $\lambda^4-1$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10C](../../10c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
