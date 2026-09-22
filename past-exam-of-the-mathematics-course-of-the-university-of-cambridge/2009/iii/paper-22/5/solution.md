<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $p=|a|$, $q=|b|$ and $r=|ab|$ denote element orders. Remove three points from an oriented [sphere](../../../../../sphere.md). Its [fundamental group](../../../../../fundamental-group.md) has peripheral generators $\gamma_a,\gamma_b,\gamma_c$ with $\gamma_a\gamma_b\gamma_c=1$. Send them to $a,b,(ab)^{-1}$. Since $a,b$ generate $T$, the kernel defines a connected [regular covering](../../../../../regular-covering.md) of the punctured sphere with degree $|T|$ and [deck transformation group](../../../../../deck-transformation-group.md) $T$.

Complete the lifted punctures by disks. Above the three removed points the [monodromy](../../../../../monodromy.md) cycles have lengths $p,q,r$, respectively, and the disk projection has the local form $z\mapsto z^p$, $z^q$ or $z^r$. This gives a closed connected oriented [topological surface](../../../../../topological-surface.md) $M$ and an orientation-preserving $T$-action. At the three kinds of filled-in points the [stabiliser subgroups](../../../../../stabilizer-subgroup.md) are conjugates of $\langle a\rangle$, $\langle b\rangle$ and $\langle ab\rangle$, respectively. Every other point has trivial [stabiliser subgroup](../../../../../stabilizer-subgroup.md). Orders equal to one simply correspond to unbranched filled points.

The punctured sphere has [Euler characteristic](../../../../../euler-characteristic.md) $-1$, so its cover has [Euler characteristic](../../../../../euler-characteristic.md) $-|T|$. Filling the ends adds $|T|/p+|T|/q+|T|/r$ disks. This proves the formula for the [branched surface action from two generators](../../../../../branched-surface-action-from-two-generators.md):

$$
\boxed{\chi(M)=|T|\left(\frac1p+\frac1q+\frac1r-1\right).}
$$

For a subgroup $U$, its quotient map is always regular as a branched quotient. It is an ordinary unbranched [normal covering map](../../../../../normal-covering-map.md) exactly when $U$ acts freely, that is,

$$
\boxed{U\cap t\langle a\rangle t^{-1}
=U\cap t\langle b\rangle t^{-1}
=U\cap t\langle ab\rangle t^{-1}=\{1\}quad\text{for every }t\in T.}
$$

Necessity follows from the listed [stabiliser subgroups](../../../../../stabilizer-subgroup.md). Conversely, these conditions eliminate every possible nontrivial point stabiliser. A free finite action gives a [covering space](../../../../../covering-space.md), and its [deck transformations](../../../../../deck-transformation.md) are $U$, acting transitively on each fibre; hence the cover is normal. In this case

$$
\boxed{\chi(U\backslash M)=\frac{|T|}{|U|}
\left(\frac1p+\frac1q+\frac1r-1\right).}
$$

The condition $U\trianglelefteq T$ concerns regularity of the different map $U\backslash M\to T\backslash M$; it is not needed for $M\to U\backslash M$ when the action of $U$ is free.

For the specified order-$96$ group, $p=q=3$. Set $c=ab$ and $z=c^3$. Since $z$ has order two, $c^6=1$ and $c^3\ne1$, so $|c|$ is either two or six. The order-two alternative would make the displayed formula give $\chi(M)=96(1/3+1/3+1/2-1)=16$. That is impossible for a connected closed oriented [topological surface](../../../../../topological-surface.md), whose [Euler characteristic](../../../../../euler-characteristic.md) is $2-2g\leq2$. Thus $|c|=6$, and

$$
\boxed{\chi(M)=96\left(\frac13+\frac13+\frac16-1\right)=-16,
\qquad g(M)=9.}
$$

Each $U_i$ has order eight. By [Lagrange's theorem](../../../../../lagrange-s-theorem.md), it contains no element of order three or six, so it meets all conjugates of $\langle a\rangle$ and $\langle b\rangle$ trivially. In $\langle c\rangle$, the only nonidentity element whose order divides eight is $z=c^3$. Since $z$ is central, it is also the unique such element in every conjugate of $\langle c\rangle$, and it is excluded from both $U_i$ by hypothesis. Both subgroup actions are therefore free. The quotients are closed oriented surfaces with

$$
\boxed{\chi(U_i\backslash M)=-16/8=-2,\qquad g(U_i\backslash M)=2.}
$$

The branched-cover construction supplies a smooth structure, with the stabilisers acting by rotations in the disk charts. Average a smooth [Riemannian metric](../../../../../riemannian-metric.md) over $T$ to make the whole action isometric. The [Gassmann equivalence](../../../../../gassmann-equivalence.md) of $U_1,U_2$ then gives [isospectral manifolds](../../../../../isospectral-manifolds.md): for every upstairs [eigenspace](../../../../../eigenspace.md) with [character](../../../../../character-of-a-representation.md) $\chi_\lambda$, its downstairs multiplicities are $|U_i|^{-1}\sum_{u\in U_i}\chi_\lambda(u)$, and these are equal because the two subgroups have equal intersection sizes with every [conjugacy class](../../../../../conjugacy-class.md). This proves the spectral assertion for any such invariant metric.

To guarantee nonisometry, choose the invariant metric with [curvature markers distinguishing finite-cover quotients](../../../../../curvature-markers-distinguishing-finite-cover-quotients.md). Here are the geometric details, since nonconjugacy alone would not guarantee nonisometry for an arbitrary metric. Choose a small disk in the free locus of the $T$-action, with all its translates disjoint. In that disk choose three noncollinear points in a geodesically convex neighbourhood. Supported conformal [smooth bump functions](../../../../../smooth-bump-function.md) can give them three distinct high values as strict [Gaussian curvature](../../../../../gaussian-curvature.md) maxima, occurring nowhere else in the unmodified metric. Arrange these three maxima as one tight cluster, much closer to each other than to any translated cluster, and copy the same modification to every translate. Curvature and its first few derivatives can be adjusted by the second and higher derivatives of the conformal factor; narrow bumps give high distinguished curvature with small change in metric distances. Further small supported perturbations remove accidental maxima of these exact heights. Thus the resulting metric remains smooth and $T$-invariant, and its marked clusters are intrinsic and uniquely labelled by their three curvature values.

Any proposed quotient [isometry](../../../../../isometry.md) $F:U_1\backslash M\to U_2\backslash M$ must carry a whole labelled cluster to another. Lift its restriction near that cluster to the corresponding two marked disks in $M$, and identify these disks using the appropriate group element $t\in T$. The resulting local [isometry](../../../../../isometry.md) fixes all three marked points. Its differential at the first point fixes the two independent directions of the unique geodesics to the other two; hence it is the identity, and the local [isometry](../../../../../isometry.md) itself is the identity near that point. If $p_i:M\to U_i\backslash M$ are the quotient maps, we therefore have

$$
F\circ p_1=p_2\circ t
$$

on an open set. Both sides are local [isometries](../../../../../isometry.md) on the connected complete [Riemannian surface](../../../../../riemannian-surface.md) $M$. A local [isometry](../../../../../isometry.md) is determined along each [geodesic](../../../../../geodesic.md) by its value and differential at the initial point, so the equality propagates to all of $M$.

For $u\in U_1$, this equality implies $p_2\circ tu=p_2\circ t$. Evaluating at a free point of the $T$-action shows $tut^{-1}\in U_2$; equivalently these maps differ by a [deck transformation](../../../../../deck-transformation.md) of $p_2$. Thus $tU_1t^{-1}\subseteq U_2$, and equality of subgroup orders gives equality. This contradicts their assumed nonconjugacy. **For this marked invariant metric the two quotients are nonisometric, isospectral Riemannian surfaces of genus two.** No constant-curvature requirement is imposed or used.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
