<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $a=B_{12}$, $b=B_{13}$, $c=B_{21}$, $d=B_{23}$, $e=B_{31}$, and $f=B_{32}$. Zero row sums put $B$ in the form used in the [spectrum of a three-dimensional matrix with zero row sums](../../../../../../spectrum-of-a-three-dimensional-matrix-with-zero-row-sums.md). In particular, $B(1,1,1)^T=0$. Define

$$
S=a+b+c+d+e+f,
$$



$$
T=ad+bc+bd+ae+af+bf+ce+cf+de.
$$

Expanding the [characteristic polynomial](../../../../../../characteristic-polynomial.md) gives $\det(\lambda I-B)=\lambda(\lambda^2+S\lambda+T)$, so

$$
\boxed{\lambda_0=0,\qquad\lambda_\pm=\frac{-S\pm\sqrt{S^2-4T}}2.}
$$

For the physical coefficients, $L_jB_{jk}=L_kB_{kj}$ with $L_j=M_j\sqrt{GM_\star a_j}$. Thus $W=\operatorname{diag}(L_j)$ gives [positive diagonal symmetrization of a matrix](../../../../../../positive-diagonal-symmetrization-of-a-matrix.md), and

$$
\mathbf z^\dagger WB\mathbf z=-\sum_{j<k}L_jB_{jk}|z_j-z_k|^2\le0.
$$

Consequently the [eigenvalues](../../../../../../eigenvalue.md) are real and nonpositive, and $B$ has a complete [eigenvector](../../../../../../eigenvector.md) basis. This justifies the mode expansion in part (i).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
