# Topological manifold

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_manifold)

A topological $n$-manifold without boundary is a [topological space](topology.md#topological-space) $M$ satisfying three conditions: it is [Hausdorff](topology.md#hausdorff-space), it is [second countable](topology.md#second-countable-space), and every point $p\in M$ lies in an [open set](topology.md#open-set) $U\subseteq M$ with a [homeomorphism](topology.md#homeomorphism) $\varphi:U\to V$ onto an [open set](topology.md#open-set) $V\subseteq\mathbb R^n$. Here $n\geq0$ is a fixed [dimension of a manifold](#dimension-of-a-manifold), and $\mathbb R^n$ has the usual [topology](topology.md) of [Euclidean space](normed-vector-space.md#euclidean-norm). The pair $(U,\varphi)$ is a [coordinate chart](differential-geometry.md#manifold-chart). Unless explicitly qualified, “topological manifold” here means without boundary.[Topology I: smooth manifolds, Week 1, Section 1.1, Definition 1.1, page 1](mathematics-bibliography.md#topology-i-smooth-manifolds-university-of-toronto-mat1300hf-2012/week-1-course-notes)

The [Hausdorff](topology.md#hausdorff-space) condition requires disjoint [open](topology.md#open-set) [neighbourhoods](topology.md#neighbourhood-mathematics) for distinct points. [Second countability](topology.md#second-countable-space) requires a [countable](cardinal-number.md#countable-set) [basis of a topology](topology.md#basis-of-a-topology). Neither follows merely from the local [homeomorphisms](topology.md#homeomorphism): [non-Hausdorff manifolds](topology.md#non-hausdorff-manifold) fail the first condition, while an uncountable [disjoint union](set-theory.md#disjoint-union) of copies of the [real line](real-analysis.md#real-line) fails the second. Indeed, a [basis of a topology](topology.md#basis-of-a-topology) must supply a different nonempty member inside each copy, so it cannot be [countable](cardinal-number.md#countable-set).

The [circle](topology.md#circle) and the [real line](real-analysis.md#real-line) are both one-dimensional [topological manifolds](topological-manifold.md), with the same local model. Their global [topologies](topology.md) differ: the [circle](topology.md#circle) is [compact](topology.md#compact-space), while the [real line](real-analysis.md#real-line) is not. By contrast, the junction of a [topological tripod](#topological-tripod) already fails the local test. Thus local [coordinate charts](differential-geometry.md#manifold-chart) specify what kind of small pieces are allowed; global [topological invariants](topology.md#topological-invariant) distinguish how those pieces fit together.[Introduction to Topological Manifolds by John M. Lee, second edition, Chapter 1, pages 1–3 on local models and pages 5–6 on topological invariants](mathematics-bibliography.md#introduction-to-topological-manifolds-second-edition-by-john-m-lee/introduction)

The usefulness of a [topological manifold](topological-manifold.md) is that local questions about [continuity](calculus.md#continuous-function) can be transported into [Euclidean space](normed-vector-space.md#euclidean-norm), while [compactness](topology.md#compact-space), [connectedness](geometry-and-topology.md#connected-space), and the [fundamental group](algebraic-topology.md#fundamental-group) still record global information. For [calculus](calculus.md), further structure is needed: a [smooth atlas](differential-geometry.md#smooth-atlas) requires [smooth transition maps](differential-geometry.md#smooth-transition-map), letting the [chain rule](calculus.md#chain-rule) reconcile [derivatives](calculus.md#derivative) computed in different [coordinate charts](differential-geometry.md#manifold-chart). A [topological atlas](#topological-atlas) by itself only guarantees [homeomorphisms](topology.md#homeomorphism) between coordinates.[Topology I: smooth manifolds, Week 2, Section 1.2, equation (11) and Definitions 1.15–1.16, pages 5–6](mathematics-bibliography.md#topology-i-smooth-manifolds-university-of-toronto-mat1300hf-2012/week-2-course-notes)

**Table of contents**

- [Topological atlas](#topological-atlas)
  - [Topological transition map](#topological-transition-map)
- [Two stereographic charts on the circle](#two-stereographic-charts-on-the-circle)
- [Topological manifold with boundary](#topological-manifold-with-boundary)
- [Category of topological manifolds](#category-of-topological-manifolds)
- [Piecewise linear ball](#piecewise-linear-ball)
  - [Gluing three-balls along a boundary disk](#gluing-three-balls-along-a-boundary-disk)
- [4-manifold](#4-manifold)
  - [Smooth four-manifold](#smooth-four-manifold)
    - [Fiber sum of four-manifolds](#fiber-sum-of-four-manifolds)
      - [Smooth fiber sum along unknotted null-homologous spheres](#smooth-fiber-sum-along-unknotted-null-homologous-spheres)
    - [Seiberg–Witten invariant of a four-manifold](#seiberg-witten-invariant-of-a-four-manifold)
      - [Connected-sum vanishing of the Seiberg–Witten invariant](#connected-sum-vanishing-of-the-seiberg-witten-invariant)
      - [Taubes nonvanishing theorem](#taubes-nonvanishing-theorem)
        - [Symplectic connected-sum obstruction](#symplectic-connected-sum-obstruction)
- [Double of a manifold](#double-of-a-manifold)
- [Topological tripod](#topological-tripod)
- [Invariance of domain](#invariance-of-domain)
- [Lorentzian manifold](#lorentzian-manifold)
  - [Metric signature](#metric-signature)
  - [Spacelike submanifold](#spacelike-submanifold)
- [Dimension of a manifold](#dimension-of-a-manifold)
  - [Codimension of a submanifold](#codimension-of-a-submanifold)
- [Handle attachment](#handle-attachment)
  - [Four-handle](#four-handle)
  - [Handle](#handle)
  - [Surgery on a smooth manifold](#surgery-on-a-smooth-manifold)
  - [Zero-handle](#zero-handle)
  - [Core disk of a handle](#core-disk-of-a-handle)
  - [Handle decomposition](#handle-decomposition)
    - [Critical level handle embedding](#critical-level-handle-embedding)
    - [Zero-framed Hopf-link handle decomposition of the sphere product](#zero-framed-hopf-link-handle-decomposition-of-the-sphere-product)
    - [Commutator handlebody of the torus](#commutator-handlebody-of-the-torus)
    - [Handle slide](#handle-slide)
      - [Handle-slide isolation of a cancelling pair](#handle-slide-isolation-of-a-cancelling-pair)
    - [Belt sphere](#belt-sphere)
    - [Attaching sphere](#attaching-sphere)
  - [Three-handle](#three-handle)
  - [Two-handle](#two-handle)
  - [One-handle](#one-handle)
- [3-manifold](#3-manifold)
  - [Normal surface](#normal-surface)
    - [Normal surface coordinates](#normal-surface-coordinates)
      - [Normal surface weight](#normal-surface-weight)
      - [Haken sum](#haken-sum)
      - [Fundamental normal surface](#fundamental-normal-surface)
  - [Punctured three-sphere](#punctured-three-sphere)
    - [Sphere surgery preserving nontrivial complementary pieces](#sphere-surgery-preserving-nontrivial-complementary-pieces)
  - [Three-ball](#three-ball)
  - [Poincaré conjecture](#poincare-conjecture)
  - [Loop theorem](#loop-theorem)
    - [Tower proof of the loop theorem](#tower-proof-of-the-loop-theorem)
    - [Dehn's lemma](#dehn-s-lemma)
  - [Sphere theorem for three-manifolds](#sphere-theorem-for-three-manifolds)
  - [Hyperbolic three-manifold](#hyperbolic-three-manifold)
    - [Mostow rigidity theorem](#mostow-rigidity-theorem)
  - [Three-dimensional Schoenflies theorem](#three-dimensional-schoenflies-theorem)
  - [Geometrizable three-manifold](#geometrizable-three-manifold)
    - [Geometrization conjecture](#geometrization-conjecture)
    - [Thurston geometry](#thurston-geometry)
  - [Prime three-manifold](#prime-three-manifold)
    - [Prime decomposition of a closed orientable three-manifold](#prime-decomposition-of-a-closed-orientable-three-manifold)
    - [Nonseparating sphere gives a sphere-circle summand](#nonseparating-sphere-gives-a-sphere-circle-summand)
  - [Boundary-irreducible three-manifold](#boundary-irreducible-three-manifold)
  - [Irreducible three-manifold](#irreducible-three-manifold)
  - [Excellent three-manifold](#excellent-three-manifold)
    - [Excellent knot representative theorem](#excellent-knot-representative-theorem)
  - [Thurston norm](#thurston-norm)
    - [Thurston norm of a pair-of-pants product](#thurston-norm-of-a-pair-of-pants-product)
    - [Thurston norm gluing along an incompressible torus](#thurston-norm-gluing-along-an-incompressible-torus)
    - [Dual Thurston polytope](#dual-thurston-polytope)
  - [Incompressible surface](#incompressible-surface)
    - [Three-manifold hierarchy](#three-manifold-hierarchy)
      - [Relative boundary rigidity from a hierarchy](#relative-boundary-rigidity-from-a-hierarchy)
      - [Asphericity from a three-manifold hierarchy](#asphericity-from-a-three-manifold-hierarchy)
      - [Self-reproducing incompressible annulus cut](#self-reproducing-incompressible-annulus-cut)
    - [Compression disk](#compression-disk)
    - [Boundary-parallel surface](#boundary-parallel-surface)
    - [Classification of incompressible surfaces in Seifert fibered spaces](#classification-of-incompressible-surfaces-in-seifert-fibered-spaces)
    - [Boundary-incompressible surface](#boundary-incompressible-surface)
  - [Heegaard splitting](#heegaard-splitting)
    - [Common nonseparating disks in a Heegaard splitting](#common-nonseparating-disks-in-a-heegaard-splitting)
    - [Heegaard genus](#heegaard-genus)
    - [Heegaard Floer homology](#heegaard-floer-homology)
      - [Mixed Heegaard Floer invariant](#mixed-heegaard-floer-invariant)
        - [Adjunction inequality for the mixed Heegaard Floer invariant](#adjunction-inequality-for-the-mixed-heegaard-floer-invariant)
        - [Blowup formula for the mixed Heegaard Floer invariant](#blowup-formula-for-the-mixed-heegaard-floer-invariant)
      - [Integer-surgery exact triangle in Heegaard Floer homology](#integer-surgery-exact-triangle-in-heegaard-floer-homology)
      - [Heegaard Floer cobordism map](#heegaard-floer-cobordism-map)
        - [Admissible cut for a Heegaard Floer mixed map](#admissible-cut-for-a-heegaard-floer-mixed-map)
      - [Variants of Heegaard Floer homology](#variants-of-heegaard-floer-homology)
        - [Non-torsion Heegaard Floer homology of the sphere-circle product](#non-torsion-heegaard-floer-homology-of-the-sphere-circle-product)
        - [Reduced Heegaard Floer homology](#reduced-heegaard-floer-homology)
        - [U-adic completion of Heegaard Floer homology](#u-adic-completion-of-heegaard-floer-homology)
      - [Heegaard Floer chain complex](#heegaard-floer-chain-complex)
        - [Coherent orientations in Heegaard Floer homology](#coherent-orientations-in-heegaard-floer-homology)
        - [Empty bigon and rectangle counts in Heegaard Floer homology](#empty-bigon-and-rectangle-counts-in-heegaard-floer-homology)
        - [Relative grading in Heegaard Floer homology](#relative-grading-in-heegaard-floer-homology)
          - [Absolute grading in Heegaard Floer homology](#absolute-grading-in-heegaard-floer-homology)
        - [Whitney disk class](#whitney-disk-class)
    - [Compression body](#compression-body)
    - [Heegaard surface](#heegaard-surface)
      - [Heegaard diagram](#heegaard-diagram)
        - [Generalized Heegaard diagram](#generalized-heegaard-diagram)
        - [Dehn presentation Heegaard diagram](#dehn-presentation-heegaard-diagram)
  - [Handlebody](#handlebody)
  - [Thurston elliptization conjecture](#thurston-elliptization-conjecture)
- [Homology above the dimension of a manifold](#homology-above-the-dimension-of-a-manifold)

## Topological atlas

↑ **Parent:** [Topological manifold](topological-manifold.md)

A topological atlas is a family $\mathcal A=\{(U_i,\varphi_i)\}$ of [coordinate charts](differential-geometry.md#manifold-chart) whose domains form an [open cover](topology.md#open-cover) of a [topological manifold](topological-manifold.md). Each point must belong to at least one chart domain; no individual domain needs to cover the entire [topological manifold](topological-manifold.md). On overlaps, [topological transition maps](#topological-transition-map) describe the same points in two coordinate systems.

### Topological transition map

↑ **Parent:** [Topological atlas](#topological-atlas)

For two [coordinate charts](differential-geometry.md#manifold-chart) in a [topological atlas](#topological-atlas), the topological transition map is the [homeomorphism](topology.md#homeomorphism)

$$
g_{ji}:\varphi_i(U_i\cap U_j)\longrightarrow\varphi_j(U_i\cap U_j),\qquad g_{ji}=\varphi_j\circ\varphi_i^{-1}.
$$

Both domains are [open sets](topology.md#open-set) in [Euclidean space](normed-vector-space.md#euclidean-norm). [Function composition](function.md#function-composition) gives $g_{ij}=g_{ji}^{-1}$ and $g_{ki}=g_{kj}\circ g_{ji}$ wherever all three [coordinate charts](differential-geometry.md#manifold-chart) overlap. These identities express consistency of the coordinate descriptions; imposing [smooth functions](analysis.md#smooth-function) as the coordinate changes gives a [smooth atlas](differential-geometry.md#smooth-atlas).

## Two stereographic charts on the circle

↑ **Parent:** [Topological manifold](topological-manifold.md)

Take the [circle](topology.md#circle) $S^1=\{(x,y)\in\mathbb R^2:x^2+y^2=1\}$ with its [subspace topology](topology.md#subspace-topology). Write $W=(-1,0)$ for its west point and $E=(1,0)$ for its east point. Two [coordinate charts](differential-geometry.md#manifold-chart) obtained by [stereographic projection](riemann-surfaces.md#stereographic-projection) are

$$
U=S^1\setminus\{W\},\qquad \varphi(x,y)=t=\frac{y}{1+x},\qquad V=S^1\setminus\{E\},\qquad \psi(x,y)=u=\frac{y}{1-x}.
$$

Both take values in the entire [real line](real-analysis.md#real-line). Geometrically, join $W$ to $(x,y)$ and intersect the resulting line with $x=0$: the height is $t$. Projecting from $E$ instead gives height $u$. Each projection omits its own starting point, but the other [coordinate chart](differential-geometry.md#manifold-chart) includes that point. Hence $U\cup V=S^1$.[Topology I: smooth manifolds, Week 1, Example 1.6, equations (4)–(5), page 2; specialize the sphere charts to dimension one](mathematics-bibliography.md#topology-i-smooth-manifolds-university-of-toronto-mat1300hf-2012/week-1-course-notes)

<a id="image-two-stereographic-charts-cover-the-circle-and-unfold-it-onto-two-real-lines"></a>
![](circle-stereographic-charts-unfolding.png)

**[Figure 1](#image-two-stereographic-charts-cover-the-circle-and-unfold-it-onto-two-real-lines). Two stereographic charts cover the circle and unfold it onto two real lines**.

To verify the [homeomorphisms](topology.md#homeomorphism), solve the displayed equations for $(x,y)$. The [inverse functions](function.md#inverse-function) are

$$
\varphi^{-1}(t)=\left(\frac{1-t^2}{1+t^2},\frac{2t}{1+t^2}\right),\qquad \psi^{-1}(u)=\left(\frac{u^2-1}{1+u^2},\frac{2u}{1+u^2}\right).
$$

Each formula lies on the [circle](topology.md#circle), avoids its excluded point, and is [continuous](calculus.md#continuous-function) for every real argument. Substitution into the projection formulas returns $t$ or $u$; substitution in the other direction returns $(x,y)$. Thus these are [continuous](calculus.md#continuous-function) [bijections](function.md#bijection) with [continuous](calculus.md#continuous-function) [inverse functions](function.md#inverse-function), as required for [coordinate charts](differential-geometry.md#manifold-chart). Since the [Euclidean plane](geometry-and-topology.md#euclidean-plane) is [Hausdorff](topology.md#hausdorff-space) and [second countable](topology.md#second-countable-space), the [subset](set.md#subset) $S^1$ with its [subspace topology](topology.md#subspace-topology) is too. This checks all three conditions for a [topological manifold](topological-manifold.md), rather than just drawing a smooth-looking curve.

On the overlap $U\cap V$, both $x=\pm1$ are excluded, so $y\neq0$. Using $y^2=1-x^2$, the [topological transition map](#topological-transition-map) is

$$
u=\frac{y}{1-x}=\frac{1+x}{y}=\frac1t,\qquad t\in\mathbb R\setminus\{0\}.
$$

For example, $(x,y)=(3/5,4/5)$ has $t=1/2$ and $u=2$. The two [connected components](geometry-and-topology.md#connected-component) of the overlap, the upper and lower arcs, correspond to the positive and negative parts of the punctured [real line](real-analysis.md#real-line). The values $t=0$ and $u=0$ represent $E$ and $W$, respectively, and belong to only one chart each. The reciprocal coordinate change and its [inverse function](function.md#inverse-function) are [smooth functions](analysis.md#smooth-function) away from zero, so this [topological atlas](#topological-atlas) also supplies a [smooth atlas](differential-geometry.md#smooth-atlas).

Why can neither chart be enlarged to a single [coordinate chart](differential-geometry.md#manifold-chart) on the whole [circle](topology.md#circle)? The [circle](topology.md#circle) is a [closed set](topology.md#closed-set) and a [bounded set](topological-analysis.md#bounded-set) in the [Euclidean plane](geometry-and-topology.md#euclidean-plane), hence [compact](topology.md#compact-space) by the [Heine-Borel theorem](topology.md#heine-borel-theorem). A global [coordinate chart](differential-geometry.md#manifold-chart) would give a [homeomorphism](topology.md#homeomorphism) to a nonempty [open set](topology.md#open-set) $O\subseteq\mathbb R$. Its image would be [compact](topology.md#compact-space) and therefore [closed](topology.md#closed-set) in the [real line](real-analysis.md#real-line). By [connectedness](geometry-and-topology.md#connected-space) of the [real line](real-analysis.md#real-line), this forces $O=\mathbb R$, which is not [compact](topology.md#compact-space). This is the one-dimensional instance of [no compact manifold has a single Euclidean chart](differential-geometry.md#no-compact-manifold-has-a-single-euclidean-chart). Locally the [circle](topology.md#circle) is indistinguishable from the [real line](real-analysis.md#real-line); globally [compactness](topology.md#compact-space) obstructs a single chart.

## Topological manifold with boundary

↑ **Parent:** [Topological manifold](topological-manifold.md)

For $n\geq1$, a topological $n$-manifold with boundary is a [Hausdorff](topology.md#hausdorff-space) [second-countable space](topology.md#second-countable-space) locally [homeomorphic](topology.md#homeomorphism) to relatively [open sets](topology.md#open-set) in the [half-space](geometry-and-topology.md#half-space) $\mathbb H^n$. The openness here is in the [subspace topology](topology.md#subspace-topology) of $\mathbb H^n$, not necessarily in $\mathbb R^n$. Its intrinsic boundary $\partial M$ consists of points sent to $x_n=0$; the remaining points have ordinary [coordinate charts](differential-geometry.md#manifold-chart) with images open in [Euclidean space](normed-vector-space.md#euclidean-norm). The intrinsic boundary is independent of the chosen chart.[Topology I: smooth manifolds, Week 2, Section 1.3, equation (21), Definition 1.21 and Remark 1.24, page 7](mathematics-bibliography.md#topology-i-smooth-manifolds-university-of-toronto-mat1300hf-2012/week-2-course-notes)

The [closed interval](real-analysis.md#closed-real-interval) $[0,1]$ illustrates the distinction: its interior points have [open interval](topology.md#open-interval) charts, while $0$ and $1$ have charts modeled on $[0,\varepsilon)\subseteq\mathbb H^1$, using $x$ and $1-x$. Its intrinsic boundary is $\{0,1\}$. The [circle](topology.md#circle) has empty intrinsic boundary even though its [boundary of a set](topology.md#boundary-of-a-set) as a [subset](set.md#subset) of the [Euclidean plane](geometry-and-topology.md#euclidean-plane) is the whole [circle](topology.md#circle). A [topological manifold](topological-manifold.md) without boundary is therefore a special case with $\partial M=\varnothing$, and a [smooth atlas](differential-geometry.md#smooth-atlas) on the half-space charts gives a [manifold with boundary](smooth-manifold.md#manifold-with-boundary) in the smooth sense.

## Category of topological manifolds

↑ **Parent:** [Topological manifold](topological-manifold.md)

The [category](category.md) of topological manifolds has [topological manifolds](topological-manifold.md) without boundary as its [objects of a category](category.md#object-of-a-category) and all [continuous maps](topology.md#continuous-map) between them as its [categorical morphisms](category.md#morphism-in-a-category). Allowing every [dimension of a manifold](#dimension-of-a-manifold) lets maps connect spaces of different dimensions. [Identity functions](function.md#identity-function) are [continuous](calculus.md#continuous-function), and [function composition](function.md#function-composition) preserves [continuity](calculus.md#continuous-function), so the [category](category.md) laws are inherited from [functions](function.md). Its [isomorphisms](algebra.md#isomorphism) are exactly [homeomorphisms](topology.md#homeomorphism).

In [coordinate charts](differential-geometry.md#manifold-chart) $(U,\varphi)$ on $M$ and $(V,\psi)$ on $N$, a [continuous map](topology.md#continuous-map) $f:M\to N$ is represented locally by $\psi\circ f\circ\varphi^{-1}$ on $\varphi(U\cap f^{-1}(V))$. Changing [coordinate charts](differential-geometry.md#manifold-chart) changes this expression through [topological transition maps](#topological-transition-map), while $f$ itself stays fixed. This viewpoint separates the underlying [continuous map](topology.md#continuous-map) from the coordinates used to describe it; restricting to [smooth manifolds](smooth-manifold.md) and [smooth maps](smooth-manifold.md#smooth-map-between-manifolds) gives the corresponding smooth [category](category.md).

## Piecewise linear ball

↑ **Parent:** [Topological manifold](topological-manifold.md)

A piecewise linear ball is a [simplicial complex](algebraic-topology.md#simplicial-complex) admitting a [homeomorphism](topology.md#homeomorphism) to an $n$-[simplex](algebraic-topology.md#simplex) that is linear on the [simplexes](algebraic-topology.md#simplex) of suitable finite [simplicial subdivisions](algebraic-topology.md#simplicial-subdivision). Its [boundary](topology.md#boundary-of-a-set) is a piecewise linear [sphere](euclidean-geometry.md#sphere).

### Gluing three-balls along a boundary disk

↑ **Parent:** [Piecewise linear ball](#piecewise-linear-ball)

Two [piecewise linear balls](#piecewise-linear-ball) of dimension three glued along a common [boundary](topology.md#boundary-of-a-set) [disk](topology.md#disk-mathematics) form another [piecewise linear ball](#piecewise-linear-ball). The [Schoenflies theorem](topological-surface.md#schoenflies-theorem) identifies each [boundary](topology.md#boundary-of-a-set) pair with a [sphere](euclidean-geometry.md#sphere) and a hemisphere. Coning the resulting [boundary](topology.md#boundary-of-a-set) [homeomorphisms](topology.md#homeomorphism) extends them over the balls, which then become the two halves of a standard ball. The same argument shows that removing a ball attached along one [boundary](topology.md#boundary-of-a-set) [disk](topology.md#disk-mathematics) leaves a ball.

## 4-manifold

↑ **Parent:** [Topological manifold](topological-manifold.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/4-manifold)

### Smooth four-manifold

↑ **Parent:** [4-manifold](#4-manifold)

A smooth four-manifold is a four-dimensional [smooth manifold](smooth-manifold.md). Its [intersection form](homology.md#intersection-form) and gauge-theoretic invariants impose strong constraints on its possible smooth and symplectic structures.

#### Fiber sum of four-manifolds

↑ **Parent:** [Smooth four-manifold](#smooth-four-manifold)

Remove [tubular neighborhoods](differential-geometry.md#tubular-neighborhood) of diffeomorphic embedded oriented surfaces with opposite normal Euler numbers, and glue their boundary circle bundles by a fiber-reversing identification. The resulting smooth [manifold](topological-manifold.md) is a fiber sum. The square-zero case uses trivial [normal bundles](algebraic-geometry.md#normal-bundle). Additional symplectic hypotheses give a [symplectic fiber sum along a square-zero surface](symplectic-geometry.md#symplectic-fiber-sum-along-a-square-zero-surface).

##### Smooth fiber sum along unknotted null-homologous spheres

↑ **Parent:** [Fiber sum of four-manifolds](#fiber-sum-of-four-manifolds)

For standard unknotted [spheres](euclidean-geometry.md#sphere) contained in four-balls in $X$ and $Y$, the standard fiber-reversing gluing gives the displayed [connected sum](smooth-manifold.md#connected-sum-of-oriented-manifolds). The complement of an unknotted $S^2\times D^2$ in $S^4$ is $S^1\times D^3$, and its double is $S^1\times S^3$. The portions of $X$ and $Y$ outside the four-balls remain as connected summands. Taking both ambient manifolds to be the [Complex projective plane](algebraic-topology.md#complex-projective-plane) gives a smooth fiber sum with no [symplectic form](symplectic-geometry.md#symplectic-form), by the [symplectic connected-sum obstruction](#symplectic-connected-sum-obstruction).

<h4 id="seiberg-witten-invariant-of-a-four-manifold">Seiberg–Witten invariant of a four-manifold</h4>

↑ **Parent:** [Smooth four-manifold](#smooth-four-manifold)

<h5 id="connected-sum-vanishing-of-the-seiberg-witten-invariant">Connected-sum vanishing of the Seiberg–Witten invariant</h5>

↑ **Parent:** [Seiberg–Witten invariant of a four-manifold](#seiberg-witten-invariant-of-a-four-manifold)

If a closed oriented [smooth four-manifold](#smooth-four-manifold) splits as a [connected sum](smooth-manifold.md#connected-sum-of-oriented-manifolds) $X_1\#X_2$ with both $b_2^+(X_i)>0$, its ordinary [Seiberg–Witten invariants of a four-manifold](#seiberg-witten-invariant-of-a-four-manifold) vanish. Combined with [Taubes nonvanishing theorem](#taubes-nonvanishing-theorem), this obstructs a symplectic structure in that orientation.

##### Taubes nonvanishing theorem

↑ **Parent:** [Seiberg–Witten invariant of a four-manifold](#seiberg-witten-invariant-of-a-four-manifold)

A closed [symplectic manifold](symplectic-geometry.md#symplectic-manifold) of real dimension four with $b_2^+>1$ has a nonzero [Seiberg–Witten invariant of a four-manifold](#seiberg-witten-invariant-of-a-four-manifold) in its canonical structure, with value $\pm1$. The [positive index of the intersection form](homology.md#positive-index-of-the-intersection-form) hypothesis avoids chamber dependence. This provides the [symplectic connected-sum obstruction](#symplectic-connected-sum-obstruction).

[https://intlpress.com/site/pub/files/_fulltext/journals/mrl/1994/0001/0006/MRL-1994-0001-0006-a015.pdf](https://intlpress.com/site/pub/files/_fulltext/journals/mrl/1994/0001/0006/MRL-1994-0001-0006-a015.pdf)

###### Symplectic connected-sum obstruction

↑ **Parent:** [Taubes nonvanishing theorem](#taubes-nonvanishing-theorem)

A closed [symplectic manifold](symplectic-geometry.md#symplectic-manifold) of real dimension four cannot be a [connected sum](smooth-manifold.md#connected-sum-of-oriented-manifolds) of two oriented [smooth four-manifolds](#smooth-four-manifold) each with positive [positive index of the intersection form](homology.md#positive-index-of-the-intersection-form). The total $b_2^+$ exceeds one; [Taubes nonvanishing theorem](#taubes-nonvanishing-theorem) and [connected-sum vanishing of the Seiberg–Witten invariant](#connected-sum-vanishing-of-the-seiberg-witten-invariant) would force the same invariant to be both nonzero and zero.

[https://web.ma.utexas.edu/users/perutz/SFT6/SFT6.pdf](https://web.ma.utexas.edu/users/perutz/SFT6/SFT6.pdf)

## Double of a manifold

↑ **Parent:** [Topological manifold](topological-manifold.md)

Glue two copies of a compact [manifold](topological-manifold.md) along their boundaries to form its double. A collar gives the double a smooth structure when $W$ is smooth. Folding the copies onto $W$ gives a [retraction](topology.md#retraction); in particular, inclusion of either copy is injective on [homology](homology.md). For an oriented [manifold](topological-manifold.md), use the opposite [orientation](algebraic-topology.md#orientation-of-a-simplex) on the second copy.

## Topological tripod

↑ **Parent:** [Topological manifold](topological-manifold.md)

A topological tripod is three copies of the [closed interval](real-analysis.md#closed-real-interval) $[0,1]$ with their zero endpoints identified to a single junction $o$. Equivalently, embed three line segments with distinct directions in the [Euclidean plane](geometry-and-topology.md#euclidean-plane) and use the [subspace topology](topology.md#subspace-topology). It is a [compact](topology.md#compact-space), [connected](geometry-and-topology.md#connected-space) [metric space](topological-analysis.md#metric-space), and is [Hausdorff](topology.md#hausdorff-space), [second countable](topology.md#second-countable-space), and [paracompact](topology.md#paracompact-space). Every interior arm point has a [coordinate chart](differential-geometry.md#manifold-chart) to an [open interval](topology.md#open-interval), and each outer endpoint has a half-interval chart as in a [topological manifold with boundary](#topological-manifold-with-boundary). The junction has neither kind of chart.

<a id="image-removing-the-center-of-a-small-neighborhood-leaves-two-pieces-on-a-line-or-circle-but-three-at-a-tripod-junction"></a>
![](line-circle-tripod-punctured-neighborhoods.png)

**[Figure 2](#image-removing-the-center-of-a-small-neighborhood-leaves-two-pieces-on-a-line-or-circle-but-three-at-a-tripod-junction). Removing the center of a small neighborhood leaves two pieces on a line or circle, but three at a tripod junction**.

Here is a precise local obstruction. Let $S$ be a small [open](topology.md#open-set) [neighbourhood](topology.md#neighbourhood-mathematics) of $o$ consisting of initial segments of the three arms, excluding their outer endpoints. Every [connected](geometry-and-topology.md#connected-space) [open](topology.md#open-set) [neighbourhood](topology.md#neighbourhood-mathematics) $N$ of $o$ contained in $S$ contains an initial segment on every arm, because $N$ is open at $o$. Its intersection with each arm has no gaps: if a point between $o$ and a point of $N$ were missing, cutting there would separate the part beyond it from the rest of $N$, contradicting [connectedness](geometry-and-topology.md#connected-space). Thus $N\setminus\{o\}$ has exactly three [connected components](geometry-and-topology.md#connected-component), one [interval](real-analysis.md#interval-mathematics) per arm.

Suppose a [coordinate chart](differential-geometry.md#manifold-chart) $h$ to the [real line](real-analysis.md#real-line) existed at $o$. Choose a small [open interval](topology.md#open-interval) $I$ about $h(o)$ lying inside $h(S\cap\operatorname{domain}(h))$, and restrict the chart to $N=h^{-1}(I)$. This is a [connected](geometry-and-topology.md#connected-space) [open](topology.md#open-set) [neighbourhood](topology.md#neighbourhood-mathematics) of $o$ contained in $S$. Removing $o$ leaves three [connected components](geometry-and-topology.md#connected-component) in $N$, while removing $h(o)$ leaves two in $I$. A [homeomorphism](topology.md#homeomorphism) preserves [connected components](geometry-and-topology.md#connected-component), so this is impossible. This restriction step is essential: the count is proved for any sufficiently small connected chart neighborhood, not merely one chosen drawing.

A higher [dimension of a manifold](#dimension-of-a-manifold) cannot repair the junction. For $n\geq2$, repeat the argument with an [open ball](topology.md#open-ball) about $h(o)$: a punctured [open ball](topology.md#open-ball) in $\mathbb R^n$ is [path-connected](geometry-and-topology.md#path-connected-space), whereas $N\setminus\{o\}$ still has three [connected components](geometry-and-topology.md#connected-component). A zero-dimensional chart would make $o$ an [isolated point](topological-analysis.md#isolated-point), which it is not. A chart at a boundary point of a [topological manifold with boundary](#topological-manifold-with-boundary) similarly gives a punctured relative half-ball: one [connected component](geometry-and-topology.md#connected-component) when $n=1$, and a [path-connected](geometry-and-topology.md#path-connected-space) space when $n\geq2$. Consequently the [topological tripod](#topological-tripod) fails the local definition even when intrinsic boundary is allowed.

The [circle](topology.md#circle) provides a useful warning about scale: deleting a point from the whole [circle](topology.md#circle) leaves a [connected space](geometry-and-topology.md#connected-space), but deleting it from a sufficiently small connected arc leaves two [connected components](geometry-and-topology.md#connected-component). Local chart tests use the latter. The [circle and interval are not homeomorphic](topology.md#circle-and-interval-are-not-homeomorphic) article uses deletion from the whole spaces for a different, global obstruction.

## Invariance of domain

↑ **Parent:** [Topological manifold](topological-manifold.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Invariance_of_domain)

[Invariance of domain](#invariance-of-domain) says that a [continuous map](topology.md#continuous-map) that is an [injective function](algebra.md#injective-function) between [topological manifolds](topological-manifold.md) without boundary of the same dimension is an [open map](multivariable-calculus.md#open-map). It is useful in the [Penrose singularity theorem](general-relativity.md#penrose-singularity-theorem): projecting a [compact](topology.md#compact-space) [achronal boundary](general-relativity.md#achronal-boundary) along timelike curves onto a [Cauchy hypersurface](general-relativity.md#cauchy-surface) gives a nonempty subset that is both [open](topology.md#open-set) and [closed](topology.md#closed-set), forcing that [connected](geometry-and-topology.md#connected-space) [Cauchy hypersurface](general-relativity.md#cauchy-surface) to be [compact](topology.md#compact-space).

## Lorentzian manifold

↑ **Parent:** [Topological manifold](topological-manifold.md)

A smooth [manifold](topological-manifold.md) carrying a [nondegenerate bilinear form](bilinear-form.md#nondegenerate-bilinear-form) on each [tangent space](tangent-vector.md#tangent-space), with one negative and all remaining positive [eigenvalues](linear-operator-theory.md#eigenvalue), or the overall reversed-sign convention. Its nonzero [null vectors](special-relativity.md#null-vector) have vanishing metric [quadratic form](quadratic-form.md).

### Metric signature

↑ **Parent:** [Lorentzian manifold](#lorentzian-manifold)

The [metric signature](#metric-signature) records the signs of the diagonalized nondegenerate [metric tensor](general-relativity.md#metric-tensor), equivalently its numbers of negative and positive directions. For a four-dimensional [Lorentzian manifold](#lorentzian-manifold), both $(-,+,+,+)$ and its overall negative convention are common. The numerical signs of contractions and component [Hodge star operator](differential-form.md#hodge-star-operator) identities must be consistent with that choice and the [orientation](algebraic-topology.md#orientation-of-a-simplex).

### Spacelike submanifold

↑ **Parent:** [Lorentzian manifold](#lorentzian-manifold)

In [metric signature](#metric-signature) $(-,+,\ldots,+)$, a [spacelike submanifold](#spacelike-submanifold) of a [Lorentzian manifold](#lorentzian-manifold) has an induced [metric tensor](general-relativity.md#metric-tensor) defining a [positive-definite quadratic form](quadratic-form.md#positive-definite-quadratic-form). With the overall reversed [metric signature](#metric-signature), its induced [metric tensor](general-relativity.md#metric-tensor) instead has only negative [eigenvalues](linear-operator-theory.md#eigenvalue). The definition applies to any dimension: enclosing charge-integration surfaces in four dimensions are two-dimensional examples, whereas a spacelike [Cauchy hypersurface](general-relativity.md#cauchy-surface) in four dimensions is three-dimensional.

## Dimension of a manifold

↑ **Parent:** [Topological manifold](topological-manifold.md)

A [topological manifold](topological-manifold.md) has dimension $n$ when its [manifold charts](differential-geometry.md#manifold-chart) have coordinate domains open in $\mathbb R^n$. For a [smooth manifold](smooth-manifold.md), each [tangent space](tangent-vector.md#tangent-space) has [dimension](vector-space.md#dimension-vector-space) $n$, and a [tangent bundle](vector-bundle.md#tangent-bundle) has [vector bundle rank](vector-bundle.md#rank-of-a-vector-bundle) $n$.

### Codimension of a submanifold

↑ **Parent:** [Dimension of a manifold](#dimension-of-a-manifold)

The codimension is the difference between the [dimension of a manifold](#dimension-of-a-manifold) and that of its submanifold. For [complex submanifolds](complex-geometry.md#complex-submanifold), complex codimension one means real codimension two.

## Handle attachment

↑ **Parent:** [Topological manifold](topological-manifold.md)

Attaching an index-$k$ handle to an $n$-dimensional [manifold with boundary](smooth-manifold.md#manifold-with-boundary) glues $D^k\times D^{n-k}$ along $\partial D^k\times D^{n-k}$. The complementary $D^k\times\partial D^{n-k}$ replaces the attaching region in the boundary.

### Four-handle

↑ **Parent:** [Handle attachment](#handle-attachment)

A four-handle is an index-four [handle](#handle). In a four-dimensional [handle decomposition](#handle-decomposition) it is a four-ball attached along its whole boundary, a [three-sphere](euclidean-geometry.md#three-sphere). It caps a spherical boundary component left by earlier [handle attachments](#handle-attachment).

### Handle

↑ **Parent:** [Handle attachment](#handle-attachment)

An index-$\lambda$ [handle](#handle) in dimension $d$ is this product of [disks](topology.md#disk-mathematics), attached along $S^{\lambda-1}\times D^{d-\lambda}$. Its [core disk](#core-disk-of-a-handle) is $D^\lambda\times\{0\}$, and its [belt sphere](#belt-sphere) is $\{0\}\times S^{d-\lambda-1}$. The complementary boundary piece is $D^\lambda\times S^{d-\lambda-1}$. Crossing a [critical point](analysis.md#critical-point) in the [Morse handle-attachment theorem](differential-geometry.md#morse-handle-attachment-theorem) produces precisely this local change.

### Surgery on a smooth manifold

↑ **Parent:** [Handle attachment](#handle-attachment)

A framed embedding of the left-hand region in an $m$-dimensional [manifold](topological-manifold.md) specifies an index-$\lambda$ surgery. Remove its interior and glue the right-hand region along their common boundary $S^{\lambda-1}\times S^{m-\lambda}$. The [cobordism](geometry-and-topology.md#cobordism) realizing this change attaches an index-$\lambda$ [handle](#handle) of dimension $m+1$. On an oriented [surface](topological-surface.md), index-two surgery cuts out an annular neighbourhood of a simple closed curve and caps its two boundary circles.

### Zero-handle

↑ **Parent:** [Handle attachment](#handle-attachment)

A zero-handle in an $n$-dimensional [handle decomposition](#handle-decomposition) is $D^0\times D^n=D^n$. Its attaching region is empty, so it starts a connected component of the manifold. In dimension four it is a four-ball; adding [one-handles](#one-handle) and [two-handles](#two-handle) gives a four-dimensional handlebody with a two-dimensional CW spine.

### Core disk of a handle

↑ **Parent:** [Handle attachment](#handle-attachment)

The core disk of a $k$-[handle attachment](#handle-attachment) $D^k\times D^{n-k}$ is $D^k\times\{0\}$. Together with its cap in the preceding stage, it often represents a [homology class](homology.md#homology-class); for a [surgery trace](knot-theory.md#surgery-trace), capped two-handle cores give the basis of its [surgery linking matrix](knot-theory.md#surgery-linking-matrix).

### Handle decomposition

↑ **Parent:** [Handle attachment](#handle-attachment)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Handle_decomposition)

A handle decomposition builds an $n$-dimensional [manifold](topological-manifold.md) by successively adjoining $D^h\times D^{n-h}$ along $S^{h-1}\times D^{n-h}$. The attaching data comprise an [attaching sphere](#attaching-sphere) and its [framing of an embedded sphere](algebraic-geometry.md#framing-of-an-embedded-sphere). Reading a decomposition backwards replaces index $h$ by index $n-h$ and interchanges its [attaching spheres](#attaching-sphere) and [belt spheres](#belt-sphere).

#### Critical level handle embedding

↑ **Parent:** [Handle decomposition](#handle-decomposition)

In a critical level [handle](#handle) embedding, the [handles](#handle) occur at distinct heights in an ambient product with the real line. Between consecutive heights, the [boundary](topology.md#boundary-of-a-set) of the already attached [handles](#handle) travels through a product [collar neighbourhood](smooth-manifold.md#collar-neighbourhood). At a [handle](#handle) height the horizontal slice contains the [handle](#handle), attached to the incoming [boundary](topology.md#boundary-of-a-set) along its attaching region. This separates the local topology changes from the intervening product regions.

#### Zero-framed Hopf-link handle decomposition of the sphere product

↑ **Parent:** [Handle decomposition](#handle-decomposition)

Write each [sphere](euclidean-geometry.md#sphere) as two [disks](topology.md#disk-mathematics), $S^2=D_-^2\cup D_+^2$. In their product, $D_-^2\times D_-^2$ is a [zero-handle](#zero-handle); $D_+^2\times D_-^2$ and $D_-^2\times D_+^2$ are [two-handles](#two-handle). Their attaching circles are the core circles of the complementary solid tori in $\partial(D^2\times D^2)$, hence a [Hopf link](knot-theory.md#hopf-link). Constant normal directions from the disk factors give both components the zero [Seifert framing](knot-theory.md#seifert-framing). The remaining $D_+^2\times D_+^2$ is a four-handle. This product construction establishes the actual [diffeomorphism](geometry-and-topology.md#diffeomorphism) type, rather than relying on its [intersection form](homology.md#intersection-form) alone. The resulting intersection matrix is $\left(\begin{smallmatrix}0&1\\1&0\end{smallmatrix}\right)$.

#### Commutator handlebody of the torus

↑ **Parent:** [Handle decomposition](#handle-decomposition)

Attach two [one-handles](#one-handle) to a four-dimensional [zero-handle](#zero-handle), then a [two-handle](#two-handle) along the commutator of their generators with the product zero framing. The result is $T^2\times D^2$. Its spine is the usual cell structure of the [torus](topological-surface.md#torus): one vertex, two one-cells, and a two-cell attached by $xyx^{-1}y^{-1}$. An embedded representative of its $H_2$ generator is obtained by taking a once-punctured torus carried by the two one-handles and capping its boundary by the core disk of the two-handle. It meets the relative co-core once and has self-intersection zero. The boundary is $T^3$, whose integral homology has ranks $1,3,3,1$.

#### Handle slide

↑ **Parent:** [Handle decomposition](#handle-decomposition)

A handle slide replaces the framed [attaching sphere](#attaching-sphere) of one handle by a [band sum](smooth-manifold.md#band-sum) with a parallel copy of another handle of the same index. It changes the attaching data while preserving the diffeomorphism type of the resulting [manifold](topological-manifold.md). On the handle incidence matrix it performs an elementary row operation, or a column operation when applied to the dual decomposition.

##### Handle-slide isolation of a cancelling pair

↑ **Parent:** [Handle slide](#handle-slide)

In the intermediate-index range, if an [attaching sphere](#attaching-sphere) $A_1$ meets a [belt sphere](#belt-sphere) $B_1$ at exactly one transverse point, [handle slides](#handle-slide) can remove the intersections of every other attaching sphere with $B_1$. The dual slides then remove the intersections of $A_1$ with the other belt spheres. Each move uses a band to the unique pivot sheet and a local isotopy removing the old and new intersections. If $m_{ji}=A_j\cdot B_i$ and $\delta=m_{11}=\pm1$, the remaining incidence block is $m_{ji}-m_{j1}m_{1i}/\delta$, the [Schur complement](linear-algebra.md#schur-complement) of the pivot. Extreme-index cases need separate hypotheses.

#### Belt sphere

↑ **Parent:** [Handle decomposition](#handle-decomposition)

The belt sphere of an index-$h$ handle is $\{0\}\times S^{n-h-1}$ in the boundary after attachment. It is the [attaching sphere](#attaching-sphere) of the dual index-$(n-h)$ handle. Its intersections with the [attaching spheres](#attaching-sphere) of later handles detect passages through this handle.

#### Attaching sphere

↑ **Parent:** [Handle decomposition](#handle-decomposition)

The attaching sphere of an index-$h$ handle $D^h\times D^{n-h}$ is $S^{h-1}\times\{0\}$ in the previous boundary. Its [framing of an embedded sphere](algebraic-geometry.md#framing-of-an-embedded-sphere) identifies a neighbourhood with $S^{h-1}\times D^{n-h}$ and specifies the [handle attachment](#handle-attachment).

### Three-handle

↑ **Parent:** [Handle attachment](#handle-attachment)

### Two-handle

↑ **Parent:** [Handle attachment](#handle-attachment)

### One-handle

↑ **Parent:** [Handle attachment](#handle-attachment)

## 3-manifold

↑ **Parent:** [Topological manifold](topological-manifold.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/3-manifold)

A three-manifold is a [topological manifold](topological-manifold.md) locally modeled on $\mathbb R^3$, or on a half-space at its boundary.

### Normal surface

↑ **Parent:** [3-manifold](#3-manifold)

Relative to a [triangulation](algebraic-topology.md#triangulation), a [normal surface](#normal-surface) meets every [tetrahedron](euclidean-geometry.md#tetrahedron) in disjoint normal [disks](topology.md#disk-mathematics): four types of triangles cutting off vertices and three types of quadrilaterals separating opposite pairs of edges. A normal [disk](topology.md#disk-mathematics) meets any edge at most once; its face arcs join distinct edges. Two different quadrilateral types cannot coexist in a [tetrahedron](euclidean-geometry.md#tetrahedron).

#### Normal surface coordinates

↑ **Parent:** [Normal surface](#normal-surface)

For $t$ [tetrahedra](euclidean-geometry.md#tetrahedron), count the seven [disk](topology.md#disk-mathematics) types in each [tetrahedron](euclidean-geometry.md#tetrahedron). Across each glued face the counts of each of its three normal arc types must agree. These are homogeneous [linear equations](linear-algebra.md#linear-equation) with integer coefficients. An admissible solution also has at most one nonzero quadrilateral type in each [tetrahedron](euclidean-geometry.md#tetrahedron). Matching the arcs in their [boundary](topology.md#boundary-of-a-set) order reconstructs the [normal surface](#normal-surface) up to an [isotopy](smooth-manifold.md#isotopy) preserving the [tetrahedra](euclidean-geometry.md#tetrahedron).

##### Normal surface weight

↑ **Parent:** [Normal surface coordinates](#normal-surface-coordinates)

The weight of a [normal surface](#normal-surface) counts its intersections with the edges of the [triangulation](algebraic-topology.md#triangulation). It is a positive linear function of its coordinates: each corner of a normal [disk](topology.md#disk-mathematics) contributes the reciprocal of the number of tetrahedral sectors around its edge. Thus a nontrivial decomposition into compatible coordinate vectors gives both summands strictly smaller weight.

##### Haken sum

↑ **Parent:** [Normal surface coordinates](#normal-surface-coordinates)

The Haken sum of compatible [normal surfaces](#normal-surface) is obtained by resolving their intersection curves in the way that preserves the normal [disk](topology.md#disk-mathematics) types. It adds [normal surface coordinates](#normal-surface-coordinates), [Euler characteristic](homology.md#euler-characteristic) and mod-two [homology](homology.md) classes. The alternative local resolution can create returning face arcs and need not be normal.

##### Fundamental normal surface

↑ **Parent:** [Normal surface coordinates](#normal-surface-coordinates)

A fundamental [normal surface](#normal-surface) has a nonzero admissible coordinate vector which is not the sum of two nonzero admissible vectors. Fixing the allowed quadrilateral type in every [tetrahedron](euclidean-geometry.md#tetrahedron) reduces the problem to the [Hilbert basis of a rational cone](toric-geometry.md#hilbert-basis-of-a-rational-cone). There are finitely many choices of quadrilateral types and finitely many indecomposable vectors for each choice.

### Punctured three-sphere

↑ **Parent:** [3-manifold](#3-manifold)

A punctured three-sphere is $S^3$ with the interiors of finitely many disjoint [piecewise linear balls](#piecewise-linear-ball) removed. Capping its spherical [boundary](topology.md#boundary-of-a-set) components with balls restores $S^3$. Removing another ball or gluing two such manifolds along one spherical [boundary](topology.md#boundary-of-a-set) component preserves this class.

#### Sphere surgery preserving nontrivial complementary pieces

↑ **Parent:** [Punctured three-sphere](#punctured-three-sphere)

Suppose disjoint separating [spheres](euclidean-geometry.md#sphere) cut a [3-manifold](#3-manifold) into pieces none of which is a [punctured three-sphere](#punctured-three-sphere). Compress one [sphere](euclidean-geometry.md#sphere) along a [disk](topology.md#disk-mathematics) disjoint from the others. The old [sphere](euclidean-geometry.md#sphere) and the two new [spheres](euclidean-geometry.md#sphere) enclose a three-times punctured [sphere](euclidean-geometry.md#sphere). At least one of the two pieces on the compressed side is not a punctured [sphere](euclidean-geometry.md#sphere); retain that new [sphere](euclidean-geometry.md#sphere) and discard the other. The piece on its opposite side cannot become a punctured [sphere](euclidean-geometry.md#sphere), since capping its boundaries and applying the [Three-dimensional Schoenflies theorem](#three-dimensional-schoenflies-theorem) would make the original opposite piece a punctured [sphere](euclidean-geometry.md#sphere) as well. Hence the number of [spheres](euclidean-geometry.md#sphere) and the nontriviality condition can be preserved.

### Three-ball

↑ **Parent:** [3-manifold](#3-manifold)

A three-ball is a [three-manifold](#3-manifold) [homeomorphic](topology.md#homeomorphism) to the closed unit [ball](topological-analysis.md#ball-mathematics) in $\mathbb R^3$. Its [boundary](topology.md#boundary-of-a-set) is a [two-sphere](euclidean-geometry.md#two-sphere). Attaching a three-ball to a spherical boundary component is called capping that boundary; marked endpoints may be joined by a straight arc inside the cap.

<h3 id="poincare-conjecture">Poincaré conjecture</h3>

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincaré_conjecture)

A closed [simply connected](algebraic-topology.md#simply-connected-space) [three-manifold](#3-manifold) is homeomorphic to the [three-sphere](euclidean-geometry.md#three-sphere). Now a theorem, this identifies every [homotopy](homotopy.md) [three-sphere](euclidean-geometry.md#three-sphere) with the standard sphere and removes homotopy-sphere ambiguities in three-dimensional connected-sum classification. Smooth structures are also unique in dimension three.

### Loop theorem

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loop_theorem)

If a boundary surface inclusion has noninjective [fundamental group](algebraic-topology.md#fundamental-group) map, there is a [compression disk](#compression-disk) whose boundary represents a nontrivial element of that kernel. More generally the boundary can be required to avoid a prescribed normal subgroup if a singular disk with that property exists.

#### Tower proof of the loop theorem

↑ **Parent:** [Loop theorem](#loop-theorem)

Start with a singular [disk](topology.md#disk-mathematics) whose [boundary](topology.md#boundary-of-a-set) represents a prescribed nontrivial class in a [boundary](topology.md#boundary-of-a-set) subsurface. Repeatedly lift it through double [covering spaces](algebraic-topology.md#covering-space) of regular neighbourhoods of its image. The number of distinct image [simplexes](algebraic-topology.md#simplex) strictly increases and is bounded by the number of domain [simplexes](algebraic-topology.md#simplex), so the tower ends. At the top, vanishing first mod-two [homology](homology.md) forces every [boundary](topology.md#boundary-of-a-set) component to be a [sphere](euclidean-geometry.md#sphere). An embedded [disk](topology.md#disk-mathematics) can then be constructed and projected down the tower. Resolving double curves preserves a [boundary](topology.md#boundary-of-a-set) class outside a chosen [normal subgroup](group-theory.md#normal-subgroup), giving an embedded compression [disk](topology.md#disk-mathematics) at the bottom.

<h4 id="dehn-s-lemma">Dehn's lemma</h4>

↑ **Parent:** [Loop theorem](#loop-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dehn's_lemma)

A simple closed curve on the boundary of a [three-manifold](#3-manifold) which is nullhomotopic in the manifold bounds a properly embedded disk. The boundary curve is retained; the [Loop theorem](#loop-theorem) can instead find a different simple essential curve in a nontrivial kernel.

### Sphere theorem for three-manifolds

↑ **Parent:** [3-manifold](#3-manifold)

If an orientable [three-manifold](#3-manifold) has nonzero $\pi_2$, it contains an embedded essential two-sphere. Consequently a closed orientable [irreducible three-manifold](#irreducible-three-manifold) with infinite fundamental group is [aspherical](homotopy.md#aspherical-space): its simply connected noncompact universal cover has zero second homotopy and top ordinary homology, hence is acyclic and contractible by the [Hurewicz theorem](homotopy.md#hurewicz-theorem) and [Whitehead theorem](homotopy.md#whitehead-theorem).

### Hyperbolic three-manifold

↑ **Parent:** [3-manifold](#3-manifold)

A complete hyperbolic three-manifold is a complete [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) of dimension three with constant [sectional curvature](second-fundamental-form.md#sectional-curvature) $-1$. Its [universal cover](algebraic-topology.md#universal-cover) is [hyperbolic space](hyperbolic-geometry.md#hyperbolic-space) $\mathbb H^3$ and its deck group acts freely and discretely by [Riemannian isometries](differential-geometry.md#riemannian-isometry). In the orientable case it is a torsion-free [Kleinian group](topological-group.md#kleinian-group).

#### Mostow rigidity theorem

↑ **Parent:** [Hyperbolic three-manifold](#hyperbolic-three-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mostow_rigidity_theorem)

For complete finite-volume [hyperbolic space](hyperbolic-geometry.md#hyperbolic-space) manifolds of dimension at least three, an isomorphism of [fundamental groups](algebraic-topology.md#fundamental-group) is induced, up to the usual basepoint-path choice, by a unique hyperbolic [isometry](riemannian-geometry.md#isometry). The finite-volume noncompact case includes the Prasad extension. Thus complete hyperbolic metrics on a fixed finite-volume three-manifold have no deformation moduli, unlike metrics on closed hyperbolic surfaces.

### Three-dimensional Schoenflies theorem

↑ **Parent:** [3-manifold](#3-manifold)

A smooth, piecewise-linear or locally flat embedded two-sphere in the [three-sphere](euclidean-geometry.md#three-sphere) has two complementary components, each with closure homeomorphic to a three-ball. Equivalently a tame embedded two-sphere in $\mathbb R^3$ bounds a ball on its compact side. Local flatness is essential; arbitrary wild sphere embeddings are excluded.

### Geometrizable three-manifold

↑ **Parent:** [3-manifold](#3-manifold)

A closed orientable [three-manifold](#3-manifold) is geometrizable if its prime summands can be split along finitely many disjoint essential [tori](topological-surface.md#torus) into pieces whose interiors carry complete geometric structures modeled on the eight [Thurston geometries](#thurston-geometry). Prime decomposition and capping sphere boundaries precede the torus cuts; a single homogeneous geometry on the original connected sum is not required.

#### Geometrization conjecture

↑ **Parent:** [Geometrizable three-manifold](#geometrizable-three-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometrization_conjecture)

Every closed orientable [three-manifold](#3-manifold) admits a prime and [torus](topological-surface.md#torus) decomposition into pieces modeled on the eight [Thurston geometries](#thurston-geometry). In particular, a closed irreducible orientable [three-manifold](#3-manifold) with [fundamental group](algebraic-topology.md#fundamental-group) $\mathbb Z^3$ carries a flat metric. The [Bieberbach theorem](second-fundamental-form.md#bieberbach-theorem) then identifies it with the three-torus because an abelian crystallographic group has trivial linear holonomy. [Simply connected](algebraic-topology.md#simply-connected-space) closed [three-manifolds](#3-manifold) are three-spheres by the [Poincaré conjecture](#poincare-conjecture).

#### Thurston geometry

↑ **Parent:** [Geometrizable three-manifold](#geometrizable-three-manifold)

The eight simply connected three-dimensional homogeneous model geometries are $S^3$, $\mathbb R^3$, $\mathbb H^3$, $S^2\times\mathbb R$, $\mathbb H^2\times\mathbb R$, $\widetilde{\operatorname{SL}}_2(\mathbb R)$, $\mathrm{Nil}$ and $\mathrm{Sol}$. A geometric structure is a locally homogeneous structure obtained as a quotient of a model by a discrete freely acting isometry group, equivalently with compatible model charts.

### Prime three-manifold

↑ **Parent:** [3-manifold](#3-manifold)

A closed connected [orientable smooth manifold](smooth-manifold.md#orientable-smooth-manifold) of dimension three is prime when a decomposition as a [connected sum](smooth-manifold.md#connected-sum-of-oriented-manifolds) forces at least one summand to be the [three-sphere](euclidean-geometry.md#three-sphere). Unlike an [irreducible three-manifold](#irreducible-three-manifold), it may contain a nonseparating embedded two-sphere.

#### Prime decomposition of a closed orientable three-manifold

↑ **Parent:** [Prime three-manifold](#prime-three-manifold)

Every closed connected orientable [three-manifold](#3-manifold) is a finite [connected sum](smooth-manifold.md#connected-sum-of-oriented-manifolds) of [prime three-manifolds](#prime-three-manifold), unique up to order and the insertion of three-sphere factors. The corresponding [fundamental group](algebraic-topology.md#fundamental-group) is the free product of the summand groups. A prime orientable three-manifold is either irreducible or $S^2\times S^1$; this separates aspherical infinite-group cases from the infinite cyclic case.

#### Nonseparating sphere gives a sphere-circle summand

↑ **Parent:** [Prime three-manifold](#prime-three-manifold)

In an orientable [three-manifold](#3-manifold), an embedded nonseparating two-sphere has a product neighborhood. Join its two boundary spheres by an arc outside that neighborhood and take a regular neighborhood of the union. This region is $S^2\times S^1$ with an open ball removed. Its boundary sphere exhibits the displayed [connected sum](smooth-manifold.md#connected-sum-of-oriented-manifolds). Consequently a prime but nonirreducible orientable [three-manifold](#3-manifold) is $S^2\times S^1$.

### Boundary-irreducible three-manifold

↑ **Parent:** [3-manifold](#3-manifold)

A compact [three-manifold](#3-manifold) is boundary-irreducible when there is no embedded disk with interior in the manifold and boundary an essential curve in its boundary. Thus its boundary has no compressing disk.

### Irreducible three-manifold

↑ **Parent:** [3-manifold](#3-manifold)

An orientable [three-manifold](#3-manifold) is irreducible if every embedded two-sphere bounds a three-ball. This makes innermost-disk simplifications of embedded [topological surfaces](topological-surface.md) possible without changing the ambient [three-manifold](#3-manifold).

### Excellent three-manifold

↑ **Parent:** [3-manifold](#3-manifold)

In the orientable case an excellent compact three-manifold is an [irreducible three-manifold](#irreducible-three-manifold) and a [boundary-irreducible three-manifold](#boundary-irreducible-three-manifold), is not a ball, contains a two-sided properly embedded [incompressible surface](#incompressible-surface), and has every properly embedded incompressible zero-[Euler characteristic](homology.md#euler-characteristic) surface a [boundary-parallel surface](#boundary-parallel-surface). In particular it has no essential [annulus](topology.md#annulus-mathematics) or [torus](topological-surface.md#torus). These properties give lower bounds on the [Thurston norm](#thurston-norm) of classes with essential boundary.

#### Excellent knot representative theorem

↑ **Parent:** [Excellent three-manifold](#excellent-three-manifold)

In a compact connected orientable [three-manifold](#3-manifold) with no spherical boundary components, every embedded [knot](knot-theory.md#knot) is homotopic to a [knot](knot-theory.md#knot) with an [excellent three-manifold](#excellent-three-manifold) as exterior. In particular this can preserve the generator class in $S^1\times S^2$, or the [winding number of a satellite pattern](knot-theory.md#winding-number-of-a-satellite-pattern) one class in a [solid torus](topological-surface.md#solid-torus). Homotopy here is weaker than [isotopy](smooth-manifold.md#isotopy).

### Thurston norm

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thurston_norm)

For a compact oriented [three-manifold](#3-manifold), the integral relative class $u$ has norm the minimum of $\chi_-(F)=\sum_j\max(0,-\chi(F_j))$ over properly embedded oriented [topological surfaces](topological-surface.md) representing $u$. Homogeneity and continuity extend it to real [relative homology](homology.md#relative-homology). It is a [seminorm](topological-vector-space.md#seminorm), since spheres, disks, [annuli](topology.md#annulus-mathematics) and [tori](topological-surface.md#torus) have zero cost.

#### Thurston norm of a pair-of-pants product

↑ **Parent:** [Thurston norm](#thurston-norm)

For $Y=P\times S^1$ with $P$ a [pair of pants](topological-surface.md#pair-of-pants-mathematics) and $h$ its circle fiber, a [horizontal surface in a Seifert fibered space](knot-theory.md#horizontal-surface-in-a-seifert-fibered-space) of degree $d$ has $\chi_- = |d|$; [vertical surfaces in a Seifert fibered space](knot-theory.md#vertical-surface-in-a-seifert-fibered-space) have zero cost. Cutting and pasting these representatives, and classifying essential surfaces, proves $\|u\|_T=|u\cdot h|$. The [dual Thurston polytope](#dual-thurston-polytope) is therefore the segment between the two functionals $\pm h$ under the natural pairing.

#### Thurston norm gluing along an incompressible torus

↑ **Parent:** [Thurston norm](#thurston-norm)

In an irreducible [three-manifold](#3-manifold) with incompressible boundary, a minimizing surface can be cut along a separating incompressible [torus](topological-surface.md#torus) after removing inessential intersection circles. The essential pieces have no disk or sphere components, so their $\chi_-$ costs add. Minimizing independently in the pieces and gluing their matching boundary curves gives the corresponding upper bound. This allows [Thurston norm](#thurston-norm) calculations for [satellite knots](knot-theory.md#satellite-knot).

#### Dual Thurston polytope

↑ **Parent:** [Thurston norm](#thurston-norm)

The dual polytope consists of the real linear functionals $\alpha$ on $H_2(Y,\partial Y;\mathbb R)$ such that $|\alpha(u)|\leq\|u\|_T$ for every $u$. Thus it is the polar of the unit ball of the [Thurston norm](#thurston-norm) and annihilates that [seminorm](topological-vector-space.md#seminorm)'s kernel.

### Incompressible surface

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Incompressible_surface)

An incompressible surface is a properly embedded two-sided [topological surface](topological-surface.md) with no compressing disk, subject to the usual exclusion of inessential spherical components. A compressing disk has boundary an essential closed curve on the [topological surface](topological-surface.md) and interior disjoint from it.

#### Three-manifold hierarchy

↑ **Parent:** [Incompressible surface](#incompressible-surface)

A hierarchy is a finite sequence of cuts along properly embedded two-sided [incompressible surfaces](#incompressible-surface), without spherical components, ending in disjoint three-balls. [Disks](topology.md#disk-mathematics) are allowed. For an ambient manifold which is not [orientable](differential-geometry.md#orientable-surface) the two-sided cutting [surfaces](topological-surface.md) need not themselves be [orientable](differential-geometry.md#orientable-surface). The existence of a hierarchy does not imply that every choice of incompressible cuts terminates.

##### Relative boundary rigidity from a hierarchy

↑ **Parent:** [Three-manifold hierarchy](#three-manifold-hierarchy)

A map between [compact](topology.md#compact-space) [connected](geometry-and-topology.md#connected-space) [orientable](differential-geometry.md#orientable-surface) irreducible [3-manifolds](#3-manifold) with nonempty boundaries, [injective](algebra.md#injective-function) on the [boundary](topology.md#boundary-of-a-set) and on the [fundamental group](algebraic-topology.md#fundamental-group), is [homotopic](homotopy.md) to a [homeomorphism](topology.md#homeomorphism) relative to the [boundary](topology.md#boundary-of-a-set). The [boundary](topology.md#boundary-of-a-set) determines degree $\pm1$, and the cover corresponding to the image of the [fundamental group](algebraic-topology.md#fundamental-group) consequently has one sheet. Straighten the preimage of an incompressible hierarchy [surface](topological-surface.md), cut both manifolds, and repeat. At the terminal balls, extend the prescribed [boundary](topology.md#boundary-of-a-set) [homeomorphisms](topology.md#homeomorphism) by coning. The [homotopies](homotopy.md) and [homeomorphisms](topology.md#homeomorphism) glue across the straightened [surface](topological-surface.md) collars.

##### Asphericity from a three-manifold hierarchy

↑ **Parent:** [Three-manifold hierarchy](#three-manifold-hierarchy)

In an [orientable](differential-geometry.md#orientable-surface) [irreducible three-manifold](#irreducible-three-manifold), an incompressible cut is [fundamental group](algebraic-topology.md#fundamental-group)-injective by the [Loop theorem](#loop-theorem). Lift a [three-manifold hierarchy](#three-manifold-hierarchy) to the [universal cover](algebraic-topology.md#universal-cover). The terminal ball pieces are [contractible](homotopy.md#contractible-space) and their gluing [surfaces](topological-surface.md) have [contractible](homotopy.md#contractible-space) universal covers. The incidence graph is a tree, by the [van Kampen theorem](algebraic-topology.md#seifert-van-kampen-theorem) normal form for successive cuts. Finite subtrees are [contractible](homotopy.md#contractible-space) by successively attaching a terminal piece along a [contractible](homotopy.md#contractible-space) intersection. Every [sphere](euclidean-geometry.md#sphere) map has [compact](topology.md#compact-space) image contained in a finite subtree, so all higher [homotopy groups](homotopy.md#homotopy-group) of the [universal cover](algebraic-topology.md#universal-cover) vanish.

##### Self-reproducing incompressible annulus cut

↑ **Parent:** [Three-manifold hierarchy](#three-manifold-hierarchy)

Let $P$ be a once-punctured [torus](topological-surface.md#torus) and let $c$ be a nonseparating essential curve. The [annulus](topology.md#annulus-mathematics) $c\times[0,1]$ is an [incompressible surface](#incompressible-surface) in $P\times[0,1]$. Cutting gives a [pair of pants](topological-surface.md#pair-of-pants-mathematics) times an interval. Both products are genus-two [handlebodies](#handlebody), since a [compact](topology.md#compact-space) [connected](geometry-and-topology.md#connected-space) [surface](topological-surface.md) with [boundary](topology.md#boundary-of-a-set) times an interval is a handlebody of [genus](topological-surface.md#genus-of-a-surface) $1-\chi(P)$.

#### Compression disk

↑ **Parent:** [Incompressible surface](#incompressible-surface)

A compression disk for a two-sided embedded [surface](topological-surface.md) $F$ in a [three-manifold](#3-manifold) is an embedded disk meeting $F$ exactly in its boundary, with boundary essential in $F$. Replacing an annular neighborhood of this boundary by two parallel copies of the disk reduces the surface's genus or separates it into simpler pieces.

#### Boundary-parallel surface

↑ **Parent:** [Incompressible surface](#incompressible-surface)

A properly embedded [topological surface](topological-surface.md) is boundary-parallel if it cobounds a product region with a [topological surface](topological-surface.md) in the ambient boundary, with the remaining boundary of that product contained in the ambient boundary. An [annulus](topology.md#annulus-mathematics) parallel into one boundary component has zero net oriented boundary class on that component.

#### Classification of incompressible surfaces in Seifert fibered spaces

↑ **Parent:** [Incompressible surface](#incompressible-surface)

In an orientable irreducible [Seifert fibered space](knot-theory.md#seifert-fibered-space), an essential two-sided [incompressible surface](#incompressible-surface) that is also a [boundary-incompressible surface](#boundary-incompressible-surface) can be isotoped to a [horizontal surface in a Seifert fibered space](knot-theory.md#horizontal-surface-in-a-seifert-fibered-space) or a [vertical surface in a Seifert fibered space](knot-theory.md#vertical-surface-in-a-seifert-fibered-space).

#### Boundary-incompressible surface

↑ **Parent:** [Incompressible surface](#incompressible-surface)

A properly embedded [topological surface](topological-surface.md) is boundary-incompressible when no disk in the ambient [three-manifold](#3-manifold) joins an essential arc on the [topological surface](topological-surface.md) to an arc on the ambient boundary, with the disk's interior disjoint from both.

### Heegaard splitting

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heegaard_splitting)

A Heegaard splitting divides a closed [three-manifold](#3-manifold) into two [handlebodies](#handlebody) with common boundary. For a [three-manifold](#3-manifold) with boundary, one uses compression bodies, which can retain negative boundary components.

#### Common nonseparating disks in a Heegaard splitting

↑ **Parent:** [Heegaard splitting](#heegaard-splitting)

Two nonseparating compressing disks on opposite sides with the same boundary form an embedded sphere. Cutting each [handlebody](#handlebody) along its disk leaves it connected, so the sphere is nonseparating in the glued [three-manifold](#3-manifold). Capping the two resulting sphere boundaries gives a splitting of one lower genus of the remaining summand; the removed summand is $S^1\times S^2$.

#### Heegaard genus

↑ **Parent:** [Heegaard splitting](#heegaard-splitting)

The least genus of a [Heegaard surface](#heegaard-surface) among all [Heegaard splittings](#heegaard-splitting) of a closed orientable [three-manifold](#3-manifold). Having a splitting of genus $g$ only proves $g_H(M)\le g$; stabilization supplies larger-genus splittings of the same manifold.

#### Heegaard Floer homology

↑ **Parent:** [Heegaard splitting](#heegaard-splitting)

Heegaard Floer homology assigns groups $HF^\circ(Y,\mathfrak s)$ to a closed oriented three-manifold with a [Spin-c structure](riemannian-geometry.md#spin-c-structure). A pointed [Heegaard diagram](#heegaard-diagram) of genus $g$ gives product [Lagrangian tori](symplectic-geometry.md#lagrangian-torus) $\mathbb T_\alpha,\mathbb T_\beta\subset\operatorname{Sym}^g(\Sigma)$; the [chain complex](homology.md#chain-complex) is generated by their intersection points and its differential counts [Whitney disk classes](#whitney-disk-class) represented by holomorphic disks. The minus, infinity, plus and hat versions use different powers or quotients of the variable $U$. The [Heegaard Floer cobordism maps](#heegaard-floer-cobordism-map) and the [Mixed Heegaard Floer invariant](#mixed-heegaard-floer-invariant) relate these groups to smooth four-dimensional topology.

##### Mixed Heegaard Floer invariant

↑ **Parent:** [Heegaard Floer homology](#heegaard-floer-homology)

For a closed smooth oriented four-manifold $M$ with $b_2^+(M)>1$, remove two balls to obtain $W:S^3\to S^3$, and choose an [Admissible cut for a Heegaard Floer mixed map](#admissible-cut-for-a-heegaard-floer-mixed-map). Positivity and naturality show that the minus map of $W_1$ lands in $HF^-_{\mathrm{red}}$, while the plus map of $W_2$ descends from $HF^+_{\mathrm{red}}$. Thus

$$
F^{\mathrm{mix}}_{W,\mathfrak s}=F^+_{W_2,\mathfrak s|W_2}\,\delta^{-1}\,F^-_{W_1,\mathfrak s|W_1}:HF^-(S^3)\longrightarrow HF^+(S^3).
$$

The coefficient of the bottom plus generator in this map, applied to $U^r\Theta^-\otimes\zeta$, defines $\Phi_{M,\mathfrak s}(U^r\otimes\zeta)\in\mathbb Z$, up to the orientation sign, with $\zeta\in\Lambda^*(H_1(M)/\mathrm{torsion})$. It vanishes unless $2r+\deg\zeta=(c_1(\mathfrak s)^2-2\chi(M)-3\sigma(M))/4$. The construction is independent of the admissible cut by the cobordism composition and associativity laws. Two positive pieces explain the condition $b_2^+>1$.

###### Adjunction inequality for the mixed Heegaard Floer invariant

↑ **Parent:** [Mixed Heegaard Floer invariant](#mixed-heegaard-floer-invariant)

If $\Phi_{M,\mathfrak s}\ne0$ and a connected closed oriented embedded surface $S$ has positive genus and $S^2\ge0$, then

$$
|\langle c_1(\mathfrak s),[S]\rangle|+S^2\le2g(S)-2.
$$

Blow up $S^2$ points on $S$ and choose the $\pm1$ exceptional determinant classes which increase the Chern pairing on its proper transform by $S^2$. The [Blowup formula for the mixed Heegaard Floer invariant](#blowup-formula-for-the-mixed-heegaard-floer-invariant) preserves nonvanishing, while the proper transform has square zero. A cut disjoint from it allows the relevant cobordism map to pass through $HF^\pm(S\times S^1,\mathfrak s|_{S\times S^1})$. These groups vanish when the Chern pairing exceeds $2g-2$, so the mixed map would then vanish, a contradiction. Reverse the surface orientation for the absolute value. The positive-genus condition is essential: a small nullhomologous sphere has square zero and zero pairing and would violate the displayed inequality.

###### Blowup formula for the mixed Heegaard Floer invariant

↑ **Parent:** [Mixed Heegaard Floer invariant](#mixed-heegaard-floer-invariant)

Let $\widetilde M=M\#\overline{\mathbb {CP}}^{,2}$, and let $E$ be the exceptional sphere. Extend a [Spin-c structure](riemannian-geometry.md#spin-c-structure) by $c_1(\widetilde{\mathfrak s})=c_1(\mathfrak s)\pm\operatorname{PD}[E]$. Then $\Phi_{\widetilde M,\widetilde{\mathfrak s}}=\Phi_{M,\mathfrak s}$. More generally, an evaluation $\langle c_1(\widetilde{\mathfrak s}),E\rangle=\pm(2\ell+1)$ introduces the factor $U^{\ell(\ell+1)/2}$. This follows by putting the blowup on one side of an admissible cut: the punctured exceptional piece is negative definite, its minus and plus tower maps are multiplication by this power of $U$, and the cobordism composition law gives the formula. In the $\pm1$ case the exponent is zero, so nonvanishing is preserved.

##### Integer-surgery exact triangle in Heegaard Floer homology

↑ **Parent:** [Heegaard Floer homology](#heegaard-floer-homology)

For a knot $K$ in an integral homology three-sphere and $n>0$, fix a [Spin-c structure](riemannian-geometry.md#spin-c-structure) $\mathfrak t_k$ on the $n$-surgery. Write $\mathfrak s_i$ for structures on zero-surgery with $\langle c_1(\mathfrak s_i),[\widehat F]\rangle=2i$, using a capped Seifert surface. In compatible labels the completed-minus triangle is

$$
\cdots\longrightarrow\mathbf{HF}^-(Y)\longrightarrow\bigoplus_{i\equiv k\ (\mathrm{mod}\ n)}\mathbf{HF}^-(Y_0,\mathfrak s_i)\longrightarrow\mathbf{HF}^-(Y_n,\mathfrak t_k)\longrightarrow\mathbf{HF}^-(Y)\longrightarrow\cdots.
$$

One can equally use the plus theory without completing. The first map is the congruence-restricted zero-surgery trace map; the last is the sum of reverse, orientation-reversed $n$-surgery trace maps. The middle map uses a Heegaard triple with an auxiliary lens-space generator. For $n=1$ that lens space is $S^3$, giving the usual three two-ended cobordism maps. For $n>1$ it is important to retain the auxiliary boundary and its fixed Spin-c structure. The [U-adic completion of Heegaard Floer homology](#u-adic-completion-of-heegaard-floer-homology) makes the sums of maps well-defined.

##### Heegaard Floer cobordism map

↑ **Parent:** [Heegaard Floer homology](#heegaard-floer-homology)

A smooth oriented [cobordism](geometry-and-topology.md#cobordism) $W:Y_1\to Y_2$ with a [Spin-c structure](riemannian-geometry.md#spin-c-structure) induces $U$-equivariant maps $F^\circ_{W,\mathfrak s}$ on the corresponding [Heegaard Floer homology](#heegaard-floer-homology) groups. A [handle decomposition](#handle-decomposition) defines the maps using generator selection for one- and three-handles and holomorphic triangle counts for two-handles. Composition sums over extensions of the prescribed Spin-c structures. When the boundary determinant classes are torsion, the absolute grading shift is

$$
\Delta(W,\mathfrak s)=\frac{c_1(\mathfrak s)^2-2\chi(W)-3\sigma(W)}4.
$$

The square is defined using the rational relative lift. If $b_2^+(W)>0$, the infinity map vanishes. Between rational homology spheres, when $b_1(W)=b_2^+(W)=0$, the infinity map is an isomorphism of Laurent towers.

###### Admissible cut for a Heegaard Floer mixed map

↑ **Parent:** [Heegaard Floer cobordism map](#heegaard-floer-cobordism-map)

An admissible cut splits a four-dimensional [cobordism](geometry-and-topology.md#cobordism) as $W=W_1\cup_N W_2$, with $b_2^+(W_1),b_2^+(W_2)>0$, and with the Mayer-Vietoris connecting map $H^1(N;\mathbb Z)\to H^2(W;\mathbb Z)$ equal to zero. The last condition removes the ambiguity in gluing [Spin-c structures](riemannian-geometry.md#spin-c-structure) on the two pieces. Positivity makes both infinity cobordism maps vanish, allowing passage through the [Reduced Heegaard Floer homology](#reduced-heegaard-floer-homology) of $N$. A useful cut is the boundary of a neighborhood of a positive-square embedded surface, chosen so that its complement still has a positive direction. The nonzero normal Euler number makes $H^1$ of the neighborhood surject onto $H^1$ of its boundary, proving the connecting-map condition.

##### Variants of Heegaard Floer homology

↑ **Parent:** [Heegaard Floer homology](#heegaard-floer-homology)

Use the convention that $CF^-$ is generated by $[\mathbf x,i]$ with $i<0$, and $U[\mathbf x,i]=[\mathbf x,i-1]$. The [chain complexes](homology.md#chain-complex) are

$$
CF^\infty=CF^-\otimes_{\mathbb Z[U]}\mathbb Z[U,U^{-1}],\qquad CF^+=CF^\infty/CF^-,\qquad \widehat{CF}=\ker(U:CF^+\to CF^+).
$$

The last complex is generated by $[\mathbf x,0]$. Equivalently it is $CF^-/UCF^-$ with its absolute grading shifted up by two. The short exact sequence $0\to CF^-\to CF^\infty\to CF^+\to0$ gives the fundamental [long exact sequence](homology.md#long-exact-sequence). For a rational homology sphere in each [Spin-c structure](riemannian-geometry.md#spin-c-structure), $HF^\infty\cong\mathbb Z[U,U^{-1}]$. The plus tower is $\mathcal T_d^+=\mathbb Z[U,U^{-1}]/U\mathbb Z[U]$, with bottom degree $d$; its corresponding minus tower is a free $\mathbb Z[U]$ module with top degree $d-2$.

###### Non-torsion Heegaard Floer homology of the sphere-circle product

↑ **Parent:** [Variants of Heegaard Floer homology](#variants-of-heegaard-floer-homology)

Let $\mathfrak s_k$ on $S^1\times S^2$ have $\langle c_1(\mathfrak s_k),[S^2]\rangle=2k\ne0$. The ordinary groups are

$$
HF^-(S^1\times S^2,\mathfrak s_k)=\mathbb Z[U]/(1-U^{|k|}),\qquad HF^\infty(S^1\times S^2,\mathfrak s_k)=\mathbb Z[U,U^{-1}]/(1-U^{|k|}),\qquad HF^+=\widehat{HF}=0.
$$

A sufficiently wound genus-one diagram gives a two-generator summand whose [chain differential](homology.md#boundary-operator) is multiplication by $1-U^{|k|}$: the two relevant disks have opposite coherent signs and basepoint multiplicities differing by $|k|$. The map is injective over $\mathbb Z[U]$, so its homology is the displayed quotient. Multiplication by $U$ is invertible in the quotient, showing that minus-to-infinity is an isomorphism and that the plus and hat groups vanish. In the [U-adic completion of Heegaard Floer homology](#u-adic-completion-of-heegaard-floer-homology), $1-U^{|k|}$ is a unit, so both completed minus and infinity groups vanish. This example shows why genus bounds for the completed-minus or plus groups must not be transferred unchanged to the ordinary minus theory.

###### Reduced Heegaard Floer homology

↑ **Parent:** [Variants of Heegaard Floer homology](#variants-of-heegaard-floer-homology)

The reduced minus and plus groups are

$$
HF^-_{\mathrm{red}}=\ker(HF^-\to HF^\infty),\qquad HF^+_{\mathrm{red}}=\operatorname{coker}(HF^\infty\to HF^+).
$$

The connecting homomorphism of the fundamental [long exact sequence](homology.md#long-exact-sequence) induces an isomorphism $\delta:HF^+_{\mathrm{red}}\to HF^-_{\mathrm{red}}$ of degree $-1$. This follows immediately from exactness: its image is the indicated kernel, and its kernel is precisely the image quotiented out on the plus side. These groups isolate the information lost by inverting $U$.

###### U-adic completion of Heegaard Floer homology

↑ **Parent:** [Variants of Heegaard Floer homology](#variants-of-heegaard-floer-homology)

Completing the minus [chain complex](homology.md#chain-complex) in powers of $U$ replaces $\mathbb Z[U]$ by the [formal power series ring](commutative-algebra.md#formal-power-series) $\mathbb Z[[U]]$; its homology is written $\mathbf{HF}^-$. This permits infinite sums of [Heegaard Floer cobordism maps](#heegaard-floer-cobordism-map) whose exponents tend to infinity, as occur in surgery formulas. A series with constant coefficient $\pm1$ is a unit: its inverse is found recursively, or by the geometric series for its positive-order part. Such a series need not have a polynomial inverse, which is why exact triangles involving sums over all Spin-c extensions require a completion in the minus theory. Individual homogeneous cobordism maps are still defined on the ordinary minus groups.

##### Heegaard Floer chain complex

↑ **Parent:** [Heegaard Floer homology](#heegaard-floer-homology)

For an admissible pointed [Heegaard diagram](#heegaard-diagram), $CF^-$ is a free $\mathbb Z[U]$ [chain complex](homology.md#chain-complex) with one generator for each point of $\mathbb T_\alpha\cap\mathbb T_\beta$. Each generator is an unordered selection containing exactly one intersection on each alpha circle and exactly one on each beta circle. After choosing coherent orientations,

$$
\partial^-\mathbf x=\sum_{\mathbf y}\sum_{\substack{\psi\in\pi_2(\mathbf x,\mathbf y)\\\mu(\psi)=1}}\#\widehat{\mathcal M}(\psi)\,U^{n_z(\psi)}\mathbf y.
$$

Here $\widehat{\mathcal M}$ is the moduli space modulo strip translation, $\mu$ is the [Maslov index](symplectic-geometry.md#maslov-index), and $n_z$ is multiplicity at the basepoint. Holomorphic representatives have nonnegative domain multiplicities. The differential lowers grading by one and $U$ lowers it by two. Boundary strata of one-dimensional moduli spaces give the cancellation proving $\partial^2=0$. Its homology is $HF^-$.

###### Coherent orientations in Heegaard Floer homology

↑ **Parent:** [Heegaard Floer chain complex](#heegaard-floer-chain-complex)

Over $\mathbb Z$, holomorphic disk moduli spaces in a [Heegaard Floer chain complex](#heegaard-floer-chain-complex) must be oriented compatibly with gluing: the orientation of a concatenated disk class is the product determinant-line orientation of its two factors. Boundary orientations of compactified one-dimensional moduli spaces then make broken disks cancel, yielding $\partial^2=0$. Isolated regular disks contribute $+1$ or $-1$. Changing the chosen orientation at an intersection generator changes the corresponding row and column signs of the differential and yields an isomorphic integral chain complex. Cobordism triangle counts require compatible orientation choices as well; an overall orientation ambiguity accounts for the usual sign ambiguity of the closed invariant.

###### Empty bigon and rectangle counts in Heegaard Floer homology

↑ **Parent:** [Heegaard Floer chain complex](#heegaard-floer-chain-complex)

An embedded positive domain which is a bigon or rectangle, has convex alternating alpha and beta corners, and contains no other selected coordinate in its interior, has [Maslov index](symplectic-geometry.md#maslov-index) one. A bigon has Euler measure $1/2$ and two corner averages $1/4$; a rectangle has Euler measure zero and four corner averages $1/4$. For the usual regular complex structure, its holomorphic disk count modulo translation is $\pm1$. For a bigon the Riemann map to the strip is unique up to translation. For a rectangle, the tautological correspondence represents the disk in the [symmetric product](topology.md#symmetric-product) by a branched double cover of the strip onto the rectangular domain: its conformal modulus fixes the branch parameter, and the only remaining freedom is translation. The resulting isolated regular disk gives one point in the oriented moduli space. The differential coefficient is $\pm U^{n_z}$, so a basepoint-free domain contributes a unit.

###### Relative grading in Heegaard Floer homology

↑ **Parent:** [Heegaard Floer chain complex](#heegaard-floer-chain-complex)

For generators in the same [Spin-c structure](riemannian-geometry.md#spin-c-structure) and a [Whitney disk class](#whitney-disk-class) $\psi$ joining them,

$$
\operatorname{gr}(\mathbf x)-\operatorname{gr}(\mathbf y)=\mu(\psi)-2n_z(\psi).
$$

The ambiguity is the divisibility of $c_1(\mathfrak s)$ on $H_2(Y)$; a torsion determinant class gives an integer relative grading. Adding a sphere class changes $\mu$ by two and $n_z$ by one, so it leaves the difference unchanged. For a domain $D$, the index can be calculated as $\mu(D)=e(D)+n_{\mathbf x}(D)+n_{\mathbf y}(D)$, where $e$ is Euler measure and each $n_{\mathbf x}$ is the sum of averages of the four adjacent region multiplicities at the selected intersections.

###### Absolute grading in Heegaard Floer homology

↑ **Parent:** [Relative grading in Heegaard Floer homology](#relative-grading-in-heegaard-floer-homology)

For a torsion [Spin-c structure](riemannian-geometry.md#spin-c-structure), the relative grading of [Heegaard Floer homology](#heegaard-floer-homology) lifts canonically to a rational absolute grading, normalized by the bottom plus generator of $S^3$ having degree zero. Multiplication by $U$ has degree $-2$, and a [Heegaard Floer cobordism map](#heegaard-floer-cobordism-map) has degree $(c_1^2-2\chi-3\sigma)/4$. The correction term $d(Y,\mathfrak s)$ is the lowest grading of the image of $HF^\infty$ in $HF^+$ for a rational homology sphere. A pure tower then has bottom plus degree $d$ and top minus degree $d-2$ in the $i<0$ minus convention. Keeping that shift explicit prevents errors of two in surgery and mixed-invariant calculations.

###### Whitney disk class

↑ **Parent:** [Heegaard Floer chain complex](#heegaard-floer-chain-complex)

For intersection generators $\mathbf x,\mathbf y$, a Whitney disk is a map of a disk into the [symmetric product](topology.md#symmetric-product), with its two boundary semicircles mapped to the two product tori and its endpoints mapped to $\mathbf x,\mathbf y$. Its homotopy class belongs to $\pi_2(\mathbf x,\mathbf y)$. Projecting it to the [Heegaard surface](#heegaard-surface) gives an integral domain. With the surface oriented, the convention is $\partial_\alpha D=\mathbf y-\mathbf x$. The obstruction to a disk is the class $\epsilon(\mathbf x,\mathbf y)\in H_1(Y)$ obtained by joining the points along alpha arcs and returning along beta arcs. In the Heegaard Floer setup, its vanishing is equivalent to equality of the generators' [Spin-c structures](riemannian-geometry.md#spin-c-structure); for the rational homology sphere diagrams this is equivalent to $\pi_2(\mathbf x,\mathbf y)\ne\varnothing$.

#### Compression body

↑ **Parent:** [Heegaard splitting](#heegaard-splitting)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compression_body)

A compression body is obtained from a product $F\times I$ by attaching [one-handles](#one-handle) to $F\times\{1\}$, allowing three-ball components as well. Its negative boundary is the retained copy of $F$ and its positive boundary is the other boundary component. A [handlebody](#handlebody) has empty negative boundary.

#### Heegaard surface

↑ **Parent:** [Heegaard splitting](#heegaard-splitting)

The Heegaard surface is the common positive boundary of the two pieces in a [Heegaard splitting](#heegaard-splitting).

##### Heegaard diagram

↑ **Parent:** [Heegaard surface](#heegaard-surface)

A Heegaard diagram marks the boundaries of compressing disks from the two sides of a [Heegaard surface](#heegaard-surface). Attaching [two-handles](#two-handle) along the two collections, and capping resulting spherical boundary components, reconstructs the [three-manifold](#3-manifold).

###### Generalized Heegaard diagram

↑ **Parent:** [Heegaard diagram](#heegaard-diagram)

A generalized [Heegaard diagram](#heegaard-diagram) permits [compression bodies](#compression-body) and a nonempty negative boundary. Equivalently, a suitable [handlebody](#handlebody) with [two-handles](#two-handle) attached along only part of a compressing system can retain torus boundary components. Disk crossings supply generators and attaching-curve words supply relators for its [fundamental group](algebraic-topology.md#fundamental-group).

###### Dehn presentation Heegaard diagram

↑ **Parent:** [Heegaard diagram](#heegaard-diagram)

Thicken the planar graph underlying a [knot diagram](knot-theory.md#knot-diagram). Its boundary supports a [Heegaard diagram](#heegaard-diagram) with face disks on one side and crossing-tunnel disks on the other. The face generators and crossing curves give a [Dehn presentation of a knot group](knot-theory.md#dehn-presentation-of-a-knot-group).

### Handlebody

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Handlebody)

A genus-$g$ handlebody is a three-ball with $g$ [one-handles](#one-handle) attached. Its boundary is a closed orientable [topological surface](topological-surface.md) of [genus](topological-surface.md#genus-of-a-surface) $g$.

### Thurston elliptization conjecture

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thurston_elliptization_conjecture)

Every connected closed orientable [three-manifold](#3-manifold) with finite [fundamental group](algebraic-topology.md#fundamental-group) admits spherical geometry. With cyclic [fundamental group](algebraic-topology.md#fundamental-group), it is a [lens space](knot-theory.md#lens-space).

## Homology above the dimension of a manifold

↑ **Parent:** [Topological manifold](topological-manifold.md)

An $n$-manifold has zero singular homology in every degree greater than $n$. One proof uses a countable exhaustion by subsets that retract onto $n$-dimensional CW complexes and the compact support of every singular cycle.

## ↑ Ancestors (5)

1. [Topology](topology.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (17)

- [3-manifold](#3-manifold)
- [Category of topological manifolds](#category-of-topological-manifolds)
- [Dimension of a manifold](#dimension-of-a-manifold)
- [Foliation](geometry-and-topology.md#foliation)
- [Invariance of domain](#invariance-of-domain)
- [Manifold criterion for a suspension](algebraic-topology.md#manifold-criterion-for-a-suspension)
- [Paracompact space](topology.md#paracompact-space)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-19.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-15.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-118.md#1/a/solution)
- [Smooth atlas](differential-geometry.md#smooth-atlas)
- [Topological atlas](#topological-atlas)
- [Topological generalized Poincare theorem](cohomology.md#topological-generalized-poincare-theorem)
- [Topological manifold](topological-manifold.md)
- [Topological manifold with boundary](#topological-manifold-with-boundary)
- [Two stereographic charts on the circle](#two-stereographic-charts-on-the-circle)
