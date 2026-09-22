<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

To form the [connected sum of knots](../../../../../connected-sum-of-knots.md) $K_1\#K_2$, remove a short unknotted arc from each oriented [knot](../../../../../knot.md) in two disjoint balls and join the remaining endpoints by a pair of parallel arcs respecting the orientations. Equivalently, a [sphere](../../../../../sphere.md) meeting a [knot](../../../../../knot.md) in two points cuts it into two one-string [tangles](../../../../../tangle.md); close each by an arc in the [sphere](../../../../../sphere.md) to recover its summands. Sliding the small joining balls along the [knots](../../../../../knot.md) shows that the [isotopy](../../../../../isotopy.md) type does not depend on these choices. The [unknot](../../../../../unknot.md) is the identity for this operation. A [prime knot](../../../../../prime-knot.md) is a nontrivial [knot](../../../../../knot.md) such that every expression $K=K_1\#K_2$ has an [unknot](../../../../../unknot.md) summand.

We first prove [additivity of Seifert genus](../../../../../additivity-of-seifert-genus.md), which also supplies a terminating measure for decomposition. Joining minimal [Seifert surfaces](../../../../../seifert-surface.md) along their boundary arcs gives $g_s(K_1\#K_2)\leq g_s(K_1)+g_s(K_2)$. For the reverse inequality, let $F$ be a minimal-genus [Seifert surface](../../../../../seifert-surface.md) for the sum and $S$ a [splitting sphere of a knot](../../../../../splitting-sphere-of-a-knot.md). Arrange transverse intersection so that $F\cap S$ consists of one arc joining the two boundary-intersection points and some [circles](../../../../../circle.md), with the number of [circles](../../../../../circle.md) minimal among genus-minimizing [surfaces](../../../../../topological-surface.md).

Each [circle](../../../../../circle.md) separates the [sphere](../../../../../sphere.md) into two disks; since it is disjoint from the intersection arc, one disk contains neither marked endpoint. Choose an innermost such [circle](../../../../../circle.md) and its disk $D\subset S$, whose interior misses $F$. If its boundary were essential in $F$, compressing $F$ along $D$ would lower the genus of its component with boundary K: for a nonseparating curve genus drops by one, and for a separating essential curve the removed boundaryless side has positive genus. This contradicts minimal genus. Its boundary therefore bounds a disk in $F$. Replace that disk by a small push-off of $D$, removing the intersection [circle](../../../../../circle.md) without changing genus or boundary, again contradicting minimal intersection. Thus no [circles](../../../../../circle.md) remain.

Cutting $F$ along its single intersection arc gives two connected [surfaces](../../../../../topological-surface.md) with boundaries the two summand [knots](../../../../../knot.md) after the closing arcs are added. [Euler characteristic](../../../../../euler-characteristic.md) shows that their genera add to $g(F)$. Each genus is at least the minimum genus of its summand, so

$$
\boxed{g_s(K_1\#K_2)=g_s(K_1)+g_s(K_2).}
$$

Genus zero means that the [knot](../../../../../knot.md) bounds a disk and is the [unknot](../../../../../unknot.md). Every nontrivial [knot](../../../../../knot.md) therefore has positive genus. Induct on this nonnegative integer: a nontrivial nonprime [knot](../../../../../knot.md) splits into two nontrivial summands, each with strictly smaller genus by the equality above, and induction decomposes both into primes. This proves **every [knot](../../../../../knot.md) is a finite connected sum of [prime knots](../../../../../prime-knot.md)**, with the [unknot](../../../../../unknot.md) the empty sum. Uniqueness is not needed here.

For coprime integers p,q, define the [torus knot](../../../../../torus-knot.md) as the oriented parametrized curve

$$
T_{p,q}(s)=2^{-1/2}(e^{ips},e^{iqs})\subset S^3\subset\mathbb C^2,\qquad s\in\mathbb R/2\pi\mathbb Z.
$$

Coprimality makes it an embedded single [circle](../../../../../circle.md): two parameters with both coordinate phases equal differ by a multiple of $2\pi$. It lies on the standard unknotted [torus](../../../../../torus.md) separating the two [solid tori](../../../../../solid-torus.md). Negative exponents change the slope/[orientation](../../../../../orientation-of-a-simplex.md) convention; they are allowed. If an exponent is zero, coprimality forces the other to be plus or minus one, giving an [unknot](../../../../../unknot.md).

Assume now $|p|,|q|\geq2$. We give a group-theoretic proof that [torus knots are prime](../../../../../torus-knots-are-prime.md), making the peripheral ingredient explicit. The [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) applied to the two solid-torus sides of the exterior, joined along the annulus parallel to the [knot](../../../../../knot.md), gives

$$
G=\langle a,b\mid a^p=b^q\rangle.
$$

Here a and b are the two core loops. The element $z=a^p=b^q$ is central. Under the [abelianization](../../../../../abelianization.md) $G\to\mathbb Z$, choose $a\mapsto q$, $b\mapsto p$; these generate the target because p,q are coprime. Thus $z\mapsto pq\ne0$, so z is nontrivial. A meridian has, up to conjugacy, the form $m=a^ub^v$ with $qu+pv=1$. This follows by tracing the meridional disk across the two [torus](../../../../../torus.md) sides, using a dual primitive slope intersecting the [knot](../../../../../knot.md) slope once. Different Bezout solutions change u by a multiple of p and v by the opposite multiple of q, leaving the same word because z is central.

Quotienting by z gives $G/\langle z\rangle=C_{|p|}*C_{|q|}$. Neither u nor v is zero modulo the corresponding cyclic order, by $qu+pv=1$. Hence the image of m is a cyclically reduced word of two syllables. All its nonzero powers remain reduced, so it has infinite order. In particular G is nonabelian and the [knot](../../../../../knot.md) is not an [unknot](../../../../../unknot.md).

We use the [Loop theorem](../../../../../loop-theorem.md) in its usual form: a noninjective boundary fundamental-group map of a three-manifold supplies an embedded compression disk. For a nontrivial [knot](../../../../../knot.md), its boundary [torus](../../../../../torus.md) is incompressible. To see why, every [sphere](../../../../../sphere.md) in its exterior bounds a ball on the side not containing the [knot](../../../../../knot.md), by the [Schoenflies theorem](../../../../../schoenflies-theorem.md). A compression of the boundary [torus](../../../../../torus.md) would produce a [sphere](../../../../../sphere.md) and make the exterior a solid [torus](../../../../../torus.md). The compression disk has zero [homology](../../../../../homology-split.md) class in the exterior, so its boundary is the preferred longitude; attaching the annulus from that longitude to the [knot](../../../../../knot.md) gives a spanning disk and an [unknot](../../../../../unknot.md). This proves that [nontrivial knot exteriors have incompressible boundary](../../../../../nontrivial-knot-exteriors-have-incompressible-boundary.md). Their peripheral [groups](../../../../../group-split.md) inject as $\mathbb Z^2$, so their [groups](../../../../../group-split.md) strictly contain the cyclic meridian subgroup.

If the [torus knot](../../../../../torus-knot.md) were a connected sum of two nontrivial [knots](../../../../../knot.md), van Kampen on the decomposing annulus would give $G=G_1*_{\langle m\rangle}G_2$, with the meridian subgroup proper in each factor. The [center of a proper amalgam lies in the amalgamated subgroup](../../../../../center-of-a-proper-amalgam-lies-in-the-amalgamated-subgroup.md). One proof uses its [Bass-Serre tree](../../../../../bass-serre-tree.md): a central elliptic element fixes a vertex orbit and its convex hull, which is the whole tree; a central translation would force the minimal tree to be its invariant axis, but a nontrivial vertex reflection reverses that translation. Thus a central element fixes every edge and lies in the edge subgroup.

The central element z would therefore equal $m^k$. Its image in $G/\langle z\rangle$ would give $\overline m^k=1$, forcing $k=0$ because that image has infinite order. This contradicts $z\ne1$. Consequently

$$
\boxed{T_{p,q}\text{ is prime whenever }\gcd(p,q)=1,\quad |p|,|q|\geq2.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
