# Topology

↑ **Parent:** [Geometry and topology](geometry-and-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topology)

Topology studies spaces and properties preserved by continuous deformation.

**Table of contents**

- [End (topology)](#end-topology)
- [Orientability](#orientability)
- [Non-Hausdorff manifold](#non-hausdorff-manifold)
- [Stone space](#stone-space)
- [Tail topology on the natural numbers](#tail-topology-on-the-natural-numbers)
  - [Continuous maps between cofinite and tail topologies](#continuous-maps-between-cofinite-and-tail-topologies)
- [Fell topology](#fell-topology)
- [Upper-ray topology on the real line](#upper-ray-topology-on-the-real-line)
- [Hyperconnected space](#hyperconnected-space)
- [Closed cover](#closed-cover)
- [Partition topology](#partition-topology)
- [Finite subsets do not define a topology on an infinite set](#finite-subsets-do-not-define-a-topology-on-an-infinite-set)
- [Lower limit topology](#lower-limit-topology)
  - [Sorgenfrey plane](#sorgenfrey-plane)
- [Symmetric product](#symmetric-product)
- [Extremally disconnected space](#extremally-disconnected-space)
- [Countable complement topology](#countable-complement-topology)
  - [Compact subsets of a cocountable space](#compact-subsets-of-a-cocountable-space)
- [Locally finite family of subsets](#locally-finite-family-of-subsets)
- [Indiscrete topology](#indiscrete-topology)
- [Triangulation of a surface](#triangulation-of-a-surface)
- [Pasting lemma for closed subspaces](#pasting-lemma-for-closed-subspaces)
- [Cofinite topology](#cofinite-topology)
- [Hahn-Mazurkiewicz theorem](#hahn-mazurkiewicz-theorem)
  - [Peano continuum](#peano-continuum)
- [Topological manifold](#topological-manifold)
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
- [Closed set](#closed-set)
  - [Sequentially closed set](#sequentially-closed-set)
  - [Limit point](#limit-point)
- [Closure (topology)](#closure-topology)
  - [Adherent point](#adherent-point)
- [Interior (topology)](#interior-topology)
- [Topological space](#topological-space)
  - [Open and closed maps](#open-and-closed-maps)
  - [Stratified space](#stratified-space)
    - [Stratum of a stratified space](#stratum-of-a-stratified-space)
    - [Stratified pseudomanifold](#stratified-pseudomanifold)
      - [Normalization of a two-dimensional pseudomanifold](#normalization-of-a-two-dimensional-pseudomanifold)
      - [Witt space](#witt-space)
        - [Witt space with collared boundary](#witt-space-with-collared-boundary)
      - [Link of a stratum](#link-of-a-stratum)
  - [Continuous real maps from the initial-segment topology](#continuous-real-maps-from-the-initial-segment-topology)
  - [Sigma-compact space](#sigma-compact-space)
  - [Sober space](#sober-space)
    - [Sobrification](#sobrification)
  - [Separable topological space](#separable-topological-space)
  - [G-delta set](#g-delta-set)
  - [Net (mathematics)](#net-mathematics)
    - [Subnet of a net](#subnet-of-a-net)
  - [Separation axiom](#separation-axiom)
    - [T1 space](#t1-space)
  - [Closed point](#closed-point)
  - [Locally connected space](#locally-connected-space)
  - [Boundary of a set](#boundary-of-a-set)
    - [Boundary of a domain](#boundary-of-a-domain)
  - [Basis of a topology](#basis-of-a-topology)
  - [Second-countable space](#second-countable-space)
  - [Paracompact space](#paracompact-space)
  - [Kolmogorov space](#kolmogorov-space)
    - [Sierpiński space](#sierpinski-space)
      - [Embedding of a T0 space into a power of the Sierpiński space](#embedding-of-a-t0-space-into-a-power-of-the-sierpinski-space)
  - [Continuous map](#continuous-map)
    - [Scalar clipping](#scalar-clipping)
    - [Topological embedding](#topological-embedding)
  - [Retraction](#retraction)
    - [Retraction onto a punctured oriented surface](#retraction-onto-a-punctured-oriented-surface)
  - [Subspace topology](#subspace-topology)
  - [Alexandroff extension](#alexandroff-extension)
    - [Hawaiian earring](#hawaiian-earring)
      - [Rational summand in Hawaiian earring homology](#rational-summand-in-hawaiian-earring-homology)
  - [Circle](#circle)
    - [Chord of a circle](#chord-of-a-circle)
    - [Reflection symmetry of a complex circle equation](#reflection-symmetry-of-a-complex-circle-equation)
    - [Maximum separation of two circles](#maximum-separation-of-two-circles)
    - [Steiner chain](#steiner-chain)
      - [Steiner porism](#steiner-porism)
      - [Tangency locus of a Steiner chain](#tangency-locus-of-a-steiner-chain)
    - [Circle from an affine complex-modulus equation](#circle-from-an-affine-complex-modulus-equation)
    - [Radius](#radius)
    - [Pi](#pi)
      - [Wallis product](#wallis-product)
      - [Proof that π is irrational](#proof-that-pi-is-irrational)
  - [Wedge sum](#wedge-sum)
    - [Pinch map](#pinch-map)
    - [Wedge of two circles](#wedge-of-two-circles)
  - [Inclusion map](#inclusion-map)
  - [Topology axiom](#topology-axiom)
  - [Open cover](#open-cover)
    - [Affine open cover](#affine-open-cover)
    - [Acyclic cover](#acyclic-cover)
- [Quotient topology](#quotient-topology)
  - [Quotient topological space](#quotient-topological-space)
  - [Quotient map](#quotient-map)
  - [Universal property of the quotient topology](#universal-property-of-the-quotient-topology)
  - [Non-Hausdorff quotient of the real line by rational translation](#non-hausdorff-quotient-of-the-real-line-by-rational-translation)
  - [Square quotient model of the two-sphere](#square-quotient-model-of-the-two-sphere)
- [Open set](#open-set)
  - [Domain (mathematical analysis)](#domain-mathematical-analysis)
  - [Clopen set](#clopen-set)
  - [Open interval](#open-interval)
    - [Nondegenerate interval](#nondegenerate-interval)
  - [Neighbourhood (mathematics)](#neighbourhood-mathematics)
    - [Neighbourhood system](#neighbourhood-system)
      - [Neighbourhood basis](#neighbourhood-basis)
  - [Open ball](#open-ball)
  - [Annulus (mathematics)](#annulus-mathematics)
    - [Fixed-point-free rotation of an annulus](#fixed-point-free-rotation-of-an-annulus)
- [Disk (mathematics)](#disk-mathematics)
  - [Open disc](#open-disc)
    - [Unit disc](#unit-disc)
      - [Automorphism of the unit disk](#automorphism-of-the-unit-disk)
- [Topological disc](#topological-disc)
  - [Closed disc](#closed-disc)
- [Level set](#level-set)
  - [Level curve](#level-curve)
  - [Regular level set](#regular-level-set)
  - [Superlevel set](#superlevel-set)
- [Dense set](#dense-set)
- [Discrete space](#discrete-space)
  - [Discrete subset](#discrete-subset)
    - [Closed discrete subset](#closed-discrete-subset)
    - [Discrete subsets of the real line are countable](#discrete-subsets-of-the-real-line-are-countable)
- [Connected-space zero-product dichotomy](#connected-space-zero-product-dichotomy)
- [Normal space](#normal-space)
  - [Closed-neighborhood shrinking in a normal space](#closed-neighborhood-shrinking-in-a-normal-space)
  - [Urysohn's lemma](#urysohn-s-lemma)
    - [Tietze extension theorem](#tietze-extension-theorem)
      - [Metric Tietze two-thirds approximation](#metric-tietze-two-thirds-approximation)
  - [Closed G-delta set as a zero set](#closed-g-delta-set-as-a-zero-set)
- [Compact space](#compact-space)
  - [Ultrafilter characterization of compactness](#ultrafilter-characterization-of-compactness)
  - [Compact exhaustion](#compact-exhaustion)
  - [Compact Hausdorff space](#compact-hausdorff-space)
    - [Supremum convergence for decreasing continuous functions](#supremum-convergence-for-decreasing-continuous-functions)
    - [Closed relation generated by a set-split pair of compact Hausdorff maps](#closed-relation-generated-by-a-set-split-pair-of-compact-hausdorff-maps)
    - [Separable compactification need not be metrizable](#separable-compactification-need-not-be-metrizable)
  - [Heine-Borel theorem](#heine-borel-theorem)
  - [Finite intersection property](#finite-intersection-property)
  - [Continuous image of a compact space](#continuous-image-of-a-compact-space)
  - [Quotient of a compact space](#quotient-of-a-compact-space)
  - [Lebesgue number lemma](#lebesgue-number-lemma)
  - [Normality of a compact Hausdorff space](#normality-of-a-compact-hausdorff-space)
  - [Alexander's subbase lemma](#alexander-s-subbase-lemma)
  - [Locally compact space](#locally-compact-space)
    - [Compactly detected closed-set theorem in a locally compact Hausdorff space](#compactly-detected-closed-set-theorem-in-a-locally-compact-hausdorff-space)
- [Hausdorff space](#hausdorff-space)
  - [Completely regular Hausdorff space](#completely-regular-hausdorff-space)
  - [Compact subset of a Hausdorff space](#compact-subset-of-a-hausdorff-space)
  - [Compact-to-Hausdorff continuous bijection theorem](#compact-to-hausdorff-continuous-bijection-theorem)
  - [Closed diagonal theorem](#closed-diagonal-theorem)
- [Homeomorphism](#homeomorphism)
  - [Inverse continuity from an open bijection](#inverse-continuity-from-an-open-bijection)
  - [Local homeomorphism](#local-homeomorphism)
  - [Closed map](#closed-map)
    - [Projection with a compact factor is closed](#projection-with-a-compact-factor-is-closed)
    - [Compact-preimage theorem for closed maps](#compact-preimage-theorem-for-closed-maps)
- [Unit sphere](#unit-sphere)
- [Closed graph theorem for compact spaces](#closed-graph-theorem-for-compact-spaces)
  - [Closed-graph criterion with compact codomain](#closed-graph-criterion-with-compact-codomain)
- [Curve](#curve)
  - [Asymptote](#asymptote)
  - [Parametric curve](#parametric-curve)
    - [Parametric curve interrogation](#parametric-curve-interrogation)
      - [Certified curve-plane intersection](#certified-curve-plane-intersection)
    - [Cycloid](#cycloid)
  - [Space curve](#space-curve)
    - [Helix](#helix)
      - [Logarithmic conical helix](#logarithmic-conical-helix)
      - [Pitch of a helix](#pitch-of-a-helix)
  - [Inflection point](#inflection-point)
  - [Logarithmic spiral](#logarithmic-spiral)
    - [Logarithmic spiral as an embedded real line](#logarithmic-spiral-as-an-embedded-real-line)
  - [Simple curve](#simple-curve)
  - [Space-filling curve](#space-filling-curve)
- [Topological surface](#topological-surface)
  - [Classification of compact surfaces](#classification-of-compact-surfaces)
  - [Thrice-punctured sphere](#thrice-punctured-sphere)
  - [Integral top homology of a compact connected surface](#integral-top-homology-of-a-compact-connected-surface)
  - [Surface with boundary](#surface-with-boundary)
    - [Topology of disk tiles glued along disjoint boundary arcs](#topology-of-disk-tiles-glued-along-disjoint-boundary-arcs)
    - [Pair of pants (mathematics)](#pair-of-pants-mathematics)
      - [Hyperbolic Y-piece](#hyperbolic-y-piece)
        - [Hyperbolic X-piece](#hyperbolic-x-piece)
      - [Homology action of a pair-of-pants homeomorphism](#homology-action-of-a-pair-of-pants-homeomorphism)
  - [Genus of a surface](#genus-of-a-surface)
    - [Genus monotonicity under nonzero-degree surface maps](#genus-monotonicity-under-nonzero-degree-surface-maps)
  - [Closed orientable surface](#closed-orientable-surface)
    - [Genus of a finite cover of a closed orientable surface](#genus-of-a-finite-cover-of-a-closed-orientable-surface)
  - [Non-orientable surface](#non-orientable-surface)
    - [Closed nonorientable surface](#closed-nonorientable-surface)
  - [Surface quotient by a free finite action](#surface-quotient-by-a-free-finite-action)
  - [Jordan curve theorem](#jordan-curve-theorem)
    - [Jordan separation from the exponential quotient](#jordan-separation-from-the-exponential-quotient)
    - [Jordan domain](#jordan-domain)
    - [Schoenflies theorem](#schoenflies-theorem)
    - [Outer boundary of a planar compact set](#outer-boundary-of-a-planar-compact-set)
  - [Moore triod theorem](#moore-triod-theorem)
  - [Polygonal schema](#polygonal-schema)
    - [Polygonal-schema Euler count](#polygonal-schema-euler-count)
    - [Regular hyperbolic octagon fundamental polygon](#regular-hyperbolic-octagon-fundamental-polygon)
  - [Mapping class group](#mapping-class-group)
    - [Mapping class](#mapping-class)
    - [Injection of a finite hyperbolic isometry group into a mapping class group](#injection-of-a-finite-hyperbolic-isometry-group-into-a-mapping-class-group)
    - [Realization of a finite group as a surface deck group](#realization-of-a-finite-group-as-a-surface-deck-group)
    - [Dehn twist](#dehn-twist)
      - [Lickorish-Dehn theorem](#lickorish-dehn-theorem)
      - [Homology action of a Dehn twist](#homology-action-of-a-dehn-twist)
      - [Right-handed Dehn twist](#right-handed-dehn-twist)
    - [Essential proper arc on a punctured surface](#essential-proper-arc-on-a-punctured-surface)
      - [Bigon formed by two arcs](#bigon-formed-by-two-arcs)
      - [Minimal position of curves or arcs](#minimal-position-of-curves-or-arcs)
        - [Bigon criterion](#bigon-criterion)
    - [Geometric intersection number](#geometric-intersection-number)
      - [Algebraic intersection number of curves on an oriented surface](#algebraic-intersection-number-of-curves-on-an-oriented-surface)
        - [Isotopy invariance of algebraic intersection number](#isotopy-invariance-of-algebraic-intersection-number)
    - [Arc complex](#arc-complex)
      - [Arc complex of the three-punctured sphere](#arc-complex-of-the-three-punctured-sphere)
      - [Arc-complex vertex orbits of the four-punctured sphere](#arc-complex-vertex-orbits-of-the-four-punctured-sphere)
    - [Alexander system](#alexander-system)
      - [Structure graph of an Alexander system](#structure-graph-of-an-alexander-system)
      - [Alexander method](#alexander-method)
        - [Alexander trick](#alexander-trick)
        - [Center of the mapping class group of the torus](#center-of-the-mapping-class-group-of-the-torus)
    - [Mapping-class action on the outer automorphism group of the fundamental group](#mapping-class-action-on-the-outer-automorphism-group-of-the-fundamental-group)
    - [Pure mapping class group](#pure-mapping-class-group)
      - [Point-pushing map](#point-pushing-map)
        - [Birman exact sequence](#birman-exact-sequence)
      - [Pure mapping class group of the three-punctured sphere](#pure-mapping-class-group-of-the-three-punctured-sphere)
      - [Pure mapping class group of the four-punctured sphere](#pure-mapping-class-group-of-the-four-punctured-sphere)
      - [Semidirect-product decomposition of the pure mapping class group of the five-punctured sphere](#semidirect-product-decomposition-of-the-pure-mapping-class-group-of-the-five-punctured-sphere)
    - [Curve complex](#curve-complex)
      - [Connectedness of the curve complex](#connectedness-of-the-curve-complex)
      - [Filling set of curves](#filling-set-of-curves)
        - [Filling pair on a closed genus-two surface](#filling-pair-on-a-closed-genus-two-surface)
  - [Torus](#torus)
    - [Three-critical-point function on a torus](#three-critical-point-function-on-a-torus)
    - [Pinched torus](#pinched-torus)
    - [Three-dimensional torus](#three-dimensional-torus)
    - [Cohomology ring of a torus](#cohomology-ring-of-a-torus)
    - [Homology of an integer torus endomorphism](#homology-of-an-integer-torus-endomorphism)
    - [Solid torus](#solid-torus)
      - [Solid-torus recognition by a compression disk](#solid-torus-recognition-by-a-compression-disk)
      - [Meridian of a solid torus](#meridian-of-a-solid-torus)
    - [Embedding of the n-dimensional torus in codimension one](#embedding-of-the-n-dimensional-torus-in-codimension-one)
    - [Embedded torus of revolution](#embedded-torus-of-revolution)
    - [Fundamental group of the torus](#fundamental-group-of-the-torus)
      - [Lift-endpoint description of the fundamental group of the torus](#lift-endpoint-description-of-the-fundamental-group-of-the-torus)
    - [Integral linear automorphism of the torus](#integral-linear-automorphism-of-the-torus)
      - [Equivalence of connected double covers of the torus](#equivalence-of-connected-double-covers-of-the-torus)
  - [Möbius band](#mobius-band)
  - [Klein bottle](#klein-bottle)
    - [Mod-two intersection pairing of the Klein bottle](#mod-two-intersection-pairing-of-the-klein-bottle)
    - [Integral cohomology ring of the Klein bottle](#integral-cohomology-ring-of-the-klein-bottle)
      - [Integral cohomology ring of the wedge of the real projective plane and a circle](#integral-cohomology-ring-of-the-wedge-of-the-real-projective-plane-and-a-circle)
    - [Orientation double cover of the Klein bottle](#orientation-double-cover-of-the-klein-bottle)
      - [Klein-bottle mapping-cylinder obstruction to simple connectivity](#klein-bottle-mapping-cylinder-obstruction-to-simple-connectivity)
    - [Flat Klein-bottle geodesic model](#flat-klein-bottle-geodesic-model)
  - [Double cone singularity](#double-cone-singularity)
- [Knaster-Kuratowski-Mazurkiewicz lemma](#knaster-kuratowski-mazurkiewicz-lemma)
  - [Triangle KKM lemma](#triangle-kkm-lemma)
    - [Distance-function barycentric map](#distance-function-barycentric-map)
    - [No-retraction covering principle](#no-retraction-covering-principle)

## End (topology)

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/End_(topology))

An end of a noncompact [topological space](#topological-space) describes a coherent way to escape every compact subset. For a cofinal compact exhaustion, when one exists, $K_1\subseteq K_2\subseteq\cdots$, it is represented by nested connected components of the complements. A connected noncompact manifold is [disconnected at infinity](riemannian-geometry.md#disconnected-at-infinity) when it has more than one end.

## Orientability

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orientability)

Orientability is the existence of a consistent choice of orientation across a [manifold](#topological-manifold). For a [smooth manifold](differential-geometry.md#smooth-manifold), the transition maps of an oriented atlas have positive Jacobian determinant; for a surface this rules out a Möbius-band neighborhood. The [orientable smooth manifold](differential-geometry.md#orientable-smooth-manifold) condition is its differentiable formulation.

## Non-Hausdorff manifold

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Non-Hausdorff_manifold)

A [non-Hausdorff manifold](#non-hausdorff-manifold) is a locally Euclidean [topological space](#topological-space) for which distinct points need not have disjoint neighborhoods. The real line with two origins is a basic example. Nonseparated algebraic schemes exhibit analogous gluing phenomena, but are not generally topological manifolds.

## Stone space

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stone_space)

A [Stone space](#stone-space) is a [compact](#compact-space) [Hausdorff space](#hausdorff-space) that is [totally disconnected](arithmetic.md#totally-disconnected-space), equivalently a compact Hausdorff space with a basis of clopen sets. The topology on a [type space](foundations-of-mathematics.md#type-space) gives an important example.

## Tail topology on the natural numbers

↑ **Parent:** [Topology](topology.md)

The nonempty open sets are the upper tails of the [natural numbers](arithmetic.md#natural-number). Arbitrary nonempty unions select the smallest starting index, and finite intersections select the largest, so these sets form a [topology](topology.md). A map into this space is [continuous](calculus.md#continuous-function) exactly when the inverse image of every upper tail is open.

### Continuous maps between cofinite and tail topologies

↑ **Parent:** [Tail topology on the natural numbers](#tail-topology-on-the-natural-numbers)

For a map $f:\mathbb N\to\mathbb N$ from the [cofinite topology](#cofinite-topology) to the [tail topology on the natural numbers](#tail-topology-on-the-natural-numbers), [continuity](calculus.md#continuous-function) is equivalent to every set $\{n:f(n)\ge k\}$ being empty or cofinite. If the image is unbounded, every such set is nonempty and cofinite, so $f(n)\to\infty$. If it is bounded, its maximum $M$ exists, and the inverse image of the tail at $M$ forces $f(n)=M$ eventually, with $f(n)\le M$ always. Conversely either condition makes every tail preimage empty or cofinite.

## Fell topology

↑ **Parent:** [Topology](topology.md)

The [Fell topology](#fell-topology) on the closed subsets of a [locally compact space](#locally-compact-space) has subbasic open sets requiring intersection with an open set or avoidance of a [compact set](#compact-space). On a locally compact separable metric space, its sequential convergence says that every convergent subsequence of points from the varying sets has its limit in the limiting set, and every point of the limiting set is approximated by points from the varying sets.

## Upper-ray topology on the real line

↑ **Parent:** [Topology](topology.md)

These sets form a [topology](topology.md): a nonempty union of upper rays is another upper ray, or all of $\mathbb R$ when their endpoints have no lower bound; a finite intersection of rays has endpoint the maximum of their endpoints. The whole line must be included. The [continuous map](#continuous-map) $n\mapsto n$ from $\mathbb N$ with the [cofinite topology](#cofinite-topology) to this space is nonconstant, because each upper ray has cofinite inverse image.

## Hyperconnected space

↑ **Parent:** [Topology](topology.md)

A [topological space](#topological-space) is hyperconnected if any two nonempty [open sets](#open-set) intersect. Every [continuous map](#continuous-map) from a nonempty hyperconnected space to a [Hausdorff space](#hausdorff-space) is constant: two distinct image points would have disjoint open neighbourhoods whose nonempty inverse images contradict hyperconnectedness. Every infinite set with the [cofinite topology](#cofinite-topology) is hyperconnected.

## Closed cover

↑ **Parent:** [Topology](topology.md)

A closed cover of a [topological space](#topological-space) is a family of [closed sets](#closed-set) whose union is the whole space. A finite closed cover can be used in separation and antipodal arguments: in a [metric space](topological-analysis.md#metric-space), vanishing distance to a closed member means actual membership. Unlike an [open cover](#open-cover), a closed cover does not automatically have a partition of unity subordinate to its members.

## Partition topology

↑ **Parent:** [Topology](topology.md)

Given a partition of a [set](set.md), declare a subset open precisely when it is a union of partition blocks. Arbitrary unions and finite intersections of such unions are again unions of blocks, giving a [topology](topology.md). The quotient map to the block set with its [discrete topology](#discrete-space) pulls that topology back to the original set. For the partition of $\mathbb Z$ into its two parity classes, the only open sets are the empty set, those two classes, and all of $\mathbb Z$.

## Finite subsets do not define a topology on an infinite set

↑ **Parent:** [Topology](topology.md)

On an infinite [set](set.md), the family consisting of all finite subsets and the whole set need not be closed under arbitrary unions. On $\mathbb Z$, the union of the singleton subsets of $2\mathbb Z$ is infinite and proper, so this family is not a [topology](topology.md). It must not be confused with the [cofinite topology](#cofinite-topology), whose proper open sets have finite complements.

## Lower limit topology

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lower_limit_topology)

The lower limit topology on $\mathbb R$ has [basis of a topology](#basis-of-a-topology) $\{[a,b):a<b\}$. Every such nonempty interval contains a rational, so this [topological space](#topological-space) is separable. Its topology is finer than the usual Euclidean topology; the one-sided basic neighbourhoods allow its square to have an uncountable discrete antidiagonal.

### Sorgenfrey plane

↑ **Parent:** [Lower limit topology](#lower-limit-topology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sorgenfrey_plane)

The Sorgenfrey plane is the [product topology](geometry-and-topology.md#product-topology) on two copies of the [Sorgenfrey line](#lower-limit-topology). It is separable because $\mathbb Q^2$ meets every nonempty basic rectangle $[a,b)\times[c,d)$. Its antidiagonal $\{(x,-x):x\in\mathbb R\}$ is an uncountable discrete subspace: $[x,x+\epsilon)\times[-x,-x+\epsilon)$ meets it only at $(x,-x)$. In a discrete space every dense subset is the whole space, so this subspace is not separable. Thus separability need not pass to subspaces of nonmetrizable spaces.

// Target: analysis.bigb

## Symmetric product

↑ **Parent:** [Topology](topology.md)

The $g$th symmetric product of a space $X$ is $\operatorname{Sym}^g(X)=X^g/S_g$, where the [symmetric group](finite-group-theory.md#symmetric-group) permutes the factors. Its points are unordered $g$-tuples, with repetitions allowed. If $X$ is a [Riemann surface](complex-analysis.md#riemann-surfaces), elementary symmetric functions in local complex coordinates make its symmetric product a smooth complex manifold, including along the locus of repeated points. A collection of disjoint circles in $X$ gives a product torus in this symmetric product.

## Extremally disconnected space

↑ **Parent:** [Topology](topology.md)

A [topological space](#topological-space) is extremally disconnected when the closure of every [open set](#open-set) is open. This concerns open sets, not arbitrary subsets. In particular, a nonisolated singleton in a [Hausdorff space](#hausdorff-space) is closed but not open, so its closure gives a counterexample to that stronger condition.

## Countable complement topology

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Countable_complement_topology)

The open sets are the empty set and subsets whose complement is countable. On an uncountable set, any two nonempty open sets intersect, so the space is not [Hausdorff](#hausdorff-space). On a countable underlying set this topology is discrete. The [compact subsets of a cocountable space](#compact-subsets-of-a-cocountable-space) are finite, regardless of the cardinality of the underlying set.

### Compact subsets of a cocountable space

↑ **Parent:** [Countable complement topology](#countable-complement-topology)

Only finite subsets are compact in the [cocountable topology](#countable-complement-topology). An infinite subset contains distinct $c_1,c_2,\ldots$. The open sets obtained by removing the tails $\{c_j:j\geq n\}$ form an increasing [open cover](#open-cover), but every finite selection misses a tail point. Finite sets are compact in every topology.

## Locally finite family of subsets

↑ **Parent:** [Topology](topology.md)

A family $(A_i)$ of subsets of a [topological space](#topological-space) is locally finite if every point has a neighbourhood meeting only finitely many of its members. On a compact space such a family has only finitely many nonempty members. For singleton subsets of a [Riemann surface](complex-analysis.md#riemann-surfaces), this is the condition permitting prescribed poles of a [meromorphic function](isolated-singularity.md#meromorphic-function) without accumulation inside the surface.

## Indiscrete topology

↑ **Parent:** [Topology](topology.md)

The indiscrete topology on a set $X$ has only the empty set and the whole set as [open sets](#open-set). When $X$ has more than one point it is not a [Hausdorff space](#hausdorff-space). For example the [quotient topology](#quotient-topology) on $\mathbb R/\mathbb Q$ is indiscrete: a nonempty open saturated subset contains an interval and all its rational translates, which cover $\mathbb R$.

## Triangulation of a surface

↑ **Parent:** [Topology](topology.md)

A triangulation of a surface decomposes it into triangles meeting along full edges or vertices. On a closed surface, each edge is incident with two triangle faces, so $3F=2E$. [Euler characteristic](homology.md#euler-characteristic) connects this local counting relation with the surface's topology.

## Pasting lemma for closed subspaces

↑ **Parent:** [Topology](topology.md)

If a space is the union of finitely many closed subspaces and continuous maps on those subspaces agree on every overlap, they combine into a continuous map on the whole space. For a closed target set, its preimage is a finite union of closed sets.

## Cofinite topology

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cofinite_topology)

The cofinite topology on a set $X$ consists of the empty set together with every subset whose complement is finite. On an infinite set, any two nonempty open sets intersect.

## Hahn-Mazurkiewicz theorem

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hahn-Mazurkiewicz_theorem)

A nonempty Hausdorff space is the continuous image of $[0,1]$ exactly when it is compact, connected, locally connected, and second-countable.

### Peano continuum

↑ **Parent:** [Hahn-Mazurkiewicz theorem](#hahn-mazurkiewicz-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Peano_continuum)

A Peano continuum is a compact, connected, locally connected metric space. By the [Hahn-Mazurkiewicz theorem](#hahn-mazurkiewicz-theorem), every Peano continuum is the image of a continuous surjection from $[0,1]$.

## Topological manifold

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_manifold)

A topological $n$-manifold is a Hausdorff second-countable space in which every point has a neighborhood homeomorphic to an open subset of $\mathbb R^n$.

### Piecewise linear ball

↑ **Parent:** [Topological manifold](#topological-manifold)

A piecewise linear ball is a [simplicial complex](algebraic-topology.md#simplicial-complex) admitting a [homeomorphism](#homeomorphism) to an $n$-[simplex](algebraic-topology.md#simplex) that is linear on the [simplexes](algebraic-topology.md#simplex) of suitable finite [simplicial subdivisions](algebraic-topology.md#simplicial-subdivision). Its [boundary](#boundary-of-a-set) is a piecewise linear [sphere](geometry-and-topology.md#sphere).

#### Gluing three-balls along a boundary disk

↑ **Parent:** [Piecewise linear ball](#piecewise-linear-ball)

Two [piecewise linear balls](#piecewise-linear-ball) of dimension three glued along a common [boundary](#boundary-of-a-set) [disk](#disk-mathematics) form another [piecewise linear ball](#piecewise-linear-ball). The [Schoenflies theorem](#schoenflies-theorem) identifies each [boundary](#boundary-of-a-set) pair with a [sphere](geometry-and-topology.md#sphere) and a hemisphere. Coning the resulting [boundary](#boundary-of-a-set) [homeomorphisms](#homeomorphism) extends them over the balls, which then become the two halves of a standard ball. The same argument shows that removing a ball attached along one [boundary](#boundary-of-a-set) [disk](#disk-mathematics) leaves a ball.

### 4-manifold

↑ **Parent:** [Topological manifold](#topological-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/4-manifold)

#### Smooth four-manifold

↑ **Parent:** [4-manifold](#4-manifold)

A smooth four-manifold is a four-dimensional [smooth manifold](differential-geometry.md#smooth-manifold). Its [intersection form](homology.md#intersection-form) and gauge-theoretic invariants impose strong constraints on its possible smooth and symplectic structures.

##### Fiber sum of four-manifolds

↑ **Parent:** [Smooth four-manifold](#smooth-four-manifold)

Remove [tubular neighborhoods](differential-geometry.md#tubular-neighborhood) of diffeomorphic embedded oriented surfaces with opposite normal Euler numbers, and glue their boundary circle bundles by a fiber-reversing identification. The resulting smooth [manifold](#topological-manifold) is a fiber sum. The square-zero case uses trivial [normal bundles](algebraic-geometry.md#normal-bundle). Additional symplectic hypotheses give a [symplectic fiber sum along a square-zero surface](symplectic-geometry.md#symplectic-fiber-sum-along-a-square-zero-surface).

###### Smooth fiber sum along unknotted null-homologous spheres

↑ **Parent:** [Fiber sum of four-manifolds](#fiber-sum-of-four-manifolds)

For standard unknotted [spheres](geometry-and-topology.md#sphere) contained in four-balls in $X$ and $Y$, the standard fiber-reversing gluing gives the displayed [connected sum](differential-geometry.md#connected-sum-of-oriented-manifolds). The complement of an unknotted $S^2\times D^2$ in $S^4$ is $S^1\times D^3$, and its double is $S^1\times S^3$. The portions of $X$ and $Y$ outside the four-balls remain as connected summands. Taking both ambient manifolds to be the [Complex projective plane](algebraic-topology.md#complex-projective-plane) gives a smooth fiber sum with no [symplectic form](symplectic-geometry.md#symplectic-form), by the [symplectic connected-sum obstruction](#symplectic-connected-sum-obstruction).

<h5 id="seiberg-witten-invariant-of-a-four-manifold">Seiberg–Witten invariant of a four-manifold</h5>

↑ **Parent:** [Smooth four-manifold](#smooth-four-manifold)

<h6 id="connected-sum-vanishing-of-the-seiberg-witten-invariant">Connected-sum vanishing of the Seiberg–Witten invariant</h6>

↑ **Parent:** [Seiberg–Witten invariant of a four-manifold](#seiberg-witten-invariant-of-a-four-manifold)

If a closed oriented [smooth four-manifold](#smooth-four-manifold) splits as a [connected sum](differential-geometry.md#connected-sum-of-oriented-manifolds) $X_1\#X_2$ with both $b_2^+(X_i)>0$, its ordinary [Seiberg–Witten invariants of a four-manifold](#seiberg-witten-invariant-of-a-four-manifold) vanish. Combined with [Taubes nonvanishing theorem](#taubes-nonvanishing-theorem), this obstructs a symplectic structure in that orientation.

###### Taubes nonvanishing theorem

↑ **Parent:** [Seiberg–Witten invariant of a four-manifold](#seiberg-witten-invariant-of-a-four-manifold)

A closed [symplectic manifold](symplectic-geometry.md#symplectic-manifold) of real dimension four with $b_2^+>1$ has a nonzero [Seiberg–Witten invariant of a four-manifold](#seiberg-witten-invariant-of-a-four-manifold) in its canonical structure, with value $\pm1$. The [positive index of the intersection form](homology.md#positive-index-of-the-intersection-form) hypothesis avoids chamber dependence. This provides the [symplectic connected-sum obstruction](#symplectic-connected-sum-obstruction).

[https://intlpress.com/site/pub/files/_fulltext/journals/mrl/1994/0001/0006/MRL-1994-0001-0006-a015.pdf](https://intlpress.com/site/pub/files/_fulltext/journals/mrl/1994/0001/0006/MRL-1994-0001-0006-a015.pdf)

###### Symplectic connected-sum obstruction

↑ **Parent:** [Taubes nonvanishing theorem](#taubes-nonvanishing-theorem)

A closed [symplectic manifold](symplectic-geometry.md#symplectic-manifold) of real dimension four cannot be a [connected sum](differential-geometry.md#connected-sum-of-oriented-manifolds) of two oriented [smooth four-manifolds](#smooth-four-manifold) each with positive [positive index of the intersection form](homology.md#positive-index-of-the-intersection-form). The total $b_2^+$ exceeds one; [Taubes nonvanishing theorem](#taubes-nonvanishing-theorem) and [connected-sum vanishing of the Seiberg–Witten invariant](#connected-sum-vanishing-of-the-seiberg-witten-invariant) would force the same invariant to be both nonzero and zero.

[https://web.ma.utexas.edu/users/perutz/SFT6/SFT6.pdf](https://web.ma.utexas.edu/users/perutz/SFT6/SFT6.pdf)

### Double of a manifold

↑ **Parent:** [Topological manifold](#topological-manifold)

Glue two copies of a compact [manifold](#topological-manifold) along their boundaries to form its double. A collar gives the double a smooth structure when $W$ is smooth. Folding the copies onto $W$ gives a [retraction](#retraction); in particular, inclusion of either copy is injective on [homology](homology.md). For an oriented [manifold](#topological-manifold), use the opposite [orientation](algebraic-topology.md#orientation-of-a-simplex) on the second copy.

### Topological tripod

↑ **Parent:** [Topological manifold](#topological-manifold)

Three intervals joined at one endpoint form a [compact](#compact-space) [connected](geometry-and-topology.md#connected-space) metric space. It is [second countable](#second-countable-space), [Hausdorff](#hausdorff-space) and [paracompact](#paracompact-space), but is not a [topological manifold](#topological-manifold). At regular arm points a putative manifold has [dimension](vector-space.md#dimension-vector-space) one; deleting the junction from a small neighborhood instead gives three components, incompatible with an interval chart. This local obstruction precedes any question about a smooth structure.

### Invariance of domain

↑ **Parent:** [Topological manifold](#topological-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Invariance_of_domain)

[Invariance of domain](#invariance-of-domain) says that a [continuous map](#continuous-map) that is an [injective function](algebra.md#injective-function) between [topological manifolds](#topological-manifold) without boundary of the same dimension is an [open map](calculus.md#open-map). It is useful in the [Penrose singularity theorem](general-relativity.md#penrose-singularity-theorem): projecting a [compact](#compact-space) [achronal boundary](general-relativity.md#achronal-boundary) along timelike curves onto a [Cauchy hypersurface](general-relativity.md#cauchy-surface) gives a nonempty subset that is both [open](#open-set) and [closed](#closed-set), forcing that [connected](geometry-and-topology.md#connected-space) [Cauchy hypersurface](general-relativity.md#cauchy-surface) to be [compact](#compact-space).

### Lorentzian manifold

↑ **Parent:** [Topological manifold](#topological-manifold)

A smooth [manifold](#topological-manifold) carrying a [nondegenerate bilinear form](linear-algebra.md#nondegenerate-bilinear-form) on each [tangent space](differential-geometry.md#tangent-space), with one negative and all remaining positive [eigenvalues](linear-operator-theory.md#eigenvalue), or the overall reversed-sign convention. Its nonzero [null vectors](special-relativity.md#null-vector) have vanishing metric [quadratic form](linear-algebra.md#quadratic-form).

#### Metric signature

↑ **Parent:** [Lorentzian manifold](#lorentzian-manifold)

The [metric signature](#metric-signature) records the signs of the diagonalized nondegenerate [metric tensor](general-relativity.md#metric-tensor), equivalently its numbers of negative and positive directions. For a four-dimensional [Lorentzian manifold](#lorentzian-manifold), both $(-,+,+,+)$ and its overall negative convention are common. The numerical signs of contractions and component [Hodge star operator](differential-form.md#hodge-star-operator) identities must be consistent with that choice and the [orientation](algebraic-topology.md#orientation-of-a-simplex).

#### Spacelike submanifold

↑ **Parent:** [Lorentzian manifold](#lorentzian-manifold)

In [metric signature](#metric-signature) $(-,+,\ldots,+)$, a [spacelike submanifold](#spacelike-submanifold) of a [Lorentzian manifold](#lorentzian-manifold) has an induced [metric tensor](general-relativity.md#metric-tensor) defining a [positive-definite quadratic form](linear-algebra.md#positive-definite-quadratic-form). With the overall reversed [metric signature](#metric-signature), its induced [metric tensor](general-relativity.md#metric-tensor) instead has only negative [eigenvalues](linear-operator-theory.md#eigenvalue). The definition applies to any dimension: enclosing charge-integration surfaces in four dimensions are two-dimensional examples, whereas a spacelike [Cauchy hypersurface](general-relativity.md#cauchy-surface) in four dimensions is three-dimensional.

### Dimension of a manifold

↑ **Parent:** [Topological manifold](#topological-manifold)

A [topological manifold](#topological-manifold) has dimension $n$ when its [manifold charts](differential-geometry.md#manifold-chart) have coordinate domains open in $\mathbb R^n$. For a [smooth manifold](differential-geometry.md#smooth-manifold), each [tangent space](differential-geometry.md#tangent-space) has [dimension](vector-space.md#dimension-vector-space) $n$, and a [tangent bundle](fiber-bundle.md#tangent-bundle) has [vector bundle rank](fiber-bundle.md#rank-of-a-vector-bundle) $n$.

#### Codimension of a submanifold

↑ **Parent:** [Dimension of a manifold](#dimension-of-a-manifold)

The codimension is the difference between the [dimension of a manifold](#dimension-of-a-manifold) and that of its submanifold. For [complex submanifolds](complex-geometry.md#complex-submanifold), complex codimension one means real codimension two.

### Handle attachment

↑ **Parent:** [Topological manifold](#topological-manifold)

Attaching an index-$k$ handle to an $n$-dimensional [manifold with boundary](differential-geometry.md#manifold-with-boundary) glues $D^k\times D^{n-k}$ along $\partial D^k\times D^{n-k}$. The complementary $D^k\times\partial D^{n-k}$ replaces the attaching region in the boundary.

#### Four-handle

↑ **Parent:** [Handle attachment](#handle-attachment)

A four-handle is an index-four [handle](#handle). In a four-dimensional [handle decomposition](#handle-decomposition) it is a four-ball attached along its whole boundary, a [three-sphere](geometry-and-topology.md#three-sphere). It caps a spherical boundary component left by earlier [handle attachments](#handle-attachment).

#### Handle

↑ **Parent:** [Handle attachment](#handle-attachment)

An index-$\lambda$ [handle](#handle) in dimension $d$ is this product of [disks](#disk-mathematics), attached along $S^{\lambda-1}\times D^{d-\lambda}$. Its [core disk](#core-disk-of-a-handle) is $D^\lambda\times\{0\}$, and its [belt sphere](#belt-sphere) is $\{0\}\times S^{d-\lambda-1}$. The complementary boundary piece is $D^\lambda\times S^{d-\lambda-1}$. Crossing a [critical point](analysis.md#critical-point) in the [Morse handle-attachment theorem](differential-geometry.md#morse-handle-attachment-theorem) produces precisely this local change.

#### Surgery on a smooth manifold

↑ **Parent:** [Handle attachment](#handle-attachment)

A framed embedding of the left-hand region in an $m$-dimensional [manifold](#topological-manifold) specifies an index-$\lambda$ surgery. Remove its interior and glue the right-hand region along their common boundary $S^{\lambda-1}\times S^{m-\lambda}$. The [cobordism](geometry-and-topology.md#cobordism) realizing this change attaches an index-$\lambda$ [handle](#handle) of dimension $m+1$. On an oriented [surface](#topological-surface), index-two surgery cuts out an annular neighbourhood of a simple closed curve and caps its two boundary circles.

#### Zero-handle

↑ **Parent:** [Handle attachment](#handle-attachment)

A zero-handle in an $n$-dimensional [handle decomposition](#handle-decomposition) is $D^0\times D^n=D^n$. Its attaching region is empty, so it starts a connected component of the manifold. In dimension four it is a four-ball; adding [one-handles](#one-handle) and [two-handles](#two-handle) gives a four-dimensional handlebody with a two-dimensional CW spine.

#### Core disk of a handle

↑ **Parent:** [Handle attachment](#handle-attachment)

The core disk of a $k$-[handle attachment](#handle-attachment) $D^k\times D^{n-k}$ is $D^k\times\{0\}$. Together with its cap in the preceding stage, it often represents a [homology class](homology.md#homology-class); for a [surgery trace](knot-theory.md#surgery-trace), capped two-handle cores give the basis of its [surgery linking matrix](knot-theory.md#surgery-linking-matrix).

#### Handle decomposition

↑ **Parent:** [Handle attachment](#handle-attachment)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Handle_decomposition)

A handle decomposition builds an $n$-dimensional [manifold](#topological-manifold) by successively adjoining $D^h\times D^{n-h}$ along $S^{h-1}\times D^{n-h}$. The attaching data comprise an [attaching sphere](#attaching-sphere) and its [framing of an embedded sphere](algebraic-geometry.md#framing-of-an-embedded-sphere). Reading a decomposition backwards replaces index $h$ by index $n-h$ and interchanges its [attaching spheres](#attaching-sphere) and [belt spheres](#belt-sphere).

##### Critical level handle embedding

↑ **Parent:** [Handle decomposition](#handle-decomposition)

In a critical level [handle](#handle) embedding, the [handles](#handle) occur at distinct heights in an ambient product with the real line. Between consecutive heights, the [boundary](#boundary-of-a-set) of the already attached [handles](#handle) travels through a product [collar neighbourhood](differential-geometry.md#collar-neighbourhood). At a [handle](#handle) height the horizontal slice contains the [handle](#handle), attached to the incoming [boundary](#boundary-of-a-set) along its attaching region. This separates the local topology changes from the intervening product regions.

##### Zero-framed Hopf-link handle decomposition of the sphere product

↑ **Parent:** [Handle decomposition](#handle-decomposition)

Write each [sphere](geometry-and-topology.md#sphere) as two [disks](#disk-mathematics), $S^2=D_-^2\cup D_+^2$. In their product, $D_-^2\times D_-^2$ is a [zero-handle](#zero-handle); $D_+^2\times D_-^2$ and $D_-^2\times D_+^2$ are [two-handles](#two-handle). Their attaching circles are the core circles of the complementary solid tori in $\partial(D^2\times D^2)$, hence a [Hopf link](knot-theory.md#hopf-link). Constant normal directions from the disk factors give both components the zero [Seifert framing](knot-theory.md#seifert-framing). The remaining $D_+^2\times D_+^2$ is a four-handle. This product construction establishes the actual [diffeomorphism](geometry-and-topology.md#diffeomorphism) type, rather than relying on its [intersection form](homology.md#intersection-form) alone. The resulting intersection matrix is $\left(\begin{smallmatrix}0&1\\1&0\end{smallmatrix}\right)$.

##### Commutator handlebody of the torus

↑ **Parent:** [Handle decomposition](#handle-decomposition)

Attach two [one-handles](#one-handle) to a four-dimensional [zero-handle](#zero-handle), then a [two-handle](#two-handle) along the commutator of their generators with the product zero framing. The result is $T^2\times D^2$. Its spine is the usual cell structure of the [torus](#torus): one vertex, two one-cells, and a two-cell attached by $xyx^{-1}y^{-1}$. An embedded representative of its $H_2$ generator is obtained by taking a once-punctured torus carried by the two one-handles and capping its boundary by the core disk of the two-handle. It meets the relative co-core once and has self-intersection zero. The boundary is $T^3$, whose integral homology has ranks $1,3,3,1$.

##### Handle slide

↑ **Parent:** [Handle decomposition](#handle-decomposition)

A handle slide replaces the framed [attaching sphere](#attaching-sphere) of one handle by a [band sum](differential-geometry.md#band-sum) with a parallel copy of another handle of the same index. It changes the attaching data while preserving the diffeomorphism type of the resulting [manifold](#topological-manifold). On the handle incidence matrix it performs an elementary row operation, or a column operation when applied to the dual decomposition.

###### Handle-slide isolation of a cancelling pair

↑ **Parent:** [Handle slide](#handle-slide)

In the intermediate-index range, if an [attaching sphere](#attaching-sphere) $A_1$ meets a [belt sphere](#belt-sphere) $B_1$ at exactly one transverse point, [handle slides](#handle-slide) can remove the intersections of every other attaching sphere with $B_1$. The dual slides then remove the intersections of $A_1$ with the other belt spheres. Each move uses a band to the unique pivot sheet and a local isotopy removing the old and new intersections. If $m_{ji}=A_j\cdot B_i$ and $\delta=m_{11}=\pm1$, the remaining incidence block is $m_{ji}-m_{j1}m_{1i}/\delta$, the [Schur complement](linear-algebra.md#schur-complement) of the pivot. Extreme-index cases need separate hypotheses.

##### Belt sphere

↑ **Parent:** [Handle decomposition](#handle-decomposition)

The belt sphere of an index-$h$ handle is $\{0\}\times S^{n-h-1}$ in the boundary after attachment. It is the [attaching sphere](#attaching-sphere) of the dual index-$(n-h)$ handle. Its intersections with the [attaching spheres](#attaching-sphere) of later handles detect passages through this handle.

##### Attaching sphere

↑ **Parent:** [Handle decomposition](#handle-decomposition)

The attaching sphere of an index-$h$ handle $D^h\times D^{n-h}$ is $S^{h-1}\times\{0\}$ in the previous boundary. Its [framing of an embedded sphere](algebraic-geometry.md#framing-of-an-embedded-sphere) identifies a neighbourhood with $S^{h-1}\times D^{n-h}$ and specifies the [handle attachment](#handle-attachment).

#### Three-handle

↑ **Parent:** [Handle attachment](#handle-attachment)

#### Two-handle

↑ **Parent:** [Handle attachment](#handle-attachment)

#### One-handle

↑ **Parent:** [Handle attachment](#handle-attachment)

### 3-manifold

↑ **Parent:** [Topological manifold](#topological-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/3-manifold)

A three-manifold is a [topological manifold](#topological-manifold) locally modeled on $\mathbb R^3$, or on a half-space at its boundary.

#### Normal surface

↑ **Parent:** [3-manifold](#3-manifold)

Relative to a [triangulation](algebraic-topology.md#triangulation), a [normal surface](#normal-surface) meets every [tetrahedron](geometry-and-topology.md#tetrahedron) in disjoint normal [disks](#disk-mathematics): four types of triangles cutting off vertices and three types of quadrilaterals separating opposite pairs of edges. A normal [disk](#disk-mathematics) meets any edge at most once; its face arcs join distinct edges. Two different quadrilateral types cannot coexist in a [tetrahedron](geometry-and-topology.md#tetrahedron).

##### Normal surface coordinates

↑ **Parent:** [Normal surface](#normal-surface)

For $t$ [tetrahedra](geometry-and-topology.md#tetrahedron), count the seven [disk](#disk-mathematics) types in each [tetrahedron](geometry-and-topology.md#tetrahedron). Across each glued face the counts of each of its three normal arc types must agree. These are homogeneous [linear equations](linear-algebra.md#linear-equation) with integer coefficients. An admissible solution also has at most one nonzero quadrilateral type in each [tetrahedron](geometry-and-topology.md#tetrahedron). Matching the arcs in their [boundary](#boundary-of-a-set) order reconstructs the [normal surface](#normal-surface) up to an [isotopy](differential-geometry.md#isotopy) preserving the [tetrahedra](geometry-and-topology.md#tetrahedron).

###### Normal surface weight

↑ **Parent:** [Normal surface coordinates](#normal-surface-coordinates)

The weight of a [normal surface](#normal-surface) counts its intersections with the edges of the [triangulation](algebraic-topology.md#triangulation). It is a positive linear function of its coordinates: each corner of a normal [disk](#disk-mathematics) contributes the reciprocal of the number of tetrahedral sectors around its edge. Thus a nontrivial decomposition into compatible coordinate vectors gives both summands strictly smaller weight.

###### Haken sum

↑ **Parent:** [Normal surface coordinates](#normal-surface-coordinates)

The Haken sum of compatible [normal surfaces](#normal-surface) is obtained by resolving their intersection curves in the way that preserves the normal [disk](#disk-mathematics) types. It adds [normal surface coordinates](#normal-surface-coordinates), [Euler characteristic](homology.md#euler-characteristic) and mod-two [homology](homology.md) classes. The alternative local resolution can create returning face arcs and need not be normal.

###### Fundamental normal surface

↑ **Parent:** [Normal surface coordinates](#normal-surface-coordinates)

A fundamental [normal surface](#normal-surface) has a nonzero admissible coordinate vector which is not the sum of two nonzero admissible vectors. Fixing the allowed quadrilateral type in every [tetrahedron](geometry-and-topology.md#tetrahedron) reduces the problem to the [Hilbert basis of a rational cone](toric-geometry.md#hilbert-basis-of-a-rational-cone). There are finitely many choices of quadrilateral types and finitely many indecomposable vectors for each choice.

#### Punctured three-sphere

↑ **Parent:** [3-manifold](#3-manifold)

A punctured three-sphere is $S^3$ with the interiors of finitely many disjoint [piecewise linear balls](#piecewise-linear-ball) removed. Capping its spherical [boundary](#boundary-of-a-set) components with balls restores $S^3$. Removing another ball or gluing two such manifolds along one spherical [boundary](#boundary-of-a-set) component preserves this class.

##### Sphere surgery preserving nontrivial complementary pieces

↑ **Parent:** [Punctured three-sphere](#punctured-three-sphere)

Suppose disjoint separating [spheres](geometry-and-topology.md#sphere) cut a [3-manifold](#3-manifold) into pieces none of which is a [punctured three-sphere](#punctured-three-sphere). Compress one [sphere](geometry-and-topology.md#sphere) along a [disk](#disk-mathematics) disjoint from the others. The old [sphere](geometry-and-topology.md#sphere) and the two new [spheres](geometry-and-topology.md#sphere) enclose a three-times punctured [sphere](geometry-and-topology.md#sphere). At least one of the two pieces on the compressed side is not a punctured [sphere](geometry-and-topology.md#sphere); retain that new [sphere](geometry-and-topology.md#sphere) and discard the other. The piece on its opposite side cannot become a punctured [sphere](geometry-and-topology.md#sphere), since capping its boundaries and applying the [Three-dimensional Schoenflies theorem](#three-dimensional-schoenflies-theorem) would make the original opposite piece a punctured [sphere](geometry-and-topology.md#sphere) as well. Hence the number of [spheres](geometry-and-topology.md#sphere) and the nontriviality condition can be preserved.

#### Three-ball

↑ **Parent:** [3-manifold](#3-manifold)

A three-ball is a [three-manifold](#3-manifold) [homeomorphic](#local-homeomorphism) to the closed unit [ball](topological-analysis.md#ball-mathematics) in $\mathbb R^3$. Its [boundary](#boundary-of-a-set) is a [two-sphere](geometry-and-topology.md#two-sphere). Attaching a three-ball to a spherical boundary component is called capping that boundary; marked endpoints may be joined by a straight arc inside the cap.

<h4 id="poincare-conjecture">Poincaré conjecture</h4>

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincaré_conjecture)

A closed [simply connected](algebraic-topology.md#simply-connected-space) [three-manifold](#3-manifold) is homeomorphic to the [three-sphere](geometry-and-topology.md#three-sphere). Now a theorem, this identifies every [homotopy](algebraic-topology.md#homotopy) [three-sphere](geometry-and-topology.md#three-sphere) with the standard sphere and removes homotopy-sphere ambiguities in three-dimensional connected-sum classification. Smooth structures are also unique in dimension three.

#### Loop theorem

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loop_theorem)

If a boundary surface inclusion has noninjective [fundamental group](algebraic-topology.md#fundamental-group) map, there is a [compression disk](#compression-disk) whose boundary represents a nontrivial element of that kernel. More generally the boundary can be required to avoid a prescribed normal subgroup if a singular disk with that property exists.

##### Tower proof of the loop theorem

↑ **Parent:** [Loop theorem](#loop-theorem)

Start with a singular [disk](#disk-mathematics) whose [boundary](#boundary-of-a-set) represents a prescribed nontrivial class in a [boundary](#boundary-of-a-set) subsurface. Repeatedly lift it through double [covering spaces](algebraic-topology.md#covering-space) of regular neighbourhoods of its image. The number of distinct image [simplexes](algebraic-topology.md#simplex) strictly increases and is bounded by the number of domain [simplexes](algebraic-topology.md#simplex), so the tower ends. At the top, vanishing first mod-two [homology](homology.md) forces every [boundary](#boundary-of-a-set) component to be a [sphere](geometry-and-topology.md#sphere). An embedded [disk](#disk-mathematics) can then be constructed and projected down the tower. Resolving double curves preserves a [boundary](#boundary-of-a-set) class outside a chosen [normal subgroup](group-theory.md#normal-subgroup), giving an embedded compression [disk](#disk-mathematics) at the bottom.

<h5 id="dehn-s-lemma">Dehn's lemma</h5>

↑ **Parent:** [Loop theorem](#loop-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dehn's_lemma)

A simple closed curve on the boundary of a [three-manifold](#3-manifold) which is nullhomotopic in the manifold bounds a properly embedded disk. The boundary curve is retained; the [Loop theorem](#loop-theorem) can instead find a different simple essential curve in a nontrivial kernel.

#### Sphere theorem for three-manifolds

↑ **Parent:** [3-manifold](#3-manifold)

If an orientable [three-manifold](#3-manifold) has nonzero $\pi_2$, it contains an embedded essential two-sphere. Consequently a closed orientable [irreducible three-manifold](#irreducible-three-manifold) with infinite fundamental group is [aspherical](algebraic-topology.md#aspherical-space): its simply connected noncompact universal cover has zero second homotopy and top ordinary homology, hence is acyclic and contractible by the [Hurewicz theorem](algebraic-topology.md#hurewicz-theorem) and [Whitehead theorem](algebraic-topology.md#whitehead-theorem).

#### Hyperbolic three-manifold

↑ **Parent:** [3-manifold](#3-manifold)

A complete hyperbolic three-manifold is a complete [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) of dimension three with constant [sectional curvature](second-fundamental-form.md#sectional-curvature) $-1$. Its [universal cover](algebraic-topology.md#universal-cover) is [hyperbolic space](geometry-and-topology.md#hyperbolic-space) $\mathbb H^3$ and its deck group acts freely and discretely by [Riemannian isometries](differential-geometry.md#riemannian-isometry). In the orientable case it is a torsion-free [Kleinian group](topological-group.md#kleinian-group).

##### Mostow rigidity theorem

↑ **Parent:** [Hyperbolic three-manifold](#hyperbolic-three-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mostow_rigidity_theorem)

For complete finite-volume [hyperbolic space](geometry-and-topology.md#hyperbolic-space) manifolds of dimension at least three, an isomorphism of [fundamental groups](algebraic-topology.md#fundamental-group) is induced, up to the usual basepoint-path choice, by a unique hyperbolic [isometry](riemannian-geometry.md#isometry). The finite-volume noncompact case includes the Prasad extension. Thus complete hyperbolic metrics on a fixed finite-volume three-manifold have no deformation moduli, unlike metrics on closed hyperbolic surfaces.

#### Three-dimensional Schoenflies theorem

↑ **Parent:** [3-manifold](#3-manifold)

A smooth, piecewise-linear or locally flat embedded two-sphere in the [three-sphere](geometry-and-topology.md#three-sphere) has two complementary components, each with closure homeomorphic to a three-ball. Equivalently a tame embedded two-sphere in $\mathbb R^3$ bounds a ball on its compact side. Local flatness is essential; arbitrary wild sphere embeddings are excluded.

#### Geometrizable three-manifold

↑ **Parent:** [3-manifold](#3-manifold)

A closed orientable [three-manifold](#3-manifold) is geometrizable if its prime summands can be split along finitely many disjoint essential [tori](#torus) into pieces whose interiors carry complete geometric structures modeled on the eight [Thurston geometries](#thurston-geometry). Prime decomposition and capping sphere boundaries precede the torus cuts; a single homogeneous geometry on the original connected sum is not required.

##### Geometrization conjecture

↑ **Parent:** [Geometrizable three-manifold](#geometrizable-three-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometrization_conjecture)

Every closed orientable [three-manifold](#3-manifold) admits a prime and [torus](#torus) decomposition into pieces modeled on the eight [Thurston geometries](#thurston-geometry). In particular, a closed irreducible orientable [three-manifold](#3-manifold) with [fundamental group](algebraic-topology.md#fundamental-group) $\mathbb Z^3$ carries a flat metric. The [Bieberbach theorem](second-fundamental-form.md#bieberbach-theorem) then identifies it with the three-torus because an abelian crystallographic group has trivial linear holonomy. [Simply connected](algebraic-topology.md#simply-connected-space) closed [three-manifolds](#3-manifold) are three-spheres by the [Poincaré conjecture](#poincare-conjecture).

##### Thurston geometry

↑ **Parent:** [Geometrizable three-manifold](#geometrizable-three-manifold)

The eight simply connected three-dimensional homogeneous model geometries are $S^3$, $\mathbb R^3$, $\mathbb H^3$, $S^2\times\mathbb R$, $\mathbb H^2\times\mathbb R$, $\widetilde{\operatorname{SL}}_2(\mathbb R)$, $\mathrm{Nil}$ and $\mathrm{Sol}$. A geometric structure is a locally homogeneous structure obtained as a quotient of a model by a discrete freely acting isometry group, equivalently with compatible model charts.

#### Prime three-manifold

↑ **Parent:** [3-manifold](#3-manifold)

A closed connected [orientable smooth manifold](differential-geometry.md#orientable-smooth-manifold) of dimension three is prime when a decomposition as a [connected sum](differential-geometry.md#connected-sum-of-oriented-manifolds) forces at least one summand to be the [three-sphere](geometry-and-topology.md#three-sphere). Unlike an [irreducible three-manifold](#irreducible-three-manifold), it may contain a nonseparating embedded two-sphere.

##### Prime decomposition of a closed orientable three-manifold

↑ **Parent:** [Prime three-manifold](#prime-three-manifold)

Every closed connected orientable [three-manifold](#3-manifold) is a finite [connected sum](differential-geometry.md#connected-sum-of-oriented-manifolds) of [prime three-manifolds](#prime-three-manifold), unique up to order and the insertion of three-sphere factors. The corresponding [fundamental group](algebraic-topology.md#fundamental-group) is the free product of the summand groups. A prime orientable three-manifold is either irreducible or $S^2\times S^1$; this separates aspherical infinite-group cases from the infinite cyclic case.

##### Nonseparating sphere gives a sphere-circle summand

↑ **Parent:** [Prime three-manifold](#prime-three-manifold)

In an orientable [three-manifold](#3-manifold), an embedded nonseparating two-sphere has a product neighborhood. Join its two boundary spheres by an arc outside that neighborhood and take a regular neighborhood of the union. This region is $S^2\times S^1$ with an open ball removed. Its boundary sphere exhibits the displayed [connected sum](differential-geometry.md#connected-sum-of-oriented-manifolds). Consequently a prime but nonirreducible orientable [three-manifold](#3-manifold) is $S^2\times S^1$.

#### Boundary-irreducible three-manifold

↑ **Parent:** [3-manifold](#3-manifold)

A compact [three-manifold](#3-manifold) is boundary-irreducible when there is no embedded disk with interior in the manifold and boundary an essential curve in its boundary. Thus its boundary has no compressing disk.

#### Irreducible three-manifold

↑ **Parent:** [3-manifold](#3-manifold)

An orientable [three-manifold](#3-manifold) is irreducible if every embedded two-sphere bounds a three-ball. This makes innermost-disk simplifications of embedded [topological surfaces](#topological-surface) possible without changing the ambient [three-manifold](#3-manifold).

#### Excellent three-manifold

↑ **Parent:** [3-manifold](#3-manifold)

In the orientable case an excellent compact three-manifold is an [irreducible three-manifold](#irreducible-three-manifold) and a [boundary-irreducible three-manifold](#boundary-irreducible-three-manifold), is not a ball, contains a two-sided properly embedded [incompressible surface](#incompressible-surface), and has every properly embedded incompressible zero-[Euler characteristic](homology.md#euler-characteristic) surface a [boundary-parallel surface](#boundary-parallel-surface). In particular it has no essential [annulus](#annulus-mathematics) or [torus](#torus). These properties give lower bounds on the [Thurston norm](#thurston-norm) of classes with essential boundary.

##### Excellent knot representative theorem

↑ **Parent:** [Excellent three-manifold](#excellent-three-manifold)

In a compact connected orientable [three-manifold](#3-manifold) with no spherical boundary components, every embedded [knot](knot-theory.md#knot) is homotopic to a [knot](knot-theory.md#knot) with an [excellent three-manifold](#excellent-three-manifold) as exterior. In particular this can preserve the generator class in $S^1\times S^2$, or the [winding number of a satellite pattern](knot-theory.md#winding-number-of-a-satellite-pattern) one class in a [solid torus](#solid-torus). Homotopy here is weaker than [isotopy](differential-geometry.md#isotopy).

#### Thurston norm

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thurston_norm)

For a compact oriented [three-manifold](#3-manifold), the integral relative class $u$ has norm the minimum of $\chi_-(F)=\sum_j\max(0,-\chi(F_j))$ over properly embedded oriented [topological surfaces](#topological-surface) representing $u$. Homogeneity and continuity extend it to real [relative homology](homology.md#relative-homology). It is a [seminorm](topological-vector-space.md#seminorm), since spheres, disks, [annuli](#annulus-mathematics) and [tori](#torus) have zero cost.

##### Thurston norm of a pair-of-pants product

↑ **Parent:** [Thurston norm](#thurston-norm)

For $Y=P\times S^1$ with $P$ a [pair of pants](#pair-of-pants-mathematics) and $h$ its circle fiber, a [horizontal surface in a Seifert fibered space](knot-theory.md#horizontal-surface-in-a-seifert-fibered-space) of degree $d$ has $\chi_- = |d|$; [vertical surfaces in a Seifert fibered space](knot-theory.md#vertical-surface-in-a-seifert-fibered-space) have zero cost. Cutting and pasting these representatives, and classifying essential surfaces, proves $\|u\|_T=|u\cdot h|$. The [dual Thurston polytope](#dual-thurston-polytope) is therefore the segment between the two functionals $\pm h$ under the natural pairing.

##### Thurston norm gluing along an incompressible torus

↑ **Parent:** [Thurston norm](#thurston-norm)

In an irreducible [three-manifold](#3-manifold) with incompressible boundary, a minimizing surface can be cut along a separating incompressible [torus](#torus) after removing inessential intersection circles. The essential pieces have no disk or sphere components, so their $\chi_-$ costs add. Minimizing independently in the pieces and gluing their matching boundary curves gives the corresponding upper bound. This allows [Thurston norm](#thurston-norm) calculations for [satellite knots](knot-theory.md#satellite-knot).

##### Dual Thurston polytope

↑ **Parent:** [Thurston norm](#thurston-norm)

The dual polytope consists of the real linear functionals $\alpha$ on $H_2(Y,\partial Y;\mathbb R)$ such that $|\alpha(u)|\leq\|u\|_T$ for every $u$. Thus it is the polar of the unit ball of the [Thurston norm](#thurston-norm) and annihilates that [seminorm](topological-vector-space.md#seminorm)'s kernel.

#### Incompressible surface

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Incompressible_surface)

An incompressible surface is a properly embedded two-sided [topological surface](#topological-surface) with no compressing disk, subject to the usual exclusion of inessential spherical components. A compressing disk has boundary an essential closed curve on the [topological surface](#topological-surface) and interior disjoint from it.

##### Three-manifold hierarchy

↑ **Parent:** [Incompressible surface](#incompressible-surface)

A hierarchy is a finite sequence of cuts along properly embedded two-sided [incompressible surfaces](#incompressible-surface), without spherical components, ending in disjoint three-balls. [Disks](#disk-mathematics) are allowed. For an ambient manifold which is not [orientable](differential-geometry.md#orientable-surface) the two-sided cutting [surfaces](#topological-surface) need not themselves be [orientable](differential-geometry.md#orientable-surface). The existence of a hierarchy does not imply that every choice of incompressible cuts terminates.

###### Relative boundary rigidity from a hierarchy

↑ **Parent:** [Three-manifold hierarchy](#three-manifold-hierarchy)

A map between [compact](#compact-space) [connected](geometry-and-topology.md#connected-space) [orientable](differential-geometry.md#orientable-surface) irreducible [3-manifolds](#3-manifold) with nonempty boundaries, [injective](algebra.md#injective-function) on the [boundary](#boundary-of-a-set) and on the [fundamental group](algebraic-topology.md#fundamental-group), is [homotopic](algebraic-topology.md#homotopy) to a [homeomorphism](#homeomorphism) relative to the [boundary](#boundary-of-a-set). The [boundary](#boundary-of-a-set) determines degree $\pm1$, and the cover corresponding to the image of the [fundamental group](algebraic-topology.md#fundamental-group) consequently has one sheet. Straighten the preimage of an incompressible hierarchy [surface](#topological-surface), cut both manifolds, and repeat. At the terminal balls, extend the prescribed [boundary](#boundary-of-a-set) [homeomorphisms](#homeomorphism) by coning. The [homotopies](algebraic-topology.md#homotopy) and [homeomorphisms](#homeomorphism) glue across the straightened [surface](#topological-surface) collars.

###### Asphericity from a three-manifold hierarchy

↑ **Parent:** [Three-manifold hierarchy](#three-manifold-hierarchy)

In an [orientable](differential-geometry.md#orientable-surface) [irreducible three-manifold](#irreducible-three-manifold), an incompressible cut is [fundamental group](algebraic-topology.md#fundamental-group)-injective by the [Loop theorem](#loop-theorem). Lift a [three-manifold hierarchy](#three-manifold-hierarchy) to the [universal cover](algebraic-topology.md#universal-cover). The terminal ball pieces are [contractible](algebraic-topology.md#contractible-space) and their gluing [surfaces](#topological-surface) have [contractible](algebraic-topology.md#contractible-space) universal covers. The incidence graph is a tree, by the [van Kampen theorem](algebraic-topology.md#seifert-van-kampen-theorem) normal form for successive cuts. Finite subtrees are [contractible](algebraic-topology.md#contractible-space) by successively attaching a terminal piece along a [contractible](algebraic-topology.md#contractible-space) intersection. Every [sphere](geometry-and-topology.md#sphere) map has [compact](#compact-space) image contained in a finite subtree, so all higher [homotopy groups](algebraic-topology.md#homotopy-group) of the [universal cover](algebraic-topology.md#universal-cover) vanish.

###### Self-reproducing incompressible annulus cut

↑ **Parent:** [Three-manifold hierarchy](#three-manifold-hierarchy)

Let $P$ be a once-punctured [torus](#torus) and let $c$ be a nonseparating essential curve. The [annulus](#annulus-mathematics) $c\times[0,1]$ is an [incompressible surface](#incompressible-surface) in $P\times[0,1]$. Cutting gives a [pair of pants](#pair-of-pants-mathematics) times an interval. Both products are genus-two [handlebodies](#handlebody), since a [compact](#compact-space) [connected](geometry-and-topology.md#connected-space) [surface](#topological-surface) with [boundary](#boundary-of-a-set) times an interval is a handlebody of [genus](#genus-of-a-surface) $1-\chi(P)$.

##### Compression disk

↑ **Parent:** [Incompressible surface](#incompressible-surface)

A compression disk for a two-sided embedded [surface](#topological-surface) $F$ in a [three-manifold](#3-manifold) is an embedded disk meeting $F$ exactly in its boundary, with boundary essential in $F$. Replacing an annular neighborhood of this boundary by two parallel copies of the disk reduces the surface's genus or separates it into simpler pieces.

##### Boundary-parallel surface

↑ **Parent:** [Incompressible surface](#incompressible-surface)

A properly embedded [topological surface](#topological-surface) is boundary-parallel if it cobounds a product region with a [topological surface](#topological-surface) in the ambient boundary, with the remaining boundary of that product contained in the ambient boundary. An [annulus](#annulus-mathematics) parallel into one boundary component has zero net oriented boundary class on that component.

##### Classification of incompressible surfaces in Seifert fibered spaces

↑ **Parent:** [Incompressible surface](#incompressible-surface)

In an orientable irreducible [Seifert fibered space](knot-theory.md#seifert-fibered-space), an essential two-sided [incompressible surface](#incompressible-surface) that is also a [boundary-incompressible surface](#boundary-incompressible-surface) can be isotoped to a [horizontal surface in a Seifert fibered space](knot-theory.md#horizontal-surface-in-a-seifert-fibered-space) or a [vertical surface in a Seifert fibered space](knot-theory.md#vertical-surface-in-a-seifert-fibered-space).

##### Boundary-incompressible surface

↑ **Parent:** [Incompressible surface](#incompressible-surface)

A properly embedded [topological surface](#topological-surface) is boundary-incompressible when no disk in the ambient [three-manifold](#3-manifold) joins an essential arc on the [topological surface](#topological-surface) to an arc on the ambient boundary, with the disk's interior disjoint from both.

#### Heegaard splitting

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heegaard_splitting)

A Heegaard splitting divides a closed [three-manifold](#3-manifold) into two [handlebodies](#handlebody) with common boundary. For a [three-manifold](#3-manifold) with boundary, one uses compression bodies, which can retain negative boundary components.

##### Common nonseparating disks in a Heegaard splitting

↑ **Parent:** [Heegaard splitting](#heegaard-splitting)

Two nonseparating compressing disks on opposite sides with the same boundary form an embedded sphere. Cutting each [handlebody](#handlebody) along its disk leaves it connected, so the sphere is nonseparating in the glued [three-manifold](#3-manifold). Capping the two resulting sphere boundaries gives a splitting of one lower genus of the remaining summand; the removed summand is $S^1\times S^2$.

##### Heegaard genus

↑ **Parent:** [Heegaard splitting](#heegaard-splitting)

The least genus of a [Heegaard surface](#heegaard-surface) among all [Heegaard splittings](#heegaard-splitting) of a closed orientable [three-manifold](#3-manifold). Having a splitting of genus $g$ only proves $g_H(M)\le g$; stabilization supplies larger-genus splittings of the same manifold.

##### Heegaard Floer homology

↑ **Parent:** [Heegaard splitting](#heegaard-splitting)

Heegaard Floer homology assigns groups $HF^\circ(Y,\mathfrak s)$ to a closed oriented three-manifold with a [Spin-c structure](riemannian-geometry.md#spin-c-structure). A pointed [Heegaard diagram](#heegaard-diagram) of genus $g$ gives product [Lagrangian tori](symplectic-geometry.md#lagrangian-torus) $\mathbb T_\alpha,\mathbb T_\beta\subset\operatorname{Sym}^g(\Sigma)$; the [chain complex](homology.md#chain-complex) is generated by their intersection points and its differential counts [Whitney disk classes](#whitney-disk-class) represented by holomorphic disks. The minus, infinity, plus and hat versions use different powers or quotients of the variable $U$. The [Heegaard Floer cobordism maps](#heegaard-floer-cobordism-map) and the [Mixed Heegaard Floer invariant](#mixed-heegaard-floer-invariant) relate these groups to smooth four-dimensional topology.

###### Mixed Heegaard Floer invariant

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

###### Integer-surgery exact triangle in Heegaard Floer homology

↑ **Parent:** [Heegaard Floer homology](#heegaard-floer-homology)

For a knot $K$ in an integral homology three-sphere and $n>0$, fix a [Spin-c structure](riemannian-geometry.md#spin-c-structure) $\mathfrak t_k$ on the $n$-surgery. Write $\mathfrak s_i$ for structures on zero-surgery with $\langle c_1(\mathfrak s_i),[\widehat F]\rangle=2i$, using a capped Seifert surface. In compatible labels the completed-minus triangle is

$$
\cdots\longrightarrow\mathbf{HF}^-(Y)\longrightarrow\bigoplus_{i\equiv k\ (\mathrm{mod}\ n)}\mathbf{HF}^-(Y_0,\mathfrak s_i)\longrightarrow\mathbf{HF}^-(Y_n,\mathfrak t_k)\longrightarrow\mathbf{HF}^-(Y)\longrightarrow\cdots.
$$

One can equally use the plus theory without completing. The first map is the congruence-restricted zero-surgery trace map; the last is the sum of reverse, orientation-reversed $n$-surgery trace maps. The middle map uses a Heegaard triple with an auxiliary lens-space generator. For $n=1$ that lens space is $S^3$, giving the usual three two-ended cobordism maps. For $n>1$ it is important to retain the auxiliary boundary and its fixed Spin-c structure. The [U-adic completion of Heegaard Floer homology](#u-adic-completion-of-heegaard-floer-homology) makes the sums of maps well-defined.

###### Heegaard Floer cobordism map

↑ **Parent:** [Heegaard Floer homology](#heegaard-floer-homology)

A smooth oriented [cobordism](geometry-and-topology.md#cobordism) $W:Y_1\to Y_2$ with a [Spin-c structure](riemannian-geometry.md#spin-c-structure) induces $U$-equivariant maps $F^\circ_{W,\mathfrak s}$ on the corresponding [Heegaard Floer homology](#heegaard-floer-homology) groups. A [handle decomposition](#handle-decomposition) defines the maps using generator selection for one- and three-handles and holomorphic triangle counts for two-handles. Composition sums over extensions of the prescribed Spin-c structures. When the boundary determinant classes are torsion, the absolute grading shift is

$$
\Delta(W,\mathfrak s)=\frac{c_1(\mathfrak s)^2-2\chi(W)-3\sigma(W)}4.
$$

The square is defined using the rational relative lift. If $b_2^+(W)>0$, the infinity map vanishes. Between rational homology spheres, when $b_1(W)=b_2^+(W)=0$, the infinity map is an isomorphism of Laurent towers.

###### Admissible cut for a Heegaard Floer mixed map

↑ **Parent:** [Heegaard Floer cobordism map](#heegaard-floer-cobordism-map)

An admissible cut splits a four-dimensional [cobordism](geometry-and-topology.md#cobordism) as $W=W_1\cup_N W_2$, with $b_2^+(W_1),b_2^+(W_2)>0$, and with the Mayer-Vietoris connecting map $H^1(N;\mathbb Z)\to H^2(W;\mathbb Z)$ equal to zero. The last condition removes the ambiguity in gluing [Spin-c structures](riemannian-geometry.md#spin-c-structure) on the two pieces. Positivity makes both infinity cobordism maps vanish, allowing passage through the [Reduced Heegaard Floer homology](#reduced-heegaard-floer-homology) of $N$. A useful cut is the boundary of a neighborhood of a positive-square embedded surface, chosen so that its complement still has a positive direction. The nonzero normal Euler number makes $H^1$ of the neighborhood surject onto $H^1$ of its boundary, proving the connecting-map condition.

###### Variants of Heegaard Floer homology

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

###### Heegaard Floer chain complex

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

An embedded positive domain which is a bigon or rectangle, has convex alternating alpha and beta corners, and contains no other selected coordinate in its interior, has [Maslov index](symplectic-geometry.md#maslov-index) one. A bigon has Euler measure $1/2$ and two corner averages $1/4$; a rectangle has Euler measure zero and four corner averages $1/4$. For the usual regular complex structure, its holomorphic disk count modulo translation is $\pm1$. For a bigon the Riemann map to the strip is unique up to translation. For a rectangle, the tautological correspondence represents the disk in the [symmetric product](#symmetric-product) by a branched double cover of the strip onto the rectangular domain: its conformal modulus fixes the branch parameter, and the only remaining freedom is translation. The resulting isolated regular disk gives one point in the oriented moduli space. The differential coefficient is $\pm U^{n_z}$, so a basepoint-free domain contributes a unit.

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

For intersection generators $\mathbf x,\mathbf y$, a Whitney disk is a map of a disk into the [symmetric product](#symmetric-product), with its two boundary semicircles mapped to the two product tori and its endpoints mapped to $\mathbf x,\mathbf y$. Its homotopy class belongs to $\pi_2(\mathbf x,\mathbf y)$. Projecting it to the [Heegaard surface](#heegaard-surface) gives an integral domain. With the surface oriented, the convention is $\partial_\alpha D=\mathbf y-\mathbf x$. The obstruction to a disk is the class $\epsilon(\mathbf x,\mathbf y)\in H_1(Y)$ obtained by joining the points along alpha arcs and returning along beta arcs. In the Heegaard Floer setup, its vanishing is equivalent to equality of the generators' [Spin-c structures](riemannian-geometry.md#spin-c-structure); for the rational homology sphere diagrams this is equivalent to $\pi_2(\mathbf x,\mathbf y)\ne\varnothing$.

##### Compression body

↑ **Parent:** [Heegaard splitting](#heegaard-splitting)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compression_body)

A compression body is obtained from a product $F\times I$ by attaching [one-handles](#one-handle) to $F\times\{1\}$, allowing three-ball components as well. Its negative boundary is the retained copy of $F$ and its positive boundary is the other boundary component. A [handlebody](#handlebody) has empty negative boundary.

##### Heegaard surface

↑ **Parent:** [Heegaard splitting](#heegaard-splitting)

The Heegaard surface is the common positive boundary of the two pieces in a [Heegaard splitting](#heegaard-splitting).

###### Heegaard diagram

↑ **Parent:** [Heegaard surface](#heegaard-surface)

A Heegaard diagram marks the boundaries of compressing disks from the two sides of a [Heegaard surface](#heegaard-surface). Attaching [two-handles](#two-handle) along the two collections, and capping resulting spherical boundary components, reconstructs the [three-manifold](#3-manifold).

###### Generalized Heegaard diagram

↑ **Parent:** [Heegaard diagram](#heegaard-diagram)

A generalized [Heegaard diagram](#heegaard-diagram) permits [compression bodies](#compression-body) and a nonempty negative boundary. Equivalently, a suitable [handlebody](#handlebody) with [two-handles](#two-handle) attached along only part of a compressing system can retain torus boundary components. Disk crossings supply generators and attaching-curve words supply relators for its [fundamental group](algebraic-topology.md#fundamental-group).

###### Dehn presentation Heegaard diagram

↑ **Parent:** [Heegaard diagram](#heegaard-diagram)

Thicken the planar graph underlying a [knot diagram](knot-theory.md#knot-diagram). Its boundary supports a [Heegaard diagram](#heegaard-diagram) with face disks on one side and crossing-tunnel disks on the other. The face generators and crossing curves give a [Dehn presentation of a knot group](knot-theory.md#dehn-presentation-of-a-knot-group).

#### Handlebody

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Handlebody)

A genus-$g$ handlebody is a three-ball with $g$ [one-handles](#one-handle) attached. Its boundary is a closed orientable [topological surface](#topological-surface) of [genus](#genus-of-a-surface) $g$.

#### Thurston elliptization conjecture

↑ **Parent:** [3-manifold](#3-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thurston_elliptization_conjecture)

Every connected closed orientable [three-manifold](#3-manifold) with finite [fundamental group](algebraic-topology.md#fundamental-group) admits spherical geometry. With cyclic [fundamental group](algebraic-topology.md#fundamental-group), it is a [lens space](knot-theory.md#lens-space).

### Homology above the dimension of a manifold

↑ **Parent:** [Topological manifold](#topological-manifold)

An $n$-manifold has zero singular homology in every degree greater than $n$. One proof uses a countable exhaustion by subsets that retract onto $n$-dimensional CW complexes and the compact support of every singular cycle.

## Closed set

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed_set)

A closed set contains all its [limit points](#limit-point); equivalently, its complement is [open](#open-set).

### Sequentially closed set

↑ **Parent:** [Closed set](#closed-set)

A [sequentially closed set](#sequentially-closed-set) is one that contains every limit of its convergent sequences. This is weaker than being a [closed set](#closed-set) in a general [topological space](#topological-space), but the two conditions agree in [metric spaces](topological-analysis.md#metric-space).

### Limit point

↑ **Parent:** [Closed set](#closed-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Limit_point)

A limit point of a set is a point whose every neighbourhood contains a different point of the set.

## Closure (topology)

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closure_(topology))

The closure of a subset is the smallest closed set containing it, equivalently the set of points whose every neighbourhood meets it.

### Adherent point

↑ **Parent:** [Closure (topology)](#closure-topology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Adherent_point)

An adherent point of $A$ is a point whose every [neighbourhood](#neighbourhood-mathematics) meets $A$. The set of adherent points is the [closure](#closure-topology) of $A$. This includes all points of $A$, even isolated ones; a [limit point](#limit-point) in the accumulation-point convention instead requires each neighbourhood to meet $A\setminus\{x\}$.

## Interior (topology)

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interior_(topology))

The interior of a subset $A$ of a [topological space](#topological-space) is the union of all [open sets](#open-set) contained in $A$, equivalently the largest open subset of $A$.

## Topological space

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_space)

A topological space is a set together with a family of open subsets containing the empty set and the whole set and closed under arbitrary unions and finite intersections.

### Open and closed maps

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Open_and_closed_maps)

An [open map](calculus.md#open-map) sends each [open set](#open-set) to an [open set](#open-set); a closed map sends each [closed set](#closed-set) to a [closed set](#closed-set). These properties concern images, whereas [continuity](calculus.md#continuous-function) concerns inverse images of open sets. Neither openness nor closedness alone implies continuity.

### Stratified space

↑ **Parent:** [Topological space](#topological-space)

A space partitioned into [manifold](#topological-manifold) strata, with a locally finite frontier-compatible partition. In the conical setting, a neighbourhood of a point in an $s$-dimensional stratum has the form $\mathbb R^s\times cL$, respecting the strata, for a compact stratified link $L$.

#### Stratum of a stratified space

↑ **Parent:** [Stratified space](#stratified-space)

A stratum is one [manifold](#topological-manifold) piece of a stratification, with locally constant dimension and prescribed conical normal neighbourhoods. Its codimension in a pure $N$-dimensional space is $N$ minus its dimension.

#### Stratified pseudomanifold

↑ **Parent:** [Stratified space](#stratified-space)

An $N$-dimensional conically [stratified space](#stratified-space) has a closed filtration $\varnothing=X_{-1}\subseteq X_0\subseteq\cdots\subseteq X_N=X$, with each nonempty $X_j\setminus X_{j-1}$ a $j$-manifold, $X_{N-1}=X_{N-2}$, and dense top stratum. At an $s$-stratum the conical link is a compact $(N-s-1)$-dimensional [stratified pseudomanifold](#stratified-pseudomanifold). In dimension zero a compact link is a finite set. Connected links are an additional normality condition, not part of this definition.

##### Normalization of a two-dimensional pseudomanifold

↑ **Parent:** [Stratified pseudomanifold](#stratified-pseudomanifold)

The link of an isolated stratum of a closed two-dimensional pseudomanifold is a finite disjoint union of circles. Separate these branches, replacing the cone on their union by separate disks. This produces a closed [surface](#topological-surface) and a finite surjective map to the original space, a [homeomorphism](#homeomorphism) on the regular stratum. [Orientations](algebraic-topology.md#orientation-of-a-simplex) on the regular stratum extend over the disks.

##### Witt space

↑ **Parent:** [Stratified pseudomanifold](#stratified-pseudomanifold)

A rational [Witt space](#witt-space) is a [stratified pseudomanifold](#stratified-pseudomanifold) such that the link $L$ of every stratum of odd codimension $2r+1$ satisfies $IH_r^{\bar m}(L;\mathbb Q)=0$. This removes the only difference between lower and upper middle extensions and gives rational middle-perversity [Poincare duality](cohomology.md#poincare-duality) on closed oriented [Witt spaces](#witt-space).

###### Witt space with collared boundary

↑ **Parent:** [Witt space](#witt-space)

A compact [stratified space](#stratified-space) with boundary is a [Witt space](#witt-space) with collared boundary when its interior and boundary are [Witt spaces](#witt-space) and a stratified neighbourhood of the boundary is $\partial X\times[0,\varepsilon)$, with product stratification. [Orientations](algebraic-topology.md#orientation-of-a-simplex) are carried by the regular strata and induce the usual boundary [orientation](algebraic-topology.md#orientation-of-a-simplex).

##### Link of a stratum

↑ **Parent:** [Stratified pseudomanifold](#stratified-pseudomanifold)

The compact space $L$ in a stratified neighbourhood $\mathbb R^s\times cL$ is the link of the stratum. Its dimension is one less than the codimension of that stratum. A disconnected link records distinct local branches.

### Continuous real maps from the initial-segment topology

↑ **Parent:** [Topological space](#topological-space)

Give $\mathbb N$ the [topology](topology.md) whose nonempty [open sets](#open-set) are $\mathbb N$ and the finite initial segments. Every nonempty [open set](#open-set) contains $1$, so any two nonempty [open sets](#open-set) intersect. A [continuous map](#continuous-map) from this [topological space](#topological-space) into a [Hausdorff space](#hausdorff-space) is constant: distinct image points would have disjoint [open](#open-set) [neighbourhoods](#neighbourhood-mathematics), whose inverse images would be disjoint nonempty [open sets](#open-set). This includes [continuous](calculus.md#continuous-function) real-valued maps.

### Sigma-compact space

↑ **Parent:** [Topological space](#topological-space)

A space is sigma-compact if it is a countable union of compact subsets. A locally compact, sigma-compact [metrizable space](mathematics.md#metrizable-space) is [second countable](#second-countable-space): each compact metrizable subset has a countable dense set, their union is countable and dense, and a separable metric space has a countable basis.

### Sober space

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sober_space)

A [topological space](#topological-space) is sober when every nonempty [irreducible closed subset](algebraic-geometry.md#irreducible-closed-subset) is the closure of a unique point. Every [Hausdorff space](#hausdorff-space) is sober. In contrast, an infinite set with the [cofinite topology](#cofinite-topology) has the whole space irreducible and closed, while every singleton is closed, so it is not sober.

#### Sobrification

↑ **Parent:** [Sober space](#sober-space)

The sobrification has one point for every nonempty [irreducible closed subset](algebraic-geometry.md#irreducible-closed-subset) $A$ of $X$, with opens $\widehat U=\{A:A\cap U\ne\varnothing\}$. Irreducibility gives $\widehat U\cap\widehat V=\widehat{U\cap V}$, and the map from original opens to these opens is bijective, detected by singleton closures. An irreducible closed subset of the new space has complement $\widehat W$; $F=X\setminus W$ is an irreducible closed subset of $X$ and uniquely generates it. Thus the new space is a [sober space](#sober-space).

### Separable topological space

↑ **Parent:** [Topological space](#topological-space)

A [topological space](#topological-space) is separable when it has a countable [dense subset](#dense-set). The topology is part of the assertion: a dual may be separable in its [weak-star topology](weak-topology.md#weak-star-topology) and not in its [norm topology](functional-analysis.md#norm-topology). A compact [metric space](topological-analysis.md#metric-space) is separable by taking the union of finite nets at scales tending to zero.

### G-delta set

↑ **Parent:** [Topological space](#topological-space)

A G-delta set is a countable intersection of open subsets of a topological space. In a complete [metric](topological-analysis.md#metric) space these are precisely the [topologically complete](topological-analysis.md#topological-completeness) subspaces, by the [G-delta criterion for topological completeness](topological-analysis.md#g-delta-criterion-for-topological-completeness).

### Net (mathematics)

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Net_(mathematics))

A net is a family indexed by a directed ordered set: every pair of indices has a common upper bound. It converges to $x$ when it is eventually in every neighbourhood of $x$. Unlike [sequences](real-analysis.md#sequence), nets characterize closure in every [topological space](#topological-space): a point is in the closure of a set precisely when some net in that set converges to it.

#### Subnet of a net

↑ **Parent:** [Net (mathematics)](#net-mathematics)

A subnet is obtained from a [net](#net-mathematics) by an order-preserving cofinal map from another directed index set. It preserves any limit of the original net, and eventual properties still hold along it. Every net in a [compact set](#compact-space) has a convergent subnet. This supplies compactness arguments when sequential compactness is unavailable.

### Separation axiom

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Separation_axiom)

A separation axiom is a condition on a [topological space](#topological-space) expressing how points or closed subsets can be distinguished by [open sets](#open-set). The [Kolmogorov space](#kolmogorov-space) condition distinguishes distinct points by some open set; the [T1 space](#t1-space) condition makes every point closed; the stronger [Hausdorff space](#hausdorff-space) condition gives disjoint neighbourhoods to distinct points.

#### T1 space

↑ **Parent:** [Separation axiom](#separation-axiom)

A [topological space](#topological-space) is T1 when every point is a [closed point](#closed-point). Equivalently, for distinct $x,y$ there is an open set containing $x$ but not $y$, and an open set containing $y$ but not $x$. These open sets need not be disjoint. Every [Hausdorff space](#hausdorff-space) is T1, but an infinite set with its [cofinite topology](#cofinite-topology) is T1 without being Hausdorff.

### Closed point

↑ **Parent:** [Topological space](#topological-space)

A point of a [topological space](#topological-space) is closed when its singleton is a [closed set](#closed-set). In a [T1 space](#t1-space) every point is closed. The closed points of an [affine scheme](ringed-space.md#affine-scheme) $\operatorname{Spec}A$ are its [maximal ideals](commutative-algebra.md#maximal-ideal); the closure of the point corresponding to $\mathfrak p$ is $V(\mathfrak p)$.

### Locally connected space

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Locally_connected_space)

A [topological space](#topological-space) has [local connectedness](#locally-connected-space) when every point has a [neighborhood](#neighbourhood-mathematics) basis of [connected](geometry-and-topology.md#connected-space) [open sets](#open-set). In particular, a planar [domain](#domain-mathematical-analysis) has [local connectedness](#locally-connected-space), but its [domain boundary](#boundary-of-a-domain) need not be. [Local connectedness](#locally-connected-space) of the [boundary](#boundary-of-a-set) is the condition governing a continuous extension of a [conformal bijection](complex-analysis.md#biholomorphism) to the parametrizing circle.

### Boundary of a set

↑ **Parent:** [Topological space](#topological-space)

The [boundary](#boundary-of-a-set) of a subset $A$ of a [topological space](#topological-space) consists of the points whose every [neighborhood](#neighbourhood-mathematics) meets both $A$ and its complement. Equivalently, $\partial A=\overline A\setminus A^\circ$, where the bar denotes [closure](#closure-topology) and the circle denotes [interior](#interior-topology).

#### Boundary of a domain

↑ **Parent:** [Boundary of a set](#boundary-of-a-set)

The [boundary](#boundary-of-a-set) of a planar [domain](#domain-mathematical-analysis) $D$ is its [boundary of a set](#boundary-of-a-set). It is distinct from the [boundary](#boundary-of-a-set) of a parametrizing interval: a curve can begin on $\partial D$ while all its positive-time points lie inside $D$.

### Basis of a topology

↑ **Parent:** [Topological space](#topological-space)

A basis of a topology is a family of open sets such that every open set is a union of members of that family. Equivalently, every point of every open set lies in a basis member contained in it. The rectangles $U\times V$ form a basis for the [product topology](geometry-and-topology.md#product-topology) of two spaces. This topological meaning differs from a linear-algebra [basis](vector-space.md#basis).

### Second-countable space

↑ **Parent:** [Topological space](#topological-space)

A second-countable [topological space](#topological-space) has a countable collection of open sets such that every open set is a union of members of that collection. A space covered by countably many open [manifold charts](differential-geometry.md#manifold-chart) is second countable because each coordinate domain has a countable basis of rational balls.

### Paracompact space

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Paracompact_space)

A topological space is paracompact when every [open cover](#open-cover) has a locally finite open refinement. Every [metric space](topological-analysis.md#metric-space) and every second-countable [topological manifold](#topological-manifold) is paracompact.

### Kolmogorov space

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kolmogorov_space)

A topological space is $T_0$ when every pair of distinct points is distinguished by an [open set](#open-set) containing exactly one of them.

<h4 id="sierpinski-space">Sierpiński space</h4>

↑ **Parent:** [Kolmogorov space](#kolmogorov-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sierpiński_space)

The Sierpiński space is $\{0,1\}$ with open sets $\varnothing$, $\{1\}$, and $\{0,1\}$. Continuous maps $X\to S$ are in bijection with open subsets of $X$ through $g\mapsto g^{-1}(1)$.

<h5 id="embedding-of-a-t0-space-into-a-power-of-the-sierpinski-space">Embedding of a T0 space into a power of the Sierpiński space</h5>

↑ **Parent:** [Sierpiński space](#sierpinski-space)

For a [T0 space](#kolmogorov-space) $X$, evaluation against all continuous maps $g:X\to S$ is a [homeomorphism](#homeomorphism) onto its image under the map

$$
x\longmapsto(g(x))_g
$$

into a power of the [Sierpiński space](#sierpinski-space). The $T_0$ axiom makes it injective, and the coordinate inverse images of $\{1\}$ recover every open subset of $X$.

### Continuous map

↑ **Parent:** [Topological space](#topological-space)

A map between topological spaces is continuous when the inverse image of every open set is open.

#### Scalar clipping

↑ **Parent:** [Continuous map](#continuous-map)

The [continuous map](#continuous-map) projecting a real number onto the [closed interval](real-analysis.md#closed-real-interval) $[a,b]$, with $a\le b$. It equals $a$ below the interval, equals the input inside it, and equals $b$ above it. It is nondecreasing and has [Lipschitz constant](real-analysis.md#lipschitz-constant) one.

#### Topological embedding

↑ **Parent:** [Continuous map](#continuous-map)

A [continuous map](#continuous-map) [injective](algebra.md#injective-function) map $f:X\to Y$ that is a [homeomorphism](#homeomorphism) onto its image with the [subspace topology](#subspace-topology). A [continuous map](#continuous-map) [injective](algebra.md#injective-function) map from a [compact](#compact-space) space into a [Hausdorff space](#hausdorff-space) is a [topological embedding](#topological-embedding).

### Retraction

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Retraction)

A retraction of a [topological space](#topological-space) $X$ onto a subspace $A$ is a continuous map $r:X\to A$ whose restriction to $A$ is the identity.

#### Retraction onto a punctured oriented surface

↑ **Parent:** [Retraction](#retraction)

A once-punctured genus-$h$ [closed orientable surface](#closed-orientable-surface) retracts to a wedge of $2h$ circles. A [retraction](#retraction) from $\Sigma_g$ would inject its degree-one [cohomology](cohomology.md) as an [isotropic subspace of a symplectic vector space](linear-algebra.md#isotropic-subspace-of-a-symplectic-vector-space) for the [Poincare duality pairing](cohomology.md#poincare-duality-pairing), since the punctured surface has zero degree-two cohomology. The maximal isotropic dimension is $g$, giving $2h\leq g$. Equality is realized by folding the double of the punctured surface onto one copy. Additional handles in the other copy can be pinched away while fixing the joining boundary, proving sufficiency for every embedding of such a one-boundary subsurface when $g\geq2h$.

### Subspace topology

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subspace_topology)

For $A\subseteq X$, the subspace topology consists of the intersections $A\cap U$ with open subsets $U\subseteq X$.

### Alexandroff extension

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alexandroff_extension)

The one-point compactification of a locally compact noncompact Hausdorff space adjoins one point whose neighbourhoods are complements of compact subsets. The result is compact Hausdorff.

#### Hawaiian earring

↑ **Parent:** [Alexandroff extension](#alexandroff-extension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hawaiian_earring)

The Hawaiian earring is the union of a countable family of circles tangent at one point, with their radii tending to zero, endowed with its planar subspace topology. Equivalently it is the [one-point compactification](#alexandroff-extension) of a countable disjoint union of real lines. Every neighbourhood of the common point contains all but finitely many whole circles. This compact [topological space](#topological-space) is not locally contractible there and has different [singular homology](homology.md#singular-homology) from the infinite [CW complex](algebraic-topology.md#cw-complex) wedge of circles.

##### Rational summand in Hawaiian earring homology

↑ **Parent:** [Hawaiian earring](#hawaiian-earring)

The first integral [singular homology](homology.md#singular-homology) of the [Hawaiian earring](#hawaiian-earring) has a [direct summand](vector-space.md#direct-summand) isomorphic to $\mathbb Q$. This consequence of its structural homology theorem suffices, through the [universal coefficient theorem for cohomology](cohomology.md#universal-coefficient-theorem-for-cohomology) and [nonzero Ext of the rationals with integer coefficients](algebra.md#nonzero-ext-of-the-rationals-with-integer-coefficients), to show that its integral $H^2$ is nonzero. The precise structural theorem is Theorem 3.1 of [https://www.sas.rochester.edu/mth/sites/doug-ravenel/otherpapers/eda-kawamura2.pdf.](https://www.sas.rochester.edu/mth/sites/doug-ravenel/otherpapers/eda-kawamura2.pdf.)

### Circle

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circle)

The circle is the subspace $S^1=\{z\in\mathbb C:|z|=1\}$, equivalently the quotient of a closed interval obtained by identifying its endpoints.

#### Chord of a circle

↑ **Parent:** [Circle](#circle)

A chord joins two points of a [circle](#circle) by a straight segment. If the circle has radius $r$ and the chord midpoint lies a distance $d$ from its center, the perpendicular bisector and [Pythagorean theorem](geometry-and-topology.md#pythagorean-theorem) give the displayed length. The length exceeds that of an inscribed [equilateral triangle](geometry-and-topology.md#equilateral-triangle) precisely when $d<r/2$.

#### Reflection symmetry of a complex circle equation

↑ **Parent:** [Circle](#circle)

For real $\alpha\ne0,\gamma$ and complex $\beta\ne0$, completing the square in $\alpha|z|^2-\beta\bar z-\bar\beta z+\gamma=0$ gives center $\beta/\alpha$ and radius $\sqrt{|\beta|^2-\alpha\gamma}/|\alpha|$, when the radicand is nonnegative. The displayed map is reflection in the line through $0$ and $\beta$: it preserves the [complex modulus](complex-analysis.md#complex-modulus), fixes the center, and squares to the identity. Hence it maps the [circle](#circle) onto itself, including a radius-zero degeneration.

#### Maximum separation of two circles

↑ **Parent:** [Circle](#circle)

For two nonempty planar [circles](#circle) with centers $c_i$ and radii $r_i\ge0$, the greatest [Euclidean distance](topological-analysis.md#euclidean-distance) between their points is the displayed expression. The [triangle inequality](topological-analysis.md#triangle-inequality) gives the upper bound. When the centers differ, choose the two boundary points outward along the line of centers to attain it; when they coincide, choose opposite radial directions. For any third nonempty [circle](#circle) and a point $u$ on it, $|z-w|\le|z-u|+|u-w|$ proves $m(C_1,C_2)\le m(C_1,C_3)+m(C_2,C_3)$. This is not a [metric](topological-analysis.md#metric), since $m(C,C)=2r$ for a positive-radius [circle](#circle).

#### Steiner chain

↑ **Parent:** [Circle](#circle)

A cyclic chain of distinct [circles](#circle) between two disjoint [circle](#circle) boundaries, each tangent to both boundaries and its two neighbours. In concentric coordinates with inner radius $\rho$ and outer radius $R$, the chain [circles](#circle) have radius $r=(R-\rho)/2$ and centre distance $d=(R+\rho)/2$. A simple disjoint chain with $n\geq3$ closes when $r/d=\sin(\pi/n)$.

##### Steiner porism

↑ **Parent:** [Steiner chain](#steiner-chain)

If a simple [Steiner chain](#steiner-chain) closes after $n\geq3$ [circles](#circle), rotating the starting [circle](#circle) between concentric boundaries gives another closed $n$-[circle](#circle) chain. Applying a [Möbius transformation](group-theory.md#mobius-transformation) proves the corresponding statement for arbitrary boundary [circles](#circle). Construction must stay in the same intervening family and proceed without reversing the chosen direction. Merely choosing arbitrary [circles](#circle) tangent to the preceding [circle](#circle) permits backtracking and does not assert closure.

##### Tangency locus of a Steiner chain

↑ **Parent:** [Steiner chain](#steiner-chain)

For a [Steiner chain](#steiner-chain) between concentric [circles](#circle), tangencies of neighbouring [circles](#circle) are midpoints of their centres and lie on the [circle](#circle) of radius $\sqrt{R\rho}$. Under a [Möbius transformation](group-theory.md#mobius-transformation), their locus is a [generalized circle](group-theory.md#generalized-circle-under-a-mobius-transformation), which may be a line. An ordinary-[circle](#circle) conclusion requires the pole of the inverse transformation to avoid the original locus.

#### Circle from an affine complex-modulus equation

↑ **Parent:** [Circle](#circle)

An equation $|az+b\overline z|=ux+v$, with $z=x+iy$ and real coefficients, becomes $(a+b)^2x^2+(a-b)^2y^2=(ux+v)^2$ after squaring. If $(a+b)^2-u^2=(a-b)^2>0$, completing the square gives a [circle](#circle). The original locus is only the part where $ux+v\geq0$. Checking this sign on the candidate [circle](#circle) prevents extraneous points introduced by squaring. This method combines the [complex modulus](complex-analysis.md#complex-modulus) with elementary conic geometry.

#### Radius

↑ **Parent:** [Circle](#circle)

The radius of a [circle](#circle) or [sphere](geometry-and-topology.md#sphere) is the [Euclidean distance](topological-analysis.md#euclidean-distance) from its centre to its boundary. The diameter is twice the radius.

#### Pi

↑ **Parent:** [Circle](#circle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pi)

Pi is the ratio of a Euclidean circle's circumference to its diameter.

##### Wallis product

↑ **Parent:** [Pi](#pi)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wallis_product)

The [Wallis product](#wallis-product) is

$$
\frac\pi2=\prod_{j=1}^{\infty}\frac{(2j)^2}{(2j-1)(2j+1)}.
$$

Its finite product is $W_n=2^{4n}(n!)^4/[(2n+1)((2n)!)^2]$. The [Wallis integrals](calculus.md#wallis-integrals) give $2W_n/\pi=I_{2n+1}/I_{2n}\to1$, proving both convergence of the product and its value. The strict integral bounds also give $\pi n/(2n+1)<W_n<\pi/2$.

<h5 id="proof-that-pi-is-irrational">Proof that π is irrational</h5>

↑ **Parent:** [Pi](#pi)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proof_that_π_is_irrational)

Assuming $\pi=a/b$ and integrating a suitably normalized polynomial times $\sin x$ produces a positive integer that tends to zero as the polynomial degree grows. This contradiction proves that $\pi$ is an [irrational number](algebra.md#irrational-number).

### Wedge sum

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wedge_sum)

The wedge sum of pointed spaces identifies all their basepoints. In particular, a wedge of $m$ circles has first homology $\mathbb Z^m$.

#### Pinch map

↑ **Parent:** [Wedge sum](#wedge-sum)

A pinch map collapses a separating subspace to a point so that the quotient splits into a [wedge sum](#wedge-sum). For a [connected sum of oriented manifolds](differential-geometry.md#connected-sum-of-oriented-manifolds), collapsing the separating boundary sphere gives a map $M\mathbin\#N\to M\vee N$. The two wedge projections have [degree of a continuous mapping](homology.md#degree-of-a-continuous-mapping) one with compatible orientations. Consequently their pullbacks identify the two top [orientation classes](cohomology.md#fundamental-class), while positive-degree classes from different summands have zero [cup product](cohomology.md#cup-product).

#### Wedge of two circles

↑ **Parent:** [Wedge sum](#wedge-sum)

The wedge of two circles is a graph with one vertex and two loop edges. Its [fundamental group](algebraic-topology.md#fundamental-group) is the free group on the two oriented loops.

### Inclusion map

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inclusion_map)

For a subspace $A\subseteq X$, the inclusion map is the [injective function](algebra.md#injective-function) $i:A\to X$ given by $i(a)=a$.

### Topology axiom

↑ **Parent:** [Topological space](#topological-space)

A family $\mathcal T$ of [subsets](set.md#subset) of a [set](set.md) $X$ is a topology when $\varnothing,X\in\mathcal T$, every [union](set.md#set-union) of members of $\mathcal T$ belongs to $\mathcal T$, and every finite [intersection](set.md#set-intersection) of members of $\mathcal T$ belongs to $\mathcal T$.

### Open cover

↑ **Parent:** [Topological space](#topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Open_cover)

An open cover of a subset $A$ is a family of open sets whose union contains $A$.

#### Affine open cover

↑ **Parent:** [Open cover](#open-cover)

An affine open cover of a [scheme](ringed-space.md#scheme) is an [open cover](#open-cover) by [affine open subsets](ringed-space.md#affine-open-subscheme). Every [scheme](ringed-space.md#scheme) has such a cover by definition. A [quasi-compact scheme](ringed-space.md#quasi-compact-scheme) has a finite affine open cover. Whether the intersections are affine is a further condition, supplied in particular by separatedness over an affine base.

#### Acyclic cover

↑ **Parent:** [Open cover](#open-cover)

An open cover is acyclic for a specified [sheaf](algebraic-geometry.md#sheaf-mathematics) if its restriction to every nonempty finite intersection has zero higher [sheaf cohomology](ringed-space.md#sheaf-cohomology). The [acyclic cover theorem](ringed-space.md#leray-s-theorem) then identifies the cover's [Čech cohomology](ringed-space.md#cech-cohomology) with sheaf cohomology. On a [separated scheme](ringed-space.md#separated-scheme), an affine open cover is acyclic for every [quasi-coherent sheaf](ringed-space.md#quasi-coherent-sheaf).

## Quotient topology

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quotient_topology)

For an equivalence relation $R$ on a topological space $X$, the quotient topology on the set $X/R$ declares $U\subseteq X/R$ open exactly when its inverse image under the projection $q:X\to X/R$ is open in $X$.

### Quotient topological space

↑ **Parent:** [Quotient topology](#quotient-topology)

A quotient topological space identifies points of a [topological space](#topological-space) according to an [equivalence relation](set-theory.md#equivalence-relation) and equips the set of equivalence classes with the [quotient topology](#quotient-topology). A subset is open exactly when its inverse image under the canonical [quotient map](#quotient-map) is open. Even a [Hausdorff space](#hausdorff-space) can have a non-Hausdorff quotient; identifying real numbers differing by a rational number gives a multi-point quotient with the [indiscrete topology](#indiscrete-topology).

### Quotient map

↑ **Parent:** [Quotient topology](#quotient-topology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quotient_map)

A quotient map is a surjective continuous map $q:X\to Y$ for which $U\subseteq Y$ is open exactly when $q^{-1}(U)$ is open.

### Universal property of the quotient topology

↑ **Parent:** [Quotient topology](#quotient-topology)

If $q:X\to X/R$ is the quotient map and a continuous map $f:X\to Y$ is constant on each equivalence class, there is a unique continuous map $F:X/R\to Y$ satisfying $Fq=f$. It is given by $F([x])=f(x)$; continuity follows because

$$
q^{-1}(F^{-1}(U))=f^{-1}(U)
$$

for every open $U\subseteq Y$.

### Non-Hausdorff quotient of the real line by rational translation

↑ **Parent:** [Quotient topology](#quotient-topology)

Identify $x,y\in\mathbb R$ when $x-y\in\mathbb Q$. Every nonempty saturated open subset of $\mathbb R$ meets every other one because rational translates of any open interval meet any prescribed nonempty open interval. The quotient $\mathbb R/\mathbb Q$ has multiple points but no two nonempty disjoint open subsets, so it is not Hausdorff.

### Square quotient model of the two-sphere

↑ **Parent:** [Quotient topology](#quotient-topology)

Identify the vertical sides of $[0,1]^2$, then collapse each horizontal side separately to a point. The resulting quotient is homeomorphic to $S^2$ through

$$
(x,y)\longmapsto
\bigl(\sin(\pi y)\cos(2\pi x),
\sin(\pi y)\sin(2\pi x),\cos(\pi y)\bigr).
$$

Equivalently, the quotient is the suspension of the circle.

## Open set

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Open_set)

An open set is a member of the topology on a topological space.

### Domain (mathematical analysis)

↑ **Parent:** [Open set](#open-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Domain_(mathematical_analysis))

A domain is a nonempty connected [open set](#open-set) in the ambient space under discussion. In [complex analysis](complex-analysis.md) this normally means an open connected subset of $\mathbb C$. A [star-shaped set](algebra.md#star-shaped-set) that is open is a domain, but a domain need not be a [simply connected domain](complex-analysis.md#simply-connected-domain) and can have a [period obstruction to a holomorphic antiderivative](complex-analysis.md#period-obstruction-to-a-holomorphic-antiderivative).

### Clopen set

↑ **Parent:** [Open set](#open-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Clopen_set)

A clopen set is a subset that is both [open](#open-set) and [closed](#closed-set).

### Open interval

↑ **Parent:** [Open set](#open-set)

This is the open-boundary case of an [interval](real-analysis.md#interval-mathematics).

An open interval in the real line is a set $(a,b)=\{x:a<x<b\}$, allowing either endpoint to be infinite.

#### Nondegenerate interval

↑ **Parent:** [Open interval](#open-interval)

A nondegenerate interval contains more than one point; for an interval with finite endpoints, this means that its endpoints are distinct.

### Neighbourhood (mathematics)

↑ **Parent:** [Open set](#open-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neighbourhood_(mathematics))

A neighbourhood of a point is a set containing an open set that contains that point.

#### Neighbourhood system

↑ **Parent:** [Neighbourhood (mathematics)](#neighbourhood-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neighbourhood_system)

The [neighbourhood system](#neighbourhood-system) at a point consists of all its [neighbourhoods](#neighbourhood-mathematics). A [neighbourhood basis](#neighbourhood-basis) is a subfamily cofinal under reverse inclusion.

##### Neighbourhood basis

↑ **Parent:** [Neighbourhood system](#neighbourhood-system)

A neighbourhood basis at a point is a family of neighbourhoods such that every neighbourhood of the point contains one of them.

### Open ball

↑ **Parent:** [Open set](#open-set)

In a [metric space](topological-analysis.md#metric-space), the [open ball](#open-ball) of radius $r>0$ about $x$ is $\{y:d(x,y)<r\}$; it is the open-boundary convention for a [ball](topological-analysis.md#ball-mathematics).

### Annulus (mathematics)

↑ **Parent:** [Open set](#open-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Annulus_(mathematics))

An annulus is the region between two concentric circles.

#### Fixed-point-free rotation of an annulus

↑ **Parent:** [Annulus (mathematics)](#annulus-mathematics)

Rotation through any nonzero angle defines a continuous self-map of a circular annulus with no fixed point. Hence an annulus does not have the [fixed-point property](analysis.md#fixed-point-property).

## Disk (mathematics)

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Disk_(mathematics))

A planar [Euclidean disk](#disk-mathematics) consists of the points within a fixed radius of a centre, with either the open or closed boundary convention. The closed disk centered at the origin is $D_R=\{x\in\mathbb R^2:|x|\leq R\}$ and has [area](differential-geometry.md#surface-area) $\pi R^2$. It is the two-dimensional closed Euclidean ball; the general [closed disc](#closed-disc) may have any dimension.

### Open disc

↑ **Parent:** [Disk (mathematics)](#disk-mathematics)

The open disc with centre $z$ and radius $r>0$ is $\{w:|w-z|<r\}$.

#### Unit disc

↑ **Parent:** [Open disc](#open-disc)

The unit disc in the [complex plane](complex-analysis.md#complex-plane) is $\mathbb D=\{z\in\mathbb C:|z|<1\}$.

##### Automorphism of the unit disk

↑ **Parent:** [Unit disc](#unit-disc)

A [biholomorphism](complex-analysis.md#biholomorphism) of the unit disk to itself. Every such map has the form $e^{i\theta}(z-a)/(1-\overline a z)$ with $|a|<1$. These maps normalize an extremal [univalent function](complex-analysis.md#univalent-function) in the proof of the [Riemann mapping theorem](complex-analysis.md#riemann-mapping-theorem).

## Topological disc

↑ **Parent:** [Topology](topology.md)

An $n$-dimensional topological disc is a space homeomorphic to a Euclidean ball in $\mathbb R^n$, with its open or closed convention specified. A [closed disc](#closed-disc) is homeomorphic to $D^n=\{x\in\mathbb R^n:|x|\leq1\}$. The planar [disk](#disk-mathematics) is the Euclidean two-dimensional instance, rather than the whole abstract topological class.

### Closed disc

↑ **Parent:** [Topological disc](#topological-disc)

A closed $n$-disc is a space homeomorphic to $D^n=\{x\in\mathbb R^n:|x|\leq1\}$; its boundary is the sphere $S^{n-1}$.

## Level set

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Level_set)

A level set of a function $f$ is a set of the form $\{x:f(x)=c\}$.

### Level curve

↑ **Parent:** [Level set](#level-set)

A [level curve](#level-curve) is the planar [level set](#level-set) of a scalar function. Where the gradient does not vanish, the [implicit function theorem](calculus.md#implicit-function-theorem) makes it locally a smooth curve. At a [critical point](analysis.md#critical-point), branches may cross, narrow into a cusp or shrink to a point, so a plot should be interpreted with the local critical-point analysis.

### Regular level set

↑ **Parent:** [Level set](#level-set)

A [level set](#level-set) at a [regular value](differential-geometry.md#regular-value) is a smooth [submanifold](differential-geometry.md#submanifold). By the [regular level set theorem](differential-geometry.md#regular-level-set-theorem), its codimension is the dimension of the target. For determinant-one real [symmetric matrices](linear-algebra.md#symmetric-matrix), $D(\det)_B(C)=\operatorname{tr}(B^{-1}C)$ is nonzero because $C=B$ gives $n$, so the constraint has codimension one.

### Superlevel set

↑ **Parent:** [Level set](#level-set)

A superlevel set of a real-valued function $f$ is a set of the form $\{x:f(x)\geq c\}$ or $\{x:f(x)>c\}$.

## Dense set

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dense_set)

A subset is dense when every nonempty [open set](#open-set) meets it, equivalently when its closure is the whole ambient space.

## Discrete space

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discrete_space)

A topological space is discrete when every subset is an [open set](#open-set).

### Discrete subset

↑ **Parent:** [Discrete space](#discrete-space)

A subset of a [topological space](#topological-space) is discrete when its [subspace topology](#subspace-topology) is a [discrete topology](#discrete-space): every point has an ambient neighbourhood meeting the subset only in that point. A discrete subset need not be closed; for example $\{1/n:n\geq1\}$ in the real line accumulates at zero. The group structure makes a [discrete subgroup](topological-group.md#discrete-subgroup) of a Hausdorff [topological group](topological-group.md) closed, an additional property used in discontinuity arguments.

#### Closed discrete subset

↑ **Parent:** [Discrete subset](#discrete-subset)

In a plane [domain](#domain-mathematical-analysis), a closed [discrete subset](#discrete-subset) is exactly a set meeting every [compact subset](#compact-space) in finitely many points. This local finiteness is necessary for a nonzero [holomorphic function](complex-analysis.md#holomorphic-function) to have the subset as its entire zero set. A merely isolated-point subset can have an accumulation point outside the subset but inside the domain, as $\{1/n:n\geq1\}\subset\mathbb C$ does.

// Destination: analysis.bigb

#### Discrete subsets of the real line are countable

↑ **Parent:** [Discrete subset](#discrete-subset)

Enumerate all intervals with rational endpoints, using the countability of the [rational numbers](number-theory.md#rational-number) and listing pairs of enumeration indices by increasing sum. If every point $b$ of $B$ is an [isolated point](topological-analysis.md#isolated-point), some such interval contains $b$ and no other point of $B$. Assign to $b$ the least index of such an interval. Distinct points cannot have the same index, so this gives an [injective function](algebra.md#injective-function) into $\mathbb N$ and proves that $B$ is a [countable set](set-theory.md#countable-set). The argument uses isolation in the [subspace topology](#subspace-topology), not closedness: the [discrete subset](#discrete-subset) $\{1/n:n\ge1\}$ illustrates that an accumulation point outside $B$ is allowed.

## Connected-space zero-product dichotomy

↑ **Parent:** [Topology](topology.md)

If continuous functions $f,g$ on a connected space satisfy $fg=0$ and never vanish simultaneously, then the disjoint open sets $\{f\ne0\}$ and $\{g\ne0\}$ cover the space. One is empty, so one function vanishes identically.

## Normal space

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_space)

A topological space is normal when every two disjoint closed subsets have disjoint open neighbourhoods.

### Closed-neighborhood shrinking in a normal space

↑ **Parent:** [Normal space](#normal-space)

If $F$ is closed, $U$ is open, and $F\subset U$ in a [normal topological space](#normal-space), separate $F$ from the closed complement $X\setminus U$ by disjoint open sets $W,V$. Then $\overline W\subset X\setminus V\subset U$. In particular, first separate two disjoint closed sets by disjoint open sets and then shrink each neighborhood this way: their closures are disjoint. No additional metric or compactness assumption is needed.

<h3 id="urysohn-s-lemma">Urysohn's lemma</h3>

↑ **Parent:** [Normal space](#normal-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Urysohn's_lemma)

If $A,B$ are disjoint closed subsets of a normal space, there is a continuous function $f:X\to[0,1]$ with $f|_A=0$ and $f|_B=1$.

#### Tietze extension theorem

↑ **Parent:** [Urysohn's lemma](#urysohn-s-lemma)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tietze_extension_theorem)

Every continuous real-valued function on a closed subspace of a normal space extends continuously to the whole space. If its values lie in a closed interval, the extension can be kept in that interval.

##### Metric Tietze two-thirds approximation

↑ **Parent:** [Tietze extension theorem](#tietze-extension-theorem)

For a real function $g$ in the [bounded continuous functions](calculus.md#bounded-continuous-functions) of norm $M$ on a closed subset $Y$ of a [metric space](topological-analysis.md#metric-space), separate its closed level sets $A=\{g\le-M/3\}$ and $B=\{g\ge M/3\}$ by $u=(M/3)(d(\cdot,A)-d(\cdot,B))/(d(\cdot,A)+d(\cdot,B))$. The [distance to a set](topological-analysis.md#distance-to-a-set) functions make $u$ continuous with the displayed bounds. Empty level sets are handled by the constants $M/3$, $-M/3$ or $0$. Iterating on the residual yields a uniformly convergent continuous extension with no increase in the [supremum norm](functional-analysis.md#supremum-norm).

### Closed G-delta set as a zero set

↑ **Parent:** [Normal space](#normal-space)

A closed subset $A$ of a normal space is a countable intersection of open sets exactly when it is the zero set of some continuous function $f:X\to[0,1]$.

## Compact space

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compact_space)

A topological space is compact when every open cover has a finite subcover. Every closed subspace of a compact space is compact. This open-cover definition does not require the space to be Hausdorff; in algebraic geometry it is often called quasi-compactness.

### Ultrafilter characterization of compactness

↑ **Parent:** [Compact space](#compact-space)

A [topological space](#topological-space) is [compact](#compact-space) if and only if every [ultrafilter](set-theory.md#ultrafilter) on it converges to at least one point, assuming the [ultrafilter lemma](set-theory.md#ultrafilter-lemma). No [Hausdorff](#hausdorff-space) assumption is needed. In a compact space, the closures of the filter members have the [finite intersection property](#finite-intersection-property), so choose a point in their intersection. Every open neighbourhood of that point belongs to the ultrafilter, since otherwise its closed complement would be a filter member. Conversely, extend the complements of a cover with no finite subcover to an ultrafilter; a limit point lies in a covering open set, contradicting the simultaneous membership of that set and its complement.

### Compact exhaustion

↑ **Parent:** [Compact space](#compact-space)

A compact exhaustion of an open subset $U$ of a finite-dimensional [Euclidean space](functional-analysis.md#euclidean-norm) is an increasing sequence of compact subsets $K_n\subset U$ with $K_n\subset\operatorname{int}K_{n+1}$ and $\bigcup_nK_n=U$. For example, choose smoothed bounds or suitable nested levels of distance from the complement and distance from the origin. Exit times from these sets express the lifetime of a [maximal local solution of a stochastic differential equation](stochastic-calculus.md#maximal-local-solution-of-a-stochastic-differential-equation); every finite-time continuous path lying in $U$ has compact image and is contained in some $K_n$.

### Compact Hausdorff space

↑ **Parent:** [Compact space](#compact-space)

A compact Hausdorff space is both [compact](#compact-space) and [Hausdorff](#hausdorff-space). Such a space is [normal](#normal-space), and every real-valued [continuous function](calculus.md#continuous-function) on it is bounded.

#### Supremum convergence for decreasing continuous functions

↑ **Parent:** [Compact Hausdorff space](#compact-hausdorff-space)

On a nonempty [compact Hausdorff space](#compact-hausdorff-space), let continuous nonnegative functions decrease pointwise. Their suprema decrease to a finite number $L$. For every $t<L$, the sets $\{f_n\geq t\}$ are nonempty nested closed sets; compactness gives a common point with limit value at least $t$. Thus the supremum of the pointwise limit is $L$. The limit need not be continuous, and this conclusion does not claim uniform convergence as in the [Dini theorem](real-analysis.md#dini-s-theorem).

#### Closed relation generated by a set-split pair of compact Hausdorff maps

↑ **Parent:** [Compact Hausdorff space](#compact-hausdorff-space)

Let continuous maps $f,g:X\rightrightarrows Y$ between [compact Hausdorff spaces](#compact-hausdorff-space) have an underlying [split coequalizer](category.md#split-coequalizer) $q:Y\to Z$ with set maps $s,t$ satisfying $qs=1$, $ft=1$ and $gt=sq$. Its equivalence relation is the image of the closed subset $\{(x,x')\in X^2:g(x)=g(x')\}$ under $(f,f)$. One inclusion follows from $qf=qg$; for the other use $x=t(y)$ and $x'=t(y')$ whenever $q(y)=q(y')$. This image is compact and hence closed in the Hausdorff product $Y^2$. The quotient is therefore compact Hausdorff, giving the preserved [coequalizer](category.md#coequalizer) required by the [Beck monadicity theorem](category-theory.md#beck-s-monadicity-theorem).

#### Separable compactification need not be metrizable

↑ **Parent:** [Compact Hausdorff space](#compact-hausdorff-space)

Embed $\mathbb N$ into the compact product $\{0,1\}^{\mathcal P(\mathbb N)}$ by $j(n)_S=\mathbf1_S(n)$ and take its closure $X$. The [Tychonoff theorem](geometry-and-topology.md#tychonoff-s-theorem) makes $X$ a [compact Hausdorff space](#compact-hausdorff-space), while $j(\mathbb N)$ is countable, dense and discrete in its subspace topology. Yet $X$ is not metrizable. Any convergent subsequence $j(n_k)$ of distinct points would have a convergent coordinate for $S=\{n_2,n_4,\ldots\}$, whereas that coordinate alternates between zero and one. This contradicts sequential compactness of a [compact metric space](topological-analysis.md#compact-metric-space). Thus a dense metrizable subspace does not force a separable compact Hausdorff ambient space to be metrizable.

### Heine-Borel theorem

↑ **Parent:** [Compact space](#compact-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heine–Borel_theorem)

A subset of a finite-dimensional real vector space is compact exactly when it is closed and bounded.

### Finite intersection property

↑ **Parent:** [Compact space](#compact-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_intersection_property)

A family of sets has the finite intersection property when every finite subfamily has nonempty intersection. A [topological space](#topological-space) is compact exactly when every family of closed subsets with the finite intersection property has nonempty total intersection.

### Continuous image of a compact space

↑ **Parent:** [Compact space](#compact-space)

The continuous image of a compact space is compact: pull an open cover of the image back to the domain, take a finite subcover there, and map it forward.

### Quotient of a compact space

↑ **Parent:** [Compact space](#compact-space)

Every quotient of a compact space is compact because the quotient projection is continuous and surjective.

### Lebesgue number lemma

↑ **Parent:** [Compact space](#compact-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lebesgue_number_lemma)

Every open cover of a compact metric space has a number $\delta>0$ such that every subset of diameter less than $\delta$ lies in one member of the cover.

### Normality of a compact Hausdorff space

↑ **Parent:** [Compact space](#compact-space)

Every compact Hausdorff space is normal: disjoint closed subsets have disjoint open neighbourhoods. Pointwise Hausdorff separation becomes uniform first over one compact closed set and then over the other by taking finite subcovers.

<h3 id="alexander-s-subbase-lemma">Alexander's subbase lemma</h3>

↑ **Parent:** [Compact space](#compact-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alexander's_subbase_lemma)

A topological space is compact when every cover by members of a fixed subbase has a finite subcover. Equivalently, every family of complements of subbasic opens with the finite-intersection property has nonempty intersection.

### Locally compact space

↑ **Parent:** [Compact space](#compact-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Locally_compact_space)

A space is locally compact when every point has a base of neighbourhoods containing compact neighbourhoods. A compact Hausdorff space is locally compact because regular separation produces $x\in V\subseteq\overline V\subseteq U$.

#### Compactly detected closed-set theorem in a locally compact Hausdorff space

↑ **Parent:** [Locally compact space](#locally-compact-space)

If $X$ is locally compact Hausdorff and $A\cap K$ is closed in every compact subset $K$, then $A$ is closed. Around each point outside $A$, use a compact neighbourhood and the relative openness of its complement of $A\cap K$.

## Hausdorff space

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hausdorff_space)

A Hausdorff space separates any two distinct points by disjoint open neighborhoods.

### Completely regular Hausdorff space

↑ **Parent:** [Hausdorff space](#hausdorff-space)

A [Hausdorff space](#hausdorff-space) is completely regular if a point $x$ outside a [closed set](#closed-set) $F$ can be separated from $F$ by a [continuous function](calculus.md#continuous-function) $u:X\to[0,1]$ with $u(x)=1$ and $u|_F=0$. These functions determine the original [topology](topology.md): for any neighborhood $O$ of $x$, choose $F=X\setminus O$ to obtain $x\in\{u>1/2\}\subseteq O$. This is exactly the point-separation property needed for the evaluation embedding into the weak-star dual of bounded continuous functions.

### Compact subset of a Hausdorff space

↑ **Parent:** [Hausdorff space](#hausdorff-space)

Every compact subset of a Hausdorff space is closed. For a point outside the compact set, separate it from each point of the set and use a finite subcover to obtain one neighbourhood disjoint from the whole set.

### Compact-to-Hausdorff continuous bijection theorem

↑ **Parent:** [Hausdorff space](#hausdorff-space)

A continuous bijection from a compact space to a Hausdorff space is a homeomorphism. It maps closed sets to compact sets, which are closed in the codomain, so it is a closed map and its inverse is continuous.

### Closed diagonal theorem

↑ **Parent:** [Hausdorff space](#hausdorff-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed_diagonal_theorem)

A space is Hausdorff exactly when its diagonal is closed in its square.

## Homeomorphism

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homeomorphism)

### Inverse continuity from an open bijection

↑ **Parent:** [Homeomorphism](#homeomorphism)

A continuous bijection that is an [open map](calculus.md#open-map) is a [homeomorphism](#homeomorphism). If $g=f^{-1}$ and $U$ is open in the original domain, then $g^{-1}(U)=f(U)$ is open by the open-map property. This proves continuity of the inverse directly.

### Local homeomorphism

↑ **Parent:** [Homeomorphism](#homeomorphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_homeomorphism)

A local homeomorphism is a continuous map $f:X\to Y$ such that every point of $X$ has a neighbourhood on which $f$ restricts to a homeomorphism onto an open subset of $Y$.

A homeomorphism is a bijective continuous map whose inverse is continuous. Two spaces related by one have the same topological properties.

### Closed map

↑ **Parent:** [Homeomorphism](#homeomorphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed_map)

A closed map sends closed subsets of its domain to closed subsets of its codomain. A bijection is a homeomorphism exactly when it is continuous and closed.

#### Projection with a compact factor is closed

↑ **Parent:** [Closed map](#closed-map)

For [metric spaces](topological-analysis.md#metric-space) $X,Y$ with $X$ [compact](#compact-space), the [projection with a compact factor is closed](#projection-with-a-compact-factor-is-closed): if $F\subset X\times Y$ is a [closed set](#closed-set) and $y_n\in\pi_Y(F)$ converges to $y$, choose $x_n$ with $(x_n,y_n)\in F$. [Sequential compactness](geometry-and-topology.md#sequentially-compact-space) supplies $x_{n_k}\to x$, so $(x_{n_k},y_{n_k})\to(x,y)\in F$, proving $y\in\pi_Y(F)$. The [projection map](function.md#projection-map) is also [continuous](calculus.md#continuous-function) for the sum [metric](topological-analysis.md#metric). Without [compactness](#compact-space), the [closed set](#closed-set) $\{(x,y)\in\mathbb R^2:xy=1\}$ projects to the nonclosed set $\mathbb R\setminus\{0\}$.

#### Compact-preimage theorem for closed maps

↑ **Parent:** [Closed map](#closed-map)

Let $f:X\to Y$ be a [continuous map](#continuous-map) that is a [closed map](#closed-map) and whose fibres are [compact](#compact-space). Then $f^{-1}(K)$ is [compact](#compact-space) for every [compact set](#compact-space) $K\subseteq Y$, without a [Hausdorff](#hausdorff-space) hypothesis. Given an [open cover](#open-cover), cover each fibre by a finite union $V_y$ of its members. The set $W_y=Y\setminus f(X\setminus V_y)$ is open, contains $y$, and has $f^{-1}(W_y)\subseteq V_y$. A finite subcover of $K$ by the $W_y$ uses only finitely many original cover members and covers $f^{-1}(K)$. Empty fibres cause no exception.

## Unit sphere

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unit_sphere)

The unit sphere in $\mathbb R^{n+1}$ is

$$
S^n=\{x\in\mathbb R^{n+1}:\|x\|=1\}.
$$

## Closed graph theorem for compact spaces

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed_graph_theorem_for_compact_spaces)

A map between compact Hausdorff spaces is continuous exactly when its graph is closed.

### Closed-graph criterion with compact codomain

↑ **Parent:** [Closed graph theorem for compact spaces](#closed-graph-theorem-for-compact-spaces)

If $X,Y$ are metric spaces, $Y$ is compact, and the graph of $f:X\to Y$ is closed, then $f$ is continuous. Any failure of sequential continuity gives a subsequence whose images stay away from the proposed limit; compactness produces a convergent image subsequence, and closedness of the graph forces its limit to be the correct value.

## Curve

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Curve)

A curve in a [topological space](#topological-space) $X$ is a [continuous function](calculus.md#continuous-function) from an interval into $X$.

### Asymptote

↑ **Parent:** [Curve](#curve)

An asymptote of an unbounded [curve](#curve) is a straight line whose distance from the curve tends to zero along a specified end. For a graph, a sloping asymptote $y=mx+b$ satisfies $y(x)-(mx+b)\to0$ as $x$ tends to the relevant infinity. Factorization of the leading quadratic part locates the two asymptotes of a nondegenerate [hyperbola](geometry-and-topology.md#hyperbola).

### Parametric curve

↑ **Parent:** [Curve](#curve)

A [parametric curve](#parametric-curve) is described by a vector-valued map $t\mapsto Q(t)$. Its [derivative](calculus.md#derivative) gives a [tangent vector](differential-geometry.md#tangent-vector) wherever it is nonzero.

// Target: geometry-and-topology.bigb

#### Parametric curve interrogation

↑ **Parent:** [Parametric curve](#parametric-curve)

A [parametric curve](#parametric-curve) interface supplies its parameter domain, evaluation, and [derivatives](calculus.md#derivative) where they exist. Robust geometric algorithms also need restricted subcurves and certified range or [derivative](calculus.md#derivative) bounds on parameter intervals. Tangent, speed and [curvature](differential-geometry.md#curvature) are derived from point and [derivative](calculus.md#derivative) enquiries when the relevant [derivatives](calculus.md#derivative) are regular. Finite point samples alone cannot certify the absence of every plane intersection of an arbitrary smooth curve.

##### Certified curve-plane intersection

↑ **Parent:** [Parametric curve interrogation](#parametric-curve-interrogation)

Intersecting a [parametric curve](#parametric-curve) with a plane reduces to isolating zeros of a scalar function. A certified range for $F$ rejects intervals that do not contain zero. On an interval whose [derivative](calculus.md#derivative) range excludes zero, a sign-changing endpoint bracket gives exactly one root, which [bisection method](numerical-analysis.md#bisection-method) or a safeguarded [Newton root-finding iteration](numerical-analysis.md#newton-root-finding-iteration) refines. Other intervals are subdivided conservatively; tangencies and coplanar pieces need multiplicity or identity tests supported by the representation. An unresolved small interval is a possible contact, not a proof of an intersection. With finitely many transverse intersections and convergent enclosures, isolation terminates to any prescribed tolerance.

#### Cycloid

↑ **Parent:** [Parametric curve](#parametric-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cycloid)

A cycloid is the [plane curve](algebraic-geometry.md#plane-curve) traced by a point on a circle rolling without slipping along a straight line. A parametrization with rolling radius $R$ is $x=R(\theta-\sin\theta)$, $y=R(1-\cos\theta)$; reversing the sign of $y$ reflects the curve. Its cusps occur at integer multiples of $2\pi$. A descending cycloidal arc solves the classical [brachistochrone problem](calculus-of-variations.md#brachistochrone-problem).

### Space curve

↑ **Parent:** [Curve](#curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Space_curve)

A space curve is a [curve](#curve) in three-dimensional [Euclidean space](functional-analysis.md#euclidean-norm).

#### Helix

↑ **Parent:** [Space curve](#space-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Helix)

A helix is a [space curve](#space-curve) that winds around an axis while advancing along it at a constant rate. A circular helix can be parametrized by $(R\cos t,R\sin t,at)$.

##### Logarithmic conical helix

↑ **Parent:** [Helix](#helix)

The displayed [space curve](#space-curve), $s>0$, lies on a cone and is parametrized by [arc length](riemannian-geometry.md#arc-length). It has a constant tangent angle with its axis, while the turn spacing shrinks geometrically toward the limiting apex. Its [curvature](differential-geometry.md#curvature) is $1/(\sqrt2s)$: differentiate its unit tangent with respect to $s$. Infinitely many turns accumulate at the apex with finite [arc length](riemannian-geometry.md#arc-length); the apex itself is not a regular point of the curve.

##### Pitch of a helix

↑ **Parent:** [Helix](#helix)

The pitch is the axial displacement per complete turn. For a circular [helix](#helix) with $z=a\phi+b$, the signed pitch for increasing angle is $2\pi a$, and its magnitude is $2\pi|a|$. Pitch is independent of the cylinder radius.

### Inflection point

↑ **Parent:** [Curve](#curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inflection_point)

An inflection point of a smooth plane curve is a point where its signed curvature changes sign. At a regular inflection point the curvature vanishes.

### Logarithmic spiral

↑ **Parent:** [Curve](#curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Logarithmic_spiral)

A logarithmic spiral has polar equation $r=Ae^{b\theta}$. Its tangent meets each radial line at a constant angle.

#### Logarithmic spiral as an embedded real line

↑ **Parent:** [Logarithmic spiral](#logarithmic-spiral)

The map $h$ is a [homeomorphism](#homeomorphism) from the [real line](real-analysis.md#real-line) to its image with the [subspace topology](#subspace-topology): its continuous inverse is $h^{-1}(x,y)=\log\sqrt{x^2+y^2}$. Different parameters have different radii, so winding does not destroy injectivity. The origin is an accumulation point of the spiral but is not a point of this space.

### Simple curve

↑ **Parent:** [Curve](#curve)

A simple curve is an [injective](algebra.md#injective-function) curve, apart from the permitted coincidence of its two endpoints when it is closed.

### Space-filling curve

↑ **Parent:** [Curve](#curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Space-filling_curve)

A space-filling curve is a [surjective](algebra.md#surjective-function) continuous map from an interval onto a region of dimension at least two.

## Topological surface

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_surface)

A topological surface is a [Hausdorff space](#hausdorff-space) with a countable basis in which every point has a neighborhood homeomorphic to an open subset of $\mathbb R^2$.

### Classification of compact surfaces

↑ **Parent:** [Topological surface](#topological-surface)

A [connected](geometry-and-topology.md#connected-space) [compact](#compact-space) [surface](#topological-surface) is determined by its [orientability](#orientability), number $b$ of [boundary](#boundary-of-a-set) circles and [genus](#genus-of-a-surface). An [orientable](differential-geometry.md#orientable-surface) [surface](#topological-surface) of [genus](#genus-of-a-surface) $g$ has [Euler characteristic](homology.md#euler-characteristic) $2-2g-b$; a [surface](#topological-surface) which is not [orientable](differential-geometry.md#orientable-surface) with $r$ crosscaps has [Euler characteristic](homology.md#euler-characteristic) $2-r-b$. In particular, a closed [connected](geometry-and-topology.md#connected-space) [surface](#topological-surface) with vanishing first mod-two [homology](homology.md) is a [sphere](geometry-and-topology.md#sphere), and a [connected](geometry-and-topology.md#connected-space) closed [orientable](differential-geometry.md#orientable-surface) [surface](#topological-surface) of [Euler characteristic](homology.md#euler-characteristic) zero is a [torus](#torus).

### Thrice-punctured sphere

↑ **Parent:** [Topological surface](#topological-surface)

The sphere with three points removed is an orientable noncompact surface of genus zero with three ends. It can be realized by pairing the two sides at each of two opposite ideal vertices of an [ideal hyperbolic quadrilateral](geometry-and-topology.md#ideal-hyperbolic-quadrilateral) in the [hyperbolic disk](geometry-and-topology.md#hyperbolic-disc). The four ideal vertices fall into three equivalence classes; after adding these three points the cell structure has one face, two edges and three vertices, hence [Euler characteristic](homology.md#euler-characteristic) two. Removing these added vertices recovers the original quotient.

### Integral top homology of a compact connected surface

↑ **Parent:** [Topological surface](#topological-surface)

For a compact connected surface $S$,

$$
H_2(S;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&S\text{ is closed and orientable},\\
0,&S\text{ is nonorientable or has nonempty boundary}.
\end{cases}
$$

In particular, its second integral homology has rank at most one.

### Surface with boundary

↑ **Parent:** [Topological surface](#topological-surface)

A surface with boundary is a two-dimensional [manifold with boundary](differential-geometry.md#manifold-with-boundary): it is locally homeomorphic to the plane or to the closed upper half-plane. Points represented on the edge of a half-plane chart form its one-dimensional boundary.

#### Topology of disk tiles glued along disjoint boundary arcs

↑ **Parent:** [Surface with boundary](#surface-with-boundary)

Consider a connected assembly of $n$ [closed discs](#closed-disc) formed by identifying $e$ pairs of boundary arcs, each arc used once and all arcs in a given tile having disjoint endpoints. Its gluing [graph](graph.md) has one vertex per tile and one edge per paired arc. A [spanning tree](combinatorics.md#spanning-tree) joins the initial discs into a single [closed disc](#closed-disc); each of the remaining $e-n+1$ pairings attaches a band. This is a thickening of the gluing [graph](graph.md), so it is [homotopy equivalent](algebraic-topology.md#homotopy-inverse) to that [graph](graph.md). Thus its [Euler characteristic](homology.md#euler-characteristic) is $n-e$ and its [fundamental group](algebraic-topology.md#fundamental-group) is the [free group](geometric-group-theory.md#free-group) $F_{e-n+1}$. If the gluing [graph](graph.md) is a tree, the assembled surface is itself a [closed disc](#closed-disc).

Suppose each pairing preserves the positive boundary parameter of the reference discs. A global [orientation](algebraic-topology.md#orientation-of-a-simplex) must then assign opposite orientation signs to adjacent tiles, because their induced [boundary orientations](differential-geometry.md#boundary-orientation) on an interior seam must oppose one another. Such signs exist exactly when the gluing [graph](graph.md) is [bipartite](graph-theory.md#bipartite-graph). An odd gluing cycle therefore proves that the assembly is a [nonorientable surface](#non-orientable-surface). A [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) or a [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) on an unpaired arc has no effect on this topological calculation.

#### Pair of pants (mathematics)

↑ **Parent:** [Surface with boundary](#surface-with-boundary)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pair_of_pants_(mathematics))

The pair of pants is the compact genus-zero [surface with boundary](#surface-with-boundary) having three boundary components. It is obtained from the sphere by deleting the interiors of three disjoint discs and is homotopy equivalent to a wedge of two circles.

##### Hyperbolic Y-piece

↑ **Parent:** [Pair of pants (mathematics)](#pair-of-pants-mathematics)

A [Y-piece](#hyperbolic-y-piece) is a compact curvature-$-1$ [hyperbolic surface](geometry-and-topology.md#hyperbolic-surface) homeomorphic to a [pair of pants](#pair-of-pants-mathematics), with three geodesic boundary curves. Its labelled boundary lengths $\ell_1,\ell_2,\ell_3>0$ determine it up to [isometry](riemannian-geometry.md#isometry). Cutting along the three mutually perpendicular seams produces two congruent [right-angled hyperbolic hexagons](geometry-and-topology.md#right-angled-hyperbolic-hexagon) with alternating sides $\ell_i/2$. Conversely, doubling the hexagon along its other three sides constructs the [Y-piece](#hyperbolic-y-piece) for arbitrary positive lengths.

###### Hyperbolic X-piece

↑ **Parent:** [Hyperbolic Y-piece](#hyperbolic-y-piece)

An [X-piece](#hyperbolic-x-piece) is a curvature-$-1$ four-holed sphere with geodesic boundary, formed by gluing two [Y-pieces](#hyperbolic-y-piece) along equal-length cuffs. For a specified separating cuff and labelled outer boundaries, four outer lengths, the internal cuff length $s>0$, and a twist $\tau$ determine the metric. The gluing is orientation-reversing on boundary circles, with relative arclength displacement $\tau$ measured from chosen seam endpoints. Without markings, the gluing displacement is taken modulo $s$; with a marking, $\tau\in\mathbb R$ records [Dehn twists](#dehn-twist) as well. Changing the chosen separating curve can give different parameter descriptions of the same unmarked surface.

##### Homology action of a pair-of-pants homeomorphism

↑ **Parent:** [Pair of pants (mathematics)](#pair-of-pants-mathematics)

Orient the three boundary classes $c_1,c_2,c_3$ so that $c_1+c_2+c_3=0$ in $H_1(N;\mathbb Z)$. A homeomorphism with orientation sign $\epsilon$ and boundary permutation $\sigma$ sends $c_i$ to $\epsilon c_{\sigma(i)}$. Its trace on the rank-two quotient of $\mathbb Z^3$ by $c_1+c_2+c_3$ is therefore $\epsilon(\#\operatorname{Fix}\sigma-1)$.

### Genus of a surface

↑ **Parent:** [Topological surface](#topological-surface)

The genus counts the handles of a connected closed orientable surface. Such a surface has [Euler characteristic](homology.md#euler-characteristic) $2-2g$.

#### Genus monotonicity under nonzero-degree surface maps

↑ **Parent:** [Genus of a surface](#genus-of-a-surface)

For a [continuous map](#continuous-map) of nonzero [mapping degree](homology.md#degree-of-a-continuous-mapping) between closed connected oriented surfaces, [rational cohomology injectivity of a nonzero-degree map](cohomology.md#rational-cohomology-injectivity-of-a-nonzero-degree-map) gives an injection on $H^1$. Since the first [Betti number](homology.md#betti-number) of an oriented surface of genus $g$ is $2g$, the source genus is at least the target genus.

### Closed orientable surface

↑ **Parent:** [Topological surface](#topological-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed_orientable_surface)

A closed orientable surface of genus $g$ is homeomorphic to a sphere with $g$ handles. Its Euler characteristic is $2-2g$.

#### Genus of a finite cover of a closed orientable surface

↑ **Parent:** [Closed orientable surface](#closed-orientable-surface)

A connected $n$-sheeted [covering space](algebraic-topology.md#covering-space) of a [closed orientable surface](#closed-orientable-surface) of genus $g$ has genus $1+n(g-1)$. Lifting a finite cell decomposition gives $n$ cells above every base cell, so its [Euler characteristic](homology.md#euler-characteristic) is $n(2-2g)$. Equating this with $2-2g'$ gives the formula. For $g\ge1$, every positive $n$ occurs: send one handle generator of the [fundamental group](algebraic-topology.md#fundamental-group) to $1$ in $\mathbb Z/n$ and all remaining generators to zero, then use the [classification of connected covering spaces](algebraic-topology.md#classification-of-connected-covering-spaces) for the kernel of that surjection.

### Non-orientable surface

↑ **Parent:** [Topological surface](#topological-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Non-orientable_surface)

A non-orientable surface has no consistent choice of local orientation.

#### Closed nonorientable surface

↑ **Parent:** [Non-orientable surface](#non-orientable-surface)

A connected closed nonorientable surface of crosscap genus $k$ is the connected sum of $k$ real projective planes and has Euler characteristic $2-k$.

### Surface quotient by a free finite action

↑ **Parent:** [Topological surface](#topological-surface)

A free action of a finite group on a topological surface has a surface quotient: sufficiently small coordinate discs have disjoint translates and descend homeomorphically to quotient neighbourhoods.

### Jordan curve theorem

↑ **Parent:** [Topological surface](#topological-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jordan_curve_theorem)

Every simple closed curve on the sphere separates it into two connected components, each having the curve as its boundary.

#### Jordan separation from the exponential quotient

↑ **Parent:** [Jordan curve theorem](#jordan-curve-theorem)

For a [compact](#compact-space) set $J$ homeomorphic to a circle, lifting an argument along its parametrization identifies the quotient by continuous exponentials with $\mathbb Z$. By [planar logarithm factorization](functional-analysis.md#planar-logarithm-factorization) it is also free abelian on the bounded complementary components, so exactly one exists. A proper [closed](#closed-set) arc has trivial exponential quotient, and therefore connected complement. Given a small [open](#open-set) arc of $J$ inside any neighborhood of a point, join points from the two complementary regions by a path avoiding the remaining [closed](#closed-set) arc. The first and last intersections with $J$ occur in the small arc, proving that the neighborhood meets both regions. Thus $J$ is the common [boundary](#boundary-of-a-set) of its unique bounded and unbounded regions.

#### Jordan domain

↑ **Parent:** [Jordan curve theorem](#jordan-curve-theorem)

A Jordan domain is the bounded complementary component of a closed [simple curve](#simple-curve) in the plane. The [Jordan curve theorem](#jordan-curve-theorem) separates the plane into this inside component and one unbounded outside component. A [conformal bijection](complex-analysis.md#biholomorphism) from the disc or [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) to this [simply connected](algebraic-topology.md#simply-connected-space) domain extends to a homeomorphism of their closed conformal boundaries by the [Caratheodory boundary extension theorem](complex-analysis.md#caratheodory-boundary-extension-theorem).

#### Schoenflies theorem

↑ **Parent:** [Jordan curve theorem](#jordan-curve-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schoenflies_theorem)

A Jordan curve in the two-sphere is carried to an equator by a homeomorphism of the sphere; equivalently, the closures of its two complementary regions are discs. This strengthens the separation assertion of the [Jordan curve theorem](#jordan-curve-theorem) and controls the boundary degrees of characteristic maps for cell decompositions of a surface.

#### Outer boundary of a planar compact set

↑ **Parent:** [Jordan curve theorem](#jordan-curve-theorem)

The outer boundary of a compact planar set $K$ is the boundary of the unbounded component $C_\infty(K)$ of its complement. Its filled hull is $\mathbb C\setminus C_\infty(K)$. When the outer boundary is a [simple closed curve](geometry-and-topology.md#simple-closed-curve), the hull is its closed interior. For a simply connected open domain $U$, containment of a compact trace and of its filled hull are equivalent. This lets outer-boundary pushforwards retain simply connected domain-containment information.

### Moore triod theorem

↑ **Parent:** [Topological surface](#topological-surface)

A simple triod is the union of three arcs that share one endpoint and are otherwise disjoint. The Moore triod theorem states that every pairwise disjoint family of simple triods in the plane is countable. One proof chooses data from a countable basis of open disks around each branch point; the [Jordan curve theorem](#jordan-curve-theorem) shows that two disjoint triods cannot determine the same finite basis data, giving an injection into a countable set of finite tuples.

### Polygonal schema

↑ **Parent:** [Topological surface](#topological-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polygonal_schema)

A polygonal schema constructs a surface by identifying paired polygon edges.

#### Polygonal-schema Euler count

↑ **Parent:** [Polygonal schema](#polygonal-schema)

Identifying the $2n$ sides of one polygon in pairs gives a cell structure with one face, $n$ edges and some number $V$ of vertex classes. For a closed orientable surface of genus $g$,

$$
V-n+1=2-2g.
$$

Since $V\geq1$, every such schema satisfies $n\geq2g$.

#### Regular hyperbolic octagon fundamental polygon

↑ **Parent:** [Polygonal schema](#polygonal-schema)

A regular hyperbolic octagon with opposite sides paired gives a genus-two surface when each angle is $\pi/4$. The eight vertices then form one smooth quotient point because their angles sum to $2\pi$.

### Mapping class group

↑ **Parent:** [Topological surface](#topological-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mapping_class_group)

The mapping class group $\operatorname{Mod}(S)$ of an oriented surface $S$ is the group of orientation-preserving self-homeomorphisms of $S$ modulo [isotopy](differential-geometry.md#isotopy). It acts on isotopy classes of curves and arcs.

#### Mapping class

↑ **Parent:** [Mapping class group](#mapping-class-group)

A mapping class is an [isotopy](differential-geometry.md#isotopy) class of self-homeomorphisms of a surface. Orientation-preserving classes form the [mapping class group](#mapping-class-group). Acting on markings changes a point of [Teichmüller space](complex-analysis.md#teichmuller-space) while preserving the underlying unmarked [Riemann surface](complex-analysis.md#riemann-surfaces).

#### Injection of a finite hyperbolic isometry group into a mapping class group

↑ **Parent:** [Mapping class group](#mapping-class-group)

If a finite group $G$ acts faithfully by orientation-preserving isometries on a closed hyperbolic surface $S$ of genus at least two, then $G\hookrightarrow\operatorname{Mod}(S)$. An isometry isotopic to the identity induces an inner automorphism of the surface group; its suitable lift commutes with every deck transformation and fixes their limit set, forcing the lift and the original isometry to be the identity.

#### Realization of a finite group as a surface deck group

↑ **Parent:** [Mapping class group](#mapping-class-group)

Every finite group $G$ is the deck group of a connected finite regular covering of some closed orientable surface of genus at least two. Choose a surface group that surjects onto $G$ and take the covering corresponding to the kernel. The resulting free action embeds $G$ into the mapping class group of the covering surface.

#### Dehn twist

↑ **Parent:** [Mapping class group](#mapping-class-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dehn_twist)

A Dehn twist $T_\gamma$ cuts an oriented surface along a simple closed curve $\gamma$, rotates one side once, and glues it back. If a curve or arc $\alpha$ has nonzero geometric intersection with $\gamma$, the iterates $T_\gamma^n(\alpha)$ usually represent distinct isotopy classes, with intersection numbers growing linearly in $|n|$.

##### Lickorish-Dehn theorem

↑ **Parent:** [Dehn twist](#dehn-twist)

The [mapping class group](#mapping-class-group) of a compact connected oriented [topological surface](#topological-surface), for orientation-preserving maps fixing its boundary pointwise and isotopies relative to that boundary, is generated by [Dehn twists](#dehn-twist) about simple closed curves. Boundary-parallel twists are allowed. For a closed surface of positive genus a finite generating collection exists. Permuting boundary components requires additional generators if that larger group is used.

##### Homology action of a Dehn twist

↑ **Parent:** [Dehn twist](#dehn-twist)

If $\gamma\cdot u$ uses the ordered-tangent orientation convention for [algebraic intersection number of curves on an oriented surface](#algebraic-intersection-number-of-curves-on-an-oriented-surface), a [right-handed Dehn twist](#right-handed-dehn-twist) takes $u$ to $u+([\gamma]\cdot u)[\gamma]$ on [first homology](homology.md#first-homology). In particular a separating-curve twist acts trivially there.

##### Right-handed Dehn twist

↑ **Parent:** [Dehn twist](#dehn-twist)

In orientation-preserving annular coordinates $(\theta,r)$ with orientation $d\theta\wedge dr$, the twist is $(\theta,r)\mapsto(\theta+2\pi f(r),r)$, where $f$ increases from zero to one. The map is the identity outside this [annulus](#annulus-mathematics) and near its boundary. The orientation of the ambient [topological surface](#topological-surface), rather than the orientation assigned to the curve, fixes the handedness.

#### Essential proper arc on a punctured surface

↑ **Parent:** [Mapping class group](#mapping-class-group)

A proper arc on a punctured surface approaches punctures at both ends. It is simple when its interior is embedded, and essential when it cannot be isotoped, relative to its ends, into a puncture.

##### Bigon formed by two arcs

↑ **Parent:** [Essential proper arc on a punctured surface](#essential-proper-arc-on-a-punctured-surface)

Two transverse arcs form a bigon when subarcs between two consecutive intersection points together bound an embedded disc whose interior is disjoint from both arcs. Pushing one side across the disc removes the two corner intersections.

##### Minimal position of curves or arcs

↑ **Parent:** [Essential proper arc on a punctured surface](#essential-proper-arc-on-a-punctured-surface)

Two curves or proper arcs are in minimal position when their number of transverse intersection points is the least possible among representatives of their isotopy classes.

###### Bigon criterion

↑ **Parent:** [Minimal position of curves or arcs](#minimal-position-of-curves-or-arcs)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bigon_criterion)

Two transverse essential simple curves or proper arcs on a surface are in [minimal position](#minimal-position-of-curves-or-arcs) exactly when they form no [bigon](#bigon-formed-by-two-arcs). For proper arcs, the proof uses the compactification of the universal cover to control their ends at punctures.

#### Geometric intersection number

↑ **Parent:** [Mapping class group](#mapping-class-group)

The geometric intersection number $i(\alpha,\beta)$ is the minimum number of transverse intersection points among representatives of the isotopy classes of $\alpha$ and $\beta$. Representatives in [minimal position](#minimal-position-of-curves-or-arcs) realize it.

##### Algebraic intersection number of curves on an oriented surface

↑ **Parent:** [Geometric intersection number](#geometric-intersection-number)

This is the surface curve-pair version of an [intersection number](algebraic-geometry.md#intersection-number-of-a-cartier-divisor-with-a-curve).

For transverse oriented curves on an oriented surface, the algebraic intersection number is the sum of the local signs of their crossings. It depends only on their oriented homology classes and is antisymmetric:

$$
\langle\alpha,\beta\rangle=-\langle\beta,\alpha\rangle.
$$

Its absolute value is at most the [geometric intersection number](#geometric-intersection-number).

###### Isotopy invariance of algebraic intersection number

↑ **Parent:** [Algebraic intersection number of curves on an oriented surface](#algebraic-intersection-number-of-curves-on-an-oriented-surface)

During a generic isotopy of one transverse curve, crossings with a fixed curve can only be created or removed in pairs of opposite local sign. Their signed sum, and hence the algebraic intersection number, is therefore invariant.

#### Arc complex

↑ **Parent:** [Mapping class group](#mapping-class-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arc_complex)

The vertices of the arc complex of a punctured surface $S$ are isotopy classes of unoriented essential simple proper arcs. A finite set spans a simplex when its classes have representatives with pairwise disjoint interiors. The [mapping class group](#mapping-class-group) acts on the complex by simplicial automorphisms.

##### Arc complex of the three-punctured sphere

↑ **Parent:** [Arc complex](#arc-complex)

The three-punctured sphere has six arc classes: one joining each unordered pair of distinct punctures and one returning to each puncture. The three joining arcs span one triangle; for each puncture, its returning arc and the two joining arcs incident to it span another triangle. Its mapping class group is the symmetric group on the three punctures and has two vertex orbits, distinguished by whether the endpoints agree.

##### Arc-complex vertex orbits of the four-punctured sphere

↑ **Parent:** [Arc complex](#arc-complex)

The mapping class group of the four-punctured sphere has two orbits on vertices of its arc complex: arcs whose endpoints are distinct and arcs whose endpoints coincide. Each orbit is infinite, and [Dehn twists](#dehn-twist) exhibit infinitely many classes of the second type based at any fixed puncture.

#### Alexander system

↑ **Parent:** [Mapping class group](#mapping-class-group)

An Alexander system is a finite collection of pairwise nonisotopic essential simple curves and proper arcs in pairwise minimal position, arranged without triple intersections and with no three members intersecting pairwise. Pairwise isotopic Alexander systems can be carried to one another simultaneously by an ambient isotopy.

##### Structure graph of an Alexander system

↑ **Parent:** [Alexander system](#alexander-system)

For a filling [Alexander system](#alexander-system) $\{\alpha_i\}$, the structure graph is the embedded graph

$$
\Gamma=\bigcup_i\alpha_i\cup\partial S,
$$

with vertices at all curve intersections, arc endpoints, and punctures. Its edges are the curve, arc, and boundary segments between consecutive vertices. A homeomorphism preserving the system induces a graph automorphism.

##### Alexander method

↑ **Parent:** [Alexander system](#alexander-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alexander_method)

If an Alexander system fills a surface, a homeomorphism preserving every member up to isotopy is determined up to isotopy by its induced automorphism of the structure graph. A trivial graph action makes it isotopic to the identity; the finite graph automorphism group shows that the pointwise curve-class stabilizer is finite.

###### Alexander trick

↑ **Parent:** [Alexander method](#alexander-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alexander_trick)

A homeomorphism of a closed disc that fixes its boundary pointwise is isotopic relative to the boundary to the identity. Radially interpolate the action toward the center after identifying the disc with the unit ball.

###### Center of the mapping class group of the torus

↑ **Parent:** [Alexander method](#alexander-method)

The center of $\operatorname{Mod}(T^2)$ has order two. A central class commutes with twists about two curves intersecting once, hence preserves both curve classes. The [Alexander method](#alexander-method) reduces it to the identity or the elliptic involution $\iota:x\mapsto-x$, and both are central.

#### Mapping-class action on the outer automorphism group of the fundamental group

↑ **Parent:** [Mapping class group](#mapping-class-group)

A self-homeomorphism of a connected surface induces an automorphism of its fundamental group after a path from the old basepoint to its image is chosen. Changing that path changes the automorphism by an inner automorphism, so isotopy classes define a homomorphism

$$
\operatorname{Mod}(S)\longrightarrow\operatorname{Out}(\pi_1(S)).
$$

#### Pure mapping class group

↑ **Parent:** [Mapping class group](#mapping-class-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pure_mapping_class_group)

The pure mapping class group consists of mapping classes that fix every puncture individually.

##### Point-pushing map

↑ **Parent:** [Pure mapping class group](#pure-mapping-class-group)

Pushing a distinguished puncture once around a loop $\gamma$ defines a mapping class. For a simple loop, the push is the product of opposite Dehn twists about the two boundary components of a thin annular neighborhood of $\gamma$.

###### Birman exact sequence

↑ **Parent:** [Point-pushing map](#point-pushing-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Birman_exact_sequence)

For a finite-type surface $S$ of negative Euler characteristic and the surface $S^*$ obtained by adding a puncture, forgetting that puncture gives

$$
1\longrightarrow\pi_1(S)\xrightarrow{\operatorname{Push}}
\operatorname{PMod}(S^*)\longrightarrow\operatorname{PMod}(S)\longrightarrow1.
$$

##### Pure mapping class group of the three-punctured sphere

↑ **Parent:** [Pure mapping class group](#pure-mapping-class-group)

The pure mapping class group of the three-punctured sphere is trivial. The three simple arcs joining distinct puncture pairs form an ideal triangulation; a pure homeomorphism can be isotoped to fix these arcs, and the [Alexander trick](#alexander-trick) on the two complementary discs finishes the isotopy to the identity.

##### Pure mapping class group of the four-punctured sphere

↑ **Parent:** [Pure mapping class group](#pure-mapping-class-group)

The [Birman exact sequence](#birman-exact-sequence) and $\operatorname{PMod}(S_{0,3})=1$ identify $\operatorname{PMod}(S_{0,4})$ with $\pi_1(S_{0,3})$, the free group of rank two.

##### Semidirect-product decomposition of the pure mapping class group of the five-punctured sphere

↑ **Parent:** [Pure mapping class group](#pure-mapping-class-group)

Forgetting the fifth puncture gives a split [Birman exact sequence](#birman-exact-sequence)

$$
1\to F_3\to\operatorname{PMod}(S_{0,5})\to F_2\to1.
$$

Lifts of two free generators generate a copy of $F_2$ meeting the point-pushing kernel $F_3$ trivially.

#### Curve complex

↑ **Parent:** [Mapping class group](#mapping-class-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Curve_complex)

The vertices of the curve complex are isotopy classes of essential simple closed curves. Distinct vertices span a simplex when they have pairwise disjoint representatives.

##### Connectedness of the curve complex

↑ **Parent:** [Curve complex](#curve-complex)

For every connected orientable surface of complexity above one, the one-skeleton of the curve complex is connected. Surgery replaces one curve by an essential curve disjoint from it while reducing intersection with a fixed target; induction on geometric intersection number gives a path.

##### Filling set of curves

↑ **Parent:** [Curve complex](#curve-complex)

A collection of curves fills a surface when every essential simple closed curve intersects at least one member. For curves in minimal position on a closed surface, this is equivalent to every complementary component being a disc.

###### Filling pair on a closed genus-two surface

↑ **Parent:** [Filling set of curves](#filling-set-of-curves)

Split a closed genus-two surface along a separating curve $\alpha$ into two one-holed tori. In each torus choose two disjoint proper arcs that cut it into a disc, and match their four endpoints across $\alpha$ so that the four arcs join into one simple closed curve $\beta$. Then $i(\alpha,\beta)=4$ and the complement of $\alpha\cup\beta$ is two discs, so the pair fills.

### Torus

↑ **Parent:** [Topological surface](#topological-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Torus)

The torus is the product of two circles and can be formed by identifying opposite sides of a square.

#### Three-critical-point function on a torus

↑ **Parent:** [Torus](#torus)

Take $u,v$ modulo $\pi$; shifting either coordinate by $\pi$ leaves $h$ unchanged. Its partial derivatives are $h_u=\sin v\sin(2u-v)$ and $h_v=\sin u\sin(u-2v)$. The only [critical points](analysis.md#critical-point) are $(0,0)$, $(\pi/3,2\pi/3)$ and $(2\pi/3,\pi/3)$. The latter are a nondegenerate minimum and maximum, with values $\mp3\sqrt3/8$. At the origin the leading cubic is $uv(u-v)$, linearly equivalent to a [monkey saddle](analysis.md#monkey-saddle); its [critical point](analysis.md#critical-point) is isolated but degenerate. Thus three smooth [critical points](analysis.md#critical-point) coexist with the Morse lower bound of four for the [torus](#torus).

#### Pinched torus

↑ **Parent:** [Torus](#torus)

Collapsing an essential meridian circle of a [torus](#torus) to one point gives the [pinched torus](#pinched-torus). In the [torus](#torus)'s CW structure, the two-cell attaches to two circles by the [commutator](lie-algebra.md#commutator). Collapsing one circle leaves one one-cell and a two-cell attached by a [null-homotopic](algebraic-topology.md#null-homotopic-map) word. Thus the quotient is homotopy equivalent to $S^1\vee S^2$. Its cellular chain groups are $\mathbb Z$ in degrees zero, one and two, with zero differentials, so its integral [homology groups](homology.md#homology-group) are $H_0=H_1=H_2=\mathbb Z$ and vanish in all higher degrees. This illustrates that collapsing a circle can preserve a top-dimensional homology class even while reducing the first homology rank.

#### Three-dimensional torus

↑ **Parent:** [Torus](#torus)

The product of three circles is a compact smooth three-manifold. Quotient coordinates allow constant commuting [vector fields](calculus.md#vector-field). A rank-two plane field can have dense immersed leaves, as in a [dense immersed cylinder in a three-dimensional torus](differential-geometry.md#dense-immersed-cylinder-in-a-three-dimensional-torus).

#### Cohomology ring of a torus

↑ **Parent:** [Torus](#torus)

Since $T^r$ is a product of circles, the [Künneth theorem](cohomology.md#kunneth-theorem) identifies its [cohomology ring](cohomology.md#cohomology-ring) with the [exterior algebra](linear-algebra.md#exterior-algebra) on the coordinate degree-one classes. Inversion negates each integral degree-one class, so it acts as $(-1)^q$ in degree $q$. Even in characteristic two, each degree-one class has square zero.

#### Homology of an integer torus endomorphism

↑ **Parent:** [Torus](#torus)

On the [torus](#torus) $\mathbb R^d/\mathbb Z^d$, an integer [matrix](vector-space.md#matrix) $A$ defines an [endomorphism](algebra.md#endomorphism). The coordinate circles give a basis of the [first homology group](homology.md#first-homology), and the induced map on that group is $A$. The [Künneth theorem](cohomology.md#kunneth-theorem) identifies higher [integral homology](homology.md#integral-homology) with the [exterior powers](linear-algebra.md#exterior-power) of $\mathbb Z^d$, so the degree-$q$ map is $\bigwedge^q A$. In top degree it is multiplication by $\det A$. The map is a [homeomorphism](#homeomorphism) precisely when $A$ is a [unimodular matrix](linear-algebra.md#unimodular-matrix); a merely nonsingular integer [matrix](vector-space.md#matrix) need not have an integer inverse.

#### Solid torus

↑ **Parent:** [Torus](#torus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Solid_torus)

A solid torus is the product of a circle with a closed disk. Its boundary is the [torus](#torus) $S^1\times S^1$. It deformation retracts onto its central circle, so its degree-one [de Rham cohomology](differential-form.md#de-rham-cohomology) is one dimensional and injects into that of its boundary.

##### Solid-torus recognition by a compression disk

↑ **Parent:** [Solid torus](#solid-torus)

A compact orientable [irreducible three-manifold](#irreducible-three-manifold) with connected torus boundary which is compressible is a [solid torus](#solid-torus). Compressing along a [compression disk](#compression-disk) gives an embedded sphere. The compressed component has one sphere boundary and irreducibility makes it a ball; undoing compression attaches one one-handle, giving $D^2\times S^1$.

##### Meridian of a solid torus

↑ **Parent:** [Solid torus](#solid-torus)

A meridian of a [solid torus](#solid-torus) is a primitive curve on its boundary that bounds an embedded disk in the [solid torus](#solid-torus).

#### Embedding of the n-dimensional torus in codimension one

↑ **Parent:** [Torus](#torus)

Suppose a compact $m$-manifold $N$ is embedded in the half-space $x_{m+1}>0$ of $\mathbb R^{m+1}$. Spinning it around the boundary hyperplane gives the embedding

$$
N\times S^1\longrightarrow\mathbb R^{m+2},
\qquad
(x,e^{i\theta})\longmapsto
(x_1,\ldots,x_m,x_{m+1}\cos\theta,x_{m+1}\sin\theta).
$$

Starting with a circle and iterating proves that $T^n=(S^1)^n$ embeds in $\mathbb R^{n+1}$.

#### Embedded torus of revolution

↑ **Parent:** [Torus](#torus)

For major radius $R$ and minor radius $r$ with $R>r>0$, the standard embedded torus of revolution in $\mathbb R^3$ is

$$
(\sqrt{x^2+y^2}-R)^2+z^2=r^2.
$$

It is parametrized by

$$
(s,t)\longmapsto
\bigl((R+r\cos 2\pi t)\cos2\pi s,
(R+r\cos2\pi t)\sin2\pi s,
r\sin2\pi t\bigr),
$$

which identifies the opposite sides of the unit square.

#### Fundamental group of the torus

↑ **Parent:** [Torus](#torus)

For the standard longitude $a$ and meridian $b$,

$$
\pi_1(T^2)\cong\langle a,b\mid[a,b]=1\rangle\cong\mathbb Z^2.
$$

##### Lift-endpoint description of the fundamental group of the torus

↑ **Parent:** [Fundamental group of the torus](#fundamental-group-of-the-torus)

For the universal covering

$$
p:\mathbb R^2\to S^1\times S^1,
\qquad
p(r_1,r_2)=(e^{2\pi i r_1},e^{2\pi i r_2}),
$$

lift a based loop from the origin. Its endpoint lies in the fibre $\mathbb Z^2$, depends only on its based homotopy class, and turns concatenation into addition. This gives a natural isomorphism $\pi_1(T^2)\simeq\mathbb Z^2$.

#### Integral linear automorphism of the torus

↑ **Parent:** [Torus](#torus)

Every $A\in GL_2(\mathbb Z)$ induces a based homeomorphism

$$
f_A:\mathbb R^2/\mathbb Z^2\to\mathbb R^2/\mathbb Z^2,
\qquad
f_A([r])=[Ar].
$$

Its inverse is $f_{A^{-1}}$, and under the [lift-endpoint description of the fundamental group of the torus](#lift-endpoint-description-of-the-fundamental-group-of-the-torus), its induced map on $\pi_1(T^2)$ is multiplication by $A$.

##### Equivalence of connected double covers of the torus

↑ **Parent:** [Integral linear automorphism of the torus](#integral-linear-automorphism-of-the-torus)

Any two connected degree-two coverings of the torus fit into a commuting square with homeomorphisms of their total and base spaces. They correspond to index-two subgroups of $\mathbb Z^2$, which are kernels of the three nonzero maps $\mathbb Z^2\to\mathbb Z/2\mathbb Z$. Reduction modulo two shows that $GL_2(\mathbb Z)$ acts transitively on these subgroups; the [classification of connected covering spaces](algebraic-topology.md#classification-of-connected-covering-spaces) and the [lifting criterion for a covering space](algebraic-topology.md#lifting-criterion-for-a-covering-space) then supply the homeomorphism of total spaces.

<h3 id="mobius-band">Möbius band</h3>

↑ **Parent:** [Topological surface](#topological-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Möbius_band)

The Möbius band deformation retracts onto its core circle. Under this retraction its boundary circle has degree two, so the boundary class is the square of the core class in the fundamental group.

### Klein bottle

↑ **Parent:** [Topological surface](#topological-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Klein_bottle)

The Klein bottle is obtained from a square by identifying one pair of opposite sides with matching direction and the other pair with reversed direction.

#### Mod-two intersection pairing of the Klein bottle

↑ **Parent:** [Klein bottle](#klein-bottle)

A one-sided section loop and a two-sided fiber loop in the reflection [mapping torus](algebraic-topology.md#mapping-torus) have mod-two self-intersections one and zero and meet once. Their [intersection form](homology.md#intersection-form) is $Q$. In the evaluation-dual [cohomology](cohomology.md) basis, the [Poincare duality pairing](cohomology.md#poincare-duality-pairing) has matrix $Q^{-1}$, giving $t^2=0$ and $x^2=tx\ne0$.

#### Integral cohomology ring of the Klein bottle

↑ **Parent:** [Klein bottle](#klein-bottle)

The integral cohomology groups of the Klein bottle are $H^0(K;\mathbb Z)=\mathbb Z$, $H^1(K;\mathbb Z)=\mathbb Z$, $H^2(K;\mathbb Z)=\mathbb Z/2$, and zero in higher degrees. The degree-one generator is pulled back from the base circle of the circle-bundle presentation, so its square is zero; hence every product of positive-degree classes vanishes.

##### Integral cohomology ring of the wedge of the real projective plane and a circle

↑ **Parent:** [Integral cohomology ring of the Klein bottle](#integral-cohomology-ring-of-the-klein-bottle)

The wedge $\mathbb{RP}^2\vee S^1$ has the same additive integral cohomology as the [Klein bottle](#klein-bottle): $\mathbb Z$ in degree zero, $\mathbb Z$ in degree one, and $\mathbb Z/2$ in degree two. Products of positive-degree classes vanish because the degree-one class comes from the circle summand, so its [cohomology ring](cohomology.md#cohomology-ring) is isomorphic to that of the Klein bottle.

#### Orientation double cover of the Klein bottle

↑ **Parent:** [Klein bottle](#klein-bottle)

For

$$
(x,y)\simeq(x+c,(-1)^cy+d),
$$

the transformations with even $c$ form an index-two translation subgroup. Its quotient is a torus, giving the orientation double cover $T^2\to K$.

##### Klein-bottle mapping-cylinder obstruction to simple connectivity

↑ **Parent:** [Orientation double cover of the Klein bottle](#orientation-double-cover-of-the-klein-bottle)

Let $Y$ be the mapping cylinder of the orientation double cover $T^2\to K$ with its free end omitted. If a Hausdorff space contains $Y$ as an open subset, van Kampen extends the orientation quotient of $\pi_1(K)$ to a surjection of the ambient fundamental group onto $C_2$. The ambient space is therefore not simply connected.

#### Flat Klein-bottle geodesic model

↑ **Parent:** [Klein bottle](#klein-bottle)

In a flat fundamental square, straight horizontal, vertical and rational-slope lines project to closed geodesics. The central horizontal glide axis is one-sided, a vertical line is two-sided, and the line $(2t,t)$ closes with one transverse self-intersection.

### Double cone singularity

↑ **Parent:** [Topological surface](#topological-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Double_cone_singularity)

The vertex of a double cone is not a surface point because its punctured neighborhood disconnects into two pieces.

## Knaster-Kuratowski-Mazurkiewicz lemma

↑ **Parent:** [Topology](topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Knaster–Kuratowski–Mazurkiewicz_lemma)

For a simplex with vertices indexed by $0,\ldots,n$, let closed sets $F_i$ have the property that every face spanned by an index set $I$ lies in $\bigcup_{i\in I}F_i$. Then $\bigcap_{i=0}^nF_i$ is nonempty. The [triangle KKM lemma](#triangle-kkm-lemma) is a two-dimensional covering formulation of this simplex-intersection principle.

### Triangle KKM lemma

↑ **Parent:** [Knaster-Kuratowski-Mazurkiewicz lemma](#knaster-kuratowski-mazurkiewicz-lemma)

If three closed sets cover a triangle and respectively contain its three opposite sides, then their triple intersection is nonempty.

#### Distance-function barycentric map

↑ **Parent:** [Triangle KKM lemma](#triangle-kkm-lemma)

Normalized distances to three closed sets give continuous barycentric coordinates; a covering forces at least one coordinate to vanish, placing the image on the simplex boundary.

#### No-retraction covering principle

↑ **Parent:** [Triangle KKM lemma](#triangle-kkm-lemma)

A closed-cover intersection statement for a simplex is equivalent to the nonexistence of a boundary-valued map that preserves every face.

## ↑ Ancestors (4)

1. [Geometry and topology](geometry-and-topology.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (76)

- [Cantor space](geometry-and-topology.md#cantor-space)
- [Closed convex hull](mathematical-optimization.md#closed-convex-hull)
- [Completely regular Hausdorff space](#completely-regular-hausdorff-space)
- [Cone on an infinite coinfinite ground set](ramsey-theory.md#cone-on-an-infinite-coinfinite-ground-set)
- [Continuous real maps from the initial-segment topology](#continuous-real-maps-from-the-initial-segment-topology)
- [Convergence of a filter](set-theory.md#convergence-of-a-filter)
- [Countable product compactness implies countable choice](set-theory.md#countable-product-compactness-implies-countable-choice)
- [Embedding](geometry-and-topology.md#embedding)
- [Equivalent absolute values](arithmetic.md#equivalent-absolute-values)
- [Finite subsets do not define a topology on an infinite set](#finite-subsets-do-not-define-a-topology-on-an-infinite-set)
- [Flat linearized metric perturbations are locally pure gauge](general-relativity.md#flat-linearized-metric-perturbations-are-locally-pure-gauge)
- [Function space](functional-analysis.md#function-space)
- [Gamma-convergence](calculus-of-variations.md#gamma-convergence)
- [Irreducible closed subset](algebraic-geometry.md#irreducible-closed-subset)
- [Lexicographic order topology on the real plane](set.md#lexicographic-order-topology-on-the-real-plane)
- [Nottingham group](topological-group.md#nottingham-group)
- [Open normal subgroup](topological-group.md#open-normal-subgroup)
- [Original and weak continuity of linear maps between Fréchet spaces](weak-topology.md#original-and-weak-continuity-of-linear-maps-between-frechet-spaces)
- [Parameter continuity of variational regularization](inverse-problem.md#parameter-continuity-of-variational-regularization)
- [Partition topology](#partition-topology)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3.md#1a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-68.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2.md#13g/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2.md#13g/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2.md#13g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-10.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-2.md#4e/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-2.md#4e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-11.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-11.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-20.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2.md#15e/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2.md#4e/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-12.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-6.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-3.md#4a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-16.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-26.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-26.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3.md#4f/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-2.md#4a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-2.md#4a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3.md#4a/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-5.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-5.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-5.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1.md#12f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1.md#12f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1.md#12f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1.md#12f/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1.md#12f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-3.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-24.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-5.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3.md#4c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-24.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-24.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4.md#10f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-4.md#13e/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#1/1/2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#1/1/2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2.md#2e/solution)
- [Point of a frame](category-theory.md#point-of-a-frame)
- [Pro-p ring](commutative-algebra.md#pro-p-ring)
- [Profinite topology on the integers is not compact](topological-group.md#profinite-topology-on-the-integers-is-not-compact)
- [Sublevel set](calculus.md#sublevel-set)
- [Tail topology on the natural numbers](#tail-topology-on-the-natural-numbers)
- [Topological ring](commutative-algebra.md#topological-ring)
- [Topologies on integral formal power series](commutative-algebra.md#topologies-on-integral-formal-power-series)
- [Topology determines norm equivalence](functional-analysis.md#topology-determines-norm-equivalence)
- [Trivial absolute value](arithmetic.md#trivial-absolute-value)
- [Upper-ray topology on the real line](#upper-ray-topology-on-the-real-line)
