<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Lickorish-Dehn theorem](../../../../../../lickorish-dehn-theorem.md) says that every [orientation](../../../../../../orientation-of-a-simplex.md)-preserving [homeomorphism](../../../../../../homeomorphism.md) of a compact connected orientable surface, fixing its boundary pointwise, is isotopic relative to the boundary to a finite product of [Dehn twists](../../../../../../dehn-twist.md) and their inverses about simple closed curves. Boundary-parallel curves are permitted. For a closed surface of genus $g\ge1$, a finite collection of curves suffices to generate its [mapping class group](../../../../../../mapping-class-group.md). If boundary components are allowed to be permuted, twists alone do not express those permutations; the boundary condition is part of the precise statement.

The [fundamental theorem of Dehn surgery](../../../../../../fundamental-theorem-of-dehn-surgery.md) asserts that **every closed connected orientable [three-manifold](../../../../../../3-manifold.md) is integer surgery on a finite [framed link](../../../../../../framed-link.md) in $S^3$**. To prove it, first choose a [Heegaard splitting](../../../../../../heegaard-splitting.md) of $M$ of genus $g$. Existence of such splittings is a standard background result: a triangulation, with spanning trees collapsed in its primal and dual one-skeletons, gives complementary regular neighborhoods of finite graphs, hence two [handlebodies](../../../../../../handlebody.md). Choose a standard genus-$g$ splitting of $S^3$, formed by stabilizing its genus-zero splitting. Identify the two pairs of [handlebodies](../../../../../../handlebody.md). If $f_0$ is the sphere's gluing map and $f$ is the gluing map for $M$, then $f_0^{-1}f$ is an [orientation](../../../../../../orientation-of-a-simplex.md)-preserving self-[homeomorphism](../../../../../../homeomorphism.md) of the common surface. The [Lickorish-Dehn theorem](../../../../../../lickorish-dehn-theorem.md) writes it, up to isotopy, as a product $\tau_{c_1}^{\epsilon_1}\cdots\tau_{c_m}^{\epsilon_m}$, $\epsilon_i=\pm1$.

Here is the local surgery mechanism. Place $c$ on an intermediate level of a product collar of the surface. Its tubular neighborhood has longitude $\lambda$ given by that surface and meridian $\mu$ around the normal disk. Remove the neighborhood and fill with meridian slope $\mu\pm\lambda$. Cut the remaining annular neighborhood of $c$ along a transverse arc. Going around the new meridian now makes one extra positive or negative turn in the longitude direction. On gluing the cut annulus back, the two collar levels are therefore identified by $(\theta,s)\mapsto(\theta\pm\rho(s),s)$, precisely the [Dehn twist](../../../../../../dehn-twist.md) from part (a). Outside this annulus the identification is unchanged. This proves [unit surface-framed surgery realizes a Dehn twist](../../../../../../unit-surface-framed-surgery-realizes-a-dehn-twist.md); its surgery coefficient is $+1$ or $-1$ relative to the [surface framing](../../../../../../surface-framing.md), with sign fixed by the chosen normal convention.

Put the curves $c_i$ on distinct collar levels and order those levels to realize the indicated composition. They are disjoint as curves in the [three-manifold](../../../../../../3-manifold.md) even if their surface projections intersect. Performing the prescribed surgeries replaces $f_0$ by $f$, up to isotopy. An isotopy of a gluing map extends across a collar, so the filled manifold is homeomorphic to $M$.

Finally each surface framing differs from the preferred longitude framing in $S^3$ by an integer number of twists. Thus its coefficient $\pm1$ becomes an integer coefficient in the usual knot longitude convention. These finitely many disjoint curves form the required [framed link](../../../../../../framed-link.md) $L$:

$$
\boxed{M\cong S^3_L\text{ by integer Dehn surgery}.}
$$

The ingredients used were Heegaard-splitting existence, the stated twist-generation theorem, and the explicit local unit-surgery construction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
