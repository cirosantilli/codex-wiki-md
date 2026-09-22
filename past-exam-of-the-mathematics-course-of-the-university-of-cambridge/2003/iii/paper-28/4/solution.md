<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the [Loop theorem](../../../../../loop-theorem.md), start with a nullhomotopy $f:(D^2,\partial D^2)\to(M,\partial M)$ whose boundary represents a nontrivial boundary-group element. The required conclusion is an embedded [compression disk](../../../../../compression-disk.md), whose boundary may differ from that original loop. A tower proof proceeds as follows.

Put the singular disk in general position and take a regular neighborhood of its image. Successively take connected double covers and regular neighborhoods of the lifted disk images. Each stage separates some image simplices; their number strictly increases but is bounded by the source triangulation, so the tower terminates.

At the top there is no connected double cover, hence $H^1(-;\mathbb Z/2)=0$. Poincare-Lefschetz duality makes every boundary component a sphere. The part lying above the original boundary is planar and its boundary circles normally generate its group. Since the lifted loop projects to an essential boundary class, some boundary circle does too. Cap that circle on the sphere and push the disk inward.

Descend each double cover. The projected embedded disk has only double arcs and circles. Innermost disk exchanges and cut-and-paste surgeries remove these. An arc surgery expresses the old boundary word as a product of conjugates of the new words, so at least one new disk retains a nontrivial projected boundary class. Circle surgery retains that class. Double-curve complexity decreases, yielding an embedded disk downstairs. Iterating reaches the required [compression disk](../../../../../compression-disk.md) in $M$.

Now let $E$ be a [knot exterior](../../../../../knot-exterior.md), and choose a meridian $\mu$ and [Seifert longitude](../../../../../seifert-longitude.md) $\lambda$ on $\partial E$. The [homology](../../../../../homology-split.md) of the exterior is $\mathbb Z$, measured by linking number with the [knot](../../../../../knot.md): $\mu$ maps to a generator and $\lambda$ to zero. This follows from [Alexander duality](../../../../../alexander-duality.md), or from a [Seifert surface](../../../../../seifert-surface.md) giving the [Seifert longitude](../../../../../seifert-longitude.md) and the linking homomorphism.

If $\pi_1(\partial E)\to\pi_1(E)$ were not injective, the [Loop theorem](../../../../../loop-theorem.md) would supply a properly embedded disk $D$ with essential boundary on the [torus](../../../../../torus.md). An essential simple curve on a [torus](../../../../../torus.md) has primitive slope $a\mu+b\lambda$, with $\gcd(a,b)=1$. Since $\partial D$ bounds a disk in the exterior, its [homology](../../../../../homology-split.md) image is zero, forcing $a=0$ and $b=\pm1$. Thus $\partial D$ is a [Seifert longitude](../../../../../seifert-longitude.md). Inside the tubular [solid torus](../../../../../solid-torus.md) it cobounds an embedded annulus with the core [knot](../../../../../knot.md). Joining that annulus to $D$, and smoothing their common boundary, gives an embedded spanning disk for the [knot](../../../../../knot.md) in $S^3$. A [knot](../../../../../knot.md) bounding such a disk is the [unknot](../../../../../unknot.md). Contraposition proves

$$
\boxed{K\text{ nontrivial}\quad\Longrightarrow\quad
\pi_1(\partial E)\hookrightarrow\pi_1(E).}
$$

Finally, $S^3\setminus K$ deformation retracts onto its exterior, so their [fundamental groups](../../../../../fundamental-group.md) agree. For the [unknot](../../../../../unknot.md) the exterior is a [solid torus](../../../../../solid-torus.md), with [fundamental group](../../../../../fundamental-group.md) $\mathbb Z$. Conversely, if the knot-complement group were $\mathbb Z$, it could not contain an injected subgroup $\pi_1(\partial E)=\mathbb Z^2$. The preceding result therefore forces the [knot](../../../../../knot.md) to be trivial. Hence

$$
\boxed{K\text{ is unknotted}\iff\pi_1(S^3\setminus K)\cong\mathbb Z.}
$$

Merely having [homology](../../../../../homology-split.md) $\mathbb Z$ would not suffice: every [knot exterior](../../../../../knot-exterior.md) has that [homology](../../../../../homology-split.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
