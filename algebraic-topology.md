# Algebraic topology

↑ **Parent:** [Geometry and topology](geometry-and-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_topology)

**Table of contents**

- [Intersection homology](#intersection-homology)
  - [Perversity](#perversity)
    - [Allowable singular simplex](#allowable-singular-simplex)
      - [Intersection chains](#intersection-chains)
    - [Upper middle perversity](#upper-middle-perversity)
    - [Lower middle perversity](#lower-middle-perversity)
  - [Intersection homology cone formula](#intersection-homology-cone-formula)
    - [Intersection homology of an even-dimensional suspension](#intersection-homology-of-an-even-dimensional-suspension)
  - [Intersection cohomology](#intersection-cohomology)
    - [Capped-boundary intersection cohomology](#capped-boundary-intersection-cohomology)
    - [Intersection complex](#intersection-complex)
      - [Intersection-complex support and cosupport axioms](#intersection-complex-support-and-cosupport-axioms)
- [Homotopy colimit of spaces](#homotopy-colimit-of-spaces)
- [Stable homotopy theory](#stable-homotopy-theory)
  - [Universe for spectra](#universe-for-spectra)
    - [Subordinate flag for a family of linear isometries](#subordinate-flag-for-a-family-of-linear-isometries)
  - [Homotopy colimit of spectra](#homotopy-colimit-of-spectra)
    - [Milnor exact sequence for maps of spectra](#milnor-exact-sequence-for-maps-of-spectra)
  - [Cofiber of spectra](#cofiber-of-spectra)
    - [Cofiber sequence of spectra](#cofiber-sequence-of-spectra)
  - [Smash product of spectra](#smash-product-of-spectra)
    - [Function spectrum](#function-spectrum)
      - [Function spectrum with values in a ring spectrum](#function-spectrum-with-values-in-a-ring-spectrum)
  - [Stable homotopy category](#stable-homotopy-category)
    - [Stable equivalence of spectra](#stable-equivalence-of-spectra)
  - [Spectrum (topology)](#spectrum-topology)
    - [Connective spectrum](#connective-spectrum)
      - [Bottom-degree generalized Hurewicz isomorphism](#bottom-degree-generalized-hurewicz-isomorphism)
        - [Connective generalized homology detects simply connected equivalences](#connective-generalized-homology-detects-simply-connected-equivalences)
    - [Ring spectrum](#ring-spectrum)
      - [Commutative ring spectrum](#commutative-ring-spectrum)
    - [Indexed prespectrum](#indexed-prespectrum)
      - [Twisted half-smash product](#twisted-half-smash-product)
        - [Associativity of twisted half-smash products](#associativity-of-twisted-half-smash-products)
      - [Spectrification](#spectrification)
    - [Stable homotopy group](#stable-homotopy-group)
    - [Suspension of spectra](#suspension-of-spectra)
    - [Suspension spectrum](#suspension-spectrum)
      - [Sphere spectrum](#sphere-spectrum)
    - [Cell spectrum](#cell-spectrum)
      - [Finite spectrum](#finite-spectrum)
        - [Spanier-Whitehead dual](#spanier-whitehead-dual)
          - [Spanier-Whitehead duality](#spanier-whitehead-duality)
    - [Omega-spectrum](#omega-spectrum)
    - [Map of topological spectra](#map-of-topological-spectra)
      - [Phantom map of spectra](#phantom-map-of-spectra)
        - [Phantom maps vanish on represented homology](#phantom-maps-vanish-on-represented-homology)
        - [Universal evaluation phantom map](#universal-evaluation-phantom-map)
        - [Hyperphantom map of spectra](#hyperphantom-map-of-spectra)
      - [Spectrum homotopy](#spectrum-homotopy)
- [Based space](#based-space)
- [Lusternik–Schnirelmann category](#lusternik-schnirelmann-category)
  - [Lusternik–Schnirelmann critical point theorem](#lusternik-schnirelmann-critical-point-theorem)
- [Theta graph](#theta-graph)
- [Dumbbell graph](#dumbbell-graph)
- [Borsuk-Ulam theorem](#borsuk-ulam-theorem)
  - [Lusternik–Schnirelmann theorem](#lusternik-schnirelmann-theorem)
    - [Antipodal-free closed cover from simplex Voronoi cells](#antipodal-free-closed-cover-from-simplex-voronoi-cells)
    - [Open-cover proof of the Lusternik-Schnirelmann-Borsuk theorem](#open-cover-proof-of-the-lusternik-schnirelmann-borsuk-theorem)
- [CW complex](#cw-complex)
  - [Compact subsets of CW complexes lie in finite subcomplexes](#compact-subsets-of-cw-complexes-lie-in-finite-subcomplexes)
  - [Skeleton of a CW complex](#skeleton-of-a-cw-complex)
  - [Topological cell](#topological-cell)
  - [CW pair](#cw-pair)
  - [Cell attachment](#cell-attachment)
    - [Homotopy-group effect of attaching higher cells](#homotopy-group-effect-of-attaching-higher-cells)
  - [Weak topology of a CW complex](#weak-topology-of-a-cw-complex)
  - [Graph (topology)](#graph-topology)
  - [CW subcomplex](#cw-subcomplex)
  - [1-skeleton](#1-skeleton)
  - [2-complex](#2-complex)
    - [Disc diagram](#disc-diagram)
      - [Disc diagram ladder](#disc-diagram-ladder)
      - [Disc diagram spur](#disc-diagram-spur)
      - [Disc diagram shell](#disc-diagram-shell)
      - [van Kampen lemma](#van-kampen-lemma)
      - [Reduced disc diagram](#reduced-disc-diagram)
  - [Cellular map](#cellular-map)
    - [Cellular approximation theorem](#cellular-approximation-theorem)
      - [Dimension reduction of sphere maps into CW skeleta](#dimension-reduction-of-sphere-maps-into-cw-skeleta)
  - [Finite CW complex](#finite-cw-complex)
    - [Euclidean embedding by finite cell attachment](#euclidean-embedding-by-finite-cell-attachment)
  - [CW approximation](#cw-approximation)
    - [Finite type CW approximation](#finite-type-cw-approximation)
      - [Finite CW approximation from bounded homology](#finite-cw-approximation-from-bounded-homology)
  - [CW filtration](#cw-filtration)
  - [Moore space (algebraic topology)](#moore-space-algebraic-topology)
    - [Bockstein on a cyclic Moore space](#bockstein-on-a-cyclic-moore-space)
    - [Cyclic Moore space in dimension one](#cyclic-moore-space-in-dimension-one)
- [Mapping cylinder](#mapping-cylinder)
  - [Mapping cone (topology)](#mapping-cone-topology)
    - [Puppe sequence](#puppe-sequence)
    - [Cellular chain complex of a mapping cone](#cellular-chain-complex-of-a-mapping-cone)
    - [Mapping cone exact sequence](#mapping-cone-exact-sequence)
  - [Mapping telescope](#mapping-telescope)
    - [Mapping-telescope realization of the rational group with square-free denominators](#mapping-telescope-realization-of-the-rational-group-with-square-free-denominators)
- [Smash product](#smash-product)
  - [Smash product of CW pairs](#smash-product-of-cw-pairs)
- [Real projective space](#real-projective-space)
  - [Orientability of real projective space](#orientability-of-real-projective-space)
  - [Real projective 3-space](#real-projective-3-space)
  - [Nonsurjective self-map of real projective space is null-homotopic](#nonsurjective-self-map-of-real-projective-space-is-null-homotopic)
  - [Fixed-point-free complex-structure map on odd-dimensional real projective space](#fixed-point-free-complex-structure-map-on-odd-dimensional-real-projective-space)
  - [Integral homology of a circle times a real projective plane](#integral-homology-of-a-circle-times-a-real-projective-plane)
  - [Infinite-dimensional real projective space](#infinite-dimensional-real-projective-space)
  - [Stunted real projective space](#stunted-real-projective-space)
    - [Homotopy groups of the stunted projective space through degree nine](#homotopy-groups-of-the-stunted-projective-space-through-degree-nine)
  - [Steenrod squares on real projective space](#steenrod-squares-on-real-projective-space)
  - [Standard affine atlas of real projective space](#standard-affine-atlas-of-real-projective-space)
  - [Integral cohomology ring of real projective space](#integral-cohomology-ring-of-real-projective-space)
    - [Integral cohomology of a product of finite real projective spaces](#integral-cohomology-of-a-product-of-finite-real-projective-spaces)
  - [Cellular homology of real projective space](#cellular-homology-of-real-projective-space)
  - [Mod-two cohomology ring of real projective space](#mod-two-cohomology-ring-of-real-projective-space)
    - [Gysin proof of mod-two projective-space cohomology](#gysin-proof-of-mod-two-projective-space-cohomology)
    - [Mod-two degree obstruction for equal projective factors](#mod-two-degree-obstruction-for-equal-projective-factors)
  - [Mapping-cylinder model of punctured real projective three-space](#mapping-cylinder-model-of-punctured-real-projective-three-space)
  - [Integral homology of real projective three-space](#integral-homology-of-real-projective-three-space)
  - [Double of punctured real projective three-space](#double-of-punctured-real-projective-three-space)
- [Mapping torus](#mapping-torus)
  - [Unipotent torus-bundle group](#unipotent-torus-bundle-group)
  - [Inversion mapping torus of a torus](#inversion-mapping-torus-of-a-torus)
    - [Mod-two cohomology ring of an inversion mapping torus](#mod-two-cohomology-ring-of-an-inversion-mapping-torus)
    - [Integral cohomology of an inversion mapping torus](#integral-cohomology-of-an-inversion-mapping-torus)
      - [Integral cup products in the four-dimensional inversion mapping torus](#integral-cup-products-in-the-four-dimensional-inversion-mapping-torus)
  - [Fiber monodromy](#fiber-monodromy)
    - [Homological monodromy](#homological-monodromy)
  - [Heisenberg nilmanifold as a torus mapping torus](#heisenberg-nilmanifold-as-a-torus-mapping-torus)
  - [Wang sequence](#wang-sequence)
    - [Homology of the antipodal sphere mapping torus](#homology-of-the-antipodal-sphere-mapping-torus)
      - [Cohomology ring of the antipodal two-sphere mapping torus](#cohomology-ring-of-the-antipodal-two-sphere-mapping-torus)
        - [Mod-two cohomology ring of the antipodal two-sphere mapping torus](#mod-two-cohomology-ring-of-the-antipodal-two-sphere-mapping-torus)
    - [Mapping-torus homology from Mayer–Vietoris](#mapping-torus-homology-from-mayer-vietoris)
- [Homology (mathematics)](homology.md)
  - [Borel-Moore homology](homology.md#borel-moore-homology)
  - [Generalized homology theory](homology.md#generalized-homology-theory)
    - [Represented homology theory](homology.md#represented-homology-theory)
  - [Null-homologous cycle](homology.md#null-homologous-cycle)
  - [Primitive homology class](homology.md#primitive-homology-class)
  - [Acyclic space](homology.md#acyclic-space)
  - [Homology of a directed union](homology.md#homology-of-a-directed-union)
    - [Countability of the homology of an open Euclidean subset](homology.md#countability-of-the-homology-of-an-open-euclidean-subset)
  - [Reduced homology](homology.md#reduced-homology)
  - [Homology group](homology.md#homology-group)
    - [Zeroth homology group](homology.md#zeroth-homology-group)
    - [Homology class](homology.md#homology-class)
  - [Functoriality of homology](homology.md#functoriality-of-homology)
    - [Homotopy invariance of homology](homology.md#homotopy-invariance-of-homology)
      - [Singular prism operator](homology.md#singular-prism-operator)
  - [First homology](homology.md#first-homology)
  - [Singular homology](homology.md#singular-homology)
    - [Singular chain complex](homology.md#singular-chain-complex)
    - [Small singular chains for an open cover](homology.md#small-singular-chains-for-an-open-cover)
    - [Local coefficient system](homology.md#local-coefficient-system)
      - [Orientation local system](homology.md#orientation-local-system)
    - [Betti number](homology.md#betti-number)
      - [Poincaré polynomial](homology.md#poincare-polynomial)
    - [Singular chain](homology.md#singular-chain)
      - [Singular chain group](homology.md#singular-chain-group)
    - [Singular simplex](homology.md#singular-simplex)
  - [Intersection form](homology.md#intersection-form)
    - [Rank-one intersection form and the projective-plane cohomology ring](homology.md#rank-one-intersection-form-and-the-projective-plane-cohomology-ring)
    - [Positive index of the intersection form](homology.md#positive-index-of-the-intersection-form)
    - [Intersection form of a product of two closed oriented surfaces](homology.md#intersection-form-of-a-product-of-two-closed-oriented-surfaces)
    - [Unimodular intersection pairing](homology.md#unimodular-intersection-pairing)
    - [Novikov additivity](homology.md#novikov-additivity)
    - [Intersection pairing](homology.md#intersection-pairing)
      - [Intersection matrix](homology.md#intersection-matrix)
      - [Coordinate sphere intersection basis](homology.md#coordinate-sphere-intersection-basis)
      - [Half-lives-half-dies theorem](homology.md#half-lives-half-dies-theorem)
    - [Degree constraint from intersection forms](homology.md#degree-constraint-from-intersection-forms)
    - [Real de Rham intersection form in dimension four](homology.md#real-de-rham-intersection-form-in-dimension-four)
      - [Signature of the intersection form from harmonic duality](homology.md#signature-of-the-intersection-form-from-harmonic-duality)
  - [Integral homology](homology.md#integral-homology)
  - [Homology of a sphere](homology.md#homology-of-a-sphere)
    - [Homology of an equatorial sphere complement](homology.md#homology-of-an-equatorial-sphere-complement)
  - [Degree of a continuous mapping](homology.md#degree-of-a-continuous-mapping)
    - [Mod-two degree of a map between closed manifolds](homology.md#mod-two-degree-of-a-map-between-closed-manifolds)
    - [Nonzero degree from a sphere obstructs manifold products](homology.md#nonzero-degree-from-a-sphere-obstructs-manifold-products)
    - [Degrees of maps of the zero-sphere](homology.md#degrees-of-maps-of-the-zero-sphere)
    - [Relative mapping degree](homology.md#relative-mapping-degree)
      - [Graph intersection formula for mapping degree](homology.md#graph-intersection-formula-for-mapping-degree)
      - [Quotient-sphere degree identity](homology.md#quotient-sphere-degree-identity)
    - [Local degree of a continuous map](homology.md#local-degree-of-a-continuous-map)
      - [Local degrees of arbitrary integer value](homology.md#local-degrees-of-arbitrary-integer-value)
      - [Degree as a sum of local degrees](homology.md#degree-as-a-sum-of-local-degrees)
    - [Degree under suspension](homology.md#degree-under-suspension)
      - [Sphere maps of arbitrary integer degree](homology.md#sphere-maps-of-arbitrary-integer-degree)
    - [Degree of a map between oriented manifolds](homology.md#degree-of-a-map-between-oriented-manifolds)
      - [Cup-power obstruction to nonzero degree](homology.md#cup-power-obstruction-to-nonzero-degree)
      - [Arbitrary-degree maps to a surface of genus two](homology.md#arbitrary-degree-maps-to-a-surface-of-genus-two)
      - [Collapse map of degree one onto a sphere](homology.md#collapse-map-of-degree-one-onto-a-sphere)
      - [Surjective degree-zero sphere-to-torus map](homology.md#surjective-degree-zero-sphere-to-torus-map)
      - [Multiplicativity of mapping degree](homology.md#multiplicativity-of-mapping-degree)
      - [Homotopy invariance of mapping degree](homology.md#homotopy-invariance-of-mapping-degree)
      - [Degree does not classify general manifold maps](homology.md#degree-does-not-classify-general-manifold-maps)
      - [Degree by integration of a pullback volume form](homology.md#degree-by-integration-of-a-pullback-volume-form)
      - [Spherical degree by area pullback](homology.md#spherical-degree-by-area-pullback)
      - [Degree-one maps between closed oriented surfaces](homology.md#degree-one-maps-between-closed-oriented-surfaces)
      - [Prime-degree sphere map forces primary torsion](homology.md#prime-degree-sphere-map-forces-primary-torsion)
      - [Degrees of maps factoring through real projective space](homology.md#degrees-of-maps-factoring-through-real-projective-space)
    - [Antipodal map](homology.md#antipodal-map)
      - [Fixed-point-free sphere maps are homotopic to the antipodal map](homology.md#fixed-point-free-sphere-maps-are-homotopic-to-the-antipodal-map)
      - [Odd map between spheres](homology.md#odd-map-between-spheres)
        - [Cohomological obstruction to separately odd sphere multiplication](homology.md#cohomological-obstruction-to-separately-odd-sphere-multiplication)
        - [Odd maps pull back the real tautological line bundle](homology.md#odd-maps-pull-back-the-real-tautological-line-bundle)
      - [Invariant primitive under a finite group action](homology.md#invariant-primitive-under-a-finite-group-action)
        - [Top-degree differential forms on even-dimensional real projective space are exact](homology.md#top-degree-differential-forms-on-even-dimensional-real-projective-space-are-exact)
    - [Degree of a Euclidean homeomorphism](homology.md#degree-of-a-euclidean-homeomorphism)
    - [Degree of a factor swap](homology.md#degree-of-a-factor-swap)
  - [Relative homology](homology.md#relative-homology)
    - [Relative homology of a surface modulo disjoint circles](homology.md#relative-homology-of-a-surface-modulo-disjoint-circles)
    - [Relative homology class](homology.md#relative-homology-class)
    - [Relative chain complex](homology.md#relative-chain-complex)
      - [Relative cycle](homology.md#relative-cycle)
      - [Relative simplicial chain complex](homology.md#relative-simplicial-chain-complex)
    - [Long exact sequence in relative homology](homology.md#long-exact-sequence-in-relative-homology)
    - [Relative homology of a simplex and its boundary](homology.md#relative-homology-of-a-simplex-and-its-boundary)
    - [Good pair](homology.md#good-pair)
      - [Collapsing a pair theorem](homology.md#collapsing-a-pair-theorem)
        - [Collapsing a simple closed curve on a surface](homology.md#collapsing-a-simple-closed-curve-on-a-surface)
          - [Homology after collapsing a nonseparating surface curve](homology.md#homology-after-collapsing-a-nonseparating-surface-curve)
          - [Homology after collapsing a separating surface curve](homology.md#homology-after-collapsing-a-separating-surface-curve)
  - [Excision theorem](homology.md#excision-theorem)
  - [Exact sequence](homology.md#exact-sequence)
    - [Long exact sequence](homology.md#long-exact-sequence)
  - [Commutative diagram](homology.md#commutative-diagram)
  - [Chain complex](homology.md#chain-complex)
    - [Hopf trace identity](homology.md#hopf-trace-identity)
    - [Differential of a chain complex](homology.md#differential-of-a-chain-complex)
    - [Reversed dual chain complex](homology.md#reversed-dual-chain-complex)
    - [Graded Hom complex of chain complexes](homology.md#graded-hom-complex-of-chain-complexes)
      - [Sign conjugation for the tensor-Hom identification](homology.md#sign-conjugation-for-the-tensor-hom-identification)
    - [Tensor product of chain complexes](homology.md#tensor-product-of-chain-complexes)
      - [Koszul sign rule](homology.md#koszul-sign-rule)
    - [Disk chain complex](homology.md#disk-chain-complex)
    - [Sphere chain complex](homology.md#sphere-chain-complex)
    - [Double complex](homology.md#double-complex)
      - [Double cochain complex](homology.md#double-cochain-complex)
        - [Two spectral sequences of a bounded double complex](homology.md#two-spectral-sequences-of-a-bounded-double-complex)
        - [Total cochain complex](homology.md#total-cochain-complex)
    - [Koszul complex](homology.md#koszul-complex)
      - [Self-duality of the Koszul complex](homology.md#self-duality-of-the-koszul-complex)
      - [Koszul acyclicity criterion in a Noetherian local ring](homology.md#koszul-acyclicity-criterion-in-a-noetherian-local-ring)
      - [Koszul complex with module coefficients](homology.md#koszul-complex-with-module-coefficients)
      - [Koszul homology](homology.md#koszul-homology)
        - [Koszul homotopy for multiplication by a generator](homology.md#koszul-homotopy-for-multiplication-by-a-generator)
      - [Koszul complex on central ring elements](homology.md#koszul-complex-on-central-ring-elements)
    - [Augmented chain complex](homology.md#augmented-chain-complex)
    - [Chain group](homology.md#chain-group)
    - [Chain subcomplex](homology.md#chain-subcomplex)
    - [Boundary operator](homology.md#boundary-operator)
    - [Cellular chain complex](homology.md#cellular-chain-complex)
      - [Cellular chain group](homology.md#cellular-chain-group)
      - [Cellular chain](homology.md#cellular-chain)
      - [Cellular cycle](homology.md#cellular-cycle)
        - [Cellular boundary](homology.md#cellular-boundary)
      - [Cellular chains of a product of finite CW complexes](homology.md#cellular-chains-of-a-product-of-finite-cw-complexes)
      - [Homology of a torus with two parallel circles collapsed](homology.md#homology-of-a-torus-with-two-parallel-circles-collapsed)
      - [Cellular homology theorem](homology.md#cellular-homology-theorem)
      - [Cellular cochain complex](homology.md#cellular-cochain-complex)
        - [Cellular cohomology](homology.md#cellular-cohomology)
          - [One-cell bound on next-degree cohomology](homology.md#one-cell-bound-on-next-degree-cohomology)
          - [Coprime two-cell attachments to a circle](homology.md#coprime-two-cell-attachments-to-a-circle)
      - [Cellular boundary formula](homology.md#cellular-boundary-formula)
    - [Chain cycle](homology.md#chain-cycle)
    - [Chain boundary](homology.md#chain-boundary)
    - [Chain coefficient](homology.md#chain-coefficient)
    - [Chain map](homology.md#chain-map)
      - [Quasi-isomorphism](homology.md#quasi-isomorphism)
        - [Prime coefficient detection of quasi-isomorphisms](homology.md#prime-coefficient-detection-of-quasi-isomorphisms)
      - [Induced map on homology](homology.md#induced-map-on-homology)
      - [Chain homotopy](homology.md#chain-homotopy)
        - [Contracting homotopy](homology.md#contracting-homotopy)
        - [Cochain homotopy](homology.md#cochain-homotopy)
        - [Small simplex theorem](homology.md#small-simplex-theorem)
    - [Mapping cone (homological algebra)](homology.md#mapping-cone-homological-algebra)
      - [Mapping cone acyclicity criterion](homology.md#mapping-cone-acyclicity-criterion)
    - [Short exact sequence of chain complexes](homology.md#short-exact-sequence-of-chain-complexes)
      - [Long exact sequence in homology](homology.md#long-exact-sequence-in-homology)
        - [Connecting homomorphism](homology.md#connecting-homomorphism)
          - [Relative homology connecting homomorphism](homology.md#relative-homology-connecting-homomorphism)
          - [Bockstein homomorphism](homology.md#bockstein-homomorphism)
            - [Bockstein on infinite real projective space](homology.md#bockstein-on-infinite-real-projective-space)
            - [Bockstein factorization through integral cohomology](homology.md#bockstein-factorization-through-integral-cohomology)
              - [Degree-one Bockstein square identity](homology.md#degree-one-bockstein-square-identity)
              - [Bockstein square-zero identity](homology.md#bockstein-square-zero-identity)
                - [Bockstein cohomology](homology.md#bockstein-cohomology)
            - [Integral Bockstein homomorphism](homology.md#integral-bockstein-homomorphism)
            - [Bockstein isomorphism for a three-dimensional lens space](homology.md#bockstein-isomorphism-for-a-three-dimensional-lens-space)
              - [Bockstein linking invariant of a three-dimensional lens space](homology.md#bockstein-linking-invariant-of-a-three-dimensional-lens-space)
            - [Bockstein homology](homology.md#bockstein-homology)
            - [Long exact sequence from a coefficient sequence](homology.md#long-exact-sequence-from-a-coefficient-sequence)
            - [Bockstein derivation rule](homology.md#bockstein-derivation-rule)
    - [Elementary decomposition of a finite free chain complex](homology.md#elementary-decomposition-of-a-finite-free-chain-complex)
    - [Detection of integral acyclicity modulo primes](homology.md#detection-of-integral-acyclicity-modulo-primes)
  - [Universal coefficient theorem for homology](homology.md#universal-coefficient-theorem-for-homology)
    - [Rational homology](homology.md#rational-homology)
  - [Simplicial homology](homology.md#simplicial-homology)
    - [Simplicial cycle](homology.md#simplicial-cycle)
    - [Simplicial chain complex](homology.md#simplicial-chain-complex)
      - [Simplicial cone chain contraction](homology.md#simplicial-cone-chain-contraction)
    - [Euler characteristic](homology.md#euler-characteristic)
      - [Odd-dimensional closed manifolds have zero Euler characteristic](homology.md#odd-dimensional-closed-manifolds-have-zero-euler-characteristic)
      - [Euler characteristics of closed oriented four-manifolds](homology.md#euler-characteristics-of-closed-oriented-four-manifolds)
      - [Ordinary vertex in a nonconcurrent great-circle arrangement](homology.md#ordinary-vertex-in-a-nonconcurrent-great-circle-arrangement)
      - [Euler formula for a sphere](homology.md#euler-formula-for-a-sphere)
      - [Euler characteristic of a product](homology.md#euler-characteristic-of-a-product)
      - [Euler characteristic under a finite covering](homology.md#euler-characteristic-under-a-finite-covering)
      - [Euler characteristic of an odd-dimensional closed manifold](homology.md#euler-characteristic-of-an-odd-dimensional-closed-manifold)
      - [Euler-Poincare formula](homology.md#euler-poincare-formula)
    - [Barycentric subdivision](homology.md#barycentric-subdivision)
      - [Iterated barycentric subdivision](homology.md#iterated-barycentric-subdivision)
      - [Mesh of a simplicial complex](homology.md#mesh-of-a-simplicial-complex)
      - [Barycentric subdivision of a tetrahedron](homology.md#barycentric-subdivision-of-a-tetrahedron)
  - [Local homology](homology.md#local-homology)
    - [Local homology from a link](homology.md#local-homology-from-a-link)
    - [Fixed barycentre of the barycentric tetrahedral two-skeleton](homology.md#fixed-barycentre-of-the-barycentric-tetrahedral-two-skeleton)
  - [Intersection form of a 4-manifold](homology.md#intersection-form-of-a-4-manifold)
  - [Universal coefficient theorem](homology.md#universal-coefficient-theorem)
- [Homotopy](#homotopy)
  - [Homotopy category](#homotopy-category)
    - [Homotopy pushout](#homotopy-pushout)
    - [H-space](#h-space)
      - [H-group](#h-group)
    - [Topological half-exact functor](#topological-half-exact-functor)
      - [Brown's representability theorem](#brown-s-representability-theorem)
  - [Homotopy inverse limit of a tower](#homotopy-inverse-limit-of-a-tower)
  - [Maps to a sphere above the dimension of a compact smooth manifold are null-homotopic](#maps-to-a-sphere-above-the-dimension-of-a-compact-smooth-manifold-are-null-homotopic)
  - [Rational homotopy theory](#rational-homotopy-theory)
    - [Nilpotent space](#nilpotent-space)
    - [Rational space](#rational-space)
      - [Rationalization of a topological space](#rationalization-of-a-topological-space)
        - [Rational homotopy equivalence](#rational-homotopy-equivalence)
          - [Rational homotopy type](#rational-homotopy-type)
    - [Sullivan minimal model](#sullivan-minimal-model)
      - [Relative Sullivan algebra](#relative-sullivan-algebra)
      - [Sullivan fibre-model theorem](#sullivan-fibre-model-theorem)
      - [Sullivan minimal-model classification](#sullivan-minimal-model-classification)
      - [Rational polynomial differential forms](#rational-polynomial-differential-forms)
      - [Minimal model of the fibre of the projective-space collapse map](#minimal-model-of-the-fibre-of-the-projective-space-collapse-map)
      - [Rational model of a collapsed complex projective subspace](#rational-model-of-a-collapsed-complex-projective-subspace)
      - [Minimal model of a wedge of simply connected spheres](#minimal-model-of-a-wedge-of-simply-connected-spheres)
      - [Formal space](#formal-space)
      - [Sullivan model of the connected sum of two complex projective planes](#sullivan-model-of-the-connected-sum-of-two-complex-projective-planes)
  - [Reduced suspension](#reduced-suspension)
    - [Suspension-loop adjunction](#suspension-loop-adjunction)
  - [Homotopy class](#homotopy-class)
  - [Free homotopy](#free-homotopy)
  - [Null-homotopic map](#null-homotopic-map)
    - [Extension-null-homotopy criterion for a sphere](#extension-null-homotopy-criterion-for-a-sphere)
  - [Contractible space](#contractible-space)
    - [Contraction of a topological space](#contraction-of-a-topological-space)
  - [Homotopy equivalence](#homotopy-equivalence)
    - [Homology obstruction to carrying surface curves onto one another](#homology-obstruction-to-carrying-surface-curves-onto-one-another)
    - [Separate homotopy inverses combine into a homotopy equivalence](#separate-homotopy-inverses-combine-into-a-homotopy-equivalence)
    - [Homotopy type](#homotopy-type)
    - [Homotopy inverse](#homotopy-inverse)
  - [Retract](#retract)
    - [Deformation retraction](#deformation-retraction)
    - [Retract of a contractible space](#retract-of-a-contractible-space)
  - [Homotopy extension property](#homotopy-extension-property)
    - [Cofibration](#cofibration)
    - [Collapsing a contractible cofibration](#collapsing-a-contractible-cofibration)
  - [Homotopy group](#homotopy-group)
    - [Whitehead product](#whitehead-product)
      - [Whitehead square](#whitehead-square)
    - [Postnikov tower](#postnikov-tower)
      - [Principal Eilenberg–MacLane fibration](#principal-eilenberg-maclane-fibration)
        - [Postnikov invariant](#postnikov-invariant)
    - [First homotopy group above the dimension of a sphere](#first-homotopy-group-above-the-dimension-of-a-sphere)
    - [Serre finiteness theorem for homotopy groups](#serre-finiteness-theorem-for-homotopy-groups)
    - [Relative homotopy group](#relative-homotopy-group)
      - [Homotopy excision theorem](#homotopy-excision-theorem)
      - [Long exact sequence of relative homotopy groups](#long-exact-sequence-of-relative-homotopy-groups)
    - [Eilenberg–MacLane space](#eilenberg-maclane-space)
      - [Low-degree integral homology of a mod-two Eilenberg–MacLane space](#low-degree-integral-homology-of-a-mod-two-eilenberg-maclane-space)
      - [Serre polynomial generators for mod-two Eilenberg–MacLane cohomology](#serre-polynomial-generators-for-mod-two-eilenberg-maclane-cohomology)
        - [Low-degree mod-two cohomology of an Eilenberg–MacLane space](#low-degree-mod-two-cohomology-of-an-eilenberg-maclane-space)
      - [Rational cohomology of an integral Eilenberg–MacLane space](#rational-cohomology-of-an-integral-eilenberg-maclane-space)
      - [Representability of cohomology by Eilenberg–MacLane spaces](#representability-of-cohomology-by-eilenberg-maclane-spaces)
      - [Universal cohomology class of an Eilenberg–MacLane space](#universal-cohomology-class-of-an-eilenberg-maclane-space)
      - [Aspherical space](#aspherical-space)
    - [Homotopy groups as modules over the fundamental group](#homotopy-groups-as-modules-over-the-fundamental-group)
    - [Freudenthal suspension theorem](#freudenthal-suspension-theorem)
      - [Freudenthal suspension from two cones](#freudenthal-suspension-from-two-cones)
      - [Homology comparison proof of Freudenthal suspension](#homology-comparison-proof-of-freudenthal-suspension)
    - [Hopf invariant](#hopf-invariant)
      - [Cohomology ring of a Hopf attachment with a sphere summand](#cohomology-ring-of-a-hopf-attachment-with-a-sphere-summand)
        - [Third homotopy group of a Hopf attachment with a sphere summand](#third-homotopy-group-of-a-hopf-attachment-with-a-sphere-summand)
      - [Precomposition scales the Hopf invariant by degree](#precomposition-scales-the-hopf-invariant-by-degree)
    - [Weak homotopy equivalence](#weak-homotopy-equivalence)
    - [n-connected map](#n-connected-map)
    - [Loop-space shift of homotopy groups](#loop-space-shift-of-homotopy-groups)
    - [Rational homotopy group](#rational-homotopy-group)
      - [Rational homotopy groups of the connected sum of two complex projective planes](#rational-homotopy-groups-of-the-connected-sum-of-two-complex-projective-planes)
      - [Rational homotopy groups of a sphere](#rational-homotopy-groups-of-a-sphere)
    - [Hurewicz theorem](#hurewicz-theorem)
      - [Hurewicz homomorphism](#hurewicz-homomorphism)
        - [Surjective rational Hurewicz homomorphism gives a wedge of spheres](#surjective-rational-hurewicz-homomorphism-gives-a-wedge-of-spheres)
      - [Relative Hurewicz theorem](#relative-hurewicz-theorem)
      - [Hurewicz theorem modulo a Serre class](#hurewicz-theorem-modulo-a-serre-class)
    - [Whitehead theorem](#whitehead-theorem)
      - [Rational Whitehead theorem](#rational-whitehead-theorem)
      - [Homological Whitehead theorem](#homological-whitehead-theorem)
  - [Homotopy fiber](#homotopy-fiber)
    - [Principal fibration](#principal-fibration)
    - [Path-space fibration](#path-space-fibration)
  - [Fibration](#fibration)
  - [Homotopy fiber sequence](#homotopy-fiber-sequence)
  - [Homotopy pullback](#homotopy-pullback)
  - [Loop space](#loop-space)
    - [Samelson product](#samelson-product)
    - [Based path space and the path-loop fibration](#based-path-space-and-the-path-loop-fibration)
    - [Integral homology of the loop space of a sphere](#integral-homology-of-the-loop-space-of-a-sphere)
    - [Integral cohomology of an odd-sphere loop space](#integral-cohomology-of-an-odd-sphere-loop-space)
    - [Pontryagin ring](#pontryagin-ring)
      - [Milnor–Moore theorem](#milnor-moore-theorem)
      - [Pontryagin ring of an odd-sphere loop space](#pontryagin-ring-of-an-odd-sphere-loop-space)
      - [Pontryagin product on loop-space homology](#pontryagin-product-on-loop-space-homology)
    - [James reduced product](#james-reduced-product)
      - [Bott–Samelson theorem](#bott-samelson-theorem)
    - [Loop-space homology](#loop-space-homology)
    - [Path-loop fibration](#path-loop-fibration)
      - [Cohomology suspension](#cohomology-suspension)
  - [Simplicial homotopy theory](#simplicial-homotopy-theory)
    - [Simplex category](#simplex-category)
    - [Simplicial set](#simplicial-set)
      - [Geometric realization of a simplicial set](#geometric-realization-of-a-simplicial-set)
      - [Singular simplicial set](#singular-simplicial-set)
      - [Standard simplex](#standard-simplex)
        - [Simplicial horn](#simplicial-horn)
          - [Inner horn](#inner-horn)
      - [Quasicategory](#quasicategory)
      - [Kan complex](#kan-complex)
      - [Nerve (category theory)](#nerve-category-theory)
      - [Simplicial mapping space](#simplicial-mapping-space)
    - [Simplicial abelian group](#simplicial-abelian-group)
      - [Normalized chain complex of a simplicial abelian group](#normalized-chain-complex-of-a-simplicial-abelian-group)
        - [Dold–Kan correspondence](#dold-kan-correspondence)
  - [Serre spectral sequence](#serre-spectral-sequence)
    - [Cohomological Serre spectral sequence](#cohomological-serre-spectral-sequence)
      - [A sphere cannot fibre over a lower-dimensional odd sphere](#a-sphere-cannot-fibre-over-a-lower-dimensional-odd-sphere)
    - [Serre fibration](#serre-fibration)
      - [Relative homotopy of a Serre fibration](#relative-homotopy-of-a-serre-fibration)
      - [Relative homology of a fibration over a sphere](#relative-homology-of-a-fibration-over-a-sphere)
      - [Splitting of a simply connected Eilenberg–MacLane fibration](#splitting-of-a-simply-connected-eilenberg-maclane-fibration)
      - [Mapping-path fibration replacement](#mapping-path-fibration-replacement)
      - [Homotopy lifting property](#homotopy-lifting-property)
      - [Long exact sequence of homotopy groups of a fibration](#long-exact-sequence-of-homotopy-groups-of-a-fibration)
    - [Wang homomorphism](#wang-homomorphism)
      - [Wang sequence over a sphere](#wang-sequence-over-a-sphere)
    - [Transgression](#transgression)
      - [Transgressive pair](#transgressive-pair)
        - [Kudo transgression theorem](#kudo-transgression-theorem)
- [Loop (topology)](#loop-topology)
  - [Based loop](#based-loop)
    - [Based homotopy](#based-homotopy)
    - [Path reversal](#path-reversal)
- [Fundamental group](#fundamental-group)
  - [Fundamental group of a surface](#fundamental-group-of-a-surface)
    - [Dehn-Nielsen-Baer theorem for closed orientable surfaces](#dehn-nielsen-baer-theorem-for-closed-orientable-surfaces)
  - [Closed-manifold realization of a finitely presented fundamental group](#closed-manifold-realization-of-a-finitely-presented-fundamental-group)
  - [Simply connected space](#simply-connected-space)
  - [Fundamental group of a bouquet of circles](#fundamental-group-of-a-bouquet-of-circles)
  - [Change of basepoint isomorphism](#change-of-basepoint-isomorphism)
  - [Well-defined loop concatenation](#well-defined-loop-concatenation)
  - [Functoriality of the fundamental group](#functoriality-of-the-fundamental-group)
  - [Seifert-van Kampen theorem](#seifert-van-kampen-theorem)
    - [Fundamental group of a wedge of circles and a real projective plane](#fundamental-group-of-a-wedge-of-circles-and-a-real-projective-plane)
    - [Amalgamated free product](#amalgamated-free-product)
      - [Free product](#free-product)
        - [Effective cyclic membership in a free product](#effective-cyclic-membership-in-a-free-product)
        - [Free factor](#free-factor)
        - [Universal property of a free product](#universal-property-of-a-free-product)
        - [Nontrivial free product](#nontrivial-free-product)
        - [Free product with factor generating set](#free-product-with-factor-generating-set)
        - [Normal form for free groups and free product of groups](#normal-form-for-free-groups-and-free-product-of-groups)
          - [Normal form theorem for a free product](#normal-form-theorem-for-a-free-product)
            - [Syllable in a free product](#syllable-in-a-free-product)
    - [Generation of a fundamental group by two open sets](#generation-of-a-fundamental-group-by-two-open-sets)
    - [Fundamental group after attaching a Möbius band](#fundamental-group-after-attaching-a-mobius-band)
      - [Homology after attaching a Möbius band to the real projective plane](#homology-after-attaching-a-mobius-band-to-the-real-projective-plane)
      - [Two Möbius bands attached to a torus](#two-mobius-bands-attached-to-a-torus)
    - [Fundamental group after attaching a 2-cell](#fundamental-group-after-attaching-a-2-cell)
      - [Presentation complex](#presentation-complex)
        - [Presentation complex for the symmetric group on three letters](#presentation-complex-for-the-symmetric-group-on-three-letters)
  - [Fundamental group of a closed orientable surface](#fundamental-group-of-a-closed-orientable-surface)
- [Covering space](#covering-space)
  - [Semilocally simply connected space](#semilocally-simply-connected-space)
  - [Riemannian covering](#riemannian-covering)
  - [Homological transfer for a finite covering](#homological-transfer-for-a-finite-covering)
  - [Double covers of the figure-eight space](#double-covers-of-the-figure-eight-space)
  - [Orientation double cover](#orientation-double-cover)
    - [Connectedness criterion for the orientation double cover](#connectedness-criterion-for-the-orientation-double-cover)
    - [Canonical orientation of the orientation double cover](#canonical-orientation-of-the-orientation-double-cover)
  - [Homotopy lifting theorem for a covering map](#homotopy-lifting-theorem-for-a-covering-map)
  - [Branched covering](#branched-covering)
    - [Branched surface action from two generators](#branched-surface-action-from-two-generators)
  - [Infinite cyclic cover associated to an epimorphism](#infinite-cyclic-cover-associated-to-an-epimorphism)
    - [Alexander module of a space](#alexander-module-of-a-space)
  - [Universal abelian cover](#universal-abelian-cover)
  - [Kernel cover of a real projective plane wedged with a circle](#kernel-cover-of-a-real-projective-plane-wedged-with-a-circle)
  - [Four-sheeted cover of a wedge of circles and a real projective plane](#four-sheeted-cover-of-a-wedge-of-circles-and-a-real-projective-plane)
  - [Uniqueness of lifts to a covering space](#uniqueness-of-lifts-to-a-covering-space)
  - [Monodromy action of a covering space](#monodromy-action-of-a-covering-space)
    - [Monodromy of hyperplane sections of a smooth curve](#monodromy-of-hyperplane-sections-of-a-smooth-curve)
    - [Monodromy permutation](#monodromy-permutation)
  - [Deck transformation](#deck-transformation)
    - [Deck transformation group](#deck-transformation-group)
      - [Finite groups act freely on suitable closed orientable surfaces](#finite-groups-act-freely-on-suitable-closed-orientable-surfaces)
      - [Free isometric realization of a finitely generated group](#free-isometric-realization-of-a-finitely-generated-group)
      - [Deck transformation group as a monodromy centralizer](#deck-transformation-group-as-a-monodromy-centralizer)
    - [Deck involution of a double covering](#deck-involution-of-a-double-covering)
    - [Transfer chain map of a double covering](#transfer-chain-map-of-a-double-covering)
  - [Universal cover](#universal-cover)
    - [Universal cover of a closed three-manifold with finite fundamental group](#universal-cover-of-a-closed-three-manifold-with-finite-fundamental-group)
    - [Component of a pulled-back universal cover](#component-of-a-pulled-back-universal-cover)
    - [Uniqueness of a universal covering space](#uniqueness-of-a-universal-covering-space)
    - [Extension criterion into a space with contractible universal cover](#extension-criterion-into-a-space-with-contractible-universal-cover)
  - [Classification of connected covering spaces](#classification-of-connected-covering-spaces)
    - [Path-class construction of a subgroup covering](#path-class-construction-of-a-subgroup-covering)
    - [Regular covering](#regular-covering)
    - [Degree of a connected covering](#degree-of-a-connected-covering)
      - [Fibre bijection by path lifting](#fibre-bijection-by-path-lifting)
    - [Cell complex of a covering from a coset graph](#cell-complex-of-a-covering-from-a-coset-graph)
    - [Permutation covering of a wedge of circles](#permutation-covering-of-a-wedge-of-circles)
    - [Covering-space subgroup and deck-group quotient](#covering-space-subgroup-and-deck-group-quotient)
    - [Normal covering map](#normal-covering-map)
      - [Universal covering map is normal](#universal-covering-map-is-normal)
      - [Forced normality of finite connected covers of orientable surfaces](#forced-normality-of-finite-connected-covers-of-orientable-surfaces)
        - [Nonnormal finite cover of a higher-genus orientable surface](#nonnormal-finite-cover-of-a-higher-genus-orientable-surface)
  - [Path lifting theorem](#path-lifting-theorem)
  - [Lifting criterion for a covering space](#lifting-criterion-for-a-covering-space)
  - [Covering space action](#covering-space-action)
    - [Quotient of a topological group by a discrete subgroup](#quotient-of-a-topological-group-by-a-discrete-subgroup)
    - [Non-Hausdorff orbit space of a covering action](#non-hausdorff-orbit-space-of-a-covering-action)
      - [Simply connected non-Hausdorff orbit-space example](#simply-connected-non-hausdorff-orbit-space-example)
- [Topological group](topological-group.md)
  - [Locally profinite group](topological-group.md#locally-profinite-group)
    - [Compact-open subgroup](topological-group.md#compact-open-subgroup)
  - [Continuous unitary character](topological-group.md#continuous-unitary-character)
  - [Right-invariant group metric](topological-group.md#right-invariant-group-metric)
  - [Left-invariant group metric](topological-group.md#left-invariant-group-metric)
    - [Bi-invariant group metric](topological-group.md#bi-invariant-group-metric)
      - [Affine conjugation obstruction to a bi-invariant group metric](topological-group.md#affine-conjugation-obstruction-to-a-bi-invariant-group-metric)
    - [Birkhoff-Kakutani theorem](topological-group.md#birkhoff-kakutani-theorem)
      - [Dyadic product estimate for group neighbourhoods](topological-group.md#dyadic-product-estimate-for-group-neighbourhoods)
  - [Closed subgroup](topological-group.md#closed-subgroup)
  - [Open subgroup](topological-group.md#open-subgroup)
    - [Open normal subgroup](topological-group.md#open-normal-subgroup)
  - [Compactly generated group](topological-group.md#compactly-generated-group)
    - [Compact generation does not imply local compactness](topological-group.md#compact-generation-does-not-imply-local-compactness)
  - [Locally compact group](topological-group.md#locally-compact-group)
    - [Sigma-compact open subgroup of a locally compact group](topological-group.md#sigma-compact-open-subgroup-of-a-locally-compact-group)
  - [Neighbourhood criterion for a topological group](topological-group.md#neighbourhood-criterion-for-a-topological-group)
  - [Discrete subgroup](topological-group.md#discrete-subgroup)
    - [Discrete additive subgroup of a real vector space](topological-group.md#discrete-additive-subgroup-of-a-real-vector-space)
    - [Planar discrete-subgroup basis](topological-group.md#planar-discrete-subgroup-basis)
    - [Kleinian group](topological-group.md#kleinian-group)
      - [Gaussian Bianchi group](topological-group.md#gaussian-bianchi-group)
      - [Jørgensen's inequality](topological-group.md#jorgensen-s-inequality)
      - [Schottky group](topological-group.md#schottky-group)
        - [Tangent-disk Schottky group](topological-group.md#tangent-disk-schottky-group)
      - [Rank-one convergence of divergent Möbius transformations](topological-group.md#rank-one-convergence-of-divergent-mobius-transformations)
      - [Elliptic stabilizer obstruction to a hyperbolic manifold quotient](topological-group.md#elliptic-stabilizer-obstruction-to-a-hyperbolic-manifold-quotient)
      - [Non-elementary Kleinian group](topological-group.md#non-elementary-kleinian-group)
      - [Limit set of a Kleinian group](topological-group.md#limit-set-of-a-kleinian-group)
        - [Minimality of the Kleinian limit set](topological-group.md#minimality-of-the-kleinian-limit-set)
          - [Limit set of an infinite normal Kleinian subgroup](topological-group.md#limit-set-of-an-infinite-normal-kleinian-subgroup)
      - [Gaussian-integer parabolic construction](topological-group.md#gaussian-integer-parabolic-construction)
      - [A free Kleinian group generated by two parabolic transformations](topological-group.md#a-free-kleinian-group-generated-by-two-parabolic-transformations)
  - [Compact group](topological-group.md#compact-group)
    - [Compact groups with a descending chain condition are Lie groups](topological-group.md#compact-groups-with-a-descending-chain-condition-are-lie-groups)
    - [Closed subsemigroup of a compact group](topological-group.md#closed-subsemigroup-of-a-compact-group)
  - [Profinite group](topological-group.md#profinite-group)
    - [Just-infinite profinite group](topological-group.md#just-infinite-profinite-group)
      - [Hereditarily just-infinite profinite group](topological-group.md#hereditarily-just-infinite-profinite-group)
    - [Rank of a profinite group](topological-group.md#rank-of-a-profinite-group)
    - [Procyclic group](topological-group.md#procyclic-group)
    - [Open normal subgroup basis of a profinite group](topological-group.md#open-normal-subgroup-basis-of-a-profinite-group)
    - [Profinite Frattini subgroup](topological-group.md#profinite-frattini-subgroup)
    - [Profinite abelian group](topological-group.md#profinite-abelian-group)
    - [Pro-p group](topological-group.md#pro-p-group)
      - [Pro-p subgroup](topological-group.md#pro-p-subgroup)
      - [R-analytic pro-p group](topological-group.md#r-analytic-pro-p-group)
      - [Nottingham group](topological-group.md#nottingham-group)
        - [Finite p-group embedding in the Nottingham group](topological-group.md#finite-p-group-embedding-in-the-nottingham-group)
        - [Depth filtration of the Nottingham group](topological-group.md#depth-filtration-of-the-nottingham-group)
          - [Derived-series growth of the Nottingham group](topological-group.md#derived-series-growth-of-the-nottingham-group)
      - [Golod-Shafarevich infinitude criterion for pro-p groups](topological-group.md#golod-shafarevich-infinitude-criterion-for-pro-p-groups)
      - [Powerful pro-p group](topological-group.md#powerful-pro-p-group)
      - [Pro-p completion](topological-group.md#pro-p-completion)
      - [Free pro-p group](topological-group.md#free-pro-p-group)
        - [Magnus degree of a free pro-p group element](topological-group.md#magnus-degree-of-a-free-pro-p-group-element)
        - [Finite pro-p presentation](topological-group.md#finite-pro-p-presentation)
          - [Finite extensions preserve finite pro-p presentations](topological-group.md#finite-extensions-preserve-finite-pro-p-presentations)
      - [Generator number and first cohomology of a finitely generated pro-p group](topological-group.md#generator-number-and-first-cohomology-of-a-finitely-generated-pro-p-group)
        - [Infinite-rank failure of the first-cohomology generator formula](topological-group.md#infinite-rank-failure-of-the-first-cohomology-generator-formula)
      - [Uniform pro-p group](topological-group.md#uniform-pro-p-group)
        - [Odd-prime principal p-adic congruence subgroup is uniform](topological-group.md#odd-prime-principal-p-adic-congruence-subgroup-is-uniform)
        - [Root correction criterion for uniformity](topological-group.md#root-correction-criterion-for-uniformity)
        - [Linearity of a uniform pro-p group](topological-group.md#linearity-of-a-uniform-pro-p-group)
        - [Power congruences in a uniform pro-p group](topological-group.md#power-congruences-in-a-uniform-pro-p-group)
        - [Transported addition on a uniform pro-p group](topological-group.md#transported-addition-on-a-uniform-pro-p-group)
        - [Uniform pro-p group and powerful Lie lattice correspondence](topological-group.md#uniform-pro-p-group-and-powerful-lie-lattice-correspondence)
        - [Uniform group and powerful Lie lattice correspondence](topological-group.md#uniform-group-and-powerful-lie-lattice-correspondence)
      - [Strong completeness of finitely generated pro-p groups](topological-group.md#strong-completeness-of-finitely-generated-pro-p-groups)
      - [Profinite Sylow subgroup](topological-group.md#profinite-sylow-subgroup)
    - [Profinite topology](topological-group.md#profinite-topology)
      - [Profinite topology on the integers is not compact](topological-group.md#profinite-topology-on-the-integers-is-not-compact)
      - [Inverse-limit topology](topological-group.md#inverse-limit-topology)
    - [Profinite completion](topological-group.md#profinite-completion)
      - [Universal property of profinite completion](topological-group.md#universal-property-of-profinite-completion)
    - [Topological generating set](topological-group.md#topological-generating-set)
      - [Topological generator](topological-group.md#topological-generator)
      - [Topologically finitely generated group](topological-group.md#topologically-finitely-generated-group)
      - [Finite-quotient criterion for topological generation](topological-group.md#finite-quotient-criterion-for-topological-generation)
    - [Finite-quotient criterion for conjugacy in a profinite group](topological-group.md#finite-quotient-criterion-for-conjugacy-in-a-profinite-group)
    - [Topological Hopf property](topological-group.md#topological-hopf-property)
      - [Hopf property of a topologically finitely generated profinite group](topological-group.md#hopf-property-of-a-topologically-finitely-generated-profinite-group)
    - [Finite-quotient criterion for roots in a profinite group](topological-group.md#finite-quotient-criterion-for-roots-in-a-profinite-group)
  - [Fundamental group of a topological group](topological-group.md#fundamental-group-of-a-topological-group)
    - [Eckmann-Hilton argument](topological-group.md#eckmann-hilton-argument)
      - [Homotopy-group addition in a topological group](topological-group.md#homotopy-group-addition-in-a-topological-group)
  - [Unitary group](topological-group.md#unitary-group)
    - [Unitary sphere quotient and stability range](topological-group.md#unitary-sphere-quotient-and-stability-range)
    - [Unitary group as a regular level set](topological-group.md#unitary-group-as-a-regular-level-set)
    - [Restricted unitary group](topological-group.md#restricted-unitary-group)
    - [Projective unitary group](topological-group.md#projective-unitary-group)
      - [Circle projective representations lift to unitary representations](topological-group.md#circle-projective-representations-lift-to-unitary-representations)
    - [Compact symplectic group](topological-group.md#compact-symplectic-group)
      - [Logarithm charts for the compact symplectic group](topological-group.md#logarithm-charts-for-the-compact-symplectic-group)
    - [Special unitary group](topological-group.md#special-unitary-group)
      - [Logarithm charts for the special unitary group](topological-group.md#logarithm-charts-for-the-special-unitary-group)
      - [SU(4) group](topological-group.md#su-4-group)
      - [Unit sphere orbit of the defining special unitary action](topological-group.md#unit-sphere-orbit-of-the-defining-special-unitary-action)
      - [SU(3) group](topological-group.md#su-3-group)
        - [Triality (SU(3))](topological-group.md#triality-su-3)
        - [Mixed SU(3) tensor representation](topological-group.md#mixed-su-3-tensor-representation)
          - [Explicit cubic SU3 tensor projections](topological-group.md#explicit-cubic-su3-tensor-projections)
          - [Symmetric traceless SU(3) tensor representation](topological-group.md#symmetric-traceless-su-3-tensor-representation)
            - [Symmetric cubic representation of SU(3)](topological-group.md#symmetric-cubic-representation-of-su-3)
            - [Maximal dimension in mixed SU(3) tensor powers](topological-group.md#maximal-dimension-in-mixed-su-3-tensor-powers)
      - [SU(2) group](topological-group.md#su-2-group)
        - [SU(2) matrix](topological-group.md#su-2-matrix)
      - [SU(2) as the three-sphere](topological-group.md#su-2-as-the-three-sphere)
    - [Determinant detects the order of a unitary loop](topological-group.md#determinant-detects-the-order-of-a-unitary-loop)
- [Lefschetz number](#lefschetz-number)
  - [Lefschetz coincidence number](#lefschetz-coincidence-number)
    - [Self-coincidence number of a map of nonzero degree](#self-coincidence-number-of-a-map-of-nonzero-degree)
    - [Lefschetz coincidence theorem](#lefschetz-coincidence-theorem)
- [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem)
  - [Oriented manifold retract for the Lefschetz theorem](#oriented-manifold-retract-for-the-lefschetz-theorem)
  - [Fixed-point-free perturbation of a doubled-surface reflection](#fixed-point-free-perturbation-of-a-doubled-surface-reflection)
  - [Lefschetz fixed-point property of even-dimensional real projective space](#lefschetz-fixed-point-property-of-even-dimensional-real-projective-space)
  - [Fixed-point-free self-maps homotopic to the identity on products of surfaces](#fixed-point-free-self-maps-homotopic-to-the-identity-on-products-of-surfaces)
  - [Cohomology class of the diagonal](#cohomology-class-of-the-diagonal)
    - [Mod-two diagonal class of the real projective plane](#mod-two-diagonal-class-of-the-real-projective-plane)
    - [Graph-diagonal formula for the Lefschetz number](#graph-diagonal-formula-for-the-lefschetz-number)
  - [Lefschetz number of a doubled map](#lefschetz-number-of-a-doubled-map)
  - [Euler-characteristic divisibility from a fixed-point-free cyclic action](#euler-characteristic-divisibility-from-a-fixed-point-free-cyclic-action)
  - [Cyclic point-gluing of two-spheres](#cyclic-point-gluing-of-two-spheres)
  - [Lefschetz-Hopf fixed-point theorem](#lefschetz-hopf-fixed-point-theorem)
    - [Fixed-point congruence for an involution on an odd-sphere connected sum](#fixed-point-congruence-for-an-involution-on-an-odd-sphere-connected-sum)
- [Mayer–Vietoris sequence](#mayer-vietoris-sequence)
  - [Homology after identifying two points on a sphere](#homology-after-identifying-two-points-on-a-sphere)
  - [Homology of two disks meeting inside a sphere](#homology-of-two-disks-meeting-inside-a-sphere)
  - [Acyclic intersection cover homology bound](#acyclic-intersection-cover-homology-bound)
- [Simplicial complex](#simplicial-complex)
  - [Simplicial subdivision](#simplicial-subdivision)
  - [Regular antipodal triangulation of a sphere](#regular-antipodal-triangulation-of-a-sphere)
    - [Standard simplicial decomposition of a sphere](#standard-simplicial-decomposition-of-a-sphere)
  - [Triangulation](#triangulation)
  - [Vertex of a simplicial complex](#vertex-of-a-simplicial-complex)
  - [Simplicial subcomplex](#simplicial-subcomplex)
  - [Geometric realization of a simplicial complex](#geometric-realization-of-a-simplicial-complex)
    - [Open star in a simplicial complex](#open-star-in-a-simplicial-complex)
  - [Simplicial map](#simplicial-map)
    - [Positive alternating simplex](#positive-alternating-simplex)
      - [Antipodal alternating-simplex parity lemma](#antipodal-alternating-simplex-parity-lemma)
    - [Simplicial approximation](#simplicial-approximation)
      - [Straight-line homotopy from a simplicial approximation](#straight-line-homotopy-from-a-simplicial-approximation)
      - [Simplicial approximation theorem](#simplicial-approximation-theorem)
        - [Lower-dimensional sphere maps are null-homotopic](#lower-dimensional-sphere-maps-are-null-homotopic)
    - [Contiguous simplicial maps](#contiguous-simplicial-maps)
  - [Clique complex](#clique-complex)
  - [Simplex](#simplex)
    - [Probability simplex](#probability-simplex)
      - [Closest point of a probability simplex to the origin](#closest-point-of-a-probability-simplex-to-the-origin)
    - [Face of a simplex](#face-of-a-simplex)
    - [Boundary subcomplex of a simplex](#boundary-subcomplex-of-a-simplex)
    - [Regular simplex](#regular-simplex)
  - [Orientation of a simplex](#orientation-of-a-simplex)
  - [Simplicial pseudomanifold](#simplicial-pseudomanifold)
    - [Fundamental class of an orientable simplicial pseudomanifold](#fundamental-class-of-an-orientable-simplicial-pseudomanifold)
- [Cone (topology)](#cone-topology)
- [Simplicial cone](#simplicial-cone)
- [Suspension (topology)](#suspension-topology)
  - [Manifold criterion for a suspension](#manifold-criterion-for-a-suspension)
  - [Suspension isomorphism](#suspension-isomorphism)
  - [Reduced homology of a suspension](#reduced-homology-of-a-suspension)
  - [Union of cones along a common base](#union-of-cones-along-a-common-base)
- [Cohomology](cohomology.md)
  - [Gysin homomorphism](cohomology.md#gysin-homomorphism)
  - [Generalized cohomology theory](cohomology.md#generalized-cohomology-theory)
    - [Represented cohomology theory](cohomology.md#represented-cohomology-theory)
    - [Multiplicative generalized cohomology theory](cohomology.md#multiplicative-generalized-cohomology-theory)
    - [Atiyah-Hirzebruch spectral sequence](cohomology.md#atiyah-hirzebruch-spectral-sequence)
      - [Homological Atiyah-Hirzebruch spectral sequence](cohomology.md#homological-atiyah-hirzebruch-spectral-sequence)
  - [Cohomology groups do not determine homotopy type](cohomology.md#cohomology-groups-do-not-determine-homotopy-type)
  - [Singular cohomology](cohomology.md#singular-cohomology)
    - [Singular cochain](cohomology.md#singular-cochain)
      - [Cochain pullback](cohomology.md#cochain-pullback)
  - [Cohomology operation](cohomology.md#cohomology-operation)
    - [Stable cohomology operation](cohomology.md#stable-cohomology-operation)
      - [Comparison of stable maps and cohomology operations](cohomology.md#comparison-of-stable-maps-and-cohomology-operations)
      - [Integral generator signs constrain Steenrod comparisons](cohomology.md#integral-generator-signs-constrain-steenrod-comparisons)
      - [Steenrod algebra](cohomology.md#steenrod-algebra)
        - [Admissible sequence of Steenrod squares](cohomology.md#admissible-sequence-of-steenrod-squares)
          - [Excess of an admissible Steenrod sequence](cohomology.md#excess-of-an-admissible-steenrod-sequence)
        - [Adem relations](cohomology.md#adem-relations)
        - [Steenrod square](cohomology.md#steenrod-square)
        - [Cartan formula (algebraic topology)](cohomology.md#cartan-formula-algebraic-topology)
        - [Steenrod reduced power](cohomology.md#steenrod-reduced-power)
          - [Steenrod powers on quaternionic projective space](cohomology.md#steenrod-powers-on-quaternionic-projective-space)
  - [Reduced cohomology](cohomology.md#reduced-cohomology)
  - [Equivariant cohomology](cohomology.md#equivariant-cohomology)
    - [Borel construction](cohomology.md#borel-construction)
  - [Cohomology group](cohomology.md#cohomology-group)
    - [Cohomology class](cohomology.md#cohomology-class)
  - [Integral cohomology](cohomology.md#integral-cohomology)
  - [Relative cohomology](cohomology.md#relative-cohomology)
    - [Long exact cohomology sequence of a pair](cohomology.md#long-exact-cohomology-sequence-of-a-pair)
  - [Induced map on cohomology](cohomology.md#induced-map-on-cohomology)
    - [Homotopy invariance of cohomology](cohomology.md#homotopy-invariance-of-cohomology)
    - [Realization of top-dimensional cohomology by a sphere map](cohomology.md#realization-of-top-dimensional-cohomology-by-a-sphere-map)
  - [Universal coefficient theorem for cohomology](cohomology.md#universal-coefficient-theorem-for-cohomology)
    - [First cohomology of the countably punctured plane](cohomology.md#first-cohomology-of-the-countably-punctured-plane)
  - [Alexander duality](cohomology.md#alexander-duality)
    - [Mod-two homology of a submanifold complement](cohomology.md#mod-two-homology-of-a-submanifold-complement)
    - [Complement homology of a compact codimension-zero submanifold](cohomology.md#complement-homology-of-a-compact-codimension-zero-submanifold)
  - [Compactly supported cohomology](cohomology.md#compactly-supported-cohomology)
    - [Top compactly supported cohomology from orientation signs](cohomology.md#top-compactly-supported-cohomology-from-orientation-signs)
    - [Compactly supported cohomology of Euclidean space](cohomology.md#compactly-supported-cohomology-of-euclidean-space)
    - [Compact-support comparison with a one-point compactification](cohomology.md#compact-support-comparison-with-a-one-point-compactification)
    - [Proper map](cohomology.md#proper-map)
  - [Cap product](cohomology.md#cap-product)
    - [Naturality of the cap product](cohomology.md#naturality-of-the-cap-product)
    - [Fundamental class](cohomology.md#fundamental-class)
      - [Local orientation of a manifold](cohomology.md#local-orientation-of-a-manifold)
      - [R-fundamental class](cohomology.md#r-fundamental-class)
      - [Poincare duality](cohomology.md#poincare-duality)
        - [Poincaré duality for noncompact manifolds](cohomology.md#poincare-duality-for-noncompact-manifolds)
        - [Rational cohomology injectivity of a nonzero-degree map](cohomology.md#rational-cohomology-injectivity-of-a-nonzero-degree-map)
        - [Third homology of a closed oriented four-manifold](cohomology.md#third-homology-of-a-closed-oriented-four-manifold)
        - [Poincare duality with the orientation local system](cohomology.md#poincare-duality-with-the-orientation-local-system)
          - [Second homology of a closed nonorientable three-manifold](cohomology.md#second-homology-of-a-closed-nonorientable-three-manifold)
        - [Intersection pairing on an oriented surface](cohomology.md#intersection-pairing-on-an-oriented-surface)
        - [Mod-two Poincare duality](cohomology.md#mod-two-poincare-duality)
        - [Euler characteristic parity in dimensions congruent to two modulo four](cohomology.md#euler-characteristic-parity-in-dimensions-congruent-to-two-modulo-four)
          - [Every even integer is the Euler characteristic of a closed oriented six-manifold](cohomology.md#every-even-integer-is-the-euler-characteristic-of-a-closed-oriented-six-manifold)
        - [Cohomological pushforward between closed oriented manifolds](cohomology.md#cohomological-pushforward-between-closed-oriented-manifolds)
        - [Poincare duality pairing](cohomology.md#poincare-duality-pairing)
          - [Even rank of middle cohomology in dimension four k plus two](cohomology.md#even-rank-of-middle-cohomology-in-dimension-four-k-plus-two)
        - [Cohomological injectivity of a map of invertible degree](cohomology.md#cohomological-injectivity-of-a-map-of-invertible-degree)
        - [Lefschetz duality](cohomology.md#lefschetz-duality)
          - [Mod-two handle duality](cohomology.md#mod-two-handle-duality)
        - [Poincare dual](cohomology.md#poincare-dual)
          - [Compactly supported dual of a compact submanifold](cohomology.md#compactly-supported-dual-of-a-compact-submanifold)
        - [Cap-product support lemma for a two-set cover](cohomology.md#cap-product-support-lemma-for-a-two-set-cover)
        - [Cohomological injectivity of a degree-one map](cohomology.md#cohomological-injectivity-of-a-degree-one-map)
        - [Homology sphere](cohomology.md#homology-sphere)
          - [Simply connected closed three-manifolds are homology spheres](cohomology.md#simply-connected-closed-three-manifolds-are-homology-spheres)
          - [Homotopy sphere](cohomology.md#homotopy-sphere)
            - [Topological generalized Poincare theorem](cohomology.md#topological-generalized-poincare-theorem)
  - [Cup product](cohomology.md#cup-product)
    - [Cup power](cohomology.md#cup-power)
    - [Cohomological cross product](cohomology.md#cohomological-cross-product)
    - [Cup length](cohomology.md#cup-length)
    - [Relative cup product](cohomology.md#relative-cup-product)
      - [Nilpotence from a contractible subcomplex cover](cohomology.md#nilpotence-from-a-contractible-subcomplex-cover)
      - [Vanishing cup product from an open cover](cohomology.md#vanishing-cup-product-from-an-open-cover)
    - [Graded commutativity of the cup product](cohomology.md#graded-commutativity-of-the-cup-product)
    - [Exterior product in cohomology](cohomology.md#exterior-product-in-cohomology)
    - [Cohomology ring](cohomology.md#cohomology-ring)
      - [Degree-one cup-square obstruction to ring isomorphism](cohomology.md#degree-one-cup-square-obstruction-to-ring-isomorphism)
      - [Cohomology ring of a product of two spheres](cohomology.md#cohomology-ring-of-a-product-of-two-spheres)
        - [Cohomology ring of a product of unequal-dimensional spheres](cohomology.md#cohomology-ring-of-a-product-of-unequal-dimensional-spheres)
        - [Cup square after a diagonal sphere attachment](cohomology.md#cup-square-after-a-diagonal-sphere-attachment)
      - [Mod-p cup-square obstruction to a homotopy equivalence](cohomology.md#mod-p-cup-square-obstruction-to-a-homotopy-equivalence)
      - [Cohomology ring of a closed oriented surface](cohomology.md#cohomology-ring-of-a-closed-oriented-surface)
  - [Künneth theorem](cohomology.md#kunneth-theorem)
    - [Cohomology cross product](cohomology.md#cohomology-cross-product)
    - [Cohomological Künneth theorem over a field](cohomology.md#cohomological-kunneth-theorem-over-a-field)
    - [Integral cohomological Künneth theorem for finite cell complexes](cohomology.md#integral-cohomological-kunneth-theorem-for-finite-cell-complexes)
    - [Diagonal-degree obstruction to a symmetric sphere retraction](cohomology.md#diagonal-degree-obstruction-to-a-symmetric-sphere-retraction)
    - [Homology cross product](cohomology.md#homology-cross-product)
      - [Eilenberg–Zilber theorem](cohomology.md#eilenberg-zilber-theorem)
    - [Integral Künneth torsion polynomial](cohomology.md#integral-kunneth-torsion-polynomial)
- [Fiber bundle](fiber-bundle.md)
  - [Affine bundle](fiber-bundle.md#affine-bundle)
  - [Section (fiber bundle)](fiber-bundle.md#section-fiber-bundle)
    - [Cohomological obstruction to a section of the twistor bundle](fiber-bundle.md#cohomological-obstruction-to-a-section-of-the-twistor-bundle)
  - [Leray-Hirsch theorem](fiber-bundle.md#leray-hirsch-theorem)
    - [Finite-cover proof of the Leray-Hirsch theorem](fiber-bundle.md#finite-cover-proof-of-the-leray-hirsch-theorem)
    - [Local basis criterion for Leray-Hirsch classes](fiber-bundle.md#local-basis-criterion-for-leray-hirsch-classes)
  - [Local trivialization](fiber-bundle.md#local-trivialization)
    - [Transition function of a vector bundle](fiber-bundle.md#transition-function-of-a-vector-bundle)
      - [Structure group of a vector bundle](fiber-bundle.md#structure-group-of-a-vector-bundle)
  - [Circle bundle](fiber-bundle.md#circle-bundle)
  - [Ehresmann fibration theorem](fiber-bundle.md#ehresmann-fibration-theorem)
  - [Principal bundle](fiber-bundle.md#principal-bundle)
    - [Principal circle bundle on real projective three-space](fiber-bundle.md#principal-circle-bundle-on-real-projective-three-space)
    - [Transition function of a principal bundle](fiber-bundle.md#transition-function-of-a-principal-bundle)
    - [Frame bundle](fiber-bundle.md#frame-bundle)
    - [Orthonormal frame bundle](fiber-bundle.md#orthonormal-frame-bundle)
      - [Oriented orthonormal frame bundle of anti-de Sitter spacetime](fiber-bundle.md#oriented-orthonormal-frame-bundle-of-anti-de-sitter-spacetime)
      - [Oriented orthonormal frame bundle of Minkowski spacetime](fiber-bundle.md#oriented-orthonormal-frame-bundle-of-minkowski-spacetime)
      - [Oriented frame bundle of de Sitter spacetime](fiber-bundle.md#oriented-frame-bundle-of-de-sitter-spacetime)
        - [Global frame on four-dimensional de Sitter spacetime](fiber-bundle.md#global-frame-on-four-dimensional-de-sitter-spacetime)
    - [Associated bundle](fiber-bundle.md#associated-bundle)
    - [Principal bundle trivialization by a global section](fiber-bundle.md#principal-bundle-trivialization-by-a-global-section)
    - [Associated vector bundle](fiber-bundle.md#associated-vector-bundle)
      - [Adjoint bundle](fiber-bundle.md#adjoint-bundle)
    - [Classifying space](fiber-bundle.md#classifying-space)
      - [Rational odd-rank stabilization of orthogonal classifying spaces](fiber-bundle.md#rational-odd-rank-stabilization-of-orthogonal-classifying-spaces)
      - [Classifying space of a discrete group](fiber-bundle.md#classifying-space-of-a-discrete-group)
    - [General linear group modulo the unitary group](fiber-bundle.md#general-linear-group-modulo-the-unitary-group)
    - [Free proper Lie-group action theorem](fiber-bundle.md#free-proper-lie-group-action-theorem)
    - [Connection (principal bundle)](fiber-bundle.md#connection-principal-bundle)
      - [Translational connection for a convex body rolling on a plane](fiber-bundle.md#translational-connection-for-a-convex-body-rolling-on-a-plane)
      - [U(1) connection](fiber-bundle.md#u-1-connection)
      - [Gauge equivalence of principal connections](fiber-bundle.md#gauge-equivalence-of-principal-connections)
      - [Local principal connection form](fiber-bundle.md#local-principal-connection-form)
        - [Reconstruction of a principal connection from local gauge potentials](fiber-bundle.md#reconstruction-of-a-principal-connection-from-local-gauge-potentials)
      - [Horizontal distribution of a principal connection](fiber-bundle.md#horizontal-distribution-of-a-principal-connection)
        - [Coordinate horizontal lifts of a principal connection](fiber-bundle.md#coordinate-horizontal-lifts-of-a-principal-connection)
        - [Horizontal section of a principal bundle](fiber-bundle.md#horizontal-section-of-a-principal-bundle)
        - [Holonomy](fiber-bundle.md#holonomy)
          - [Reducible SU2 connection](fiber-bundle.md#reducible-su2-connection)
          - [Reflection holonomy along a closed projective geodesic](fiber-bundle.md#reflection-holonomy-along-a-closed-projective-geodesic)
          - [Holonomy around circular fibres](fiber-bundle.md#holonomy-around-circular-fibres)
            - [Flat circular metrics with trivial holonomy](fiber-bundle.md#flat-circular-metrics-with-trivial-holonomy)
          - [Riemannian holonomy group](fiber-bundle.md#riemannian-holonomy-group)
            - [Holonomy representation](fiber-bundle.md#holonomy-representation)
              - [Irreducible holonomy in dimension at least two has no parallel one-form](fiber-bundle.md#irreducible-holonomy-in-dimension-at-least-two-has-no-parallel-one-form)
              - [Fundamental principle of Riemannian holonomy](fiber-bundle.md#fundamental-principle-of-riemannian-holonomy)
      - [Canonical principal connection on the Stiefel bundle over a Grassmannian](fiber-bundle.md#canonical-principal-connection-on-the-stiefel-bundle-over-a-grassmannian)
  - [Vector bundle](fiber-bundle.md#vector-bundle)
    - [Density bundle](fiber-bundle.md#density-bundle)
      - [Riemannian volume density](fiber-bundle.md#riemannian-volume-density)
    - [Tensor bundle](fiber-bundle.md#tensor-bundle)
    - [G-structure on a vector bundle](fiber-bundle.md#g-structure-on-a-vector-bundle)
    - [Globally generated vector bundle](fiber-bundle.md#globally-generated-vector-bundle)
      - [Global generation of positive twists on a smooth curve](fiber-bundle.md#global-generation-of-positive-twists-on-a-smooth-curve)
      - [Nowhere-vanishing section of a globally generated bundle on a curve](fiber-bundle.md#nowhere-vanishing-section-of-a-globally-generated-bundle-on-a-curve)
    - [Whitney sum of vector bundles](fiber-bundle.md#whitney-sum-of-vector-bundles)
    - [Symplectic vector bundle](fiber-bundle.md#symplectic-vector-bundle)
      - [Lagrangian subbundle](fiber-bundle.md#lagrangian-subbundle)
    - [Thom space](fiber-bundle.md#thom-space)
      - [Projective-space quotient as a Thom space of conjugate tautological lines](fiber-bundle.md#projective-space-quotient-as-a-thom-space-of-conjugate-tautological-lines)
    - [Line subbundle](fiber-bundle.md#line-subbundle)
    - [Birkhoff–Grothendieck theorem](fiber-bundle.md#birkhoff-grothendieck-theorem)
    - [Stable framing of a vector bundle](fiber-bundle.md#stable-framing-of-a-vector-bundle)
    - [Endomorphism bundle](fiber-bundle.md#endomorphism-bundle)
    - [Exterior power of a vector bundle](fiber-bundle.md#exterior-power-of-a-vector-bundle)
    - [Clutching construction](fiber-bundle.md#clutching-construction)
      - [Clutching function](fiber-bundle.md#clutching-function)
        - [Section obstruction for a clutched vector bundle](fiber-bundle.md#section-obstruction-for-a-clutched-vector-bundle)
    - [Clifford module bundle](fiber-bundle.md#clifford-module-bundle)
    - [Determinant line bundle](fiber-bundle.md#determinant-line-bundle)
    - [Zero section of a vector bundle](fiber-bundle.md#zero-section-of-a-vector-bundle)
    - [Fiber metric](fiber-bundle.md#fiber-metric)
      - [Orthogonal structure on a real vector bundle](fiber-bundle.md#orthogonal-structure-on-a-real-vector-bundle)
        - [Euclidean orthonormal frame](fiber-bundle.md#euclidean-orthonormal-frame)
        - [Orthogonal local trivialization](fiber-bundle.md#orthogonal-local-trivialization)
    - [Eigenbundle](fiber-bundle.md#eigenbundle)
    - [Hermitian vector bundle](fiber-bundle.md#hermitian-vector-bundle)
    - [Complex vector bundle](fiber-bundle.md#complex-vector-bundle)
      - [Hermitian metric on a smooth complex vector bundle](fiber-bundle.md#hermitian-metric-on-a-smooth-complex-vector-bundle)
      - [Stable complex structure on a real vector bundle](fiber-bundle.md#stable-complex-structure-on-a-real-vector-bundle)
      - [Conjugate vector bundle](fiber-bundle.md#conjugate-vector-bundle)
        - [Conjugate connection](fiber-bundle.md#conjugate-connection)
    - [Rank of a vector bundle](fiber-bundle.md#rank-of-a-vector-bundle)
    - [Vector bundle morphism](fiber-bundle.md#vector-bundle-morphism)
      - [Kernel bundle of a surjective vector bundle morphism](fiber-bundle.md#kernel-bundle-of-a-surjective-vector-bundle-morphism)
      - [Vector bundle endomorphism](fiber-bundle.md#vector-bundle-endomorphism)
      - [Holomorphic bundle map](fiber-bundle.md#holomorphic-bundle-map)
      - [Bundle morphisms from maps of smooth sections](fiber-bundle.md#bundle-morphisms-from-maps-of-smooth-sections)
      - [Vector bundle isomorphism](fiber-bundle.md#vector-bundle-isomorphism)
    - [Vector bundle trivialization](fiber-bundle.md#vector-bundle-trivialization)
      - [Frame of a vector bundle](fiber-bundle.md#frame-of-a-vector-bundle)
        - [Pseudo-orthonormal frame](fiber-bundle.md#pseudo-orthonormal-frame)
        - [Coframe](fiber-bundle.md#coframe)
    - [Complexification of a real vector bundle](fiber-bundle.md#complexification-of-a-real-vector-bundle)
    - [Projective bundle](fiber-bundle.md#projective-bundle)
      - [Projectivization by quotients](fiber-bundle.md#projectivization-by-quotients)
        - [Universal quotient line bundle](fiber-bundle.md#universal-quotient-line-bundle)
        - [Rational normal scroll](fiber-bundle.md#rational-normal-scroll)
          - [Fiber class of a rational normal scroll](fiber-bundle.md#fiber-class-of-a-rational-normal-scroll)
          - [Isomorphism classification of abstract rational scrolls](fiber-bundle.md#isomorphism-classification-of-abstract-rational-scrolls)
      - [Chern classes of a tautological-line complement](fiber-bundle.md#chern-classes-of-a-tautological-line-complement)
      - [Holomorphic projectivization by lines](fiber-bundle.md#holomorphic-projectivization-by-lines)
        - [Relative tautological line bundle](fiber-bundle.md#relative-tautological-line-bundle)
          - [Relative hyperplane line bundle](fiber-bundle.md#relative-hyperplane-line-bundle)
      - [Sections of a projective bundle](fiber-bundle.md#sections-of-a-projective-bundle)
      - [Orthogonal complex line flag manifold](fiber-bundle.md#orthogonal-complex-line-flag-manifold)
        - [Cohomology ring of the orthogonal complex line flag manifold](fiber-bundle.md#cohomology-ring-of-the-orthogonal-complex-line-flag-manifold)
      - [Projective bundle formula for complex vector bundles](fiber-bundle.md#projective-bundle-formula-for-complex-vector-bundles)
    - [Complex line bundle](fiber-bundle.md#complex-line-bundle)
      - [Smooth exponential sequence](fiber-bundle.md#smooth-exponential-sequence)
      - [Smooth classification of complex line bundles on the complex projective line](fiber-bundle.md#smooth-classification-of-complex-line-bundles-on-the-complex-projective-line)
    - [Real line bundle](fiber-bundle.md#real-line-bundle)
      - [Möbius line bundle](fiber-bundle.md#mobius-line-bundle)
      - [Classification of real line bundles](fiber-bundle.md#classification-of-real-line-bundles)
      - [Mod-two Euler class of a real line bundle](fiber-bundle.md#mod-two-euler-class-of-a-real-line-bundle)
    - [Vector subbundle](fiber-bundle.md#vector-subbundle)
      - [Orthogonal splitting of a vector subbundle](fiber-bundle.md#orthogonal-splitting-of-a-vector-subbundle)
      - [Quotient vector bundle](fiber-bundle.md#quotient-vector-bundle)
        - [Universal quotient bundle on a real Grassmannian](fiber-bundle.md#universal-quotient-bundle-on-a-real-grassmannian)
          - [Universal quotient bundle need not have a nowhere-zero section](fiber-bundle.md#universal-quotient-bundle-need-not-have-a-nowhere-zero-section)
          - [Classification of vector bundles by a universal quotient bundle](fiber-bundle.md#classification-of-vector-bundles-by-a-universal-quotient-bundle)
    - [Trivial vector bundle](fiber-bundle.md#trivial-vector-bundle)
    - [Section of a vector bundle](fiber-bundle.md#section-of-a-vector-bundle)
      - [Regular zero locus](fiber-bundle.md#regular-zero-locus)
      - [Module of smooth sections](fiber-bundle.md#module-of-smooth-sections)
      - [Nowhere-zero section](fiber-bundle.md#nowhere-zero-section)
        - [Nonvanishing tangent field on an odd-dimensional sphere](fiber-bundle.md#nonvanishing-tangent-field-on-an-odd-dimensional-sphere)
        - [Splitting a trivial line from a nowhere-zero section](fiber-bundle.md#splitting-a-trivial-line-from-a-nowhere-zero-section)
        - [Hairy ball theorem](fiber-bundle.md#hairy-ball-theorem)
          - [Degree proof of the hairy ball theorem](fiber-bundle.md#degree-proof-of-the-hairy-ball-theorem)
    - [Sphere bundle](fiber-bundle.md#sphere-bundle)
      - [Three-sphere bundle over the four-sphere](fiber-bundle.md#three-sphere-bundle-over-the-four-sphere)
      - [Unit tangent bundle](fiber-bundle.md#unit-tangent-bundle)
        - [Canonical coframe of a surface unit tangent bundle](fiber-bundle.md#canonical-coframe-of-a-surface-unit-tangent-bundle)
          - [Vertical vector field of a surface unit tangent bundle](fiber-bundle.md#vertical-vector-field-of-a-surface-unit-tangent-bundle)
          - [Liouville volume of a surface geodesic flow](fiber-bundle.md#liouville-volume-of-a-surface-geodesic-flow)
        - [Stiefel manifold](fiber-bundle.md#stiefel-manifold)
          - [Unordered Stiefel bundle](fiber-bundle.md#unordered-stiefel-bundle)
            - [Subset cover of a framed vector bundle](fiber-bundle.md#subset-cover-of-a-framed-vector-bundle)
          - [Complex Stiefel manifold](fiber-bundle.md#complex-stiefel-manifold)
            - [Integral cohomology of a complex Stiefel manifold](fiber-bundle.md#integral-cohomology-of-a-complex-stiefel-manifold)
            - [Complement bundle on a complex Stiefel manifold](fiber-bundle.md#complement-bundle-on-a-complex-stiefel-manifold)
        - [Cohomology of the unit tangent bundle of an even-dimensional sphere](fiber-bundle.md#cohomology-of-the-unit-tangent-bundle-of-an-even-dimensional-sphere)
    - [Disk bundle](fiber-bundle.md#disk-bundle)
      - [Plumbing of oriented disk bundles](fiber-bundle.md#plumbing-of-oriented-disk-bundles)
    - [Tangent bundle](fiber-bundle.md#tangent-bundle)
      - [Stabilized tangent bundle of real projective space](fiber-bundle.md#stabilized-tangent-bundle-of-real-projective-space)
      - [Tangent coordinate transition](fiber-bundle.md#tangent-coordinate-transition)
    - [Projectivization of a real vector bundle](fiber-bundle.md#projectivization-of-a-real-vector-bundle)
      - [Tangent bundle of a projectivized real vector bundle](fiber-bundle.md#tangent-bundle-of-a-projectivized-real-vector-bundle)
      - [Projectivization of copies of the real tautological line bundle](fiber-bundle.md#projectivization-of-copies-of-the-real-tautological-line-bundle)
    - [Dual bundle](fiber-bundle.md#dual-bundle)
      - [Canonical trivialization of a line bundle tensored with its dual](fiber-bundle.md#canonical-trivialization-of-a-line-bundle-tensored-with-its-dual)
    - [Pullback vector bundle](fiber-bundle.md#pullback-vector-bundle)
      - [Pullback tangent bundle](fiber-bundle.md#pullback-tangent-bundle)
        - [Vector field along a map](fiber-bundle.md#vector-field-along-a-map)
          - [Local extension of a vector field along a submanifold](fiber-bundle.md#local-extension-of-a-vector-field-along-a-submanifold)
          - [Vector field along a curve](fiber-bundle.md#vector-field-along-a-curve)
    - [Kernel bundle of a constant-rank family of linear maps](fiber-bundle.md#kernel-bundle-of-a-constant-rank-family-of-linear-maps)
    - [Tensor product of vector bundles](fiber-bundle.md#tensor-product-of-vector-bundles)
      - [Second Chern class of a tensor product of rank-two bundles](fiber-bundle.md#second-chern-class-of-a-tensor-product-of-rank-two-bundles)
      - [Tensor field](fiber-bundle.md#tensor-field)
        - [Lie derivative of a covariant tensor field](fiber-bundle.md#lie-derivative-of-a-covariant-tensor-field)
        - [Tensoriality](fiber-bundle.md#tensoriality)
        - [Tensor derivation](fiber-bundle.md#tensor-derivation)
          - [Lie derivative of a tensor field](fiber-bundle.md#lie-derivative-of-a-tensor-field)
            - [Lie derivative at a zero of its generator](fiber-bundle.md#lie-derivative-at-a-zero-of-its-generator)
            - [Coordinate tensor Lie derivative](fiber-bundle.md#coordinate-tensor-lie-derivative)
            - [Commutator identity for Lie derivatives](fiber-bundle.md#commutator-identity-for-lie-derivatives)
            - [Lie derivative of a vector field](fiber-bundle.md#lie-derivative-of-a-vector-field)
            - [Lie derivative of a function](fiber-bundle.md#lie-derivative-of-a-function)
            - [Flow definition of the Lie derivative of a tensor field](fiber-bundle.md#flow-definition-of-the-lie-derivative-of-a-tensor-field)
            - [Scaled Lie derivative defect identity](fiber-bundle.md#scaled-lie-derivative-defect-identity)
          - [Endomorphism-induced tensor derivation](fiber-bundle.md#endomorphism-induced-tensor-derivation)
    - [Connection (vector bundle)](fiber-bundle.md#connection-vector-bundle)
      - [Parallel vector field](fiber-bundle.md#parallel-vector-field)
      - [Projection connection](fiber-bundle.md#projection-connection)
      - [Connection difference as an endomorphism-valued one-form](fiber-bundle.md#connection-difference-as-an-endomorphism-valued-one-form)
      - [Change of frame of a vector-bundle connection](fiber-bundle.md#change-of-frame-of-a-vector-bundle-connection)
      - [Affine space of vector-bundle connections](fiber-bundle.md#affine-space-of-vector-bundle-connections)
      - [Construction of a vector bundle connection by a partition of unity](fiber-bundle.md#construction-of-a-vector-bundle-connection-by-a-partition-of-unity)
      - [Determinant connection](fiber-bundle.md#determinant-connection)
      - [Rough Laplacian](fiber-bundle.md#rough-laplacian)
      - [Affine connection](fiber-bundle.md#affine-connection)
        - [Projective equivalence of affine connections](fiber-bundle.md#projective-equivalence-of-affine-connections)
          - [Geodesic reparametrization under projective equivalence](fiber-bundle.md#geodesic-reparametrization-under-projective-equivalence)
          - [Projective covector from metric volume densities](fiber-bundle.md#projective-covector-from-metric-volume-densities)
        - [Bracket connection on a Lie group](fiber-bundle.md#bracket-connection-on-a-lie-group)
        - [Connection components](fiber-bundle.md#connection-components)
        - [Affine exponential map](fiber-bundle.md#affine-exponential-map)
          - [Affine normal coordinates](fiber-bundle.md#affine-normal-coordinates)
        - [Affine connection decomposition](fiber-bundle.md#affine-connection-decomposition)
        - [Nonmetricity tensor](fiber-bundle.md#nonmetricity-tensor)
          - [Disformation tensor](fiber-bundle.md#disformation-tensor)
        - [Torsion tensor](fiber-bundle.md#torsion-tensor)
          - [Contorsion tensor](fiber-bundle.md#contorsion-tensor)
        - [Parallel covector field](fiber-bundle.md#parallel-covector-field)
        - [Projected ambient connection](fiber-bundle.md#projected-ambient-connection)
        - [Difference of affine connections is a tensor](fiber-bundle.md#difference-of-affine-connections-is-a-tensor)
          - [Parametrized geodesics determine the symmetric part of an affine connection](fiber-bundle.md#parametrized-geodesics-determine-the-symmetric-part-of-an-affine-connection)
            - [Torsion-free connections are determined by their parametrized geodesics](fiber-bundle.md#torsion-free-connections-are-determined-by-their-parametrized-geodesics)
        - [Affine connection for a velocity-linear force](fiber-bundle.md#affine-connection-for-a-velocity-linear-force)
        - [Product affine connection](fiber-bundle.md#product-affine-connection)
          - [Curvature splitting for a product connection](fiber-bundle.md#curvature-splitting-for-a-product-connection)
      - [Covariant derivative along a curve](fiber-bundle.md#covariant-derivative-along-a-curve)
      - [Connection one-form](fiber-bundle.md#connection-one-form)
      - [Exterior covariant derivative](fiber-bundle.md#exterior-covariant-derivative)
        - [Endomorphism-valued exterior product](fiber-bundle.md#endomorphism-valued-exterior-product)
      - [Horizontal subspace of a vector bundle connection](fiber-bundle.md#horizontal-subspace-of-a-vector-bundle-connection)
        - [Linear horizontal distribution on a vector bundle](fiber-bundle.md#linear-horizontal-distribution-on-a-vector-bundle)
        - [Horizontal connection associated to a covariant derivative](fiber-bundle.md#horizontal-connection-associated-to-a-covariant-derivative)
      - [Pullback connection](fiber-bundle.md#pullback-connection)
        - [Curvature of a pullback connection](fiber-bundle.md#curvature-of-a-pullback-connection)
        - [Restriction of a connection to an embedded submanifold](fiber-bundle.md#restriction-of-a-connection-to-an-embedded-submanifold)
      - [Dual connection](fiber-bundle.md#dual-connection)
      - [Tensor product connection](fiber-bundle.md#tensor-product-connection)
        - [Curvature of a tensor product connection](fiber-bundle.md#curvature-of-a-tensor-product-connection)
      - [Endomorphism bundle connection](fiber-bundle.md#endomorphism-bundle-connection)
        - [Commutator identity for an endomorphism connection](fiber-bundle.md#commutator-identity-for-an-endomorphism-connection)
        - [Curvature of an endomorphism bundle connection](fiber-bundle.md#curvature-of-an-endomorphism-bundle-connection)
          - [Scalar-curvature criterion for a flat endomorphism connection](fiber-bundle.md#scalar-curvature-criterion-for-a-flat-endomorphism-connection)
      - [Solder form](fiber-bundle.md#solder-form)
        - [Torsion form](fiber-bundle.md#torsion-form)
          - [Cartan first structure equation with input-first indices](fiber-bundle.md#cartan-first-structure-equation-with-input-first-indices)
          - [Torsion-free connection](fiber-bundle.md#torsion-free-connection)
      - [Metric connection](fiber-bundle.md#metric-connection)
        - [Metric compatibility](fiber-bundle.md#metric-compatibility)
          - [Lie derivative of a metric with nonmetricity](fiber-bundle.md#lie-derivative-of-a-metric-with-nonmetricity)
        - [Normal connection](fiber-bundle.md#normal-connection)
        - [Skew-adjoint difference criterion for metric connections](fiber-bundle.md#skew-adjoint-difference-criterion-for-metric-connections)
        - [Smooth unitary frame for a Hermitian connection](fiber-bundle.md#smooth-unitary-frame-for-a-hermitian-connection)
        - [Parallel transport preserves a fibre metric](fiber-bundle.md#parallel-transport-preserves-a-fibre-metric)
        - [Connection matrix in an orthonormal frame is skew-symmetric](fiber-bundle.md#connection-matrix-in-an-orthonormal-frame-is-skew-symmetric)
        - [Koszul formula](fiber-bundle.md#koszul-formula)
          - [Existence and uniqueness of the Levi-Civita connection](fiber-bundle.md#existence-and-uniqueness-of-the-levi-civita-connection)
        - [Unitary connection](fiber-bundle.md#unitary-connection)
          - [Uhlenbeck small-energy Coulomb gauge](fiber-bundle.md#uhlenbeck-small-energy-coulomb-gauge)
          - [Harmonic-curvature unitary line connection](fiber-bundle.md#harmonic-curvature-unitary-line-connection)
          - [Unitary bundle gauge transformation](fiber-bundle.md#unitary-bundle-gauge-transformation)
            - [Unitary bundle gauge group](fiber-bundle.md#unitary-bundle-gauge-group)
              - [Coulomb slice for unitary connections](fiber-bundle.md#coulomb-slice-for-unitary-connections)
              - [Based unitary gauge group](fiber-bundle.md#based-unitary-gauge-group)
          - [Anti-self-dual connection](fiber-bundle.md#anti-self-dual-connection)
            - [Abelian anti-self-dual connections from harmonic scalar potentials](fiber-bundle.md#abelian-anti-self-dual-connections-from-harmonic-scalar-potentials)
            - [ASD deformation complex](fiber-bundle.md#asd-deformation-complex)
              - [Local cone at an unobstructed reducible SU2 instanton](fiber-bundle.md#local-cone-at-an-unobstructed-reducible-su2-instanton)
              - [ASD deformation index](fiber-bundle.md#asd-deformation-index)
            - [Uhlenbeck-Donaldson compactness for charge-one ASD connections](fiber-bundle.md#uhlenbeck-donaldson-compactness-for-charge-one-asd-connections)
            - [Uhlenbeck removable singularity theorem for ASD connections](fiber-bundle.md#uhlenbeck-removable-singularity-theorem-for-asd-connections)
            - [Positive-square obstruction to ASD line connections](fiber-bundle.md#positive-square-obstruction-to-asd-line-connections)
      - [Horizontal lift](fiber-bundle.md#horizontal-lift)
        - [Parallel transport](fiber-bundle.md#parallel-transport)
          - [Parallel vector field along a curve](fiber-bundle.md#parallel-vector-field-along-a-curve)
          - [Parallel transport around a spherical triangle](fiber-bundle.md#parallel-transport-around-a-spherical-triangle)
          - [Global continuation of linear parallel transport](fiber-bundle.md#global-continuation-of-linear-parallel-transport)
          - [Parallel frame along a curve](fiber-bundle.md#parallel-frame-along-a-curve)
          - [Parallel transport on an endomorphism bundle](fiber-bundle.md#parallel-transport-on-an-endomorphism-bundle)
          - [Parallel transport around a latitude of the unit sphere](fiber-bundle.md#parallel-transport-around-a-latitude-of-the-unit-sphere)
    - [Orientation of a vector bundle](fiber-bundle.md#orientation-of-a-vector-bundle)
      - [Orientability of a vector bundle total space](fiber-bundle.md#orientability-of-a-vector-bundle-total-space)
      - [Canonical orientation of a complex vector bundle](fiber-bundle.md#canonical-orientation-of-a-complex-vector-bundle)
      - [Thom class](fiber-bundle.md#thom-class)
        - [Cohomology class of a cooriented submanifold](fiber-bundle.md#cohomology-class-of-a-cooriented-submanifold)
        - [Thom class in a generalized cohomology theory](fiber-bundle.md#thom-class-in-a-generalized-cohomology-theory)
        - [Cup square of a Thom class](fiber-bundle.md#cup-square-of-a-thom-class)
        - [Thom isomorphism theorem](fiber-bundle.md#thom-isomorphism-theorem)
          - [Gysin sequence of an embedding](fiber-bundle.md#gysin-sequence-of-an-embedding)
            - [Cohomological Gysin map of an embedding](fiber-bundle.md#cohomological-gysin-map-of-an-embedding)
        - [Euler class of a vector bundle](fiber-bundle.md#euler-class-of-a-vector-bundle)
          - [Euler class in a generalized cohomology theory](fiber-bundle.md#euler-class-in-a-generalized-cohomology-theory)
            - [A nowhere-zero section annihilates generalized Euler classes](fiber-bundle.md#a-nowhere-zero-section-annihilates-generalized-euler-classes)
          - [Euler class of a complex vector bundle](fiber-bundle.md#euler-class-of-a-complex-vector-bundle)
          - [Euler class of an oriented odd-rank vector bundle is two-torsion](fiber-bundle.md#euler-class-of-an-oriented-odd-rank-vector-bundle-is-two-torsion)
          - [Whitney product formula for Euler classes](fiber-bundle.md#whitney-product-formula-for-euler-classes)
          - [Euler number of a vector bundle](fiber-bundle.md#euler-number-of-a-vector-bundle)
          - [Poincaré-Hopf theorem](fiber-bundle.md#poincare-hopf-theorem)
          - [Euler class of a complex line bundle](fiber-bundle.md#euler-class-of-a-complex-line-bundle)
          - [Gysin sequence of a sphere bundle](fiber-bundle.md#gysin-sequence-of-a-sphere-bundle)
            - [Gysin ring splitting for an odd-dimensional sphere bundle](fiber-bundle.md#gysin-ring-splitting-for-an-odd-dimensional-sphere-bundle)
            - [Projection formula for sphere bundle integration](fiber-bundle.md#projection-formula-for-sphere-bundle-integration)
            - [Unoriented Gysin sequence](fiber-bundle.md#unoriented-gysin-sequence)
            - [Three-dimensional lens space as a circle bundle](fiber-bundle.md#three-dimensional-lens-space-as-a-circle-bundle)
            - [Integral cohomology of a circle bundle over a product of two spheres](fiber-bundle.md#integral-cohomology-of-a-circle-bundle-over-a-product-of-two-spheres)
    - [Tautological bundle](fiber-bundle.md#tautological-bundle)
      - [Complex tautological bundle on a Grassmannian](fiber-bundle.md#complex-tautological-bundle-on-a-grassmannian)
        - [Classification of complex vector bundles by a Grassmannian](fiber-bundle.md#classification-of-complex-vector-bundles-by-a-grassmannian)
          - [Rank-two complex vector bundles over the four-sphere](fiber-bundle.md#rank-two-complex-vector-bundles-over-the-four-sphere)
          - [Close orthogonal projections identify their image bundles](fiber-bundle.md#close-orthogonal-projections-identify-their-image-bundles)
          - [Finite-dimensional embedding of a complex vector bundle](fiber-bundle.md#finite-dimensional-embedding-of-a-complex-vector-bundle)
      - [Complex tautological line bundle](fiber-bundle.md#complex-tautological-line-bundle)
        - [Punctured line bundles do not determine their duality sign](fiber-bundle.md#punctured-line-bundles-do-not-determine-their-duality-sign)
        - [Unitary transitions of the tautological line over the projective line](fiber-bundle.md#unitary-transitions-of-the-tautological-line-over-the-projective-line)
        - [Global holomorphic sections of the complex tautological line bundle vanish](fiber-bundle.md#global-holomorphic-sections-of-the-complex-tautological-line-bundle-vanish)
        - [Hyperplane line bundle](fiber-bundle.md#hyperplane-line-bundle)
          - [Hyperplane class](fiber-bundle.md#hyperplane-class)
          - [Nontrivial hyperplane powers on a compact projective submanifold](fiber-bundle.md#nontrivial-hyperplane-powers-on-a-compact-projective-submanifold)
          - [Tensor powers of the hyperplane line bundle](fiber-bundle.md#tensor-powers-of-the-hyperplane-line-bundle)
      - [Quaternionic tautological line bundle](fiber-bundle.md#quaternionic-tautological-line-bundle)
      - [Real tautological line bundle](fiber-bundle.md#real-tautological-line-bundle)
    - [Stiefel–Whitney class](fiber-bundle.md#stiefel-whitney-class)
      - [Parity of zeros of a real line-bundle section](fiber-bundle.md#parity-of-zeros-of-a-real-line-bundle-section)
      - [Codimension-one Stiefel–Whitney immersion obstruction](fiber-bundle.md#codimension-one-stiefel-whitney-immersion-obstruction)
      - [Stiefel–Whitney class of the underlying real bundle of a complex line](fiber-bundle.md#stiefel-whitney-class-of-the-underlying-real-bundle-of-a-complex-line)
      - [Projective bundle definition of Stiefel–Whitney classes](fiber-bundle.md#projective-bundle-definition-of-stiefel-whitney-classes)
      - [Splitting principle for real vector bundles](fiber-bundle.md#splitting-principle-for-real-vector-bundles)
        - [Whitney product formula for Stiefel–Whitney classes](fiber-bundle.md#whitney-product-formula-for-stiefel-whitney-classes)
          - [Stiefel–Whitney obstruction to a diagonal projective immersion](fiber-bundle.md#stiefel-whitney-obstruction-to-a-diagonal-projective-immersion)
      - [Bockstein of a Stiefel–Whitney class](fiber-bundle.md#bockstein-of-a-stiefel-whitney-class)
      - [First Stiefel–Whitney class of a tensor product of real line bundles](fiber-bundle.md#first-stiefel-whitney-class-of-a-tensor-product-of-real-line-bundles)
      - [Total Stiefel–Whitney class of the projectivization of copies of the tautological line](fiber-bundle.md#total-stiefel-whitney-class-of-the-projectivization-of-copies-of-the-tautological-line)
  - [Curvature form](fiber-bundle.md#curvature-form)
    - [Curvature of a principal connection](fiber-bundle.md#curvature-of-a-principal-connection)
      - [Flat principal connection](fiber-bundle.md#flat-principal-connection)
    - [Trace of vector-bundle curvature](fiber-bundle.md#trace-of-vector-bundle-curvature)
    - [Cartan curvature matrix equation](fiber-bundle.md#cartan-curvature-matrix-equation)
      - [Cartan curvature equation with input indices](fiber-bundle.md#cartan-curvature-equation-with-input-indices)
    - [Riemannian curvature two-form](fiber-bundle.md#riemannian-curvature-two-form)
    - [Curvature difference formula](fiber-bundle.md#curvature-difference-formula)
      - [Trace curvature transgression](fiber-bundle.md#trace-curvature-transgression)
        - [Connection-independent curvature class of a line bundle](fiber-bundle.md#connection-independent-curvature-class-of-a-line-bundle)
    - [Bianchi identity](fiber-bundle.md#bianchi-identity)
- [Complex projective space](#complex-projective-space)
  - [Differential of the projective quotient map](#differential-of-the-projective-quotient-map)
  - [Cellular homology of complex projective space](#cellular-homology-of-complex-projective-space)
  - [Fixed-point property of even-dimensional complex projective space](#fixed-point-property-of-even-dimensional-complex-projective-space)
    - [Complex projective plane has no nontrivial covering quotient](#complex-projective-plane-has-no-nontrivial-covering-quotient)
  - [Polynomial multiplication map to complex projective space](#polynomial-multiplication-map-to-complex-projective-space)
  - [Complex projective plane](#complex-projective-plane)
    - [Projective lines generate a unimodular intersection form](#projective-lines-generate-a-unimodular-intersection-form)
  - [Projective hyperplane](#projective-hyperplane)
  - [Euler sequence on complex projective space](#euler-sequence-on-complex-projective-space)
    - [Canonical bundle of complex projective space](#canonical-bundle-of-complex-projective-space)
      - [Canonical bundle of a smooth projective hypersurface](#canonical-bundle-of-a-smooth-projective-hypersurface)
        - [Canonical degree of a smooth plane curve](#canonical-degree-of-a-smooth-plane-curve)
  - [Complex projective line](#complex-projective-line)
  - [Hopf fibration](#hopf-fibration)
    - [Hopf projection of a product smash quotient](#hopf-projection-of-a-product-smash-quotient)
    - [Hopf map](#hopf-map)
  - [Cohomology ring of complex projective space](#cohomology-ring-of-complex-projective-space)
    - [Diagonal class of complex projective space](#diagonal-class-of-complex-projective-space)
    - [Factorial degree obstruction for products of two-spheres](#factorial-degree-obstruction-for-products-of-two-spheres)
    - [Mod-two restriction from complex to real projective space](#mod-two-restriction-from-complex-to-real-projective-space)
      - [Cohomology ring of the complement of even-dimensional real projective space](#cohomology-ring-of-the-complement-of-even-dimensional-real-projective-space)
    - [Cohomology automorphisms of a product of two complex projective spaces](#cohomology-automorphisms-of-a-product-of-two-complex-projective-spaces)
    - [Cohomology ring of a collapsed projective subspace](#cohomology-ring-of-a-collapsed-projective-subspace)
- [Topological K-theory](#topological-k-theory)
  - [Odd topological K-theory](#odd-topological-k-theory)
  - [Complex K-theory of odd-dimensional real projective space](#complex-k-theory-of-odd-dimensional-real-projective-space)
  - [K-theory transfer of a finite covering](#k-theory-transfer-of-a-finite-covering)
    - [Projection formula for the K-theory transfer](#projection-formula-for-the-k-theory-transfer)
  - [Rank map in topological K-theory](#rank-map-in-topological-k-theory)
    - [Nilpotence of rank-zero K-theory classes](#nilpotence-of-rank-zero-k-theory-classes)
  - [Relative topological K-theory](#relative-topological-k-theory)
    - [Relative product in topological K-theory](#relative-product-in-topological-k-theory)
  - [K-theory six-term exact sequence](#k-theory-six-term-exact-sequence)
  - [Grothendieck group](#grothendieck-group)
  - [Reduced topological K-theory](#reduced-topological-k-theory)
  - [Bott isomorphism](#bott-isomorphism)
    - [Bott element](#bott-element)
    - [Complex K-theory of a sphere](#complex-k-theory-of-a-sphere)
  - [Complex K-theory of an even-cell complex](#complex-k-theory-of-an-even-cell-complex)
    - [Künneth theorem for complex K-theory with an even-cell factor](#kunneth-theorem-for-complex-k-theory-with-an-even-cell-factor)
  - [Complex K-theory of complex projective space](#complex-k-theory-of-complex-projective-space)
  - [Stable cancellation for complex vector bundles](#stable-cancellation-for-complex-vector-bundles)
    - [Chern classes classify rank-d complex vector bundles over CPd](#chern-classes-classify-rank-d-complex-vector-bundles-over-cpd)
  - [K-theory Wang sequence of a mapping torus](#k-theory-wang-sequence-of-a-mapping-torus)
    - [K-theory of the mapping torus of the factor swap on two complex projective planes](#k-theory-of-the-mapping-torus-of-the-factor-swap-on-two-complex-projective-planes)
  - [Splitting principle for complex vector bundles](#splitting-principle-for-complex-vector-bundles)
    - [Chern root](#chern-root)
    - [Chern character](#chern-character)
      - [Chern character on an even-dimensional sphere is integral](#chern-character-on-an-even-dimensional-sphere-is-integral)
        - [Divisibility of the top Chern number on an even-dimensional sphere](#divisibility-of-the-top-chern-number-on-an-even-dimensional-sphere)
  - [K-theory Thom class](#k-theory-thom-class)
    - [K-theory Euler class](#k-theory-euler-class)
      - [K-theory Euler class of the tangent bundle of complex projective space](#k-theory-euler-class-of-the-tangent-bundle-of-complex-projective-space)
    - [K-theory Gysin sequence of a sphere bundle](#k-theory-gysin-sequence-of-a-sphere-bundle)
      - [K-theory of the sphere bundle of copies of a complexified real tautological line](#k-theory-of-the-sphere-bundle-of-copies-of-a-complexified-real-tautological-line)
      - [K-theory of the unit tangent sphere bundle of complex projective space](#k-theory-of-the-unit-tangent-sphere-bundle-of-complex-projective-space)
      - [Odd K-theory of the sphere bundle of two tautological lines](#odd-k-theory-of-the-sphere-bundle-of-two-tautological-lines)
  - [Adams operation](#adams-operation)
    - [Adams operation on a Bott class](#adams-operation-on-a-bott-class)
      - [Adams-operation obstruction to retracting a truncated complex projective space](#adams-operation-obstruction-to-retracting-a-truncated-complex-projective-space)
    - [Cannibalistic class](#cannibalistic-class)
      - [Adams operation and the boundary pushforward of a sphere bundle](#adams-operation-and-the-boundary-pushforward-of-a-sphere-bundle)
        - [Second Adams operation on the odd K-theory of the sphere bundle of two tautological lines](#second-adams-operation-on-the-odd-k-theory-of-the-sphere-bundle-of-two-tautological-lines)
- [Reidemeister torsion](#reidemeister-torsion)

## Intersection homology

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Intersection_homology)

[Intersection homology](#intersection-homology) is the homology of a [chain complex](homology.md#chain-complex) in which chains and their boundaries satisfy codimension-dependent [perversity](#perversity) restrictions at singular strata. Unless specified otherwise coefficients here are $\mathbb Q$. Ordinary homology is recovered on [manifolds](topology.md#topological-manifold).

### Perversity

↑ **Parent:** [Intersection homology](#intersection-homology)

A traditional perversity is a function $\bar p:\{2,3,\ldots\}\to\mathbb Z$ satisfying $\bar p(2)=0$ and $\bar p(k+1)-\bar p(k)\in\{0,1\}$. It specifies how far chains may meet strata of codimension $k$.

#### Allowable singular simplex

↑ **Parent:** [Perversity](#perversity)

An $i$-dimensional [singular simplex](homology.md#singular-simplex) $\sigma:\Delta^i\to X$ is $\bar p$-allowable if $\sigma^{-1}(X_{N-k})$ is contained in the $(i-k+\bar p(k))$-skeleton of $\Delta^i$ for every $k\ge2$. A negative skeleton is empty. Individual faces need not be allowable; this is why the definition of [intersection chains](#intersection-chains) separately imposes allowability on the total boundary.

##### Intersection chains

↑ **Parent:** [Allowable singular simplex](#allowable-singular-simplex)

The group $IS_i^{\bar p}(X)$ consists of finite [singular chains](homology.md#singular-chain) whose nonzero simplices are [allowable singular simplices](#allowable-singular-simplex) and whose boundary, after cancellation, also consists of allowable simplices. Since $\partial^2=0$, these groups form a [chain complex](homology.md#chain-complex). Its homology is [intersection homology](#intersection-homology).

#### Upper middle perversity

↑ **Parent:** [Perversity](#perversity)

The [upper middle perversity](#upper-middle-perversity) is $\bar n(k)=\lceil(k-2)/2\rceil$. It differs from the [lower middle perversity](#lower-middle-perversity) by one at odd codimensions, and is complementary to it.

#### Lower middle perversity

↑ **Parent:** [Perversity](#perversity)

The [lower middle perversity](#lower-middle-perversity) is $\bar m(k)=\lfloor(k-2)/2\rfloor$. The complementary [upper middle perversity](#upper-middle-perversity) is $\bar n(k)=\lceil(k-2)/2\rceil$, and $\bar m(k)+\bar n(k)=k-2$. They agree at even codimensions.

### Intersection homology cone formula

↑ **Parent:** [Intersection homology](#intersection-homology)

For a compact $(N-1)$-dimensional link $L$ and traditional perversity $\bar p$, finite-chain [intersection homology](#intersection-homology) of its open cone is $IH_i^{\bar p}(cL)=IH_i^{\bar p}(L)$ for $i<N-1-\bar p(N)$ and zero for $i\ge N-1-\bar p(N)$. Below the cutoff both chains and possible filling chains avoid the vertex. At and above the cutoff the cone on any allowable cycle is an allowable filling: its new vertex is allowed precisely when $0\le i+1-N+\bar p(N)$.

#### Intersection homology of an even-dimensional suspension

↑ **Parent:** [Intersection homology cone formula](#intersection-homology-cone-formula)

For $\dim L=2n-1$ and [lower middle perversity](#lower-middle-perversity), the suspension with two distinct vertices has $IH_i(\operatorname{Susp}L)=IH_i(L)$ for $i<n$, zero for $i=n$, and $IH_{i-1}(L)$ for $i>n$. Cover it by its two open cones. The [Mayer–Vietoris sequence](#mayer-vietoris-sequence) compares their truncated groups with $IH_*(L)$; below $n$ the overlap map is the injective signed diagonal, and above $n$ both cone groups vanish.

### Intersection cohomology

↑ **Parent:** [Intersection homology](#intersection-homology)

In the Deligne-sheaf convention, $IH_{\bar p}^i(X)=\mathbb H^i(X,IC_{\bar p})$, with $IC_{\bar p}$ normalized in degree zero on the regular stratum. For a compact oriented $N$-dimensional pseudomanifold over a field, $IH_{\bar p}^i(X)\cong IH_{N-i}^{\bar p}(X)$ and it is dual to $IH_i^{\bar q}(X)$, where $\bar p(k)+\bar q(k)=k-2$. Thus the dual of lower-middle [singular chains](homology.md#singular-chain) uses the upper-middle Deligne [sheaf](algebraic-geometry.md#sheaf-mathematics). The two middle conventions agree on [Witt spaces](topology.md#witt-space).

#### Capped-boundary intersection cohomology

↑ **Parent:** [Intersection cohomology](#intersection-cohomology)

Let a compact oriented $(2m+1)$-manifold $M$ have collared boundary $B$, and cap $B$ by its closed cone. In the lower-middle Deligne convention the result has $IH^i=H^i(M)$ for $i<m$, $IH^m=\operatorname{im}(H^m(M,B)\to H^m(M))$, and $IH^i=H^i(M,B)$ for $i>m$. [Excision](homology.md#excision-theorem) identifies the relative intersection groups with $H^*(M,B)$; the cone neighbourhood has $H^i(B)$ only for $i<m$, so its long exact sequence gives the formula. The cap is Witt exactly when $H^m(B;\mathbb Q)=0$.

#### Intersection complex

↑ **Parent:** [Intersection cohomology](#intersection-cohomology)

The degree-zero normalized Deligne [intersection complex](#intersection-complex) extends the constant [sheaf](algebraic-geometry.md#sheaf-mathematics) from the regular stratum by successive derived direct images and cohomological truncations at degree $\bar p(k)$ when codimension-$k$ strata are added. Its [hypercohomology](ringed-space.md#hypercohomology) defines [intersection cohomology](#intersection-cohomology). On a cone with vertex of codimension $k$, its local [cohomology](cohomology.md) is the link [intersection cohomology](#intersection-cohomology) in degrees at most $\bar p(k)$ and zero above.

##### Intersection-complex support and cosupport axioms

↑ **Parent:** [Intersection complex](#intersection-complex)

For an isolated singular point of an $N$-dimensional oriented pseudomanifold, the unshifted middle [intersection complex](#intersection-complex) restricts to $\mathbb Q$ on the regular stratum and has no negative [cohomology](cohomology.md). Its support condition is $H^j(i_x^*IC_{\bar p})=0$ for $j>\bar p(N)$; its cosupport condition is $H^j(i_x^!IC_{\bar p})=0$ for $j\le\bar p(N)+1$. These conditions, together with constructibility and normalization, characterize it. On a [Witt space](topology.md#witt-space) they are exchanged by $IC\cong D(IC)[-N]$.

## Homotopy colimit of spaces

↑ **Parent:** [Algebraic topology](algebraic-topology.md)

A [homotopy colimit of spaces](#homotopy-colimit-of-spaces) is the homotopy-invariant replacement for a [colimit](category.md#colimit) of spaces. For a filtered diagram of [CW complexes](#cw-complex) with subcomplex inclusions, the union is a model: the inclusions are [cofibrations](#cofibration), and every sphere map and homotopy has image in a finite subcomplex. A [suspension spectrum](#suspension-spectrum) carries this construction to the corresponding [homotopy colimit of spectra](#homotopy-colimit-of-spectra).

## Stable homotopy theory

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stable_homotopy_theory)

[Stable homotopy theory](#stable-homotopy-theory) studies [topological spectra](#spectrum-topology), which retain the information that persists under repeated [reduced suspension](#reduced-suspension). Its [stable homotopy category](#stable-homotopy-category) admits invertible [suspension of spectra](#suspension-of-spectra) and exact [cofiber sequences of spectra](#cofiber-sequence-of-spectra).

### Universe for spectra

↑ **Parent:** [Stable homotopy theory](#stable-homotopy-theory)

A [universe for spectra](#universe-for-spectra) is a countably infinite-dimensional real [inner product space](linear-algebra.md#inner-product-space), normally with its direct-limit topology, used to index finite-dimensional suspension coordinates. A cofinal indexing family contains arbitrarily large finite-dimensional subspaces.

#### Subordinate flag for a family of linear isometries

↑ **Parent:** [Universe for spectra](#universe-for-spectra)

Given a compact parameter space $X$ and a family $f_x:U\to U\prime$ of [linear isometries](hilbert-space.md#linear-isometry-of-hilbert-spaces), a [subordinate flag for a family of linear isometries](#subordinate-flag-for-a-family-of-linear-isometries) consists of nested cofinal source and target subspaces $V_i,W_i$ with $f_x(V_i)\subset W_i$ for every $x$. After enlarging the target stages, compactness makes this possible for every finite source stage. It permits simultaneous finite-dimensional [Thom space](fiber-bundle.md#thom-space) constructions.

### Homotopy colimit of spectra

↑ **Parent:** [Stable homotopy theory](#stable-homotopy-theory)

A [homotopy colimit of spectra](#homotopy-colimit-of-spectra) is the derived [colimit](category.md#colimit) of a diagram of [topological spectra](#spectrum-topology). For a sequential diagram $T_0\to T_1\to\cdots$, it is the [cofiber of spectra](#cofiber-of-spectra) of $1-s:\bigvee_jT_j\to\bigvee_jT_j$, where $s$ uses the bonding maps into the next summands.

#### Milnor exact sequence for maps of spectra

↑ **Parent:** [Homotopy colimit of spectra](#homotopy-colimit-of-spectra)

For $D=\operatorname{hocolim}_jT_j$, applying $[-,E]_{\mathrm{st}}$ to the telescope [cofiber sequence of spectra](#cofiber-sequence-of-spectra) gives

$$
0\longrightarrow\lim\nolimits^1_j[\Sigma T_j,E]_{\mathrm{st}}\longrightarrow[D,E]_{\mathrm{st}}\longrightarrow\lim_j[T_j,E]_{\mathrm{st}}\longrightarrow0.
$$

Here $\lim^1$ is the cokernel of $1-r$ on the product of the inverse tower, where $r$ uses its bonding maps. This records the obstruction to uniqueness when compatible stage maps are realized.

### Cofiber of spectra

↑ **Parent:** [Stable homotopy theory](#stable-homotopy-theory)

The homotopy [cofiber of spectra](#cofiber-of-spectra) of $u:A\to B$ is the derived pushout $B\cup_A CA$. It fits into a [cofiber sequence of spectra](#cofiber-sequence-of-spectra).

#### Cofiber sequence of spectra

↑ **Parent:** [Cofiber of spectra](#cofiber-of-spectra)

A [cofiber sequence of spectra](#cofiber-sequence-of-spectra) $A\to B\to C\to\Sigma A$ induces exact sequences after either mapping into or out of a fixed [topological spectrum](#spectrum-topology), and on [stable homotopy groups](#stable-homotopy-group). In particular the second map is zero precisely when the first map admits a right inverse in the [stable homotopy category](#stable-homotopy-category).

### Smash product of spectra

↑ **Parent:** [Stable homotopy theory](#stable-homotopy-theory)

The derived [smash product of spectra](#smash-product-of-spectra) is the symmetric monoidal product on the [stable homotopy category](#stable-homotopy-category). It has unit [sphere spectrum](#sphere-spectrum), preserves [cofiber sequences of spectra](#cofiber-sequence-of-spectra) and [homotopy colimits of spectra](#homotopy-colimit-of-spectra) in each variable, and satisfies $\Sigma^\infty X\wedge\Sigma^\infty Y\simeq\Sigma^\infty(X\wedge Y)$.

#### Function spectrum

↑ **Parent:** [Smash product of spectra](#smash-product-of-spectra)

The internal [function spectrum](#function-spectrum) is characterized by $[C,F(A,E)]_{\mathrm{st}}=[C\wedge A,E]_{\mathrm{st}}$. For a [based space](#based-space) $K$, notation $F(K,E)$ abbreviates $F(\Sigma^\infty K,E)$.

##### Function spectrum with values in a ring spectrum

↑ **Parent:** [Function spectrum](#function-spectrum)

If $E$ is a [ring spectrum](#ring-spectrum), then $F(X_+,E)$ is a [ring spectrum](#ring-spectrum). Its multiplication is adjoint to evaluating the two functions on the two copies supplied by the diagonal of $X$, then multiplying in $E$. Its unit is the constant unit function. Coassociativity of the diagonal and associativity in $E$ prove the associative identity; the counit and unit identities prove both unit laws.

### Stable homotopy category

↑ **Parent:** [Stable homotopy theory](#stable-homotopy-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stable_homotopy_category)

The [stable homotopy category](#stable-homotopy-category) is obtained from [topological spectra](#spectrum-topology) by inverting [stable equivalences of spectra](#stable-equivalence-of-spectra). Its morphisms are abelian groups; for a cellular source and fibrant target they are [spectrum homotopy](#spectrum-homotopy) classes of point-set [maps of topological spectra](#map-of-topological-spectra).

#### Stable equivalence of spectra

↑ **Parent:** [Stable homotopy category](#stable-homotopy-category)

A [map of topological spectra](#map-of-topological-spectra) inducing isomorphisms on every [stable homotopy group](#stable-homotopy-group) is a [stable equivalence of spectra](#stable-equivalence-of-spectra).

### Spectrum (topology)

↑ **Parent:** [Stable homotopy theory](#stable-homotopy-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spectrum_(topology))

A sequential model of a [topological spectrum](#spectrum-topology) consists of [based spaces](#based-space) $E_j$ and structure maps $S^1\wedge E_j\to E_{j+1}$. Indexed models use finite-dimensional subspaces of a [universe for spectra](#universe-for-spectra) and structure maps $S^{W\ominus V}\wedge E(V)\to E(W)$. Different standard models present the same [stable homotopy category](#stable-homotopy-category).

#### Connective spectrum

↑ **Parent:** [Spectrum (topology)](#spectrum-topology)

A [connective spectrum](#connective-spectrum) has $\pi_qE=0$ for $q<0$. This makes the homological [Atiyah-Hirzebruch spectral sequence](cohomology.md#atiyah-hirzebruch-spectral-sequence) first quadrant for a [based space](#based-space), and prevents negative coefficient degrees from affecting its first nonzero [represented homology theory](homology.md#represented-homology-theory).

##### Bottom-degree generalized Hurewicz isomorphism

↑ **Parent:** [Connective spectrum](#connective-spectrum)

If $E$ is [connective spectrum](#connective-spectrum) in the sense of a [connective spectrum](#connective-spectrum), $\pi_0E\cong\mathbb Z$, and $X$ is $(n-1)$-connected with $n\ge2$, then $\widetilde E_n(X)\cong\pi_n(X)$. In the [homological Atiyah-Hirzebruch spectral sequence](cohomology.md#homological-atiyah-hirzebruch-spectral-sequence), the only nonzero term in total degree $n$ is $\widetilde H_n(X;\pi_0E)$. Incoming differentials have negative coefficient degree, and outgoing differentials have spatial degree below $n$. The [Hurewicz theorem](#hurewicz-theorem) identifies this term with $\pi_nX$.

###### Connective generalized homology detects simply connected equivalences

↑ **Parent:** [Bottom-degree generalized Hurewicz isomorphism](#bottom-degree-generalized-hurewicz-isomorphism)

For a [connective spectrum](#connective-spectrum) with $\pi_0E\cong\mathbb Z$, an $E$-homology isomorphism of [simply connected spaces](#simply-connected-space) is a [weak homotopy equivalence](#weak-homotopy-equivalence). Its simply connected homotopy [mapping cone](homology.md#mapping-cone-homological-algebra) is $E$-acyclic. If it had a first nonzero integral [homology](homology.md) group, the [Hurewicz theorem](#hurewicz-theorem) and the [bottom-degree generalized Hurewicz isomorphism](#bottom-degree-generalized-hurewicz-isomorphism) would produce a nonzero $E$-homology group. Thus the cone is integrally acyclic and the [homological Whitehead theorem](#homological-whitehead-theorem) applies.

#### Ring spectrum

↑ **Parent:** [Spectrum (topology)](#spectrum-topology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ring_spectrum)

A [ring spectrum](#ring-spectrum) is a unital associative monoid object of the [stable homotopy category](#stable-homotopy-category) under the [smash product of spectra](#smash-product-of-spectra). It has $\mu:E\wedge E\to E$ and $\eta:\mathbb S\to E$, satisfying the associative and two unit identities. Structured ring spectra additionally specify coherent point-set or higher homotopies; a ring object alone does not assert those enhancements.

##### Commutative ring spectrum

↑ **Parent:** [Ring spectrum](#ring-spectrum)

A [commutative ring spectrum](#commutative-ring-spectrum), in the homotopy-category convention, satisfies $\mu\tau=\mu$, where $\tau$ interchanges the factors of the [smash product of spectra](#smash-product-of-spectra). This condition alone does not assert an $E_\infty$ refinement.

#### Indexed prespectrum

↑ **Parent:** [Spectrum (topology)](#spectrum-topology)

An [indexed prespectrum](#indexed-prespectrum) over $U$ consists of [based spaces](#based-space) $E(V)$ indexed by finite-dimensional $V\subset U$, with unital associative maps $S^{W\ominus V}\wedge E(V)\to E(W)$ for inclusions $V\subset W$. The orthogonal differences make iterated suspension coordinates compose consistently.

##### Twisted half-smash product

↑ **Parent:** [Indexed prespectrum](#indexed-prespectrum)

For compact $X$ over the space of [linear isometries](hilbert-space.md#linear-isometry-of-hilbert-spaces) $U\to U\prime$, choose a [subordinate flag for a family of linear isometries](#subordinate-flag-for-a-family-of-linear-isometries) $V_i,W_i$. The [vector bundle](fiber-bundle.md#vector-bundle) $\xi_i$ has fiber $W_i\ominus f_x(V_i)$. Form $P(W_i)=\operatorname{Th}(\xi_i)\wedge E(V_i)$. Its structure maps use the orthogonal decomposition

$$
(W_j\ominus W_i)\oplus\xi_i\cong\xi_j\oplus f_x(V_j\ominus V_i)
$$

and the structure map of $E$. The [twisted half-smash product](#twisted-half-smash-product) is the [spectrification](#spectrification) $LP$, after extending from the cofinal flag. Unlike an arbitrary replacement by $X_+\wedge E$, this definition retains the specified isometry family at the point-set level.

###### Associativity of twisted half-smash products

↑ **Parent:** [Twisted half-smash product](#twisted-half-smash-product)

For isometry families $f_x:U\to U\prime$ and $g_y:U\prime\to U\prime\prime$, the complement of $g_yf_x(V)$ decomposes orthogonally as the complement of $g_y(W)$ plus the image under $g_y$ of the complement of $f_x(V)$ in $W$. Their fiberwise one-point compactifications therefore give the same [Thom space](fiber-bundle.md#thom-space) as the external direct sum. The resulting stage isomorphisms respect structure maps and give $Y\ltimes_g(X\ltimes_fE)\cong(Y\times X)\ltimes_{g\circ f}E$ in the [stable homotopy category](#stable-homotopy-category).

##### Spectrification

↑ **Parent:** [Indexed prespectrum](#indexed-prespectrum)

In the genuine indexed point-set model, [spectrification](#spectrification) $L$ is the left adjoint to the forgetful functor from indexed spectra to [indexed prespectra](#indexed-prespectrum). An indexed spectrum has adjoint structure maps $E(V)\to\Omega^{W\ominus V}E(W)$ that are homeomorphisms. Applying $L$ to a cellular [indexed prespectrum](#indexed-prespectrum) supplies the associated genuine [topological spectrum](#spectrum-topology).

#### Stable homotopy group

↑ **Parent:** [Spectrum (topology)](#spectrum-topology)

The $k$th [stable homotopy group](#stable-homotopy-group) of $E$ is $\pi_kE=[\Sigma^k\mathbb S,E]_{\mathrm{st}}$, equivalently $\operatorname{colim}_j\pi_{k+j}E_j$ in a sequential model.

#### Suspension of spectra

↑ **Parent:** [Spectrum (topology)](#spectrum-topology)

[Suspension of spectra](#suspension-of-spectra) shifts the stable degree. Unlike [reduced suspension](#reduced-suspension) of [based spaces](#based-space), it is invertible in the [stable homotopy category](#stable-homotopy-category), with inverse denoted $\Sigma^{-1}$.

#### Suspension spectrum

↑ **Parent:** [Spectrum (topology)](#spectrum-topology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Suspension_spectrum)

For a [based space](#based-space) $X$, its [suspension spectrum](#suspension-spectrum) has level $j$ equal to $S^j\wedge X$. Its derived adjunction with the infinite [loop space](#loop-space) is $[\Sigma^\infty X,E]_{\mathrm{st}}=[X,\Omega^\infty E]_*$.

##### Sphere spectrum

↑ **Parent:** [Suspension spectrum](#suspension-spectrum)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sphere_spectrum)

The [sphere spectrum](#sphere-spectrum) is $\mathbb S=\Sigma^\infty S^0$. It is the unit of the [smash product of spectra](#smash-product-of-spectra). Its integer [suspensions of spectra](#suspension-of-spectra) represent [stable homotopy groups](#stable-homotopy-group).

#### Cell spectrum

↑ **Parent:** [Spectrum (topology)](#spectrum-topology)

A [cell spectrum](#cell-spectrum) is obtained by attaching stable cells, with successive [cofibers of spectra](#cofiber-of-spectra) wedges of [suspensions of spectra](#suspension-of-spectra) of the [sphere spectrum](#sphere-spectrum). Cellular models provide the cofibrant objects needed to compute derived [maps of topological spectra](#map-of-topological-spectra). Stable cells may occur in arbitrary integer degrees.

##### Finite spectrum

↑ **Parent:** [Cell spectrum](#cell-spectrum)

A [finite spectrum](#finite-spectrum) is a [topological spectrum](#spectrum-topology) equivalent to a [cell spectrum](#cell-spectrum) with finitely many cells. Such an object is compact in the [stable homotopy category](#stable-homotopy-category) and has a [Spanier-Whitehead dual](#spanier-whitehead-dual). Compactness means maps out of it commute with filtered [homotopy colimits of spectra](#homotopy-colimit-of-spectra).

###### Spanier-Whitehead dual

↑ **Parent:** [Finite spectrum](#finite-spectrum)

The [Spanier-Whitehead dual](#spanier-whitehead-dual) of a [finite spectrum](#finite-spectrum) $A$ is $A^\vee=F(A,\mathbb S)$. It is finite, and evaluation and coevaluation give the natural [Spanier-Whitehead duality](#spanier-whitehead-duality) adjunction.

###### Spanier-Whitehead duality

↑ **Parent:** [Spanier-Whitehead dual](#spanier-whitehead-dual)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spanier-Whitehead_duality)

For a [finite spectrum](#finite-spectrum) $A$, evaluation and coevaluation identify $[B,D\wedge A]_{\mathrm{st}}$ with $[B\wedge A^\vee,D]_{\mathrm{st}}$. Cellular induction constructs the dual from the duals of stable cells and verifies these identities across [cofiber sequences of spectra](#cofiber-sequence-of-spectra). In particular $\pi_k(D\wedge A)=[\Sigma^kA^\vee,D]_{\mathrm{st}}$.

#### Omega-spectrum

↑ **Parent:** [Spectrum (topology)](#spectrum-topology)

An [Omega-spectrum](#omega-spectrum) has structure adjoints $E_j\to\Omega E_{j+1}$ that are [weak homotopy equivalences](#weak-homotopy-equivalence). For such a model the level spaces represent the degrees of its [represented cohomology theory](cohomology.md#represented-cohomology-theory).

#### Map of topological spectra

↑ **Parent:** [Spectrum (topology)](#spectrum-topology)

A [map of topological spectra](#map-of-topological-spectra) is a compatible family of based maps of the level spaces: $u_{j+1}\sigma_j^D=\sigma_j^E(1\wedge u_j)$. It is distinct from its class in the [stable homotopy category](#stable-homotopy-category).

##### Phantom map of spectra

↑ **Parent:** [Map of topological spectra](#map-of-topological-spectra)

A [phantom map of spectra](#phantom-map-of-spectra) is a stable map $p:D\to E$ with $pu=0$ for every map $u:F\to D$ from a [finite spectrum](#finite-spectrum). Such a map can be nonzero even though it induces zero on all [represented homology theories](homology.md#represented-homology-theory) on [based spaces](#based-space).

###### Phantom maps vanish on represented homology

↑ **Parent:** [Phantom map of spectra](#phantom-map-of-spectra)

For a [phantom map of spectra](#phantom-map-of-spectra) $p:D\to E$ and a finite [CW complex](#cw-complex) $K$, [Spanier-Whitehead duality](#spanier-whitehead-duality) identifies $D_k(K)$ with maps from the finite spectrum $\Sigma^k(\Sigma^\infty K)^\vee$. Hence $p_*=0$ there. An arbitrary [CW complex](#cw-complex) is the filtered union of its finite subcomplexes, and [represented homology theory](homology.md#represented-homology-theory) commutes with that filtered union because spheres are compact. Thus $p$ induces zero on the entire [represented homology theory](homology.md#represented-homology-theory).

###### Universal evaluation phantom map

↑ **Parent:** [Phantom map of spectra](#phantom-map-of-spectra)

Choose one representative of each [finite spectrum](#finite-spectrum) and form $X=\bigvee_{(F,u:F\to D)}F$. Let $e:X\to D$ evaluate each summand and let $p:D\to\operatorname{cofib}(e)$. Every map from a [finite spectrum](#finite-spectrum) factors through its corresponding summand, so $p$ is a [phantom map of spectra](#phantom-map-of-spectra). If $p=0$, exactness supplies a section of $e$, making $D$ a [retract](#retract) of $X$. Consequently a spectrum that is not a retract of any wedge of finite spectra has a nonzero such phantom.

###### Hyperphantom map of spectra

↑ **Parent:** [Phantom map of spectra](#phantom-map-of-spectra)

A [hyperphantom map of spectra](#hyperphantom-map-of-spectra) is a stable map $p:D\to E$ such that $pu=0$ for every $u:\Sigma^{-j}\Sigma^\infty X\to D$, for arbitrary [based spaces](#based-space) $X$ and all nonnegative $j$. Equivalently it induces zero on the entire [represented cohomology theory](cohomology.md#represented-cohomology-theory). This is a stronger condition than being a [phantom map of spectra](#phantom-map-of-spectra), which tests only [finite spectra](#finite-spectrum).

##### Spectrum homotopy

↑ **Parent:** [Map of topological spectra](#map-of-topological-spectra)

A [spectrum homotopy](#spectrum-homotopy) between compatible maps $D\to E$ is a map from the cylinder spectrum $D\wedge[0,1]_+$ restricting to them at the endpoints. Thus the homotopies at all levels must themselves respect the structure maps.

## Based space

↑ **Parent:** [Algebraic topology](algebraic-topology.md)

A [topological space](topology.md#topological-space) with a distinguished basepoint. Maps preserve the basepoint, and [based homotopies](#based-homotopy) keep it fixed.

<h2 id="lusternik-schnirelmann-category">Lusternik–Schnirelmann category</h2>

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lusternik–Schnirelmann_category)

Use the unnormalized convention: the least number of open subsets covering $X$ whose inclusions into $X$ are [null-homotopic](#null-homotopic-map). The subsets need not themselves be contractible. This number is one for a nonempty contractible space. If $r$ positive-degree classes have nonzero product, a cover by $r$ categorical sets would make that product zero by relative [cup products](cohomology.md#cup-product); hence $\operatorname{cat}(X)\geq r+1$.

<h3 id="lusternik-schnirelmann-critical-point-theorem">Lusternik–Schnirelmann critical point theorem</h3>

↑ **Parent:** [Lusternik–Schnirelmann category](#lusternik-schnirelmann-category)

Every smooth real-valued function on a closed connected [smooth manifold](differential-geometry.md#smooth-manifold) has at least its unnormalized [Lusternik–Schnirelmann category](#lusternik-schnirelmann-category) many distinct [critical points](analysis.md#critical-point). No nondegeneracy hypothesis is required. If there are infinitely many critical points the bound is immediate; in the finite case, the sublevel-set deformation argument shows that category can increase only at critical levels, by at most the number of critical points on that level. In conjunction with [cup length](cohomology.md#cup-length), this gives at least $r+1$ critical points whenever there is a nonzero $r$-fold positive-degree [cup product](cohomology.md#cup-product). This theorem is distinct from the antipodal covering theorem also sometimes named the Lusternik–Schnirelmann theorem. A primary account of the critical-point formulation is [Conley pairs in geometry—Lusternik–Schnirelmann theory and more](https://doi.org/10.1016/j.exmath.2017.10.003).

## Theta graph

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Theta_graph)

The theta graph $\Theta_n$ has two vertices joined by $n$ edges. It has first Betti number $n-1$ and occurs as the link of a point on the spine of a book with $n$ two-dimensional pages.

## Dumbbell graph

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dumbbell_graph)

A dumbbell graph consists of two cycles joined by a path. Its connecting path contains bridges, unlike a [Theta graph](#theta-graph), although both the two-loop dumbbell and $\Theta_3$ have first homology $\mathbb Z^2$.

## Borsuk-Ulam theorem

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Borsuk-Ulam_theorem)

Every continuous map $f:S^n\to\mathbb R^n$ takes the same value at some antipodal pair. Equivalently, every continuous antipodal map $S^n\to\mathbb R^n$ has a zero, and there is no antipodal map $S^n\to S^{n-1}$.

<h3 id="lusternik-schnirelmann-theorem">Lusternik–Schnirelmann theorem</h3>

↑ **Parent:** [Borsuk-Ulam theorem](#borsuk-ulam-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lusternik–Schnirelmann_theorem)

A cover of $S^d$ by $d+1$ [closed sets](topology.md#closed-set) has a member containing an [antipodal pair](geometry-and-topology.md#antipodal-pair). The equivalent version for [open sets](topology.md#open-set) follows by shrinking finite [open covers](topology.md#open-cover) on a [compact metric space](topological-analysis.md#compact-metric-space); the reverse implication follows by enlarging antipodal-pair-free [closed sets](topology.md#closed-set) slightly. This is a covering formulation of the [Borsuk-Ulam theorem](#borsuk-ulam-theorem).

#### Antipodal-free closed cover from simplex Voronoi cells

↑ **Parent:** [Lusternik–Schnirelmann theorem](#lusternik-schnirelmann-theorem)

Let $v_0,\ldots,v_{n+1}$ be the vertices of a regular simplex centered at zero in $\mathbb R^{n+1}$. The displayed spherical Voronoi cells are a [closed cover](topology.md#closed-cover) by $n+2$ sets. If $x$ and $-x$ belonged to the same cell, all their scalar products with the vertices would coincide. Their sum is zero and the vertices span the ambient [vector space](vector-space.md), so this would force $x=0$, a contradiction. Thus each cell contains no [antipodal pair](geometry-and-topology.md#antipodal-pair). Together with the [Lusternik-Schnirelmann-Borsuk theorem](#lusternik-schnirelmann-theorem), this shows $n+2$ is the minimum number of antipodal-free members of a finite [closed cover](topology.md#closed-cover).

#### Open-cover proof of the Lusternik-Schnirelmann-Borsuk theorem

↑ **Parent:** [Lusternik–Schnirelmann theorem](#lusternik-schnirelmann-theorem)

For a finite [open cover](topology.md#open-cover) $U_0,\ldots,U_d$ of $S^d$, take continuous nonnegative functions $\phi_i$ summing to one and positive only in $U_i$. Such a [partition of unity](differential-geometry.md#partition-of-unity) comes from normalizing the [distance to a set](topological-analysis.md#distance-to-a-set) functions $d(x,S^d\setminus U_i)$. The [Borsuk-Ulam theorem](#borsuk-ulam-theorem) applied to $(\phi_1,\ldots,\phi_d)$ gives equal values at an [antipodal pair](geometry-and-topology.md#antipodal-pair). The sum condition makes $\phi_0$ equal too, and some common positive value places both points in one $U_i$.

## CW complex

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/CW_complex)

A CW complex is built inductively by attaching discs along maps from their boundary spheres. Its $n$-skeleton contains all cells of dimension at most $n$.

### Compact subsets of CW complexes lie in finite subcomplexes

↑ **Parent:** [CW complex](#cw-complex)

A [compact subset](topology.md#compact-space) of a [CW complex](#cw-complex) is contained in a [finite CW complex](#finite-cw-complex) that is a subcomplex of the original complex. Otherwise choose one point in each of infinitely many cells met by the subset. The closure-finiteness axiom makes each closed cell meet the chosen set in finitely many points. The weak topology axiom then makes the chosen set, and each of its subsets, closed. It is consequently an infinite closed discrete subspace of the compact subset, a contradiction. Only finitely many cells are met; their closures form a finite subcomplex containing the subset.

### Skeleton of a CW complex

↑ **Parent:** [CW complex](#cw-complex)

The $q$-skeleton of a [CW complex](#cw-complex) is the [subcomplex](#simplicial-subcomplex) consisting of its [topological cells](#topological-cell) of dimension at most $q$. A [cellular map](#cellular-map) preserves these skeleta. The [cellular approximation theorem](#cellular-approximation-theorem) lets continuous maps respect this filtration up to [homotopy](#homotopy).

### Topological cell

↑ **Parent:** [CW complex](#cw-complex)

An open $q$-cell of a [CW complex](#cw-complex) is a copy of an open $q$-dimensional ball. Its characteristic map is a map from a closed ball whose interior parametrizes that cell and whose boundary lands in the preceding skeleton. The characteristic map need not be injective on the boundary. Each oriented cell gives one generator of the [cellular chain complex](homology.md#cellular-chain-complex).

### CW pair

↑ **Parent:** [CW complex](#cw-complex)

A CW pair consists of a [CW complex](#cw-complex) $X$ and a subcomplex $A$. Its inclusion is a [cofibration](#cofibration), so homotopies on $A$ extend across $X$. The relative lifting property of a [Serre fibration](#serre-fibration) for such pairs allows specified boundary lifts to be retained while lifting a homotopy.

### Cell attachment

↑ **Parent:** [CW complex](#cw-complex)

Attaching a $q$-cell along $\phi:S^{q-1}\to X$ forms the quotient of $X\sqcup D^q$ identifying each boundary point with its image under $\phi$. A constant attaching map gives $X\vee S^q$. An attaching map can affect the [cohomology ring](cohomology.md#cohomology-ring) even when it does not change the additive cohomology groups.

#### Homotopy-group effect of attaching higher cells

↑ **Parent:** [Cell attachment](#cell-attachment)

Attaching cells of dimension $i+1$ to a connected [CW complex](#cw-complex), for $i\geq2$, preserves all [homotopy groups](#homotopy-group) below degree $i$. In degree $i$ it takes the quotient by the subgroup generated by the attaching maps and their translates under the [fundamental group](#fundamental-group) action. This follows from the relative [homotopy](#homotopy) sequence and the generation of the first nonzero relative group by the new cells. In particular, a single attaching map representing a generator of $\pi_i\cong\mathbb Z$ kills that group even when the [fundamental group](#fundamental-group) is nontrivial. Higher attachments can create higher [homotopy groups](#homotopy-group), which may then be killed at later stages.

### Weak topology of a CW complex

↑ **Parent:** [CW complex](#cw-complex)

The weak topology of a [CW complex](#cw-complex) is determined by its closed cells: a subset is closed if and only if its inverse image under every characteristic map from a closed cell is closed. A map out of the complex is continuous when its restrictions along those characteristic maps are continuous. This is distinct from the [weak topology](weak-topology.md) of a vector space. Taking the product with a locally finite [CW complex](#cw-complex), such as a closed interval with its finite cell structure, retains the corresponding CW weak topology.

### Graph (topology)

↑ **Parent:** [CW complex](#cw-complex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_(topology))

A topological graph is a [CW complex](#cw-complex) with only zero-cells and one-cells, called vertices and edges. Edge endpoints attach to vertices; loops, multiple edges and infinitely many edges are allowed. A [subgraph](graph-theory.md#subgraph) in this setting is a [CW subcomplex](#cw-subcomplex). A connected acyclic graph is a [tree](combinatorics.md#tree-graph-theory) and is a [contractible space](#contractible-space).

### CW subcomplex

↑ **Parent:** [CW complex](#cw-complex)

A [CW subcomplex](#cw-subcomplex) is a union of cells of a [CW complex](#cw-complex) containing the attaching boundary of every included cell. In a combinatorial [2-complex](#2-complex), including a two-cell therefore includes every edge in its boundary. A connected [CW subcomplex](#cw-subcomplex) has a connected [1-skeleton](#1-skeleton), whose intrinsic path metric may differ from the ambient graph metric.

### 1-skeleton

↑ **Parent:** [CW complex](#cw-complex)

The one-skeleton $X^{(1)}$ of a [CW complex](#cw-complex) is the union of its zero-cells and one-cells. It is a graph. The unit-edge path metric measures the infimum of lengths of paths in this graph; it is different from metrics that allow paths through two-cell interiors.

### 2-complex

↑ **Parent:** [CW complex](#cw-complex)

A two-dimensional [CW complex](#cw-complex) has cells only in dimensions zero, one and two. In a combinatorial two-complex the two-cells are polygons attached by combinatorial edge paths. Its [1-skeleton](#1-skeleton) carries the path metric assigning length one to each edge. Compact combinatorial complexes have finitely many cells, so their cell-boundary lengths have a finite maximum.

#### Disc diagram

↑ **Parent:** [2-complex](#2-complex)

A [disc diagram](#disc-diagram) over a combinatorial [2-complex](#2-complex) is a finite contractible planar combinatorial complex together with a combinatorial map to that complex. Its exterior boundary circuit records a [null-homotopic](#null-homotopic-map) path. Tree portions and cut vertices are allowed; the diagram need not be an embedded disk or map injectively. Its area is its number of two-cells.

##### Disc diagram ladder

↑ **Parent:** [Disc diagram](#disc-diagram)

A ladder is a [disc diagram](#disc-diagram) whose blocks form a linear chain, each block a two-cell or a connecting edge, with cells attached successively along interior arcs. Its boundary consists of two opposite side paths between its ends. Every cell meets both side paths. If cell perimeters are bounded by $L$, each point of one side is within $L/2$ of the other by traveling around a cell boundary; connecting edge paths coincide on the two sides.

##### Disc diagram spur

↑ **Parent:** [Disc diagram](#disc-diagram)

A spur is an exposed degree-one vertex and its incident edge in a [disc diagram](#disc-diagram). The exterior boundary runs out along that edge and immediately back. Thus a spur in the interior of a boundary side contradicts that side being a reduced combinatorial path or a [metric geodesic](topological-analysis.md#metric-geodesic). A diagram with no two-cells may be a tree and have spurs rather than shells.

##### Disc diagram shell

↑ **Parent:** [Disc diagram](#disc-diagram)

A shell is an exposed two-cell in a [disc diagram](#disc-diagram), with perimeter split as an exterior boundary arc $Q$ and an interior path $P$. An $i$-shell has $P$ consisting of $i$ interior pieces. Under $C'(1/6)$, an $i$-shell with $i\leq3$ has $|P|<|\partial R|/2<|Q|$, so removal replaces a long exterior path by a strictly shorter path.

##### van Kampen lemma

↑ **Parent:** [Disc diagram](#disc-diagram)

A closed combinatorial path in a [2-complex](#2-complex) is [null-homotopic](#null-homotopic-map) exactly when it is the boundary path of a [disc diagram](#disc-diagram) over that complex. A finite cellular null-homotopy can be arranged into such a planar diagram; conversely the contractible diagram supplies a null-homotopy. In a [group presentation](geometric-group-theory.md#group-presentation), this is the geometric form of expressing a trivial word as a product of conjugates of [relators](geometric-group-theory.md#relator).

##### Reduced disc diagram

↑ **Parent:** [Disc diagram](#disc-diagram)

A [disc diagram](#disc-diagram) is reduced if it has no adjacent pair of two-cells that can be folded together across their common boundary and removed while preserving the outside boundary. A minimum-area diagram is reduced. Among diagrams of minimum area, minimizing the number of edges removes unnecessary tree portions. Internal common arcs in a reduced diagram satisfy the applicable [small cancellation theory](geometric-group-theory.md#small-cancellation-theory) piece bounds.

### Cellular map

↑ **Parent:** [CW complex](#cw-complex)

A cellular map $f:X\to Y$ between [CW complexes](#cw-complex) satisfies $f(X^q)\subseteq Y^q$ for every skeleton. It induces a [chain map](homology.md#chain-map) $f_\#:C_*^{\mathrm{cell}}(X)\to C_*^{\mathrm{cell}}(Y)$.

#### Cellular approximation theorem

↑ **Parent:** [Cellular map](#cellular-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cellular_approximation_theorem)

A [continuous map](topology.md#continuous-map) between [CW complexes](#cw-complex) is homotopic to a [cellular map](#cellular-map). If the map is already cellular on a subcomplex, the homotopy can be taken relative to that subcomplex. In particular, a map from a $d$-dimensional [CW complex](#cw-complex) can be deformed into the $d$-skeleton of the target. This permits finite [cellular chain complexes](homology.md#cellular-chain-complex) to compute induced [homology](homology.md) maps, and turns maps to [Complex projective space](#complex-projective-space) into maps to an appropriate finite-dimensional projective skeleton.

##### Dimension reduction of sphere maps into CW skeleta

↑ **Parent:** [Cellular approximation theorem](#cellular-approximation-theorem)

A map from the $n$-[sphere](geometry-and-topology.md#sphere) to a [CW complex](#cw-complex) can be homotoped into its $n$-skeleton. By [compact subsets of CW complexes lie in finite subcomplexes](#compact-subsets-of-cw-complexes-lie-in-finite-subcomplexes), its image lies in a finite subcomplex. For a top-dimensional cell of dimension $d>n$, use [smooth approximation of maps into Euclidean space](differential-geometry.md#smooth-approximation-of-maps-into-euclidean-space) in its interior, with a cutoff supported away from the cell boundary. The [Sard theorem](differential-geometry.md#sard-s-theorem) supplies a point in a smaller interior ball omitted by the smoothed map; the cutoff is chosen so the transition region also avoids that point. Radial retraction from the omitted point pushes the image into the cell boundary and fixes all other cells. Repeating over the finitely many higher-dimensional cells proves the assertion, without assuming the initial continuous image has measure zero.

### Finite CW complex

↑ **Parent:** [CW complex](#cw-complex)

A finite [CW complex](#cw-complex) has finitely many cells. Its [cellular chain complex](homology.md#cellular-chain-complex) consists of finitely generated free [abelian groups](group.md#abelian-group) and vanishes outside finitely many degrees, so its [integral homology](homology.md#integral-homology) groups are finitely generated.

#### Euclidean embedding by finite cell attachment

↑ **Parent:** [Finite CW complex](#finite-cw-complex)

Suppose a [compact](topology.md#compact-space) skeleton $Y$ embeds as $e(Y)\subset\mathbb R^m$. Attach a disk by $a:S^{k-1}\to Y$ and extend its boundary coordinate map radially by $G(ru)=r e(a(u))$. Map the disk to $(G(x),(1-|x|)x,1-|x|)$ and $Y$ to $(e(y),0,0)$. The boundary identifications agree; a positive last coordinate recovers each interior point. This defines a continuous injection of the [compact](topology.md#compact-space) quotient into [Euclidean space](functional-analysis.md#euclidean-norm), hence an [embedding](geometry-and-topology.md#embedding). Repeating proves Hausdorffness and Euclidean embeddability for every finite [CW complex](#cw-complex), without assuming triangulability of arbitrary attaching maps.

### CW approximation

↑ **Parent:** [CW complex](#cw-complex)

A CW approximation of a space $X$ is a [CW complex](#cw-complex) $X_{\mathrm{cw}}$ with a [weak homotopy equivalence](#weak-homotopy-equivalence) $X_{\mathrm{cw}}\to X$. The realization of the [singular simplicial set](#singular-simplicial-set) of $X$ supplies one functorially.

#### Finite type CW approximation

↑ **Parent:** [CW approximation](#cw-approximation)

For simply connected $X$ with finitely generated integral [homology](homology.md) in every degree, the [Hurewicz theorem modulo a Serre class](#hurewicz-theorem-modulo-a-serre-class) gives finitely generated [homotopy groups](#homotopy-group). Realize finite generating sets of successive relative [homotopy groups](#homotopy-group) by attaching finitely many cells at each stage. The resulting weak equivalence has finitely many cells in each dimension.

##### Finite CW approximation from bounded homology

↑ **Parent:** [Finite type CW approximation](#finite-type-cw-approximation)

Start with a finite $n$-dimensional $n$-connected approximation. Its degree-$n$ [homology](homology.md) kernel is finite free. Realize a basis via the [Relative Hurewicz theorem](#relative-hurewicz-theorem) and attach $(n+1)$-cells; their boundary is injective, so they kill precisely that kernel without adding top [homology](homology.md). The [homological Whitehead theorem](#homological-whitehead-theorem) gives a finite weak equivalence of dimension at most $n+1$.

### CW filtration

↑ **Parent:** [CW complex](#cw-complex)

A CW filtration builds a CW complex by its skeleta

$$
\varnothing=X^{-1}\subset X^0\subset X^1\subset\cdots,
$$

where each quotient $X^n/X^{n-1}$ is a wedge of $n$-spheres, one for each $n$-cell.

### Moore space (algebraic topology)

↑ **Parent:** [CW complex](#cw-complex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moore_space_(algebraic_topology))

For an [abelian group](group.md#abelian-group) $G$ and an integer $m\geq1$, a Moore space $M(G,m)$ is a [CW complex](#cw-complex) whose reduced [homology](homology.md) is $G$ in degree $m$ and zero in every other degree.

#### Bockstein on a cyclic Moore space

↑ **Parent:** [Moore space (algebraic topology)](#moore-space-algebraic-topology)

Attach an $(i+1)$-cell to $S^i$ by a degree-$n$ map, with $i\geq1$ and $n\geq2$. The integral cellular differential is multiplication by $n$, while its modulo-$n$ reduction is zero. Lifting the degree-$i$ generator modulo $n^2$ and applying the differential gives $n$, so the [Bockstein homomorphism](homology.md#bockstein-homomorphism) sends that generator to the degree-$(i+1)$ generator. This supplies a nonzero example in every positive degree.

#### Cyclic Moore space in dimension one

↑ **Parent:** [Moore space (algebraic topology)](#moore-space-algebraic-topology)

Attaching a two-cell to $S^1$ by a map of degree $n$ gives the Moore space $M(\mathbb Z/n,1)$. Its positive-dimensional [cellular chain complex](homology.md#cellular-chain-complex) is

$$
0\longrightarrow\mathbb Z\xrightarrow{\ n\ }\mathbb Z\longrightarrow0,
$$

so $H_1\cong\mathbb Z/n$ and all its other reduced integral homology groups vanish.

## Mapping cylinder

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mapping_cylinder)

The mapping cylinder of $f:A\to X$ is

$$
M_f=(A\times[0,1]\sqcup X)/((a,0)\sim f(a)).
$$

It deformation retracts onto the copy of $X$.

### Mapping cone (topology)

↑ **Parent:** [Mapping cylinder](#mapping-cylinder)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mapping_cone_(topology))

The topological mapping cone of $f:X\to Y$ is $Y\cup_f CX$, where $CX$ is the cone on $X$ and its base is identified with $Y$ through $f$. For nonempty $X$, the cone vertex supplies a distinguished basepoint. This construction is related to, but distinct from, the [mapping cone](homology.md#mapping-cone-homological-algebra) of a [chain map](homology.md#chain-map).

#### Puppe sequence

↑ **Parent:** [Mapping cone (topology)](#mapping-cone-topology)

Successive mapping cones of a based map give this sequence up to [homotopy](#homotopy). Applying based maps into a space gives an exact sequence of [pointed sets](set.md#pointed-set) in the opposite direction. The exactness statement at $[X,Y]$ says that a map whose restriction to $A$ is [null-homotopic](#null-homotopic-map) extends over $C_i$ using the chosen null-homotopy.

#### Cellular chain complex of a mapping cone

↑ **Parent:** [Mapping cone (topology)](#mapping-cone-topology)

For a [cellular map](#cellular-map) between nonempty [CW complexes](#cw-complex), the reduced [cellular chain complex](homology.md#cellular-chain-complex) of its [topological mapping cone](#mapping-cone-topology) has differential

$$
D(y,x)=(d_Yy+f_\#x,-d_Xx).
$$

Here $C_{-1}(X)=0$ and the degree-zero group identifies a vertex $y$ with the reduced chain $y-v$, where $v$ is the cone vertex. Thus this is the [mapping cone](homology.md#mapping-cone-homological-algebra) of $f_\#$, in the displayed ordering of the summands.

#### Mapping cone exact sequence

↑ **Parent:** [Mapping cone (topology)](#mapping-cone-topology)

For nonempty $X$, the [topological mapping cone](#mapping-cone-topology) has this [long exact sequence in homology](homology.md#long-exact-sequence-in-homology), with ordinary [homology](homology.md) for $X,Y$ and [reduced homology](homology.md#reduced-homology) for $C_f$. In degree zero, the augmentation of $X$ is accounted for by the cone vertex. The sequence follows from the [Mayer–Vietoris theorem](#mayer-vietoris-sequence) applied to neighborhoods of the cone and $Y$.

### Mapping telescope

↑ **Parent:** [Mapping cylinder](#mapping-cylinder)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mapping_telescope)

The mapping telescope of $X_0\xrightarrow{f_0}X_1\xrightarrow{f_1}\cdots$ glues the mapping cylinders of the $f_i$ end to end. Its homology is naturally the [direct limit](module-theory.md#direct-limit-of-abelian-groups) $\varinjlim_iH_*(X_i)$.

#### Mapping-telescope realization of the rational group with square-free denominators

↑ **Parent:** [Mapping telescope](#mapping-telescope)

List the primes as $p_0,p_1,\ldots$ and form the [mapping telescope](#mapping-telescope) of degree-$p_i$ maps $S^n\to S^n$. Its reduced homology vanishes outside degree $n$, while

$$
\widetilde H_n(T;\mathbb Z)\cong\varinjlim(\mathbb Z\xrightarrow{p_0}\mathbb Z\xrightarrow{p_1}\cdots)\cong\mathbb Q_{\mathrm{sq}}.
$$

## Smash product

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Smash_product)

For based spaces, the smash product is

$$
X\wedge Y=(X\times Y)/(X\vee Y),
$$

where the wedge $X\vee Y$ consists of pairs having at least one basepoint coordinate.

### Smash product of CW pairs

↑ **Parent:** [Smash product](#smash-product)

The quotient of the displayed [CW pair](#cw-pair) is $(X/A)\wedge(Y/B)$. In a multiplicative [generalized cohomology theory](cohomology.md#generalized-cohomology-theory), external products of relative classes of degrees $k,m$ take values in degree $k+m$ of this pair. Pullback along a diagonal produces the [relative cup product](cohomology.md#relative-cup-product).

## Real projective space

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Real_projective_space)

Real projective space is the antipodal quotient $\mathbb{RP}^n=S^n/(x\sim-x)$.

### Orientability of real projective space

↑ **Parent:** [Real projective space](#real-projective-space)

The outward-normal-first [volume form](differential-form.md#volume-form) on the unit sphere pulls back under the [antipodal map](homology.md#antipodal-map) by $(-1)^{n+1}$. For $n\ge1$, the sphere is connected, and its orientation descends to the twofold quotient exactly when this [deck transformation](#deck-transformation) preserves it. Thus [Real projective space](#real-projective-space) is orientable precisely in odd positive dimensions; the zero-dimensional case is one point and is also orientable.

### Real projective 3-space

↑ **Parent:** [Real projective space](#real-projective-space)

The quotient of the three-sphere by its antipodal map is a closed oriented three-manifold. Equivalently it is the lens space obtained by integer surgery of coefficient two on the [unknot](knot-theory.md#unknot). Its [fundamental group](#fundamental-group) is cyclic of order two, from the [sphere](geometry-and-topology.md#sphere) double covering. This makes it a basic example for [Jones polynomial surgery invariants](knot-theory.md#jones-polynomial-surgery-invariant).

// Target: knot-theory.bigb

### Nonsurjective self-map of real projective space is null-homotopic

↑ **Parent:** [Real projective space](#real-projective-space)

For $n\ge2$, a nonsurjective self-map of [Real projective space](#real-projective-space) $\mathbb{RP}^n$ has zero [mod-two degree of a map between closed manifolds](homology.md#mod-two-degree-of-a-map-between-closed-manifolds). In the [mod-two cohomology ring of real projective space](#mod-two-cohomology-ring-of-real-projective-space), the nonzero degree-one class $a$ has $a^n\ne0$. If pullback fixed $a$, it would fix $a^n$, contradicting zero degree. Thus the map is trivial on the [fundamental group](#fundamental-group) and lifts to $S^n$. A point missed by the original map has both its inverse images missed by the lift. The lift therefore takes values in a punctured sphere, which is contractible, and is null-homotopic. Composing its contraction with the covering projection proves the conclusion.

### Fixed-point-free complex-structure map on odd-dimensional real projective space

↑ **Parent:** [Real projective space](#real-projective-space)

Choose a [complex structure](complex-geometry.md#complex-structure) $J$ on $\mathbb R^{2m}$, with $J^2=-I$. Its induced map on $\mathbb RP^{2m-1}$ has no fixed point: $Jx=\lambda x$ for a real nonzero vector would give $\lambda^2=-1$. The maps $\cos t\,I+\sin t\,J$, for $0\leq t\leq\pi/2$, give a [homotopy](#homotopy) from the identity to $J$, because they are invertible throughout. Thus this fixed-point-free map is homotopic to the identity.

### Integral homology of a circle times a real projective plane

↑ **Parent:** [Real projective space](#real-projective-space)

Cover the circle by two arcs whose intersection has two components and take the product with the projective plane. The [Mayer–Vietoris sequence](#mayer-vietoris-sequence) has maps $(a,b)\mapsto(a+b,-a-b)$ on the two copies of the homology of the plane. Its kernels and cokernels, together with $H_1(\mathbb{RP}^2;\mathbb Z)=\mathbb Z/2$, give the displayed groups; all higher groups vanish. The product is a closed nonorientable three-manifold, but is homotopy equivalent to a noncompact oriented four-manifold.

### Infinite-dimensional real projective space

↑ **Parent:** [Real projective space](#real-projective-space)

This is the [CW complex](#cw-complex) obtained as the increasing union of finite [Real projective spaces](#real-projective-space) under their standard inclusions. It has one cell in each nonnegative dimension. Its [cellular chain complex](homology.md#cellular-chain-complex) has boundary multiplication by two in positive even dimensions and zero in odd dimensions. Consequently its integral [cohomology](cohomology.md) is $\mathbb Z$ in degree zero, $\mathbb Z/2$ in positive even degrees and zero in odd degrees. Its mod-two [cohomology](cohomology.md) is $\mathbb Z_2$ in every nonnegative degree.

### Stunted real projective space

↑ **Parent:** [Real projective space](#real-projective-space)

Collapse the indicated standard skeleton to a point. Besides its basepoint, the quotient has one cell in dimensions $k+1$ through $m$. Its integral cellular boundary is two in even dimensions and zero in odd dimensions. Steenrod operations on its relative [cohomology](cohomology.md) are inherited from real projective space.

#### Homotopy groups of the stunted projective space through degree nine

↑ **Parent:** [Stunted real projective space](#stunted-real-projective-space)

For this quotient, homotopy groups through degree six and in degree eight vanish. The degree-seven and degree-nine groups are $\mathbb Z/2$. A map to $K(\mathbb Z/2,7)$ induces an isomorphism on degree-nine integral [homology](homology.md) because the relevant square of the bottom mod-two class is nonzero. Two relative Hurewicz steps then compute degrees eight and nine.

### Steenrod squares on real projective space

↑ **Parent:** [Real projective space](#real-projective-space)

For the degree-one mod-two generator, $\operatorname{Sq}^1x=x^2$ and higher squares of $x$ vanish by instability. The Cartan formula gives the displayed binomial identity. Naturality applies it to relative classes of a [stunted real projective space](#stunted-real-projective-space).

### Standard affine atlas of real projective space

↑ **Parent:** [Real projective space](#real-projective-space)

The $n+1$ [manifold charts](differential-geometry.md#manifold-chart) $U_i=\{[X]:X_i\ne0\}$ have coordinates $X_k/X_i$, with $k\ne i$. Their inverse inserts $1$ as the $i$th homogeneous coordinate. On an overlap, changing the denominator from $X_i$ to $X_j$ divides each remaining coordinate by the nonzero coordinate $X_j/X_i$. These rational [smooth transition maps](differential-geometry.md#smooth-transition-map) give [Real projective space](#real-projective-space) its standard [smooth manifold](differential-geometry.md#smooth-manifold) structure.

### Integral cohomology ring of real projective space

↑ **Parent:** [Real projective space](#real-projective-space)

For $m\geq0$, the [cohomology ring](cohomology.md#cohomology-ring) is

$$
H^*(\mathbb{RP}^{2m};\mathbb Z)\cong\mathbb Z[a]/(2a,a^{m+1}),\qquad |a|=2,
$$

and

$$
H^*(\mathbb{RP}^{2m+1};\mathbb Z)\cong\mathbb Z[a,b]/(2a,a^{m+1},ab,b^2),\qquad |a|=2,\quad |b|=2m+1.
$$

The generator $a$ reduces to the square of the degree-one generator in the [mod-two cohomology ring of real projective space](#mod-two-cohomology-ring-of-real-projective-space); $b$ is the integral [orientation class](cohomology.md#fundamental-class) in odd top dimension.

#### Integral cohomology of a product of finite real projective spaces

↑ **Parent:** [Integral cohomology ring of real projective space](#integral-cohomology-ring-of-real-projective-space)

The [cellular cochain complex](homology.md#cellular-cochain-complex) of finite [Real projective space](#real-projective-space) consists of alternating maps zero and two. Its groups can be tensored using the [Künneth theorem](cohomology.md#kunneth-theorem); the [integral Künneth torsion polynomial](cohomology.md#integral-kunneth-torsion-polynomial) efficiently counts all tensor and [Tor functor](algebra.md#tor-functor) summands. A product of factors of dimensions two, three and four has free-rank polynomial $1+t^3$ and torsion polynomial $3t^2+3t^3+5t^4+6t^5+5t^6+4t^7+2t^8+t^9$.

### Cellular homology of real projective space

↑ **Parent:** [Real projective space](#real-projective-space)

Real projective space has one cell in every dimension from zero through $n$. With integral coefficients its cellular differential $C_k\to C_{k-1}$ is multiplication by $1+(-1)^k$, hence is zero for odd $k$ and multiplication by two for even $k$. With coefficients in $\mathbb F_2$, every cellular differential vanishes.

### Mod-two cohomology ring of real projective space

↑ **Parent:** [Real projective space](#real-projective-space)

The mod-two cohomology ring of real projective space is

$$
H^*(\mathbb{RP}^m;\mathbb F_2)\cong\mathbb F_2[y]/(y^{m+1}),
\qquad |y|=1.
$$

#### Gysin proof of mod-two projective-space cohomology

↑ **Parent:** [Mod-two cohomology ring of real projective space](#mod-two-cohomology-ring-of-real-projective-space)

The unit sphere bundle of the tautological line is the double cover $S^n\to\mathbb{RP}^n$. In its [Gysin sequence](fiber-bundle.md#gysin-sequence-of-a-sphere-bundle), multiplication by the mod-two Euler class $a$ is an isomorphism in successive interior degrees, since the sphere has no interior cohomology. Connectedness in degree zero makes multiplication into degree one injective. At the top, vanishing above dimension $n$ makes the transfer from $H^n(S^n;\mathbb F_2)$ surjective; together with that injection it makes the top group one-dimensional. Thus every $a^j$, $0\leq j\leq n$, is the nonzero generator and the next power vanishes.

#### Mod-two degree obstruction for equal projective factors

↑ **Parent:** [Mod-two cohomology ring of real projective space](#mod-two-cohomology-ring-of-real-projective-space)

For any continuous map between the displayed [Real projective spaces](#real-projective-space), the [induced map on cohomology](cohomology.md#induced-map-on-cohomology) sends the degree-one generator to $\alpha x+\beta y$. Its $2n$th power is $\binom{2n}{n}\alpha^n\beta^n x^ny^n$, since all other terms exceed the truncation exponent of one factor. The coefficient is zero modulo two because $\binom{2n}{n}=2\binom{2n-1}{n-1}$. Naturality of the evaluation pairing then makes the top [induced map on homology](homology.md#induced-map-on-homology) zero. This obstruction does not apply to $n=0$, when both spaces are points.

### Mapping-cylinder model of punctured real projective three-space

↑ **Parent:** [Real projective space](#real-projective-space)

The complement of an open three-ball in $\mathbb{RP}^3$ is the mapping cylinder of the antipodal covering $S^2\to\mathbb{RP}^2$. It deformation retracts to $\mathbb{RP}^2$ and has boundary $S^2$.

### Integral homology of real projective three-space

↑ **Parent:** [Real projective space](#real-projective-space)

The integral homology groups are

$$
H_i(\mathbb{RP}^3;\mathbb Z)=
\begin{cases}
\mathbb Z,&i=0,3,\\
\mathbb Z/2,&i=1,\\
0,&\text{otherwise}.
\end{cases}
$$

### Double of punctured real projective three-space

↑ **Parent:** [Real projective space](#real-projective-space)

Doubling $\mathbb{RP}^3$ minus an open ball along its spherical boundary gives $\mathbb{RP}^3\mathbin\#\mathbb{RP}^3$. Its fundamental group is

$$
(\mathbb Z/2)*(\mathbb Z/2)\cong D_\infty,
$$

and its universal cover is $S^2\times\mathbb R$.

## Mapping torus

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mapping_torus)

The mapping torus of $f:F\to F$ is

$$
T_f=(F\times[0,1])/((x,1)\sim(f(x),0)).
$$

If $f$ is a [homeomorphism](topology.md#homeomorphism), the projection to the [circle](topology.md#circle) $S^1$ is a [fiber bundle](fiber-bundle.md) with fiber $F$. For a general [continuous map](topology.md#continuous-map), the [mapping torus](#mapping-torus) need not be a [fiber bundle](fiber-bundle.md), but its [homology](homology.md) still has the [Wang sequence](#wang-sequence).

### Unipotent torus-bundle group

↑ **Parent:** [Mapping torus](#mapping-torus)

The [mapping torus](#mapping-torus) of a [torus](topology.md#torus) map with this monodromy has [fundamental group](#fundamental-group) generated by $x,y,t$ with $x$ central and $tyt^{-1}=x^by$. Normal forms $x^my^nt^k$ multiply by

$$
(m,n,k)(m',n',k')=(m+m'+bkn',\ n+n',\ k+k').
$$

This proves torsion-freeness and nilpotence of class at most two. For $b\ne0$ its center is $\langle x\rangle$ and commutator subgroup $\langle x^b\rangle$; for $b=0$ it is $\mathbb Z^3$. These realize all noncyclic torsion-free nilpotent closed orientable three-manifold groups.

### Inversion mapping torus of a torus

↑ **Parent:** [Mapping torus](#mapping-torus)

This [mapping torus](#mapping-torus) fibers over the circle with fiber $T^{n-1}$ and inversion as monodromy. The [Wang sequence](#wang-sequence) computes its additive [cohomology](cohomology.md). Coordinate projections to the [Klein bottle](topology.md#klein-bottle) expose its mod-two [cup products](cohomology.md#cup-product).

#### Mod-two cohomology ring of an inversion mapping torus

↑ **Parent:** [Inversion mapping torus of a torus](#inversion-mapping-torus-of-a-torus)

The base class $t$ and coordinate classes $x_i$ all have degree one. Pullback of the [mod-two intersection pairing of the Klein bottle](topology.md#mod-two-intersection-pairing-of-the-klein-bottle) gives $x_i^2=t x_i$. The [Leray-Hirsch theorem](fiber-bundle.md#leray-hirsch-theorem) gives the basis consisting of square-free products $x_I$ and $t x_I$. Thus the additive dimensions match those of a [torus](topology.md#torus), but the degree-one squares differ for $n\geq2$.

#### Integral cohomology of an inversion mapping torus

↑ **Parent:** [Inversion mapping torus of a torus](#inversion-mapping-torus-of-a-torus)

For $r=n-1$, the [Wang sequence](#wang-sequence) gives an additive splitting

$$
H^q(M_n;\mathbb Z)\cong
\operatorname{coker}((-1)^{q-1}-1:\mathbb Z^{\binom r{q-1}}\to\mathbb Z^{\binom r{q-1}})
\oplus
\ker((-1)^q-1:\mathbb Z^{\binom rq}\to\mathbb Z^{\binom rq}).
$$

The kernel is free, so the splitting exists as groups. The map in even degree is zero; the map in odd degree is multiplication by minus two.

##### Integral cup products in the four-dimensional inversion mapping torus

↑ **Parent:** [Integral cohomology of an inversion mapping torus](#integral-cohomology-of-an-inversion-mapping-torus)

Choose the base class $a$, degree-two torsion classes $\tau_i=\widehat\beta(x_i)$, and degree-two free lifts $b_{ij}$ reducing to $x_i x_j$. A generator $\kappa$ of the top $\mathbb Z/2$ reduces to $t x_1x_2x_3$. The [mod-two cohomology ring of an inversion mapping torus](#mod-two-cohomology-ring-of-an-inversion-mapping-torus) determines products in top integral degree, since reduction there is injective. The products of distinct $b_{12},b_{13},b_{23}$ equal $\kappa$; so does $b_{ij}\tau_k$ when $i,j,k$ are all distinct. Their other degree-four products vanish. Also $a\tau_i=0$ because degree-three [integral cohomology](cohomology.md#integral-cohomology) is torsion-free.

### Fiber monodromy

↑ **Parent:** [Mapping torus](#mapping-torus)

A fiber monodromy is the return [homeomorphism](topology.md#homeomorphism) of the fiber of a bundle over $S^1$. Its [mapping torus](#mapping-torus) reconstructs the total space.

#### Homological monodromy

↑ **Parent:** [Fiber monodromy](#fiber-monodromy)

Homological monodromy is the induced automorphism of the [homology](homology.md) of a fiber. For a [fibered knot](knot-theory.md#fibered-knot), its action on the [first homology group](homology.md#first-homology) presents the [Alexander module](knot-theory.md#alexander-module-of-a-knot).

### Heisenberg nilmanifold as a torus mapping torus

↑ **Parent:** [Mapping torus](#mapping-torus)

The quotient of the [real Heisenberg group](lie-algebra.md#heisenberg-group) by the [Integer Heisenberg group](lie-algebra.md#integer-heisenberg-group) is the mapping torus of the torus automorphism

$$
f:S^1\times S^1\to S^1\times S^1,
\qquad f(z,w)=(zw,w).
$$

Its universal cover is the contractible real Heisenberg group, so its [fundamental group](#fundamental-group) is the integer Heisenberg group.

### Wang sequence

↑ **Parent:** [Mapping torus](#mapping-torus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wang_sequence)

For the mapping torus of $f:F\to F$, the Wang exact sequence contains

$$
\cdots\to H_q(F)\xrightarrow{1-f_*}H_q(F)\to H_q(T_f)\to H_{q-1}(F)\xrightarrow{1-f_*}H_{q-1}(F)\to\cdots.
$$

#### Homology of the antipodal sphere mapping torus

↑ **Parent:** [Wang sequence](#wang-sequence)

For $n\geq2$, the [Wang sequence](#wang-sequence) and the [mapping degree](homology.md#degree-of-a-continuous-mapping) $(-1)^{n+1}$ of the [antipodal map](homology.md#antipodal-map) give $H_0=H_1=\mathbb Z$. If $n$ is odd, $H_n=H_{n+1}=\mathbb Z$; if $n$ is even, $H_n=\mathbb Z/2$ and $H_{n+1}=0$. All other groups vanish. At $n=1$ the [mapping torus](#mapping-torus) is a torus with $H_1=\mathbb Z^2$. At $n=0$, the two-point swapping mapping torus is a circle. Every example is already a [closed manifold](differential-geometry.md#closed-manifold); for $n\geq1$ it is orientable exactly when $n$ is odd.

##### Cohomology ring of the antipodal two-sphere mapping torus

↑ **Parent:** [Homology of the antipodal sphere mapping torus](#homology-of-the-antipodal-sphere-mapping-torus)

The [antipodal map](homology.md#antipodal-map) on the two-sphere reverses [orientation](#orientation-of-a-simplex), so its [mapping torus](#mapping-torus) is a nonorientable closed three-manifold. The [Wang sequence](#wang-sequence) gives $H_0=H_1=\mathbb Z$, $H_2=\mathbb Z/2$ and $H_3=0$. The [universal coefficient theorem for cohomology](cohomology.md#universal-coefficient-theorem-for-cohomology) therefore gives the [cohomology ring](cohomology.md#cohomology-ring) $\mathbb Z[t,u]/(t^2,tu,u^2,2u)$ with $|t|=1$, $|u|=3$. The base-circle class satisfies $t^2=0$ by pullback; the other positive-degree products vanish for dimension reasons.

###### Mod-two cohomology ring of the antipodal two-sphere mapping torus

↑ **Parent:** [Cohomology ring of the antipodal two-sphere mapping torus](#cohomology-ring-of-the-antipodal-two-sphere-mapping-torus)

Modulo two the [antipodal map](homology.md#antipodal-map) acts trivially on fiber [cohomology](cohomology.md). The [Wang sequence](#wang-sequence) supplies a class $y$ restricting to the generator of $H^2(S^2;\mathbb F_2)$. The [Leray-Hirsch theorem](fiber-bundle.md#leray-hirsch-theorem) with classes $1,y$ gives a basis $1,t,y,ty$, so $ty\ne0$. Pullback from the circle gives $t^2=0$, while dimension gives $y^2=0$. This [cohomology ring](cohomology.md#cohomology-ring) agrees with that of $S^1\times S^2$, although the original manifold is nonorientable.

<h4 id="mapping-torus-homology-from-mayer-vietoris">Mapping-torus homology from Mayer–Vietoris</h4>

↑ **Parent:** [Wang sequence](#wang-sequence)

For a continuous self-map $f:X\to X$, the [mapping torus](#mapping-torus) has the [Wang sequence](#wang-sequence) even when $f$ is not a [homeomorphism](topology.md#homeomorphism). Cover the time circle by a seam neighborhood and an interval away from the seam. Their inverse images retract to $X$: the seam neighborhood is a [mapping cylinder](#mapping-cylinder), and the other is a product. Their intersection retracts to two copies of $X$. The [Mayer–Vietoris sequence](#mayer-vietoris-sequence) map on [homology](homology.md) is, after consistent choices of signs,

$$
(a,b)\longmapsto(a+f_*b,-a-b).
$$

Invertible changes of coordinates reduce it to the direct sum of $\operatorname{id}-f_*$ and an [isomorphism](algebra.md#isomorphism). Canceling the isomorphism summands gives the [Wang sequence](#wang-sequence). This proof does not assume a [fiber bundle](fiber-bundle.md) structure for a noninvertible $f$.

<h2 id="homology">Homology (mathematics)</h2>

↑ **Parent:** [Algebraic topology](algebraic-topology.md)

[This section is present in another page, follow this link to view it.](homology.md)

## Homotopy

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homotopy)

A homotopy between maps $f,g:Y\to X$ is a continuous map $H:Y\times[0,1]\to X$ with $H(y,0)=f(y)$ and $H(y,1)=g(y)$.

### Homotopy category

↑ **Parent:** [Homotopy](#homotopy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homotopy_category)

The homotopy category of based CW complexes has spaces as objects and based homotopy classes as morphisms. Composition is well-defined because composition with continuous maps preserves homotopies. A based homotopy equivalence becomes an isomorphism. Rational localization instead inverts rational homotopy equivalences, producing a category represented by rational spaces. More general model categories have analogous homotopy categories obtained by inverting their weak equivalences.

#### Homotopy pushout

↑ **Parent:** [Homotopy category](#homotopy-category)

For maps $A\to X$ and $A\to Y$, the double [mapping cylinder](#mapping-cylinder) $X\sqcup(A\times I)\sqcup Y$, with each endpoint attached by its given map, models the homotopy pushout. A map out of this model is a pair of maps on $X$ and $Y$ together with a [homotopy](#homotopy) between their restrictions to $A$. This is why compatible [homotopy classes](#homotopy-class) extend over a homotopy pushout. For a [CW pair](#cw-pair), the inclusion is a [cofibration](#cofibration) and the ordinary pushout gives the same homotopy type.

#### H-space

↑ **Parent:** [Homotopy category](#homotopy-category)

A based [topological space](topology.md#topological-space) with a [continuous map](topology.md#continuous-map) $m$ whose left and right restrictions at the basepoint are homotopic to the identity. Associativity and inverses up to [homotopy](#homotopy) are additional conditions, not part of the bare definition.

##### H-group

↑ **Parent:** [H-space](#h-space)

An [H-space](#h-space) whose multiplication is homotopy associative and admits a homotopy inverse. These operations give $[X,Y]_*$ a [group](group.md) structure for every based [CW complex](#cw-complex) $X$. A [loop space](#loop-space) is the basic example: concatenate paths, use reversal for inversion, and use reparametrization for homotopy associativity. A bare [H-space](#h-space) should not automatically be treated as a group object.

#### Topological half-exact functor

↑ **Parent:** [Homotopy category](#homotopy-category)

For a contravariant pointed [functor](category.md#functor) on based CW [homotopy](#homotopy) types, half-exactness on a [cofibration](#cofibration) means that $F(X/A)\to F(X)\to F(A)$ is exact at $F(X)$: the image is the inverse image of the distinguished point. This does not demand injectivity or surjectivity at the ends. Set-valued exactness and group-valued exactness must be distinguished.

<h5 id="brown-s-representability-theorem">Brown's representability theorem</h5>

↑ **Parent:** [Topological half-exact functor](#topological-half-exact-functor)

A reduced contravariant [homotopy](#homotopy) [functor](category.md#functor) on based [CW complexes](#cw-complex) satisfying the wedge-to-product axiom and the Mayer-Vietoris weak-pullback gluing axiom is represented by $[X,Y]_*$ for a [CW complex](#cw-complex) $Y$. Half-exactness alone is not the full hypothesis. A reduced [generalized cohomology theory](cohomology.md#generalized-cohomology-theory) supplies these axioms; suspension compatibility assembles its representing spaces into an [Omega-spectrum](#omega-spectrum).

### Homotopy inverse limit of a tower

↑ **Parent:** [Homotopy](#homotopy)

For a sequence of maps $X_n\to X_{n-1}$, its [homotopy inverse limit](#homotopy-inverse-limit-of-a-tower) records points $x_n$ and paths from the image of $x_n$ to $x_{n-1}$, with the usual homotopy-coherent compatibility. A fibrant replacement tower computes it by an ordinary inverse limit. For a tower whose [homotopy groups](#homotopy-group) are eventually constant in each degree, the limit has those stable groups: the Milnor inverse-limit exact sequence has zero derived-limit term. In particular $X\to\operatorname{holim}P_nX$ is a weak equivalence for the [Postnikov tower](#postnikov-tower) of a connected [CW complex](#cw-complex).

### Maps to a sphere above the dimension of a compact smooth manifold are null-homotopic

↑ **Parent:** [Homotopy](#homotopy)

Approximate a continuous sphere-valued map by smooth real coordinate functions, then normalize. A sufficiently close approximation is homotopic to the original map by normalized straight interpolation. [Sard theorem](differential-geometry.md#sard-s-theorem) implies the smooth map misses a point when its source dimension is smaller than the sphere dimension. The punctured sphere is contractible, so the map is null-homotopic, even if the source is disconnected.

// Target: geometry-and-topology.bigb

### Rational homotopy theory

↑ **Parent:** [Homotopy](#homotopy)

Study [homotopy](#homotopy) after killing torsion, especially for [simply connected](#simply-connected-space) spaces of finite type. The [rational Whitehead theorem](#rational-whitehead-theorem) detects rational [homotopy](#homotopy) equivalences by rational [homology](homology.md), while [Sullivan minimal models](#sullivan-minimal-model) encode rational [homotopy](#homotopy) generators and cohomological relations.

#### Nilpotent space

↑ **Parent:** [Rational homotopy theory](#rational-homotopy-theory)

A connected space is nilpotent when its fundamental group is nilpotent and its action on each higher homotopy group is nilpotent: the module has a finite filtration whose successive quotients have trivial group action. Simply connected spaces satisfy these conditions automatically. They are the natural setting for localization and rationalization, since fibrewise coefficient localization is compatible with the successive untwisted stages of such a filtration.

#### Rational space

↑ **Parent:** [Rational homotopy theory](#rational-homotopy-theory)

In the [simply connected](#simply-connected-space) [homotopy category](#homotopy-category), a [rational space](#rational-space) is a [simply connected](#simply-connected-space) [CW complex](#cw-complex) whose positive [homotopy groups](#homotopy-group) are [vector spaces](vector-space.md) over $\mathbb Q$. Multiplication by every nonzero integer on these groups is invertible. More generally one uses nilpotent spaces with localized [fundamental group](#fundamental-group) and higher [homotopy groups](#homotopy-group); the [simply connected](#simply-connected-space) version avoids local-coefficient twisting.

##### Rationalization of a topological space

↑ **Parent:** [Rational space](#rational-space)

For [simply connected](#simply-connected-space) $X$, [rationalization of a topological space](#rationalization-of-a-topological-space) is a map $r:X\to X_{\mathbb Q}$ to a [rational space](#rational-space) inducing $\pi_n(X_{\mathbb Q})=\pi_n(X)\otimes\mathbb Q$. It is also a [rational homology](homology.md#rational-homology) equivalence. Its universal property is the bijection $r^*:[X_{\mathbb Q},Z]\to[X,Z]$ for every [rational space](#rational-space) $Z$. A [Postnikov tower](#postnikov-tower) constructs it by replacing each fibre group with its rational [tensor product](linear-algebra.md#tensor-product) and transporting the [Postnikov invariant](#postnikov-invariant) through the resulting [cohomology](cohomology.md) isomorphism, then taking the [homotopy inverse limit](#homotopy-inverse-limit-of-a-tower).

###### Rational homotopy equivalence

↑ **Parent:** [Rationalization of a topological space](#rationalization-of-a-topological-space)

A map between [simply connected](#simply-connected-space) spaces is a [rational homotopy equivalence](#rational-homotopy-equivalence) when it induces isomorphisms $\pi_n(X)\otimes\mathbb Q\to\pi_n(Y)\otimes\mathbb Q$ in every degree. Equivalently it induces an equivalence of their rationalizations, or a [rational homology](homology.md#rational-homology) isomorphism by the [rational Whitehead theorem](#rational-whitehead-theorem). Spaces have the same [rational homotopy type](#rational-homotopy-type) when they are connected by a zigzag of such maps. This is distinct from [rational homotopy equivalence](#rational-homotopy-equivalence) of algebraic cycles.

###### Rational homotopy type

↑ **Parent:** [Rational homotopy equivalence](#rational-homotopy-equivalence)

The [rational homotopy type](#rational-homotopy-type) of a [simply connected](#simply-connected-space) space is its equivalence class under zigzags of [rational homotopy equivalences](#rational-homotopy-equivalence), or equivalently the [homotopy](#homotopy) type of its [rationalization of a topological space](#rationalization-of-a-topological-space). For the usual finite-type spaces, it is encoded contravariantly by the isomorphism class of the [Sullivan minimal model](#sullivan-minimal-model). Isomorphic [cohomology](cohomology.md) rings determine this type only when additional information, such as [formality of a topological space](#formal-space), makes the cochain algebra equivalent to the [cohomology](cohomology.md) algebra.

#### Sullivan minimal model

↑ **Parent:** [Rational homotopy theory](#rational-homotopy-theory)

A free graded-commutative rational [differential graded algebra](commutative-algebra.md#differential-graded-algebra) with decomposable differentials and a [quasi-isomorphism](homology.md#quasi-isomorphism) to the rational polynomial forms of a space. For [simply connected](#simply-connected-space) finite-type spaces, $V^i$ is dual to $\pi_i(X)\otimes\mathbb Q$. A proposed finite model must have its [cohomology](cohomology.md) and representing [quasi-isomorphism](homology.md#quasi-isomorphism) checked; matching a list of relations alone is insufficient.

##### Relative Sullivan algebra

↑ **Parent:** [Sullivan minimal model](#sullivan-minimal-model)

A relative Sullivan algebra is an inclusion $(A,d)\to(A\otimes\Lambda W,D)$ with a well-ordered homogeneous basis of $W$ such that the differential of a generator lies in the algebra on $A$ and earlier generators. It need not be minimal: a differential can have linear terms from earlier generators. Such extensions supply cofibrant replacements for commutative differential graded algebras. A relative acyclic extension of a sphere model represents its path-space fibration and computes a homotopy-fibre model after base change.

##### Sullivan fibre-model theorem

↑ **Parent:** [Sullivan minimal model](#sullivan-minimal-model)

For a map $f:E\to B$ with [simply connected](#simply-connected-space) base and the usual finite-type hypotheses, choose a relative Sullivan algebra $M(B)\to M(B)\otimes\Lambda W$ modelling the path-space fibration, with acyclic total algebra. Tensor it over $M(B)$ with a model of $E$ via $f^*$. The resulting algebra models the [homotopy fibre](#homotopy-fiber). Relative Sullivan extensions are cofibrant replacements, so this [tensor product](linear-algebra.md#tensor-product) computes the derived algebraic pushout, contravariantly corresponding to the topological [homotopy pullback](#homotopy-pullback). Linear differential pairs must be cancelled before reading [rational homotopy groups](#rational-homotopy-group) from generators.

##### Sullivan minimal-model classification

↑ **Parent:** [Sullivan minimal model](#sullivan-minimal-model)

For [simply connected](#simply-connected-space) [rational spaces](#rational-space) of finite type, isomorphic minimal Sullivan models are equivalent to the same [rational homotopy type](#rational-homotopy-type). A [quasi-isomorphism](homology.md#quasi-isomorphism) between [minimal models](#sullivan-minimal-model) is an isomorphism, so a zigzag of cochain [quasi-isomorphisms](homology.md#quasi-isomorphism) produces the same [minimal model](#sullivan-minimal-model). Existence and uniqueness come from adjoining closed generators to represent missing [cohomology](cohomology.md) and generators with prescribed decomposable differential to kill kernel classes, degree by degree.

##### Rational polynomial differential forms

↑ **Parent:** [Sullivan minimal model](#sullivan-minimal-model)

For the standard $n$-simplex use $\Omega_n=\mathbb Q[t_0,\ldots,t_n,dt_0,\ldots,dt_n]/(\sum t_i-1,\sum dt_i)$, with $|t_i|=0$, $|dt_i|=1$, and $d(t_i)=dt_i$. Compatible families of these forms on the simplices of a simplicial model of $X$ form the commutative [differential graded algebra](commutative-algebra.md#differential-graded-algebra) $A_{\mathrm{PL}}(X)$. Its [cohomology](cohomology.md) is $H^*(X;\mathbb Q)$: polynomial contraction proves the simplex Poincaré lemma, and extension across faces gives the simplicial de Rham comparison. The contravariant functor takes simplicial pushouts to pullbacks of algebras.

##### Minimal model of the fibre of the projective-space collapse map

↑ **Parent:** [Sullivan minimal model](#sullivan-minimal-model)

For a degree-one map $f:\mathbb{CP}^n\to S^{2n}$ with $n\ge2$, a [minimal model](#sullivan-minimal-model) of its [homotopy fibre](#homotopy-fiber) is $(\Lambda(x_2,a_{2n-1},z_{2n+1},b_{4n-2}),d)$ with $dx=dz=0$, $da=x^n$, $db=x^{n-1}z$. Adjoin suspended sphere generators to the projective-space model to model the path pullback, then put $z=y-xa$; the differential becomes the displayed decomposable one. The [rational homotopy groups](#rational-homotopy-group) are one-dimensional in those four generator degrees and zero otherwise. At $n=1$ the map is a [rational homotopy equivalence](#rational-homotopy-equivalence) and the minimal fibre model is $\mathbb Q$.

##### Rational model of a collapsed complex projective subspace

↑ **Parent:** [Sullivan minimal model](#sullivan-minimal-model)

The quotient $\mathbb{CP}^{5}/\mathbb{CP}^{2}$ is five-connected and has [cohomology](cohomology.md) only in degrees $0,6,8,10$, with positive products zero. Its [minimal model](#sullivan-minimal-model) therefore starts with closed $a_6,b_8,c_{10}$; no decomposable differential can occur below degree twelve. Sending these three generators to the [cohomology](cohomology.md) [basis](vector-space.md#basis) and all later generators to zero is a [chain map](homology.md#chain-map) and a [quasi-isomorphism](homology.md#quasi-isomorphism). Thus its full [minimal model](#sullivan-minimal-model) is the same as that of $S^6\vee S^8\vee S^{10}$. It starts with generators $u_{11},v_{13},w_{15},t_{15}$ satisfying $du=a^2,dv=ab,dw=ac,dt=b^2$, followed by generators killing remaining products and syzygies.

##### Minimal model of a wedge of simply connected spheres

↑ **Parent:** [Sullivan minimal model](#sullivan-minimal-model)

For a finite [wedge sum](topology.md#wedge-sum) of spheres of dimensions $n_i\ge2$, let $L=\mathbb L(e_i)$ with $|e_i|=n_i-1$ and zero differential. Its [Chevalley–Eilenberg cochains of a graded Lie algebra](lie-algebra.md#chevalley-eilenberg-cochains-of-a-graded-lie-algebra) are a minimal commutative [differential graded algebra](commutative-algebra.md#differential-graded-algebra): one generator dual to each Lie [basis](vector-space.md#basis) word has degree one more than that word, and its differential is dual to the Lie bracket. Its [cohomology](cohomology.md) is $\mathbb Q\oplus\bigoplus_i\mathbb Q a_{n_i}$ with all positive products zero. One way to compute this is $U(L)=T(e_i)$; the augmentation module has a length-one free resolution, so the corresponding Ext has only the unit and the dual generating classes.

##### Formal space

↑ **Parent:** [Sullivan minimal model](#sullivan-minimal-model)

A space is formal over $\mathbb Q$ if its rational cochain commutative [differential graded algebra](commutative-algebra.md#differential-graded-algebra) is joined to $(H^*(X;\mathbb Q),0)$ by [quasi-isomorphisms](homology.md#quasi-isomorphism). Equivalently in the usual [simply connected](#simply-connected-space) Sullivan-model setting, its [minimal model](#sullivan-minimal-model) has a [quasi-isomorphism](homology.md#quasi-isomorphism) to its [cohomology](cohomology.md) algebra with zero differential. This says its [rational homotopy type](#rational-homotopy-type) can be recovered from the [cohomology](cohomology.md) algebra; zero [cup products](cohomology.md#cup-product) alone do not imply [formality of a topological space](#formal-space) without an additional argument.

##### Sullivan model of the connected sum of two complex projective planes

↑ **Parent:** [Sullivan minimal model](#sullivan-minimal-model)

The two quadratic relations form a [regular sequence](commutative-algebra.md#regular-sequence) in $\mathbb Q[a,b]$, so their [Koszul complex](homology.md#koszul-complex) has only the quotient-ring [cohomology](cohomology.md). Represent the two degree-two classes by rational polynomial forms and choose primitives for the exact relations to obtain a [quasi-isomorphism](homology.md#quasi-isomorphism). There are no further generators.

### Reduced suspension

↑ **Parent:** [Homotopy](#homotopy)

The based suspension collapses both ends and the basepoint cylinder of $X\times I$ to one basepoint. The [loop space](#loop-space) and reduced suspension are adjoint in based [homotopy](#homotopy) theory. For a connected based [CW complex](#cw-complex), the [James reduced product](#james-reduced-product) models the loop space of its reduced suspension.

#### Suspension-loop adjunction

↑ **Parent:** [Reduced suspension](#reduced-suspension)

For based spaces there is a natural bijection $[\Sigma X,Y]\cong[X,\Omega Y]$. A map on the suspension sends a point $x$ and suspension coordinate $t$ to a loop $t\mapsto f(x,t)$; the collapsed ends and basepoint give based loops. The reverse construction evaluates such loops. The two constructions commute with based homotopies. Applied to spheres it gives $\pi_{n+1}Y\cong\pi_n\Omega Y$.

### Homotopy class

↑ **Parent:** [Homotopy](#homotopy)

An equivalence class of [continuous maps](topology.md#continuous-map) under [homotopy](#homotopy), with any endpoint or boundary restrictions specified. Unbased loop classes are free homotopy classes; periods of a [closed differential form](differential-form.md#closed-differential-form) are constant on such classes.

### Free homotopy

↑ **Parent:** [Homotopy](#homotopy)

A [free homotopy](#free-homotopy) between maps is an ordinary [homotopy](#homotopy) with no specified basepoint held fixed. Two loops at the same basepoint are freely homotopic precisely when their elements of the [fundamental group](#fundamental-group) are conjugate: a [homotopy](#homotopy) traces a connecting basepoint path, and the boundary of its parameter square gives conjugation. Conversely that connecting path can be slid around the loop to realize the conjugation.

### Null-homotopic map

↑ **Parent:** [Homotopy](#homotopy)

A map is null-homotopic when it is homotopic to a constant map.

#### Extension-null-homotopy criterion for a sphere

↑ **Parent:** [Null-homotopic map](#null-homotopic-map)

A map $f:S^{n-1}\to X$ extends to $D^n$ exactly when it is null-homotopic. An extension contracts radially through the disc; conversely, a null-homotopy descends through the cone quotient $CS^{n-1}\cong D^n$.

### Contractible space

↑ **Parent:** [Homotopy](#homotopy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Contractible_space)

A space is contractible when its identity map is homotopic to a constant map. Every map into a contractible space is null-homotopic.

#### Contraction of a topological space

↑ **Parent:** [Contractible space](#contractible-space)

A contraction is a [homotopy](#homotopy) from the identity map of $X$ to a constant map. Its existence says that $X$ is a [contractible space](#contractible-space). For a [tree](combinatorics.md#tree-graph-theory), choosing a root and moving each point along its unique finite path to that root gives a contraction, with continuity understood in the [weak topology of a CW complex](#weak-topology-of-a-cw-complex).

### Homotopy equivalence

↑ **Parent:** [Homotopy](#homotopy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homotopy_equivalence)

Spaces $X$ and $Y$ are homotopy equivalent when there are continuous maps

$$
f:X\to Y,\qquad g:Y\to X
$$

such that $g\circ f$ is homotopic to $\operatorname{id}_X$ and $f\circ g$ is homotopic to $\operatorname{id}_Y$.

#### Homology obstruction to carrying surface curves onto one another

↑ **Parent:** [Homotopy equivalence](#homotopy-equivalence)

A [homotopy equivalence](#homotopy-equivalence) of a [closed surface](differential-geometry.md#closed-surface) cannot carry a [simple closed curve](geometry-and-topology.md#simple-closed-curve) of nonzero integral [homology class](homology.md#homology-class) onto a contractible [simple closed curve](geometry-and-topology.md#simple-closed-curve). Any map into the latter factors through a circle whose inclusion induces zero on first [homology](homology.md); the former class would be killed by an isomorphism. Such a carrying map can nevertheless exist: project a handle generator onto a circle and compose with the contractible embedded circle.

#### Separate homotopy inverses combine into a homotopy equivalence

↑ **Parent:** [Homotopy equivalence](#homotopy-equivalence)

If $f:X\to Y$ has maps $g,h:Y\to X$ with $fg\simeq1_Y$ and $hf\simeq1_X$, then $h\simeq hfg\simeq g$, so $g$ is a two-sided homotopy inverse. More generally, if $fg$ and $hf$ are homotopy equivalences, composing $g$ and $h$ with their respective homotopy inverses supplies a right and a left homotopy inverse of $f$, reducing to the first case.

#### Homotopy type

↑ **Parent:** [Homotopy equivalence](#homotopy-equivalence)

Two spaces have the same homotopy type when there is a [homotopy equivalence](#homotopy-equivalence) between them. Their [homology](homology.md) and [homotopy groups](#homotopy-group) are then isomorphic. In [Morse theory](differential-geometry.md#morse-theory), attaching a cell records a change in the homotopy type of a sublevel set.

#### Homotopy inverse

↑ **Parent:** [Homotopy equivalence](#homotopy-equivalence)

If $g\circ f\simeq\operatorname{id}_X$ and $f\circ g\simeq\operatorname{id}_Y$, then $g$ is a homotopy inverse of $f$ and conversely.

### Retract

↑ **Parent:** [Homotopy](#homotopy)

A subspace $A\subseteq X$ is a retract of $X$ when there is a continuous map $r:X\to A$ whose restriction to $A$ is the identity.

#### Deformation retraction

↑ **Parent:** [Retract](#retract)

A deformation retraction of $X$ onto $A$ is a homotopy from $\operatorname{id}_X$ to a retraction $r:X\to A$ that keeps $A$ inside itself throughout. It makes the inclusion $A\hookrightarrow X$ a [homotopy equivalence](#homotopy-equivalence).

#### Retract of a contractible space

↑ **Parent:** [Retract](#retract)

Every retract of a contractible space is contractible. If $i:A\hookrightarrow X$ is the inclusion, $r:X\to A$ is a retraction, and $H$ contracts $X$, then

$$
(a,t)\longmapsto r(H(i(a),t))
$$

contracts $A$.

### Homotopy extension property

↑ **Parent:** [Homotopy](#homotopy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homotopy_extension_property)

A pair $(X,A)$ has the homotopy extension property when every homotopy on $A$ whose initial map extends to $X$ can itself be extended to a homotopy on $X$.

#### Cofibration

↑ **Parent:** [Homotopy extension property](#homotopy-extension-property)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cofibration)

A cofibration is a map with the [homotopy extension property](#homotopy-extension-property). An inclusion of a [CW complex](#cw-complex) into another as a subcomplex is a cofibration; collapsing that subcomplex gives the quotient used in the [K-theory six-term exact sequence](#k-theory-six-term-exact-sequence).

#### Collapsing a contractible cofibration

↑ **Parent:** [Homotopy extension property](#homotopy-extension-property)

If $A\subseteq X$ is contractible and $(X,A)$ has the homotopy extension property, the quotient map

$$
q:X\to X/A
$$

is a [homotopy equivalence](#homotopy-equivalence). Extend a contraction of $A$ to $X$; its endpoint is constant on $A$ and therefore factors through $q$ to supply a homotopy inverse.

### Homotopy group

↑ **Parent:** [Homotopy](#homotopy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homotopy_group)

The $n$th homotopy group consists of based homotopy classes of maps $S^n\to X$. It is a group for $n\geq1$ and an [abelian group](group.md#abelian-group) for $n\geq2$.

#### Whitehead product

↑ **Parent:** [Homotopy group](#homotopy-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Whitehead_product)

The geometric [Whitehead product](#whitehead-product) of based maps $\alpha:S^p\to Y$, $\beta:S^q\to Y$ is their [wedge sum](topology.md#wedge-sum) map composed with the attaching map $S^{p+q-1}\to S^p\vee S^q$ of the top cell of $S^p\times S^q$. With the usual geometric signs it satisfies $[\alpha,\beta]_{W}=(-1)^{pq}[\beta,\alpha]_{W}$. Regrading $\pi_pY$ to degree $p-1$ and setting $\{\alpha,\beta\}=(-1)^p[\alpha,\beta]_{W}$ gives the [graded Lie bracket](lie-algebra.md#graded-lie-bracket) transported from the [Samelson product](#samelson-product) on the loop space. In degrees $p,q\ge2$ it is bilinear; fundamental-group inputs instead record [commutators](lie-algebra.md#commutator) and the action of $\pi_1$ on higher [homotopy](#homotopy).

##### Whitehead square

↑ **Parent:** [Whitehead product](#whitehead-product)

The Whitehead square of a class $\alpha\in\pi_mY$ is $[\alpha,\alpha]\in\pi_{2m-1}Y$. For the identity class of an even-dimensional sphere, the [Hopf invariant](#hopf-invariant) is two with the standard product-cell orientation: folding the two sphere summands makes the middle [cohomology class](cohomology.md#cohomology-class) of the mapping cone pull back to $a+b$ on $S^m\times S^m$, and $(a+b)^2=2ab$. For odd $m$, graded symmetry makes the square two-torsion, hence rationally zero.

#### Postnikov tower

↑ **Parent:** [Homotopy group](#homotopy-group)

A [Postnikov tower](#postnikov-tower) of a connected [CW complex](#cw-complex) $X$ consists of spaces $P_nX$ with $\pi_i(P_nX)=\pi_i(X)$ for $i\le n$ and zero for $i>n$, together with compatible maps $X\to P_nX\to P_{n-1}X$. For [simply connected](#simply-connected-space) $X$, each stage is a [principal Eilenberg–MacLane fibration](#principal-eilenberg-maclane-fibration) with fibre $K(\pi_nX,n)$, classified by a [Postnikov invariant](#postnikov-invariant). The canonical map $X\to\operatorname{holim}_nP_nX$ is a weak equivalence: in each [homotopy](#homotopy) degree the tower is eventually constant, so the derived inverse-limit obstruction vanishes.

<h5 id="principal-eilenberg-maclane-fibration">Principal Eilenberg–MacLane fibration</h5>

↑ **Parent:** [Postnikov tower](#postnikov-tower)

For an abelian group $A$, a principal fibration with fibre $K(A,n)$ is a [homotopy pullback](#homotopy-pullback) of the [path fibration](#path-space-fibration) $PK(A,n+1)\to K(A,n+1)$. It is therefore the [homotopy fibre](#homotopy-fiber) of a map $k:B\to K(A,n+1)$ and is classified by $[k]\in H^{n+1}(B;A)$. The fibre acts by translation up to [homotopy](#homotopy); in this untwisted description the [fundamental group](#fundamental-group) acts trivially on $A$. This is the principal-fibration form used for [simply connected](#simply-connected-space) [Postnikov towers](#postnikov-tower).

###### Postnikov invariant

↑ **Parent:** [Principal Eilenberg–MacLane fibration](#principal-eilenberg-maclane-fibration)

The $n$th [Postnikov invariant](#postnikov-invariant) is the [cohomology class](cohomology.md#cohomology-class) $k_n\in H^{n+1}(P_{n-1}X;\pi_nX)$ whose representing map has [homotopy fibre](#homotopy-fiber) $P_nX$. It specifies how the new [homotopy group](#homotopy-group) is attached to the previous stage. A zero invariant gives the product $P_nX\simeq P_{n-1}X\times K(\pi_nX,n)$. Merely tensoring [homotopy groups](#homotopy-group) with $\mathbb Q$ does not describe [rationalization of a topological space](#rationalization-of-a-topological-space) unless these classes are also transported.

#### First homotopy group above the dimension of a sphere

↑ **Parent:** [Homotopy group](#homotopy-group)

The [universal cover](#universal-cover) of $S^1$ gives the first case. The [Hopf fibration](#hopf-fibration) $S^1\to S^3\to S^2$ identifies $\pi_3(S^2)$ with $\pi_3(S^3)=\mathbb Z$. Starting from $\pi_4(S^3)=\mathbb Z/2$, the [Freudenthal suspension theorem](#freudenthal-suspension-theorem) makes every subsequent [suspension](#suspension-topology) in these degrees an isomorphism. The stable range does not include the first step from $\pi_3(S^2)$ to $\pi_4(S^3)$, so the integer group at $n=2$ is not a contradiction.

#### Serre finiteness theorem for homotopy groups

↑ **Parent:** [Homotopy group](#homotopy-group)

A simply connected [CW complex](#cw-complex) of finite type has finitely generated [homotopy groups](#homotopy-group) in every degree. More generally, finite generation of its integral [homology](homology.md) groups in each degree suffices. This is a finiteness theorem, not a claim that the groups are finite. A finite [fundamental group](#fundamental-group) allows the same conclusion after passing to a [universal cover](#universal-cover) with finite type: a finite number of base cells lifts to a finite number of covering cells in each degree. It permits higher [homotopy](#homotopy) to be killed with finitely many cell attachments per dimension.

#### Relative homotopy group

↑ **Parent:** [Homotopy group](#homotopy-group)

Based relative maps of a disk into $X$ with its boundary mapped into $A$, modulo homotopies preserving these conditions. Replacing a map by its [mapping cylinder](#mapping-cylinder) gives relative groups for a general map. They fit into the [long exact sequence of relative homotopy groups](#long-exact-sequence-of-relative-homotopy-groups) and detect connectivity of the map.

##### Homotopy excision theorem

↑ **Parent:** [Relative homotopy group](#relative-homotopy-group)

For a based CW triad with connected intersection $A$, if $(B,A)$ is $p$-connected and $(C,A)$ is $q$-connected, $p,q\ge1$, the comparison map is an [isomorphism](algebra.md#isomorphism) for $i<p+q$ and a surjection for $i=p+q$. This connectivity form of the Blakers-Massey theorem controls the failure of ordinary relative [homotopy](#homotopy) to satisfy unrestricted excision.

##### Long exact sequence of relative homotopy groups

↑ **Parent:** [Relative homotopy group](#relative-homotopy-group)

Inclusion, the map sending an absolute disk class to a relative one, and restriction to the disk boundary give this exact sequence. Its low-dimensional end is interpreted with pointed sets and the usual fundamental-group action. For a mapping-cylinder pair it measures the failure of a map to induce [homotopy](#homotopy) isomorphisms.

<h4 id="eilenberg-maclane-space">Eilenberg–MacLane space</h4>

↑ **Parent:** [Homotopy group](#homotopy-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eilenberg–MacLane_space)

A connected Eilenberg–MacLane space $K(G,n)$, $n\geq1$, has $\pi_n\cong G$ and all other positive-degree [homotopy groups](#homotopy-group) trivial. The group $G$ must be abelian when $n\geq2$, but may be nonabelian when $n=1$. For an [abelian group](group.md#abelian-group), the [Dold–Kan correspondence](#dold-kan-correspondence) constructs a simplicial model from the [chain complex](homology.md#chain-complex) concentrated in degree $n$. A [classifying space of a discrete group](fiber-bundle.md#classifying-space-of-a-discrete-group) gives the general $K(G,1)$ case.

<h5 id="low-degree-integral-homology-of-a-mod-two-eilenberg-maclane-space">Low-degree integral homology of a mod-two Eilenberg–MacLane space</h5>

↑ **Parent:** [Eilenberg–MacLane space](#eilenberg-maclane-space)

For $n\geq4$, the first four possible degrees have integral groups $\mathbb Z/2,0,\mathbb Z/2,\mathbb Z/2$ in degrees $n,n+1,n+2,n+3$. Mod-two Betti numbers count cyclic summands, while the nonzero first Bockstein actions on $u,\operatorname{Sq}^2u,\operatorname{Sq}^2\operatorname{Sq}^1u$ show that their orders are two. This prevents mistaking a nonzero mod-two group for a higher-order integral cyclic group.

<h5 id="serre-polynomial-generators-for-mod-two-eilenberg-maclane-cohomology">Serre polynomial generators for mod-two Eilenberg–MacLane cohomology</h5>

↑ **Parent:** [Eilenberg–MacLane space](#eilenberg-maclane-space)

For $n\geq1$, the mod-two cohomology of $K(\mathbb Z/2,n)$ is polynomial on the admissible operations in the displayed strict-excess range, including the empty operation. It is obtained from path-space transgressions and compatibility with [Steenrod squares](cohomology.md#steenrod-square). Products must still be included when listing low-degree vector-space bases.

<h6 id="low-degree-mod-two-cohomology-of-an-eilenberg-maclane-space">Low-degree mod-two cohomology of an Eilenberg–MacLane space</h6>

↑ **Parent:** [Serre polynomial generators for mod-two Eilenberg–MacLane cohomology](#serre-polynomial-generators-for-mod-two-eilenberg-maclane-cohomology)

For $n\geq2$, the positive-degree dimensions in degrees $n,n+1,n+2,n+3$ are $1,1,1,2$. The first three classes are $u,\operatorname{Sq}^1u,\operatorname{Sq}^2u$. In degree $n+3$, use $\operatorname{Sq}^3u$ and $\operatorname{Sq}^2\operatorname{Sq}^1u$ for $n\geq3$; at $n=2$ replace the unstable first class by $u\operatorname{Sq}^1u$. At $n=2$ the degree-four class is $u^2$, and at $n=3$ the degree-six class $\operatorname{Sq}^3u$ is $u^2$.

<h5 id="rational-cohomology-of-an-integral-eilenberg-maclane-space">Rational cohomology of an integral Eilenberg–MacLane space</h5>

↑ **Parent:** [Eilenberg–MacLane space](#eilenberg-maclane-space)

The ring is exterior on its degree-$n$ universal class for odd $n$, and polynomial for even $n$. The path-loop [Serre spectral sequence](#serre-spectral-sequence) alternates these two types by transgression. In the polynomial-fiber case its derivation has nonzero coefficients $k$ on powers, which become invertible over the rationals.

<h5 id="representability-of-cohomology-by-eilenberg-maclane-spaces">Representability of cohomology by Eilenberg–MacLane spaces</h5>

↑ **Parent:** [Eilenberg–MacLane space](#eilenberg-maclane-space)

For a [CW complex](#cw-complex) $X$, abelian $G$ and $n\geq1$, [homotopy](#homotopy) classes of maps to the [Eilenberg–MacLane space](#eilenberg-maclane-space) correspond to [cohomology](cohomology.md) classes by pullback of the [universal cohomology class of an Eilenberg–MacLane space](#universal-cohomology-class-of-an-eilenberg-maclane-space). Pointed maps give the reduced version. This converts a [cohomology](cohomology.md) class into an actual map realizing its effect on [homotopy](#homotopy).

<h5 id="universal-cohomology-class-of-an-eilenberg-maclane-space">Universal cohomology class of an Eilenberg–MacLane space</h5>

↑ **Parent:** [Eilenberg–MacLane space](#eilenberg-maclane-space)

For abelian $G$ and $n\geq1$, the identity of $G$ determines this class under $H^n(K(G,n);G)\cong\operatorname{Hom}(G,G)$. Pulling it back realizes [representability of cohomology by Eilenberg–MacLane spaces](#representability-of-cohomology-by-eilenberg-maclane-spaces). A map inducing this class on a fiber induces the identity of its unique positive [homotopy group](#homotopy-group).

##### Aspherical space

↑ **Parent:** [Eilenberg–MacLane space](#eilenberg-maclane-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Aspherical_space)

A path-connected space is aspherical when its higher [homotopy groups](#homotopy-group) vanish, equivalently when its universal cover is contractible. An aspherical space with fundamental group $G$ is a $K(G,1)$, so based homotopy classes of maps into it are controlled by homomorphisms of fundamental groups.

#### Homotopy groups as modules over the fundamental group

↑ **Parent:** [Homotopy group](#homotopy-group)

Moving the basepoint around a loop acts on a higher [homotopy group](#homotopy-group). Since $\pi_n(X)$ is an [abelian group](group.md#abelian-group) for $n\geq2$, this action extends linearly to its integral [group ring](commutative-algebra.md#group-ring), making $\pi_n(X)$ a module. For a connected [CW complex](#cw-complex), its [universal cover](#universal-cover) gives an equivalent description by [deck transformations](#deck-transformation), together with change of basepoint upstairs. Left and right conventions are converted by inversion of the loop. The [Hurewicz theorem](#hurewicz-theorem) respects this action whenever it identifies a higher [homotopy group](#homotopy-group) with the corresponding homology of the cover.

#### Freudenthal suspension theorem

↑ **Parent:** [Homotopy group](#homotopy-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Freudenthal_suspension_theorem)

If $X$ is an $(n-1)$-connected based [CW complex](#cw-complex), $n\geq2$, suspension induces an isomorphism $\pi_k(X)\to\pi_{k+1}(\Sigma X)$ for $k\leq2n-2$ and a surjection for $k=2n-1$. For a [sphere](geometry-and-topology.md#sphere), $\Sigma S^n\cong S^{n+1}$, giving the stable range $\pi_k(S^n)\cong\pi_{k+1}(S^{n+1})$.

##### Freudenthal suspension from two cones

↑ **Parent:** [Freudenthal suspension theorem](#freudenthal-suspension-theorem)

Write the suspension of an $(n-2)$-connected based [CW complex](#cw-complex) as two cones meeting in the original space. Each cone pair is $(n-1)$-connected because its relative [groups](group.md) shift the original [homotopy groups](#homotopy-group) by one. [Homotopy excision theorem](#homotopy-excision-theorem) compares the cone pair with the suspension relative to the other cone, giving the suspension [homomorphism](algebra.md#homomorphism) as an [isomorphism](algebra.md#isomorphism) for $i<2n-2$ and a surjection at $i=2n-2$ in the indexing $\pi_{i-1}X\to\pi_i\Sigma X$.

##### Homology comparison proof of Freudenthal suspension

↑ **Parent:** [Freudenthal suspension theorem](#freudenthal-suspension-theorem)

The [integral homology of the loop space of a sphere](#integral-homology-of-the-loop-space-of-a-sphere) implies that the unit $S^{r-1}\to\Omega S^r$ has vanishing [relative homology](homology.md#relative-homology) through degree $2r-3$. Both spaces are simply connected for $r\geq3$. The absolute [Hurewicz theorem](#hurewicz-theorem) first identifies their degree-two [homotopy groups](#homotopy-group) with [homology](homology.md); the relative [Hurewicz theorem](#hurewicz-theorem) then rules out a first nonzero [relative homotopy group](#relative-homotopy-group) in degrees three through $2r-3$. The relative [homotopy](#homotopy) sequence makes the unit an isomorphism on $\pi_i$ through degree $2r-4$. Loop-suspension adjunction identifies this map with [suspension](#suspension-topology), yielding $\pi_i(S^{r-1})\cong\pi_{i+1}(S^r)$ in that range.

#### Hopf invariant

↑ **Parent:** [Homotopy group](#homotopy-group)

For $\phi:S^{2q-1}\to S^q$, $q>1$, its mapping cone has integral [cohomology](cohomology.md) generators $a$ in degree $q$ and $b$ in degree $2q$. The integer defined by $a\smile a=H(\phi)b$, with fixed cell orientations, is the Hopf invariant. It measures how an attaching map changes multiplication without changing the additive groups. The complex [Hopf fibration](#hopf-fibration) has invariant one because its mapping cone is $\mathbb{CP}^2$; a constant attaching map has invariant zero.

##### Cohomology ring of a Hopf attachment with a sphere summand

↑ **Parent:** [Hopf invariant](#hopf-invariant)

For the [Hopf map](#hopf-map) $\eta$, the indicated four-cell attachment has cellular boundary multiplication by $f$ from dimension four to three. Its integral [cohomology](cohomology.md) is $\mathbb Z$ in degrees zero and two, $\ker(f:\mathbb Z\to\mathbb Z)$ in degree three, and $\mathbb Z/f\mathbb Z$ in degree four. If $x$ generates degree two and $z$ is the four-cell cochain class, then $x^2=dz$, with every other positive-degree product zero. Collapsing the three-sphere reduces the cup-square calculation to the [Hopf invariant](#hopf-invariant); the induced map on degree-four cohomology reduces its integer coefficient modulo $f$. When $f=0$ there is an extra free degree-three class, whose products still vanish by dimension.

###### Third homotopy group of a Hopf attachment with a sphere summand

↑ **Parent:** [Cohomology ring of a Hopf attachment with a sphere summand](#cohomology-ring-of-a-hopf-attachment-with-a-sphere-summand)

Map $X_{d,f}$ to $K(\mathbb Z,2)=\mathbb{CP}^\infty$ using its degree-two generator. The [homotopy fibre](#homotopy-fiber) is the total space of the corresponding [circle bundle](fiber-bundle.md#circle-bundle), is 2-connected, and has $\pi_3$ equal to that of $X_{d,f}$. Over $S^2\vee S^3$ its total space is $P=S^3\cup_{S^1}(S^1\times S^3)$, with $H_3(P)=\mathbb Z A\oplus\mathbb Z B$. The four-cell bundle is trivial; its relative degree-four generator has boundary $dA+fB$, the lifted attaching map. The [long exact sequence in relative homology](homology.md#long-exact-sequence-in-relative-homology) and [Hurewicz theorem](#hurewicz-theorem) therefore give $\pi_3(X_{d,f})=\mathbb Z^2/\langle(d,f)\rangle$. [Smith normal form](algebra.md#smith-normal-form) gives the displayed expression when $d>0$, including $f=0$.

##### Precomposition scales the Hopf invariant by degree

↑ **Parent:** [Hopf invariant](#hopf-invariant)

Let $\phi:S^{2q-1}\to S^q$ and precompose with a sphere self-map of [topological degree](geometry-and-topology.md#topological-degree) $d$. The resulting map of mapping cones is the identity on the bottom $q$-cell and has degree $d$ on the top $2q$-cell. Pulling back the defining [cup product](cohomology.md#cup-product) relation for the [Hopf invariant](#hopf-invariant) multiplies its coefficient by $d$. In particular the element $d\eta\in\pi_3(S^2)$ has [Hopf invariant](#hopf-invariant) $d$. Postcomposition by a degree-$d$ map of the target sphere instead multiplies the invariant by $d^2$.

#### Weak homotopy equivalence

↑ **Parent:** [Homotopy group](#homotopy-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weak_homotopy_equivalence)

A map is a weak homotopy equivalence when it induces a bijection on path components and isomorphisms on every based homotopy group.

#### n-connected map

↑ **Parent:** [Homotopy group](#homotopy-group)

A map is $n$-connected when it induces isomorphisms on homotopy groups below degree $n$ and a surjection in degree $n$. Equivalently, each of its homotopy fibers is $(n-1)$-connected.

#### Loop-space shift of homotopy groups

↑ **Parent:** [Homotopy group](#homotopy-group)

For a based space $X$, adjunction gives

$$
\pi_i(\Omega X)\cong\pi_{i+1}(X).
$$

#### Rational homotopy group

↑ **Parent:** [Homotopy group](#homotopy-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rational_homotopy_group)

The rational homotopy group is obtained by tensoring a homotopy group with the [rational numbers](number-theory.md#rational-number). It retains the free part and discards torsion.

##### Rational homotopy groups of the connected sum of two complex projective planes

↑ **Parent:** [Rational homotopy group](#rational-homotopy-group)

The [Sullivan model of the connected sum of two complex projective planes](#sullivan-model-of-the-connected-sum-of-two-complex-projective-planes) has two generators in each of degrees two and three, and none elsewhere. Its rational [homotopy groups](#homotopy-group) are therefore exactly the displayed two copies of $\mathbb Q^2$, with all other positive degrees zero.

##### Rational homotopy groups of a sphere

↑ **Parent:** [Rational homotopy group](#rational-homotopy-group)

For an odd-dimensional sphere $S^{2m+1}$, only $\pi_{2m+1}(S^{2m+1})\otimes\mathbb Q$ is nonzero. For an even-dimensional sphere $S^{2m}$, the nonzero rational homotopy groups occur in degrees $2m$ and $4m-1$, and both are isomorphic to $\mathbb Q$.

#### Hurewicz theorem

↑ **Parent:** [Homotopy group](#homotopy-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hurewicz_theorem)

If a path-connected space is $(n-1)$-connected for $n\geq2$, then its first potentially nonzero homotopy group maps isomorphically to homology:

$$
\pi_n(X)\xrightarrow{\sim}H_n(X;\mathbb Z).
$$

##### Hurewicz homomorphism

↑ **Parent:** [Hurewicz theorem](#hurewicz-theorem)

A sphere map $f:S^n\to X$ is sent to $f_*[S^n]\in H_n(X;\mathbb Z)$. After tensoring with $\mathbb Q$ this gives the rational [Hurewicz homomorphism](#hurewicz-homomorphism). It is natural in $X$, sends [Whitehead products](#whitehead-product) to zero, and is an isomorphism in the first nonzero [homotopy](#homotopy) degree of a [simply connected](#simply-connected-space) space by the [Hurewicz theorem](#hurewicz-theorem).

###### Surjective rational Hurewicz homomorphism gives a wedge of spheres

↑ **Parent:** [Hurewicz homomorphism](#hurewicz-homomorphism)

If $X$ is [simply connected](#simply-connected-space) and $h_*:\pi_*(X)\otimes\mathbb Q\to\widetilde H_*(X;\mathbb Q)$ is onto, choose a homogeneous [homology](homology.md) [basis](vector-space.md#basis) and representing sphere maps into $X_{\mathbb Q}$. Their [wedge sum](topology.md#wedge-sum) gives a [rational homology](homology.md#rational-homology) equivalence, hence a [rational homotopy equivalence](#rational-homotopy-equivalence) by the [rational Whitehead theorem](#rational-whitehead-theorem). All positive [cup products](cohomology.md#cup-product) therefore vanish. In a [minimal model](#sullivan-minimal-model), the induced map from [cohomology](cohomology.md) to the indecomposable quotient is injective; replacing a set of generators by cocycle representatives produces a [quasi-isomorphism](homology.md#quasi-isomorphism) to the square-zero [cohomology](cohomology.md) algebra, proving [formality of a topological space](#formal-space).

##### Relative Hurewicz theorem

↑ **Parent:** [Hurewicz theorem](#hurewicz-theorem)

If $X$ and $A$ are [simply connected](#simply-connected-space) and the pair is $(r-1)$-connected, with $r\geq3$, its first possible nonzero relative [homotopy group](#homotopy-group) maps isomorphically to relative integral [homology](homology.md). This lets a basis of a free relative [homology](homology.md) group be realized by attaching disks.

##### Hurewicz theorem modulo a Serre class

↑ **Parent:** [Hurewicz theorem](#hurewicz-theorem)

For a [simply connected](#simply-connected-space) space, if lower [homotopy groups](#homotopy-group) lie in an admissible [Serre class](group.md#serre-class), the Hurewicz map in the next degree is an isomorphism modulo that class, and the lower [homology](homology.md) groups lie in the class. This applies to finitely generated groups and to finite groups supported at prescribed primes.

#### Whitehead theorem

↑ **Parent:** [Homotopy group](#homotopy-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Whitehead_theorem)

A weak homotopy equivalence between connected CW complexes is a [homotopy equivalence](#homotopy-equivalence). The analogous statement holds for [Kan complexes](#kan-complex).

##### Rational Whitehead theorem

↑ **Parent:** [Whitehead theorem](#whitehead-theorem)

For maps between [simply connected](#simply-connected-space) spaces, a rational [homology](homology.md) equivalence is a rational [homotopy equivalence](#homotopy-equivalence). It follows from the relative Hurewicz theorem modulo torsion, or from rationalization and the [homological Whitehead theorem](#homological-whitehead-theorem).

##### Homological Whitehead theorem

↑ **Parent:** [Whitehead theorem](#whitehead-theorem)

An integral [homology](homology.md) equivalence between [simply connected](#simply-connected-space) spaces is a [weak homotopy equivalence](#weak-homotopy-equivalence). A first nonzero relative [homotopy group](#homotopy-group) would contradict the [Relative Hurewicz theorem](#relative-hurewicz-theorem). Between [CW complexes](#cw-complex) the ordinary [Whitehead theorem](#whitehead-theorem) then gives a [homotopy equivalence](#homotopy-equivalence).

### Homotopy fiber

↑ **Parent:** [Homotopy](#homotopy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homotopy_fiber)

The homotopy fiber of $f:X\to Y$ over $y_0$ consists of pairs $(x,\gamma)$ where $\gamma$ is a path from $f(x)$ to $y_0$. It replaces an ordinary fiber by a homotopy-invariant construction.

#### Principal fibration

↑ **Parent:** [Homotopy fiber](#homotopy-fiber)

A principal fibration, in the homotopy-theoretic sense, is a homotopy pullback of a [path-space fibration](#path-space-fibration) $PC\to C$ along a map $k:B\to C$. Its fibre is $\Omega C$ and acts on the fibre paths by concatenation, freely and transitively up to the relevant homotopies. Principal bundles for a topological group give this construction through its classifying space. When $C=K(A,n+1)$, the fibre is $K(A,n)$ and the principal fibration is classified by $H^{n+1}(B;A)$, yielding a [principal Eilenberg–MacLane fibration](#principal-eilenberg-maclane-fibration).

#### Path-space fibration

↑ **Parent:** [Homotopy fiber](#homotopy-fiber)

Let $PX$ consist of paths starting at the chosen basepoint of $X$. Endpoint evaluation is a fibration $\Omega X\to PX\to X$, and $PX$ is contractible by shortening each path. Pulling it back along a map $Y\to X$ gives its [homotopy fibre](#homotopy-fiber), after reversing the chosen path direction if needed. This makes an acyclic relative Sullivan algebra modelling $PX$ useful for explicit rational fibre calculations.

### Fibration

↑ **Parent:** [Homotopy](#homotopy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fibration)

A fibration is a map with the [homotopy lifting property](#homotopy-lifting-property). A Hurewicz fibration has this property for every source space; a [Serre fibration](#serre-fibration) requires it for [CW complexes](#cw-complex). Replacing a map by a fibration gives a model for its [homotopy fiber sequence](#homotopy-fiber-sequence).

### Homotopy fiber sequence

↑ **Parent:** [Homotopy](#homotopy)

A [homotopy fiber sequence](#homotopy-fiber-sequence) identifies a fibre after replacing a map by a suitable [fibration](#fibration).

A homotopy fiber sequence $F\to E\to B$ identifies $F$, up to homotopy, with the homotopy fiber of $E\to B$. It induces a long exact sequence of [homotopy groups](#homotopy-group).

### Homotopy pullback

↑ **Parent:** [Homotopy](#homotopy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homotopy_pullback)

A homotopy pullback is the derived form of a pullback. A strict pullback square of fibrant objects computes a homotopy pullback whenever one of the two maps into the lower-right object is a fibration.

### Loop space

↑ **Parent:** [Homotopy](#homotopy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loop_space)

The loop space $\Omega X$ is the space of based loops in $X$. It is the homotopy fiber of the inclusion of the base point into $X$.

#### Samelson product

↑ **Parent:** [Loop space](#loop-space)

For sphere maps into a loop space or a group-like homotopy-associative space, take their pointwise [commutator](lie-algebra.md#commutator). It is trivial on the [wedge sum](topology.md#wedge-sum) of the two sphere factors, so descends to their smash product and defines $\langle a,b\rangle\in\pi_{p+q}(\Omega Y)$. This product obeys graded antisymmetry and the graded Jacobi identity. [Suspension-loop adjunction](#suspension-loop-adjunction) identifies it with the sign-adjusted [Whitehead product](#whitehead-product). Under the [Hurewicz homomorphism](#hurewicz-homomorphism) it becomes the graded [commutator](lie-algebra.md#commutator) of the [Pontryagin product](#pontryagin-product-on-loop-space-homology).

#### Based path space and the path-loop fibration

↑ **Parent:** [Loop space](#loop-space)

The based path space $P_{x_0}X$ consists of continuous paths beginning at $x_0$, with variable endpoint and the compact-open topology. Endpoint evaluation is a [Serre fibration](#serre-fibration) with fiber the based [loop space](#loop-space). Its total space is contractible by $\gamma(t)\mapsto\gamma(st)$ as $s$ decreases to zero. This differs from a space of paths with both endpoints fixed, which need not be contractible. The [long exact sequence of homotopy groups of a fibration](#long-exact-sequence-of-homotopy-groups-of-a-fibration) gives $\pi_i(\Omega X)\cong\pi_{i+1}(X)$ for connected $X$ in the usual based ranges.

#### Integral homology of the loop space of a sphere

↑ **Parent:** [Loop space](#loop-space)

For $r\geq3$, the path-loop [Serre fibration](#serre-fibration) has contractible total space. The [relative homology of a fibration over a sphere](#relative-homology-of-a-fibration-over-a-sphere) gives $H_j(\Omega S^r)\cong H_{j-r+1}(\Omega S^r)$ for $j>0$, with negative [homology](homology.md) zero and $H_0=\mathbb Z$. This proves the displayed groups. The unit map $S^{r-1}\to\Omega S^r$, adjoint to the identity of $S^r$, represents the generator of the first nonzero [homotopy group](#homotopy-group). Naturality of the [Hurewicz theorem](#hurewicz-theorem) shows that it induces an integral [homology](homology.md) isomorphism in all degrees through $2r-3$.

#### Integral cohomology of an odd-sphere loop space

↑ **Parent:** [Loop space](#loop-space)

For $n\geq1$, there is one integral cohomology generator $a_k$ in every degree $2nk$, and its products are $a_i a_j=\binom{i+j}{i}a_{i+j}$. The [Bott–Samelson theorem](#bott-samelson-theorem) supplies free polynomial [homology](homology.md); its primitive generator gives the binomial diagonal dual to this [divided power algebra](commutative-algebra.md#divided-power-algebra).

#### Pontryagin ring

↑ **Parent:** [Loop space](#loop-space)

The [homology](homology.md) ring formed from loop concatenation and the [homology cross product](cohomology.md#homology-cross-product). [Homotopy](#homotopy) associativity is enough for associativity in [homology](homology.md), and the constant loop is the unit. More generally the same construction applies to a homotopy-associative H-space.

<h5 id="milnor-moore-theorem">Milnor–Moore theorem</h5>

↑ **Parent:** [Pontryagin ring](#pontryagin-ring)

For [simply connected](#simply-connected-space) $Y$, rational [Hurewicz homomorphism](#hurewicz-homomorphism) identifies $\pi_*(\Omega Y)\otimes\mathbb Q$ with the [primitive elements of a Hopf algebra](algebra.md#primitive-element-of-a-hopf-algebra) of $H_*(\Omega Y;\mathbb Q)$ and induces an isomorphism $U(\pi_*(\Omega Y)\otimes\mathbb Q)\cong H_*(\Omega Y;\mathbb Q)$ of graded Hopf algebras. The bracket on [homotopy](#homotopy) is the [Samelson product](#samelson-product). The underlying algebra theorem says that a connected graded cocommutative [Hopf algebra](algebra.md#hopf-algebra) over [characteristic zero](algebra.md#characteristic-zero) is the [universal enveloping algebra](lie-algebra.md#universal-enveloping-algebra) of its primitive [Lie algebra](lie-algebra.md). These statements let a free [tensor algebra](linear-algebra.md#tensor-algebra) of loop-space [homology](homology.md) detect a [free graded Lie algebra](lie-algebra.md#free-graded-lie-algebra) of [homotopy](#homotopy).

##### Pontryagin ring of an odd-sphere loop space

↑ **Parent:** [Pontryagin ring](#pontryagin-ring)

For $n\geq1$, the [Bott–Samelson theorem](#bott-samelson-theorem) gives a single homology generator of degree $2n$ with no word relations. Its [Pontryagin product](#pontryagin-product-on-loop-space-homology) satisfies $x^i*x^j=x^{i+j}$. Unlike this polynomial [homology](homology.md) product, the [cohomology](cohomology.md) cup product has divided-power coefficients.

##### Pontryagin product on loop-space homology

↑ **Parent:** [Pontryagin ring](#pontryagin-ring)

Apply the [homology cross product](cohomology.md#homology-cross-product) and then the map induced by loop concatenation. This degree-additive bilinear product supplies the [Pontryagin ring](#pontryagin-ring). The [Bott–Samelson theorem](#bott-samelson-theorem) computes it for looped suspensions with free [homology](homology.md).

#### James reduced product

↑ **Parent:** [Loop space](#loop-space)

Finite words in a based space, with occurrences of its basepoint deleted. Word concatenation defines a multiplication. For connected based CW spaces, the natural map to $\Omega\Sigma X$ is a [weak homotopy equivalence](#weak-homotopy-equivalence). With free integral [homology](homology.md), the [Bott–Samelson theorem](#bott-samelson-theorem) identifies its [homology](homology.md) algebra with the [tensor algebra](linear-algebra.md#tensor-algebra) on reduced [homology](homology.md).

<h5 id="bott-samelson-theorem">Bott–Samelson theorem</h5>

↑ **Parent:** [James reduced product](#james-reduced-product)

For a connected based CW complex with free integral homology, the [Pontryagin ring](#pontryagin-ring) of its looped reduced suspension is the indicated tensor algebra. The generator inclusion comes from $X\to\Omega\Sigma X$, and multiplication corresponds to concatenation of words in the [James reduced product](#james-reduced-product).

#### Loop-space homology

↑ **Parent:** [Loop space](#loop-space)

Loop-space homology is the [homology](homology.md) of the based [loop space](#loop-space). It also carries the Pontryagin product induced by concatenation of loops. For $n>2$, a [Morse theory](differential-geometry.md#morse-theory) cell structure on $\Omega S^n$ has one cell in each dimension $j(n-1)$, so its integer homology is $\mathbb Z$ in those dimensions and zero elsewhere.

#### Path-loop fibration

↑ **Parent:** [Loop space](#loop-space)

The evaluation map from the based path space gives a fiber sequence

$$
\Omega X\longrightarrow PX\longrightarrow X.
$$

Since $PX$ is contractible, it relates invariants of $X$ to those of its [loop space](#loop-space).

##### Cohomology suspension

↑ **Parent:** [Path-loop fibration](#path-loop-fibration)

Pull back along loop evaluation $S^1\times\Omega B\to B$ and take the slant product with the circle's fundamental class. This degree-lowering operation kills positive-degree cup products. It commutes with stable [cohomology](cohomology.md) operations such as [Steenrod squares](cohomology.md#steenrod-square) and identifies a transgressing base class with its fiber class in the path-loop fibration.

### Simplicial homotopy theory

↑ **Parent:** [Homotopy](#homotopy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplicial_homotopy_theory)

Simplicial homotopy theory models spaces and higher categories using [simplicial sets](#simplicial-set).

#### Simplex category

↑ **Parent:** [Simplicial homotopy theory](#simplicial-homotopy-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplex_category)

The simplex category has objects the finite nonempty ordered sets $[n]=\{0<\cdots<n\}$ and morphisms the order-preserving maps.

#### Simplicial set

↑ **Parent:** [Simplicial homotopy theory](#simplicial-homotopy-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplicial_set)

A simplicial set is a [functor](category.md#functor) from the opposite of the [simplex category](#simplex-category) to sets. Its face and degeneracy maps satisfy the simplicial identities.

##### Geometric realization of a simplicial set

↑ **Parent:** [Simplicial set](#simplicial-set)

The geometric realization of a simplicial set glues one topological simplex for each simplicial simplex, using the face and degeneracy maps as the gluing relations.

##### Singular simplicial set

↑ **Parent:** [Simplicial set](#simplicial-set)

The singular simplicial set of a topological space $X$ has the continuous maps $\Delta^n\to X$ as its $n$-simplices. Evaluation gives a natural weak homotopy equivalence $|\operatorname{Sing}X|\to X$.

##### Standard simplex

↑ **Parent:** [Simplicial set](#simplicial-set)

The standard simplicial $n$-simplex is the representable simplicial set

$$
\Delta^n_m=\operatorname{Hom}_\Delta([m],[n]).
$$

###### Simplicial horn

↑ **Parent:** [Standard simplex](#standard-simplex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplicial_horn)

The $i$th horn $\Lambda_i^n\subseteq\Delta^n$ is the union of all codimension-one faces except the face opposite vertex $i$.

###### Inner horn

↑ **Parent:** [Simplicial horn](#simplicial-horn)

A horn $\Lambda_i^n$ is inner when $0<i<n$ and outer when $i=0$ or $i=n$.

##### Quasicategory

↑ **Parent:** [Simplicial set](#simplicial-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasicategory)

A quasicategory is a simplicial set in which every [inner horn](#inner-horn) has a filler.

##### Kan complex

↑ **Parent:** [Simplicial set](#simplicial-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kan_complex)

A Kan complex is a simplicial set in which every [simplicial horn](#simplicial-horn), including every outer horn, has a filler.

##### Nerve (category theory)

↑ **Parent:** [Simplicial set](#simplicial-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nerve_(category_theory))

The nerve of a category $\mathcal C$ has

$$
N(\mathcal C)_n=\operatorname{Fun}([n],\mathcal C),
$$

so an $n$-simplex is a string of $n$ composable morphisms. Every inner horn in a nerve has a unique filler.

##### Simplicial mapping space

↑ **Parent:** [Simplicial set](#simplicial-set)

The simplicial mapping space is defined by

$$
\underline{\operatorname{Hom}}(A,X)_n
=\operatorname{Hom}(A\times\Delta^n,X).
$$

If $A\hookrightarrow B$ is a monomorphism and $X$ is a [Kan complex](#kan-complex), restriction $\underline{\operatorname{Hom}}(B,X)\to\underline{\operatorname{Hom}}(A,X)$ is a Kan fibration.

#### Simplicial abelian group

↑ **Parent:** [Simplicial homotopy theory](#simplicial-homotopy-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplicial_abelian_group)

A simplicial abelian group is a simplicial object in [abelian groups](group.md#abelian-group). Its underlying simplicial set is always a [Kan complex](#kan-complex).

##### Normalized chain complex of a simplicial abelian group

↑ **Parent:** [Simplicial abelian group](#simplicial-abelian-group)

For a simplicial abelian group $A$, one convention for normalized chains is

$$
N_nA=\bigcap_{i=1}^n\ker(d_i:A_n\to A_{n-1}),
\qquad \partial=d_0.
$$

Equivalently, it is the quotient of the unnormalized chain complex by its degenerate subcomplex.

<h6 id="dold-kan-correspondence">Dold–Kan correspondence</h6>

↑ **Parent:** [Normalized chain complex of a simplicial abelian group](#normalized-chain-complex-of-a-simplicial-abelian-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dold–Kan_correspondence)

The normalized-chain functor gives an equivalence between [simplicial abelian groups](#simplicial-abelian-group) and nonnegatively graded [chain complexes](homology.md#chain-complex) of abelian groups. Its inverse is the Eilenberg–MacLane denormalization functor $K$.

### Serre spectral sequence

↑ **Parent:** [Homotopy](#homotopy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Serre_spectral_sequence)

For a fibration $F\to E\to B$ with suitable connectivity, the cohomological Serre spectral sequence has

$$
E_2^{p,q}=H^p(B;H^q(F;R))
\Longrightarrow H^{p+q}(E;R),
$$

with differential $d_r:E_r^{p,q}\to E_r^{p+r,q-r+1}$.

#### Cohomological Serre spectral sequence

↑ **Parent:** [Serre spectral sequence](#serre-spectral-sequence)

For a [Serre fibration](#serre-fibration), this first-quadrant spectral sequence has differential of bidegree $(r,1-r)$ and a fiber-cohomology local coefficient system on the base. A [simply connected](#simply-connected-space) base makes that system constant. Its edge map is restriction to the fiber; a surviving fiber class is the restriction of a total-space class. For commutative ring coefficients it is multiplicative and its differentials are graded derivations.

##### A sphere cannot fibre over a lower-dimensional odd sphere

↑ **Parent:** [Cohomological Serre spectral sequence](#cohomological-serre-spectral-sequence)

There is no [fiber bundle](fiber-bundle.md) $F\to S^m\to S^q$ when $m>q\geq3$ and $q$ is odd. A local trivialization makes $F$ a retract of an open subset of $S^m$, so $H^j(F;\mathbb Q)=0$ for $j>m$; the [long exact sequence of homotopy groups of a fibration](#long-exact-sequence-of-homotopy-groups-of-a-fibration) makes $F$ connected. In the multiplicative rational [Serre spectral sequence](#serre-spectral-sequence), only base columns zero and $q$ occur. Since $H^q(S^m)=0$, a fibre class $a\in H^{q-1}(F;\mathbb Q)$ must satisfy $d_qa=u$, the base generator. Its degree is even. If $a^s=0$ is its first vanishing power, the derivation law gives $0=d_q(a^s)=sua^{s-1}\ne0$ on the $E_q$ page, a contradiction. Bounded fibre cohomology ensures such a vanishing power exists. In particular $S^4$ cannot be the total space of a bundle over $S^3$.

#### Serre fibration

↑ **Parent:** [Serre spectral sequence](#serre-spectral-sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Serre_fibration)

A Serre fibration is a map having the [homotopy lifting property](#homotopy-lifting-property) with respect to every disc, equivalently every CW complex.

##### Relative homotopy of a Serre fibration

↑ **Parent:** [Serre fibration](#serre-fibration)

For a based [Serre fibration](#serre-fibration) with fibre $F$ over the basepoint, lift a based cube in $B$ from its constant bottom face, keeping the side faces fixed. Its final face lies in $F$, giving surjectivity of the relative map. [Homotopies](#homotopy) in $B$ lift; two lifts of the same cube are relatively homotopic by lifting with both side liftings prescribed. This gives injectivity. For $n\ge2$ this is a [group](group.md) [isomorphism](algebra.md#isomorphism); at $n=1$ it is initially a bijection of [pointed sets](set.md#pointed-set), unless the relative set is endowed with the [group](group.md) law transported through the fibration.

##### Relative homology of a fibration over a sphere

↑ **Parent:** [Serre fibration](#serre-fibration)

For a [Serre fibration](#serre-fibration) over $S^r$, cover the base by a contractible punctured sphere and a contractible ball. [Excision](homology.md#excision-theorem) relative to the preimage of the punctured sphere identifies the relative pair with the product of $F$ and $(D^r,S^{r-1})$ up to [homotopy](#homotopy). The base pair has a single free [homology](homology.md) group in degree $r$, so the [Künneth theorem](cohomology.md#kunneth-theorem) gives the displayed shift without a torsion term. The relative [long exact sequence](homology.md#long-exact-sequence) then gives $\cdots\to H_i(F)\to H_i(E)\to H_{i-r}(F)\to H_{i-1}(F)\to\cdots$. The connecting map retains the twisting of the original [Serre fibration](#serre-fibration).

<h5 id="splitting-of-a-simply-connected-eilenberg-maclane-fibration">Splitting of a simply connected Eilenberg–MacLane fibration</h5>

↑ **Parent:** [Serre fibration](#serre-fibration)

For a [Serre fibration](#serre-fibration) with this fiber over a simply connected CW base, the fiber identity class has only one possible nonzero outgoing differential in the [cohomological Serre spectral sequence](#cohomological-serre-spectral-sequence), landing in $H^{n+1}(B;G)$. If that group vanishes, the class extends to the CW total space. Its representing map, paired with projection to $B$, is an isomorphism on fiber and base [homotopy groups](#homotopy-group) and hence a [weak homotopy equivalence](#weak-homotopy-equivalence) to the product.

##### Mapping-path fibration replacement

↑ **Parent:** [Serre fibration](#serre-fibration)

For a map $f:X\to B$, let $E_f$ consist of points of $X$ and paths starting at their images, with projection $p(x,\gamma)=\gamma(1)$. Appending segments of a base homotopy proves the [homotopy lifting property](#homotopy-lifting-property), so $p$ is a [Serre fibration](#serre-fibration). The constant-path inclusion $s:X\to E_f$ satisfies $ps=f$ and is a [homotopy equivalence](#homotopy-equivalence): forget the path for an inverse, and shorten paths to prove the homotopy. The homotopy need not preserve the endpoint in $B$, so the statement concerns an equivalence of total spaces over a commuting triangle, not a fibrewise inverse. The fibre over $b_0$ is the [homotopy fibre](#homotopy-fiber) of $f$.

##### Homotopy lifting property

↑ **Parent:** [Serre fibration](#serre-fibration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homotopy_lifting_property)

A map $p:E\to B$ has the homotopy lifting property with respect to $X$ when every homotopy $X\times I\to B$ whose initial map lifts to $E$ has a lift extending that initial lift.

##### Long exact sequence of homotopy groups of a fibration

↑ **Parent:** [Serre fibration](#serre-fibration)

For a based fibration $F\to E\to B$, lifting representatives defines connecting maps and an exact sequence

$$
\cdots\to\pi_k(F)\to\pi_k(E)\to\pi_k(B)
\xrightarrow{\partial}\pi_{k-1}(F)\to\cdots.
$$

#### Wang homomorphism

↑ **Parent:** [Serre spectral sequence](#serre-spectral-sequence)

For a fibration over $S^n$, the only possible differential in the homological Serre spectral sequence is $d_n$. Identifying its two nonzero columns with the homology of the fiber gives the Wang homomorphism $\Delta$.

##### Wang sequence over a sphere

↑ **Parent:** [Wang homomorphism](#wang-homomorphism)

For a fibration $F\to E\to S^n$, the [Wang homomorphism](#wang-homomorphism) belongs to the exact sequence

$$
\cdots\to H_j(F)\to H_j(E)\to H_{j-n}(F)
\xrightarrow{\Delta}H_{j-1}(F)\to\cdots.
$$

#### Transgression

↑ **Parent:** [Serre spectral sequence](#serre-spectral-sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transgression)

A transgression is a spectral-sequence differential from a fiber class on the vertical edge to a base class on the horizontal edge.

##### Transgressive pair

↑ **Parent:** [Transgression](#transgression)

For a fibration $F\to E\to B$, classes $x\in H^r(F)$ and $y\in H^{r+1}(B)$ form a transgressive pair when their images in relative cohomology satisfy $\delta x=\pi^*y$. In the Serre spectral sequence this relation is represented by $d_{r+1}x=y$.

###### Kudo transgression theorem

↑ **Parent:** [Transgressive pair](#transgressive-pair)

Steenrod operations preserve transgressive pairs. With mod-two coefficients, if $(x,y)$ is transgressive, then so is $(\operatorname{Sq}^j x,\operatorname{Sq}^j y)$ whenever the square is defined by the instability range. The corresponding statement holds for odd-primary reduced powers and the Bockstein, with the appropriate page shift.

## Loop (topology)

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loop_(topology))

A loop in a [topological space](topology.md#topological-space) is a continuous map $\gamma:[0,1]\to X$ with $\gamma(0)=\gamma(1)$. Equivalently it is a map from the circle. A [based loop](#based-loop) also specifies the common endpoint as a chosen base point.

### Based loop

↑ **Parent:** [Loop (topology)](#loop-topology)

A based loop in $(X,x_0)$ is a path $\alpha:[0,1]\to X$ whose two endpoints are $x_0$.

#### Based homotopy

↑ **Parent:** [Based loop](#based-loop)

A based homotopy between based loops keeps both endpoints fixed at the base point throughout the deformation.

#### Path reversal

↑ **Parent:** [Based loop](#based-loop)

The reverse of a path $\alpha$ is $\bar\alpha(t)=\alpha(1-t)$. Concatenating a path with its reverse is homotopic relative to endpoints to the constant path.

## Fundamental group

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_group)

The fundamental group $\pi_1(X,x_0)$ consists of based loops modulo based homotopy, with multiplication induced by concatenation.

### Fundamental group of a surface

↑ **Parent:** [Fundamental group](#fundamental-group)

The [fundamental group](#fundamental-group) of a [surface](topology.md#topological-surface). For a closed orientable genus-$g$ surface the [fundamental group of a closed orientable surface](#fundamental-group-of-a-closed-orientable-surface) has $2g$ generators and one relation, the product of their paired commutators.

#### Dehn-Nielsen-Baer theorem for closed orientable surfaces

↑ **Parent:** [Fundamental group of a surface](#fundamental-group-of-a-surface)

For a closed orientable aspherical [topological surface](topology.md#topological-surface), every [outer automorphism](group-theory.md#outer-automorphism-of-a-group) of its [fundamental group](#fundamental-group) is induced by a surface homeomorphism. The mapping class group allowing orientation reversal is therefore the full outer automorphism group. For the torus the statement is realized by linear maps in $GL_2(\mathbb Z)$; for higher genus it is the Dehn-Nielsen-Baer theorem. A semidirect product by the infinite cyclic group is consequently the [fundamental group](#fundamental-group) of the corresponding [mapping torus](#mapping-torus).

### Closed-manifold realization of a finitely presented fundamental group

↑ **Parent:** [Fundamental group](#fundamental-group)

Every [finitely presented group](geometric-group-theory.md#finitely-presented-group) is the [fundamental group](#fundamental-group) of a closed connected smooth manifold in dimension at least four. Build a compact zero/one/two-handle manifold $W$ with the generators and relators of the presentation. Disjoint attaching loops can be embedded in its boundary of dimension at least three. The [Seifert-van Kampen theorem](#seifert-van-kampen-theorem) gives $\pi_1(W)=T$, and the dual relative handle structure makes $\pi_1(\partial W)\to T$ surjective. Doubling $W$ along its boundary gives the amalgam of two copies of $T$ along that same surjection, which is again $T$. This construction underlies [binary families of nonhomeomorphic Sunada quotients](riemannian-geometry.md#binary-family-of-nonhomeomorphic-sunada-quotients).

### Simply connected space

↑ **Parent:** [Fundamental group](#fundamental-group)

A simply connected space is path connected and has trivial [fundamental group](#fundamental-group): every closed loop contracts to a point. The [three-sphere](geometry-and-topology.md#three-sphere) is simply connected, whereas [Real projective space](#real-projective-space) $\mathbb{RP}^3$ has [fundamental group](#fundamental-group) $\mathbb Z_2$.

### Fundamental group of a bouquet of circles

↑ **Parent:** [Fundamental group](#fundamental-group)

The [fundamental group](#fundamental-group) of a bouquet of $r$ circles is the [free group](geometric-group-theory.md#free-group) on $r$ generators, represented by the oriented circles. For finite $r$, iterated [Seifert-van Kampen theorem](#seifert-van-kampen-theorem) proves the claim by attaching one circle at a time. Nontrivial [reduced words in a free group](geometric-group-theory.md#reduced-word-in-a-free-group) distinguish based loops, while [free homotopy](#free-homotopy) classes correspond to conjugacy classes.

### Change of basepoint isomorphism

↑ **Parent:** [Fundamental group](#fundamental-group)

Let $u$ be a path from $x_0$ to $x_1$. Traversing paths from left to right gives an [isomorphism](algebra.md#isomorphism)

$$
u_\#: \pi_1(X,x_0)\longrightarrow\pi_1(X,x_1),\qquad[\alpha]\longmapsto[\bar u*\alpha*u].
$$

Concatenation and cancellation of a path with its reverse prove the homomorphism property and show that $\bar u$ supplies its inverse. A different connecting path changes this isomorphism by an inner automorphism, so it need not be canonical.

### Well-defined loop concatenation

↑ **Parent:** [Fundamental group](#fundamental-group)

Concatenating two based homotopies proves that loop concatenation depends only on based-homotopy classes. Endpoint-fixing reparametrizations provide associativity and the identity laws on classes.

### Functoriality of the fundamental group

↑ **Parent:** [Fundamental group](#fundamental-group)

A continuous based map $f:(X,x_0)\to(Y,y_0)$ induces a homomorphism $f_*:\pi_1(X,x_0)\to\pi_1(Y,y_0)$ by composition of loops with $f$.

### Seifert-van Kampen theorem

↑ **Parent:** [Fundamental group](#fundamental-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Seifert-van_Kampen_theorem)

For a suitably path-connected open cover $X=U\cup V$, the fundamental group of $X$ is the pushout of the homomorphisms from $\pi_1(U\cap V)$ to $\pi_1(U)$ and $\pi_1(V)$.

#### Fundamental group of a wedge of circles and a real projective plane

↑ **Parent:** [Seifert-van Kampen theorem](#seifert-van-kampen-theorem)

For

$$
X_n=\bigvee_{i=1}^nS^1\vee\mathbb{RP}^2,
$$

the Seifert-van Kampen theorem gives

$$
\pi_1(X_n)\cong F_n*C_2
=\langle a_1,\ldots,a_n,b\mid b^2=1\rangle.
$$

#### Amalgamated free product

↑ **Parent:** [Seifert-van Kampen theorem](#seifert-van-kampen-theorem)

Given homomorphisms $i_A:C\to A$ and $i_B:C\to B$, the amalgamated free product $A*_CB$ comes with homomorphisms from $A$ and $B$ that agree on $C$. It is universal with this property: every compatible pair of homomorphisms $A\to H$ and $B\to H$ factors uniquely through $A*_CB$.

##### Free product

↑ **Parent:** [Amalgamated free product](#amalgamated-free-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Free_product)

The free product $A*B$ is the [amalgamated free product](#amalgamated-free-product) over the trivial group. Its nonidentity elements have unique reduced alternating normal forms.

###### Effective cyclic membership in a free product

↑ **Parent:** [Free product](#free-product)

Suppose $P$ has a soluble [word problem for a group](geometric-group-theory.md#word-problem-for-groups) and $z$ generates an infinite [cyclic group](group.md#cyclic-group). In $P*\langle z\rangle$, for $g\ne1$ the words $gz$ and $[g,z]$ are cyclically reduced with two and four syllables respectively. Their nonzero powers have syllable lengths $2|k|$ and $4|k|$. Given an input's reduced [free product](#free-product) form, its length bounds the possible exponents; compare the finitely many candidates using the base word algorithm. Membership and the exponent in each of these infinite cyclic subgroups are therefore computable, with no algorithm for the order of $g$ required.

###### Free factor

↑ **Parent:** [Free product](#free-product)

A subgroup $A$ is a free factor of $G$ if $G$ is isomorphic to a [free product](#free-product) $A*B$ by an isomorphism restricting to the inclusion of $A$, for some subgroup $B$. The [normal form theorem for a free product](#normal-form-theorem-for-a-free-product) ensures that both factors embed. A free factor need not be a [normal subgroup](group-theory.md#normal-subgroup).

###### Universal property of a free product

↑ **Parent:** [Free product](#free-product)

Given [group homomorphisms](group-theory.md#group-homomorphism) $f_A:A\to H$ and $f_B:B\to H$, there is exactly one [group homomorphism](group-theory.md#group-homomorphism) $A*B\to H$ extending both. Its value on an alternating normal form is the product of the factor-map values. Thus the [free product](#free-product) is the coproduct in the [category of groups](category-theory.md#category-of-groups).

###### Nontrivial free product

↑ **Parent:** [Free product](#free-product)

A [free product](#free-product) $A*B$ is nontrivial as a splitting when both factors differ from the [trivial group](group.md#trivial-group). Alternating words $(ab)^r$ with $a,b\ne1$ in different factors show that every such splitting gives an [infinite group](group.md#infinite-group). The distinct normal forms $ab$ and $ba$ also show that the group is not an [abelian group](group.md#abelian-group).

###### Free product with factor generating set

↑ **Parent:** [Free product](#free-product)

For nontrivial groups $A,B$, the [Cayley graph](geometric-group-theory.md#cayley-graph) of $A*B$ with $S=(A\setminus\{1\})\cup(B\setminus\{1\})$ has the edges of the [Bass-Serre tree](geometric-group-theory.md#bass-serre-tree) as its vertices. Two such vertices are adjacent exactly when the tree edges share an endpoint. Mapping each group element to its tree-edge midpoint is an isometry on the vertex metrics and has image within distance $1/2$ of every tree point, hence gives a [quasi-isometry](geometric-group-theory.md#quasi-isometry) of metric graphs. The [normal form theorem for a free product](#normal-form-theorem-for-a-free-product) identifies $|g|_S$ with reduced syllable length. The factor subgroups have diameter one in this metric.

###### Normal form for free groups and free product of groups

↑ **Parent:** [Free product](#free-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_form_for_free_groups_and_free_product_of_groups)

A [normal form for free groups and free product of groups](#normal-form-for-free-groups-and-free-product-of-groups) represents elements by reduced words. In a [free group](geometric-group-theory.md#free-group), adjacent inverse letters cancel; in a [free product](#free-product), alternating nonidentity syllables from different factors are unique. In an [amalgamated free product](#amalgamated-free-product), chosen coset representatives produce the corresponding reduced form relative to the common subgroup.

###### Normal form theorem for a free product

↑ **Parent:** [Normal form for free groups and free product of groups](#normal-form-for-free-groups-and-free-product-of-groups)

Every element of a [free product](#free-product) $G*H$ has a unique expression $u_1\cdots u_n$ in which each $u_i$ is a nonidentity element of one factor and adjacent syllables belong to different factors. The identity corresponds to the empty word.

###### Syllable in a free product

↑ **Parent:** [Normal form theorem for a free product](#normal-form-theorem-for-a-free-product)

A syllable is a nonidentity element of one factor in a [free product](#free-product) word. A reduced normal form has successive syllables in different factors; its syllable length is the number of these elements. This length records factor elements, rather than letters in a chosen generating set.

#### Generation of a fundamental group by two open sets

↑ **Parent:** [Seifert-van Kampen theorem](#seifert-van-kampen-theorem)

If $X=U_1\cup U_2$, the sets $U_1,U_2$, and their intersection are path-connected, and the base point lies in the intersection, then $\pi_1(X)$ is generated by the images of $\pi_1(U_1)$ and $\pi_1(U_2)$. Subdivide each loop into arcs lying in cover members and join every transition point to the base point within the intersection; the inserted paths telescope.

<h4 id="fundamental-group-after-attaching-a-mobius-band">Fundamental group after attaching a Möbius band</h4>

↑ **Parent:** [Seifert-van Kampen theorem](#seifert-van-kampen-theorem)

A Möbius band retracts to its core circle, and its boundary wraps twice around the core. Attaching it to $X$ along a loop representing $w\in\pi_1(X)$ therefore adjoins a generator $x$ with relation $x^2=w$.

<h5 id="homology-after-attaching-a-mobius-band-to-the-real-projective-plane">Homology after attaching a Möbius band to the real projective plane</h5>

↑ **Parent:** [Fundamental group after attaching a Möbius band](#fundamental-group-after-attaching-a-mobius-band)

Glue the boundary of a [Möbius band](topology.md#mobius-band) to the projective line in the [real projective plane](differential-geometry.md#real-projective-plane) by a [mapping degree](homology.md#degree-of-a-continuous-mapping) $n$. The band is the [mapping cylinder](#mapping-cylinder) of the degree-two boundary covering of its core. Collapsing the connecting tree in the resulting double mapping cylinder gives a [CW complex](#cw-complex) with one vertex, edges $a,b$, and two attaching words $a^2$ and $a^{-n}b^2$. Its [cellular chain complex](homology.md#cellular-chain-complex) has degree-two boundary matrix $\left(\begin{smallmatrix}2&-n\\0&2\end{smallmatrix}\right)$. Its determinant is four, so $H_2=0$. The [Smith normal form](algebra.md#smith-normal-form) gives $H_1\cong\mathbb Z/4$ for odd $n$ and $(\mathbb Z/2)^2$ for even $n$; $H_0=\mathbb Z$ and higher [homology](homology.md) vanishes. The space cannot be [homotopy equivalent](#homotopy-inverse) to a [closed manifold](differential-geometry.md#closed-manifold): mod-two [homology](homology.md) forces a potential manifold to be a surface, and its [Euler characteristic](homology.md#euler-characteristic) is one, whereas the only such closed connected surface is the projective plane, with different integral $H_1$.

<h5 id="two-mobius-bands-attached-to-a-torus">Two Möbius bands attached to a torus</h5>

↑ **Parent:** [Fundamental group after attaching a Möbius band](#fundamental-group-after-attaching-a-mobius-band)

Attach Möbius bands to a torus along the classes $ab$ and $a^2b^3$. If their core generators are $x,y$, the resulting presentation is

$$
\langle a,b,x,y\mid[a,b],\ x^2=ab,\ y^2=a^2b^3\rangle.
$$

Because the exponent vectors $(1,1)$ and $(2,3)$ form a unimodular basis of $\mathbb Z^2$, eliminating $a,b$ gives

$$
\langle x,y\mid[x^2,y^2]=1\rangle.
$$

This group maps onto $S_3$ by $x\mapsto(12)$ and $y\mapsto(23)$, so it is nonabelian.

#### Fundamental group after attaching a 2-cell

↑ **Parent:** [Seifert-van Kampen theorem](#seifert-van-kampen-theorem)

Attaching a disc to $X$ along a based loop $\alpha$ kills precisely the normal closure of its homotopy class:

$$
\pi_1(X\cup_\alpha D^2)\cong
\pi_1(X)/\langle\!\langle[\alpha]\rangle\!\rangle.
$$

##### Presentation complex

↑ **Parent:** [Fundamental group after attaching a 2-cell](#fundamental-group-after-attaching-a-2-cell)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Presentation_complex)

A group presentation gives a two-dimensional cell complex with one vertex, one oriented loop for each generator, and one 2-cell attached along each relator. Its fundamental group is the presented group.

###### Presentation complex for the symmetric group on three letters

↑ **Parent:** [Presentation complex](#presentation-complex)

Attach three 2-cells to $S^1\vee S^1$ along loops representing $a^2$, $b^3$, and $(ab)^2$. The resulting group is

$$
\langle a,b\mid a^2,b^3,(ab)^2\rangle\cong S_3.
$$

Indeed, $a\mapsto(12)$ and $b\mapsto(123)$ gives a surjection to $S_3$, while $aba=b^{-1}$ reduces every word to one of $b^i$ or $ab^i$, so the presented group has at most six elements.

### Fundamental group of a closed orientable surface

↑ **Parent:** [Fundamental group](#fundamental-group)

For the closed orientable surface of genus $g$,

$$
\pi_1(\Sigma_g)
=\left\langle a_1,b_1,\ldots,a_g,b_g
\mathrel{\Big|}
\prod_{i=1}^g[a_i,b_i]=1\right\rangle.
$$

In particular, the sphere has trivial fundamental group and the torus has fundamental group $\mathbb Z^2$.

## Covering space

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Covering_space)

A covering map $p:\widetilde X\to X$ is locally a disjoint union of homeomorphisms onto the same evenly covered open neighbourhood.

### Semilocally simply connected space

↑ **Parent:** [Covering space](#covering-space)

A [topological space](topology.md#topological-space) is semilocally simply connected if every point has an open neighbourhood whose loops based at that point become [null-homotopic](#null-homotopic-map) in the whole space. The neighbourhood itself need not be [simply connected](#simply-connected-space). Together with [path connectedness](geometry-and-topology.md#path-connected-space) and [local path connectedness](geometry-and-topology.md#locally-path-connected-space), this condition gives the classical existence and classification of connected [covering spaces](#covering-space) by [subgroups](group.md#subgroup) of the [fundamental group](#fundamental-group).

### Riemannian covering

↑ **Parent:** [Covering space](#covering-space)

A [covering map](#covering-space) between [Riemannian manifolds](riemannian-geometry.md#riemannian-manifold) that is a [local isometry](differential-geometry.md#local-isometry). The metric on the covering manifold is the pullback of the base metric; its [deck transformations](#deck-transformation) are [isometries](riemannian-geometry.md#isometry). This local metric agreement makes the [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) commute with pullback of smooth functions.

### Homological transfer for a finite covering

↑ **Parent:** [Covering space](#covering-space)

For an $n$-sheeted [covering space](#covering-space) $f:X\to Y$, define the transfer of a [singular simplex](homology.md#singular-simplex) as the sum of its $n$ lifts. Restriction of these lifts to any face gives exactly the lifts of that face, so transfer is a [chain map](homology.md#chain-map). Its induced map $\operatorname{tr}:H_i(Y;R)\to H_i(X;R)$ satisfies $f_*\operatorname{tr}=n\,\mathrm{id}$ for any commutative coefficient ring $R$. If $n$ is invertible in $R$, then $n^{-1}\operatorname{tr}$ is a right inverse of $f_*$. In particular a finite covering surjects onto the base's rational [homology](homology.md).

### Double covers of the figure-eight space

↑ **Parent:** [Covering space](#covering-space)

There are three connected two-sheeted [covering spaces](#covering-space) of the wedge of two circles, distinguished by the three nonzero homomorphisms from its [fundamental group](#fundamental-group) to $\mathbb Z/2\mathbb Z$. If exactly one circle exchanges sheets, the covering graph has two parallel joining edges and one loop at each vertex. If both circles exchange sheets, it has four parallel joining edges. These give two homeomorphism types of total spaces even though they give three inequivalent covers of the fixed base.

### Orientation double cover

↑ **Parent:** [Covering space](#covering-space)

An oriented coordinate neighborhood of a [smooth manifold](differential-geometry.md#smooth-manifold) gives two sheets distinguished by the sign of its [orientation](#orientation-of-a-simplex). On an overlap, the sheets agree where the two local orientation forms differ by a positive function. These open agreement sets define a two-sheeted smooth [covering space](#covering-space), whose projection is locally a [diffeomorphism](geometry-and-topology.md#diffeomorphism).

#### Connectedness criterion for the orientation double cover

↑ **Parent:** [Orientation double cover](#orientation-double-cover)

For a connected [smooth manifold](differential-geometry.md#smooth-manifold), every component of the [orientation double cover](#orientation-double-cover) maps onto the base by the [path lifting theorem](#path-lifting-theorem). There can therefore be at most two components. A global [orientation](#orientation-of-a-simplex) splits the cover into two copies of the base. Conversely, if there are two components, each meets every fibre once, so its inverse projection gives a smooth global choice of [orientation](#orientation-of-a-simplex).

#### Canonical orientation of the orientation double cover

↑ **Parent:** [Orientation double cover](#orientation-double-cover)

At $(p,o)$ in the [orientation double cover](#orientation-double-cover), use the derivative of the covering projection to transport the chosen [orientation](#orientation-of-a-simplex) $o$ to the tangent space of the cover. In local oriented sheets this prescription is smooth, so it defines a global [orientation](#orientation-of-a-simplex). The involution $(p,o)\mapsto(p,-o)$ reverses it.

### Homotopy lifting theorem for a covering map

↑ **Parent:** [Covering space](#covering-space)

A homotopy into the base of a [covering space](#covering-space) has a unique continuous lift once its initial map is continuously lifted. Local inverse sheets construct the lift along each time interval, and compactness of that interval permits a finite subdivision locally around each point of the homotopy's parameter space. Uniqueness on overlapping intervals follows from [path lifting theorem](#path-lifting-theorem) uniqueness. In a homotopy of paths with endpoints fixed, a chosen lifted endpoint remains fixed because it varies continuously in a discrete fiber.

### Branched covering

↑ **Parent:** [Covering space](#covering-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Branched_covering)

A branched covering is a map that is a [covering space](#covering-space) away from a branch set and has a specified local covering model at that set. For a smooth two-fold covering branched over a codimension-two submanifold, the local model is $(z,u)\mapsto(z^2,u)$. A [two-fold branched cover of a knot](knot-theory.md#two-fold-branched-cover-of-a-knot) is the basic three-dimensional example.

#### Branched surface action from two generators

↑ **Parent:** [Branched covering](#branched-covering)

For a [finite group](group.md#finite-group) generated by $a,b$, take the regular covering of a thrice-punctured [sphere](geometry-and-topology.md#sphere) with [monodromy](complex-analysis.md#monodromy) $a,b,(ab)^{-1}$ and fill each lifted puncture by a disk. Locally the projection is $z\mapsto z^m$, where $m$ is the order of its monodromy. The result is a closed oriented [topological surface](topology.md#topological-surface) with an orientation-preserving group action. The nontrivial [stabiliser subgroups](group-theory.md#stabilizer-subgroup) are the conjugates of $\langle a\rangle$, $\langle b\rangle$ and $\langle ab\rangle$ at the three types of ramification points. Counting lifted cells gives the displayed [Euler characteristic](homology.md#euler-characteristic). A subgroup acts freely exactly when it meets every conjugate of these three cyclic groups trivially. Its quotient is then a [regular covering](#regular-covering) of degree equal to the subgroup order, and quotient [Euler characteristic](homology.md#euler-characteristic) is divided by that order.

### Infinite cyclic cover associated to an epimorphism

↑ **Parent:** [Covering space](#covering-space)

The connected [covering space](#covering-space) corresponding to $\ker\alpha$ has [deck transformation group](#deck-transformation-group) $\mathbb Z$. Choosing a deck generator makes its integral [homology](homology.md) a [module](module-theory.md#module-mathematics) over the [Laurent polynomial ring](commutative-algebra.md#laurent-polynomial-ring) $\mathbb Z[t,t^{-1}]$.

#### Alexander module of a space

↑ **Parent:** [Infinite cyclic cover associated to an epimorphism](#infinite-cyclic-cover-associated-to-an-epimorphism)

Given an integral epimorphism $\alpha:\pi_1(X)\to\mathbb Z$, the Alexander module is the first integral [homology](homology.md) of the corresponding [infinite cyclic cover associated to an epimorphism](#infinite-cyclic-cover-associated-to-an-epimorphism), with $t$ acting by its chosen [deck transformation](#deck-transformation). Its order is the greatest common divisor of maximal presentation [matrix minors](vector-space.md#minor-linear-algebra) when it is finitely presented and torsion. For the meridional epimorphism of a [knot exterior](knot-theory.md#knot-exterior), this is the [Alexander module of a knot](knot-theory.md#alexander-module-of-a-knot).

### Universal abelian cover

↑ **Parent:** [Covering space](#covering-space)

For a connected space, this is the connected covering corresponding to the kernel of the homomorphism from its [fundamental group](#fundamental-group) to its [abelianization](group-theory.md#abelianization). Its [deck transformation group](#deck-transformation-group) is $H_1(Y;\mathbb Z)$. Lifted cells make its [cellular chain complex](homology.md#cellular-chain-complex) a complex over the [group ring](commutative-algebra.md#group-ring) $\mathbb Z[H_1(Y)]$.

### Kernel cover of a real projective plane wedged with a circle

↑ **Parent:** [Covering space](#covering-space)

For $C_2*\mathbb Z\to S_3$ taking the two generators to a transposition and a $3$-cycle, the kernel's six-sheeted regular [covering space](#covering-space) consists of three spheres and two circles. Each sphere has two marked points, and each circle meets one point on each sphere. It retracts onto a rank-four [graph](graph.md) by replacing each sphere by a meridian arc, but admits no [deformation retraction](#deformation-retraction) onto any [graph](graph.md) because its degree-two [homology](homology.md) is $\mathbb Z^3$.

### Four-sheeted cover of a wedge of circles and a real projective plane

↑ **Parent:** [Covering space](#covering-space)

For $n\geq1$, map

$$
\pi_1\left(\bigvee_{i=1}^nS^1\vee\mathbb{RP}^2\right)
\longrightarrow C_2\times C_2
$$

by sending the projective-plane generator and the first circle generator to the two standard generators. The kernel defines a connected regular four-sheeted cover $\widetilde X_n$. Its lifted cellular boundary in degree two is multiplication by $1+v$ on $\mathbb Z[C_2\times C_2]$, so

$$
H_2(\widetilde X_n;\mathbb Z)\cong\mathbb Z^2.
$$

### Uniqueness of lifts to a covering space

↑ **Parent:** [Covering space](#covering-space)

Let $p:\widetilde X\to X$ be a covering map and let $Y$ be path-connected. If two lifts $\widetilde f_1,\widetilde f_2:Y\to\widetilde X$ of the same map $f:Y\to X$ agree at one point, they agree everywhere. Join that point to any other by a path and apply uniqueness in the [path lifting theorem](#path-lifting-theorem).

### Monodromy action of a covering space

↑ **Parent:** [Covering space](#covering-space)

Lifting loops based at $x_0$ permutes the fibre $p^{-1}(x_0)$ and defines the monodromy action of $\pi_1(X,x_0)$ on that fibre. A connected covering has transitive monodromy.

#### Monodromy of hyperplane sections of a smooth curve

↑ **Parent:** [Monodromy action of a covering space](#monodromy-action-of-a-covering-space)

For a nondegenerate embedded smooth [algebraic curve](algebraic-geometry.md#algebraic-curve) over the [complex numbers](complex-analysis.md#complex-number), the cover that chooses one point of a transverse hyperplane section has transitive [monodromy](complex-analysis.md#monodromy). The analogous incidence space for two distinct ordered points is irreducible, giving two-transitivity. A loop around an ordinary tangent hyperplane exchanges two intersection points. Two-transitivity conjugates this transposition to every transposition, so the [monodromy](complex-analysis.md#monodromy) is the full [symmetric group](finite-group-theory.md#symmetric-group). In particular its action on fixed-size subsets is transitive.

#### Monodromy permutation

↑ **Parent:** [Monodromy action of a covering space](#monodromy-action-of-a-covering-space)

Lifting a based loop in a [covering space](#covering-space) from every point of its finite fibre gives a permutation of that fibre. Composition of lifted loops yields the [monodromy action of a covering space](#monodromy-action-of-a-covering-space). If a closed [geodesic](riemannian-geometry.md#geodesic) of length $\ell$ has a cycle of length $m$ in its [monodromy permutation](#monodromy-permutation), the corresponding lift closes after $m$ traversals and has length $m\ell$. For a primitive base [geodesic](riemannian-geometry.md#geodesic), these cycles describe the primitive lift components.

### Deck transformation

↑ **Parent:** [Covering space](#covering-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Deck_transformation)

A deck transformation of a covering $p:\widetilde X\to X$ is a homeomorphism $g:\widetilde X\to\widetilde X$ satisfying $p\circ g=p$. Every double covering has a canonical nonidentity deck transformation that exchanges the two points in each fibre.

#### Deck transformation group

↑ **Parent:** [Deck transformation](#deck-transformation)

The deck transformation group consists of all deck transformations under composition. For a connected regular covering corresponding to a normal subgroup $H\triangleleft\pi_1(X)$, it is isomorphic to $\pi_1(X)/H$.

##### Finite groups act freely on suitable closed orientable surfaces

↑ **Parent:** [Deck transformation group](#deck-transformation-group)

If a finite [group](group.md) $G$ is generated by $h$ elements, send the $a$-generators of the genus-$h$ [surface group](#fundamental-group-of-a-surface) to those generators and its $b$-generators to the identity. The surface relation is satisfied, so this is a surjective [group homomorphism](group-theory.md#group-homomorphism). Its [kernel](linear-algebra.md#kernel-of-a-linear-map) defines a connected regular [covering space](#covering-space), on which the [deck transformation group](#deck-transformation-group) $G$ acts freely. The lifted [orientation](#orientation-of-a-simplex) and multiplicativity of the [Euler characteristic](homology.md#euler-characteristic) give genus $g=1+|G|(h-1)$.

##### Free isometric realization of a finitely generated group

↑ **Parent:** [Deck transformation group](#deck-transformation-group)

Every finitely generated group acts freely and properly discontinuously by [Riemannian isometries](differential-geometry.md#riemannian-isometry) on a connected manifold in any dimension $d\geq3$. Choose a surjection $F_r\to T$ and the [regular covering](#regular-covering) of $\#_r(S^1\times S^{d-1})$ associated with its kernel. Pulling back a metric makes the [deck transformation group](#deck-transformation-group) isometric. Uniqueness of lifts makes its action free. The cover can be noncompact and need not be [simply connected](#simply-connected-space); no claim about realizing every group as a closed three-manifold [fundamental group](#fundamental-group) is involved.

##### Deck transformation group as a monodromy centralizer

↑ **Parent:** [Deck transformation group](#deck-transformation-group)

For a connected covering, restriction to one fibre identifies the [deck transformation group](#deck-transformation-group) with the centralizer in the fibre's symmetric group of the [monodromy action of a covering space](#monodromy-action-of-a-covering-space). A deck transformation commutes with every lifted loop, and every commuting fibre permutation extends uniquely over the covering by path lifting.

#### Deck involution of a double covering

↑ **Parent:** [Deck transformation](#deck-transformation)

Every two-sheeted covering of a path-connected base has a nonidentity deck transformation that exchanges the two sheets. In monodromy terms, every subgroup of $S_2$ is centralized by its unique transposition.

#### Transfer chain map of a double covering

↑ **Parent:** [Deck transformation](#deck-transformation)

For a double covering $p:X\to Y$, the mod-two transfer sends a singular simplex of $Y$ to the sum of its two lifts. Together with the chain map $p_\#$, it gives a short exact sequence

$$
0\longrightarrow C_*(Y;\mathbb F_2)
\xrightarrow{\operatorname{tr}}C_*(X;\mathbb F_2)
\xrightarrow{p_\#}C_*(Y;\mathbb F_2)
\longrightarrow0.
$$

### Universal cover

↑ **Parent:** [Covering space](#covering-space)

A universal cover is a simply connected covering space. The universal cover of a cylinder is the plane, with the angular coordinate unwrapped to a real coordinate.

#### Universal cover of a closed three-manifold with finite fundamental group

↑ **Parent:** [Universal cover](#universal-cover)

The [universal cover](#universal-cover) of a connected [closed manifold](differential-geometry.md#closed-manifold) of dimension three with finite [fundamental group](#fundamental-group) is a closed simply connected three-manifold. It is orientable, since its orientation character has trivial domain. Its first integral [homology](homology.md) vanishes, and the [universal coefficient theorem for cohomology](cohomology.md#universal-coefficient-theorem-for-cohomology) then gives $H^1=0$. Integral [Poincare duality](cohomology.md#poincare-duality) gives $H_2=H^1=0$, while $H_0$ and $H_3$ are $\mathbb Z$. Thus it is an [integral homology sphere](cohomology.md#homology-sphere). This proof does not require classifying simply connected three-manifolds.

#### Component of a pulled-back universal cover

↑ **Parent:** [Universal cover](#universal-cover)

For a locally path-connected subspace $A\subseteq X$, a selected component of the inverse image in a [universal cover](#universal-cover) covers the corresponding component $A_0$ of $A$. Its covering [subgroup](group.md#subgroup) is $\ker(\pi_1(A,a_0)\to\pi_1(X,a_0))$; surjectivity onto all of $A$ additionally requires $A$ to be path connected.

#### Uniqueness of a universal covering space

↑ **Parent:** [Universal cover](#universal-cover)

For a path-connected locally path-connected base, any two based universal covers lift to one another. The two composites and the respective identity maps are based lifts of the same covering maps, so uniqueness of lifts makes the composites identities. The lift is therefore a homeomorphism.

#### Extension criterion into a space with contractible universal cover

↑ **Parent:** [Universal cover](#universal-cover)

Let $X$ have contractible universal cover, let $K$ be a path-connected simplicial complex, and let $i:K^1\hookrightarrow K$. A map $f:|K^1|\to X$ extends to $|K|$ exactly when its induced fundamental-group map factors through $i_*$. The factorization kills every 2-simplex boundary; all higher-dimensional boundary maps lift to the contractible universal cover and are null-homotopic.

### Classification of connected covering spaces

↑ **Parent:** [Covering space](#covering-space)

Under the usual local hypotheses, based connected coverings of $X$ correspond to subgroups of $\pi_1(X)$; changing the point above the base point conjugates the subgroup. Normal subgroups correspond to regular coverings.

#### Path-class construction of a subgroup covering

↑ **Parent:** [Classification of connected covering spaces](#classification-of-connected-covering-spaces)

For a path-connected, locally path-connected, [semilocally simply connected](#semilocally-simply-connected-space) space $X$, base point $x_0$, and [subgroup](group.md#subgroup) $H\le\pi_1(X,x_0)$, take [paths](geometry-and-topology.md#continuous-path) starting at $x_0$ modulo the relation $\alpha\sim\beta$ when their endpoints agree and $[\alpha\beta^{-1}]\in H$. Projection sends a class to its endpoint. Over a path-connected neighbourhood whose loops die in $X$, classes $[\alpha\eta]$, with $\eta$ inside that neighbourhood, form a sheet mapping homeomorphically to it. These sheets define a [covering space](#covering-space). A loop lifts closed precisely when its class belongs to $H$, so the injective induced [fundamental group](#fundamental-group) map has image $H$.

#### Regular covering

↑ **Parent:** [Classification of connected covering spaces](#classification-of-connected-covering-spaces)

A connected covering is regular when its deck transformation group acts transitively on every fibre. Under the classification of coverings, this is equivalent to the corresponding subgroup of the fundamental group being normal.

#### Degree of a connected covering

↑ **Parent:** [Classification of connected covering spaces](#classification-of-connected-covering-spaces)

For a connected covering corresponding to $H\leq\pi_1(X)$, every fibre has cardinality $[\pi_1(X):H]$.

##### Fibre bijection by path lifting

↑ **Parent:** [Degree of a connected covering](#degree-of-a-connected-covering)

If the base of a covering is path-connected, a path from $x_0$ to $x_1$ gives a bijection

$$
p^{-1}(x_0)\longrightarrow p^{-1}(x_1)
$$

by sending each initial lift point to the endpoint of its unique lifted path. Lifting the reversed path gives the inverse bijection.

#### Cell complex of a covering from a coset graph

↑ **Parent:** [Classification of connected covering spaces](#classification-of-connected-covering-spaces)

For a presentation complex, the covering associated with a subgroup has one vertex for each coset. A generator gives directed edges according to its coset action, and every relator has one lifted 2-cell beginning at each vertex.

#### Permutation covering of a wedge of circles

↑ **Parent:** [Classification of connected covering spaces](#classification-of-connected-covering-spaces)

Choose permutations $\alpha_1,\ldots,\alpha_r\in S_n$. A covering of a wedge of $r$ oriented circles has fibre $\{1,\ldots,n\}$ and an edge labelled $j$ from $i$ to $\alpha_j(i)$ above the $j$th circle. It is connected exactly when the generated permutation group is transitive, and its deck group is the centralizer of that group in $S_n$.

#### Covering-space subgroup and deck-group quotient

↑ **Parent:** [Classification of connected covering spaces](#classification-of-connected-covering-spaces)

For a connected regular covering corresponding to $H\leq\pi_1(X,x_0)$, the subgroup $H$ is normal and

$$
\pi_1(X,x_0)/H\cong\operatorname{Deck}(\widetilde X/X).
$$

The quotient acts on a fibre by endpoints of lifted loops, and regularity makes this action transitive with kernel $H$.

#### Normal covering map

↑ **Parent:** [Classification of connected covering spaces](#classification-of-connected-covering-spaces)

A connected covering is normal, or regular, when its deck transformations act transitively on each fibre. Under the subgroup classification, this is equivalent to the associated subgroup of the fundamental group being normal.

##### Universal covering map is normal

↑ **Parent:** [Normal covering map](#normal-covering-map)

A universal covering has simply connected total space, so its associated subgroup of the base fundamental group is trivial. The trivial subgroup is normal; hence every universal covering map is a [normal covering map](#normal-covering-map).

##### Forced normality of finite connected covers of orientable surfaces

↑ **Parent:** [Normal covering map](#normal-covering-map)

For a connected degree-$n$ cover of a closed orientable surface $\Sigma_g$, normality is forced when $n=1$, when $n=2$, or when $g=1$. For $g=0$, existence itself forces $n=1$. For every $g\geq2$ and $n\geq3$, nonnormal connected degree-$n$ covers exist.

###### Nonnormal finite cover of a higher-genus orientable surface

↑ **Parent:** [Forced normality of finite connected covers of orientable surfaces](#forced-normality-of-finite-connected-covers-of-orientable-surfaces)

For $g\geq2$ and $n\geq3$, send

$$
a_1\mapsto\sigma,\quad b_1\mapsto\tau,\quad
a_2\mapsto\tau,\quad b_2\mapsto\sigma,
$$

where $\sigma=(1\,2\,\cdots\,n)$ and $\tau=(1\,2)$ in $S_n$, and send all remaining surface generators to the identity. The two commutators cancel, and $\sigma,\tau$ generate $S_n$. The inverse image of a point stabilizer is a nonnormal subgroup of index $n$, hence defines a connected nonnormal degree-$n$ cover.

### Path lifting theorem

↑ **Parent:** [Covering space](#covering-space)

A path in the base of a covering has a unique lift after its initial point in the fibre is chosen. Subdivide its compact parameter interval so that each segment lies in an evenly covered set, then use the inverse sheet maps successively.

### Lifting criterion for a covering space

↑ **Parent:** [Covering space](#covering-space)

For a covering $p:(\widetilde X,\widetilde x_0)\to(X,x_0)$ and a based map $f:(Y,y_0)\to(X,x_0)$ from a path-connected locally path-connected space, a based lift $\widetilde f$ exists exactly when

$$
f_*\pi_1(Y,y_0)
\subseteq
p_*\pi_1(\widetilde X,\widetilde x_0).
$$

### Covering space action

↑ **Parent:** [Covering space](#covering-space)

An action of $G$ on $X$ is a covering space action when every point has a neighbourhood $U$ disjoint from $gU$ for every nonidentity $g$. The quotient map is then locally a covering map, although without stronger properness assumptions its quotient need not be Hausdorff.

#### Quotient of a topological group by a discrete subgroup

↑ **Parent:** [Covering space action](#covering-space-action)

If $\Gamma$ is a discrete subgroup of a [topological group](topological-group.md) $G$, then left translation by $\Gamma$ is a covering-space action. Choose an identity neighbourhood $U$ with $UU^{-1}\cap\Gamma=\{1\}$; the translates $\gamma U$ are pairwise disjoint, and the quotient map $G\to\Gamma\backslash G$ restricts to a homeomorphism on each translate.

#### Non-Hausdorff orbit space of a covering action

↑ **Parent:** [Covering space action](#covering-space-action)

On $\mathbb R^2\setminus\{0\}$, the powers of $T(x,y)=(2x,y/2)$ act freely with locally disjoint translates. Nevertheless $(2^{-n},1)\to(0,1)$ while $T^n(2^{-n},1)\to(1,0)$, so the two distinct limiting orbits cannot be separated in the quotient.

##### Simply connected non-Hausdorff orbit-space example

↑ **Parent:** [Non-Hausdorff orbit space of a covering action](#non-hausdorff-orbit-space-of-a-covering-action)

Lifting the hyperbolic-scaling action to the universal cover of $\mathbb C^*$ preserves the two inseparable limiting orbits. The covering surface is biholomorphic to $\mathbb C$, so a simply connected Riemann surface can still have a non-Hausdorff quotient by a covering space action of homeomorphisms.

## Topological group

↑ **Parent:** [Algebraic topology](algebraic-topology.md)

[This section is present in another page, follow this link to view it.](topological-group.md)

## Lefschetz number

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lefschetz_number)

$L(f)=\sum_i(-1)^i\operatorname{tr}(f_*:H_i\to H_i)$, equivalently the alternating trace on simplicial chains.

### Lefschetz coincidence number

↑ **Parent:** [Lefschetz number](#lefschetz-number)

For maps $f,g:M\to N$ between closed connected oriented manifolds of equal dimension, the rational Lefschetz coincidence number is the displayed alternating trace, using the [cohomological pushforward between closed oriented manifolds](cohomology.md#cohomological-pushforward-between-closed-oriented-manifolds). Equivalently it evaluates the pullback by $(f,g)$ of the [cohomology class of the diagonal](#cohomology-class-of-the-diagonal) on $[M]$. This formula fixes the signs with the product orientation on $N\times N$.

#### Self-coincidence number of a map of nonzero degree

↑ **Parent:** [Lefschetz coincidence number](#lefschetz-coincidence-number)

For $f:M\to N$ between closed connected oriented manifolds of equal dimension, cyclic invariance of trace and $f^!f^*=(\deg f)\mathrm{id}$ give the formula. Thus if both the degree and the target [Euler characteristic](homology.md#euler-characteristic) are nonzero, $f$ coincides somewhere with every map homotopic to it, by the [Lefschetz coincidence theorem](#lefschetz-coincidence-theorem). For target $\mathbb{CP}^{2k}$ the Euler characteristic is $2k+1$.

#### Lefschetz coincidence theorem

↑ **Parent:** [Lefschetz coincidence number](#lefschetz-coincidence-number)

A nonzero [Lefschetz coincidence number](#lefschetz-coincidence-number) forces a coincidence of the two maps. If their paired map misses the diagonal, the diagonal [Thom class](fiber-bundle.md#thom-class) restricts to zero on its image and its pullback vanishes, making the coincidence number zero. The argument works for continuous maps and requires neither isolated coincidences nor transversality.

## Lefschetz fixed-point theorem

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lefschetz_fixed-point_theorem)

If $L(f)\ne0$, then $f$ has a fixed point. For a fixed-point-free map, sufficiently fine simplicial approximation has zero diagonal chain coefficients, hence zero Lefschetz number.

### Oriented manifold retract for the Lefschetz theorem

↑ **Parent:** [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem)

A closed smooth manifold X embeds in Euclidean space. The double M of a closed tubular neighbourhood is a closed oriented [manifold](topology.md#topological-manifold) retracting onto X. If i is its inclusion and r its retraction, the fixed points of F correspond to those of f, and cyclicity of finite-dimensional trace gives $L(F)=L(f)$ from $i^*r^*=1$. Thus the oriented diagonal-class proof of the [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem) implies the theorem for possibly nonorientable X, without incorrectly treating its diagonal as cooriented.

### Fixed-point-free perturbation of a doubled-surface reflection

↑ **Parent:** [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem)

Double a compact orientable genus-zero [topological surface](topology.md#topological-surface) with $g+1$ boundary circles. The resulting closed surface has genus $g$. The [involution](group-theory.md#involution) exchanging the halves fixes the seam circles and has local collar form $(s,t)\mapsto(s,-t)$. Compose it with a flow rotating each seam coordinate by a small nonzero amount, with speed supported in its collar. Equality with the initial point would force $t=0$, where the rotation is nonzero; off the collars the original reflection already has no fixed points. The new map is fixed-point-free and homotopic to the reflection through the flow. This gives a surface example in every genus where having fixed points is not a [homotopy](#homotopy) invariant.

### Lefschetz fixed-point property of even-dimensional real projective space

↑ **Parent:** [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem)

Every self-map has $f^*a=\lambda a$ in the mod-two cohomology ring, with $\lambda\in\mathbb F_2$. Its mod-two Lefschetz number is $1+\lambda+\cdots+\lambda^{2r}$, equal to one for either value of $\lambda$. This is the reduction of the integral cellular Lefschetz number, so the latter is nonzero and a fixed point exists.

### Fixed-point-free self-maps homotopic to the identity on products of surfaces

↑ **Parent:** [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem)

Such a self-map of $\Sigma_{g_1}\times\Sigma_{g_2}$ exists exactly when one factor is a torus. Necessity follows because its [Lefschetz number](#lefschetz-number) equals the [Euler characteristic](homology.md#euler-characteristic) $4(1-g_1)(1-g_2)$ and must vanish. Sufficiency is translation by a nonzero point in the torus factor, times the identity on the other factor. The condition does not determine the product $g_1g_2$, since the other genus can be arbitrary.

### Cohomology class of the diagonal

↑ **Parent:** [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem)

Let $M$ be a closed oriented $n$-manifold, let $e_{p,i}$ be a homogeneous basis of $H^p(M;\mathbb Q)$, and choose its Poincare-dual basis $e_{p,i}^*\in H^{n-p}(M;\mathbb Q)$ by $\langle e_{p,i}e_{p,j}^*,[M]\rangle=\delta_{ij}$. With the product-orientation convention, the [Poincare dual](cohomology.md#poincare-dual) of the diagonal is

$$
\varepsilon_\Delta=\sum_{p,i}(-1)^{np}e_{p,i}^*\times e_{p,i}.
$$

#### Mod-two diagonal class of the real projective plane

↑ **Parent:** [Cohomology class of the diagonal](#cohomology-class-of-the-diagonal)

The [cohomology ring](cohomology.md#cohomology-ring) of the product of two [real projective planes](differential-geometry.md#real-projective-plane) is $\mathbb F_2[x,y]/(x^3,y^3)$, with $|x|=|y|=1$. Pairing against $x^2$, $xy$ and $y^2$ identifies the [Poincare dual](cohomology.md#poincare-dual) of the diagonal as $x^2+xy+y^2$. For a self-map $f$ with $f^*x=\varepsilon x$, the graph pullback evaluates on the mod-two [fundamental class](cohomology.md#fundamental-class) as $1+\varepsilon+\varepsilon^2=1$. Thus no graph of a map on the whole projective plane can avoid the diagonal. The argument uses a relative [Thom class](fiber-bundle.md#thom-class) and does not assume transverse intersections.

#### Graph-diagonal formula for the Lefschetz number

↑ **Parent:** [Cohomology class of the diagonal](#cohomology-class-of-the-diagonal)

For the graph map $(1,f):M\to M\times M$, the [cohomology class of the diagonal](#cohomology-class-of-the-diagonal) satisfies

$$
\left\langle(1,f)^*\varepsilon_\Delta,[M]\right\rangle
=\sum_p(-1)^p\operatorname{tr}\left(f^*:H^p(M;\mathbb Q)\to H^p(M;\mathbb Q)\right).
$$

If $f$ is fixed-point-free, its graph misses the diagonal, so the pullback vanishes. This proves the [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem) for closed oriented manifolds.

### Lefschetz number of a doubled map

↑ **Parent:** [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem)

Let $F$ be the self-map of the double $D(N)=N\cup_{\partial N}N$ induced by a self-map $f$ preserving the boundary. Naturality of the [Mayer–Vietoris sequence](#mayer-vietoris-sequence) and alternating-trace additivity give

$$
L(F)=2L(f)-L(f|_{\partial N}).
$$

### Euler-characteristic divisibility from a fixed-point-free cyclic action

↑ **Parent:** [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem)

Let $f$ have prime order $p$ on a finite CW complex, and suppose every nonidentity power is fixed-point-free. On rational homology,

$$
P_q=\frac1p\sum_{j=0}^{p-1}(f_*|_{H_q})^j
$$

is the projection onto the invariant subspace. Therefore

$$
\sum_q(-1)^q\dim H_q^{\langle f\rangle}
=\frac1p\sum_{j=0}^{p-1}L(f^j)
=\frac{\chi(X)}p.
$$

The left side is an integer, so $p$ divides $\chi(X)$.

### Cyclic point-gluing of two-spheres

↑ **Parent:** [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem)

Take $n$ labelled copies of $S^2$ and identify one marked point of copy $i$ with the antipodal marked point of copy $i+1$ cyclically. The resulting connected finite CW complex is homotopy equivalent to

$$
S^1\vee\bigvee_{i=1}^nS^2,
$$

so its rational homology has dimensions $1,1,n$ in degrees zero, one, and two, and its Euler characteristic is $n$.

### Lefschetz-Hopf fixed-point theorem

↑ **Parent:** [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem)

If a smooth self-map of a compact manifold has only isolated nondegenerate fixed points, then

$$
L(f)=\sum_{f(x)=x}\operatorname{sign}\det(I-Df_x).
$$

Every summand has absolute value one, so the number of fixed points is at least $|L(f)|$.

#### Fixed-point congruence for an involution on an odd-sphere connected sum

↑ **Parent:** [Lefschetz-Hopf fixed-point theorem](#lefschetz-hopf-fixed-point-theorem)

Let $W_g$ be a [connected sum of oriented manifolds](differential-geometry.md#connected-sum-of-oriented-manifolds) consisting of $g$ copies of $S^r\times S^r$ with odd $r\geq1$. Suppose an orientation-preserving smooth [involution](group-theory.md#involution) $f$ has finitely many fixed points, all nondegenerate with positive [determinant](linear-algebra.md#determinant) $\det(I-Df_x)$. The [Lefschetz-Hopf fixed-point theorem](#lefschetz-hopf-fixed-point-theorem) and the [cohomology ring of a connected sum of odd-dimensional sphere products](differential-geometry.md#cohomology-ring-of-a-connected-sum-of-odd-dimensional-sphere-products) give

$$
\#\operatorname{Fix}(f)=L(f)=2-\operatorname{tr}(f^*|_{H^r(W_g;\mathbb R)}).
$$

This middle group has dimension $2g$ and its [Poincare duality pairing](cohomology.md#poincare-duality-pairing) is alternating. The induced map preserves the pairing and squares to the identity. By [eigenspaces of a symplectic involution](linear-algebra.md#eigenspaces-of-a-symplectic-involution), its trace is $2g-4b$ for an integer $b$. Therefore $\#\operatorname{Fix}(f)\equiv2-2g\pmod4$.

<h2 id="mayer-vietoris-sequence">Mayer–Vietoris sequence</h2>

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mayer–Vietoris_sequence)

The Mayer–Vietoris sequence is a long exact homology sequence for a space decomposed into two suitable subspaces.

### Homology after identifying two points on a sphere

↑ **Parent:** [Mayer–Vietoris sequence](#mayer-vietoris-sequence)

Identifying two distinct points of $S^2$ produces a space with [homology groups](homology.md#homology-group) $H_0=H_1=H_2=\mathbb Z$ and all higher groups zero. Cover the identified point by the image of two small disks, a contractible wedge of disks, and take as the other open set the complement of the point, a cylinder. Their intersection is two annuli. In the [Mayer–Vietoris sequence](#mayer-vietoris-sequence), $H_1$ of this intersection maps onto $H_1$ of the cylinder with a rank-one kernel, producing $H_2=\mathbb Z$. The kernel at $H_0$ has rank one and produces $H_1=\mathbb Z$.

### Homology of two disks meeting inside a sphere

↑ **Parent:** [Mayer–Vietoris sequence](#mayer-vietoris-sequence)

Attach two disks to a simply connected space $A$ along disjoint null-homotopic boundary circles, and additionally identify one interior point of each disk. Assume the attachments are [CW complexes](#cw-complex) or admit compatible triangulations. The extra interior identification contributes a copy of $\mathbb Z$ to the first [homology group](homology.md#homology-group), in addition to the two new second-homology classes. Indeed, after the first attachment $Y=A\cup D_1$, the intersection with $D_2$ has two components, $S^1\sqcup\{p\}$. In the [Mayer–Vietoris sequence](#mayer-vietoris-sequence), the map $H_0(S^1\sqcup\{p\})\to H_0(Y)\oplus H_0(D_2)$ sends $(m,n)$ to $(m+n,-m-n)$, whose [kernel](linear-algebra.md#kernel-of-a-linear-map) is $\mathbb Z$. If $H_1(A)=0$, exactness gives $H_1(Y\cup D_2)=\mathbb Z$. The degree-two sequence is $0\to H_2(Y)\to H_2(Y\cup D_2)\to\mathbb Z\to0$, which splits because $\mathbb Z$ is free. For $A=S^3$, the integral [homology groups](homology.md#homology-group) are $\mathbb Z,\mathbb Z,\mathbb Z^2,\mathbb Z$ in degrees zero through three.

### Acyclic intersection cover homology bound

↑ **Parent:** [Mayer–Vietoris sequence](#mayer-vietoris-sequence)

If a space is a union of $n\geq2$ subcomplexes and every nonempty intersection is acyclic, its homology vanishes in degrees at least $n-1$. Induction with the [Mayer–Vietoris sequence](#mayer-vietoris-sequence) proves the bound; the boundary of an $(n-1)$-simplex covered by its facets shows sharpness.

## Simplicial complex

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplicial_complex)

A simplicial complex is a family of finite vertex sets closed under taking subsets.

### Simplicial subdivision

↑ **Parent:** [Simplicial complex](#simplicial-complex)

A simplicial subdivision replaces the [simplexes](#simplex) of a [simplicial complex](#simplicial-complex) by finitely many smaller [simplexes](#simplex) with the same underlying space, compatibly on common faces. A [piecewise linear ball](topology.md#piecewise-linear-ball) can be parametrized by a map linear on the [simplexes](#simplex) after appropriate subdivisions of its domain and target.

### Regular antipodal triangulation of a sphere

↑ **Parent:** [Simplicial complex](#simplicial-complex)

A [triangulation](#triangulation) of $S^k$ is regular in this antipodal-combinatorics convention when the [antipodal map](homology.md#antipodal-map) preserves its simplices and its nested coordinate equators $S^0\subset S^1\subset\cdots\subset S^{k-1}$ are subcomplexes. The two closed [hemispheres](geometry-and-topology.md#hemisphere) at each stage are then triangulated balls. [Barycentric subdivision](homology.md#barycentric-subdivision) preserves these conditions while making the [mesh of a simplicial complex](homology.md#mesh-of-a-simplicial-complex) arbitrarily small. This convention is distinct from other meanings of regular triangulation in polyhedral geometry. [Cambridge extremal-combinatorics notes](https://www.dpmms.cam.ac.uk/~par31/notes/extcomb.pdf) use this convention.

#### Standard simplicial decomposition of a sphere

↑ **Parent:** [Regular antipodal triangulation of a sphere](#regular-antipodal-triangulation-of-a-sphere)

The boundary [simplicial complex](#simplicial-complex) of the [cross-polytope](mathematical-optimization.md#cross-polytope) has vertices $\pm e_i$, and its faces choose at most one vertex from each opposite pair. Radial projection identifies its [geometric realization](#geometric-realization-of-a-simplicial-complex) with the round [sphere](geometry-and-topology.md#sphere) $S^n$. It is a [regular antipodal triangulation of a sphere](#regular-antipodal-triangulation-of-a-sphere) and is useful as a target for signed vertex labels: a vertex map is a [simplicial map](#simplicial-map) precisely when no edge receives opposite labels.

### Triangulation

↑ **Parent:** [Simplicial complex](#simplicial-complex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Triangulation_(topology))

A triangulation of a [topological space](topology.md#topological-space) is a [homeomorphism](topology.md#homeomorphism) from the realization of a [simplicial complex](#simplicial-complex) to that space. In [three-manifold](topology.md#3-manifold) topology, thickening its one-skeleton and the dual one-skeleton constructs a [Heegaard splitting](topology.md#heegaard-splitting).

### Vertex of a simplicial complex

↑ **Parent:** [Simplicial complex](#simplicial-complex)

An element of the underlying vertex set of an abstract [simplicial complex](#simplicial-complex); a simplex is a finite subset of these vertices. In a [barycentric subdivision](homology.md#barycentric-subdivision), the vertices are nonempty simplices of the original complex.

### Simplicial subcomplex

↑ **Parent:** [Simplicial complex](#simplicial-complex)

A simplicial subcomplex $L\subseteq K$ is a subfamily that is itself a [simplicial complex](#simplicial-complex). In particular, every face of a simplex in $L$ also lies in $L$.

### Geometric realization of a simplicial complex

↑ **Parent:** [Simplicial complex](#simplicial-complex)

The geometric realization $|K|$ glues one geometric simplex for every abstract simplex of $K$, identifying their common faces.

#### Open star in a simplicial complex

↑ **Parent:** [Geometric realization of a simplicial complex](#geometric-realization-of-a-simplicial-complex)

The open star of a vertex $v$ is the union of the relative interiors of the simplices containing $v$. The open stars of the vertices cover the geometric realization.

### Simplicial map

↑ **Parent:** [Simplicial complex](#simplicial-complex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplicial_map)

A simplicial map sends vertices to vertices and sends the vertex set of every simplex to the vertex set of a simplex. It induces a continuous map between geometric realizations and a chain map between simplicial chain complexes.

#### Positive alternating simplex

↑ **Parent:** [Simplicial map](#simplicial-map)

For a [simplicial map](#simplicial-map) to the [standard simplicial decomposition of a sphere](#standard-simplicial-decomposition-of-a-sphere), a $k$-simplex is positive alternating when its image has the displayed distinct labels. Reversing all signs makes it negative alternating. A collapsed or nonalternating simplex is neutral. Counting positive facets modulo two is the local ingredient in the [antipodal alternating-simplex parity lemma](#antipodal-alternating-simplex-parity-lemma).

##### Antipodal alternating-simplex parity lemma

↑ **Parent:** [Positive alternating simplex](#positive-alternating-simplex)

An antipodal [simplicial map](#simplicial-map) from a [regular antipodal triangulation of a sphere](#regular-antipodal-triangulation-of-a-sphere) $S^k$ to $F^n$ has an odd number of positive alternating $k$-simplices. For each $k$-simplex, the number of positive alternating facets is odd exactly when the simplex is positive or negative alternating; otherwise it is even, including collapsed images. Count these incidences in one [hemisphere](geometry-and-topology.md#hemisphere): interior facets contribute twice, boundary facets once. Antipodal pairing then gives $p_k\equiv p_{k-1}$, starting with one positive vertex on $S^0$. In particular, no such map exists when $k>n$.

#### Simplicial approximation

↑ **Parent:** [Simplicial map](#simplicial-map)

A map satisfying this condition is the object whose existence after subdivision is guaranteed by the [Simplicial approximation theorem](#simplicial-approximation-theorem).

A simplicial map $g:K\to L$ is a simplicial approximation to a continuous map $f:|K|\to|L|$ when

$$
f(\operatorname{st}_K(v))
\subseteq\operatorname{st}_L(g(v))
$$

for every vertex $v$ of $K$.

##### Straight-line homotopy from a simplicial approximation

↑ **Parent:** [Simplicial approximation](#simplicial-approximation)

If $g$ simplicially approximates $f$, then $f(x)$ and $|g|(x)$ lie in a common simplex for every $x$. The affine formula

$$
H(x,t)=(1-t)f(x)+t|g|(x)
$$

therefore remains in the realization and gives a homotopy from $f$ to $|g|$.

##### Simplicial approximation theorem

↑ **Parent:** [Simplicial approximation](#simplicial-approximation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplicial_approximation_theorem)

For a finite simplicial complex $K$, a simplicial complex $L$, and a continuous map $f:|K|\to|L|$, some [iterated barycentric subdivision](homology.md#iterated-barycentric-subdivision) $K^{(r)}$ admits a [simplicial approximation](#simplicial-approximation) to $f$. The proof applies the [Lebesgue number lemma](topology.md#lebesgue-number-lemma) to the inverse images of target open stars and uses that the [mesh of a simplicial complex](homology.md#mesh-of-a-simplicial-complex) tends to zero under repeated barycentric subdivision.

###### Lower-dimensional sphere maps are null-homotopic

↑ **Parent:** [Simplicial approximation theorem](#simplicial-approximation-theorem)

If $n<m$, every continuous map $S^n\to S^m$ is [null-homotopic](#null-homotopic-map). After simplicial approximation, its image lies in the $n$-skeleton of a triangulation of $S^m$, hence omits a point. The punctured sphere is homeomorphic to $\mathbb R^m$ and is therefore contractible.

#### Contiguous simplicial maps

↑ **Parent:** [Simplicial map](#simplicial-map)

Simplicial maps $f,g:K\to L$ are contiguous when $f(\sigma)\cup g(\sigma)$ lies in one simplex of $L$ for every simplex $\sigma$ of $K$. Contiguous maps have homotopic geometric realizations.

### Clique complex

↑ **Parent:** [Simplicial complex](#simplicial-complex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Clique_complex)

A simplicial complex is flag when every finite set of pairwise adjacent vertices spans a simplex.

Conversely, every flag complex is the [clique complex](#clique-complex) of its one-skeleton, so these two descriptions specify the same class of complexes.

### Simplex

↑ **Parent:** [Simplicial complex](#simplicial-complex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplex)

An $n$-simplex has $n+1$ affinely independent vertices.

#### Probability simplex

↑ **Parent:** [Simplex](#simplex)

The probability simplex consists of vectors of nonnegative weights summing to one. It is the [convex hull](mathematical-optimization.md#convex-hull) of the coordinate vectors. A [linear function](vector-space.md#linear-function) $r^Tx$ has maximum $\max_i r_i$ on this simplex; equality holds exactly when the weights are supported on maximizing indices.

##### Closest point of a probability simplex to the origin

↑ **Parent:** [Probability simplex](#probability-simplex)

On the [probability simplex](#probability-simplex), $\sum_i x_i=1$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $1\le\sqrt n\,\|x\|$, with equality only when all coordinates are equal. Thus the displayed [centroid](geometry-and-topology.md#centroid) is the unique closest point to the origin. It is also equidistant from all coordinate vertices, since $\|x-e_i\|^2=\|x\|^2-2x_i+1$.

#### Face of a simplex

↑ **Parent:** [Simplex](#simplex)

A face is the simplex spanned by a subset of the vertices.

#### Boundary subcomplex of a simplex

↑ **Parent:** [Simplex](#simplex)

The boundary subcomplex $\partial\Delta^n$ consists of all proper faces of the $n$-simplex. Its [geometric realization of a simplicial complex](#geometric-realization-of-a-simplicial-complex) is homeomorphic to the [sphere](geometry-and-topology.md#sphere) $S^{n-1}$, while $|\Delta^n|$ is homeomorphic to the [closed disk](topology.md#closed-disc) $D^n$.

#### Regular simplex

↑ **Parent:** [Simplex](#simplex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regular_simplex)

A regular simplex has pairwise equidistant vertices. Conversely, every finite equidistant subset of Euclidean space is the vertex set of a regular simplex.

### Orientation of a simplex

↑ **Parent:** [Simplicial complex](#simplicial-complex)

This simplicial notion is induced by an [orientation of a vector space](linear-algebra.md#orientation-of-a-vector-space) on the affine span of the simplex.

An orientation of a simplex is an ordering of its vertices modulo even permutations.

### Simplicial pseudomanifold

↑ **Parent:** [Simplicial complex](#simplicial-complex)

The geometric realization is a [pseudomanifold](topology.md#stratified-pseudomanifold) without boundary in the convention used here.

A pure $n$-dimensional simplicial complex is a pseudomanifold when every codimension-one simplex belongs to exactly two top-dimensional simplices and the top simplices are connected through shared codimension-one faces.

#### Fundamental class of an orientable simplicial pseudomanifold

↑ **Parent:** [Simplicial pseudomanifold](#simplicial-pseudomanifold)

Compatible orientations of all top-dimensional simplices make their signed sum a cycle. For a connected pseudomanifold this cycle generates top homology over the integers; if no compatible orientation exists, top integral homology is zero.

## Cone (topology)

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cone_(topology))

The cone of a [topological space](topology.md#topological-space) $X$ is $CX=(X\times[0,1])/(X\times\{0\})$, with one end collapsed to a vertex. Realization of a [simplicial cone](#simplicial-cone) gives this construction for the realized base complex.

## Simplicial cone

↑ **Parent:** [Algebraic topology](algebraic-topology.md)

Realization of the simplicial construction produces the corresponding [topological cone](#cone-topology).

The simplicial cone $v*K$ adjoins a new vertex $v$ to every simplex of $K$ and is contractible.

## Suspension (topology)

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Suspension_(topology))

The suspension is the union of two cones on a space along their common base.

### Manifold criterion for a suspension

↑ **Parent:** [Suspension (topology)](#suspension-topology)

For a nonempty [compact](topology.md#compact-space) [topological manifold](topology.md#topological-manifold) $X^d$ without boundary, its [suspension](#suspension-topology) is a topological [manifold](topology.md#topological-manifold) without boundary exactly when $X$ is homeomorphic to $S^d$. The forward implication is a [local homology from a link](homology.md#local-homology-from-a-link) calculation at a suspension vertex: $\widetilde H_j(X)$ is $\mathbb Z$ in degree $d$ and zero elsewhere. For $d\geq2$, put a coordinate ball between two nested cone neighbourhoods. The inclusion of their punctures is a [homotopy equivalence](#homotopy-equivalence) but factors through the [simply connected](#simply-connected-space) punctured ball, forcing $\pi_1(X)=0$. Thus $X$ is a [homotopy sphere](cohomology.md#homotopy-sphere), and the [topological generalized Poincare theorem](cohomology.md#topological-generalized-poincare-theorem) gives the result. The dimensions zero and one follow from the finite-set and [circle](topology.md#circle) classifications. Conversely $S(S^d)\cong S^{d+1}$. If manifolds with boundary are allowed, the interval and its disk suspension show why this formulation needs the boundary restriction.

### Suspension isomorphism

↑ **Parent:** [Suspension (topology)](#suspension-topology)

Every reduced cohomology theory has a natural suspension isomorphism

$$
\widetilde E^i(\Sigma X)\cong\widetilde E^{i-1}(X).
$$

For complex K-theory this combines with Bott periodicity to compute the theory of spheres.

### Reduced homology of a suspension

↑ **Parent:** [Suspension (topology)](#suspension-topology)

Suspension shifts reduced homology: $\widetilde H_n(\Sigma X)\cong\widetilde H_{n-1}(X)$.

### Union of cones along a common base

↑ **Parent:** [Suspension (topology)](#suspension-topology)

The union of $m$ cones on a nonempty space along one common base is homotopy equivalent to a wedge of $m-1$ suspensions of that space.

## Cohomology

↑ **Parent:** [Algebraic topology](algebraic-topology.md)

[This section is present in another page, follow this link to view it.](cohomology.md)

## Fiber bundle

↑ **Parent:** [Algebraic topology](algebraic-topology.md)

[This section is present in another page, follow this link to view it.](fiber-bundle.md)

## Complex projective space

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_projective_space)

Complex projective space is the space of complex lines through the origin in $\mathbb C^{n+1}$.

### Differential of the projective quotient map

↑ **Parent:** [Complex projective space](#complex-projective-space)

In the chart $x_j=X_j/X_0$ of [Complex projective space](#complex-projective-space), differentiate the quotient coordinates to obtain this formula for $\pi:\mathbb C^{n+1}\setminus\{0\}\to\mathbf P^n$. The kernel is the radial line $\mathbb CX$. A degree-one homogeneous vector field on the punctured cone descends to a [holomorphic vector field](complex-geometry.md#holomorphic-vector-field), since its scaling cancels the inverse scaling of $d\pi$. This gives the fiberwise construction of the [Euler sequence on complex projective space](#euler-sequence-on-complex-projective-space).

### Cellular homology of complex projective space

↑ **Parent:** [Complex projective space](#complex-projective-space)

The standard [CW complex](#cw-complex) structure on [Complex projective space](#complex-projective-space) has one cell in every even dimension from zero through $2n$, and no odd-dimensional cells. Its [cellular chain complex](homology.md#cellular-chain-complex) therefore has zero differential. The [fundamental classes](cohomology.md#fundamental-class) of the inclusions $\mathbb{CP}^j\hookrightarrow\mathbb{CP}^n$ generate its even-degree [integral homology](homology.md#integral-homology); all other groups vanish.

### Fixed-point property of even-dimensional complex projective space

↑ **Parent:** [Complex projective space](#complex-projective-space)

Every continuous self-map of $\mathbb{CP}^{2r}$ has a fixed point. If its pullback sends the integral degree-two generator to $d$ times itself, multiplicativity gives trace $d^j$ in degree $2j$. Thus its [Lefschetz number](#lefschetz-number) is $1+d+\cdots+d^{2r}$, which is positive: for $d\ne1$ it is $(1-d^{2r+1})/(1-d)>0$, and at $d=1$ it is $2r+1$. The [Lefschetz fixed-point theorem](#lefschetz-fixed-point-theorem) applies. In particular no nontrivial [finite group](group.md#finite-group) acts freely on this simply connected space.

#### Complex projective plane has no nontrivial covering quotient

↑ **Parent:** [Fixed-point property of even-dimensional complex projective space](#fixed-point-property-of-even-dimensional-complex-projective-space)

The [Complex projective plane](#complex-projective-plane) is simply connected. If it were the total space of a covering of degree at least two, it would be the [universal cover](#universal-cover) and have a nonidentity [deck transformation](#deck-transformation). Such a transformation acts by $u\mapsto\pm u$ on $H^*(\mathbb{CP}^2)=\mathbb Z[u]/(u^3)$, giving [Lefschetz number](#lefschetz-number) 1 or 3. It therefore has a fixed point, impossible for a nonidentity deck transformation.

### Polynomial multiplication map to complex projective space

↑ **Parent:** [Complex projective space](#complex-projective-space)

Identify $\mathbb{CP}^m$ with nonzero homogeneous binary forms of degree $m$, modulo nonzero scalar multiplication. Multiplication of $m$ projective linear forms gives a well-defined [holomorphic map](complex-analysis.md#holomorphic-map): no product is zero, and scaling one form scales the entire coefficient vector. A form with $m$ distinct roots has exactly $m!$ ordered factorizations. In affine root coordinates the derivative is a [Vandermonde determinant](galois-theory.md#vandermonde-determinant), nonzero at distinct roots. Each such preimage contributes $+1$ with complex [orientations](#orientation-of-a-simplex), so the [mapping degree](homology.md#degree-of-a-continuous-mapping) is $m!$. This also realizes the least positive degree allowed by the [factorial degree obstruction for products of two-spheres](#factorial-degree-obstruction-for-products-of-two-spheres).

### Complex projective plane

↑ **Parent:** [Complex projective space](#complex-projective-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_projective_plane)

The complex projective plane is the two-dimensional [Complex projective space](#complex-projective-space). Its second homology is generated by the class $H$ of a [projective line](finite-group-theory.md#projective-line), with $H^2=1$.

#### Projective lines generate a unimodular intersection form

↑ **Parent:** [Complex projective plane](#complex-projective-plane)

The [fundamental class](cohomology.md#fundamental-class) of a [complex projective line](#complex-projective-line) generates $H_2(\mathbb{CP}^2;\mathbb Z)$. Two distinct projective lines are homologous and meet at one transverse point. In complex affine coordinates their two complex tangent lines concatenate to the complex [orientation](#orientation-of-a-simplex) of the plane, so the signed intersection is $+1$. The integral [intersection form](homology.md#intersection-form) therefore has matrix $(1)$, giving a [unimodular intersection pairing](homology.md#unimodular-intersection-pairing). This computes a self-intersection through distinct representatives of the same class.

### Projective hyperplane

↑ **Parent:** [Complex projective space](#complex-projective-space)

A projective hyperplane in $\mathbb {CP}^n$ is the zero set of a nonzero complex-linear functional on $\mathbb C^{n+1}$. It is isomorphic to $\mathbb {CP}^{n-1}$ and determines a [hyperplane divisor](cartier-divisor.md#hyperplane-divisor).

### Euler sequence on complex projective space

↑ **Parent:** [Complex projective space](#complex-projective-space)

The Euler sequence is the short exact sequence of holomorphic vector bundles

$$
0\longrightarrow\mathcal O
\longrightarrow\mathcal O(1)^{\oplus(n+1)}
\longrightarrow T\mathbb{CP}^n
\longrightarrow0.
$$

Taking top exterior powers gives $\det T\mathbb{CP}^n\cong\mathcal O(n+1)$.

#### Canonical bundle of complex projective space

↑ **Parent:** [Euler sequence on complex projective space](#euler-sequence-on-complex-projective-space)

Dualizing the determinant identity in the [Euler sequence on complex projective space](#euler-sequence-on-complex-projective-space) gives

$$
K_{\mathbb{CP}^n}\cong\mathcal O(-n-1)\cong[-(n+1)H],
$$

where $H$ is a [hyperplane divisor](cartier-divisor.md#hyperplane-divisor).

##### Canonical bundle of a smooth projective hypersurface

↑ **Parent:** [Canonical bundle of complex projective space](#canonical-bundle-of-complex-projective-space)

For a smooth degree-$d$ hypersurface $X_d\subset\mathbb{CP}^n$, the [adjunction formula](complex-geometry.md#adjunction-formula) and $[X_d]\cong\mathcal O(d)$ give

$$
K_{X_d}\cong\bigl(K_{\mathbb{CP}^n}\otimes[X_d]\bigr)|_{X_d}
\cong\mathcal O_{X_d}(d-n-1).
$$

###### Canonical degree of a smooth plane curve

↑ **Parent:** [Canonical bundle of a smooth projective hypersurface](#canonical-bundle-of-a-smooth-projective-hypersurface)

For a smooth degree-$d$ [projective plane curve](algebraic-geometry.md#projective-plane-curve) $X$, the [adjunction formula](complex-geometry.md#adjunction-formula) gives $K_X\cong\mathcal O_X(d-3)$. A [hyperplane section](cartier-divisor.md#hyperplane-section) has degree $d$, so

$$
\deg K_X=d(d-3).
$$

### Complex projective line

↑ **Parent:** [Complex projective space](#complex-projective-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_projective_line)

The complex projective line is the space of complex lines in $\mathbb C^2$. It is diffeomorphic to the two-sphere and is the quotient $S^3/S^1$ in the [Hopf fibration](#hopf-fibration).

### Hopf fibration

↑ **Parent:** [Complex projective space](#complex-projective-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hopf_fibration)

The complex Hopf fibration is the principal circle bundle

$$
S^1\longrightarrow S^{2n-1}\longrightarrow\mathbb{CP}^{n-1}.
$$

It is the unit-sphere bundle of the tautological complex line bundle.

#### Hopf projection of a product smash quotient

↑ **Parent:** [Hopf fibration](#hopf-fibration)

Let $a,b\ge2$ with $a+b=2n+1$. Collapse the lower cells of $S^a\times S^b$ to obtain $q:S^a\times S^b\to S^{2n+1}$ and compose with the [Hopf fibration](#hopf-fibration) $p:S^{2n+1}\to\mathbb{CP}^n$. Both factor inclusions are killed by q, so every induced [homotopy group](#homotopy-group) map is zero; the induced [reduced homology](homology.md#reduced-homology) maps also vanish. If the composite were nullhomotopic, [homotopy lifting property](#homotopy-lifting-property) would deform q into the circle fibre. Every map from the simply connected product to that circle is nullhomotopic, contradicting the degree-one top [homology](homology.md) map of q.

#### Hopf map

↑ **Parent:** [Hopf fibration](#hopf-fibration)

The complex [Hopf fibration](#hopf-fibration) on the unit sphere of $\mathbb C^2$ sends $(z_0,z_1)$ to its complex line in $\mathbb{CP}^1\cong S^2$. Its fibres are circles. With compatible orientations, its [Hopf invariant](#hopf-invariant) is one and it generates $\pi_3(S^2)\cong\mathbb Z$.

### Cohomology ring of complex projective space

↑ **Parent:** [Complex projective space](#complex-projective-space)

If $x=c_1(\mathcal O(1))$ has degree two, then

$$
H^*(\mathbb{CP}^n;\mathbb Z)\cong\mathbb Z[x]/(x^{n+1}).
$$

Reducing coefficients modulo two gives

$$
H^*(\mathbb{CP}^n;\mathbb F_2)\cong\mathbb F_2[x]/(x^{n+1}),
\qquad |x|=2.
$$

#### Diagonal class of complex projective space

↑ **Parent:** [Cohomology ring of complex projective space](#cohomology-ring-of-complex-projective-space)

Give [Complex projective space](#complex-projective-space) its complex [orientation](#orientation-of-a-simplex). In the [homology cross product](cohomology.md#homology-cross-product) basis of $H_{2n}(\mathbb{CP}^n\times\mathbb{CP}^n;\mathbb Z)$, the [diagonal](geometry-and-topology.md#diagonal-subset) has the displayed class. If $a,b$ are the two normalized degree-two [hyperplane classes](fiber-bundle.md#hyperplane-class), its [Poincare dual](cohomology.md#poincare-dual) is $\sum_{j=0}^na^jb^{n-j}$. Indeed every degree-$2n$ monomial $a^rb^{n-r}$ restricts on the [diagonal](geometry-and-topology.md#diagonal-subset) to the top power of the hyperplane class, whose evaluation on the [fundamental class](cohomology.md#fundamental-class) is one. These evaluations determine all coefficients.

#### Factorial degree obstruction for products of two-spheres

↑ **Parent:** [Cohomology ring of complex projective space](#cohomology-ring-of-complex-projective-space)

Give $(S^2)^m$ its product [orientation](#orientation-of-a-simplex) and $\mathbb{CP}^m$ its complex [orientation](#orientation-of-a-simplex). If $u_i$ are the degree-two sphere classes and $h$ the normalized projective class, write $f^*h=\sum_i a_i u_i$. In the source [cohomology ring](cohomology.md#cohomology-ring), $u_i^2=0$ and the generators commute. Hence $f^*h^m=m!(\prod_i a_i)u_1\cdots u_m$. Evaluation on the [fundamental class](cohomology.md#fundamental-class) gives the displayed [mapping degree](homology.md#degree-of-a-continuous-mapping). Every positive degree is therefore at least $m!$, and the [polynomial multiplication map to complex projective space](#polynomial-multiplication-map-to-complex-projective-space) attains that bound.

#### Mod-two restriction from complex to real projective space

↑ **Parent:** [Cohomology ring of complex projective space](#cohomology-ring-of-complex-projective-space)

Let $i:\mathbb{RP}^d\hookrightarrow\mathbb{CP}^d$ be the standard inclusion. If $h=c_1(\mathcal O(1))\bmod2$ and $a=w_1(\gamma_d)$, then

$$
i^*h=a^2.
$$

The restricted complex [tautological bundle](fiber-bundle.md#tautological-bundle) is the [complexification of a real vector bundle](fiber-bundle.md#complexification-of-a-real-vector-bundle) $\gamma_d\otimes_{\mathbb R}\mathbb C$. Its underlying real bundle is $\gamma_d\oplus\gamma_d$. The [Whitney product formula for Stiefel–Whitney classes](fiber-bundle.md#whitney-product-formula-for-stiefel-whitney-classes) gives total class $(1+a)^2=1+a^2$, while the [Stiefel–Whitney class of the underlying real bundle of a complex line](fiber-bundle.md#stiefel-whitney-class-of-the-underlying-real-bundle-of-a-complex-line) identifies its second class with the reduced [First Chern class](complex-geometry.md#first-chern-class). Dualizing changes the integral sign but has no effect modulo two. Thus the full [induced map on cohomology](cohomology.md#induced-map-on-cohomology) sends $h^j$ to $a^{2j}$.

##### Cohomology ring of the complement of even-dimensional real projective space

↑ **Parent:** [Mod-two restriction from complex to real projective space](#mod-two-restriction-from-complex-to-real-projective-space)

For $k\geq1$, put $U=\mathbb{CP}^{2k}\setminus\mathbb{RP}^{2k}$. Its [cohomology ring](cohomology.md#cohomology-ring) is

$$
H^*(U;\mathbb F_2)\cong\mathbb F_2[x,y]/(x^k,y^2),\qquad |x|=2,\quad |y|=2k.
$$

Here $x$ is the restricted hyperplane class. The [cohomological Gysin map of an embedding](fiber-bundle.md#cohomological-gysin-map-of-an-embedding) sends $a^{2j}$ to $h^{k+j}$ and every odd-degree class to zero, by [Poincare duality](cohomology.md#poincare-duality) and [mod-two restriction from complex to real projective space](#mod-two-restriction-from-complex-to-real-projective-space). Its exact sequence gives one-dimensional groups in even degrees $0,2,\ldots,4k-2$, and zero otherwise. Choose $y$ with $\delta y=a$. The connecting-map module identity gives $\delta(x^j y)=a^{2j+1}$ for $0\leq j<k$, so these are the upper-half generators. The lower-half generators are $x^j$. The relations $x^k=0$ and $y^2=0$ follow respectively from $i_!1=h^k$ and $H^{4k}(U;\mathbb F_2)=0$. The result is a ring isomorphism with [Complex projective space](#complex-projective-space) $\mathbb{CP}^{k-1}$ times $S^{2k}$; it does not by itself assert a [homotopy equivalence](#homotopy-equivalence) of the spaces.

#### Cohomology automorphisms of a product of two complex projective spaces

↑ **Parent:** [Cohomology ring of complex projective space](#cohomology-ring-of-complex-projective-space)

For $n\geq1$, every graded-ring automorphism of

$$
H^*(\mathbb{CP}^n\times\mathbb{CP}^n;\mathbb Z)
\cong\mathbb Z[x,y]/(x^{n+1},y^{n+1})
$$

acts on $H^2$ by a signed permutation matrix. All eight such matrices are realized by independently applying complex conjugation to the factors and by interchanging the factors.

#### Cohomology ring of a collapsed projective subspace

↑ **Parent:** [Cohomology ring of complex projective space](#cohomology-ring-of-complex-projective-space)

For $0<k<n$, let $X=\mathbb{CP}^n/\mathbb{CP}^k$ and let $x_i\in H^{2i}(X;\mathbb Z)$ pull back to $x^i\in H^{2i}(\mathbb{CP}^n;\mathbb Z)$. Additively,

$$
H^q(X;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&q=0\text{ or }q=2i\text{ with }k+1\leq i\leq n,\\
0,&\text{otherwise},
\end{cases}
$$

and its positive-degree multiplication is

$$
x_ix_j=\begin{cases}x_{i+j},&i+j\leq n,\\0,&i+j>n.\end{cases}
$$

## Topological K-theory

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_K-theory)

Complex topological K-theory is the generalized cohomology theory built from stable equivalence classes of complex vector bundles. Its degree-zero group is the Grothendieck group $K^0(X)$, and its reduced theory is denoted $\widetilde K^*(X)$.

### Odd topological K-theory

↑ **Parent:** [Topological K-theory](#topological-k-theory)

For compact metric $X$, odd topological K-theory is the [homotopy](#homotopy) set of norm-continuous maps into unitaries equal to the identity modulo [compact operators](compact-operator.md) on a fixed separable infinite-dimensional [Hilbert space](hilbert-space.md). Uniform finite-rank approximation over $X$ and over [homotopies](#homotopy) gives the equivalent stable model $\operatorname{colim}_N[X,GL_N(\mathbb C)]$. Block sum gives an abelian group: a finite-dimensional unitary path swaps blocks, and a two-block rotation contracts $\operatorname{diag}(u,u^{-1})$ to the identity. On the circle the determinant winding identifies $K^1(S^1)$ with $\mathbb Z$; [Bott periodicity](#bott-isomorphism) gives $K^1(S^n)=\mathbb Z$ in odd dimensions and zero in even dimensions.

### Complex K-theory of odd-dimensional real projective space

↑ **Parent:** [Topological K-theory](#topological-k-theory)

If $L$ is the [complexification of a real vector bundle](fiber-bundle.md#complexification-of-a-real-vector-bundle) of the [tautological bundle](fiber-bundle.md#tautological-bundle) and $\mu=[L]-1$, then

$$
K^0(\mathbb{RP}^{2n+1})\cong\mathbb Z[\mu]/(\mu^2+2\mu,2^n\mu),\qquad K^{-1}(\mathbb{RP}^{2n+1})\cong\mathbb Z.
$$

Realizing [Real projective space](#real-projective-space) as the [circle bundle](fiber-bundle.md#circle-bundle) of the square of the [tautological bundle](fiber-bundle.md#tautological-bundle) on [Complex projective space](#complex-projective-space) gives this through the [K-theory Gysin sequence of a sphere bundle](#k-theory-gysin-sequence-of-a-sphere-bundle).

### K-theory transfer of a finite covering

↑ **Parent:** [Topological K-theory](#topological-k-theory)

For a finite [covering map](#covering-space) $p:Y\to X$, define the fiber of the transferred [vector bundle](fiber-bundle.md#vector-bundle) by $(p_!V)_x=\bigoplus_{y\in p^{-1}(x)}V_y$. Local trivializations of the [covering map](#covering-space) make this a [vector bundle](fiber-bundle.md#vector-bundle), and compatibility with [direct sums](vector-space.md#direct-sum) extends it to [Topological K-theory](#topological-k-theory).

#### Projection formula for the K-theory transfer

↑ **Parent:** [K-theory transfer of a finite covering](#k-theory-transfer-of-a-finite-covering)

The [K-theory transfer of a finite covering](#k-theory-transfer-of-a-finite-covering) distributes over a pulled-back [tensor product of vector bundles](fiber-bundle.md#tensor-product-of-vector-bundles):

$$
p_!(p^*a\cdot b)=a\cdot p_!b.
$$

For an $n$-sheeted [covering map](#covering-space), $p_!(1)$ is the permutation [vector bundle](fiber-bundle.md#vector-bundle) of rank $n$. Its difference from $n$ is a [nilpotent element](commutative-algebra.md#nilpotent) by [nilpotence of rank-zero K-theory classes](#nilpotence-of-rank-zero-k-theory-classes), so it is a unit after inverting $n$. Thus pullback on [Topological K-theory](#topological-k-theory) becomes injective after this [localization of a ring](commutative-algebra.md#localization-of-a-ring).

### Rank map in topological K-theory

↑ **Parent:** [Topological K-theory](#topological-k-theory)

The rank of a [vector bundle](fiber-bundle.md#vector-bundle) is locally constant on the base. Taking the difference of the ranks extends to the [Grothendieck group](#grothendieck-group) of [vector bundles](fiber-bundle.md#vector-bundle), giving the rank map in [Topological K-theory](#topological-k-theory). For a [finite CW complex](#finite-cw-complex), its kernel consists of classes of rank zero on every [connected component](geometry-and-topology.md#connected-component).

#### Nilpotence of rank-zero K-theory classes

↑ **Parent:** [Rank map in topological K-theory](#rank-map-in-topological-k-theory)

For a [finite CW complex](#finite-cw-complex), every element in the kernel of the [rank map in topological K-theory](#rank-map-in-topological-k-theory) is a [nilpotent element](commutative-algebra.md#nilpotent). One proof adjoins one positive-dimensional cell at a time: the restriction kernel is square-zero by the [relative product in topological K-theory](#relative-product-in-topological-k-theory). For [connected](geometry-and-topology.md#connected-space) spaces the rank-zero kernel is [Reduced topological K-theory](#reduced-topological-k-theory); for disconnected spaces the kernel of restriction to just one basepoint can contain nonzero [idempotents](commutative-algebra.md#idempotent).

### Relative topological K-theory

↑ **Parent:** [Topological K-theory](#topological-k-theory)

For a nonempty subcomplex $A\subset X$, relative [Topological K-theory](#topological-k-theory) is $K^i(X,A)=\widetilde K^i(X/A)$, where the collapsed subcomplex is the basepoint. It fits into the [K-theory six-term exact sequence](#k-theory-six-term-exact-sequence).

#### Relative product in topological K-theory

↑ **Parent:** [Relative topological K-theory](#relative-topological-k-theory)

The [relative topological K-theory](#relative-topological-k-theory) product

$$
K^i(X,A)\otimes K^j(X,A)\longrightarrow K^{i+j}(X,A)
$$

is induced by the reduced diagonal $X/A\to(X/A)\wedge(X/A)$. If $X/A$ is a positive-dimensional [sphere](geometry-and-topology.md#sphere), this diagonal is [null-homotopic](#null-homotopic-map), so the kernel of $K^0(X)\to K^0(A)$ is square-zero.

### K-theory six-term exact sequence

↑ **Parent:** [Topological K-theory](#topological-k-theory)

For a pair $(X,A)$ of [CW complexes](#cw-complex), [relative topological K-theory](#relative-topological-k-theory) and [Bott periodicity](#bott-isomorphism) give the cyclic [exact sequence](homology.md#exact-sequence)

$$
K^0(X,A)\to K^0(X)\to K^0(A)\to K^{-1}(X,A)\to K^{-1}(X)\to K^{-1}(A)\to K^0(X,A).
$$

### Grothendieck group

↑ **Parent:** [Topological K-theory](#topological-k-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Grothendieck_group)

The Grothendieck group of a commutative monoid is its universal abelian-group completion. For vector bundles under direct sum, its elements are formal differences $[E]-[F]$ modulo stabilization.

### Reduced topological K-theory

↑ **Parent:** [Topological K-theory](#topological-k-theory)

For a based compact space, reduced K-theory is the kernel of restriction to the basepoint. It satisfies

$$
\widetilde K^i(S^d)\cong K^{i-d}(\mathrm{pt}).
$$

### Bott isomorphism

↑ **Parent:** [Topological K-theory](#topological-k-theory)

Multiplication by the [Bott element](#bott-element) $\beta\in\widetilde K^0(S^2)$ gives the Bott isomorphism

$$
K^i(X)\xrightarrow{\ \cong\ }\widetilde K^i(S^2\wedge X)
\cong K^{i-2}(X).
$$

#### Bott element

↑ **Parent:** [Bott isomorphism](#bott-isomorphism)

The Bott element is the reduced class of the tautological complex line bundle over $S^2\cong\mathbb{CP}^1$, up to the choice of sign. Its exterior powers generate the reduced K-theory of even-dimensional spheres.

#### Complex K-theory of a sphere

↑ **Parent:** [Bott isomorphism](#bott-isomorphism)

Complex Bott periodicity gives

$$
\widetilde K^i(S^d)\cong
\begin{cases}
\mathbb Z,&i-d\text{ is even},\\
0,&i-d\text{ is odd}.
\end{cases}
$$

### Complex K-theory of an even-cell complex

↑ **Parent:** [Topological K-theory](#topological-k-theory)

If a finite CW-complex $Y$ has only even-dimensional cells, then

$$
K^{-1}(Y)=0
$$

and $K^0(Y)$ is free abelian, with one generator for each cell. This follows by induction from the six-term exact sequence for adjoining a wedge of even-dimensional cells.

<h4 id="kunneth-theorem-for-complex-k-theory-with-an-even-cell-factor">Künneth theorem for complex K-theory with an even-cell factor</h4>

↑ **Parent:** [Complex K-theory of an even-cell complex](#complex-k-theory-of-an-even-cell-complex)

If $Y$ is a finite even-cell complex, the exterior product is an isomorphism

$$
K^0(Y)\otimes K^i(X)\xrightarrow{\ \cong\ }K^i(Y\times X).
$$

Cellular induction proves this because $K^0(Y)$ is free and $K^{-1}(Y)=0$.

### Complex K-theory of complex projective space

↑ **Parent:** [Topological K-theory](#topological-k-theory)

If $t=1-[\overline\gamma]$ for the tautological complex line bundle, then

$$
K^0(\mathbb{CP}^n)\cong\mathbb Z[t]/(t^{n+1}),
\qquad
K^{-1}(\mathbb{CP}^n)=0.
$$

### Stable cancellation for complex vector bundles

↑ **Parent:** [Topological K-theory](#topological-k-theory)

Let $E_0,E_1$ be complex vector bundles of rank $d$ over a finite CW complex of dimension at most $2d$. If $E_0\oplus\mathbb C^r\cong E_1\oplus\mathbb C^r$ for some $r$, then $E_0\cong E_1$. This follows because the stabilization map $BU(d)\to BU$ is $2d$-connected, so stable equivalence is injective on bundles over such a complex.

#### Chern classes classify rank-d complex vector bundles over CPd

↑ **Parent:** [Stable cancellation for complex vector bundles](#stable-cancellation-for-complex-vector-bundles)

Two rank-$d$ complex vector bundles over $\mathbb{CP}^d$ are isomorphic exactly when their Chern classes agree. Equality of Chern classes gives equality of their [Chern characters](#chern-character); the Chern character is injective here because $K^0(\mathbb{CP}^d)$ is torsion-free. The bundles are therefore stably isomorphic, and [stable cancellation for complex vector bundles](#stable-cancellation-for-complex-vector-bundles) applies because $\mathbb{CP}^d$ has real dimension $2d$.

### K-theory Wang sequence of a mapping torus

↑ **Parent:** [Topological K-theory](#topological-k-theory)

For a self-map $f:Z\to Z$, the mapping torus has an exact sequence containing

$$
K^{-1}(Z)\xrightarrow{1-f^*}K^{-1}(Z)
\longrightarrow K^0(T_f)
\longrightarrow K^0(Z)\xrightarrow{1-f^*}K^0(Z).
$$

If $K^{-1}(Z)=0$, then $K^0(T_f)\cong\ker(1-f^*:K^0(Z)\to K^0(Z))$.

#### K-theory of the mapping torus of the factor swap on two complex projective planes

↑ **Parent:** [K-theory Wang sequence of a mapping torus](#k-theory-wang-sequence-of-a-mapping-torus)

For the factor swap on $\mathbb{CP}^2\times\mathbb{CP}^2$, the invariant subgroup of

$$
\mathbb Z[x,y]/(x^3,y^3)
$$

has basis $1,xy,x^2y^2,x+y,x^2+y^2,xy^2+x^2y$. Hence the mapping torus has $K^0\cong\mathbb Z^6$.

### Splitting principle for complex vector bundles

↑ **Parent:** [Topological K-theory](#topological-k-theory)

For a complex vector bundle $E\to X$, there is a map $p:F(E)\to X$ such that $p^*$ is injective on cohomology and $p^*E$ splits as a sum of line bundles. Symmetric identities in the Chern roots can therefore be proved after this pullback.

#### Chern root

↑ **Parent:** [Splitting principle for complex vector bundles](#splitting-principle-for-complex-vector-bundles)

If a pulled-back complex vector bundle splits as $L_1\oplus\cdots\oplus L_r$, its formal Chern roots are $x_i=c_1(L_i)$. The Chern classes are the elementary symmetric polynomials in these roots.

#### Chern character

↑ **Parent:** [Splitting principle for complex vector bundles](#splitting-principle-for-complex-vector-bundles)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chern_character)

If the formal Chern roots of $E$ are $x_1,\ldots,x_r$, then

$$
\operatorname{ch}(E)=\sum_{i=1}^r e^{x_i}.
$$

It extends to virtual bundles and is a ring homomorphism because direct sum joins root lists while tensor product replaces them by all sums $x_i+y_j$.

##### Chern character on an even-dimensional sphere is integral

↑ **Parent:** [Chern character](#chern-character)

Under the natural identification

$$
\widetilde H^{\mathrm{ev}}(S^{2n};\mathbb Z)\subset
\widetilde H^{\mathrm{ev}}(S^{2n};\mathbb Q),
$$

the Chern character maps $\widetilde K^0(S^{2n})$ into integral cohomology. A Bott generator is an exterior product of $n$ degree-two Bott elements, whose Chern characters multiply to an integral top-dimensional generator.

###### Divisibility of the top Chern number on an even-dimensional sphere

↑ **Parent:** [Chern character on an even-dimensional sphere is integral](#chern-character-on-an-even-dimensional-sphere-is-integral)

For a complex vector bundle $E\to S^{2n}$,

$$
\left\langle c_n(E),[S^{2n}]\right\rangle
$$

is divisible by $(n-1)!$. Since the lower Chern classes vanish, the Newton identity gives

$$
\operatorname{ch}_n(E)
=(-1)^{n+1}\frac{c_n(E)}{(n-1)!},
$$

and the [Chern character on an even-dimensional sphere is integral](#chern-character-on-an-even-dimensional-sphere-is-integral).

### K-theory Thom class

↑ **Parent:** [Topological K-theory](#topological-k-theory)

For a complex vector bundle $E\to X$, the K-theory Thom class

$$
\lambda_E\in\widetilde K^0(\operatorname{Th}(E))
$$

generates the Thom isomorphism $K^i(X)\cong\widetilde K^i(\operatorname{Th}(E))$.

#### K-theory Euler class

↑ **Parent:** [K-theory Thom class](#k-theory-thom-class)

Pulling the K-theory Thom class back along the zero section gives

$$
e^K(E)=\Lambda_{-1}(\overline E)
=\sum_j(-1)^j[\Lambda^j\overline E].
$$

##### K-theory Euler class of the tangent bundle of complex projective space

↑ **Parent:** [K-theory Euler class](#k-theory-euler-class)

Let $\gamma$ be the tautological line bundle and put $t=1-[\gamma]$. The [Euler sequence on complex projective space](#euler-sequence-on-complex-projective-space) gives

$$
T\mathbb{CP}^n\oplus\mathbb C\cong(n+1)\overline\gamma.
$$

Hence

$$
\lambda_s(\overline{T\mathbb{CP}^n})
=\frac{(1+s\gamma)^{n+1}}{1+s},
$$

and evaluating at $s=-1$ in $K^0(\mathbb{CP}^n)=\mathbb Z[t]/(t^{n+1})$ gives

$$
e^K(T\mathbb{CP}^n)=(n+1)[\gamma](1-[\gamma])^n=(n+1)t^n.
$$

#### K-theory Gysin sequence of a sphere bundle

↑ **Parent:** [K-theory Thom class](#k-theory-thom-class)

The cofibration $S(E)\to D(E)\to\operatorname{Th}(E)$ and the Thom isomorphism give

$$
\cdots\to K^i(X)\xrightarrow{\cdot e^K(E)}K^i(X)
\xrightarrow{p^*}K^i(S(E))
\xrightarrow{p_!}K^{i+1}(X)\to\cdots.
$$

##### K-theory of the sphere bundle of copies of a complexified real tautological line

↑ **Parent:** [K-theory Gysin sequence of a sphere bundle](#k-theory-gysin-sequence-of-a-sphere-bundle)

Let $L$ be the [complexification of a real vector bundle](fiber-bundle.md#complexification-of-a-real-vector-bundle) of the [tautological bundle](fiber-bundle.md#tautological-bundle) over [Real projective space](#real-projective-space) $\mathbb{RP}^{2n+1}$. For $k\geq1$, the [K-theory Euler class](#k-theory-euler-class) of $L^{\oplus k}$ is $-2^{k-1}([L]-1)$, and

$$
K^0(S(L^{\oplus k}))\cong\mathbb Z^2\oplus\mathbb Z/2^{\min(n,k-1)}.
$$

The [K-theory Gysin sequence of a sphere bundle](#k-theory-gysin-sequence-of-a-sphere-bundle) gives an extension by $\mathbb Z$, which splits as an [exact sequence](homology.md#exact-sequence) of [abelian groups](group.md#abelian-group).

##### K-theory of the unit tangent sphere bundle of complex projective space

↑ **Parent:** [K-theory Gysin sequence of a sphere bundle](#k-theory-gysin-sequence-of-a-sphere-bundle)

The [K-theory Gysin sequence of a sphere bundle](#k-theory-gysin-sequence-of-a-sphere-bundle) and $e^K(T\mathbb{CP}^n)=(n+1)t^n$ give

$$
K^0(S(T\mathbb{CP}^n))
\cong\mathbb Z[t]/(t^{n+1},(n+1)t^n)
\cong\mathbb Z^n\oplus\mathbb Z/(n+1),
$$

and

$$
K^{-1}(S(T\mathbb{CP}^n))
\cong\ker((n+1)t^n\cdot-)
=(t)\cong\mathbb Z^n.
$$

##### Odd K-theory of the sphere bundle of two tautological lines

↑ **Parent:** [K-theory Gysin sequence of a sphere bundle](#k-theory-gysin-sequence-of-a-sphere-bundle)

For $E=\gamma\oplus\gamma$ over $\mathbb{CP}^n$ and $t=1-[\overline\gamma]$, the K-theory Euler class is $t^2$. Hence

$$
K^{-1}(S(E))
\cong\ker(t^2:\mathbb Z[t]/(t^{n+1})\to\mathbb Z[t]/(t^{n+1}))
=\mathbb Z\{t^{n-1},t^n\}
$$

for $n\geq1$.

For $n=0$, the base is a point, the sphere bundle is $S^3$, and its odd K-theory is $\mathbb Z$.

### Adams operation

↑ **Parent:** [Topological K-theory](#topological-k-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Adams_operation)

The Adams operations are natural ring endomorphisms of complex K-theory characterized on line bundles by

$$
\psi^k([L])=[L]^k.
$$

#### Adams operation on a Bott class

↑ **Parent:** [Adams operation](#adams-operation)

If $u\in\widetilde K^0(S^{2m})$ is a [Bott element](#bott-element) generator, then

$$
\psi^q(u)=q^m u.
$$

##### Adams-operation obstruction to retracting a truncated complex projective space

↑ **Parent:** [Adams operation on a Bott class](#adams-operation-on-a-bott-class)

Let $\mathbb{CP}^{k+n}_k=\mathbb{CP}^{k+n}/\mathbb{CP}^{k-1}$. If the bottom-cell inclusion $S^{2k}=\mathbb{CP}^k_k\to\mathbb{CP}^{k+2}_k$ admits a retraction, then $24$ divides $k$. Writing $x=[\overline\gamma]-1$, a retracted Bott generator has the form $x^k+ax^{k+1}+bx^{k+2}$. Comparing it with its image under $\psi^2(x)=2x+x^2$ gives $a=-k/2$ and $b=k(3k+5)/24$; integrality forces both $3$ and $8$ to divide $k$.

#### Cannibalistic class

↑ **Parent:** [Adams operation](#adams-operation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cannibalistic_class)

The cannibalistic class is defined by

$$
\psi^k(\lambda_E)=\rho^k(E)\lambda_E.
$$

It satisfies $\rho^k(E\oplus F)=\rho^k(E)\rho^k(F)$. For a line bundle,

$$
\rho^k(L)=\frac{1-\overline L^k}{1-\overline L}
=1+\overline L+\cdots+\overline L^{k-1}.
$$

##### Adams operation and the boundary pushforward of a sphere bundle

↑ **Parent:** [Cannibalistic class](#cannibalistic-class)

For $p_!:K^{-1}(S(E))\to K^0(X)$ in the K-theory Gysin sequence,

$$
p_!(\psi^k x)=\rho^k(E)\psi^k(p_!x).
$$

This follows by applying $\psi^k$ to $\delta x=\lambda_Ep_!(x)$.

###### Second Adams operation on the odd K-theory of the sphere bundle of two tautological lines

↑ **Parent:** [Adams operation and the boundary pushforward of a sphere bundle](#adams-operation-and-the-boundary-pushforward-of-a-sphere-bundle)

Choose $a,b$ with $p_!(a)=t^{n-1}$ and $p_!(b)=t^n$, where $t=1-[\overline\gamma]$. Then

$$
\psi^2(a)=2^{n+1}a-(n+1)2^n b,
\qquad
\psi^2(b)=2^{n+2}b.
$$

## Reidemeister torsion

↑ **Parent:** [Algebraic topology](algebraic-topology.md)

For a based finite acyclic [chain complex](homology.md#chain-complex), Reidemeister torsion is an alternating product of determinants comparing each given chain basis with bases formed from boundaries and lifts of boundaries. With suitable local coefficients this gives an invariant of a space finer than its [homology](homology.md). Analytic torsion constructs a corresponding invariant from spectra of [Laplacian](calculus.md#laplacian) operators, while [Turaev torsion](knot-theory.md#turaev-torsion) refines combinatorial sign and normalization choices.

## ↑ Ancestors (4)

1. [Geometry and topology](geometry-and-topology.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
