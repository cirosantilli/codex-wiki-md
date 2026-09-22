<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the unique curvature $-1$ [hyperbolic metric](../../../../../hyperbolic-metric.md) on a closed [Riemann surface](../../../../../riemann-surfaces.md) of [genus](../../../../../genus-of-a-surface.md) $g\ge2$, supplied by the [uniformization theorem](../../../../../uniformization-theorem.md). This is the implicit setting for the partition and spectral theorems; a genus-zero or genus-one surface does not have this [hyperbolic metric](../../../../../hyperbolic-metric.md).

A partition is a [pants decomposition](../../../../../pants-decomposition.md) by disjoint essential simple closed [geodesics](../../../../../geodesic.md), whose complement is a union of [pairs of pants](../../../../../pair-of-pants-mathematics.md). A [pair of pants](../../../../../pair-of-pants-mathematics.md) is a sphere with three disks removed, furnished here with geodesic boundary. Its [Euler characteristic](../../../../../euler-characteristic.md) is $-1$, so there must be $2g-2$ pants. Every pant has three boundaries and every cutting curve occurs twice, giving $3g-3$ cutting curves. The [Bers pants decomposition theorem](../../../../../bers-pants-decomposition-theorem.md) asserts that a constant $B_g$ depending only on $g$ bounds the lengths of all cuffs in some such [pants decomposition](../../../../../pants-decomposition.md) of every closed genus-$g$ [hyperbolic surface](../../../../../hyperbolic-surface.md).

To see what geometry the cuffs determine, cut each [pair of pants](../../../../../pair-of-pants-mathematics.md) along its three perpendicular seams into two congruent [right-angled hyperbolic hexagons](../../../../../right-angled-hyperbolic-hexagon.md). The three alternate sides are $\ell_1/2,\ell_2/2,\ell_3/2$, where the $\ell_i>0$ are its boundary lengths. The [right-angled hyperbolic hexagon](../../../../../right-angled-hyperbolic-hexagon.md) identity determines the seam $s_i$ opposite the half-cuff $\ell_i/2$ by

$$
\cosh s_i=\frac{\cosh(\ell_i/2)+\cosh(\ell_j/2)\cosh(\ell_k/2)}{\sinh(\ell_j/2)\sinh(\ell_k/2)}.
$$

We use the standard existence and uniqueness theorem for a [right-angled hyperbolic hexagon](../../../../../right-angled-hyperbolic-hexagon.md) with prescribed positive alternating side lengths. Thus the three boundary lengths determine the [pair of pants](../../../../../pair-of-pants-mathematics.md) up to [isometry](../../../../../isometry.md).

Fix a topological [pants decomposition](../../../../../pants-decomposition.md), label its cuffs, and choose reference seam endpoints and orientations. Gluing two boundaries of the same length requires a translation along that boundary; its signed distance is a twist $\tau_i$. The gluing graph, the $3g-3$ positive cuff lengths, and the $3g-3$ twists therefore determine the unmarked [hyperbolic surface](../../../../../hyperbolic-surface.md) up to [isometry](../../../../../isometry.md). A full boundary translation has period $\ell_i$, so for an unmarked gluing one may take $0\le\tau_i<\ell_i$, with endpoints identified. For a marked surface the whole real twist records the number of [Dehn twists](../../../../../dehn-twist.md), and the [Fenchel–Nielsen coordinates](../../../../../fenchel-nielsen-coordinates.md) are

$$
\boxed{(\ell_1,\ldots,\ell_{3g-3},\tau_1,\ldots,\tau_{3g-3})\in\mathbb R_{>0}^{3g-3}\times\mathbb R^{3g-3}.}
$$

The topological gluing data are necessary when the decomposition is not fixed. Different markings or decomposition graphs can describe the same unmarked surface.

[Teichmüller space](../../../../../teichmuller-space.md) $\mathcal T_g$ consists of pairs $(X,f)$, where $X$ is a closed genus-$g$ [Riemann surface](../../../../../riemann-surfaces.md) and $f:\Sigma_g\to X$ is an orientation-preserving marking, modulo the equivalence $(X,f)\sim(Y,h)$ when a conformal orientation-preserving map $a:X\to Y$ has $a\circ f$ homotopic to $h$. The [Fenchel–Nielsen coordinates](../../../../../fenchel-nielsen-coordinates.md) identify it with $\mathbb R_{>0}^{3g-3}\times\mathbb R^{3g-3}$, of real dimension $6g-6$. The [moduli space of Riemann surfaces](../../../../../moduli-space-of-riemann-surfaces.md) forgets the marking by quotienting by the [mapping class group](../../../../../mapping-class-group.md).

The [Wolpert generic spectral rigidity theorem](../../../../../wolpert-generic-spectral-rigidity-theorem.md) says that the locus of closed genus-$g$ [hyperbolic surfaces](../../../../../hyperbolic-surface.md) possessing an isospectral but nonisometric partner lies in a locally real-analytic exceptional locus of lower dimension in [Teichmüller space](../../../../../teichmuller-space.md). Thus a generic surface is determined, up to [isometry](../../../../../isometry.md), by its unmarked [length spectrum](../../../../../length-spectrum.md), equivalently by its [Laplacian](../../../../../laplacian.md) [spectrum](../../../../../spectrum-functional-analysis.md). Here an [isometry](../../../../../isometry.md) may reverse orientation; the [length spectrum](../../../../../length-spectrum.md) cannot distinguish the two orientations of the same metric. The equivalence of the two [spectra](../../../../../spectrum-functional-analysis.md) is the compact hyperbolic [Selberg trace formula](../../../../../selberg-trace-formula.md).

The simplifying result is the [Buser finite length spectrum theorem](../../../../../buser-finite-length-spectrum-theorem.md): for every $g\ge2$ and $\varepsilon>0$ there is $L=L(g,\varepsilon)$ such that two closed genus-$g$ [hyperbolic surfaces](../../../../../hyperbolic-surface.md) with [hyperbolic systoles](../../../../../hyperbolic-systole.md) at least $\varepsilon$ have the same entire unmarked [length spectrum](../../../../../length-spectrum.md) if their length multisets up to $L$ agree. Multiplicities are included. We will count primitive unoriented [closed geodesics](../../../../../closed-geodesic.md); counting all iterates is equivalent by successively removing shorter iterates. The theorem is uniform on the thick part of [moduli space](../../../../../moduli-space.md), not merely a cutoff chosen separately for a particular pair.

Here is a proof using compactness and polynomial trace equations. We state the subsidiary facts and explain their role. First, [Mumford's compactness theorem](../../../../../mumford-s-compactness-theorem.md) makes the genus-$g$ thick moduli space compact. It can also be seen from the [Bers pants decomposition theorem](../../../../../bers-pants-decomposition-theorem.md): cuffs in a Bers decomposition lie in $[\varepsilon,B_g]$, there are finitely many [pants decomposition graphs](../../../../../pants-decomposition-graph.md), and unmarked twists may be reduced modulo their cuff lengths. These data lie in finitely many compact boxes of [Fenchel–Nielsen coordinates](../../../../../fenchel-nielsen-coordinates.md) and cover the thick moduli space.

Second, these finite compact boxes give a compact family $K$ of marked hyperbolic structures on a fixed smooth surface $\Sigma_g$ representing every member of the thick moduli space. We use the standard smooth dependence of the glued metrics and their [hyperbolic holonomy representations](../../../../../hyperbolic-holonomy-representation.md) on [Fenchel–Nielsen coordinates](../../../../../fenchel-nielsen-coordinates.md). Choose smooth representatives over finitely many parameter neighborhoods and conjugate the [hyperbolic holonomy representation](../../../../../hyperbolic-holonomy-representation.md) using a fixed lifted [Riemannian orthonormal frame](../../../../../riemannian-orthonormal-frame.md). Passing to finite compact subboxes gives a compact set of representations, together with a compact family of representative smooth metrics. Changing the markings between boxes causes no problem: all are markings from the same fixed $\Sigma_g$, and the union is finite.

Third, [uniformization theorem](../../../../../uniformization-theorem.md) identifies each marked [hyperbolic surface](../../../../../hyperbolic-surface.md) with $\mathbb H^2/\rho(\pi_1\Sigma_g)$ for a faithful discrete [hyperbolic holonomy representation](../../../../../hyperbolic-holonomy-representation.md) into $\operatorname{PSL}_2(\mathbb R)$. We use the standard lifting fact that a closed orientable [hyperbolic holonomy representation](../../../../../hyperbolic-holonomy-representation.md) admits a lift to $\operatorname{SL}_2(\mathbb R)$, and lifts may be chosen continuously on small parameter neighborhoods. Choose lifts on finitely many such neighborhoods, allowing the finitely many possible sign choices. A representation is described by the matrices of $2g$ standard [fundamental group](../../../../../fundamental-group.md) generators. The [polynomial encoding of hyperbolic geodesic lengths](../../../../../polynomial-encoding-of-hyperbolic-geodesic-lengths.md) uses, for each fixed group word $w$, its squared [matrix trace](../../../../../matrix-trace.md)

$$
p_w(\rho)=\operatorname{tr}(\rho(w))^2
$$

is a [polynomial](../../../../../polynomial-split.md) in their entries: products are polynomial, and the inverse of a determinant-one matrix is its polynomial adjugate. For a nontrivial hyperbolic word, the [hyperbolic translation length](../../../../../hyperbolic-translation-length.md) obeys

$$
p_w(\rho)=4\cosh^2\bigl(\ell_\rho(w)/2\bigr).
$$

Thus equality of the positive lengths is exactly equality of these trace polynomials, independent of lift signs.

Fourth, the [length spectrum](../../../../../length-spectrum.md) of a closed [hyperbolic surface](../../../../../hyperbolic-surface.md) is locally finite with finite multiplicities. We need the [uniform finiteness of short geodesic classes](../../../../../uniform-finiteness-of-short-geodesic-classes.md) across the compact marked family. More uniformly, for each finite $b$, only finitely many unoriented primitive [conjugacy classes](../../../../../conjugacy-class.md) can have length at most $b$ in any metric of $K$. To justify uniformity, compactness of the smooth metrics gives a common [bilipschitz equivalence](../../../../../bilipschitz-equivalence.md) comparison with one fixed metric $h_0$ on $\Sigma_g$. If $\ell_h(\alpha)\le b$, the minimizing [geodesic](../../../../../geodesic.md) has $h_0$ length at most $Cb$, so $\ell_{h_0}(\alpha)\le Cb$. Local finiteness for $h_0$ then gives a finite list. Local finiteness itself follows from proper discontinuity of the cocompact group of the [hyperbolic holonomy representation](../../../../../hyperbolic-holonomy-representation.md): conjugate a geodesic axis to meet a fixed compact fundamental set, and a bounded-length axis gives a group element moving that compact set a bounded distance, of which there are only finitely many.

Finally, the [Hilbert basis theorem](../../../../../hilbert-basis-theorem.md) says that a [polynomial ring](../../../../../polynomial-ring.md) in finitely many real variables is [Noetherian](../../../../../noetherian-ring.md). Consequently a decreasing sequence of sets cut out by polynomial equations eventually stabilizes. Indeed, their vanishing ideals form an increasing chain and stabilize. Finite unions of such sets are still algebraic: one can take all products of one defining polynomial from each component. This finiteness fact is the engine that turns arbitrarily many spectral comparisons into finitely many.

Enumerate the primitive unoriented [conjugacy classes](../../../../../conjugacy-class.md) as $\alpha_1,\alpha_2,\ldots$. For each $n$ let

$$
b_n=\max_{\rho\in K,\ 1\le i\le n}\ell_\rho(\alpha_i),
$$

and let $F_n$ be the finite set of primitive classes that can have length at most $b_n$ anywhere in $K$. Define $Z_n$ in the finite-dimensional space of pairs of generator matrices as follows: it consists of pairs $(\rho,\sigma)$ for which there exists an injection

$$
f:\{\alpha_1,\ldots,\alpha_n\}\longrightarrow F_n,
\qquad p_{\alpha_i}(\rho)=p_{f(\alpha_i)}(\sigma)\quad(1\le i\le n),
$$

and also an injection satisfying the analogous equations with $\rho$ and $\sigma$ interchanged. There are only finitely many injections. Each choice imposes finitely many [polynomial equations](../../../../../polynomial-equation.md); taking their finite unions and then intersecting the two directions proves that $Z_n$ is a real [affine algebraic set](../../../../../affine-algebraic-set.md). On determinant-one representations these equations are exactly the desired matching of lengths. Defining the polynomials on the ambient matrix-entry space is harmless; the argument will only apply them to representations in $K$.

Put $W_n=Z_1\cap\cdots\cap Z_n$. The sets $W_n$ form a decreasing chain of [affine algebraic sets](../../../../../affine-algebraic-set.md), hence for some $N$,

$$
W_N=\bigcap_{n\ge1}W_n.
$$

For representations in $K$, membership in this intersection is equivalent to equality of the full [length spectra](../../../../../length-spectrum.md). One direction follows by matching equal lengths, including their multiplicities. For the other, fix a length $\ell$. All primitive classes of length $\ell$ on the first surface occur in some finite initial segment. Its injective matching shows that the second surface has at least that multiplicity at $\ell$; the reverse injection gives the reverse inequality. Local finiteness makes both multiplicities finite. Doing this for every $\ell$ proves multiset equality.

Take

$$
L=\max_{1\le n\le N}b_n.
$$

If two surfaces in $K$ have equal length multisets up to $L$, each initial segment through $n\le N$ can be matched injectively on the other surface. Its matching classes lie in $F_n$, since the matched lengths are at most $b_n$. The reverse matching is available as well. Thus the pair belongs to $W_N$, hence to every $W_n$, and the preceding paragraph yields

$$
\boxed{\operatorname{LengthSpec}_{\le L}(X)=\operatorname{LengthSpec}_{\le L}(Y)
\ \Longrightarrow\ \operatorname{LengthSpec}(X)=\operatorname{LengthSpec}(Y).}
$$

All choices of the compact family were made using only $g$ and $\varepsilon$, so the resulting cutoff has the asserted dependence. If the thick family is empty the assertion is vacuous. This proves [Buser's finite length spectrum theorem](../../../../../buser-finite-length-spectrum-theorem.md) without claiming that equal full [length spectra](../../../../../length-spectrum.md) always force [isometry](../../../../../isometry.md); exceptional isospectral pairs are compatible with the theorem and are precisely why [Wolpert's theorem](../../../../../wolpert-generic-spectral-rigidity-theorem.md) is a generic statement.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
