<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $P$ be a Sylow p-subgroup. Since $[G:P]$ is invertible in $k$, every $kG$-module is relatively $P$-projective.

Suppose first that $kP$ has only finitely many indecomposable modules $U_1,\ldots,U_t$. For every indecomposable $kG$-module $M$, decompose $\operatorname{Res}_P^GM$ into the $U_i$. Relative projectivity makes $M$ a summand of the corresponding finite direct sum of the $\operatorname{Ind}_P^GU_i$. The [Krull–Schmidt theorem](../../../../../../krull-schmidt-theorem.md) leaves only finitely many possible indecomposable summands, so $kG$ has finite representation type.

Conversely, suppose $kG$ has finitely many indecomposables. For an indecomposable $kP$-module $U$, the identity double coset in the [Mackey restriction formula](../../../../../../mackey-restriction-formula.md) shows that $U$ is a direct summand of

$$
\operatorname{Res}_P^G\operatorname{Ind}_P^GU.
$$

Decomposing the induced module into the finitely many $kG$-indecomposables and restricting them shows, again by Krull–Schmidt, that only finitely many $U$ can occur. Thus

$$
\boxed{kG\text{ has finite representation type}
\Longleftrightarrow kP\text{ has finite representation type}.}
$$

If $P$ is cyclic, the [indecomposable modules of a cyclic p-group in characteristic p](../../../../../../indecomposable-modules-of-a-cyclic-p-group-in-characteristic-p.md) form a finite list. If $P$ is noncyclic, its [Frattini quotient](../../../../../../frattini-quotient.md) has rank at least two and therefore has a quotient $C_p\times C_p$. Inflation preserves indecomposability and nonisomorphism, while $k(C_p\times C_p)$ has infinitely many indecomposable modules. The [Higman criterion for finite representation type of a group algebra](../../../../../../higman-criterion-for-finite-representation-type-of-a-group-algebra.md) now gives

$$
\boxed{kG\text{ has finite representation type}
\Longleftrightarrow P\text{ is cyclic}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
