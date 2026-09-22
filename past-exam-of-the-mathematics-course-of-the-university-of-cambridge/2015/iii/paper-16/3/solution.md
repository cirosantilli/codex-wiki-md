<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $U_{i_0\dots i_q}=U_{i_0}\cap\cdots\cap U_{i_q}$, the [Čech cochain complex](../../../../../cech-cochain-complex.md) has groups

$$
C^q(\mathcal U,\mathcal F)=\prod_{i_0<\cdots<i_q}\mathcal F(U_{i_0\dots i_q}),\qquad
(\delta c)_{i_0\dots i_{q+1}}=\sum_{j=0}^{q+1}(-1)^j c_{i_0\dots\widehat{i_j}\dots i_{q+1}}|_{U_{i_0\dots i_{q+1}}}.
$$

Terms in $\delta^2$ cancel in pairs, and [Čech cohomology](../../../../../cech-cohomology.md) is $\ker\delta/\operatorname{im}\delta$. A degree-zero [cocycle](../../../../../cocycle.md) is exactly a family of compatible local sections. The [sheaf gluing axiom](../../../../../sheaf-gluing-axiom.md) gives their unique [global section](../../../../../global-section.md), proving $\check H^0(\mathcal U,\mathcal F)\cong\mathcal F(X)$. If the cover has affine finite intersections, a [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) has no higher [cohomology](../../../../../cohomology-split.md) on those intersections by [vanishing of quasi-coherent cohomology on an affine scheme](../../../../../vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme.md). The [acyclic cover theorem](../../../../../leray-s-theorem.md) then identifies all Čech groups with [sheaf cohomology](../../../../../sheaf-cohomology.md). In particular, a finite affine [open cover](../../../../../open-cover.md) of a [separated variety](../../../../../separated-variety.md) has this property.

For the [sheaf of units of the structure sheaf](../../../../../sheaf-of-units-of-the-structure-sheaf.md), a multiplicative degree-one [cocycle](../../../../../cocycle.md) is a family $g_{ij}\in\mathcal O_X^*(U_i\cap U_j)$ satisfying $g_{ij}g_{jk}=g_{ik}$, with $g_{ji}=g_{ij}^{-1}$. It glues trivial rank-one [free modules](../../../../../free-module.md) into an [invertible sheaf](../../../../../line-bundle.md). Changing the local frames multiplies $g_{ij}$ by a [coboundary](../../../../../coboundary.md), and two sets of transition data give isomorphic [line bundles](../../../../../line-bundle.md) precisely when their [cocycles](../../../../../cocycle.md) differ this way. Tensoring [line bundles](../../../../../line-bundle.md) multiplies their [cocycles](../../../../../cocycle.md). Thus [line bundles trivialized by an open cover](../../../../../line-bundles-trivialized-by-an-open-cover.md) give the group [isomorphism](../../../../../isomorphism.md)

$$
\operatorname{Pic}(X)_{\mathcal U}\cong\check H^1(\mathcal U,\mathcal O_X^*).
$$

For the remaining arguments, work over the algebraically closed ground field. On the [irreducible variety](../../../../../irreducible-variety.md) $V$, put $\mathcal Q=\mathcal K^*/\mathcal O_V^*$, a quotient of [sheaves of abelian groups](../../../../../sheaf-of-abelian-groups.md). A [global section](../../../../../global-section.md) of $\mathcal Q$ is locally represented by [rational functions](../../../../../rational-function.md) $f_i$ whose ratios are regular units. The corresponding unit [cocycle](../../../../../cocycle.md) $f_j/f_i$ defines an [invertible sheaf](../../../../../line-bundle.md). A single global [rational function](../../../../../rational-function.md) has trivial [cocycle](../../../../../cocycle.md). Conversely, every [line bundle](../../../../../line-bundle.md) has a nonzero rational section: choose a nonzero vector in its one-dimensional fibre at the [generic point](../../../../../generic-point.md) and express it in local frames. This supplies such local $f_i$. If the associated [line bundle](../../../../../line-bundle.md) is trivial, changing frames makes all $f_i$ restrictions of one [rational function](../../../../../rational-function.md). Therefore

$$
 k(V)^*\longrightarrow\Gamma(V,\mathcal K^*/\mathcal O_V^*)\longrightarrow\operatorname{Pic}(V)\longrightarrow0
$$

is exact. This is the [Cartier-divisor description of the Picard group](../../../../../cartier-divisor-description-of-the-picard-group.md). The [sheaf of nonzero rational functions on an irreducible variety](../../../../../sheaf-of-nonzero-rational-functions-on-an-irreducible-variety.md) is [flasque](../../../../../flasque-sheaf.md), since all restrictions between nonempty [open sets](../../../../../open-set.md) are the identity on $k(V)^*$. Apply the [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) to $1\to\mathcal O_V^*\to\mathcal K^*\to\mathcal Q\to1$. Since $H^1(V,\mathcal K^*)=0$, its connecting map has exactly the [cokernel](../../../../../cokernel.md) just computed, proving

$$
\boxed{\operatorname{Pic}(V)\cong H^1(V,\mathcal O_V^*).}
$$

Finally the [Segre description of a smooth quadric surface](../../../../../segre-description-of-a-smooth-quadric-surface.md) identifies $V$ with $\mathbb P^1\times\mathbb P^1$. The two [rulings of a smooth quadric surface](../../../../../rulings-of-a-smooth-quadric-surface.md) have classes $F_1,F_2$ generating $\operatorname{Pic}(V)\cong\mathbb Z^2$. For completeness, remove one line in each ruling: the remaining chart is the [affine plane](../../../../../affine-plane.md), with factorial [coordinate ring](../../../../../coordinate-ring.md) $k[s,t]$ and trivial [divisor class group](../../../../../divisor-class-group.md). The [localization sequence for the divisor class group](../../../../../localization-sequence-for-the-divisor-class-group.md) makes $F_1,F_2$ generators, and their degrees on the two ruling lines prove independence. The hyperplane class, and hence the conic $C$, has bidegree $(1,1)$. By [Picard-group localization on a smooth variety](../../../../../picard-group-localization-on-a-smooth-variety.md), the [Picard group of a smooth affine quadric surface](../../../../../picard-group-of-a-smooth-affine-quadric-surface.md) is

$$
\boxed{\operatorname{Pic}(U)\cong\mathbb Z^2/\mathbb Z(1,1)\cong\mathbb Z.}
$$

Explicitly, the restriction of $\mathcal O_V(1,0)$ is nontrivial: if it were trivial on $U$, its rational trivialization would have divisor supported on $C$, forcing $(1,0)$ to be an integer multiple of $(1,1)$, which is impossible.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
