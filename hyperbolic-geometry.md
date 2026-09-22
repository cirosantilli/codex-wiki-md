# Hyperbolic geometry

↑ **Parent:** [Geometry and topology](geometry-and-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbolic_geometry)

Hyperbolic geometry studies spaces of constant negative curvature.

**Table of contents**

- [Hyperbolic Pythagorean theorem](#hyperbolic-pythagorean-theorem)
- [Tessellation](#tessellation)
  - [Tatami tiling](#tatami-tiling)
    - [Tatami-free rectangle](#tatami-free-rectangle)
- [Hyperbolic circle in the Poincare disc](#hyperbolic-circle-in-the-poincare-disc)
- [Hyperbolic space](#hyperbolic-space)
  - [Bounded displacement sets of hyperbolic isometries are compact](#bounded-displacement-sets-of-hyperbolic-isometries-are-compact)
  - [Minimum enclosing ball in hyperbolic space](#minimum-enclosing-ball-in-hyperbolic-space)
  - [Axis of a hyperbolic-space isometry](#axis-of-a-hyperbolic-space-isometry)
  - [Poincare ball model](#poincare-ball-model)
    - [Hyperbolic extension of a Möbius transformation](#hyperbolic-extension-of-a-mobius-transformation)
- [Hyperbolic hexagon](#hyperbolic-hexagon)
  - [Right-angled hyperbolic hexagon](#right-angled-hyperbolic-hexagon)
- [Beltrami-Klein model](#beltrami-klein-model)
- [Hyperbolic surface](#hyperbolic-surface)
  - [Hyperbolic holonomy representation](#hyperbolic-holonomy-representation)
  - [Length spectrum](#length-spectrum)
    - [Marked length spectrum](#marked-length-spectrum)
    - [Huber spectral equivalence theorem](#huber-spectral-equivalence-theorem)
    - [Uniform finiteness of short geodesic classes](#uniform-finiteness-of-short-geodesic-classes)
    - [Buser finite length spectrum theorem](#buser-finite-length-spectrum-theorem)
      - [Finite spectral matching by polynomial invariants](#finite-spectral-matching-by-polynomial-invariants)
    - [Selberg trace formula](#selberg-trace-formula)
  - [Hyperbolic collar](#hyperbolic-collar)
  - [Shortest closed geodesic on the three-punctured sphere](#shortest-closed-geodesic-on-the-three-punctured-sphere)
  - [Pants decomposition](#pants-decomposition)
    - [Elementary move of a pants decomposition](#elementary-move-of-a-pants-decomposition)
    - [Pants decomposition graph](#pants-decomposition-graph)
    - [Bers pants decomposition theorem](#bers-pants-decomposition-theorem)
    - [Fenchel–Nielsen coordinates](#fenchel-nielsen-coordinates)
      - [Fenchel–Nielsen twist](#fenchel-nielsen-twist)
      - [Finite length coordinates for hyperbolic surfaces](#finite-length-coordinates-for-hyperbolic-surfaces)
  - [Collar lemma](#collar-lemma)
  - [Hyperbolic systole](#hyperbolic-systole)
  - [Hyperbolic area](#hyperbolic-area)
- [Hyperbolic metric](#hyperbolic-metric)
  - [Poincare metric on a Riemann surface](#poincare-metric-on-a-riemann-surface)
    - [Hyperbolic tube around a radial segment](#hyperbolic-tube-around-a-radial-segment)
    - [Hyperbolic derivative density](#hyperbolic-derivative-density)
      - [Hyperbolic characteristic of a disc map](#hyperbolic-characteristic-of-a-disc-map)
        - [Critical-point Jensen identity for the hyperbolic derivative](#critical-point-jensen-identity-for-the-hyperbolic-derivative)
  - [Hyperbolic metric on the punctured disk](#hyperbolic-metric-on-the-punctured-disk)
    - [Hyperbolic zero sequences on a punctured disk](#hyperbolic-zero-sequences-on-a-punctured-disk)
  - [Pseudohyperbolic distance](#pseudohyperbolic-distance)
- [Hyperbolic plane](#hyperbolic-plane)
  - [Hyperbolic polygon](#hyperbolic-polygon)
  - [Ideal hyperbolic quadrilateral](#ideal-hyperbolic-quadrilateral)
  - [Hyperbolic disc](#hyperbolic-disc)
  - [Horocycle](#horocycle)
    - [Common orthogonal line of two horocycles](#common-orthogonal-line-of-two-horocycles)
    - [Ideal centre of a horocycle](#ideal-centre-of-a-horocycle)
  - [Hyperbolic circle](#hyperbolic-circle)
    - [Hyperbolic circle in the upper half-plane](#hyperbolic-circle-in-the-upper-half-plane)
  - [Hyperbolic line](#hyperbolic-line)
    - [Ideal endpoint](#ideal-endpoint)
    - [Parallel hyperbolic lines](#parallel-hyperbolic-lines)
    - [Ultraparallel hyperbolic lines](#ultraparallel-hyperbolic-lines)
  - [Hyperbolic distance](#hyperbolic-distance)
  - [Horoball](#horoball)
  - [Finite-order elliptic transformation](#finite-order-elliptic-transformation)
- [Poincaré disk model](#poincare-disk-model)
  - [Poincare disc automorphism](#poincare-disc-automorphism)
  - [Area of a hyperbolic disc](#area-of-a-hyperbolic-disc)
    - [Hyperbolic area bounds an inscribed disc](#hyperbolic-area-bounds-an-inscribed-disc)
    - [Radial chain of equal hyperbolic discs](#radial-chain-of-equal-hyperbolic-discs)
  - [Geodesic obstruction for a horizontal chain of hyperbolic discs](#geodesic-obstruction-for-a-horizontal-chain-of-hyperbolic-discs)
  - [Hyperbolic length in the Poincare disc](#hyperbolic-length-in-the-poincare-disc)
  - [Geodesics of the Poincare disc](#geodesics-of-the-poincare-disc)
  - [Hyperbolic distance in the Poincare disc](#hyperbolic-distance-in-the-poincare-disc)
    - [Hyperbolic geodesic cap](#hyperbolic-geodesic-cap)
      - [Geodesic-cap and Carleson-box comparison](#geodesic-cap-and-carleson-box-comparison)
  - [Euclidean circle representing a perpendicular hyperbolic line](#euclidean-circle-representing-a-perpendicular-hyperbolic-line)
- [Poincaré half-plane model](#poincare-half-plane-model)
  - [Hyperbolic translation length](#hyperbolic-translation-length)
    - [Polynomial encoding of hyperbolic geodesic lengths](#polynomial-encoding-of-hyperbolic-geodesic-lengths)
  - [Hyperbolic distance in the Poincare half-plane](#hyperbolic-distance-in-the-poincare-half-plane)
    - [Equality of horizontal hyperbolic and Euclidean distances](#equality-of-horizontal-hyperbolic-and-euclidean-distances)
  - [Geodesic in the Poincare half-plane model](#geodesic-in-the-poincare-half-plane-model)
    - [Calibration for semicircular hyperbolic geodesics](#calibration-for-semicircular-hyperbolic-geodesics)
    - [Common perpendicular of ultraparallel hyperbolic lines](#common-perpendicular-of-ultraparallel-hyperbolic-lines)
      - [Configurations of three ultraparallel lines](#configurations-of-three-ultraparallel-lines)
    - [Hyperbolic lines meeting the imaginary axis at a fixed angle](#hyperbolic-lines-meeting-the-imaginary-axis-at-a-fixed-angle)
  - [PSL2(R)](#psl2-r)
    - [Hyperbolic element of PSL2(R)](#hyperbolic-element-of-psl2-r)
    - [Elliptic element of PSL2(R)](#elliptic-element-of-psl2-r)
    - [Parabolic element of PSL2(R)](#parabolic-element-of-psl2-r)
    - [Isometry group of the Poincare half-plane](#isometry-group-of-the-poincare-half-plane)
    - [Transitivity on pointed hyperbolic lines](#transitivity-on-pointed-hyperbolic-lines)
  - [Hyperbolic reflection](#hyperbolic-reflection)
    - [Every hyperbolic-plane isometry is a product of at most three reflections](#every-hyperbolic-plane-isometry-is-a-product-of-at-most-three-reflections)
    - [Composition of reflections in ultraparallel hyperbolic lines](#composition-of-reflections-in-ultraparallel-hyperbolic-lines)
  - [Hyperbolic half-turn](#hyperbolic-half-turn)
- [Cayley transform (hyperbolic geometry)](#cayley-transform-hyperbolic-geometry)
- [Hyperboloid model](#hyperboloid-model)
  - [Three-dimensional hyperboloid model](#three-dimensional-hyperboloid-model)
  - [Minkowski inner product](#minkowski-inner-product)
- [Lambert quadrilateral](#lambert-quadrilateral)
- [Hyperbolic triangle](#hyperbolic-triangle)
  - [Hyperbolic triangle inradius bound](#hyperbolic-triangle-inradius-bound)
  - [Ideal triangle](#ideal-triangle)
    - [Ideal vertex](#ideal-vertex)
  - [Hyperbolic side-side-angle ambiguity](#hyperbolic-side-side-angle-ambiguity)
  - [Hyperbolic side-side-side congruence](#hyperbolic-side-side-side-congruence)
  - [Hyperbolic triangle area](#hyperbolic-triangle-area)
    - [Hyperbolic polygon area](#hyperbolic-polygon-area)
      - [Regular hyperbolic polygon with prescribed area](#regular-hyperbolic-polygon-with-prescribed-area)
  - [Hyperbolic law of cosines](#hyperbolic-law-of-cosines)
    - [Hyperbolic AAA congruence](#hyperbolic-aaa-congruence)
- [Hyperbolic law of sines](#hyperbolic-law-of-sines)

## Hyperbolic Pythagorean theorem

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)

For a right-angled geodesic triangle in curvature minus one, with legs $a,b$ and hypotenuse $c$, the displayed identity replaces the Euclidean theorem. Normalize the right vertex to $i$ in the upper half-plane, one endpoint to $iy$ with $y>1$, and the other to $s+it$ with $s^2+t^2=1$ and $t>0$. The [Hyperbolic distance in the Poincare half-plane](#hyperbolic-distance-in-the-poincare-half-plane) gives $\cosh a=(y+y^{-1})/2$, $\cosh b=1/t$ and $\cosh c=(1+y^2)/(2yt)$, proving the identity. For small lengths its expansion gives $c^2=a^2+b^2$ to leading order.

## Tessellation

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)

A tessellation is a covering by tiles with pairwise disjoint interiors; a locally finite tessellation meets any compact set in only finitely many tiles. In a tessellation by congruent compact hyperbolic polygons, the adjacency graph records side-crossing steps. The area growth $\operatorname{Area}B(r)=2\pi(\cosh r-1)$ and bounded tile diameter imply exponential growth of the number of tiles within $n$ steps: a unit geodesic segment meets a uniformly bounded number of tiles, by packing congruent interior balls, so a metric ball of radius proportional to $n$ lies in the step ball. Conversely the step ball lies in a metric ball of radius proportional to $n$. The regular right-angled pentagons with four around every vertex give the tiling $\{5,4\}$.

### Tatami tiling

↑ **Parent:** [Tessellation](#tessellation)

A [tessellation](#tessellation) by rectangular tiles in which no point is a corner of four tiles. In the common lattice version, the tiles are $1\times2$ [rectangles](euclidean-geometry.md#rectangle). The local corner restriction makes existence depend on more than the total [area](differential-geometry.md#surface-area).

#### Tatami-free rectangle

↑ **Parent:** [Tatami tiling](#tatami-tiling)

## Hyperbolic circle in the Poincare disc

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)

In the [Poincare disc model](#poincare-disk-model), a [hyperbolic circle in the Poincare disc](#hyperbolic-circle-in-the-poincare-disc) consists of points at one fixed hyperbolic distance from a center. At center zero it is the Euclidean circle $|z|=\tanh(R/2)$, since radial hyperbolic distance is $2\operatorname{artanh}|z|$. A [Poincare disc automorphism](#poincare-disc-automorphism) sending a general center to zero transports this description. Conversely every Euclidean circle entirely inside the disc is such a circle: the product of inversion in that circle and unit-circle inversion has reciprocal fixed points, one inside; sending the inner fixed point to zero makes the circle concentric with the unit circle.

## Hyperbolic space

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbolic_space)

The complete simply connected [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) of dimension $n$ with constant sectional curvature $-1$ is hyperbolic space. In the upper half-space model its metric is $ds^2=(dx_1^2+\cdots+dx_n^2)/x_n^2$ for $x_n>0$. Its ideal boundary in dimension three is the [Riemann sphere](riemann-surfaces.md#riemann-sphere).

### Bounded displacement sets of hyperbolic isometries are compact

↑ **Parent:** [Hyperbolic space](#hyperbolic-space)

In the positive Hermitian determinant-one model of three-dimensional [hyperbolic space](#hyperbolic-space), the base point is $I$ and a matrix $g\in SL(2,\mathbb C)$ sends it to $gg^*$. The distance obeys $2\cosh d(I,gg^*)=\operatorname{tr}(gg^*)$. Bounded displacement therefore bounds every matrix entry, and the determinant-one condition gives a closed bounded subset of a finite-dimensional real vector space. Passing to $PSL(2,\mathbb C)$ preserves compactness. Conjugating moves any chosen base point to $I$. A discrete subgroup meets each such compact set in finitely many elements, proving escape of distinct elements and proper discontinuity, including finite stabilizers.

### Minimum enclosing ball in hyperbolic space

↑ **Parent:** [Hyperbolic space](#hyperbolic-space)

For a nonempty finite set $\{p_1,\ldots,p_m\}$ in finite-dimensional [hyperbolic space](#hyperbolic-space), the continuous function $R(x)=\max_jd(x,p_j)$ attains its minimum. Indeed, a bounded candidate radius confines all possible improving centers to a closed bounded ball about $p_1$. Such a ball is compact in the [Poincare ball model](#poincare-ball-model), since its points remain away from the ideal boundary. Minimizing $R$ on it supplies a [closed ball](topological-analysis.md#closed-ball) of smallest enclosing radius. More generally this argument works for any nonempty bounded set in a [proper metric space](geometric-group-theory.md#proper-metric-space) when the supremum-distance function is finite.

### Axis of a hyperbolic-space isometry

↑ **Parent:** [Hyperbolic space](#hyperbolic-space)

An isometry of [hyperbolic space](#hyperbolic-space) with positive attained [translation length](geometric-group-theory.md#translation-length) has an invariant complete geodesic joining its two ideal fixed points. This is its axis. It translates along the axis by its translation length; in three dimensions it may additionally rotate around it. In upper half-space, $(z,t)\mapsto(kz,|k|t)$ with $|k|\ne1$ has the vertical axis through zero and length $|\log|k||$. Every connecting path has length at least the change in $\log t$, and a vertical segment attains the bound.

### Poincare ball model

↑ **Parent:** [Hyperbolic space](#hyperbolic-space)

The unit ball in Euclidean space with the displayed [Riemannian metric](riemannian-metric.md) models [hyperbolic space](#hyperbolic-space) of curvature minus one. Its ideal boundary is the unit sphere, and its geodesics are diameters or circle arcs orthogonal to that sphere. The metric is invariant under the conformal ball automorphisms.

<h4 id="hyperbolic-extension-of-a-mobius-transformation">Hyperbolic extension of a Möbius transformation</h4>

↑ **Parent:** [Poincare ball model](#poincare-ball-model)

A [Möbius transformation](group-theory.md#mobius-transformation) of the ideal two-sphere extends uniquely to an orientation-preserving [isometry](riemannian-geometry.md#isometry) of three-dimensional [hyperbolic space](#hyperbolic-space). In upper half-space, translations, complex similarities, and $z\mapsto-1/z$ extend respectively to $(z,t)\mapsto(z+b,t)$, $(\lambda z,|\lambda|t)$, and $(-\overline z,t)/(|z|^2+t^2)$. Each preserves $(|dz|^2+dt^2)/t^2$; composing these extensions constructs the general case. Ball-origin stabilizers are ordinary rotations, represented on the boundary by $SU(2)$ modulo its central signs.

## Hyperbolic hexagon

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)

A six-sided polygon in the [hyperbolic plane](#hyperbolic-plane) whose sides are [geodesic segments](riemannian-geometry.md#geodesic-segment). The especially useful right-angled case is a [right-angled hyperbolic hexagon](#right-angled-hyperbolic-hexagon).

### Right-angled hyperbolic hexagon

↑ **Parent:** [Hyperbolic hexagon](#hyperbolic-hexagon)

A geodesic hexagon in the [hyperbolic plane](#hyperbolic-plane) with all six interior angles $\pi/2$. Any three positive alternating side lengths determine it up to [isometry](riemannian-geometry.md#isometry). If those sides are $\ell_i/2$, the opposite seam satisfies $\cosh s_i=(\cosh(\ell_i/2)+\cosh(\ell_j/2)\cosh(\ell_k/2))/(\sinh(\ell_j/2)\sinh(\ell_k/2))$. Two congruent such hexagons glued along the other three sides form a [pair of pants](topological-surface.md#pair-of-pants-mathematics) with boundary lengths $\ell_1,\ell_2,\ell_3$.

## Beltrami-Klein model

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)

The Beltrami-Klein model realizes the [hyperbolic plane](#hyperbolic-plane) inside an open Euclidean disk, with [geodesics](riemannian-geometry.md#geodesic) given by straight chords. Its metric differs from the Euclidean metric, and angles are generally distorted. The straight chords make [geodesic convexity](riemannian-geometry.md#geodesic-convexity) especially easy to see.

## Hyperbolic surface

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)

A surface with a complete [Riemannian metric](riemannian-metric.md) of constant [Gaussian curvature](second-fundamental-form.md#gaussian-curvature) $-1$. Its local model is the [Poincaré half-plane model](#poincare-half-plane-model); the orientable case is a quotient by a free [properly discontinuous group action](geometric-group-theory.md#properly-discontinuous-group-action) of orientation-preserving isometries.

### Hyperbolic holonomy representation

↑ **Parent:** [Hyperbolic surface](#hyperbolic-surface)

For a marked closed [hyperbolic surface](#hyperbolic-surface), the representation of its [fundamental group](algebraic-topology.md#fundamental-group) whose image acts as the deck group on the [hyperbolic plane](#hyperbolic-plane). It is discrete and faithful, determined up to conjugation by the marking and the metric, and gives $X=\mathbb H^2/\rho(\pi_1\Sigma_g)$. For a closed orientable surface it admits determinant-one lifts. It is different from the tangent-space action of the [Riemannian holonomy group](fiber-bundle.md#riemannian-holonomy-group).

### Length spectrum

↑ **Parent:** [Hyperbolic surface](#hyperbolic-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Length_spectrum)

The unmarked length spectrum of a compact [hyperbolic surface](#hyperbolic-surface) is the multiset of lengths of its closed [geodesics](riemannian-geometry.md#geodesic), with a consistent convention for primitive curves and orientation. The marked version labels lengths by free homotopy classes. The [Selberg trace formula](#selberg-trace-formula) relates the unmarked multiset to the [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) [spectrum](linear-operator-theory.md#spectrum-functional-analysis).

#### Marked length spectrum

↑ **Parent:** [Length spectrum](#length-spectrum)

For a closed [hyperbolic surface](#hyperbolic-surface) with a specified marking of its [fundamental group](algebraic-topology.md#fundamental-group), assign to each nontrivial conjugacy class the length of its unique closed [geodesic](riemannian-geometry.md#geodesic). Retaining the group label is stronger than retaining only the unmarked length multiset: it also records which lengths belong to intersecting curves or powers of particular curves.

#### Huber spectral equivalence theorem

↑ **Parent:** [Length spectrum](#length-spectrum)

For closed [hyperbolic surfaces](#hyperbolic-surface) of curvature $-1$, equality of the [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) [spectra](linear-operator-theory.md#spectrum-functional-analysis), including multiplicities, is equivalent to equality of the unmarked [length spectra](#length-spectrum) of closed [geodesics](riemannian-geometry.md#geodesic). The [Selberg trace formula](#selberg-trace-formula) proves the equivalence. Primitive lengths with multiplicities and the multiset including their iterates determine one another, provided the same orientation convention is used.

#### Uniform finiteness of short geodesic classes

↑ **Parent:** [Length spectrum](#length-spectrum)

In a compact smooth family of marked closed [hyperbolic surfaces](#hyperbolic-surface), only finitely many [free homotopy](homotopy.md#free-homotopy) classes of [closed geodesics](riemannian-geometry.md#closed-geodesic) have length below a fixed bound somewhere in the family. A uniform [bilipschitz equivalence](geometric-group-theory.md#bilipschitz-equivalence) with a fixed metric reduces this to local finiteness of its [length spectrum](#length-spectrum).

#### Buser finite length spectrum theorem

↑ **Parent:** [Length spectrum](#length-spectrum)

For fixed genus $g\ge2$ and systole lower bound $\varepsilon>0$, a uniform finite length cutoff $L$ determines the entire unmarked [length spectrum](#length-spectrum) of a closed [hyperbolic surface](#hyperbolic-surface) in the thick part, including multiplicities. Equality up to $L$ forces equality everywhere. This is a finite-determination statement for spectra and does not claim that all isospectral surfaces are isometric.

##### Finite spectral matching by polynomial invariants

↑ **Parent:** [Buser finite length spectrum theorem](#buser-finite-length-spectrum-theorem)

Suppose a compact parameter set carries a locally finite countable multiset of positive quantities, and a fixed injective transform of each labelled quantity is a [polynomial](polynomial.md) in finitely many ambient coordinates. Assume only finitely many labels can have bounded value anywhere in the compact set. Then a uniform finite initial multiset determines the entire multiset. For each source label there are finitely many possible matching labels. Equality for finitely many labels in both directions is a finite union of [algebraic sets](algebraic-geometry.md#algebraic-set), obtained from injective matchings and polynomial equalities. These algebraic sets decrease as more labels are included, so they stabilize by the [Hilbert basis theorem](algebra.md#hilbert-basis-theorem). A compatible infinite matching in each direction follows by the [König infinity lemma](tree-graph-theory.md#konig-s-lemma), and local finiteness makes multiplicities equal. Squared traces of [hyperbolic holonomy representations](#hyperbolic-holonomy-representation) give the application to the [Buser finite length spectrum theorem](#buser-finite-length-spectrum-theorem).

#### Selberg trace formula

↑ **Parent:** [Length spectrum](#length-spectrum)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Selberg_trace_formula)

For a compact [hyperbolic surface](#hyperbolic-surface), the Selberg trace formula equates a sum over [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) [eigenvalues](linear-operator-theory.md#eigenvalue) to an area term and a sum over primitive closed [geodesics](riemannian-geometry.md#geodesic) and their iterates. It proves that the [Laplacian](multivariable-calculus.md#laplacian) [spectrum](linear-operator-theory.md#spectrum-functional-analysis) and the unmarked [length spectrum](#length-spectrum), with multiplicities, determine each other.

### Hyperbolic collar

↑ **Parent:** [Hyperbolic surface](#hyperbolic-surface)

A collar around a simple closed [geodesic](riemannian-geometry.md#geodesic) of length $\ell$ is an embedded annulus with metric $dr^2+\ell^2\cosh^2r\,dt^2$, where $t\in\mathbb R/\mathbb Z$. The [collar lemma](#collar-lemma) gives half-width $w=\operatorname{arcsinh}(1/\sinh(\ell/2))$. As $\ell$ tends to zero the collar gets wide, forcing crossing [geodesics](riemannian-geometry.md#geodesic) to become long.

### Shortest closed geodesic on the three-punctured sphere

↑ **Parent:** [Hyperbolic surface](#hyperbolic-surface)

In curvature $-1$, its length is $2\operatorname{arcosh}3$. The level-two [principal congruence subgroup](group-theory.md#principal-congruence-subgroup) has traces congruent to two modulo four, so the smallest hyperbolic absolute [trace](linear-algebra.md#matrix-trace) is six, achieved by $\begin{pmatrix}5&2\\2&1\end{pmatrix}$. The [hyperbolic translation length](#hyperbolic-translation-length) formula gives the result; the shortest closed [geodesic](riemannian-geometry.md#geodesic) is nonsimple.

### Pants decomposition

↑ **Parent:** [Hyperbolic surface](#hyperbolic-surface)

A collection of disjoint essential [simple closed curves](geometry-and-topology.md#simple-closed-curve) that cuts a closed [genus](topological-surface.md#genus-of-a-surface)-$g$ surface into $2g-2$ surfaces of type [pair of pants](topological-surface.md#pair-of-pants-mathematics). There are $3g-3$ curves. [Geodesic](riemannian-geometry.md#geodesic) representatives are used for [Fenchel–Nielsen coordinates](#fenchel-nielsen-coordinates).

#### Elementary move of a pants decomposition

↑ **Parent:** [Pants decomposition](#pants-decomposition)

An elementary move replaces one cuff inside the four-holed sphere or one-holed torus obtained by uniting its adjacent pants. The replacement is an essential curve meeting the old cuff minimally. It changes the [pants decomposition graph](#pants-decomposition-graph) without changing the underlying surface; the identity surface map identifies the two descriptions.

#### Pants decomposition graph

↑ **Parent:** [Pants decomposition](#pants-decomposition)

The graph of a [pants decomposition](#pants-decomposition) has one vertex per [pair of pants](topological-surface.md#pair-of-pants-mathematics) and one edge per glued cuff. It is a connected trivalent multigraph, possibly with loops. A closed surface of genus $g$ gives $2g-2$ vertices and $3g-3$ edges, so its first [Betti number](homology.md#betti-number) is $g$. The graph records a decomposition rather than the homeomorphism class alone, and omits cuff lengths and twists.

#### Bers pants decomposition theorem

↑ **Parent:** [Pants decomposition](#pants-decomposition)

For fixed $g\geq2$, a constant $B_g$ bounds all cuff lengths in some [pants decomposition](#pants-decomposition) of every closed [genus](topological-surface.md#genus-of-a-surface)-$g$ [hyperbolic surface](#hyperbolic-surface). Together with [Fenchel–Nielsen coordinates](#fenchel-nielsen-coordinates) this implies [Mumford's compactness theorem](geometry-and-topology.md#mumford-s-compactness-theorem).

<h4 id="fenchel-nielsen-coordinates">Fenchel–Nielsen coordinates</h4>

↑ **Parent:** [Pants decomposition](#pants-decomposition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fenchel–Nielsen_coordinates)

For a fixed [pants decomposition](#pants-decomposition), the positive cuff lengths and real twist parameters give coordinates on [Teichmüller space](riemann-surfaces.md#teichmuller-space). With twists measured in length units, a full [Dehn twist](topological-surface.md#dehn-twist) changes $\tau_i$ by $\ell_i$; with angle units it changes the twist by $2\pi$.

<h5 id="fenchel-nielsen-twist">Fenchel–Nielsen twist</h5>

↑ **Parent:** [Fenchel–Nielsen coordinates](#fenchel-nielsen-coordinates)

After cutting a [hyperbolic surface](#hyperbolic-surface) along a simple closed [geodesic](riemannian-geometry.md#geodesic), reglue its two boundary copies after an arclength displacement $\tau$. The boundary length remains fixed, while the [Riemannian metric](riemannian-metric.md) varies. In marked [Fenchel–Nielsen coordinates](#fenchel-nielsen-coordinates), the twist is real-valued; changing it by one boundary length corresponds to a [Dehn twist](topological-surface.md#dehn-twist) in the marking. This construction also applies to a hyperbolic pair of pants with a fixed cone angle and two geodesic boundaries.

##### Finite length coordinates for hyperbolic surfaces

↑ **Parent:** [Fenchel–Nielsen coordinates](#fenchel-nielsen-coordinates)

For a fixed [pants decomposition](#pants-decomposition) of a closed [genus](topological-surface.md#genus-of-a-surface)-$g$ [hyperbolic surface](#hyperbolic-surface), its $3g-3$ cuff lengths determine all its [Y-pieces](topological-surface.md#hyperbolic-y-piece). Two suitably chosen transverse simple closed curves at each cuff, one obtained from the other by a [Dehn twist](topological-surface.md#dehn-twist), determine the corresponding twist: hyperbolic seam identities express their lengths through shifted hyperbolic cosines of that twist, removing the sign ambiguity of just one transversal. Thus finitely many marked lengths determine the [Fenchel–Nielsen coordinates](#fenchel-nielsen-coordinates). The unmarked [length spectrum](#length-spectrum) lacks these labels, which is why this fact alone does not imply global spectral uniqueness.

### Collar lemma

↑ **Parent:** [Hyperbolic surface](#hyperbolic-surface)

A [simple closed curve](geometry-and-topology.md#simple-closed-curve) that is a [geodesic](riemannian-geometry.md#geodesic) of length $\ell$ on a [hyperbolic surface](#hyperbolic-surface) has an embedded collar of half-width $w$ with $\sinh w\,\sinh(\ell/2)=1$. In circumference-one coordinates its metric is $dr^2+\ell^2\cosh^2r\,dt^2$, and its [conformal modulus of an annulus](riemann-surfaces.md#conformal-modulus-of-an-annulus) is $(2/\ell)\arctan(\operatorname{csch}(\ell/2))\sim\pi/\ell$.

### Hyperbolic systole

↑ **Parent:** [Hyperbolic surface](#hyperbolic-surface)

The [infimum](real-analysis.md#infimum) of nonconstant closed [geodesic](riemannian-geometry.md#geodesic) lengths in curvature $-1$, with value $+\infty$ if there are none. On a [closed surface](smooth-manifold.md#closed-surface) with a [hyperbolic metric](#hyperbolic-metric) this is a positive attained minimum, and a minimizing [geodesic](riemannian-geometry.md#geodesic) is simple. For fixed closed [genus](topological-surface.md#genus-of-a-surface) $g\geq2$, a common positive lower bound gives relative compactness in the unmarked [moduli space of Riemann surfaces](geometry-and-topology.md#moduli-space-of-riemann-surfaces) by [Mumford's compactness theorem](geometry-and-topology.md#mumford-s-compactness-theorem).

### Hyperbolic area

↑ **Parent:** [Hyperbolic surface](#hyperbolic-surface)

The metric area of a [hyperbolic surface](#hyperbolic-surface). In the [Poincaré half-plane model](#poincare-half-plane-model) the density is $dx\,dy/y^2$. A finite-area torsion-free quotient of [genus](topological-surface.md#genus-of-a-surface) $g$ with $r$ cusps has area $2\pi(2g-2+r)$ by the [Gauss-Bonnet theorem](differential-geometry.md#gauss-bonnet-theorem).

## Hyperbolic metric

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)

A hyperbolic metric is a complete Riemannian metric of constant sectional curvature $-1$. On a surface it supplies local charts modeled on the [hyperbolic plane](#hyperbolic-plane).

### Poincare metric on a Riemann surface

↑ **Parent:** [Hyperbolic metric](#hyperbolic-metric)

A connected [Riemann surface](riemann-surfaces.md) whose [universal cover](algebraic-topology.md#universal-cover) is the [unit disc](topology.md#unit-disc) inherits the complete curvature-minus-one metric displayed on its cover. [Möbius transformations](group-theory.md#mobius-transformation) preserving the disc are isometries, so [deck transformations](algebraic-topology.md#deck-transformation) preserve the metric and it descends to the surface. This uniformization notion must be distinguished from the potential-theoretic existence of a Green function. [Holomorphic maps](riemann-surfaces.md#holomorphic-map) between such surfaces contract their metric by lifting to [Schwarz-Pick theorem](analysis.md#schwarz-pick-theorem) on the covers.

#### Hyperbolic tube around a radial segment

↑ **Parent:** [Poincare metric on a Riemann surface](#poincare-metric-on-a-riemann-surface)

Under the [Cayley transform between the half-plane and disk](complex-analysis.md#cayley-transform-between-the-half-plane-and-disk), a radial segment ending at a boundary point becomes a vertical half-ray. If a point is within [hyperbolic distance](#hyperbolic-distance) $k$ of that half-ray, it lies in a fixed angular sector. Indeed, in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), $\cosh\rho(w,iy)=(|w|^2+y^2)/(2y\operatorname{Im}w)\geq|w|/\operatorname{Im}w$. This converts bounded hyperbolic approach to a boundary point into nontangential approach, allowing [normal-family proof of angular boundary convergence](complex-dynamics.md#normal-family-proof-of-angular-boundary-convergence) to transfer radial limits of bounded [holomorphic functions](holomorphic-function.md).

#### Hyperbolic derivative density

↑ **Parent:** [Poincare metric on a Riemann surface](#poincare-metric-on-a-riemann-surface)

For a nonconstant [holomorphic map](riemann-surfaces.md#holomorphic-map) into the [unit disc](topology.md#unit-disc), the displayed density pulls the target [hyperbolic metric](#hyperbolic-metric) back to the source Euclidean coordinate. It is not the operator norm between two hyperbolic tangent spaces, which additionally divides by the source metric density. Away from [ramification points](riemann-surfaces.md#ramification-point-of-a-holomorphic-map) $\Delta\log H_g=H_g^2$; a [ramification point](riemann-surfaces.md#ramification-point-of-a-holomorphic-map) of [multiplicity](polynomial.md#multiplicity-mathematics) $m$ adds $2\pi m$ times its point mass to the distributional [Laplacian](multivariable-calculus.md#laplacian).

##### Hyperbolic characteristic of a disc map

↑ **Parent:** [Hyperbolic derivative density](#hyperbolic-derivative-density)

This logarithmic area integral measures the accumulated pullback [hyperbolic metric](#hyperbolic-metric) area of a [holomorphic](holomorphic-function.md) disc map. Its nonnegative kernel makes it increasing in $R$. [Schwarz-Pick theorem](analysis.md#schwarz-pick-theorem) bounds $H_g(z)$ by $2/(1-|z|^2)$, which controls its characteristic through a critical-point Jensen identity.

###### Critical-point Jensen identity for the hyperbolic derivative

↑ **Parent:** [Hyperbolic characteristic of a disc map](#hyperbolic-characteristic-of-a-disc-map)

For $g'(0)\ne0$, apply [Jensen's formula](holomorphic-function.md#jensen-s-formula) with the smooth curvature term to the [hyperbolic derivative density](#hyperbolic-derivative-density). Its distributional [Laplacian](multivariable-calculus.md#laplacian) is $H_g^2+2\pi\sum m_a\delta_a$, giving the displayed identity with [ramification points](riemann-surfaces.md#ramification-point-of-a-holomorphic-map) defined by $g'(a)=0$. If $g'(z)=cz^m+\cdots$ at zero, use $m\log R$ as the origin counting term and replace the base constant by $\log\lim_{z\to0}H_g(z)/|z|^m$. Without this regularization the basepoint-critical formula is undefined.

### Hyperbolic metric on the punctured disk

↑ **Parent:** [Hyperbolic metric](#hyperbolic-metric)

The [universal covering map](algebraic-topology.md#universal-cover) $\tau\mapsto e^{i\tau}$ from the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) to the punctured [unit disc](topology.md#unit-disc) pulls back the metric $|dz|/(|z|\log(1/|z|))$ to $|d\tau|/\operatorname{Im}\tau$. This is its complete curvature-minus-one [hyperbolic metric](#hyperbolic-metric), which is different from restricting the ordinary disk metric to the punctured disk.

// Destination: analysis.bigb

#### Hyperbolic zero sequences on a punctured disk

↑ **Parent:** [Hyperbolic metric on the punctured disk](#hyperbolic-metric-on-the-punctured-disk)

The curvature-minus-one [hyperbolic metric on the punctured disk](#hyperbolic-metric-on-the-punctured-disk) assigns distance $2\log n$ along the radial geodesic from $e^{-1}$ to $e^{-n^2}$. Its exponential distances therefore sum to a finite value; the [triangle inequality](topological-analysis.md#triangle-inequality) gives the same conclusion for any fixed basepoint. Nevertheless no nonzero bounded [holomorphic function](holomorphic-function.md) has these zeros: the [Riemann removable singularity theorem](isolated-singularity.md#riemann-removable-singularity-theorem) extends it at zero, and the [identity theorem](complex-analysis.md#identity-theorem) then makes it identically zero. Simple connectivity is necessary in the hyperbolic characterization of bounded analytic zero sets.

### Pseudohyperbolic distance

↑ **Parent:** [Hyperbolic metric](#hyperbolic-metric)

On the [unit disc](topology.md#unit-disc), the [pseudohyperbolic distance](#pseudohyperbolic-distance) is

$$
\delta(z,w)=\left|\frac{z-w}{1-\overline wz}\right|.
$$

It is invariant under disc [Möbius transformations](group-theory.md#mobius-transformation). For the curvature-minus-one [hyperbolic metric](#hyperbolic-metric) with length element $2|dz|/(1-|z|^2)$, $\delta(z,w)=\tanh(\rho(z,w)/2)$ and $e^{-\rho(z,w)}=(1-\delta)/(1+\delta)$. The [Schwarz-Pick theorem](analysis.md#schwarz-pick-theorem) says that [holomorphic functions](holomorphic-function.md) from the disc into itself contract this distance. A [Blaschke factor](group-theory.md#blaschke-factor) has modulus $\delta(z,a)$, so the distance also controls the size of a product with prescribed zeros.

## Hyperbolic plane

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbolic_plane)

The hyperbolic plane is the simply connected two-dimensional geometry of constant curvature minus one.

### Hyperbolic polygon

↑ **Parent:** [Hyperbolic plane](#hyperbolic-plane)

A [geodesic](riemannian-geometry.md#geodesic) polygon in the [hyperbolic plane](#hyperbolic-plane) is bounded by finitely many [geodesic](riemannian-geometry.md#geodesic) segments. For curvature $-1$, its [area](differential-geometry.md#surface-area) is its angle defect, as given by [hyperbolic polygon area](#hyperbolic-polygon-area). Pairing equally long edges produces [hyperbolic surfaces](#hyperbolic-surface), with smoothness at glued vertices determined by their total angles.

### Ideal hyperbolic quadrilateral

↑ **Parent:** [Hyperbolic plane](#hyperbolic-plane)

An ideal hyperbolic quadrilateral is the region bounded by four [hyperbolic geodesics](#geodesic-in-the-poincare-half-plane-model) whose four consecutive endpoints are distinct points on the ideal boundary. The ideal vertices lie outside the [hyperbolic plane](#hyperbolic-plane). In the [hyperbolic disk](#hyperbolic-disc), the four vertices $1,i,-1,-i$ give a regular example: its sides are the interior arcs of the circles of radius one centered at $\pm1\pm i$. Although the sides have infinite length, the quadrilateral has finite [hyperbolic area](#hyperbolic-area) $2\pi$ in curvature $-1$.

### Hyperbolic disc

↑ **Parent:** [Hyperbolic plane](#hyperbolic-plane)

A hyperbolic disc consists of points within a specified [hyperbolic distance](#hyperbolic-distance) of its centre. In the [Poincare disc model](#poincare-disk-model), the disc centred at zero with radius $\rho$ has Euclidean radius $\tanh(\rho/2)$; an [isometry](riemannian-geometry.md#isometry) transports this description to any other centre.

### Horocycle

↑ **Parent:** [Hyperbolic plane](#hyperbolic-plane)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Horocycle)

A horocycle in the [Poincare disc model](#poincare-disk-model) is a Euclidean [circle](topology.md#circle) internally tangent to the boundary [circle](topology.md#circle). In the [upper half-plane model](#poincare-half-plane-model), a horocycle is a Euclidean [circle](topology.md#circle) tangent to the real axis from above, or a horizontal line $y=h>0$. The common geometric feature is a single [ideal centre of a horocycle](#ideal-centre-of-a-horocycle).

#### Common orthogonal line of two horocycles

↑ **Parent:** [Horocycle](#horocycle)

Two [horocycles](#horocycle) have a unique common orthogonal [hyperbolic line](#hyperbolic-line) when their [ideal centres of horocycles](#ideal-centre-of-a-horocycle) differ: it is the line with those two [ideal endpoints](#ideal-endpoint). If the centres agree, an [isometry](riemannian-geometry.md#isometry) puts both [horocycles](#horocycle) on horizontal lines; every vertical [hyperbolic line](#hyperbolic-line) meets both orthogonally, so there are infinitely many. This classification remains valid for intersecting or tangent [horocycles](#horocycle).

#### Ideal centre of a horocycle

↑ **Parent:** [Horocycle](#horocycle)

The ideal centre of a [horocycle](#horocycle) is its point of tangency to the boundary at infinity; a horizontal [horocycle](#horocycle) in the [upper half-plane model](#poincare-half-plane-model) has centre infinity. Sending the centre to infinity by an [isometry](riemannian-geometry.md#isometry) makes the [horocycle](#horocycle) horizontal. Orthogonal [hyperbolic lines](#hyperbolic-line) then become vertical, proving that a [hyperbolic line](#hyperbolic-line) meets a [horocycle](#horocycle) orthogonally exactly when it has the centre as an [ideal endpoint](#ideal-endpoint).

### Hyperbolic circle

↑ **Parent:** [Hyperbolic plane](#hyperbolic-plane)

A hyperbolic circle of centre $o$ and radius $R>0$ is the [level set](topology.md#level-set) $\{x:d_{\mathbb H}(o,x)=R\}$ for the [hyperbolic distance](#hyperbolic-distance). Equally spaced directions from its centre give vertices of a regular geodesic polygon.

#### Hyperbolic circle in the upper half-plane

↑ **Parent:** [Hyperbolic circle](#hyperbolic-circle)

In the [Poincaré half-plane model](#poincare-half-plane-model), a [hyperbolic circle](#hyperbolic-circle) of radius $R$ centred at $u+iv$ is the Euclidean circle $(x-u)^2+(y-v\cosh R)^2=v^2\sinh^2R$. Its Euclidean centre is shifted upward from its hyperbolic centre, and its Euclidean radius is $v\sinh R$. The lower height $ve^{-R}$ is positive. The formula follows by mapping the centre to zero in the [Poincare disc model](#poincare-disk-model) and using radial distance $2\operatorname{artanh}\rho$.

### Hyperbolic line

↑ **Parent:** [Hyperbolic plane](#hyperbolic-plane)

A hyperbolic line is a complete geodesic in the hyperbolic plane. In the Poincare half-plane model, hyperbolic lines are vertical rays and semicircles orthogonal to the boundary.

#### Ideal endpoint

↑ **Parent:** [Hyperbolic line](#hyperbolic-line)

An ideal endpoint of a [hyperbolic line](#hyperbolic-line) is one of its two limiting points on the boundary at infinity. In the [Poincare disc model](#poincare-disk-model) these lie on the unit [circle](topology.md#circle); in the [upper half-plane model](#poincare-half-plane-model) they lie on $\mathbb R\cup\{\infty\}$. These are boundary points, not points of the [hyperbolic plane](#hyperbolic-plane). Any two distinct [ideal endpoints](#ideal-endpoint) determine a unique [hyperbolic line](#hyperbolic-line).

#### Parallel hyperbolic lines

↑ **Parent:** [Hyperbolic line](#hyperbolic-line)

Two distinct [hyperbolic lines](#hyperbolic-line) are parallel, in the limiting-parallel convention, when they do not intersect in the [hyperbolic plane](#hyperbolic-plane) and have exactly one common [ideal endpoint](#ideal-endpoint). In the [upper half-plane model](#poincare-half-plane-model), distinct vertical lines are parallel, sharing infinity. Disjoint lines with no common [ideal endpoint](#ideal-endpoint) are instead [ultraparallel hyperbolic lines](#ultraparallel-hyperbolic-lines); only these have a [common perpendicular of ultraparallel hyperbolic lines](#common-perpendicular-of-ultraparallel-hyperbolic-lines).

#### Ultraparallel hyperbolic lines

↑ **Parent:** [Hyperbolic line](#hyperbolic-line)

Two hyperbolic lines are ultraparallel when they are disjoint and have no common ideal endpoint. They possess a unique common perpendicular, which realizes the distance between them.

### Hyperbolic distance

↑ **Parent:** [Hyperbolic plane](#hyperbolic-plane)

Hyperbolic distance is the [Riemannian distance](riemannian-geometry.md#riemannian-distance) induced by the [hyperbolic metric](#hyperbolic-metric).

### Horoball

↑ **Parent:** [Hyperbolic plane](#hyperbolic-plane)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Horoball)

A horoball in the hyperbolic plane is a region bounded by a horocycle. In the upper-half-plane model, a horoball based at infinity is a Euclidean half-plane $\{y>c\}$; quotients by parabolic isometries give cusp neighborhoods.

### Finite-order elliptic transformation

↑ **Parent:** [Hyperbolic plane](#hyperbolic-plane)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite-order_elliptic_transformation)

A noncentral finite-order orientation-preserving hyperbolic isometry fixes an interior point and is elliptic.

<h2 id="poincare-disk-model">Poincaré disk model</h2>

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincaré_disk_model)

The Poincare disc carries the metric $4|dz|^2/(1-|z|^2)^2$ on $|z|<1$.

### Poincare disc automorphism

↑ **Parent:** [Poincaré disk model](#poincare-disk-model)

For $|a|<1$, the [Möbius transformation](group-theory.md#mobius-transformation) $f_a(z)=(z-a)/(1-\overline az)$ is an [isometry](riemannian-geometry.md#isometry) of the [Poincare disc model](#poincare-disk-model) sending $a$ to zero. Rotations combined with these transformations describe its orientation-preserving [isometries](riemannian-geometry.md#isometry).

### Area of a hyperbolic disc

↑ **Parent:** [Poincaré disk model](#poincare-disk-model)

In curvature minus one, a hyperbolic disc of radius $R$ has area

$$
A(R)=4\pi\sinh^2(R/2)=2\pi(\cosh R-1).
$$

In the Poincare disc this follows by integrating $4r(1-r^2)^{-2}\,dr\,d\theta$ up to Euclidean radius $\tanh(R/2)$.

#### Hyperbolic area bounds an inscribed disc

↑ **Parent:** [Area of a hyperbolic disc](#area-of-a-hyperbolic-disc)

If a domain of finite [hyperbolic area](#hyperbolic-area) $A$ contains a hyperbolic disc of radius $r$ in curvature $-1$, then $2\pi(\cosh r-1)\leq A$, hence $r\leq\operatorname{arcosh}(1+A/(2\pi))$. For an interior point of a [hyperbolic triangle](#hyperbolic-triangle), the open disc with radius equal to its distance from the boundary lies inside the triangle. Its area is at most $\pi$ by [Gauss-Bonnet theorem](differential-geometry.md#gauss-bonnet-theorem), giving the elementary bound $r\leq\operatorname{arcosh}(3/2)$; this need not be the sharp triangle inradius bound.

#### Radial chain of equal hyperbolic discs

↑ **Parent:** [Area of a hyperbolic disc](#area-of-a-hyperbolic-disc)

Hyperbolic discs of area $\pi/2$ have radius $\log2$. Starting at the origin and placing their centers successively along one radial geodesic gives center distance $n\log4$ and Euclidean coordinate

$$
r_n=\frac{4^n-1}{4^n+1}.
$$

### Geodesic obstruction for a horizontal chain of hyperbolic discs

↑ **Parent:** [Poincaré disk model](#poincare-disk-model)

An isometry sends the centers of a collinear family of equal hyperbolic discs to points on one hyperbolic geodesic. In the upper-half-plane model no geodesic contains three distinct points on a horizontal Euclidean line, since geodesics are vertical lines or semicircles orthogonal to the boundary.

### Hyperbolic length in the Poincare disc

↑ **Parent:** [Poincaré disk model](#poincare-disk-model)

For a piecewise smooth curve $z(t)$ in the Poincare disc, its hyperbolic length is

$$
L(z)=\int\frac{2|\dot z(t)|}{1-|z(t)|^2}\,dt.
$$

### Geodesics of the Poincare disc

↑ **Parent:** [Poincaré disk model](#poincare-disk-model)

The geodesics are diameters and arcs of circles orthogonal to the unit circle. A radial segment is length minimizing because

$$
\int\frac{2\sqrt{\dot r^{,2}+r^2\dot\theta^{,2}}}{1-r^2}\,dt
\geq2\operatorname{artanh}r,
$$

with equality for constant angle and monotone radius. Hence the distance from the origin to $z$ is $2\operatorname{artanh}|z|$.

### Hyperbolic distance in the Poincare disc

↑ **Parent:** [Poincaré disk model](#poincare-disk-model)

For $z_1,z_2$ in the [Poincare disc model](#poincare-disk-model), put

$$
\rho=\left|\frac{z_2-z_1}{1-\overline{z_1}z_2}\right|.
$$

Their [hyperbolic distance](#hyperbolic-distance) is

$$
d(z_1,z_2)=2\operatorname{artanh}\rho
=\log\frac{1+\rho}{1-\rho}.
$$

#### Hyperbolic geodesic cap

↑ **Parent:** [Hyperbolic distance in the Poincare disc](#hyperbolic-distance-in-the-poincare-disc)

For a proper arc $I$ of the boundary of the [unit disc](topology.md#unit-disc), $Q(I)$ is the side of the [hyperbolic geodesic](#geodesic-in-the-poincare-half-plane-model) between its endpoints adjacent to $I$. For short arcs this is a curved boundary cap. For arcs longer than a semicircle it contains the center. With endpoints $e^{\pm i\alpha}$ and $0<\alpha<\pi/2$, the geodesic is the circle with center $\sec\alpha$ and radius $\tan\alpha$, orthogonal to the [unit circle](complex-analysis.md#complex-unit-circle). It is a diameter at $\alpha=\pi/2$.

##### Geodesic-cap and Carleson-box comparison

↑ **Parent:** [Hyperbolic geodesic cap](#hyperbolic-geodesic-cap)

For a short arc $I$ of normalized length $\ell$, every point of its [hyperbolic geodesic cap](#hyperbolic-geodesic-cap) lies within Euclidean distance $C\ell$ of its center boundary point. Conversely, for any fixed $b>0$, the region with angular projection in $I$ and depth $1-|z|\le b\ell$ lies in $Q(\kappa I)$ for a fixed enlargement $\kappa$ depending only on $b$, when $I$ is sufficiently short. To verify this, rotate the midpoint to one and write the endpoints as $e^{\pm i\alpha}$. The cap inequality is $2\operatorname{Re}z>(1+|z|^2)\cos\alpha$. Its radial depth at the midpoint is $1-\sec\alpha+\tan\alpha$, comparable to $\alpha$ for small $\alpha$; its angular projection lies in $I$. Enlarging $\alpha$ by a sufficiently large fixed factor makes the inequality hold throughout the indicated rectangle. Large arcs use a finite cover of the disc. Thus [Carleson boxes](harmonic-analysis.md#carleson-box) and [hyperbolic geodesic caps](#hyperbolic-geodesic-cap) define equivalent [Carleson measure](harmonic-analysis.md#carleson-measure) conditions.

The rectangle containment can also be checked directly. Write $z=re^{i\theta}$ with $|\theta|\le\pi\ell$ and $1-r\le b\ell$. Its membership in the enlarged cap is equivalent to

$$
\cos\theta-\cos(\kappa\pi\ell)>\frac{(1-r)^2}{2r}\cos(\kappa\pi\ell).
$$

For small enough $\ell$, $r\ge1/2$. The right side is at most $b^2\ell^2$, while the left side is at least $(\kappa^2-1)\pi^2\ell^2/8$, using the sine product formula and $\sin x\ge x/2$ for small positive $x$. Thus $\kappa=4+4b/\pi$ suffices.

### Euclidean circle representing a perpendicular hyperbolic line

↑ **Parent:** [Poincaré disk model](#poincare-disk-model)

If $P$ is at hyperbolic distance $\rho$ from the origin, the Poincare-disc geodesic through $P$ perpendicular to $OP$ is represented by a Euclidean circle of radius $\operatorname{csch}\rho$ whose centre is at Euclidean distance $\coth\rho$ from the origin.

<h2 id="poincare-half-plane-model">Poincaré half-plane model</h2>

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincaré_half-plane_model)

The upper half-plane carries the hyperbolic metric $(dx^2+dy^2)/y^2$.

### Hyperbolic translation length

↑ **Parent:** [Poincaré half-plane model](#poincare-half-plane-model)

For a [hyperbolic Möbius transformation](#hyperbolic-element-of-psl2-r) represented by $A\in\mathrm{SL}_2(\mathbb R)$, the infimum of $d(z,Az)$ is attained on its axis and equals $2\operatorname{arcosh}(|\operatorname{tr}A|/2)$. It is the length of the corresponding closed [geodesic](riemannian-geometry.md#geodesic) in a quotient.

#### Polynomial encoding of hyperbolic geodesic lengths

↑ **Parent:** [Hyperbolic translation length](#hyperbolic-translation-length)

For a determinant-one lift of a [hyperbolic holonomy representation](#hyperbolic-holonomy-representation), the squared [matrix trace](linear-algebra.md#matrix-trace) of each fixed group word is a [polynomial](polynomial.md) in the finitely many generator-matrix entries. The displayed identity identifies equal positive lengths with equal squared traces. Lift signs have no effect. Finite choices of length matchings therefore give finite unions of [affine algebraic sets](algebraic-variety.md#affine-algebraic-set).

### Hyperbolic distance in the Poincare half-plane

↑ **Parent:** [Poincaré half-plane model](#poincare-half-plane-model)

For $z,w$ in the upper half-plane,

$$
\cosh d(z,w)=1+\frac{|z-w|^2}{2\operatorname{Im}z\operatorname{Im}w}.
$$

#### Equality of horizontal hyperbolic and Euclidean distances

↑ **Parent:** [Hyperbolic distance in the Poincare half-plane](#hyperbolic-distance-in-the-poincare-half-plane)

For points $ib$ and $a+ib$ with $a,b>0$, the [hyperbolic distance](#hyperbolic-distance) is $2\operatorname{arsinh}(a/(2b))$. It equals their Euclidean distance $a$ exactly when the displayed relation holds. The function of $a$ decreases continuously from one to zero: its derivative has the sign of $\sinh(a/2)-(a/2)\cosh(a/2)<0$. Hence every height $b\in(0,1)$ has exactly one positive matching horizontal separation.

### Geodesic in the Poincare half-plane model

↑ **Parent:** [Poincaré half-plane model](#poincare-half-plane-model)

The geodesics in the upper half-plane are vertical lines and semicircles centred on the boundary axis. Indeed, the length integrand $\sqrt{1+y'^2}/y$ has the [Beltrami identity](analysis.md#beltrami-identity)

$$
\frac1{y\sqrt{1+y'^2}}=\frac1R,
$$

which integrates to $(x-c)^2+y^2=R^2$. Swapping the coordinate axes gives circles centred on the vertical boundary for the metric $(dx^2+dy^2)/x^2$.

#### Calibration for semicircular hyperbolic geodesics

↑ **Parent:** [Geodesic in the Poincare half-plane model](#geodesic-in-the-poincare-half-plane-model)

In the upper half-plane $y>0$, the [hyperbolic length](#hyperbolic-length-in-the-poincare-disc) element is $ds/y$. The function $\Phi=\operatorname{arsinh}(x/y)$ has [gradient](multivariable-calculus.md#gradient) $(1,-x/y)/\sqrt{x^2+y^2}$ and norm $1/y$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\int ds/y\geq\Phi(B)-\Phi(A)$ for any oriented path from $A$ to $B$. Equality holds along a semicircle $x^2+y^2=R^2$ traversed with increasing $x$, because its tangent is parallel to that gradient. This is a [calibration](differential-geometry.md#calibration-differential-geometry) proof of global minimality, beyond the stationary-path conclusion of the [Beltrami identity](analysis.md#beltrami-identity). Translating $x$ gives the analogous proof for semicircles with other boundary centers.

#### Common perpendicular of ultraparallel hyperbolic lines

↑ **Parent:** [Geodesic in the Poincare half-plane model](#geodesic-in-the-poincare-half-plane-model)

Two disjoint hyperbolic lines with four distinct ideal endpoints have a unique common perpendicular, and the segment of that perpendicular between them realizes their minimum distance. An upper-half-plane isometry can make the two lines concentric semicircles; their common perpendicular then becomes the imaginary axis.

##### Configurations of three ultraparallel lines

↑ **Parent:** [Common perpendicular of ultraparallel hyperbolic lines](#common-perpendicular-of-ultraparallel-hyperbolic-lines)

Three pairwise [ultraparallel hyperbolic lines](#ultraparallel-hyperbolic-lines) may have disjoint common perpendiculars or coincident ones. In the upper-half-plane model, three semicircles of radius $1/2$ centred at $-5/2,0,5/2$ have mutually disjoint common perpendiculars. Three concentric semicircles instead have the same vertical common perpendicular. Thus pairwise ultraparallelism alone does not determine the incidence of their perpendiculars.

#### Hyperbolic lines meeting the imaginary axis at a fixed angle

↑ **Parent:** [Geodesic in the Poincare half-plane model](#geodesic-in-the-poincare-half-plane-model)

The hyperbolic metric in the half-plane model is conformal, so hyperbolic and Euclidean angles agree. The line meeting the imaginary axis at $iy$, $y>0$, at signed angle $\alpha\in(0,\pi)$ is represented by the Euclidean circle with centre $y\cot\alpha$ on the real axis and radius $y\csc\alpha$.

<h3 id="psl2-r">PSL2(R)</h3>

↑ **Parent:** [Poincaré half-plane model](#poincare-half-plane-model)

PSL2(R) is $SL_2(\mathbb R)/\{\pm I\}$. It acts on the upper half-plane by the Möbius transformations

$$
z\longmapsto\frac{az+b}{cz+d}
$$

and is the group of orientation-preserving hyperbolic isometries.

<h4 id="hyperbolic-element-of-psl2-r">Hyperbolic element of PSL2(R)</h4>

↑ **Parent:** [PSL2(R)](#psl2-r)

A real [Möbius transformation](group-theory.md#mobius-transformation) represented by $A\in\mathrm{SL}_2(\mathbb R)$ with $|\operatorname{tr}A|>2$. It has two fixed ideal boundary points and translates along the [geodesic](riemannian-geometry.md#geodesic) joining them; its [hyperbolic translation length](#hyperbolic-translation-length) is $2\operatorname{arcosh}(|\operatorname{tr}A|/2)$. Conjugating by a real [Möbius transformation](group-theory.md#mobius-transformation) puts it in the form $z\mapsto e^\ell z$ with $\ell>0$; its axis is then the imaginary axis.

<h4 id="elliptic-element-of-psl2-r">Elliptic element of PSL2(R)</h4>

↑ **Parent:** [PSL2(R)](#psl2-r)

A real [Möbius transformation](group-theory.md#mobius-transformation) represented by $A\in\mathrm{SL}_2(\mathbb R)$ with $|\operatorname{tr}A|<2$. It fixes a point of the [Poincaré half-plane model](#poincare-half-plane-model); an integral matrix of this type has [trace](linear-algebra.md#matrix-trace) $0$ or $\pm1$. In the [Poincare disc model](#poincare-disk-model), moving its fixed point to zero makes it a rotation about zero.

<h4 id="parabolic-element-of-psl2-r">Parabolic element of PSL2(R)</h4>

↑ **Parent:** [PSL2(R)](#psl2-r)

A nonidentity real [Möbius transformation](group-theory.md#mobius-transformation) represented by $A\in\mathrm{SL}_2(\mathbb R)$ with $|\operatorname{tr}A|=2$. It has one ideal boundary fixed point and is conjugate to a nonzero translation on the [Poincaré half-plane model](#poincare-half-plane-model).

#### Isometry group of the Poincare half-plane

↑ **Parent:** [PSL2(R)](#psl2-r)

Every orientation-preserving isometry of the [Poincaré half-plane model](#poincare-half-plane-model) lies in $PSL_2(\mathbb R)$. Every orientation-reversing isometry is the composition of one of these with the [hyperbolic reflection](#hyperbolic-reflection) $z\mapsto-\overline z$ in the imaginary axis. Equivalently, the full isometry group consists of real Möbius and anti-Möbius transformations, modulo nonzero scalar matrices.

#### Transitivity on pointed hyperbolic lines

↑ **Parent:** [PSL2(R)](#psl2-r)

The group $PSL_2(\mathbb R)$ acts transitively on pairs $(\ell,P)$ consisting of a hyperbolic line and a point on it. Send the two ideal endpoints of $\ell$ to $0$ and $\infty$, then use a positive dilation to move the resulting point on the imaginary axis to $i$.

### Hyperbolic reflection

↑ **Parent:** [Poincaré half-plane model](#poincare-half-plane-model)

Reflection in a hyperbolic line is the unique orientation-reversing hyperbolic isometry fixing that line pointwise. The product of reflections in intersecting lines is a rotation through twice their angle.

#### Every hyperbolic-plane isometry is a product of at most three reflections

↑ **Parent:** [Hyperbolic reflection](#hyperbolic-reflection)

A reflection in the perpendicular bisector of a point and its image corrects that point. A second bisector reflection through the corrected point can correct another point without moving the first. An [isometry](riemannian-geometry.md#isometry) fixing two distinct points is either the identity or reflection in their joining geodesic: points with prescribed distances from both centres have at most two possibilities, exchanged by that reflection. Fixing a third noncollinear point then fixes every point. This constructs a factorization with at most three [hyperbolic reflections](#hyperbolic-reflection).

#### Composition of reflections in ultraparallel hyperbolic lines

↑ **Parent:** [Hyperbolic reflection](#hyperbolic-reflection)

The composition of [hyperbolic reflections](#hyperbolic-reflection) in two [ultraparallel hyperbolic lines](#ultraparallel-hyperbolic-lines) has infinite order. Map their common perpendicular to the [imaginary axis](complex-analysis.md#imaginary-axis) in the [Poincaré half-plane model](#poincare-half-plane-model). The two reflecting [hyperbolic lines](#hyperbolic-line) become semicircles centred at zero, with distinct radii $r_1,r_2$. Reflection in the radius-$r$ semicircle is $z\mapsto r^2/\overline z$, so their composition is $z\mapsto(r_2/r_1)^2z$. Every positive power remains nonidentity, because $(r_2/r_1)^{2k}\ne1$ for $k\ge1$.

### Hyperbolic half-turn

↑ **Parent:** [Poincaré half-plane model](#poincare-half-plane-model)

A hyperbolic half-turn is the unique orientation-preserving isometry of order two fixing a given point. It exchanges every pair of points lying at equal opposite distances along a geodesic through its centre.

## Cayley transform (hyperbolic geometry)

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cayley_transform_(hyperbolic_geometry))

The map $z\mapsto i(1+z)/(1-z)$ is an isometry from the Poincare disc to the upper half-plane.

## Hyperboloid model

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperboloid_model)

The hyperboloid model of the curvature-minus-one hyperbolic plane is

$$
\{x\in\mathbb R^3:-x_0^2+x_1^2+x_2^2=-1, x_0>0\}.
$$

Its metric is the restriction of the Minkowski bilinear form to tangent planes, and its geodesics are intersections with two-dimensional linear subspaces through the origin.

### Three-dimensional hyperboloid model

↑ **Parent:** [Hyperboloid model](#hyperboloid-model)

The three-dimensional hyperboloid model is

$$
\mathbb H^3
=\{x\in\mathbb R^4:x^TMx=-1,\ x_0>0\},
\qquad
M=\operatorname{diag}(-1,1,1,1).
$$

It is a regular level set with

$$
T_x\mathbb H^3=\{v\in\mathbb R^4:x^TMv=0\}.
$$

### Minkowski inner product

↑ **Parent:** [Hyperboloid model](#hyperboloid-model)

This indefinite bilinear form supplies the metric of [Minkowski spacetime](special-relativity.md#minkowski-spacetime). On $\mathbb R^{n+1}$ the Minkowski inner product with mostly-positive convention is

$$
\langle x,y\rangle_M=-x_0y_0+x_1y_1+\cdots+x_ny_n.
$$

## Lambert quadrilateral

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lambert_quadrilateral)

A Lambert quadrilateral is a hyperbolic quadrilateral with three right angles. If its remaining angle is $\theta$ and the two sides incident with that angle have lengths $a,b$, then

$$
\cos\theta=\tanh a\tanh b.
$$

## Hyperbolic triangle

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbolic_triangle)

A hyperbolic triangle is bounded by three hyperbolic geodesics and may have vertices on the ideal boundary.

### Hyperbolic triangle inradius bound

↑ **Parent:** [Hyperbolic triangle](#hyperbolic-triangle)

For curvature minus one, no [hyperbolic triangle](#hyperbolic-triangle) contains an open hyperbolic disc of radius greater than $\tfrac12\log3$. Move the disc centre to zero in the [Poincare disc model](#poincare-disk-model) and enclose the triangle in an ideal triangle with the same radial vertex directions. One gap between ideal directions is at least $2\pi/3$. Its opposite geodesic is at distance at most $2\operatorname{artanh}(2-\sqrt3)=\tfrac12\log3$ from zero. The symmetric [ideal hyperbolic triangle](#ideal-triangle) attains the bound as its inradius.

### Ideal triangle

↑ **Parent:** [Hyperbolic triangle](#hyperbolic-triangle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ideal_triangle)

An ideal hyperbolic triangle has all three vertices on the boundary at infinity of the [hyperbolic plane](#hyperbolic-plane). All its angles are zero and its [hyperbolic area](#hyperbolic-area) in curvature $-1$ is $\pi$, by [hyperbolic triangle area](#hyperbolic-triangle-area).

#### Ideal vertex

↑ **Parent:** [Ideal triangle](#ideal-triangle)

An [ideal vertex](#ideal-vertex) is a vertex at infinity of an [ideal triangle](#ideal-triangle) or another ideal hyperbolic polygon. An ideal vertex lies on the boundary at infinity and has internal angle zero.

### Hyperbolic side-side-angle ambiguity

↑ **Parent:** [Hyperbolic triangle](#hyperbolic-triangle)

Two corresponding side lengths and an equal nonincluded angle need not determine a [hyperbolic triangle](#hyperbolic-triangle). Set $A=\pi/6$, $\cosh a=3/2$, $\cosh b=2$. The [hyperbolic law of cosines](#hyperbolic-law-of-cosines) has two distinct positive solutions $c=\ln(3\pm\sqrt2)$. The two triangles share $a,b,A$ but have different third sides. An included angle instead determines the third side by the cosine rule.

### Hyperbolic side-side-side congruence

↑ **Parent:** [Hyperbolic triangle](#hyperbolic-triangle)

Three corresponding side lengths determine a [hyperbolic triangle](#hyperbolic-triangle) up to an [isometry](riemannian-geometry.md#isometry) of the [hyperbolic plane](#hyperbolic-plane). First match an ordered pair of vertices by an isometry. The third vertex lies at the intersection of two prescribed hyperbolic distance circles. There are at most two choices, interchanged by reflection in the geodesic through the matched pair; either choice can therefore be matched.

### Hyperbolic triangle area

↑ **Parent:** [Hyperbolic triangle](#hyperbolic-triangle)

For curvature $-1$, a triangle of angles $\alpha,\beta,\gamma$ has area $\pi-\alpha-\beta-\gamma$ by Gauss--Bonnet.

#### Hyperbolic polygon area

↑ **Parent:** [Hyperbolic triangle area](#hyperbolic-triangle-area)

For a geodesic hyperbolic $n$-gon of curvature $-1$ with interior angles $\alpha_1,\ldots,\alpha_n$, triangulation or the Gauss--Bonnet theorem gives

$$
\operatorname{area}=(n-2)\pi-\sum_{j=1}^n\alpha_j.
$$

##### Regular hyperbolic polygon with prescribed area

↑ **Parent:** [Hyperbolic polygon area](#hyperbolic-polygon-area)

In curvature $-1$, a regular $n$-gon of circumradius $R>0$ has interior angle $\alpha(R)=2\arctan(\cot(\pi/n)/\cosh R)$, by the right-triangle angle form of the [hyperbolic law of cosines](#hyperbolic-law-of-cosines). Thus its [hyperbolic polygon area](#hyperbolic-polygon-area) is $(n-2)\pi-n\alpha(R)$, continuously and strictly increasing from $0$ to $(n-2)\pi$. Every area in that open interval is therefore attained at exactly one circumradius.

### Hyperbolic law of cosines

↑ **Parent:** [Hyperbolic triangle](#hyperbolic-triangle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbolic_law_of_cosines)

For opposite side $a$, $\cosh a=(\cos\alpha+\cos\beta\cos\gamma)/(\sin\beta\sin\gamma)$.

#### Hyperbolic AAA congruence

↑ **Parent:** [Hyperbolic law of cosines](#hyperbolic-law-of-cosines)

A hyperbolic triangle is determined up to isometry by its three angles. Indeed, the angle form of the [hyperbolic law of cosines](#hyperbolic-law-of-cosines) determines every side length from the angles, after which hyperbolic side-side-side congruence determines the triangle. This differs from Euclidean geometry because hyperbolic space has an intrinsic length scale.

## Hyperbolic law of sines

↑ **Parent:** [Hyperbolic geometry](hyperbolic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbolic_law_of_sines)

For a hyperbolic triangle, $\sinh a/\sin\alpha=\sinh b/\sin\beta=\sinh c/\sin\gamma$.

## ↑ Ancestors (4)

1. [Geometry and topology](geometry-and-topology.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (2)

- [Triangle group](group.md#triangle-group)
- [Upper half-plane (complex analysis)](complex-analysis.md#upper-half-plane-complex-analysis)
