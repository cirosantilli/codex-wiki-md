<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\Gamma=\pi_1(M)$. A compact connected smooth [manifold](../../../../../../topological-manifold.md) has finite [CW complex](../../../../../../cw-complex.md) homotopy type, hence a finitely generated [fundamental group](../../../../../../fundamental-group.md). Its [universal cover](../../../../../../universal-cover.md) with the lifted [Riemannian metric](../../../../../../riemannian-metric.md) is complete by the lifted-geodesic argument in part 2(b) and has nonnegative [Ricci curvature](../../../../../../ricci-curvature.md). The [deck transformations](../../../../../../deck-transformation.md) act freely and [properly discontinuously](../../../../../../properly-discontinuous-group-action.md) by [isometries](../../../../../../isometry.md). Part (a) gives

$$
\beta_\Gamma(m)\leq C(1+m)^n.
$$

The degree-one [Hurewicz theorem](../../../../../../hurewicz-theorem.md) identifies $H_1(M;\mathbb Z)$ with the [abelianization](../../../../../../abelianization.md) of $\Gamma$. This finitely generated abelian group has free rank $b=b_1(M)$, so there is a surjection $\Gamma\to\mathbb Z^b$. Choose lifts $\gamma_1,\ldots,\gamma_b$ of a basis and let $A\geq1$ bound their [word lengths](../../../../../../word-length.md). For every $(z_1,\ldots,z_b)$ with $\sum|z_i|\leq m$, the product $\gamma_1^{z_1}\cdots\gamma_b^{z_b}$ has word length at most $Am$ and maps to that vector. Distinct vectors therefore give distinct group elements. The integer cube $|z_i|\leq\lfloor m/b\rfloor$ shows, for $b>0$, that

$$
\beta_\Gamma(Am)\geq c m^b
$$

for some $c>0$ and all sufficiently large $m$. Comparing with the degree-$n$ upper bound forces $b\leq n$; the case $b=0$ is immediate. Thus

$$
\boxed{b_1(M)\leq n.}
$$

This is the [first Betti-number bound from polynomial fundamental-group growth](../../../../../../first-betti-number-bound-from-polynomial-fundamental-group-growth.md).

The standard connectedness convention for a [Riemannian manifold](../../../../../../riemannian-manifold.md) is needed here. If disconnected manifolds are allowed, the bound applies to each connected component; a disjoint union of two flat $n$-tori has first [Betti number](../../../../../../betti-number.md) $2n$ and contradicts a global bound by $n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
