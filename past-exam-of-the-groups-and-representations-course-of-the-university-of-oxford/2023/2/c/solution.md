<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the composition convention $(\sigma\tau)(i)=\sigma(\tau(i))$. Then $R_+(\sigma)R_+(\tau)e_i=e_{\sigma(\tau(i))}=R_+(\sigma\tau)e_i$. Since the [sign of a permutation](../../../../sign-of-a-permutation.md) is multiplicative, the same calculation gives $R_-(\sigma)R_-(\tau)=R_-(\sigma\tau)$. Both send the identity to $I$ and have inverses given by $\sigma^{-1}$, so both are [group representations](../../../../group-representation.md).

The [trace](../../../../matrix-trace.md) of a [permutation matrix](../../../../permutation-matrix.md) counts fixed points, and multiplying that [matrix](../../../../matrix.md) by its [sign of a permutation](../../../../sign-of-a-permutation.md) multiplies its [trace](../../../../matrix-trace.md) by that sign. Thus the two [characters](../../../../character-of-a-representation.md) are

$$
\chi_+=(4,2,0,1,0),\qquad
\chi_-=(4,-2,0,1,0).
$$

Let $u=e_1+e_2+e_3+e_4$ and $W=\{x\in\mathbb C^4:\sum_ix_i=0\}$. Both are [invariant subspaces](../../../../invariant-subspace.md), and $\mathbb C^4=\mathbb Cu\oplus W$. On $\mathbb Cu$, $R_+$ is the [trivial representation](../../../../trivial-representation.md) and $R_-$ is the sign [representation](../../../../group-representation.md). Subtracting their [characters](../../../../character-of-a-representation.md) yields

$$
\boxed{\chi_3=\chi_+-\chi_0=(3,1,-1,0,-1),\qquad
\chi_4=\chi_--\chi_1=(3,-1,-1,0,1).}
$$

The [character inner product](../../../../character-inner-product.md) verifies that it is an [irreducible representation](../../../../irreducible-representation.md):

$$
\langle\chi_3,\chi_3\rangle
=\frac{9+6+3+0+6}{24}=1.
$$

The squares of the entries of $\chi_4$ are identical, so its [character inner product](../../../../character-inner-product.md) with itself is also one. Their values at a transposition differ, so these [irreducible representations](../../../../irreducible-representation.md) are inequivalent. Therefore

$$
\boxed{R_+=R_0\oplus R_3,\qquad R_-=R_1\oplus R_4,\qquad R_4=R_1\otimes R_3.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../e/solution.md)
