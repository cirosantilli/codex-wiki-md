<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $n=bk$, let $I_n$ be the [identity matrix](../../../../../../identity-matrix.md), let $J_m$ be the $m$-by-$m$ [all-ones matrix](../../../../../../all-ones-matrix.md), and put $B=\operatorname{diag}(J_k,\ldots,J_k)$, with one diagonal block per experimental block. The [variance-covariance matrix](../../../../../../covariance-matrix.md) is

$$
\Sigma=\sigma^2\{(1-\rho_1)I_n+(\rho_1-\rho_2)B+\rho_2J_n\}.
$$

Its [orthogonal decomposition](../../../../../../orthogonal-decomposition-by-a-closed-subspace.md) is obtained by first subtracting each block's [sample mean](../../../../../../sample-mean.md), then subtracting the grand [sample mean](../../../../../../sample-mean.md) from the block means. More explicitly, writing $x_{jt}$ for coordinate $t$ in block $j$, the three invariant subspaces are

$$
W=\{x:\sum_{t=1}^kx_{jt}=0\text{ for every }j\},\qquad
U=\{x:x_{jt}=a_j,\ \sum_{j=1}^ba_j=0\},\qquad
G=\operatorname{span}\{\mathbf1_n\}.
$$

They are pairwise [orthogonal](../../../../../../orthogonal-vectors.md), with [dimensions](../../../../../../dimension-vector-space.md) $b(k-1)$, $b-1$ and $1$, and their [direct sum](../../../../../../direct-sum.md) is $\mathbb R^n$. On $W$, both $B$ and $J_n$ vanish. On $U$, $B=kI$ and $J_n=0$. On $G$, $B=kI$ and $J_n=nI$. Thus the **[eigenvalues](../../../../../../eigenvalue.md) and corresponding invariant subspaces** are

$$
\boxed{\begin{array}{c|c|c}
\text{subspace}&\text{eigenvalue}&\text{dimension}\\
W&\sigma^2(1-\rho_1)&b(k-1)\\
U&\sigma^2[1+(k-1)\rho_1-k\rho_2]&b-1\\
G&\sigma^2[1+(k-1)\rho_1+k(b-1)\rho_2]&1
\end{array}}
$$

If some [eigenvalues](../../../../../../eigenvalue.md) coincide, their [eigenspace](../../../../../../eigenspace.md) is the [direct sum](../../../../../../direct-sum.md) of the listed subspaces with that value. Zero-dimensional rows are omitted when $b=1$ or $k=1$. For an admissible [covariance matrix](../../../../../../covariance-matrix.md) the [eigenvalues](../../../../../../eigenvalue.md) on nonzero subspaces must be nonnegative; these conditions are also sufficient for [positive semidefiniteness](../../../../../../positive-semidefinite-matrix.md). The [expectation](../../../../../../expected-value.md) parameters do not affect this calculation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
