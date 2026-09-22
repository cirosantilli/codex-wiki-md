<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $D_n=\det[K(x_i,x_j)]_{i,j=1}^n$ and expand it by [permutations](../../../../../../permutation.md). The assumptions ensure that the indicated single-variable integrals exist; the [finite-rank projection kernel](../../../../../../finite-rank-projection-kernel.md) constructed above satisfies them with $r=m$. No symmetry of a general kernel is needed for the following argument.

If a [permutation](../../../../../../permutation.md) fixes $n$, its product contains the separate factor $K(x_n,x_n)$. Integration gives $r$ times the term of the corresponding [permutation](../../../../../../permutation.md) of $\{1,\ldots,n-1\}$. These terms contribute $rD_{n-1}$.

Otherwise $n$ belongs to a longer [permutation cycle](../../../../../../permutation-cycle.md). Let $i$ precede $n$ and let $j$ follow it. The only factors containing $x_n$ are $K(x_i,x_n)K(x_n,x_j)$, whose integral is $K(x_i,x_j)$ by the reproducing assumption. Delete $n$ from the cycle to obtain a [permutation](../../../../../../permutation.md) $\tau$ on $n-1$ letters. Inserting $n$ back after any of the $n-1$ possible letters reconstructs exactly one [permutation](../../../../../../permutation.md); its [sign of a permutation](../../../../../../sign-of-a-permutation.md) is $-\operatorname{sgn}(\tau)$, since increasing a cycle length by one reverses its sign. Thus the nonfixed terms contribute $-(n-1)D_{n-1}$.

Combining these two disjoint classes proves [projection kernel determinant integration](../../../../../../projection-kernel-determinant-integration.md):

$$
\boxed{\int_{\mathbb R}D_n\,dx_n=(r-n+1)D_{n-1}.}
$$

For $n=1$, use the empty [determinant](../../../../../../determinant.md) $D_0=1$, and the statement is precisely the assumed diagonal integral. For our kernel, [orthonormality](../../../../../../orthonormal-set.md) directly yields

$$
\int_{\mathbb R}K_m(x,y)K_m(y,z)\,dy=K_m(x,z),\qquad \int_{\mathbb R}K_m(x,x)\,dx=m,
$$

so every step of the marginal integration is justified.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
