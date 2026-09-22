<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

Choose the real embeddings $\sigma_i$ and one from each complex pair $\tau_j$. The [logarithmic embedding of number field units](../../../../../logarithmic-embedding-of-number-field-units.md) is

$$
\lambda(u)=(\log|\sigma_1u|,\ldots,\log|\sigma_ru|,2\log|\tau_1u|,\ldots,2\log|\tau_su|).
$$

It is a [group homomorphism](../../../../../group-homomorphism.md) from multiplication to addition. A unit has absolute [norm](../../../../../norm.md) one, so the coordinate sum is zero and its image lies in a Euclidean hyperplane of dimension $r+s-1$.

Here is the required discreteness argument. There are only finitely many algebraic integers of $K$ whose conjugate absolute values are bounded by a fixed constant: their monic minimal [polynomials](../../../../../polynomial-split.md) have degree at most $n$, and each integer coefficient is an elementary symmetric function of bounded roots, hence belongs to a fixed finite range. There are finitely many such [polynomials](../../../../../polynomial-split.md) and finitely many roots of each. A bounded set of logarithms bounds all conjugate absolute values, so every compact region in the logarithmic hyperplane meets the unit image in finitely many points. Thus the image is a discrete additive [subgroup](../../../../../subgroup.md).

Use the allowed Euclidean-group theorem: a discrete [subgroup](../../../../../subgroup.md) of a finite-dimensional real [vector space](../../../../../vector-space-split.md) is free abelian on finitely many vectors, with [rank](../../../../../rank-one-quadratic-form.md) at most the dimension. Therefore $\lambda(\mathcal O_K^\times)$ has [rank](../../../../../rank-one-quadratic-form.md) at most $r+s-1$. Its [kernel](../../../../../kernel-of-a-linear-map.md) is finite by the same bounded-conjugate argument, now with every absolute value one. Each element of a finite multiplicative group is a [root of unity](../../../../../root-of-unity.md), and conversely every [root of unity](../../../../../root-of-unity.md) has all logarithms zero. Thus the [kernel](../../../../../kernel-of-a-linear-map.md) is exactly the [finite group](../../../../../finite-group.md) of [roots of unity](../../../../../root-of-unity.md), and exactly the [torsion subgroup](../../../../../torsion-subgroup.md) of units.

Lift generators of the free logarithmic image to units; together with the finite [kernel](../../../../../kernel-of-a-linear-map.md) they generate every unit. Hence

$$
\boxed{\mathcal O_K^\times\text{ is finitely generated abelian of rank at most }r+s-1,\quad
\operatorname{tors}(\mathcal O_K^\times)=\mu(K).}
$$

This proves the requested upper bound without invoking the existence half of the [Dirichlet unit theorem](../../../../../dirichlet-s-unit-theorem.md). The field $\mathbb Q(\sqrt{11})$ is a subfield of $\mathbb R$, and its only real [roots of unity](../../../../../root-of-unity.md) are $\boxed{1,-1}$.

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
