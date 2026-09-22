<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For fixed $g\geq2$, [Mumford's compactness theorem](../../../../../../mumford-s-compactness-theorem.md) states that

$$
\boxed{\mathcal M_g^\varepsilon
=\{X\in\mathcal M_g:\operatorname{sys}_{\rm hyp}(X)\geq\varepsilon\}
\text{ is compact for every }\varepsilon>0.}
$$

Here $\mathcal M_g$ is the unmarked [moduli space of Riemann surfaces](../../../../../../moduli-space-of-riemann-surfaces.md), with its usual topology, and the [hyperbolic systole](../../../../../../hyperbolic-systole.md) is the shortest nonconstant closed hyperbolic [geodesic](../../../../../../geodesic.md), in [Gaussian curvature](../../../../../../gaussian-curvature.md) $-1$. Equivalently, a subset of $\mathcal M_g$ is relatively [compact](../../../../../../compact-space.md) exactly when its [hyperbolic systoles](../../../../../../hyperbolic-systole.md) have a common positive lower bound.

We use two standard structural results. The [Bers pants decomposition theorem](../../../../../../bers-pants-decomposition-theorem.md) provides a constant $B_g$ such that every closed [genus](../../../../../../genus-of-a-surface.md)-$g$ [hyperbolic surface](../../../../../../hyperbolic-surface.md) has a [pants decomposition](../../../../../../pants-decomposition.md) with all $3g-3$ cuff lengths at most $B_g$. For a fixed topological [pants decomposition](../../../../../../pants-decomposition.md), the [Fenchel–Nielsen coordinates](../../../../../../fenchel-nielsen-coordinates.md) identify [Teichmüller space](../../../../../../teichmuller-space.md) with

$$
(0,\infty)^{3g-3}\times\mathbb R^{3g-3}.
$$

The length coordinates are $\ell_i$, and the twist coordinates $\tau_i$ are measured in length units: a full [Dehn twist](../../../../../../dehn-twist.md) changes $\tau_i$ by $\ell_i$. Reconstruction from these coordinates is continuous; locally the marked metrics can be chosen to vary smoothly on a fixed reference surface, and the quotient by the [mapping class group](../../../../../../mapping-class-group.md) is the Hausdorff [moduli space of Riemann surfaces](../../../../../../moduli-space-of-riemann-surfaces.md).

Take any sequence in $\mathcal M_g^\varepsilon$. The [pants decompositions](../../../../../../pants-decomposition.md) supplied by the [Bers pants decomposition theorem](../../../../../../bers-pants-decomposition-theorem.md) have cuff lengths in $[\varepsilon,B_g]$. There are finitely many topological types of [pants decomposition](../../../../../../pants-decomposition.md): their dual graphs have $2g-2$ vertices and $3g-3$ edges, with loops and multiple edges allowed, giving finitely many finite graphs. Choose a subsequence of one type, and choose markings carrying each decomposition to a fixed reference one. Compose these markings with [Dehn twists](../../../../../../dehn-twist.md) so that $0\leq\tau_i\leq\ell_i$. The resulting points of [Teichmüller space](../../../../../../teichmuller-space.md) lie in the [compact](../../../../../../compact-space.md) box

$$
[\varepsilon,B_g]^{3g-3}\times[0,B_g]^{3g-3}.
$$

They therefore have a convergent subsequence inside [Teichmüller space](../../../../../../teichmuller-space.md); its continuous projection gives a convergent subsequence in the [moduli space of Riemann surfaces](../../../../../../moduli-space-of-riemann-surfaces.md). If $\varepsilon>B_g$ the thick set is empty, which is already [compact](../../../../../../compact-space.md). Equivalently, using all the finitely many reference decompositions gives a finite union of [compact](../../../../../../compact-space.md) projected boxes containing the whole thick set.

Finally the [hyperbolic systole](../../../../../../hyperbolic-systole.md) is continuous. Nearby marked [hyperbolic surfaces](../../../../../../hyperbolic-surface.md) admit metric comparisons with [bi-Lipschitz distortion](../../../../../../stretch-factor.md) tending to one; the length of every loop, and hence the [infimum](../../../../../../infimum.md) over all essential loops, obeys the same multiplicative comparison. Therefore $\mathcal M_g^\varepsilon$ is closed in that [compact](../../../../../../compact-space.md) union and is [compact](../../../../../../compact-space.md). A [compact](../../../../../../compact-space.md) subset has a positive minimum [hyperbolic systole](../../../../../../hyperbolic-systole.md), proving the converse characterization of relative compactness. This theorem concerns the unmarked quotient: repeated [Dehn twists](../../../../../../dehn-twist.md) can give an unbounded sequence in [Teichmüller space](../../../../../../teichmuller-space.md) while leaving the underlying surface and its [hyperbolic systole](../../../../../../hyperbolic-systole.md) unchanged.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
