<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Gaudin's lemma](../../../../../projection-kernel-determinant-integration.md) is the [projection kernel determinant integration](../../../../../projection-kernel-determinant-integration.md) identity. Suppose an [integral kernel](../../../../../integral-kernel.md) $K$ satisfies

$$
\int K(x,y)K(y,z)\,d\mu(y)=K(x,z),
\qquad \int K(x,x)\,d\mu(x)=N,
$$

with the relevant integrals absolutely convergent. Define $D_k(x_1,\ldots,x_k)=\det[K(x_i,x_j)]_{i,j=1}^k$ and $D_0=1$. Then

$$
\boxed{\int D_k(x_1,\ldots,x_k)\,d\mu(x_k)
=(N-k+1)D_{k-1}(x_1,\ldots,x_{k-1}).}
$$

In particular, a [finite-rank projection kernel](../../../../../finite-rank-projection-kernel.md) of rank $N$ has $\int D_N\,d\mu^N=N!$.

One can see the factor directly from the [permutation](../../../../../permutation.md) expansion of the [determinant](../../../../../determinant.md). Terms whose [permutation](../../../../../permutation.md) fixes $k$ integrate to $ND_{k-1}$. Every [permutation](../../../../../permutation.md) on the other $k-1$ indices admits $k-1$ insertions of $k$ into a cycle. Each insertion reverses its sign, and the reproducing identity contracts its two adjacent kernel factors into one. These terms integrate to $-(k-1)D_{k-1}$, proving the formula.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
