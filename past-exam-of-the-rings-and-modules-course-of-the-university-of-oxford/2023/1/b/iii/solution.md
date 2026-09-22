<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [polynomial ring](../../../../../polynomial-ring.md) $\mathbb F_2[X]$ is a [euclidean domain](../../../../../euclidean-domain.md) under [polynomial degree](../../../../../degree-of-a-polynomial.md), hence a [principal ideal domain](../../../../../principal-ideal-domain.md). By part (b)(i), each

$$
K_j=\mathbb F_2[X]/(f_j)
$$

is a [field](../../../../../field.md). By [polynomial division](../../../../../polynomial-division.md), every residue class has exactly one representative of [polynomial degree](../../../../../degree-of-a-polynomial.md) less than $n_j$. Thus $1,\overline X,\ldots,\overline X^{n_j-1}$ form a [basis](../../../../../basis.md) over $\mathbb F_2$, and $|K_j|=2^{n_j}$.

For $j\ne k$, the [ideals](../../../../../ideal.md) $(f_j)$ and $(f_k)$ are distinct [maximal ideals](../../../../../maximal-ideal.md), so they are [comaximal ideals](../../../../../comaximal-ideals.md): their sum is an [ideal](../../../../../ideal.md) properly containing $(f_j)$ and must be the whole [ring](../../../../../ring.md). The [Chinese remainder theorem for ideals](../../../../../chinese-remainder-theorem-for-ideals.md) and part (b)(ii) therefore give the [ring isomorphism](../../../../../ring-isomorphism.md)

$$
\boxed{\mathbb F_2[X]/(f_1\cdots f_r)\ \cong\ \prod_{j=1}^rK_j,\qquad\overline g\longmapsto(g+(f_j))_{j=1}^r}.
$$

In particular, this is a product of [finite fields](../../../../../finite-field.md) of the required sizes. The map preserves multiplication as well as addition and is surjective by the [Chinese remainder theorem for ideals](../../../../../chinese-remainder-theorem-for-ideals.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the rings and modules course of the University of Oxford](../../../../split.md)
6. [Rings and modules course of the University of Oxford](../../../../../rings-and-modules-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
