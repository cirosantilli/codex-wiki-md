# Smooth manifold

↑ **Parent:** [Differential geometry](differential-geometry.md)

A smooth $k$-manifold is a Hausdorff second-countable space locally homeomorphic to $\mathbb R^k$, equipped with smoothly compatible coordinate charts.

**Table of contents**

- [Smooth embedded surface](#smooth-embedded-surface)
- [Four-manifold realization of finitely presented groups](#four-manifold-realization-of-finitely-presented-groups)
- [Product manifold](#product-manifold)
- [Band sum](#band-sum)
- [Compact manifold](#compact-manifold)
- [Closed manifold](#closed-manifold)
  - [Closed surface](#closed-surface)
  - [Connected sum of oriented manifolds](#connected-sum-of-oriented-manifolds)
    - [Connected-sum gluing of functions](#connected-sum-gluing-of-functions)
    - [Permutation diffeomorphisms of identical connected summands](#permutation-diffeomorphisms-of-identical-connected-summands)
    - [Separating projective three-space in a positive connected sum](#separating-projective-three-space-in-a-positive-connected-sum)
    - [Euler characteristic of a connected sum](#euler-characteristic-of-a-connected-sum)
    - [Cohomology ring of the connected sum of two complex projective planes](#cohomology-ring-of-the-connected-sum-of-two-complex-projective-planes)
    - [Cohomology ring of a connected sum of odd-dimensional sphere products](#cohomology-ring-of-a-connected-sum-of-odd-dimensional-sphere-products)
- [Manifold with boundary](#manifold-with-boundary)
  - [Collar neighbourhood](#collar-neighbourhood)
- [Parallelizable manifold](#parallelizable-manifold)
  - [Parallelizable sphere](#parallelizable-sphere)
    - [Quaternionic left-invariant frame on the three-sphere](#quaternionic-left-invariant-frame-on-the-three-sphere)
- [Full-row-rank matrix manifold](#full-row-rank-matrix-manifold)
- [Isotopy](#isotopy)
  - [Ambient isotopy](#ambient-isotopy)
  - [Smooth isotopy](#smooth-isotopy)
- [Boundary connected sum](#boundary-connected-sum)
- [Embedded submanifold](#embedded-submanifold)
  - [Normal-bundle obstruction to being a regular level set](#normal-bundle-obstruction-to-being-a-regular-level-set)
  - [Slice chart for an embedded submanifold](#slice-chart-for-an-embedded-submanifold)
  - [Smooth extension criterion for an immersed submanifold](#smooth-extension-criterion-for-an-immersed-submanifold)
  - [Vanishing ideal of an embedded submanifold](#vanishing-ideal-of-an-embedded-submanifold)
    - [Tangency under the Lie bracket](#tangency-under-the-lie-bracket)
  - [Transverse intersection theorem](#transverse-intersection-theorem)
  - [Clean intersection](#clean-intersection)
    - [Transverse intersection](#transverse-intersection)
      - [Smooth intersection number](#smooth-intersection-number)
- [Hypersurface](#hypersurface)
  - [Non-null hypersurface projection](#non-null-hypersurface-projection)
  - [Defining line bundle of a properly embedded hypersurface](#defining-line-bundle-of-a-properly-embedded-hypersurface)
  - [Extrinsic curvature](#extrinsic-curvature)
    - [Totally geodesic hypersurface](#totally-geodesic-hypersurface)
- [Abstract smooth surface](#abstract-smooth-surface)
  - [Smooth quotient by a free finite group action](#smooth-quotient-by-a-free-finite-group-action)
- [Smooth map between manifolds](#smooth-map-between-manifolds)
  - [Smooth approximation of maps into Euclidean space](#smooth-approximation-of-maps-into-euclidean-space)
  - [Transversality of a map to a submanifold](#transversality-of-a-map-to-a-submanifold)
    - [General position for curves in a manifold](#general-position-for-curves-in-a-manifold)
    - [Transverse preimage theorem](#transverse-preimage-theorem)
  - [Pushforward of a curve](#pushforward-of-a-curve)
  - [Pullback of a smooth function](#pullback-of-a-smooth-function)
  - [Differential of a smooth map](#differential-of-a-smooth-map)
    - [Differential of a smooth function](#differential-of-a-smooth-function)
    - [Zero-differential constancy theorem](#zero-differential-constancy-theorem)
    - [Pushforward of a contravariant tensor](#pushforward-of-a-contravariant-tensor)
    - [Pullback of a covariant tensor](#pullback-of-a-covariant-tensor)
      - [Pullback of a covector](#pullback-of-a-covector)
    - [Pushforward of a vector field](#pushforward-of-a-vector-field)
      - [Diffeomorphism invariance of a vector field is equivalent to commuting with its local flow](#diffeomorphism-invariance-of-a-vector-field-is-equivalent-to-commuting-with-its-local-flow)
      - [Projectable vector field](#projectable-vector-field)
- [Local flow](#local-flow)
  - [Complete vector field](#complete-vector-field)
    - [Complete vector fields need not be closed under addition or Lie brackets](#complete-vector-fields-need-not-be-closed-under-addition-or-lie-brackets)
  - [Straightening theorem](#straightening-theorem)
- [Partition of unity](#partition-of-unity)
- [Orientable smooth manifold](#orientable-smooth-manifold)
  - [Orientation of a smooth manifold](#orientation-of-a-smooth-manifold)
  - [Oriented atlas](#oriented-atlas)
  - [Outward-normal-first boundary orientation](#outward-normal-first-boundary-orientation)
  - [Equivalent formulations of orientability of a smooth manifold](#equivalent-formulations-of-orientability-of-a-smooth-manifold)
  - [Orientability of factors of a product manifold](#orientability-of-factors-of-a-product-manifold)
  - [Orientation-reversing diffeomorphism](#orientation-reversing-diffeomorphism)

## Smooth embedded surface

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

A smooth embedded surface in $\mathbb R^3$ is a two-dimensional [smooth manifold](smooth-manifold.md) locally represented by an injective regular [parametrized surface](multivariable-calculus.md#parametrized-surface) $\sigma:U\subset\mathbb R^2\to\mathbb R^3$, with $\sigma_u\times\sigma_v\ne0$. The [first fundamental form](differential-geometry.md#first-fundamental-form) measures lengths and angles, and a choice of [unit normal](differential-geometry.md#unit-normal) determines the [second fundamental form](second-fundamental-form.md), which measures bending. A surface with boundary additionally uses local half-plane charts along its boundary.

## Four-manifold realization of finitely presented groups

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

Every finitely presented [group](group.md) is the [fundamental group](algebraic-topology.md#fundamental-group) of a closed connected smooth oriented four-manifold. Build a compact four-dimensional [handle decomposition](topological-manifold.md#handle-decomposition) with one zero-handle, a one-handle for each [generator of a group](group.md#generator-of-a-group) and a two-handle for each [relator](geometric-group-theory.md#relator). Turning the [handle decomposition](topological-manifold.md#handle-decomposition) upside down shows that its boundary surjects on the [fundamental group](algebraic-topology.md#fundamental-group). Its [double of a manifold](topological-manifold.md#double-of-a-manifold) has the same [fundamental group](algebraic-topology.md#fundamental-group) by the [Seifert-van Kampen theorem](algebraic-topology.md#seifert-van-kampen-theorem).

## Product manifold

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

Products of [manifold charts](differential-geometry.md#manifold-chart) form a [smooth atlas](differential-geometry.md#smooth-atlas) on the topological product of two [smooth manifolds](smooth-manifold.md). The transition maps are products of the two smooth transition maps, so the [dimension](vector-space.md#dimension-vector-space) is the sum of the dimensions. The smooth structure is independent of the chosen compatible atlases.

## Band sum

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

A band sum joins two embedded spheres or links by a narrow tube along an arc, removing a small disk from each and joining their boundaries. In a [handle slide](topological-manifold.md#handle-slide), the construction uses a parallel framed copy of the second [attaching sphere](topological-manifold.md#attaching-sphere) and transports its [framing of an embedded sphere](algebraic-geometry.md#framing-of-an-embedded-sphere) along the band.

## Compact manifold

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

A compact manifold is a [smooth manifold](smooth-manifold.md) whose underlying [topological space](topology.md#topological-space) is [compact](topology.md#compact-space). Every smooth [vector field](multivariable-calculus.md#vector-field) on a compact manifold without boundary has a flow defined for all real time. On a manifold with boundary, tangency to the boundary or an appropriate inward-flow condition must also be imposed.

## Closed manifold

↑ **Parent:** [Smooth manifold](smooth-manifold.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed_manifold)

A closed manifold is a compact [manifold with boundary](#manifold-with-boundary) whose boundary is empty. Here “closed” includes compactness.

### Closed surface

↑ **Parent:** [Closed manifold](#closed-manifold)

A [compact](topology.md#compact-space) two-dimensional [manifold](topological-manifold.md) without boundary. A [connected](geometry-and-topology.md#connected-space) [oriented surface](differential-geometry.md#oriented-surface) is classified by its [genus](topological-surface.md#genus-of-a-surface); for [genus](topological-surface.md#genus-of-a-surface) $g$ its [Euler characteristic](homology.md#euler-characteristic) is $2-2g$.

### Connected sum of oriented manifolds

↑ **Parent:** [Closed manifold](#closed-manifold)

For connected oriented closed $d$-dimensional [manifolds](topological-manifold.md) with $d\geq2$, their connected sum removes an open $d$-dimensional ball from each and identifies the resulting boundary [spheres](euclidean-geometry.md#sphere) by an [orientation-reversing diffeomorphism](#orientation-reversing-diffeomorphism). The remaining orientations fit together. Collapsing the separating sphere gives a [pinch map](topology.md#pinch-map) to the [wedge sum](topology.md#wedge-sum) of the two closed manifolds, and projection to either summand has [degree of a continuous mapping](homology.md#degree-of-a-continuous-mapping) one. In intermediate positive degrees the [cohomology](cohomology.md) is the direct sum of the summand groups. Products of classes from different summands vanish; products landing in top degree use the single common [orientation class](cohomology.md#fundamental-class). These statements follow from [excision](homology.md#excision-theorem), the [Mayer–Vietoris sequence](algebraic-topology.md#mayer-vietoris-sequence) and the degree-one projections.

#### Connected-sum gluing of functions

↑ **Parent:** [Connected sum of oriented manifolds](#connected-sum-of-oriented-manifolds)

Remove small [disks](topology.md#disk-mathematics) around a nondegenerate maximum of a [smooth function](analysis.md#smooth-function) on one closed [surface](topological-surface.md) and a nondegenerate minimum on another. Rescale their values so the boundary values agree with the two ends of a neck. Their regular level collars allow a strictly monotone function on the neck, with nonzero derivative, matching smoothly to both sides. The resulting [connected sum](#connected-sum-of-oriented-manifolds) has all the old [critical points](analysis.md#critical-point) except the deleted maximum and minimum. This permits one degenerate [torus](topological-surface.md#torus) saddle to be retained while adding ordinary [handles](topological-manifold.md#handle) for higher genus.

#### Permutation diffeomorphisms of identical connected summands

↑ **Parent:** [Connected sum of oriented manifolds](#connected-sum-of-oriented-manifolds)

For a connected sum of identical oriented manifolds of dimension at least three, one can permute the attachment balls in a punctured sphere and match the attached copies by their chosen parametrizations. This gives orientation-preserving diffeomorphisms realizing the permutations on the middle cohomology summands. For sums of complex projective planes, these permutations preserve the diagonal positive intersection form.

// Destination: geometry-and-topology.bigb

#### Separating projective three-space in a positive connected sum

↑ **Parent:** [Connected sum of oriented manifolds](#connected-sum-of-oriented-manifolds)

Tube the projective lines in the two summands of $\mathbb{CP}^2\#\mathbb{CP}^2$ through the connecting neck. Their connected sum is an embedded two-sphere in the class $h_1+h_2$, with self-intersection two. Its oriented normal disk bundle has Euler number two, so its boundary is the [unit tangent bundle](vector-bundle.md#unit-tangent-bundle) of $S^2$, namely $SO(3)\cong\mathbb{RP}^3$. The boundary separates the interior of the tubular neighborhood from its nonempty exterior.

// Destination: geometry-and-topology.bigb

#### Euler characteristic of a connected sum

↑ **Parent:** [Connected sum of oriented manifolds](#connected-sum-of-oriented-manifolds)

For closed connected oriented $d$-manifolds with $d\geq2$,

$$
\chi(M\#N)=\chi(M)+\chi(N)-\chi(S^d).
$$

Deleting an open ball changes the [Euler characteristic](homology.md#euler-characteristic) by $-1+\chi(S^{d-1})$, and gluing subtracts $\chi(S^{d-1})$. Since $\chi(S^{d-1})+\chi(S^d)=2$, the formula follows. Thus a [connected sum of oriented manifolds](#connected-sum-of-oriented-manifolds) subtracts two from the sum of Euler characteristics in even dimension and subtracts zero in odd dimension.

#### Cohomology ring of the connected sum of two complex projective planes

↑ **Parent:** [Connected sum of oriented manifolds](#connected-sum-of-oriented-manifolds)

For the standard complex orientations, the two summand classes have zero product and equal squares, the oriented degree-four class. The quadratic relations imply all cubic monomials vanish. The rational Betti numbers are $1,2,1$ in degrees zero, two and four.

#### Cohomology ring of a connected sum of odd-dimensional sphere products

↑ **Parent:** [Connected sum of oriented manifolds](#connected-sum-of-oriented-manifolds)

For odd $r\geq1$ and $W_g=\mathbin\#_{i=1}^g(S^r\times S^r)$, the [integral cohomology](cohomology.md#integral-cohomology) has one copy of $\mathbb Z$ in degrees zero and $2r$, $\mathbb Z^{2g}$ in degree $r$, and zero elsewhere. Choose the top [orientation class](cohomology.md#fundamental-class) $\omega$ and degree-$r$ classes $\alpha_i,\beta_i$ from the two factors of summand $i$. Their nonzero positive-degree basis products are

$$
\alpha_i\smile\beta_j=\delta_{ij}\omega,\qquad \beta_j\smile\alpha_i=-\delta_{ij}\omega.
$$

All $\alpha_i\alpha_j$ and $\beta_i\beta_j$ vanish, and $\omega$ annihilates positive-degree classes. The [Künneth theorem](cohomology.md#kunneth-theorem) computes each sphere product; the [Mayer–Vietoris sequence](algebraic-topology.md#mayer-vietoris-sequence) computes the connected sum groups, and its degree-one [pinch maps](topology.md#pinch-map) determine the products. Thus its middle-degree [Poincare duality pairing](cohomology.md#poincare-duality-pairing) is a [symplectic vector space](bilinear-form.md#symplectic-vector-space) after changing coefficients to a field of characteristic different from two. The case $r=1$ is the usual [cohomology ring of a closed oriented surface](cohomology.md#cohomology-ring-of-a-closed-oriented-surface).

## Manifold with boundary

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

A smooth manifold with boundary has charts in the half-space $\{x_n\geq0\}\subseteq\mathbb R^n$, with smoothly compatible transition maps. The boundary is the locus modeled on $x_n=0$.

### Collar neighbourhood

↑ **Parent:** [Manifold with boundary](#manifold-with-boundary)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Collar_neighbourhood)

A collar neighborhood identifies a neighborhood of the boundary with $\partial W\times[0,\varepsilon)$, with the boundary at parameter zero. It allows a manifold's boundary to be pushed slightly inward by a [homotopy](homotopy.md).

## Parallelizable manifold

↑ **Parent:** [Smooth manifold](smooth-manifold.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parallelizable_manifold)

A parallelizable manifold is a smooth $n$-manifold whose tangent bundle is trivial, equivalently one admitting $n$ smooth vector fields that form a basis of every tangent space. Every [Lie group](lie-theory.md#lie-group) is parallelizable because a basis at the identity extends to a global frame by left translation.

### Parallelizable sphere

↑ **Parent:** [Parallelizable manifold](#parallelizable-manifold)

Among positive-dimensional spheres, precisely $S^1$, $S^3$, and $S^7$ are parallelizable. The circle and three-sphere inherit Lie-group frames from $U(1)$ and $SU(2)$; the seven-sphere has a frame constructed from octonion multiplication.

#### Quaternionic left-invariant frame on the three-sphere

↑ **Parent:** [Parallelizable sphere](#parallelizable-sphere)

For $q=(q_0,q_1,q_2,q_3)\in S^3$, the vectors $(-q_1,q_0,q_3,-q_2)$, $(-q_2,-q_3,q_0,q_1)$ and $(-q_3,q_2,-q_1,q_0)$ are tangent and orthonormal. Under [SU(2) as the three-sphere](topological-group.md#su-2-as-the-three-sphere) they are the [left-invariant vector fields](lie-theory.md#left-invariant-vector-field) obtained by translating $-i$ times the [Pauli matrices](algebra.md#pauli-matrices). This explicitly realizes the [parallelization of a Lie group by left translations](lie-theory.md#parallelization-of-a-lie-group-by-left-translations).

## Full-row-rank matrix manifold

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

The real $m$ by $n$ matrices of [matrix rank](vector-space.md#matrix-rank) $m\leq n$ form an open [smooth manifold](smooth-manifold.md) $X_{m,n}\subseteq\mathbb R^{mn}$. Indeed, it is the union of the open sets on which a chosen $m$ by $m$ minor has nonzero [determinant](multilinear-algebra.md#determinant), so its dimension is $mn$.

## Isotopy

↑ **Parent:** [Smooth manifold](smooth-manifold.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isotopy)

An isotopy is a continuous one-parameter family of embeddings or homeomorphisms beginning at a given map.

### Ambient isotopy

↑ **Parent:** [Isotopy](#isotopy)

Two embeddings $f_0,f_1:N\hookrightarrow M$ are ambient isotopic when a continuously varying family of ambient [homeomorphisms](topology.md#homeomorphism) $F_t$ starting at the identity satisfies $F_1f_0=f_1$. This is stronger than an arbitrary homotopy of maps. Smooth versions use smooth families of diffeomorphisms; unparametrized versions identify embedded images, and oriented versions preserve their orientations.

### Smooth isotopy

↑ **Parent:** [Isotopy](#isotopy)

A smooth isotopy is a smooth family of [smooth embeddings](differential-geometry.md#smooth-embedding) or [diffeomorphisms](geometry-and-topology.md#diffeomorphism) parametrized by an interval and beginning at the given map.

## Boundary connected sum

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

The boundary connected sum of two manifolds with boundary removes a boundary half-ball from each and glues the resulting hemispherical faces. Its boundary is the ordinary connected sum of the original boundaries.

This boundary gluing operation is related to the [connected sum](#connected-sum-of-oriented-manifolds), but applies along boundary disks rather than removing interior balls.

## Embedded submanifold

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

An embedded submanifold $M\subseteq N$ is a subset whose inclusion is an embedding. Around every point there are coordinates on $N$ in which $M$ is a coordinate plane.

An embedded submanifold is a [submanifold](differential-geometry.md#submanifold) for which the inclusion gives the subspace topology, unlike a merely immersed submanifold.

### Normal-bundle obstruction to being a regular level set

↑ **Parent:** [Embedded submanifold](#embedded-submanifold)

If an embedded codimension-$k$ submanifold $X\subset M$ is $f^{-1}(y)$ for a [regular value](differential-geometry.md#regular-value) $y$ of a smooth map $f:M\to\mathbb R^k$, then $df$ identifies its [normal bundle](algebraic-geometry.md#normal-bundle) with the trivial bundle $X\times\mathbb R^k$. A submanifold with nontrivial normal bundle therefore cannot be such a regular level set. The core circle of the [Möbius band](topological-surface.md#mobius-band) is a codimension-one example.

### Slice chart for an embedded submanifold

↑ **Parent:** [Embedded submanifold](#embedded-submanifold)

If $N^n\subset M^m$ is embedded and $p\in N$, there are smooth coordinates $(x^1,\ldots,x^m)$ around $p$ in which

$$
N=\{x^{n+1}=\cdots=x^m=0\}.
$$

The first $n$ coordinates restrict to a chart on $N$.

### Smooth extension criterion for an immersed submanifold

↑ **Parent:** [Embedded submanifold](#embedded-submanifold)

An injectively immersed submanifold $N\subset M$ is embedded if every smooth function on $N$ extends to a smooth function on $M$. Otherwise a sequence from a different local sheet can converge in $M$ to a point $p$ while remaining outside a small embedded neighborhood of $p$ in $N$; a bump function supported on that neighborhood cannot have a continuous ambient extension.

### Vanishing ideal of an embedded submanifold

↑ **Parent:** [Embedded submanifold](#embedded-submanifold)

The vanishing ideal is $I(N)=\{f\in C^\infty(M):f|_N=0\}$. A vector field $X$ is tangent to $N$ exactly when $X(I(N))\subseteq I(N)$.

#### Tangency under the Lie bracket

↑ **Parent:** [Vanishing ideal of an embedded submanifold](#vanishing-ideal-of-an-embedded-submanifold)

If $X$ and $Y$ preserve $I(N)$, then their commutator preserves it because

$$
[X,Y]f=X(Yf)-Y(Xf)\in I(N)
$$

for every $f\in I(N)$. Thus vector fields tangent to an embedded submanifold are closed under the [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields), and the restricted bracket depends only on their restrictions to the submanifold.

### Transverse intersection theorem

↑ **Parent:** [Embedded submanifold](#embedded-submanifold)

If embedded submanifolds $A,B\subseteq M$ meet transversely, then $A\cap B$ is an embedded submanifold of dimension $\dim A+\dim B-\dim M$.

The hypothesis is [transversality](#transversality-of-a-map-to-a-submanifold): tangent spaces to the two submanifolds span the ambient tangent space at each intersection point.

### Clean intersection

↑ **Parent:** [Embedded submanifold](#embedded-submanifold)

Submanifolds $A,B\subseteq M$ intersect cleanly when $A\cap B$ is an [embedded submanifold](#embedded-submanifold) and

$$
T_x(A\cap B)=T_xA\cap T_xB
$$

at every $x\in A\cap B$. A [transverse intersection](#transverse-intersection) is the special case in which $T_xA+T_xB=T_xM$.

#### Transverse intersection

↑ **Parent:** [Clean intersection](#clean-intersection)

Submanifolds $A,B\subseteq M$ intersect transversely when $T_xA+T_xB=T_xM$ at every intersection point. The [transverse intersection theorem](#transverse-intersection-theorem) then determines the dimension and smoothness of $A\cap B$.

##### Smooth intersection number

↑ **Parent:** [Transverse intersection](#transverse-intersection)

For complementary-dimensional oriented [submanifolds](differential-geometry.md#submanifold) of an oriented [manifold](topological-manifold.md) meeting transversely in finitely many points, the smooth intersection number is the sum of their local orientation signs. Geometric disjointness implies number zero, but number zero alone need not imply geometric disjointness. Without coherent [orientations](algebraic-topology.md#orientation-of-a-simplex), use the count modulo $2$.

## Hypersurface

↑ **Parent:** [Smooth manifold](smooth-manifold.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hypersurface)

A hypersurface in an $n$-dimensional [smooth manifold](smooth-manifold.md) is a smooth submanifold of dimension $n-1$. Locally, a regular level set $\{\phi=0\}$ with $\nabla\phi\ne0$ is a hypersurface whose [normal vector](differential-geometry.md#normal-vector) is $\nabla\phi$.

### Non-null hypersurface projection

↑ **Parent:** [Hypersurface](#hypersurface)

A [non-null hypersurface projection](#non-null-hypersurface-projection) annihilates the unit [normal vector](differential-geometry.md#normal-vector) and fixes tangent vectors to the [hypersurface](#hypersurface). It obeys $P^2=P$. Apply it to every tensor index to remove normal components, with the metric used to lower or raise the index pair for covariant slots. For a timelike unit normal in mostly-plus signature it is the [spatial projection tensor](numerical-relativity.md#spatial-projection-tensor). A null normal cannot be normalized this way, and a null hypersurface requires additional choices for a corresponding projection.

### Defining line bundle of a properly embedded hypersurface

↑ **Parent:** [Hypersurface](#hypersurface)

Local defining functions $f_\alpha$ for a properly embedded hypersurface $Y\subset X$ have nowhere-zero smooth ratios $f_\alpha/f_\beta$ on overlaps. These ratios define a [real line bundle](vector-bundle.md#real-line-bundle) with a global transverse section whose local representatives are the $f_\alpha$ and whose zero set is $Y$. The bundle is naturally isomorphic to the [normal bundle](algebraic-geometry.md#normal-bundle) of $Y$.

### Extrinsic curvature

↑ **Parent:** [Hypersurface](#hypersurface)

The extrinsic curvature of a hypersurface is the tangential bilinear form obtained by differentiating its unit normal. It measures how the hypersurface bends in the ambient manifold, with an overall sign depending on convention.

#### Totally geodesic hypersurface

↑ **Parent:** [Extrinsic curvature](#extrinsic-curvature)

A hypersurface is totally geodesic when every ambient geodesic initially tangent to it remains in it. Equivalently, its extrinsic curvature vanishes identically.

## Abstract smooth surface

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

An abstract smooth surface is a two-dimensional [smooth manifold](smooth-manifold.md). Thus it is a Hausdorff second-countable space with an atlas of plane-valued coordinate charts whose transition maps are smooth.

### Smooth quotient by a free finite group action

↑ **Parent:** [Abstract smooth surface](#abstract-smooth-surface)

A finite group acting freely by diffeomorphisms on a [smooth manifold](smooth-manifold.md) has a smooth quotient. Choose each coordinate neighbourhood disjoint from all its nontrivial translates and transport its chart through the quotient map. The resulting transition maps are restrictions of the original transition maps composed with group elements.

## Smooth map between manifolds

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

A map between smooth manifolds is smooth when its expression in every pair of coordinate charts is a [smooth function](analysis.md#smooth-function).

A map between [smooth manifolds](smooth-manifold.md) is smooth when its coordinate expressions in compatible charts have derivatives of every order. The condition is invariant under smooth chart changes and expresses [smoothness](analysis.md#smoothness) in charts.

### Smooth approximation of maps into Euclidean space

↑ **Parent:** [Smooth map between manifolds](#smooth-map-between-manifolds)

A [continuous map](topology.md#continuous-map) from a [smooth manifold](smooth-manifold.md) to $\mathbb R^d$ can be approximated by a [smooth map](#smooth-map-between-manifolds) with any prescribed positive continuous pointwise error bound. In coordinate charts, smoothing by local [convolution](fourier-analysis.md#convolution) and then combining with a smooth [partition of unity](#partition-of-unity) gives the approximation. On a compact subset of an open chart domain, a smooth cutoff allows the resulting straight-line [homotopy](homotopy.md) to be supported in that domain. This permits the [Sard theorem](differential-geometry.md#sard-s-theorem) to be used after approximation; the original continuous map can be space-filling and need not omit a point.

### Transversality of a map to a submanifold

↑ **Parent:** [Smooth map between manifolds](#smooth-map-between-manifolds)

A [smooth map](#smooth-map-between-manifolds) $f:M\to N$ is transverse to an [embedded submanifold](#embedded-submanifold) $S\subset N$ when

$$
df_p(T_pM)+T_{f(p)}S=T_{f(p)}N
\quad\text{for every }p\in f^{-1}(S).
$$

This is a sum of [vector subspaces](vector-space.md#vector-subspace), not necessarily a [direct sum](vector-space.md#direct-sum). Equivalently the composition of $df_p$ with the quotient to $T_{f(p)}N/T_{f(p)}S$ is surjective. In a [slice chart for an embedded submanifold](#slice-chart-for-an-embedded-submanifold) of codimension $k$, the $k$ normal coordinate functions composed with $f$ have surjective derivative on their common zero set. If the preimage is empty the condition holds vacuously.

#### General position for curves in a manifold

↑ **Parent:** [Transversality of a map to a submanifold](#transversality-of-a-map-to-a-submanifold)

Smooth maps of finitely many circles into a [manifold](topological-manifold.md) of dimension at least three can be perturbed within their homotopy classes to disjoint embeddings. The [transversality](#transversality-of-a-map-to-a-submanifold) dimension count for two curve branches is $1+1-m<0$, so their images avoid one another after perturbation; one also removes self-intersections and obtains immersions by the jet version of [transversality](#transversality-of-a-map-to-a-submanifold). This allows disjoint representative loops for relators in high-dimensional surgery constructions of prescribed [fundamental groups](algebraic-topology.md#fundamental-group).

#### Transverse preimage theorem

↑ **Parent:** [Transversality of a map to a submanifold](#transversality-of-a-map-to-a-submanifold)

If $f:M\to N$ satisfies [transversality of a map to a submanifold](#transversality-of-a-map-to-a-submanifold) $S$, its nonempty preimage is an [embedded submanifold](#embedded-submanifold) of the displayed codimension. Choose a [slice chart for an embedded submanifold](#slice-chart-for-an-embedded-submanifold) around $f(p)$ in which $S$ is the zero set of the first $k$ coordinates. Their composition with $f$ has surjective derivative on its zero set, so the [regular level set theorem](differential-geometry.md#regular-level-set-theorem) gives a local embedded slice of dimension $\dim M-k$. These slices give the [subspace topology](topology.md#subspace-topology) and a compatible [smooth atlas](differential-geometry.md#smooth-atlas) on the preimage. Its [tangent space](tangent-vector.md#tangent-space) is

$$
T_pf^{-1}(S)=\{v\in T_pM:df_pv\in T_{f(p)}S\}.
$$

### Pushforward of a curve

↑ **Parent:** [Smooth map between manifolds](#smooth-map-between-manifolds)

A [pushforward of a curve](#pushforward-of-a-curve) composes a parametrized curve in the source with a [smooth map between manifolds](#smooth-map-between-manifolds). Its tangent is the image of the original tangent under the [differential of a smooth map](#differential-of-a-smooth-map). A constant image curve has zero tangent, so a general smooth map need not preserve regularity of curves.

### Pullback of a smooth function

↑ **Parent:** [Smooth map between manifolds](#smooth-map-between-manifolds)

A [pullback of a smooth function](#pullback-of-a-smooth-function) composes a function on the target with a [smooth map between manifolds](#smooth-map-between-manifolds), producing a function on the source. It needs no inverse map. Acting on the pulled-back function defines the [differential of a smooth map](#differential-of-a-smooth-map) intrinsically as a map of derivations.

### Differential of a smooth map

↑ **Parent:** [Smooth map between manifolds](#smooth-map-between-manifolds)

For a [smooth map between manifolds](#smooth-map-between-manifolds) $f:M\to N$, the [differential](#differential-of-a-smooth-map) $df_x:T_xM\to T_{f(x)}N$ is the linear map obtained by differentiating in charts. Intrinsically it sends the tangent vector of a curve $\gamma$ through $x$ to the tangent vector of $f\circ\gamma$. The chain rule makes it independent of charts and gives $d(g\circ f)_x=dg_{f(x)}\circ df_x$.

#### Differential of a smooth function

↑ **Parent:** [Differential of a smooth map](#differential-of-a-smooth-map)

For a real-valued [smooth function](analysis.md#smooth-function) on a [smooth manifold](smooth-manifold.md), its [differential of a smooth map](#differential-of-a-smooth-map) is a [differential one-form](differential-form.md#one-form): $df_p$ maps a [tangent vector](tangent-vector.md) to the directional derivative of the function. In local coordinates, $df=\sum_i(\partial_i f)dx^i$. The [exterior derivative](differential-form.md#exterior-derivative) extends this operation from functions to higher-degree [differential forms](differential-form.md).

#### Zero-differential constancy theorem

↑ **Parent:** [Differential of a smooth map](#differential-of-a-smooth-map)

A [smooth map](#smooth-map-between-manifolds) between [smooth manifolds](smooth-manifold.md) with zero differential is locally constant: each target coordinate function has zero [derivatives](calculus.md#derivative) on a sufficiently small source coordinate ball. Integration along straight segments proves constancy there. Its fibers are open and closed, so a [connected](geometry-and-topology.md#connected-space) source makes the map constant globally.

#### Pushforward of a contravariant tensor

↑ **Parent:** [Differential of a smooth map](#differential-of-a-smooth-map)

The [pushforward of a contravariant tensor](#pushforward-of-a-contravariant-tensor) applies the [differential of a smooth map](#differential-of-a-smooth-map) to each vector factor of a type $(r,0)$ tensor. It is defined pointwise at a specified source point. A field generally gives a field along the map, not necessarily a unique tensor field on the image when several points have the same image. A [diffeomorphism](geometry-and-topology.md#diffeomorphism) allows the usual transport of arbitrary mixed tensors through its inverse as well.

#### Pullback of a covariant tensor

↑ **Parent:** [Differential of a smooth map](#differential-of-a-smooth-map)

The [pullback of a covariant tensor](#pullback-of-a-covariant-tensor) composes each of its vector arguments with the [differential of a smooth map](#differential-of-a-smooth-map). It takes a type $(0,s)$ tensor on the target to one on the source. Antisymmetry is not required; the [pullback of a differential form](differential-form.md#pullback-of-a-differential-form) is the alternating special case. If the target vectors are projected onto the image tangent space first, evaluating the pullback is unchanged.

##### Pullback of a covector

↑ **Parent:** [Pullback of a covariant tensor](#pullback-of-a-covariant-tensor)

The [pullback of a covector](#pullback-of-a-covector) is the dual linear map to the [differential of a smooth map](#differential-of-a-smooth-map). In coordinates its components are $(\phi^*\eta)_i=(\partial_i y^\alpha)\eta_\alpha$. The same rectangular Jacobian defines vector pushforward, with its other index contracted. No invertibility is needed.

#### Pushforward of a vector field

↑ **Parent:** [Differential of a smooth map](#differential-of-a-smooth-map)

For a [vector field](multivariable-calculus.md#vector-field) $X$ on $M$, its pushforward by a [smooth map between manifolds](#smooth-map-between-manifolds) $f:M\to N$ is the [vector field along a map](vector-bundle.md#vector-field-along-a-map) defined by $(f_*X)_p=df_p(X_p)$. Acting on a function $h$ on $N$, it satisfies $(f_*X)_p(h)=X_p(h\circ f)$. For a [diffeomorphism](geometry-and-topology.md#diffeomorphism) this defines a vector field on $N$ by evaluation at $p=f^{-1}(q)$. For a general map there need not be a single vector at each image point: $f(x)=x^2$, $X=\partial_x$ gives $2x\partial_y$, with opposite values over $y>0$.

##### Diffeomorphism invariance of a vector field is equivalent to commuting with its local flow

↑ **Parent:** [Pushforward of a vector field](#pushforward-of-a-vector-field)

The [chain rule](calculus.md#chain-rule) shows that $\alpha\phi_t\alpha^{-1}$ is the [local flow](#local-flow) of the [pushforward of a vector field](#pushforward-of-a-vector-field) $\alpha_*X$. If this equals $X$, uniqueness of [integral curves of a vector field](multivariable-calculus.md#integral-curve-of-a-vector-field) gives commutation. Conversely, differentiate the commuting identity at $t=0$ to obtain $d\alpha_pX_p=X_{\alpha(p)}$. All identities hold on their common domains; the [vector field](multivariable-calculus.md#vector-field) need not be complete.

##### Projectable vector field

↑ **Parent:** [Pushforward of a vector field](#pushforward-of-a-vector-field)

A [vector field](multivariable-calculus.md#vector-field) $X$ is projectable through a [smooth map between manifolds](#smooth-map-between-manifolds) $f:M\to N$ if there is a smooth vector field $Y$ on $N$ with $df_pX_p=Y_{f(p)}$ for every $p$. Agreement on fibres is necessary. For a surjective [submersion](differential-geometry.md#submersion) it is also sufficient: smooth local sections of the submersion express $Y$ locally as $df(X)$ and prove its smoothness. An arbitrary non-surjective map may instead give a field only along its image, with extension to $N$ requiring additional choices.

## Local flow

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

A local flow of a smooth [vector field](multivariable-calculus.md#vector-field) $V$ is a smooth map $\Phi:D\to M$, defined on an open neighborhood of $\{0\}\times M$, such that $\Phi^0(x)=x$, $\partial_t\Phi^t(x)=V(\Phi^t(x))$, and $\Phi^{s+t}=\Phi^s\circ\Phi^t$ whenever both sides are defined.

### Complete vector field

↑ **Parent:** [Local flow](#local-flow)

A smooth [vector field](multivariable-calculus.md#vector-field) is complete if its maximal [integral curves of a vector field](multivariable-calculus.md#integral-curve-of-a-vector-field) exist for every real time. Its [local flow](#local-flow) is then a global one-parameter group of [diffeomorphisms](geometry-and-topology.md#diffeomorphism); uniqueness of [ordinary differential equations](differential-equation.md#ordinary-differential-equation) proves the group law and the inverse-time identity. On a [compact](topology.md#compact-space) manifold without boundary, every smooth vector field is complete: [compactness](topology.md#compact-space) gives a uniform positive local existence interval through every point, so a curve can be successively extended past any proposed finite endpoint. On $\mathbb R$, $x^2\partial_x$ is not complete because its solution $x(t)=x_0/(1-tx_0)$ has finite-time blowup for $x_0>0$.

#### Complete vector fields need not be closed under addition or Lie brackets

↑ **Parent:** [Complete vector field](#complete-vector-field)

On $\mathbb R^2$, the [vector fields](multivariable-calculus.md#vector-field) $X=y\partial_x$ and $Y=(x^2/2)\partial_y$ are complete, since their [local flows](#local-flow) are $(x+ty,y)$ and $(x,y+tx^2/2)$. Their [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields) is $-(x^2/2)\partial_x+xy\partial_y$. Its [integral curve of a vector field](multivariable-calculus.md#integral-curve-of-a-vector-field) starting at $(2,0)$ is $(2/(1+t),0)$, which cannot continue through $t=-1$. The sum has an [integral curve of a vector field](multivariable-calculus.md#integral-curve-of-a-vector-field)

$$
\left(\left(1-\frac{t}{2\sqrt3}\right)^{-2},\frac1{\sqrt3}\left(1-\frac{t}{2\sqrt3}\right)^{-3}\right)
$$

that cannot continue through $t=2\sqrt3$. Thus neither operation preserves [complete vector fields](#complete-vector-field) on a general noncompact [smooth manifold](smooth-manifold.md). This contrasts with a [compact manifold](#compact-manifold) without boundary, where every smooth [vector field](multivariable-calculus.md#vector-field) is complete.

### Straightening theorem

↑ **Parent:** [Local flow](#local-flow)

Near a point where a smooth [vector field](multivariable-calculus.md#vector-field) is nonzero, there are coordinates in which it is $\partial/\partial x_1$. Flow a transverse coordinate slice by the [local flow](#local-flow); the [inverse function theorem](multivariable-calculus.md#inverse-function-theorem) makes the resulting map a coordinate chart. This is the first step of the [coordinate proof of the Frobenius theorem](differential-geometry.md#coordinate-proof-of-the-frobenius-theorem).

## Partition of unity

↑ **Parent:** [Smooth manifold](smooth-manifold.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partition_of_unity)

Every open cover of a smooth paracompact manifold admits a smooth partition of unity subordinate to it: nonnegative smooth functions with locally finite supports in the cover whose sum is one.

## Orientable smooth manifold

↑ **Parent:** [Smooth manifold](smooth-manifold.md)

A smooth manifold is orientable when it admits an atlas whose transition maps have positive Jacobian determinant wherever they are defined.

This atlas criterion expresses [orientability](topology.md#orientability) for a differentiable manifold.

### Orientation of a smooth manifold

↑ **Parent:** [Orientable smooth manifold](#orientable-smooth-manifold)

An orientation of a [smooth manifold](smooth-manifold.md) is a continuous choice of [orientation of a vector space](multilinear-algebra.md#orientation-of-a-vector-space) in every [tangent space](tangent-vector.md#tangent-space), equivalently an [orientation of a vector bundle](vector-bundle.md#orientation-of-a-vector-bundle) on its [tangent bundle](vector-bundle.md#tangent-bundle). It can be specified by an atlas with positive [Jacobian determinants](multivariable-calculus.md#jacobian-determinant) on all overlaps or by a nowhere-vanishing top-degree [differential form](differential-form.md). On a connected orientable manifold there are two choices, interchanged by reversing every tangent-space orientation.

// Target: differential-geometry.bigb

### Oriented atlas

↑ **Parent:** [Orientable smooth manifold](#orientable-smooth-manifold)

An oriented atlas is a [smooth atlas](differential-geometry.md#smooth-atlas) whose [smooth transition maps](differential-geometry.md#smooth-transition-map) have positive [Jacobian determinants](multivariable-calculus.md#jacobian-determinant) on every overlap. The coordinate [bases](vector-space.md#basis) then give compatible choices of [orientation of a vector space](multilinear-algebra.md#orientation-of-a-vector-space) on all [tangent spaces](tangent-vector.md#tangent-space). A nowhere-vanishing top-degree [differential form](differential-form.md) gives such an atlas: restrict each chart until its coefficient has constant sign, reverse one coordinate if necessary to make that sign positive, and compare the positive coefficients on overlaps. Conversely, a [partition of unity](#partition-of-unity) glues positive local coordinate top forms to a global [volume form](differential-form.md#volume-form).

### Outward-normal-first boundary orientation

↑ **Parent:** [Orientable smooth manifold](#orientable-smooth-manifold)

The boundary of an oriented manifold with boundary is oriented by the outward-normal-first convention: an ordered basis $(v_2,\ldots,v_n)$ of $T_p\partial X$ is positive when $(v_1,v_2,\ldots,v_n)$ is positive in $T_pX$ for an outward-pointing normal $v_1$.

### Equivalent formulations of orientability of a smooth manifold

↑ **Parent:** [Orientable smooth manifold](#orientable-smooth-manifold)

For a smooth $n$-manifold, the following are equivalent: an atlas with positive transition Jacobians, a smooth choice of orientation of every tangent space, and a nowhere-vanishing smooth $n$-form. Positive charts orient their coordinate frames; oriented frames select the positive local coordinate volume forms, which a [partition of unity](#partition-of-unity) glues; and a nonzero top form declares a frame positive when its value on that frame is positive.

### Orientability of factors of a product manifold

↑ **Parent:** [Orientable smooth manifold](#orientable-smooth-manifold)

If $M\times N$ is orientable, fix a point of $N$ and an ordered basis of its tangent space. Contracting a product orientation with that basis gives a smooth orientation of $M$. Interchanging the factors gives an orientation of $N$.

### Orientation-reversing diffeomorphism

↑ **Parent:** [Orientable smooth manifold](#orientable-smooth-manifold)

An orientation-reversing diffeomorphism reverses the chosen orientation. In oriented local coordinates its derivative has negative determinant.

## ↑ Ancestors (5)

1. [Differential geometry](differential-geometry.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (138)

- [Abstract smooth surface](#abstract-smooth-surface)
- [Affine connection](vector-bundle.md#affine-connection)
- [Anosov diffeomorphism](dynamical-systems.md#anosov-diffeomorphism)
- [Anosov flow](dynamical-systems.md#anosov-flow)
- [C1 openness of diffeomorphisms](geometry-and-topology.md#c1-openness-of-diffeomorphisms)
- [Category of topological manifolds](topological-manifold.md#category-of-topological-manifolds)
- [Compact manifold](#compact-manifold)
- [Complete vector fields need not be closed under addition or Lie brackets](#complete-vector-fields-need-not-be-closed-under-addition-or-lie-brackets)
- [Complex Stiefel manifold](vector-bundle.md#complex-stiefel-manifold)
- [Complex structure](complex-geometry.md#complex-structure)
- [Connectedness criterion for the orientation double cover](algebraic-topology.md#connectedness-criterion-for-the-orientation-double-cover)
- [Cotangent coordinate transition](symplectic-geometry.md#cotangent-coordinate-transition)
- [Critical point of a smooth map](differential-geometry.md#critical-point-of-a-smooth-map)
- [Critical value](differential-geometry.md#critical-value)
- [de Rham cohomology of a finite quotient](differential-form.md#de-rham-cohomology-of-a-finite-quotient)
- [Degree-zero de Rham cohomology](differential-form.md#degree-zero-de-rham-cohomology)
- [Density bundle](vector-bundle.md#density-bundle)
- [Derivation at a point](tangent-vector.md#derivation-at-a-point)
- [Derivations of smooth functions are vector fields](associative-algebra.md#derivations-of-smooth-functions-are-vector-fields)
- [Differential geometry](differential-geometry.md)
- [Differential of a smooth function](#differential-of-a-smooth-function)
- [Dimension of a manifold](topological-manifold.md#dimension-of-a-manifold)
- [Distribution (differential geometry)](differential-geometry.md#distribution-differential-geometry)
- [Fiber metric](vector-bundle.md#fiber-metric)
- [Frame bundle](fiber-bundle.md#frame-bundle)
- [Free proper Lie-group action theorem](fiber-bundle.md#free-proper-lie-group-action-theorem)
- [Full-row-rank matrix manifold](#full-row-rank-matrix-manifold)
- [Group manifold](lie-theory.md#group-manifold)
- [Hypersurface](#hypersurface)
- [Invariant primitive under a finite group action](homology.md#invariant-primitive-under-a-finite-group-action)
- [Lagrangian graph](symplectic-geometry.md#lagrangian-graph)
- [Lie group](lie-theory.md#lie-group)
- [Lusternik–Schnirelmann critical point theorem](algebraic-topology.md#lusternik-schnirelmann-critical-point-theorem)
- [Moser theorem for volume forms](symplectic-geometry.md#moser-theorem-for-volume-forms)
- [Musical isomorphism](riemannian-metric.md#musical-isomorphism)
- [Nontrivial exact fiber translation](symplectic-geometry.md#nontrivial-exact-fiber-translation)
- [Normal vector](differential-geometry.md#normal-vector)
- [One-form](differential-form.md#one-form)
- [Orientability](topology.md#orientability)
- [Orientation double cover](algebraic-topology.md#orientation-double-cover)
- [Orientation of a smooth manifold](#orientation-of-a-smooth-manifold)
- [Orthogonal group as a regular level set](linear-algebra.md#orthogonal-group-as-a-regular-level-set)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-12.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-68.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-71.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-14.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-27.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-27.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-14.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-15.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-15.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-63.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-1.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-15.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-21.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-15.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-15.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-15.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-15.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-15.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-15.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-19.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-25.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-65.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-65.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-16.md#4/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-17.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1.md#25h/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-19.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-15.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-17.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-17.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-15.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-15.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-15.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-15.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-15.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-16.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-16.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-2.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-17.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-17.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-18.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-2.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-102.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-115.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-309.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-118.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140.md#6/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-115.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-302.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-313.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#26i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4.md#37d/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-115.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-118.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-302.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-302.md#1/d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-131.md#1/a/solution)
- [Poincaré-Hopf theorem](vector-bundle.md#poincare-hopf-theorem)
- [Product manifold](#product-manifold)
- [Pseudo-Riemannian manifold](differential-geometry.md#pseudo-riemannian-manifold)
- [Real de Rham intersection form in dimension four](homology.md#real-de-rham-intersection-form-in-dimension-four)
- [Riemannian distance induces the manifold topology](riemannian-geometry.md#riemannian-distance-induces-the-manifold-topology)
- [Riemannian geometry](riemannian-geometry.md)
- [Riemannian manifold](riemannian-geometry.md#riemannian-manifold)
- [Riemannian metric](riemannian-metric.md)
- [Riemannian volume density](vector-bundle.md#riemannian-volume-density)
- [Sheaf of smooth differential forms](differential-form.md#sheaf-of-smooth-differential-forms)
- [Smooth approximation of maps into Euclidean space](#smooth-approximation-of-maps-into-euclidean-space)
- [Smooth atlas](differential-geometry.md#smooth-atlas)
- [Smooth embedded surface](#smooth-embedded-surface)
- [Smooth exponential sequence](vector-bundle.md#smooth-exponential-sequence)
- [Smooth four-manifold](topological-manifold.md#smooth-four-manifold)
- [Smooth map between manifolds](#smooth-map-between-manifolds)
- [Smooth quotient by a free finite group action](#smooth-quotient-by-a-free-finite-group-action)
- [Smooth surface](differential-geometry.md#smooth-surface)
- [Spacetime dimension](general-relativity.md#spacetime-dimension)
- [Standard affine atlas of real projective space](algebraic-topology.md#standard-affine-atlas-of-real-projective-space)
- [Symplectic manifold](symplectic-geometry.md#symplectic-manifold)
- [Symplectic orientation](symplectic-geometry.md#symplectic-orientation)
- [Tangent bundle](vector-bundle.md#tangent-bundle)
- [Tangent space](tangent-vector.md#tangent-space)
- [Tangent vector](tangent-vector.md)
- [Tensor bundle](vector-bundle.md#tensor-bundle)
- [Top de Rham cohomology of a compact connected oriented manifold](differential-form.md#top-de-rham-cohomology-of-a-compact-connected-oriented-manifold)
- [Top-degree de Rham cohomology](differential-form.md#top-degree-de-rham-cohomology)
- [Two-chart smooth atlas of an ellipsoid](euclidean-geometry.md#two-chart-smooth-atlas-of-an-ellipsoid)
- [Unitary group as a regular level set](topological-group.md#unitary-group-as-a-regular-level-set)
- [Zero-differential constancy theorem](#zero-differential-constancy-theorem)
