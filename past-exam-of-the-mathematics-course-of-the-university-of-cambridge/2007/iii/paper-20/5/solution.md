<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Throughout the hyperbolic discussion take curvature $-1$ and $g\geq2$. A [Y-piece](../../../../../hyperbolic-y-piece.md) is a [pair of pants](../../../../../pair-of-pants-mathematics.md) with a [hyperbolic metric](../../../../../hyperbolic-metric.md) and three [geodesic](../../../../../geodesic.md) boundary components. Three labelled positive boundary lengths $\ell_1,\ell_2,\ell_3$ determine it up to [isometry](../../../../../isometry.md). To see existence and uniqueness, cut along the three shortest perpendicular seams. The two resulting [right-angled hyperbolic hexagons](../../../../../right-angled-hyperbolic-hexagon.md) have alternating side lengths $\ell_i/2$, which determine each hexagon. Conversely, any three positive alternating lengths produce such a hexagon, and doubling along the other sides produces the desired [Y-piece](../../../../../hyperbolic-y-piece.md). In particular the seam opposite $\ell_i$ satisfies

$$
\cosh s_i=\frac{\cosh(\ell_i/2)+\cosh(\ell_j/2)\cosh(\ell_k/2)}{\sinh(\ell_j/2)\sinh(\ell_k/2)}.
$$

An [X-piece](../../../../../hyperbolic-x-piece.md) is a four-holed hyperbolic sphere with [geodesic](../../../../../geodesic.md) boundaries, obtained by joining two [Y-pieces](../../../../../hyperbolic-y-piece.md) along one pair of equal-length boundaries. For a chosen separating curve, it is determined by

$$
\boxed{\ell_1,\ell_2,\ell_3,\ell_4>0,\quad s>0,\quad\tau},
$$

where $s$ is the common gluing length and $\tau$ is the relative arclength twist, measured between chosen seam endpoints. The identification reverses [boundary orientation](../../../../../boundary-orientation.md) so that the surface is oriented. For an unmarked gluing, $\tau$ is periodic modulo $s$; a marking retains $\tau\in\mathbb R$, because a full [Dehn twist](../../../../../dehn-twist.md) changes the marking. These six parameters describe the [X-piece](../../../../../hyperbolic-x-piece.md) with its chosen separating curve; different curve choices or boundary symmetries can describe the same unmarked surface.

Choose a [pants decomposition](../../../../../pants-decomposition.md) of a closed oriented [genus](../../../../../genus-of-a-surface.md)-$g$ surface. Each [Y-piece](../../../../../hyperbolic-y-piece.md) has [Euler characteristic](../../../../../euler-characteristic.md) $-1$, and gluing boundary circles does not change the total [Euler characteristic](../../../../../euler-characteristic.md). Thus there are $2g-2$ pieces. Their $3(2g-2)$ boundary circles are paired, giving $3g-3$ gluing curves. Choose their disjoint [geodesic](../../../../../geodesic.md) representatives, then prescribe each cuff length and its relative twist. The [Fenchel–Nielsen coordinates](../../../../../fenchel-nielsen-coordinates.md) are

$$
\boxed{(\ell_i,\tau_i)_{i=1}^{3g-3}\in(0,\infty)^{3g-3}\times\mathbb R^{3g-3}}.
$$

They determine the marked [hyperbolic surface](../../../../../hyperbolic-surface.md) and hence its unmarked [isometry](../../../../../isometry.md) class, with $6g-6$ real parameters. One must also fix the combinatorial gluing pattern of the chosen [pants decomposition](../../../../../pants-decomposition.md). Full twists and other changes of marking identify some parameter sets in unmarked [moduli space of Riemann surfaces](../../../../../moduli-space-of-riemann-surfaces.md). The [genus](../../../../../genus-of-a-surface.md) restriction matters: a sphere and a torus do not admit a closed curvature-$-1$ metric or such a decomposition into [geodesic](../../../../../geodesic.md) [Y-pieces](../../../../../hyperbolic-y-piece.md).

For a fixed oriented topological surface $S_g$, [Teichmüller space](../../../../../teichmuller-space.md) $\mathcal T_g$ consists of marked [Riemann surfaces](../../../../../riemann-surfaces.md) $(X,f:S_g\to X)$. Two markings represent the same point when a [conformal isomorphism](../../../../../biholomorphism.md) between the surfaces carries one marking to the other up to [homotopy](../../../../../homotopy.md). By the [uniformization theorem](../../../../../uniformization-theorem.md), for $g\geq2$ these are equivalently marked curvature-$-1$ metrics. The displayed [Fenchel–Nielsen coordinates](../../../../../fenchel-nielsen-coordinates.md) identify $\mathcal T_g$ with a cell of real dimension $6g-6$; the [mapping class group](../../../../../mapping-class-group.md) quotient gives the unmarked [moduli space of Riemann surfaces](../../../../../moduli-space-of-riemann-surfaces.md).

The spectral version of the [Wolpert generic spectral rigidity theorem](../../../../../wolpert-generic-spectral-rigidity-theorem.md) says that **outside a closed proper real-analytic exceptional subset of $\mathcal T_g$, the Laplace spectrum determines the [hyperbolic surface](../../../../../hyperbolic-surface.md) up to [isometry](../../../../../isometry.md)**. The exceptional subset has positive codimension and is invariant under changes of marking. [Orientation](../../../../../orientation-of-a-simplex.md) reversal must be allowed, since the [Laplacian](../../../../../laplacian.md) cannot detect [orientation](../../../../../orientation-of-a-simplex.md). Equivalently, a generic surface is determined by its unmarked [length spectrum](../../../../../length-spectrum.md), counted with multiplicities. This is a generic uniqueness statement, not a claim that every isospectral pair is isometric; the construction in Question 4 lies in the exceptional locus.

Three major ingredients and their roles are as follows.

- The [Selberg trace formula](../../../../../selberg-trace-formula.md) converts the [Laplacian](../../../../../laplacian.md) spectrum into the lengths and multiplicities of closed [geodesics](../../../../../geodesic.md), and conversely. It moves the problem from [eigenvalues](../../../../../eigenvalue.md) to geometric length data, where pants and twists can be used.
- [Finite length coordinates for hyperbolic surfaces](../../../../../finite-length-coordinates-for-hyperbolic-surfaces.md) and real-analytic length functions reduce candidate spectral matchings to finitely many local analytic systems. The cuff lengths fix the [Y-pieces](../../../../../hyperbolic-y-piece.md); two transverse curves at each cuff fix its twist, giving $9g-9$ labelled length functions. Hyperbolic holonomy gives $2\cosh(\ell_\gamma/2)=|\operatorname{tr}\rho(\gamma)|$, so these lengths obey analytic [trace](../../../../../matrix-trace.md) relations. Discreteness of bounded length data, compactness in the thick part, and finite determination of those [trace](../../../../../matrix-trace.md) relations control the locally possible unlabelled matchings. A matching that is not an identity therefore lies in a proper analytic zero set.
- Geometric decoding of the persistent identities uses the [collar lemma](../../../../../collar-lemma.md) and variations of [Fenchel–Nielsen coordinates](../../../../../fenchel-nielsen-coordinates.md). Pinching a cuff makes crossing curves long while disjoint ones remain bounded; twisting controls the transverse length relations. These behaviours recover the pants incidence and the twist data, and show that a matching persisting on an open parameter set comes from a change of marking, possibly with [orientation](../../../../../orientation-of-a-simplex.md) reversal. Thus any genuinely nonisometric matching is confined to the lower-dimensional exceptional analytic locus.

For completeness, a related finiteness statement sometimes grouped with this theorem is that a fixed closed [hyperbolic surface](../../../../../hyperbolic-surface.md) has only finitely many isospectral [isometry](../../../../../isometry.md) classes. Its short proof uses three particularly concrete tools: a common discrete [length spectrum](../../../../../length-spectrum.md); [Mumford's compactness theorem](../../../../../mumford-s-compactness-theorem.md), applied to the common positive systole; and finitely many determining marked lengths. Compactness would give an accumulation point if an isospectral family were infinite. Nearby markings make each determining length converge, while discreteness of the fixed spectrum makes it eventually constant. The determining lengths then force eventual equality of the marked surfaces, a contradiction. This [finiteness of isospectral hyperbolic surfaces](../../../../../finiteness-of-isospectral-hyperbolic-surfaces.md) statement does not replace the stronger generic uniqueness assertion above.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
