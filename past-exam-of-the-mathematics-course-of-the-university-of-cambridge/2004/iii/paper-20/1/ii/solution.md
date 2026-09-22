<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [complex analytic Lie group](../../../../../../complex-lie-group.md) is a [complex manifold](../../../../../../complex-manifold.md) whose multiplication and inversion are [holomorphic maps between complex manifolds](../../../../../../holomorphic-map-between-complex-manifolds.md). Its identity [tangent space](../../../../../../tangent-space.md) is a complex [Lie algebra](../../../../../../lie-algebra-split.md), and the [Adjoint representation of a Lie group](../../../../../../adjoint-representation-of-a-lie-group.md)

$$
\operatorname{Ad}:G\longrightarrow\operatorname{GL}_{\mathbb C}(\mathfrak g),\qquad
\operatorname{Ad}_g=d_e(h\mapsto ghg^{-1})
$$

is holomorphic: differentiating the holomorphic conjugation map with respect to its second variable gives holomorphically varying matrix entries.

Every scalar holomorphic [function](../../../../../../function-split.md) on a compact connected [complex manifold](../../../../../../complex-manifold.md) is constant. Indeed its modulus attains a maximum; the [maximum modulus principle](../../../../../../maximum-modulus-principle.md), applied in complex coordinate charts and along complex lines, makes it locally constant there, and connectedness propagates that constancy. Apply this to each entry of $\operatorname{Ad}$. Since $\operatorname{Ad}_e=I$, it follows that $\operatorname{Ad}_g=I$ for every $g$. Differentiation gives

$$
\operatorname{ad}_X(Y)=[X,Y]=0.
$$

Thus $\mathfrak g$ is abelian, and the connected [group](../../../../../../group-split.md) $G$ is abelian by the identity-neighbourhood argument in part (i). This proves that [compact connected complex Lie groups are complex tori](../../../../../../compact-connected-complex-lie-groups-are-complex-tori.md).

If $n=\dim_{\mathbb C}G$, identify $\mathfrak g$ with $\mathbb C^n$. The [Lie exponential map](../../../../../../exponential-map-of-a-lie-group.md) is holomorphic, additive, onto, and a local biholomorphism, by the holomorphic left-invariant differential equation and its identity derivative. Its kernel $B$ is a [discrete subgroup](../../../../../../discrete-subgroup.md) of the additive space $\mathbb C^n$. The induced map yields

$$
\boxed{G\cong\mathbb C^n/B}
$$

as complex [Lie groups](../../../../../../lie-group.md), not merely as real [groups](../../../../../../group-split.md). Compactness further forces $B$ to be a full-rank real lattice. If its real span $W$ were proper, projection would give a surjective continuous map $\mathbb C^n/B\to\mathbb R^{2n}/W$, contradicting compactness. The discrete-subgroup argument in part (i) therefore gives $B\cong\mathbb Z^{2n}$. The quotient is a [complex torus](../../../../../../complex-torus.md); it need not split into one-dimensional complex tori.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
