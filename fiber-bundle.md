# Fiber bundle

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fiber_bundle)

A fiber bundle is a map $\pi:E\to B$ locally isomorphic over each open set $U\subseteq B$ to the projection $U\times F\to U$ for a fixed fiber $F$.

**Table of contents**

- [Affine bundle](#affine-bundle)
- [Section (fiber bundle)](#section-fiber-bundle)
  - [Cohomological obstruction to a section of the twistor bundle](#cohomological-obstruction-to-a-section-of-the-twistor-bundle)
- [Leray-Hirsch theorem](#leray-hirsch-theorem)
  - [Finite-cover proof of the Leray-Hirsch theorem](#finite-cover-proof-of-the-leray-hirsch-theorem)
  - [Local basis criterion for Leray-Hirsch classes](#local-basis-criterion-for-leray-hirsch-classes)
- [Local trivialization](#local-trivialization)
  - [Transition function of a vector bundle](#transition-function-of-a-vector-bundle)
    - [Structure group of a vector bundle](#structure-group-of-a-vector-bundle)
- [Circle bundle](#circle-bundle)
- [Ehresmann fibration theorem](#ehresmann-fibration-theorem)
- [Principal bundle](#principal-bundle)
  - [Principal circle bundle on real projective three-space](#principal-circle-bundle-on-real-projective-three-space)
  - [Transition function of a principal bundle](#transition-function-of-a-principal-bundle)
  - [Frame bundle](#frame-bundle)
  - [Orthonormal frame bundle](#orthonormal-frame-bundle)
    - [Oriented orthonormal frame bundle of anti-de Sitter spacetime](#oriented-orthonormal-frame-bundle-of-anti-de-sitter-spacetime)
    - [Oriented orthonormal frame bundle of Minkowski spacetime](#oriented-orthonormal-frame-bundle-of-minkowski-spacetime)
    - [Oriented frame bundle of de Sitter spacetime](#oriented-frame-bundle-of-de-sitter-spacetime)
      - [Global frame on four-dimensional de Sitter spacetime](#global-frame-on-four-dimensional-de-sitter-spacetime)
  - [Associated bundle](#associated-bundle)
  - [Principal bundle trivialization by a global section](#principal-bundle-trivialization-by-a-global-section)
  - [Associated vector bundle](#associated-vector-bundle)
    - [Adjoint bundle](#adjoint-bundle)
  - [Classifying space](#classifying-space)
    - [Rational odd-rank stabilization of orthogonal classifying spaces](#rational-odd-rank-stabilization-of-orthogonal-classifying-spaces)
    - [Classifying space of a discrete group](#classifying-space-of-a-discrete-group)
  - [General linear group modulo the unitary group](#general-linear-group-modulo-the-unitary-group)
  - [Free proper Lie-group action theorem](#free-proper-lie-group-action-theorem)
  - [Connection (principal bundle)](#connection-principal-bundle)
    - [Translational connection for a convex body rolling on a plane](#translational-connection-for-a-convex-body-rolling-on-a-plane)
    - [U(1) connection](#u-1-connection)
    - [Gauge equivalence of principal connections](#gauge-equivalence-of-principal-connections)
    - [Local principal connection form](#local-principal-connection-form)
      - [Reconstruction of a principal connection from local gauge potentials](#reconstruction-of-a-principal-connection-from-local-gauge-potentials)
    - [Horizontal distribution of a principal connection](#horizontal-distribution-of-a-principal-connection)
      - [Coordinate horizontal lifts of a principal connection](#coordinate-horizontal-lifts-of-a-principal-connection)
      - [Horizontal section of a principal bundle](#horizontal-section-of-a-principal-bundle)
      - [Holonomy](#holonomy)
        - [Reducible SU2 connection](#reducible-su2-connection)
        - [Reflection holonomy along a closed projective geodesic](#reflection-holonomy-along-a-closed-projective-geodesic)
        - [Holonomy around circular fibres](#holonomy-around-circular-fibres)
          - [Flat circular metrics with trivial holonomy](#flat-circular-metrics-with-trivial-holonomy)
        - [Riemannian holonomy group](#riemannian-holonomy-group)
          - [Holonomy representation](#holonomy-representation)
            - [Irreducible holonomy in dimension at least two has no parallel one-form](#irreducible-holonomy-in-dimension-at-least-two-has-no-parallel-one-form)
            - [Fundamental principle of Riemannian holonomy](#fundamental-principle-of-riemannian-holonomy)
    - [Canonical principal connection on the Stiefel bundle over a Grassmannian](#canonical-principal-connection-on-the-stiefel-bundle-over-a-grassmannian)
- [Vector bundle](#vector-bundle)
  - [Density bundle](#density-bundle)
    - [Riemannian volume density](#riemannian-volume-density)
  - [Tensor bundle](#tensor-bundle)
  - [G-structure on a vector bundle](#g-structure-on-a-vector-bundle)
  - [Globally generated vector bundle](#globally-generated-vector-bundle)
    - [Global generation of positive twists on a smooth curve](#global-generation-of-positive-twists-on-a-smooth-curve)
    - [Nowhere-vanishing section of a globally generated bundle on a curve](#nowhere-vanishing-section-of-a-globally-generated-bundle-on-a-curve)
  - [Whitney sum of vector bundles](#whitney-sum-of-vector-bundles)
  - [Symplectic vector bundle](#symplectic-vector-bundle)
    - [Lagrangian subbundle](#lagrangian-subbundle)
  - [Thom space](#thom-space)
    - [Projective-space quotient as a Thom space of conjugate tautological lines](#projective-space-quotient-as-a-thom-space-of-conjugate-tautological-lines)
  - [Line subbundle](#line-subbundle)
  - [Birkhoff–Grothendieck theorem](#birkhoff-grothendieck-theorem)
  - [Stable framing of a vector bundle](#stable-framing-of-a-vector-bundle)
  - [Endomorphism bundle](#endomorphism-bundle)
  - [Exterior power of a vector bundle](#exterior-power-of-a-vector-bundle)
  - [Clutching construction](#clutching-construction)
    - [Clutching function](#clutching-function)
      - [Section obstruction for a clutched vector bundle](#section-obstruction-for-a-clutched-vector-bundle)
  - [Clifford module bundle](#clifford-module-bundle)
  - [Determinant line bundle](#determinant-line-bundle)
  - [Zero section of a vector bundle](#zero-section-of-a-vector-bundle)
  - [Fiber metric](#fiber-metric)
    - [Orthogonal structure on a real vector bundle](#orthogonal-structure-on-a-real-vector-bundle)
      - [Euclidean orthonormal frame](#euclidean-orthonormal-frame)
      - [Orthogonal local trivialization](#orthogonal-local-trivialization)
  - [Eigenbundle](#eigenbundle)
  - [Hermitian vector bundle](#hermitian-vector-bundle)
  - [Complex vector bundle](#complex-vector-bundle)
    - [Hermitian metric on a smooth complex vector bundle](#hermitian-metric-on-a-smooth-complex-vector-bundle)
    - [Stable complex structure on a real vector bundle](#stable-complex-structure-on-a-real-vector-bundle)
    - [Conjugate vector bundle](#conjugate-vector-bundle)
      - [Conjugate connection](#conjugate-connection)
  - [Rank of a vector bundle](#rank-of-a-vector-bundle)
  - [Vector bundle morphism](#vector-bundle-morphism)
    - [Kernel bundle of a surjective vector bundle morphism](#kernel-bundle-of-a-surjective-vector-bundle-morphism)
    - [Vector bundle endomorphism](#vector-bundle-endomorphism)
    - [Holomorphic bundle map](#holomorphic-bundle-map)
    - [Bundle morphisms from maps of smooth sections](#bundle-morphisms-from-maps-of-smooth-sections)
    - [Vector bundle isomorphism](#vector-bundle-isomorphism)
  - [Vector bundle trivialization](#vector-bundle-trivialization)
    - [Frame of a vector bundle](#frame-of-a-vector-bundle)
      - [Pseudo-orthonormal frame](#pseudo-orthonormal-frame)
      - [Coframe](#coframe)
  - [Complexification of a real vector bundle](#complexification-of-a-real-vector-bundle)
  - [Projective bundle](#projective-bundle)
    - [Projectivization by quotients](#projectivization-by-quotients)
      - [Universal quotient line bundle](#universal-quotient-line-bundle)
      - [Rational normal scroll](#rational-normal-scroll)
        - [Fiber class of a rational normal scroll](#fiber-class-of-a-rational-normal-scroll)
        - [Isomorphism classification of abstract rational scrolls](#isomorphism-classification-of-abstract-rational-scrolls)
    - [Chern classes of a tautological-line complement](#chern-classes-of-a-tautological-line-complement)
    - [Holomorphic projectivization by lines](#holomorphic-projectivization-by-lines)
      - [Relative tautological line bundle](#relative-tautological-line-bundle)
        - [Relative hyperplane line bundle](#relative-hyperplane-line-bundle)
    - [Sections of a projective bundle](#sections-of-a-projective-bundle)
    - [Orthogonal complex line flag manifold](#orthogonal-complex-line-flag-manifold)
      - [Cohomology ring of the orthogonal complex line flag manifold](#cohomology-ring-of-the-orthogonal-complex-line-flag-manifold)
    - [Projective bundle formula for complex vector bundles](#projective-bundle-formula-for-complex-vector-bundles)
  - [Complex line bundle](#complex-line-bundle)
    - [Smooth exponential sequence](#smooth-exponential-sequence)
    - [Smooth classification of complex line bundles on the complex projective line](#smooth-classification-of-complex-line-bundles-on-the-complex-projective-line)
  - [Real line bundle](#real-line-bundle)
    - [Möbius line bundle](#mobius-line-bundle)
    - [Classification of real line bundles](#classification-of-real-line-bundles)
    - [Mod-two Euler class of a real line bundle](#mod-two-euler-class-of-a-real-line-bundle)
  - [Vector subbundle](#vector-subbundle)
    - [Orthogonal splitting of a vector subbundle](#orthogonal-splitting-of-a-vector-subbundle)
    - [Quotient vector bundle](#quotient-vector-bundle)
      - [Universal quotient bundle on a real Grassmannian](#universal-quotient-bundle-on-a-real-grassmannian)
        - [Universal quotient bundle need not have a nowhere-zero section](#universal-quotient-bundle-need-not-have-a-nowhere-zero-section)
        - [Classification of vector bundles by a universal quotient bundle](#classification-of-vector-bundles-by-a-universal-quotient-bundle)
  - [Trivial vector bundle](#trivial-vector-bundle)
  - [Section of a vector bundle](#section-of-a-vector-bundle)
    - [Regular zero locus](#regular-zero-locus)
    - [Module of smooth sections](#module-of-smooth-sections)
    - [Nowhere-zero section](#nowhere-zero-section)
      - [Nonvanishing tangent field on an odd-dimensional sphere](#nonvanishing-tangent-field-on-an-odd-dimensional-sphere)
      - [Splitting a trivial line from a nowhere-zero section](#splitting-a-trivial-line-from-a-nowhere-zero-section)
      - [Hairy ball theorem](#hairy-ball-theorem)
        - [Degree proof of the hairy ball theorem](#degree-proof-of-the-hairy-ball-theorem)
  - [Sphere bundle](#sphere-bundle)
    - [Three-sphere bundle over the four-sphere](#three-sphere-bundle-over-the-four-sphere)
    - [Unit tangent bundle](#unit-tangent-bundle)
      - [Canonical coframe of a surface unit tangent bundle](#canonical-coframe-of-a-surface-unit-tangent-bundle)
        - [Vertical vector field of a surface unit tangent bundle](#vertical-vector-field-of-a-surface-unit-tangent-bundle)
        - [Liouville volume of a surface geodesic flow](#liouville-volume-of-a-surface-geodesic-flow)
      - [Stiefel manifold](#stiefel-manifold)
        - [Unordered Stiefel bundle](#unordered-stiefel-bundle)
          - [Subset cover of a framed vector bundle](#subset-cover-of-a-framed-vector-bundle)
        - [Complex Stiefel manifold](#complex-stiefel-manifold)
          - [Integral cohomology of a complex Stiefel manifold](#integral-cohomology-of-a-complex-stiefel-manifold)
          - [Complement bundle on a complex Stiefel manifold](#complement-bundle-on-a-complex-stiefel-manifold)
      - [Cohomology of the unit tangent bundle of an even-dimensional sphere](#cohomology-of-the-unit-tangent-bundle-of-an-even-dimensional-sphere)
  - [Disk bundle](#disk-bundle)
    - [Plumbing of oriented disk bundles](#plumbing-of-oriented-disk-bundles)
  - [Tangent bundle](#tangent-bundle)
    - [Stabilized tangent bundle of real projective space](#stabilized-tangent-bundle-of-real-projective-space)
    - [Tangent coordinate transition](#tangent-coordinate-transition)
  - [Projectivization of a real vector bundle](#projectivization-of-a-real-vector-bundle)
    - [Tangent bundle of a projectivized real vector bundle](#tangent-bundle-of-a-projectivized-real-vector-bundle)
    - [Projectivization of copies of the real tautological line bundle](#projectivization-of-copies-of-the-real-tautological-line-bundle)
  - [Dual bundle](#dual-bundle)
    - [Canonical trivialization of a line bundle tensored with its dual](#canonical-trivialization-of-a-line-bundle-tensored-with-its-dual)
  - [Pullback vector bundle](#pullback-vector-bundle)
    - [Pullback tangent bundle](#pullback-tangent-bundle)
      - [Vector field along a map](#vector-field-along-a-map)
        - [Local extension of a vector field along a submanifold](#local-extension-of-a-vector-field-along-a-submanifold)
        - [Vector field along a curve](#vector-field-along-a-curve)
  - [Kernel bundle of a constant-rank family of linear maps](#kernel-bundle-of-a-constant-rank-family-of-linear-maps)
  - [Tensor product of vector bundles](#tensor-product-of-vector-bundles)
    - [Second Chern class of a tensor product of rank-two bundles](#second-chern-class-of-a-tensor-product-of-rank-two-bundles)
    - [Tensor field](#tensor-field)
      - [Lie derivative of a covariant tensor field](#lie-derivative-of-a-covariant-tensor-field)
      - [Tensoriality](#tensoriality)
      - [Tensor derivation](#tensor-derivation)
        - [Lie derivative of a tensor field](#lie-derivative-of-a-tensor-field)
          - [Lie derivative at a zero of its generator](#lie-derivative-at-a-zero-of-its-generator)
          - [Coordinate tensor Lie derivative](#coordinate-tensor-lie-derivative)
          - [Commutator identity for Lie derivatives](#commutator-identity-for-lie-derivatives)
          - [Lie derivative of a vector field](#lie-derivative-of-a-vector-field)
          - [Lie derivative of a function](#lie-derivative-of-a-function)
          - [Flow definition of the Lie derivative of a tensor field](#flow-definition-of-the-lie-derivative-of-a-tensor-field)
          - [Scaled Lie derivative defect identity](#scaled-lie-derivative-defect-identity)
        - [Endomorphism-induced tensor derivation](#endomorphism-induced-tensor-derivation)
  - [Connection (vector bundle)](#connection-vector-bundle)
    - [Parallel vector field](#parallel-vector-field)
    - [Projection connection](#projection-connection)
    - [Connection difference as an endomorphism-valued one-form](#connection-difference-as-an-endomorphism-valued-one-form)
    - [Change of frame of a vector-bundle connection](#change-of-frame-of-a-vector-bundle-connection)
    - [Affine space of vector-bundle connections](#affine-space-of-vector-bundle-connections)
    - [Construction of a vector bundle connection by a partition of unity](#construction-of-a-vector-bundle-connection-by-a-partition-of-unity)
    - [Determinant connection](#determinant-connection)
    - [Rough Laplacian](#rough-laplacian)
    - [Affine connection](#affine-connection)
      - [Projective equivalence of affine connections](#projective-equivalence-of-affine-connections)
        - [Geodesic reparametrization under projective equivalence](#geodesic-reparametrization-under-projective-equivalence)
        - [Projective covector from metric volume densities](#projective-covector-from-metric-volume-densities)
      - [Bracket connection on a Lie group](#bracket-connection-on-a-lie-group)
      - [Connection components](#connection-components)
      - [Affine exponential map](#affine-exponential-map)
        - [Affine normal coordinates](#affine-normal-coordinates)
      - [Affine connection decomposition](#affine-connection-decomposition)
      - [Nonmetricity tensor](#nonmetricity-tensor)
        - [Disformation tensor](#disformation-tensor)
      - [Torsion tensor](#torsion-tensor)
        - [Contorsion tensor](#contorsion-tensor)
      - [Parallel covector field](#parallel-covector-field)
      - [Projected ambient connection](#projected-ambient-connection)
      - [Difference of affine connections is a tensor](#difference-of-affine-connections-is-a-tensor)
        - [Parametrized geodesics determine the symmetric part of an affine connection](#parametrized-geodesics-determine-the-symmetric-part-of-an-affine-connection)
          - [Torsion-free connections are determined by their parametrized geodesics](#torsion-free-connections-are-determined-by-their-parametrized-geodesics)
      - [Affine connection for a velocity-linear force](#affine-connection-for-a-velocity-linear-force)
      - [Product affine connection](#product-affine-connection)
        - [Curvature splitting for a product connection](#curvature-splitting-for-a-product-connection)
    - [Covariant derivative along a curve](#covariant-derivative-along-a-curve)
    - [Connection one-form](#connection-one-form)
    - [Exterior covariant derivative](#exterior-covariant-derivative)
      - [Endomorphism-valued exterior product](#endomorphism-valued-exterior-product)
    - [Horizontal subspace of a vector bundle connection](#horizontal-subspace-of-a-vector-bundle-connection)
      - [Linear horizontal distribution on a vector bundle](#linear-horizontal-distribution-on-a-vector-bundle)
      - [Horizontal connection associated to a covariant derivative](#horizontal-connection-associated-to-a-covariant-derivative)
    - [Pullback connection](#pullback-connection)
      - [Curvature of a pullback connection](#curvature-of-a-pullback-connection)
      - [Restriction of a connection to an embedded submanifold](#restriction-of-a-connection-to-an-embedded-submanifold)
    - [Dual connection](#dual-connection)
    - [Tensor product connection](#tensor-product-connection)
      - [Curvature of a tensor product connection](#curvature-of-a-tensor-product-connection)
    - [Endomorphism bundle connection](#endomorphism-bundle-connection)
      - [Commutator identity for an endomorphism connection](#commutator-identity-for-an-endomorphism-connection)
      - [Curvature of an endomorphism bundle connection](#curvature-of-an-endomorphism-bundle-connection)
        - [Scalar-curvature criterion for a flat endomorphism connection](#scalar-curvature-criterion-for-a-flat-endomorphism-connection)
    - [Solder form](#solder-form)
      - [Torsion form](#torsion-form)
        - [Cartan first structure equation with input-first indices](#cartan-first-structure-equation-with-input-first-indices)
        - [Torsion-free connection](#torsion-free-connection)
    - [Metric connection](#metric-connection)
      - [Metric compatibility](#metric-compatibility)
        - [Lie derivative of a metric with nonmetricity](#lie-derivative-of-a-metric-with-nonmetricity)
      - [Normal connection](#normal-connection)
      - [Skew-adjoint difference criterion for metric connections](#skew-adjoint-difference-criterion-for-metric-connections)
      - [Smooth unitary frame for a Hermitian connection](#smooth-unitary-frame-for-a-hermitian-connection)
      - [Parallel transport preserves a fibre metric](#parallel-transport-preserves-a-fibre-metric)
      - [Connection matrix in an orthonormal frame is skew-symmetric](#connection-matrix-in-an-orthonormal-frame-is-skew-symmetric)
      - [Koszul formula](#koszul-formula)
        - [Existence and uniqueness of the Levi-Civita connection](#existence-and-uniqueness-of-the-levi-civita-connection)
      - [Unitary connection](#unitary-connection)
        - [Uhlenbeck small-energy Coulomb gauge](#uhlenbeck-small-energy-coulomb-gauge)
        - [Harmonic-curvature unitary line connection](#harmonic-curvature-unitary-line-connection)
        - [Unitary bundle gauge transformation](#unitary-bundle-gauge-transformation)
          - [Unitary bundle gauge group](#unitary-bundle-gauge-group)
            - [Coulomb slice for unitary connections](#coulomb-slice-for-unitary-connections)
            - [Based unitary gauge group](#based-unitary-gauge-group)
        - [Anti-self-dual connection](#anti-self-dual-connection)
          - [Abelian anti-self-dual connections from harmonic scalar potentials](#abelian-anti-self-dual-connections-from-harmonic-scalar-potentials)
          - [ASD deformation complex](#asd-deformation-complex)
            - [Local cone at an unobstructed reducible SU2 instanton](#local-cone-at-an-unobstructed-reducible-su2-instanton)
            - [ASD deformation index](#asd-deformation-index)
          - [Uhlenbeck-Donaldson compactness for charge-one ASD connections](#uhlenbeck-donaldson-compactness-for-charge-one-asd-connections)
          - [Uhlenbeck removable singularity theorem for ASD connections](#uhlenbeck-removable-singularity-theorem-for-asd-connections)
          - [Positive-square obstruction to ASD line connections](#positive-square-obstruction-to-asd-line-connections)
    - [Horizontal lift](#horizontal-lift)
      - [Parallel transport](#parallel-transport)
        - [Parallel vector field along a curve](#parallel-vector-field-along-a-curve)
        - [Parallel transport around a spherical triangle](#parallel-transport-around-a-spherical-triangle)
        - [Global continuation of linear parallel transport](#global-continuation-of-linear-parallel-transport)
        - [Parallel frame along a curve](#parallel-frame-along-a-curve)
        - [Parallel transport on an endomorphism bundle](#parallel-transport-on-an-endomorphism-bundle)
        - [Parallel transport around a latitude of the unit sphere](#parallel-transport-around-a-latitude-of-the-unit-sphere)
  - [Orientation of a vector bundle](#orientation-of-a-vector-bundle)
    - [Orientability of a vector bundle total space](#orientability-of-a-vector-bundle-total-space)
    - [Canonical orientation of a complex vector bundle](#canonical-orientation-of-a-complex-vector-bundle)
    - [Thom class](#thom-class)
      - [Cohomology class of a cooriented submanifold](#cohomology-class-of-a-cooriented-submanifold)
      - [Thom class in a generalized cohomology theory](#thom-class-in-a-generalized-cohomology-theory)
      - [Cup square of a Thom class](#cup-square-of-a-thom-class)
      - [Thom isomorphism theorem](#thom-isomorphism-theorem)
        - [Gysin sequence of an embedding](#gysin-sequence-of-an-embedding)
          - [Cohomological Gysin map of an embedding](#cohomological-gysin-map-of-an-embedding)
      - [Euler class of a vector bundle](#euler-class-of-a-vector-bundle)
        - [Euler class in a generalized cohomology theory](#euler-class-in-a-generalized-cohomology-theory)
          - [A nowhere-zero section annihilates generalized Euler classes](#a-nowhere-zero-section-annihilates-generalized-euler-classes)
        - [Euler class of a complex vector bundle](#euler-class-of-a-complex-vector-bundle)
        - [Euler class of an oriented odd-rank vector bundle is two-torsion](#euler-class-of-an-oriented-odd-rank-vector-bundle-is-two-torsion)
        - [Whitney product formula for Euler classes](#whitney-product-formula-for-euler-classes)
        - [Euler number of a vector bundle](#euler-number-of-a-vector-bundle)
        - [Poincaré-Hopf theorem](#poincare-hopf-theorem)
        - [Euler class of a complex line bundle](#euler-class-of-a-complex-line-bundle)
        - [Gysin sequence of a sphere bundle](#gysin-sequence-of-a-sphere-bundle)
          - [Gysin ring splitting for an odd-dimensional sphere bundle](#gysin-ring-splitting-for-an-odd-dimensional-sphere-bundle)
          - [Projection formula for sphere bundle integration](#projection-formula-for-sphere-bundle-integration)
          - [Unoriented Gysin sequence](#unoriented-gysin-sequence)
          - [Three-dimensional lens space as a circle bundle](#three-dimensional-lens-space-as-a-circle-bundle)
          - [Integral cohomology of a circle bundle over a product of two spheres](#integral-cohomology-of-a-circle-bundle-over-a-product-of-two-spheres)
  - [Tautological bundle](#tautological-bundle)
    - [Complex tautological bundle on a Grassmannian](#complex-tautological-bundle-on-a-grassmannian)
      - [Classification of complex vector bundles by a Grassmannian](#classification-of-complex-vector-bundles-by-a-grassmannian)
        - [Rank-two complex vector bundles over the four-sphere](#rank-two-complex-vector-bundles-over-the-four-sphere)
        - [Close orthogonal projections identify their image bundles](#close-orthogonal-projections-identify-their-image-bundles)
        - [Finite-dimensional embedding of a complex vector bundle](#finite-dimensional-embedding-of-a-complex-vector-bundle)
    - [Complex tautological line bundle](#complex-tautological-line-bundle)
      - [Punctured line bundles do not determine their duality sign](#punctured-line-bundles-do-not-determine-their-duality-sign)
      - [Unitary transitions of the tautological line over the projective line](#unitary-transitions-of-the-tautological-line-over-the-projective-line)
      - [Global holomorphic sections of the complex tautological line bundle vanish](#global-holomorphic-sections-of-the-complex-tautological-line-bundle-vanish)
      - [Hyperplane line bundle](#hyperplane-line-bundle)
        - [Hyperplane class](#hyperplane-class)
        - [Nontrivial hyperplane powers on a compact projective submanifold](#nontrivial-hyperplane-powers-on-a-compact-projective-submanifold)
        - [Tensor powers of the hyperplane line bundle](#tensor-powers-of-the-hyperplane-line-bundle)
    - [Quaternionic tautological line bundle](#quaternionic-tautological-line-bundle)
    - [Real tautological line bundle](#real-tautological-line-bundle)
  - [Stiefel–Whitney class](#stiefel-whitney-class)
    - [Parity of zeros of a real line-bundle section](#parity-of-zeros-of-a-real-line-bundle-section)
    - [Codimension-one Stiefel–Whitney immersion obstruction](#codimension-one-stiefel-whitney-immersion-obstruction)
    - [Stiefel–Whitney class of the underlying real bundle of a complex line](#stiefel-whitney-class-of-the-underlying-real-bundle-of-a-complex-line)
    - [Projective bundle definition of Stiefel–Whitney classes](#projective-bundle-definition-of-stiefel-whitney-classes)
    - [Splitting principle for real vector bundles](#splitting-principle-for-real-vector-bundles)
      - [Whitney product formula for Stiefel–Whitney classes](#whitney-product-formula-for-stiefel-whitney-classes)
        - [Stiefel–Whitney obstruction to a diagonal projective immersion](#stiefel-whitney-obstruction-to-a-diagonal-projective-immersion)
    - [Bockstein of a Stiefel–Whitney class](#bockstein-of-a-stiefel-whitney-class)
    - [First Stiefel–Whitney class of a tensor product of real line bundles](#first-stiefel-whitney-class-of-a-tensor-product-of-real-line-bundles)
    - [Total Stiefel–Whitney class of the projectivization of copies of the tautological line](#total-stiefel-whitney-class-of-the-projectivization-of-copies-of-the-tautological-line)
- [Curvature form](#curvature-form)
  - [Curvature of a principal connection](#curvature-of-a-principal-connection)
    - [Flat principal connection](#flat-principal-connection)
  - [Trace of vector-bundle curvature](#trace-of-vector-bundle-curvature)
  - [Cartan curvature matrix equation](#cartan-curvature-matrix-equation)
    - [Cartan curvature equation with input indices](#cartan-curvature-equation-with-input-indices)
  - [Riemannian curvature two-form](#riemannian-curvature-two-form)
  - [Curvature difference formula](#curvature-difference-formula)
    - [Trace curvature transgression](#trace-curvature-transgression)
      - [Connection-independent curvature class of a line bundle](#connection-independent-curvature-class-of-a-line-bundle)
  - [Bianchi identity](#bianchi-identity)

## Affine bundle

↑ **Parent:** [Fiber bundle](fiber-bundle.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affine_bundle)

A [fiber bundle](fiber-bundle.md) whose fibers are [affine spaces](geometry-and-topology.md#affine-space) and whose transition functions are affine. Differences of points in one fiber lie in a corresponding model [vector bundle](#vector-bundle), but there need not be a preferred zero in each fiber.

## Section (fiber bundle)

↑ **Parent:** [Fiber bundle](fiber-bundle.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Section_(fiber_bundle))

A section of a [fiber bundle](fiber-bundle.md) $\pi:E\to B$ is a continuous map $s:B\to E$ with $\pi\circ s=\mathrm{id}_B$. It chooses a point of each fibre continuously. A [section of a vector bundle](#section-of-a-vector-bundle) is the special case for vector fibres; a [projective bundle](#projective-bundle) section chooses a line in each fibre of the underlying [vector bundle](#vector-bundle).

### Cohomological obstruction to a section of the twistor bundle

↑ **Parent:** [Section (fiber bundle)](#section-fiber-bundle)

If the displayed [fiber bundle](fiber-bundle.md) had a section $s$, its projection $p$ would satisfy $s^*p^*=1$. The [cohomology ring of complex projective space](algebraic-topology.md#cohomology-ring-of-complex-projective-space) is $\mathbb Z[h]/(h^4)$ with $|h|=2$. For a generator $u\in H^4(S^4;\mathbb Z)$, write $p^*u=mh^2$. But $s^*h=0$ since $H^2(S^4;\mathbb Z)=0$, giving $u=s^*p^*u=0$. This contradiction proves that no section exists, without needing the value of $m$.

## Leray-Hirsch theorem

↑ **Parent:** [Fiber bundle](fiber-bundle.md)

For a [fiber bundle](fiber-bundle.md) $\pi:E\to B$ admitting a finite trivializing open cover, whose fiber has finite free [cohomology](cohomology.md) over $R$, suppose classes $e_j\in H^*(E;R)$ restrict to a basis on every fiber. Then multiplication $a\otimes e_j\mapsto\pi^*a\smile e_j$ gives the indicated module isomorphism. A finite trivializing open cover suffices, by the local [Künneth theorem](cohomology.md#kunneth-theorem) and the [Mayer–Vietoris sequence](algebraic-topology.md#mayer-vietoris-sequence). This determines an additive module structure; multiplicative relations must still be computed. Powers of the hyperplane class on a complex [projective bundle](#projective-bundle) provide an important application.

### Finite-cover proof of the Leray-Hirsch theorem

↑ **Parent:** [Leray-Hirsch theorem](#leray-hirsch-theorem)

For global [cohomology classes](cohomology.md#cohomology-class) satisfying the [local basis criterion for Leray-Hirsch classes](#local-basis-criterion-for-leray-hirsch-classes), multiplication commutes with the [Mayer–Vietoris sequence](algebraic-topology.md#mayer-vietoris-sequence), including its connecting homomorphism: multiply cochains on the right by global cocycle representatives. Induct over a finite trivializing open cover. If $U$ is a union of $r-1$ patches and $V$ is the last patch, $U\cap V$ has a cover by at most $r-1$ trivialized intersections. The induction hypothesis on $U$, $V$ and $U\cap V$, followed by the [Five lemma](category-theory.md#five-lemma), proves the theorem on $U\cup V$. A [compact](topology.md#compact-space) base supplies the finite cover.

### Local basis criterion for Leray-Hirsch classes

↑ **Parent:** [Leray-Hirsch theorem](#leray-hirsch-theorem)

On a trivialized [fiber bundle](fiber-bundle.md) over $U$, assume the fiber has finite-dimensional total [cohomology](cohomology.md) over a [field](algebra.md#field). The [Künneth theorem](cohomology.md#kunneth-theorem) identifies the total-space cohomology with a finite free graded module over $H^*(U)$. Classes restricting to a basis on every fiber give an invertible change of generators: its degree-zero coefficient blocks are invertible on each path component, while its positive-base-degree terms strictly decrease fiber degree and are therefore nilpotent. Inverting the diagonal blocks and then using a finite geometric series proves that multiplication by the chosen classes is an [isomorphism](algebra.md#isomorphism) over $U$.

## Local trivialization

↑ **Parent:** [Fiber bundle](fiber-bundle.md)

A local trivialization of a [fiber bundle](fiber-bundle.md) $p:E\to B$ over an open set $U\subseteq B$ is a [homeomorphism](topology.md#homeomorphism) $p^{-1}(U)\cong U\times F$ commuting with the projections to $U$. For a [vector bundle](#vector-bundle), it must be linear on each fiber. Compatible local trivializations specify the bundle structure and give its transition functions on overlaps.

### Transition function of a vector bundle

↑ **Parent:** [Local trivialization](#local-trivialization)

Two local frames of a [vector bundle](#vector-bundle) differ on their overlap by an invertible matrix-valued function. These functions satisfy the [Čech cocycle condition](ringed-space.md#cech-cocycle-condition). For a [holomorphic vector bundle](complex-geometry.md#holomorphic-vector-bundle) they are [holomorphic](complex-analysis.md#complex-differentiability-at-a-point), and for a [holomorphic line bundle](complex-geometry.md#holomorphic-line-bundle) they are scalar holomorphic units.

#### Structure group of a vector bundle

↑ **Parent:** [Transition function of a vector bundle](#transition-function-of-a-vector-bundle)

A [complex vector bundle](#complex-vector-bundle) has structure group $G$ when it admits fiber-linear [local trivializations](#local-trivialization) whose transition matrices take values in $G$. Replacing frames by $h_i$ changes transitions to $h_i^{-1}g_{ij}h_j$ in the frame convention. Reducing the structure group means choosing new trivializations with values in a specified subgroup. The same transitions glue $U_i\times G$ by left multiplication to a right [principal bundle](#principal-bundle).

## Circle bundle

↑ **Parent:** [Fiber bundle](fiber-bundle.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circle_bundle)

A circle bundle is a [fiber bundle](fiber-bundle.md) with fiber $S^1$. Oriented circle bundles over a paracompact base are classified by their [Euler class](#euler-class-of-a-vector-bundle) in $H^2(B;\mathbb Z)$.

## Ehresmann fibration theorem

↑ **Parent:** [Fiber bundle](fiber-bundle.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ehresmann_fibration_theorem)

Every proper surjective [submersion](differential-geometry.md#submersion) is a locally trivial smooth [fiber bundle](fiber-bundle.md). In particular, the fibers in a proper smooth family are diffeomorphic.

## Principal bundle

↑ **Parent:** [Fiber bundle](fiber-bundle.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principal_bundle)

A principal $G$-bundle is a [fiber bundle](fiber-bundle.md) $\pi:P\to B$ with a free right action of a [Lie group](lie-theory.md#lie-group) $G$ that is locally equivariantly isomorphic to $U\times G\to U$. Each fiber is a single $G$-orbit.

### Principal circle bundle on real projective three-space

↑ **Parent:** [Principal bundle](#principal-bundle)

Write a point of [Real projective space](algebraic-topology.md#real-projective-space) as a nonzero vector $(w_1,w_2)\in\mathbb C^2$ modulo real nonzero scaling. The map to [Complex projective space](algebraic-topology.md#complex-projective-space) sends its class to the complex line through that vector. A free right action of the [circle group](lie-theory.md#circle-group) is $[w]\cdot u=[\lambda w]$ where $\lambda^2=u$; the two possible roots differ by a real sign and therefore give the same projective point. Local smooth square-root branches prove smoothness. Over $[z:1]$, the fibre coordinate is $(w_2/|w_2|)^2$; over $[1:\zeta]$, it is $(w_1/|w_1|)^2$. On the overlap $\zeta=1/z$, the [transition function of a principal bundle](#transition-function-of-a-principal-bundle) is $u\mapsto(z/\overline z)u$. Its phase winds twice. Ordinary scalar multiplication by $u$ instead has a kernel of order two and is not a [free action of a group](group-theory.md#free-action-of-a-group).

### Transition function of a principal bundle

↑ **Parent:** [Principal bundle](#principal-bundle)

For equivariant [local trivializations](#local-trivialization) of a right [principal bundle](#principal-bundle), the change of coordinates is left multiplication in the group coordinate. Indeed an equivariant change $H$ satisfies $H(x,gh)=H(x,g)h$, so evaluating at the identity gives $H(x,g)=(x,\psi(x)g)$. Its inverse shows that $\psi$ takes values in the [Lie group](lie-theory.md#lie-group), and restriction to $(x,e)$ makes it smooth. Composition on triple overlaps gives $\psi_{ki}=\psi_{kj}\psi_{ji}$.

### Frame bundle

↑ **Parent:** [Principal bundle](#principal-bundle)

The frame bundle of an $n$-dimensional [smooth manifold](differential-geometry.md#smooth-manifold) has fiber over $x$ consisting of linear [isomorphisms](algebra.md#isomorphism) $u:\mathbb R^n\to T_xM$. Right composition by $GL(n,\mathbb R)$ makes it a [principal bundle](#principal-bundle). A global [frame of a vector bundle](#frame-of-a-vector-bundle) is a global [section of a fiber bundle](#section-fiber-bundle) and trivializes the [tangent bundle](#tangent-bundle). A metric restricts the allowed frames to the [orthonormal frame bundle](#orthonormal-frame-bundle).

### Orthonormal frame bundle

↑ **Parent:** [Principal bundle](#principal-bundle)

For a metric of signature $(r,s)$, the orthonormal frame bundle consists of all linear isometries $u:\mathbb R^{r,s}\to T_xM$. Right composition by $O(r,s)$ makes it a [principal bundle](#principal-bundle). Its standard [associated vector bundle](#associated-vector-bundle) is the [tangent bundle](#tangent-bundle), via $[u,v]\mapsto u(v)$. A global orthonormal frame is a global section and therefore trivializes this principal bundle. A [Lie group](lie-theory.md#lie-group) with a left-invariant metric has such a frame by left translating an orthonormal basis at the identity.

#### Oriented orthonormal frame bundle of anti-de Sitter spacetime

↑ **Parent:** [Orthonormal frame bundle](#orthonormal-frame-bundle)

Represent the [Anti-de Sitter spacetime](general-relativity.md#anti-de-sitter-spacetime) quadric by $x\cdot x=-\ell^2$ in $\mathbb R^{3,2}$. Appending its timelike unit normal $x/\ell$ to an oriented tangent pseudo-orthonormal frame identifies the frame bundle with $SO(3,2)$. The stabilizer of that normal is $SO(3,1)$, so projection realizes $SO(3,2)/SO(3,1)$ as the base of a [principal bundle](#principal-bundle). For the commonly used universal cover of the anti-de Sitter quadric, pull this bundle back along the covering map; the quadric itself has a periodic timelike coordinate.

#### Oriented orthonormal frame bundle of Minkowski spacetime

↑ **Parent:** [Orthonormal frame bundle](#orthonormal-frame-bundle)

An oriented pseudo-orthonormal frame in [Minkowski spacetime](special-relativity.md#minkowski-spacetime) consists of its base point $a$ and a Lorentz matrix $L$ acting on a fixed reference frame. The pairs $(a,L)$ form the [Poincaré group](special-relativity.md#poincare-group), and right multiplication by $(0,h)$ sends the frame to $(a,Lh)$ while fixing its base point. Thus the displayed projection is a [principal bundle](#principal-bundle) with group $SO(3,1)$. The full frame bundle uses $O(3,1)$; a specified time orientation restricts to the corresponding connected component.

#### Oriented frame bundle of de Sitter spacetime

↑ **Parent:** [Orthonormal frame bundle](#orthonormal-frame-bundle)

Represent unit-radius [de Sitter spacetime](general-relativity.md#de-sitter-spacetime) by the spacelike unit [hyperboloid](differential-geometry.md#hyperboloid) in five-dimensional [Minkowski spacetime](special-relativity.md#minkowski-spacetime). Appending its position vector as the last column of an oriented [pseudo-orthonormal frame](#pseudo-orthonormal-frame) produces a matrix in $SO(4,1)$. Projection to that last column identifies $SO(4,1)$ with the oriented [orthonormal frame bundle](#orthonormal-frame-bundle), a [principal bundle](#principal-bundle) with group $SO(3,1)$. The full bundle allowing both orientations is $O(4,1)$ with group $O(3,1)$. Requiring a time orientation as well selects the corresponding identity components.

##### Global frame on four-dimensional de Sitter spacetime

↑ **Parent:** [Oriented frame bundle of de Sitter spacetime](#oriented-frame-bundle-of-de-sitter-spacetime)

In global coordinates the [de Sitter spacetime](general-relativity.md#de-sitter-spacetime) metric is $-d\tau^2+\cosh^2\tau\,g_{S^3}$. A global [frame of a vector bundle](#frame-of-a-vector-bundle) orthonormal for the round metric $Y_1,Y_2,Y_3$ on $S^3$ gives the displayed global [pseudo-orthonormal frame](#pseudo-orthonormal-frame). For example, identify $S^3$ with the [unit quaternions](algebra.md#unit-quaternion) and use $qi,qj,qk$. Choosing the spatial orientation and the future direction consistently gives a [section of a fiber bundle](#section-fiber-bundle) for the oriented, time-oriented frame bundle. The [principal bundle trivialization by a global section](#principal-bundle-trivialization-by-a-global-section) then proves that bundle is trivial.

### Associated bundle

↑ **Parent:** [Principal bundle](#principal-bundle)

For a [principal bundle](#principal-bundle) $P\to B$ and a left action of its structure group on a manifold $F$, the associated bundle is $(P\times F)/\sim$, where $(pg,f)\sim(p,gf)$. Local sections identify it with $U\times F$; principal transition functions act on $F$. Linear actions give [associated vector bundles](#associated-vector-bundle).

### Principal bundle trivialization by a global section

↑ **Parent:** [Principal bundle](#principal-bundle)

A [principal bundle](#principal-bundle) is trivial exactly when it has a global [section of a fiber bundle](#section-fiber-bundle). Given such a section, the displayed map is a smooth equivariant isomorphism: the free transitive action on each fiber gives the unique inverse group coordinate, and local trivializations make it smooth. Conversely, a product trivialization has the section $x\mapsto(x,e)$.

### Associated vector bundle

↑ **Parent:** [Principal bundle](#principal-bundle)

A linear representation $\rho:G\to GL(V)$ of a [principal bundle](#principal-bundle)'s structure group defines the quotient of $P\times V$ by $(p,v)\sim(pg,\rho(g)^{-1}v)$. It is a [vector bundle](#vector-bundle) over the same base. A [principal connection](#connection-principal-bundle) induces [parallel transport](#parallel-transport) and a local [covariant derivative](general-relativity.md#covariant-derivative) $d+\rho_*(A)$ on its sections.

#### Adjoint bundle

↑ **Parent:** [Associated vector bundle](#associated-vector-bundle)

The adjoint bundle is the [associated vector bundle](#associated-vector-bundle) for the [Adjoint representation of a Lie group](lie-theory.md#adjoint-representation-of-a-lie-group) on its [Lie algebra](lie-algebra.md). The [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) of a [principal connection](#connection-principal-bundle) is globally a two-form with values in this bundle. Differences of [principal connections](#connection-principal-bundle) and their infinitesimal variations are one-forms with values in the same bundle.

### Classifying space

↑ **Parent:** [Principal bundle](#principal-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Classifying_space)

For a [topological group](topological-group.md) $G$, a universal [principal bundle](#principal-bundle) $EG\to BG$ has contractible total space and classifies numerable principal $G$-bundles by pullback. Over a paracompact base, isomorphism classes correspond to [homotopy classes](algebraic-topology.md#homotopy-class) of maps to $BG$. For a discrete group, its [classifying space of a discrete group](#classifying-space-of-a-discrete-group) is a $K(G,1)$; for the circle, $BS^1\simeq\mathbb{CP}^\infty$.

#### Rational odd-rank stabilization of orthogonal classifying spaces

↑ **Parent:** [Classifying space](#classifying-space)

The stabilizer of a line in $O(n)$ is $O(1)\times O(n-1)$, giving the [homogeneous space](lie-theory.md#homogeneous-space) $\mathbb{RP}^{n-1}$. Its classifying-space [Serre fibration](algebraic-topology.md#serre-fibration) has rationally acyclic fiber for odd $n$, so its cohomological [Serre spectral sequence](algebraic-topology.md#serre-spectral-sequence) has only its degree-zero row and gives the displayed restriction isomorphism. The factor $BO(1)=\mathbb{RP}^\infty$ is itself rationally acyclic. For even $n$, the fiber has a top rational class, with determinant-sign monodromy, so the one-row argument fails. The top universal [Pontryagin class](geometry-and-topology.md#pontryagin-class) $p_{n/2}$ is nonzero on $BO(n)$ but vanishes on restriction to $BO(n-1)$, witnessing genuine failure of stabilization.

#### Classifying space of a discrete group

↑ **Parent:** [Classifying space](#classifying-space)

Give a discrete group $G$ a contractible free [CW complex](algebraic-topology.md#cw-complex) $EG$. The quotient $BG=EG/G$ has [universal cover](algebraic-topology.md#universal-cover) $EG$, so it has [fundamental group](algebraic-topology.md#fundamental-group) $G$ and no higher [homotopy groups](algebraic-topology.md#homotopy-group). It is thus an [Eilenberg–MacLane space](algebraic-topology.md#eilenberg-maclane-space) $K(G,1)$, even when $G$ is nonabelian. The cohomology of $BG$ with the appropriate local coefficients computes [group cohomology](group-theory.md#group-cohomology).

### General linear group modulo the unitary group

↑ **Parent:** [Principal bundle](#principal-bundle)

Let $H(n)$ be the real [vector space](vector-space.md) of [Hermitian matrices](hilbert-space.md#hermitian-operator). The [polar decomposition of an invertible complex matrix](linear-algebra.md#polar-decomposition-of-an-invertible-complex-matrix) gives a diffeomorphism

$$
H(n)\times U(n)\longrightarrow GL(n,\mathbb C),
\qquad (B,u)\longmapsto e^Bu.
$$

Its inverse sends $g$ to

$$
B=\frac12\log(gg^*),
\qquad u=e^{-B}g.
$$

Right multiplication by $U(n)$ changes only $u$, so the orbit space is smoothly $H(n)$ and the quotient map is a globally trivial [principal bundle](#principal-bundle).

### Free proper Lie-group action theorem

↑ **Parent:** [Principal bundle](#principal-bundle)

If a [Lie group](lie-theory.md#lie-group) acts smoothly, freely, and properly on a [smooth manifold](differential-geometry.md#smooth-manifold) $P$, then the quotient $P/G$ has a unique smooth structure for which $P\to P/G$ is a [principal bundle](#principal-bundle). An action by a compact Lie group is automatically proper.

### Connection (principal bundle)

↑ **Parent:** [Principal bundle](#principal-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Connection_(principal_bundle))

A principal connection can be specified by a $G$-equivariant horizontal distribution $H\subset TP$ complementary to the vertical bundle, or equivalently by a Lie-algebra-valued connection form $\mathcal A$ that reproduces infinitesimal generators and has $H=\ker\mathcal A$.

#### Translational connection for a convex body rolling on a plane

↑ **Parent:** [Connection (principal bundle)](#connection-principal-bundle)

For a smooth strictly convex [rigid body](classical-mechanics.md#rigid-body-dynamics) with a smooth unique contact point, a configuration consists of its orientation $R\in SO(3)$ and horizontal position $c_{\parallel}\in\mathbb R^2$; its height is fixed by contact. Translation makes this a [principal bundle](#principal-bundle) over $SO(3)$ with group $\mathbb R^2$. If $r(R)$ points from its reference point to contact and $\Omega$ is its spatial [angular velocity](classical-mechanics.md#angular-velocity), [rolling without slipping](classical-mechanics.md#rolling-without-slipping) requires $\dot c+\Omega\times r=0$. The displayed translation-valued [principal connection](#connection-principal-bundle) vanishes on precisely these velocities. It is translation-invariant and equals the identity on vertical translation vectors. A prescribed orientation curve consequently has a unique horizontal lift from a given initial position. No-slip alone leaves spin free and does not specify a connection over the plane with orientation as its fiber; an additional no-twist constraint is needed for that familiar spherical model.

<h4 id="u-1-connection">U(1) connection</h4>

↑ **Parent:** [Connection (principal bundle)](#connection-principal-bundle)

A connection on a principal circle bundle has local real [one-form](differential-form.md#one-form) representatives $A$ transforming by $A\mapsto A+d\chi$. Its curvature is the globally defined [two-form](differential-form.md#2-form) $F=dA$. In unit-charge normalization its [holonomy](#holonomy) around a closed loop is $e^{i\oint A}$, and curvature periods are integer multiples of $2\pi$ on closed surfaces. A circulation representative is defined modulo $2\pi$ under large [gauge transformations](electromagnetism.md#gauge-transformation).

#### Gauge equivalence of principal connections

↑ **Parent:** [Connection (principal bundle)](#connection-principal-bundle)

A gauge transformation is an automorphism of a [principal bundle](#principal-bundle) covering the identity on the base and commuting with its right group action. Pullback relates gauge-equivalent [principal connections](#connection-principal-bundle). Locally it acts by the displayed formula; the [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) transforms by conjugation. Gauge functions on overlapping charts satisfy the bundle's transition compatibility. Infinitesimally $g=e^\varepsilon$ gives $\delta A=D_A\varepsilon$.

#### Local principal connection form

↑ **Parent:** [Connection (principal bundle)](#connection-principal-bundle)

Pulling a [principal connection](#connection-principal-bundle) back along a local section $s$ gives a Lie-algebra-valued one-form on the base. If the section changes to $sg$, the form has the displayed inhomogeneous transformation. Its [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) $F=dA+A\wedge A$ transforms homogeneously as $F'=g^{-1}Fg$. The collection of such local forms encodes a global [principal connection](#connection-principal-bundle) even when no single section exists globally.

##### Reconstruction of a principal connection from local gauge potentials

↑ **Parent:** [Local principal connection form](#local-principal-connection-form)

A [local principal connection form](#local-principal-connection-form) $A$ and a fiber coordinate $\gamma$ reconstruct the connection on a [principal bundle](#principal-bundle) in a local section. Changing that section by $s'=su$ changes $\gamma$ to $u^{-1}\gamma$ and $A$ to $u^{-1}Au+u^{-1}du$. Substitution cancels the two terms involving $du$, so the reconstructed forms agree on overlaps. Here $A$ is Lie-algebra-valued and matrix conjugation denotes the adjoint action. Agreement across trivializations differs from the right-action equivariance $R_h^*\omega=\operatorname{Ad}_{h^{-1}}\omega$.

#### Horizontal distribution of a principal connection

↑ **Parent:** [Connection (principal bundle)](#connection-principal-bundle)

The horizontal distribution of a [principal connection](#connection-principal-bundle) is the smooth complement $H$ to the tangent spaces of the group orbits. A tangent vector is horizontal exactly when the connection form $\mathcal A$ annihilates it.

##### Coordinate horizontal lifts of a principal connection

↑ **Parent:** [Horizontal distribution of a principal connection](#horizontal-distribution-of-a-principal-connection)

On a coordinate trivialization of a [principal bundle](#principal-bundle), the [right-invariant vector fields](lie-theory.md#right-invariant-vector-field) $R_a(\gamma)=T_a\gamma$ satisfy $[R_a,R_b]=-c^d{}_{ab}R_d$. With $A=A_i^aT_a\,dx^i$, the displayed lifts project to the commuting coordinate fields and contract to zero with the [principal connection](#connection-principal-bundle). Taking their [Lie brackets](lie-algebra.md#lie-bracket) gives the local [curvature of a principal connection](#curvature-of-a-principal-connection) coefficients $F_{ij}=\partial_iA_j-\partial_jA_i+[A_i,A_j]$. Thus these lifts commute exactly when the connection is flat. Arbitrary base fields need not commute, and flatness alone does not supply a global coordinate frame or remove [holonomy of a connection](#holonomy).

##### Horizontal section of a principal bundle

↑ **Parent:** [Horizontal distribution of a principal connection](#horizontal-distribution-of-a-principal-connection)

A local section $s:U\to P$ is horizontal when $ds(TU)\subseteq H$, equivalently when $s^*\mathcal A=0$. A [flat principal connection](#flat-principal-connection) has horizontal sections locally, while its [holonomy](#holonomy) can obstruct a global horizontal section.

##### Holonomy

↑ **Parent:** [Horizontal distribution of a principal connection](#horizontal-distribution-of-a-principal-connection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Holonomy)

The holonomy of a connection along a closed curve is the group element relating the endpoints of its horizontal lift. A flat connection can have nontrivial holonomy around a noncontractible loop.

###### Reducible SU2 connection

↑ **Parent:** [Holonomy](#holonomy)

An $SU(2)$ connection whose holonomy lies in a maximal circle, equivalently one preserving a splitting $E=L\oplus L^{-1}$. If its holonomy is the entire circle, parallel adjoint sections are exactly the one-real-dimensional diagonal Lie algebra. The off-diagonal real plane is the underlying real bundle of $L^2$ and has circle weight two.

// Destination: geometry-and-topology.bigb

###### Reflection holonomy along a closed projective geodesic

↑ **Parent:** [Holonomy](#holonomy)

In the round [real projective plane](differential-geometry.md#real-projective-plane), project the great-circle arc $(\cos t,\sin t,0)$ for $0\le t\le\pi$. Its endpoint and velocity match after antipodal identification, so it is a closed [geodesic](riemannian-geometry.md#geodesic). On the sphere its tangent and the constant vector $(0,0,1)$ are parallel. Endpoint identification fixes the returned tangent and reverses the returned transverse vector. Its [parallel transport](#parallel-transport) is therefore a reflection. Nonorientability permits determinant-minus-one holonomy.

###### Holonomy around circular fibres

↑ **Parent:** [Holonomy](#holonomy)

For the [Riemannian metric](differential-geometry.md#riemannian-metric) $dr^2+f(r)^2d\phi^2$, where $f>0$ and $\phi$ has period $2\pi$, [parallel transport](#parallel-transport) around $r=r_0$ acts on the [orthonormal basis](linear-algebra.md#orthonormal-basis) components of a [tangent vector](differential-geometry.md#tangent-vector) by a rotation through $-2\pi f'(r_0)$. Indeed, those components obey $u'=f'(r_0)v$ and $v'=-f'(r_0)u$ as functions of $\phi$. Thus all [tangent vectors](differential-geometry.md#tangent-vector) return to themselves exactly when $f'(r_0)\in\mathbb Z$. The integer criterion concerns [holonomy](#holonomy) and is stronger than local flatness.

###### Flat circular metrics with trivial holonomy

↑ **Parent:** [Holonomy around circular fibres](#holonomy-around-circular-fibres)

On a connected regular radial interval, trivial [holonomy around circular fibres](#holonomy-around-circular-fibres) forces the continuous function $f'$ to be integer-valued, hence constant. The resulting [Riemannian metrics](differential-geometry.md#riemannian-metric) have $f(r)=nr+b$, with $n\in\mathbb Z$ and $f>0$ on the interval. Their [Gaussian curvature](second-fundamental-form.md#gaussian-curvature) is $-f''/f=0$. For $n\ne0$, $\rho=f/|n|$ and $\theta=|n|\phi$ give a [local isometry](differential-geometry.md#local-isometry) to the [Euclidean plane](geometry-and-topology.md#euclidean-plane); for $n=0$, $r,b\phi$ give a flat cylindrical chart. The polar [developing map](differential-geometry.md#developing-map) is injective on the regular domain when $|n|=1$, and is a multiple covering when $|n|>1$. Trivial [holonomy](#holonomy) therefore does not imply a global Euclidean chart. The slope is a discrete parameter, not an unrestricted real one.

###### Riemannian holonomy group

↑ **Parent:** [Holonomy](#holonomy)

For a connected [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), the full holonomy group consists of [parallel transport](#parallel-transport) maps around all piecewise smooth loops based at $p$. Metric compatibility makes them orthogonal. Basepoint changes conjugate this group by parallel transport. This is full holonomy, not just the subgroup using contractible loops.

###### Holonomy representation

↑ **Parent:** [Riemannian holonomy group](#riemannian-holonomy-group)

The holonomy representation is the natural action of the [Riemannian holonomy group](#riemannian-holonomy-group) on $T_pM$. It induces representations on cotangent spaces and tensor powers. Irreducibility means that no nonzero proper real linear subspace of $T_pM$ is invariant.

###### Irreducible holonomy in dimension at least two has no parallel one-form

↑ **Parent:** [Holonomy representation](#holonomy-representation)

A nonzero parallel one-form determines a nonzero parallel vector by metric duality. Its value is fixed by the full [Riemannian holonomy group](#riemannian-holonomy-group), so its span is an invariant line. This contradicts irreducibility when $\dim M\ge2$. The dimension condition matters: the standard circle has trivial but irreducible one-dimensional holonomy representation and a nonzero parallel one-form.

###### Fundamental principle of Riemannian holonomy

↑ **Parent:** [Holonomy representation](#holonomy-representation)

Evaluation at a point identifies parallel tensor fields with tensors fixed by the full [Riemannian holonomy group](#riemannian-holonomy-group). A parallel field is fixed after transport around every loop. Conversely transport a fixed tensor along paths from the basepoint; loop invariance makes the result independent of the path, and local parallel transport shows smoothness and parallelness. Connectedness gives uniqueness.

#### Canonical principal connection on the Stiefel bundle over a Grassmannian

↑ **Parent:** [Connection (principal bundle)](#connection-principal-bundle)

For the principal $O(k)$-bundle of orthonormal $k$-frames over the real Grassmannian, the canonical horizontal vectors move every frame vector orthogonally to the spanned plane. If a frame is represented by a matrix $Q$ with $Q^{\mathsf T}Q=I$, the connection form is

$$
\mathcal A=Q^{\mathsf T}dQ\in\mathfrak o(k).
$$

## Vector bundle

↑ **Parent:** [Fiber bundle](fiber-bundle.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vector_bundle)

A rank-$d$ vector bundle $\pi:E\to B$ is locally isomorphic over the base to the projection $U\times R^d\to U$, with linear transition maps on fibers.

### Density bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

On an $n$-dimensional [smooth manifold](differential-geometry.md#smooth-manifold), the density bundle $|\Lambda^nT^*M|$ is the real [line bundle](ringed-space.md#line-bundle) whose coordinate transformation uses the absolute value of the [Jacobian determinant](calculus.md#jacobian-determinant). A density can therefore be integrated without an [orientation of a smooth manifold](differential-geometry.md#orientation-of-a-smooth-manifold). A [Riemannian metric](differential-geometry.md#riemannian-metric) gives the positive density $\sqrt{\det(g_{ij})}|dx^1\cdots dx^n|$, including on a nonorientable manifold.

// Target: fiber-bundle.bigb

#### Riemannian volume density

↑ **Parent:** [Density bundle](#density-bundle)

A [Riemannian metric](differential-geometry.md#riemannian-metric) on a [smooth manifold](differential-geometry.md#smooth-manifold) gives a positive section of the [density bundle](#density-bundle), locally $d\mu_g=\sqrt{\det(g_{ij})}|dx^1\cdots dx^n|$. The absolute [Jacobian determinant](calculus.md#jacobian-determinant) makes this independent of coordinates without requiring orientability. With an [orientation of a smooth manifold](differential-geometry.md#orientation-of-a-smooth-manifold), it corresponds to the [Riemannian volume form](differential-geometry.md#riemannian-volume-form).

### Tensor bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

For a [smooth manifold](differential-geometry.md#smooth-manifold) $M$, the tensor bundle $T^r_sM=(TM)^{\otimes r}\otimes(T^*M)^{\otimes s}$ is a [vector bundle](#vector-bundle) whose smooth [sections of a vector bundle](#section-of-a-vector-bundle) are [tensor fields](#tensor-field) of type $(r,s)$. Its [transition functions of a vector bundle](#transition-function-of-a-vector-bundle) are tensor products of the [tangent bundle](#tangent-bundle) transition matrices and their inverse transposes. [Symmetric tensors](linear-algebra.md#symmetric-tensor) and [differential forms](differential-form.md) arise from the symmetric and alternating subbundles.

// Target: fiber-bundle.bigb

### G-structure on a vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

A G-structure on a real rank-$m$ [vector bundle](#vector-bundle) is a principal $G$ reduction of its [frame bundle](#frame-bundle). Equivalently it has local frames whose transition matrices take values in $G$, with the reduction consisting of their right $G$-orbits. An [orthogonal structure on a real vector bundle](#orthogonal-structure-on-a-real-vector-bundle) is equivalent to a [fiber metric](#fiber-metric); a special orthogonal reduction is equivalent to that metric together with an [orientation of a vector bundle](#orientation-of-a-vector-bundle).

### Globally generated vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

A [vector bundle](#vector-bundle) is globally generated when its [global sections](ringed-space.md#global-section) span every fibre. The evaluation map in the display expresses this condition. On a projective curve its space of [global sections](ringed-space.md#global-section) is finite-dimensional, so a finite collection of sections suffices.

#### Global generation of positive twists on a smooth curve

↑ **Parent:** [Globally generated vector bundle](#globally-generated-vector-bundle)

For a [vector bundle](#vector-bundle) of finite positive rank let $B$ be an upper degree bound for the [line subbundles](#line-subbundle) of $E^*\otimes K_C$. If $m-1>B$, no nonzero map $\mathcal O_C(mp_0-p)\to E^*\otimes K_C$ can exist for any point $p$: its saturated image would have degree at least $m-1$. [Serre duality](ringed-space.md#serre-duality) then gives $H^1(E(mp_0-p))=0$. The evaluation [exact sequence](homology.md#exact-sequence) shows that $H^0(E(mp_0))\to E(mp_0)|_p$ is [surjective](algebra.md#surjective-function) at every point, proving the assertion with a uniform bound in $p$.

#### Nowhere-vanishing section of a globally generated bundle on a curve

↑ **Parent:** [Globally generated vector bundle](#globally-generated-vector-bundle)

Let $F$ be globally generated of rank $r\ge2$ on a projective curve, and put $W=H^0(C,F)$. The pairs $(p,s)$ with $s(p)=0$ form the total space of the [kernel](linear-algebra.md#kernel-of-a-linear-map) of the evaluation map over the curve. This incidence variety has dimension $\dim W+1-r<\dim W$. Its image in $W$ is closed because the curve is proper, and is a proper subset by the dimension bound. A section outside it vanishes nowhere and gives a [line subbundle](#line-subbundle) $\mathcal O_C\subset F$ with [locally free](ringed-space.md#locally-free-sheaf) quotient.

### Whitney sum of vector bundles

↑ **Parent:** [Vector bundle](#vector-bundle)

The fiberwise direct sum of two [vector bundles](#vector-bundle) over the same base. It is formed from the fiber product of their total spaces, with the direct-sum linear structure in each fiber. Transition matrices are block diagonal.

// Target: geometry-and-topology.bigb

### Symplectic vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

A symplectic vector bundle has a smooth fiberwise [symplectic form](symplectic-geometry.md#symplectic-form), making each fiber a [symplectic vector space](linear-algebra.md#symplectic-vector-space). Its structure group reduces to the [symplectic group](symplectic-geometry.md#symplectic-group). A [symplectic normal bundle](symplectic-geometry.md#symplectic-normal-bundle) is an important example.

#### Lagrangian subbundle

↑ **Parent:** [Symplectic vector bundle](#symplectic-vector-bundle)

A rank-$n$ [vector subbundle](#vector-subbundle) of a rank-$2n$ [symplectic vector bundle](#symplectic-vector-bundle) is Lagrangian when each fibre is a [Lagrangian subspace](symplectic-geometry.md#lagrangian-subspace). If it exists, a [compatible almost complex structure](complex-geometry.md#compatible-almost-complex-structure) supplies a complementary [Lagrangian subbundle](#lagrangian-subbundle) by applying $J$. Existence is a global condition: the area-oriented [tangent bundle](#tangent-bundle) of the two-sphere has no real line subbundle, by triviality of real [line bundles](ringed-space.md#line-bundle) over the sphere and the [Hairy ball theorem](#hairy-ball-theorem).

### Thom space

↑ **Parent:** [Vector bundle](#vector-bundle)

For a real [vector bundle](#vector-bundle) over a compact base, its Thom space is the quotient of its disk bundle by its [sphere bundle](#sphere-bundle), with the collapsed sphere bundle as basepoint. Equivalently it is the one-point compactification of the total space. An oriented bundle's [Thom class](#thom-class) and Thom isomorphism identify the reduced cohomology of this space with shifted cohomology of the base.

#### Projective-space quotient as a Thom space of conjugate tautological lines

↑ **Parent:** [Thom space](#thom-space)

Decompose the ambient vector space as $V\oplus W$, of dimensions $n+1,m+1$. A projective line outside $\mathbb P(V)$ is the graph of a unique linear map from a line in $W$ to $V$. Thus the complement is the total space of $\gamma^*\otimes V$, which is complex-isomorphic to $\bar\gamma^{\oplus(n+1)}$ after choosing a [Hermitian metric](complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle). Collapsing $\mathbb P(V)$ gives its [one-point compactification](topology.md#alexandroff-extension), hence the [Thom space](#thom-space) because the base is compact.

// Target: geometry-and-topology.bigb

### Line subbundle

↑ **Parent:** [Vector bundle](#vector-bundle)

A line subbundle is an injective map from a [line bundle](ringed-space.md#line-bundle) into a [vector bundle](#vector-bundle) whose quotient is [locally free](ringed-space.md#locally-free-sheaf). Equivalently the injection splits locally. On a [smooth algebraic curve](algebraic-geometry.md#smooth-algebraic-curve), saturation of a rank-one coherent subsheaf produces a [saturated line subbundle on a smooth curve](ringed-space.md#saturated-line-subbundle-on-a-smooth-curve).

<h3 id="birkhoff-grothendieck-theorem">Birkhoff–Grothendieck theorem</h3>

↑ **Parent:** [Vector bundle](#vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Birkhoff–Grothendieck_theorem)

Every [vector bundle](#vector-bundle) on the [projective line](finite-group-theory.md#projective-line) over a [field](algebra.md#field) splits as a [direct sum](vector-space.md#direct-sum) of [line bundles](ringed-space.md#line-bundle). Choose the largest integer $a$ with $H^0(E(-a))\ne0$. A corresponding map $\mathcal O(a)\to E$ is saturated, since saturation otherwise increases its degree. Inductively split its quotient as $\bigoplus_i\mathcal O(b_i)$. Twisting the exact sequence by $-a-1$ and using $H^1(\mathcal O(-1))=0$ gives $b_i\leq a$. Hence all extension groups $H^1(\mathcal O(a-b_i))$ vanish, and the sequence splits. The multiset of degrees is determined by the dimensions of all twisted global-section spaces.

### Stable framing of a vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

A framing is a continuous ordered basis in every fiber, equivalently a trivialization of the [vector bundle](#vector-bundle). A stable framing trivializes the bundle after adding trivial real summands, up to further stabilization and homotopy. For a smooth map it is the stable normal data that is framed, not necessarily the tangent bundle of either manifold.

### Endomorphism bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

The [vector bundle](#vector-bundle) whose fibre at $p$ consists of linear maps $E_p\to E_p$. If a [local frame](#frame-of-a-vector-bundle) changes by $e'=eg$, the coefficient matrix of an [endomorphism](algebra.md#endomorphism) changes by $T'=g^{-1}Tg$, giving smooth fibre-linear transitions. For a [line bundle](ringed-space.md#line-bundle) this bundle is canonically the trivial scalar bundle, because every fibre endomorphism is scalar multiplication. A [connection on a vector bundle](#connection-vector-bundle) induces the [endomorphism bundle connection](#endomorphism-bundle-connection).

### Exterior power of a vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

For a rank-$k$ smooth [vector bundle](#vector-bundle), take the [exterior power](linear-algebra.md#exterior-power) $\Lambda^rE_p$ in each fibre. A local frame gives a trivialization with fibre $\Lambda^r\mathbb R^k$, and a transition matrix $A$ acts by $\Lambda^rA$. Functoriality preserves the cocycle identities, producing a smooth vector bundle of rank $\binom{k}{r}$, or the zero bundle when $r>k$. Its top exterior power is the [determinant line bundle](#determinant-line-bundle).

### Clutching construction

↑ **Parent:** [Vector bundle](#vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Clutching_construction)

A [vector bundle](#vector-bundle) over $S^n$ can be constructed by gluing two trivial bundles over its hemispheres with a transition map $\gamma:S^{n-1}\to GL(k,\mathbb R)$. Extend this map constantly in an equatorial collar to obtain local [vector bundle trivializations](#vector-bundle-trivialization). A transition map into the [special orthogonal group](linear-algebra.md#special-orthogonal-group) gives compatible fiber [orientations](algebraic-topology.md#orientation-of-a-simplex) and a [fiber metric](#fiber-metric). Homotopies of transition maps give isomorphic bundles.

#### Clutching function

↑ **Parent:** [Clutching construction](#clutching-construction)

A clutching function is the equatorial transition map used in the [clutching construction](#clutching-construction). For an oriented real [vector bundle](#vector-bundle) one may choose a [fiber metric](#fiber-metric) and orthonormal trivializations, so its clutching function takes values in the [special orthogonal group](linear-algebra.md#special-orthogonal-group).

##### Section obstruction for a clutched vector bundle

↑ **Parent:** [Clutching function](#clutching-function)

For an oriented rank-$k$ bundle over $S^n$, with $k\ge2$, normalize its [clutching function](#clutching-function) to be based at the identity. A [nowhere-zero section](#nowhere-zero-section) exists precisely when the displayed [homotopy class](algebraic-topology.md#homotopy-class) vanishes. If it vanishes, extend $\gamma e_k$ across one hemisphere and use the constant section $e_k$ on the other. Conversely normalize any [nowhere-zero section](#nowhere-zero-section) using the [fiber metric](#fiber-metric). Its two hemisphere maps satisfy $\sigma_-=\gamma\sigma_+$ on the boundary. The first hemisphere makes $\sigma_+$ homotopic to a constant; the second makes $\gamma\sigma_+$ null-homotopic. Thus $\gamma e_k$ is [null-homotopic](algebraic-topology.md#null-homotopic-map). If $k>n$, the lower [homotopy group](algebraic-topology.md#homotopy-group) of the [sphere](geometry-and-topology.md#sphere) vanishes and a section always exists. Rank one is already trivial because $SO(1)$ is trivial.

### Clifford module bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

A Clifford module bundle is a [vector bundle](#vector-bundle) over a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) with a fibrewise [Clifford multiplication](algebra.md#clifford-multiplication). A compatible [connection on a vector bundle](#connection-vector-bundle) satisfies $[\nabla_X,c(\alpha)]=c(\nabla_X\alpha)$ for the [Levi-Civita connection](general-relativity.md#levi-civita-connection) on covectors. On a graded Clifford module bundle, [Clifford multiplication](algebra.md#clifford-multiplication) exchanges the two grading summands. The associated [Dirac operator](riemannian-geometry.md#dirac-operator) is $D=\sum_i c(e^i)\nabla_{e_i}$. Its fibres are modules over the fibres of the [Clifford algebra bundle](algebra.md#clifford-algebra-bundle).

### Determinant line bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

The top [exterior power](linear-algebra.md#exterior-power) of a rank-$r$ [vector bundle](#vector-bundle) is its [determinant line bundle](#determinant-line-bundle). A [short exact sequence](module-theory.md#short-exact-sequence) of [vector bundles](#vector-bundle) gives a canonical isomorphism of the middle [determinant](linear-algebra.md#determinant) with the [tensor product](linear-algebra.md#tensor-product) of the other two. Locally, a subbundle frame followed by lifts of a quotient frame defines it; changing lifts only adds off-diagonal blocks. This is the [determinant](linear-algebra.md#determinant) step in [adjunction for a smooth submanifold](complex-geometry.md#adjunction-for-a-smooth-submanifold).

### Zero section of a vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

The [zero section](#zero-section-of-a-vector-bundle) sends each base point to the zero vector in its fiber. It is a smooth [section of a vector bundle](#section-of-a-vector-bundle) and an embedded copy of the base. The [Liouville one-form](symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle) vanishes as an ambient covector precisely along the [zero section](#zero-section-of-a-vector-bundle) of a [cotangent bundle](symplectic-geometry.md#cotangent-bundle).

### Fiber metric

↑ **Parent:** [Vector bundle](#vector-bundle)

A fiber metric on a real smooth [vector bundle](#vector-bundle) is a positive-definite [inner product](linear-algebra.md#inner-product) on each fiber that varies smoothly in [vector bundle trivializations](#vector-bundle-trivialization). A smooth [partition of unity](differential-geometry.md#partition-of-unity) subordinate to trivializing charts averages their Euclidean inner products. Nonnegative weights preserve positivity and local finiteness ensures smoothness. Hence every real vector bundle over a Hausdorff second-countable [smooth manifold](differential-geometry.md#smooth-manifold) admits a fiber metric. Applied to the [tangent bundle](#tangent-bundle), this is existence of a [Riemannian metric](differential-geometry.md#riemannian-metric).

#### Orthogonal structure on a real vector bundle

↑ **Parent:** [Fiber metric](#fiber-metric)

An orthogonal structure is a reduction of the transition functions of a real rank-$r$ [vector bundle](#vector-bundle) to the [orthogonal group](linear-algebra.md#orthogonal-group). Its orthonormal frames define a [fiber metric](#fiber-metric), independent of the chosen frame because orthogonal transitions preserve the [inner product](linear-algebra.md#inner-product). Conversely a [fiber metric](#fiber-metric) gives smooth orthonormal frames by the [Gram-Schmidt process](linear-algebra.md#gram-schmidt-process), with orthogonal transition matrices. This equivalence does not require the [vector bundle](#vector-bundle) to be globally trivial.

##### Euclidean orthonormal frame

↑ **Parent:** [Orthogonal structure on a real vector bundle](#orthogonal-structure-on-a-real-vector-bundle)

This is a frame of a real [vector bundle](#vector-bundle) with a positive-definite [fiber metric](#fiber-metric) for which the basis vectors are orthonormal. The [Gram-Schmidt process](linear-algebra.md#gram-schmidt-process) applied to any smooth local frame produces such frames smoothly. They are distinguished from Lorentzian orthonormal frames, whose metric has mixed signature.

##### Orthogonal local trivialization

↑ **Parent:** [Orthogonal structure on a real vector bundle](#orthogonal-structure-on-a-real-vector-bundle)

A [vector bundle trivialization](#vector-bundle-trivialization) is orthogonal when its coordinate frame is orthonormal for the [fiber metric](#fiber-metric), so each fiber is identified isometrically with Euclidean space. Overlap changes then take values in the [orthogonal group](linear-algebra.md#orthogonal-group). Local orthogonal trivializations exist even when no global frame does.

### Eigenbundle

↑ **Parent:** [Vector bundle](#vector-bundle)

For a smooth complex [vector bundle](#vector-bundle) endomorphism $A$ and a smooth eigenvalue function $\lambda$, a kernel of constant rank is a smooth vector subbundle, called its eigenbundle. Without a constant-rank hypothesis these kernels need not form a [vector bundle](#vector-bundle).

### Hermitian vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

A Hermitian vector bundle is a complex [vector bundle](#vector-bundle) with a smoothly varying positive definite [Hermitian form](linear-algebra.md#hermitian-form) on each fibre. When the bundle is holomorphic, this is a [Hermitian metric on a holomorphic vector bundle](complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle). Orthogonal projection to a smooth subbundle produces its induced metric and the [quotient Hermitian metric](complex-geometry.md#quotient-hermitian-metric).

### Complex vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

A complex vector bundle is a [vector bundle](#vector-bundle) with complex-linear local trivializations and transition maps. A rank-$r$ complex bundle has an underlying oriented real bundle of rank $2r$, using the orientation of complex bases. Rank-one bundles are [complex line bundles](#complex-line-bundle), and their higher-rank counterparts have integral [Chern classes](algebraic-geometry.md#chern-class).

#### Hermitian metric on a smooth complex vector bundle

↑ **Parent:** [Complex vector bundle](#complex-vector-bundle)

This is a smoothly varying positive-definite [Hermitian form](linear-algebra.md#hermitian-form) on each fiber, without requiring a holomorphic base or bundle. A [partition of unity](differential-geometry.md#partition-of-unity) glues local positive metrics into a global one. Applying smooth Gram-Schmidt to local frames then makes the transitions unitary, reducing the [structure group of a vector bundle](#structure-group-of-a-vector-bundle) to $U(k)$. For a line bundle its unit vectors form a [principal bundle](#principal-bundle) for the [circle group](lie-theory.md#circle-group).

#### Stable complex structure on a real vector bundle

↑ **Parent:** [Complex vector bundle](#complex-vector-bundle)

For an even-rank real [vector bundle](#vector-bundle) $\xi$, a stable complex structure is a complex structure on $\xi\oplus\mathbb R^{2s}$, considered up to adding trivial complex bundles and homotopy. This gives a stable complex class but does not necessarily make $\xi$ itself a complex vector bundle. Stable Chern classes therefore need not recover the unstable [Euler class](#euler-class-of-a-vector-bundle): $TS^4\oplus\mathbb R^2$ can be made trivial complex, while $e(TS^4)$ evaluates to $2$.

#### Conjugate vector bundle

↑ **Parent:** [Complex vector bundle](#complex-vector-bundle)

The conjugate bundle has the same underlying real bundle and the opposite complex scalar action. Its transitions are the complex conjugates of the original transitions. For a holomorphic bundle on $X$, these transitions are smooth and generally antiholomorphic on $X$; it is not automatically a holomorphic bundle there. It is naturally holomorphic over the conjugate [complex manifold](complex-geometry.md#complex-manifold) instead.

##### Conjugate connection

↑ **Parent:** [Conjugate vector bundle](#conjugate-vector-bundle)

A complex bundle connection induces a connection on its [conjugate vector bundle](#conjugate-vector-bundle) by the displayed rule on real tangent fields. The conjugate scalar action gives the correct Leibniz rule. In conjugate frames the matrix is the complex conjugate of the original connection matrix, with evaluation of one-forms on real tangent vectors understood.

### Rank of a vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

The rank of a [vector bundle](#vector-bundle) at a point is the [dimension](vector-space.md#dimension-vector-space) of its fiber as a [vector space](vector-space.md). A [vector bundle trivialization](#vector-bundle-trivialization) identifies nearby fibers with the same [vector space](vector-space.md), so this rank is locally constant. A rank-$r$ bundle has fibers of dimension $r$ everywhere.

### Vector bundle morphism

↑ **Parent:** [Vector bundle](#vector-bundle)

A morphism of [vector bundles](#vector-bundle) over one base is a smooth map between their total spaces that commutes with projection to the base and is linear on each fiber. In local [vector bundle trivializations](#vector-bundle-trivialization) it is multiplication by a smoothly varying [matrix](vector-space.md#matrix).

#### Kernel bundle of a surjective vector bundle morphism

↑ **Parent:** [Vector bundle morphism](#vector-bundle-morphism)

A fiberwise surjective morphism of constant-rank vector bundles has a kernel vector subbundle. For a morphism from a trivial rank-$N$ bundle, a local full-row-rank matrix $F(x)$ gives the continuous kernel projection $I-F(x)^T(F(x)F(x)^T)^{-1}F(x)$. Changing the local frame in the target leaves this projection unchanged. Thus its kernel defines a continuous map into the appropriate [Grassmannian](differential-geometry.md#grassmannian).

#### Vector bundle endomorphism

↑ **Parent:** [Vector bundle morphism](#vector-bundle-morphism)

A smooth [vector bundle morphism](#vector-bundle-morphism) from a [vector bundle](#vector-bundle) $E$ to itself, covering the identity on the base, is a [vector bundle](#vector-bundle) endomorphism. It is fibrewise linear and is equivalently a smooth section of $\operatorname{End}E$. In a local frame its matrix is smooth and changes by conjugation under changes of frame. An [almost complex structure](complex-geometry.md#almost-complex-manifold) is a real endomorphism of the [tangent bundle](#tangent-bundle) satisfying $J^2=-I$.

#### Holomorphic bundle map

↑ **Parent:** [Vector bundle morphism](#vector-bundle-morphism)

A holomorphic bundle map is a [holomorphic map](complex-analysis.md#holomorphic-map) between total spaces of [holomorphic vector bundles](complex-geometry.md#holomorphic-vector-bundle) that covers a holomorphic base map and is complex-linear on each fibre. Over a fixed base, its matrix in [holomorphic local frames](complex-geometry.md#holomorphic-local-trivialization) has holomorphic entries.

#### Bundle morphisms from maps of smooth sections

↑ **Parent:** [Vector bundle morphism](#vector-bundle-morphism)

Every $C^\infty(M)$-linear map between the [modules of smooth sections](#module-of-smooth-sections) of finite-rank smooth [vector bundles](#vector-bundle) is induced by a unique [vector bundle morphism](#vector-bundle-morphism). A [smooth bump function](partial-differential-equation.md#smooth-bump-function) shows that the map is local. A bumped local frame then proves that a section vanishing at $x$ has image vanishing at $x$. Evaluating the image therefore defines a well-defined fiberwise [linear map](vector-space.md#linear-map). The images of the bumped frame give smooth matrix columns, proving the resulting morphism is smooth. This elementary argument is also described in [Brian Conrad's bundle notes](https://math.stanford.edu/~conrad/diffgeomPage/handouts/bundle.pdf).

#### Vector bundle isomorphism

↑ **Parent:** [Vector bundle morphism](#vector-bundle-morphism)

A [vector bundle morphism](#vector-bundle-morphism) is an isomorphism if it admits an inverse of the same kind. A smooth fiberwise bijective bundle morphism automatically has a smooth inverse, because inverse [matrices](vector-space.md#matrix) in [vector bundle trivializations](#vector-bundle-trivialization) depend smoothly on their entries wherever their determinants are nonzero.

### Vector bundle trivialization

↑ **Parent:** [Vector bundle](#vector-bundle)

A local trivialization of a rank-$r$ [vector bundle](#vector-bundle) $\pi:E\to M$ is a bundle isomorphism $\pi^{-1}(U)\cong U\times\mathbb R^r$ over an open set $U$, linear on each fiber. Overlapping trivializations differ by $(p,v)\mapsto(p,g(p)v)$ for a smooth $GL_r(\mathbb R)$-valued function $g$. A [tangent bundle](#tangent-bundle) chart uses the derivative of its base [manifold chart](differential-geometry.md#manifold-chart) for this fiber identification.

#### Frame of a vector bundle

↑ **Parent:** [Vector bundle trivialization](#vector-bundle-trivialization)

A frame over an open set $U$ is a list of smooth sections $e_1,\ldots,e_r$ of a rank-$r$ [vector bundle](#vector-bundle) whose values form a basis in every fibre over $U$. It is equivalent to a [vector bundle trivialization](#vector-bundle-trivialization) by $(x,v)\mapsto\sum_a e_a(x)v^a$. Two local frames differ by a smooth map $g:U\to\mathrm{GL}(r)$, written $e'=eg$.

##### Pseudo-orthonormal frame

↑ **Parent:** [Frame of a vector bundle](#frame-of-a-vector-bundle)

For a [vector bundle](#vector-bundle) carrying a smooth nondegenerate symmetric [bilinear form](linear-algebra.md#bilinear-form) of constant [metric signature](topology.md#metric-signature), a pseudo-orthonormal frame is a smooth local [frame of a vector bundle](#frame-of-a-vector-bundle) whose Gram matrix is the constant diagonal signature matrix $\eta$. It identifies the metric bundle locally with a fixed model $\mathbb R^{p,q}$. Two such frames differ by a smooth map into the corresponding [orthogonal group](linear-algebra.md#orthogonal-group). Positive-definite signature is included as the ordinary orthonormal case. A global pseudo-orthonormal frame is a [section of a fiber bundle](#section-fiber-bundle) of the [orthonormal frame bundle](#orthonormal-frame-bundle) and trivializes that [principal bundle](#principal-bundle).

##### Coframe

↑ **Parent:** [Frame of a vector bundle](#frame-of-a-vector-bundle)

A coframe dual to a local frame of the [tangent bundle](#tangent-bundle) is the corresponding local frame of the [cotangent bundle](symplectic-geometry.md#cotangent-bundle). Its elements are [differential one-forms](differential-form.md#one-form). Applying the coframe to covariant derivatives of the frame extracts the [connection one-forms](#connection-one-form); applying it to the [torsion tensor](#torsion-tensor) extracts the [torsion forms](#torsion-form).

### Complexification of a real vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

Complexification replaces each fiber of a real [vector bundle](#vector-bundle) by its [tensor product](linear-algebra.md#tensor-product) with $\mathbb C$ over $\mathbb R$. The [complexification of a real vector bundle](#complexification-of-a-real-vector-bundle) of rank one is a [complex line bundle](#complex-line-bundle). For the [tautological bundle](#tautological-bundle) over [Real projective space](algebraic-topology.md#real-projective-space), this [complex line bundle](#complex-line-bundle) squares to the [trivial vector bundle](#trivial-vector-bundle).

### Projective bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

The projective bundle of a real or complex [vector bundle](#vector-bundle) $E\to X$ has fiber the space of one-dimensional subspaces of $E_x$. It carries a [tautological bundle](#tautological-bundle) $\lambda\subset p^*E$; in the real case this is the [projectivization of a real vector bundle](#projectivization-of-a-real-vector-bundle).

The same construction applies to an algebraic [vector bundle](#vector-bundle) over an [algebraic variety](algebraic-geometry.md#algebraic-variety): local trivializations glue products with [projective space](projective-space.md). In the lines convention its universal [tautological bundle](#tautological-bundle) is a [line bundle](ringed-space.md#line-bundle); the alternative [projectivization by quotients](#projectivization-by-quotients) convention parametrizes one-dimensional quotient spaces. Both conventions give dimension $\dim X+\operatorname{rank}(E)-1$ and a [proper morphism](ringed-space.md#proper-morphism) to the base.

#### Projectivization by quotients

↑ **Parent:** [Projective bundle](#projective-bundle)

This convention for a [projective bundle](#projective-bundle) parametrizes one-dimensional quotients of the fibres of a [vector bundle](#vector-bundle) $E$. Its universal quotient is $\pi^*E\twoheadrightarrow\mathcal O_{\mathbb P(E)}(1)$, and $\pi_*\mathcal O(1)=E$. Tensoring $E$ by a [line bundle](ringed-space.md#line-bundle) on the base leaves the projective bundle unchanged but tensors its universal quotient by the pullback of that line bundle. The alternative convention of [holomorphic projectivization by lines](#holomorphic-projectivization-by-lines) replaces $E$ by its dual and reverses the tautological sign.

##### Universal quotient line bundle

↑ **Parent:** [Projectivization by quotients](#projectivization-by-quotients)

On the [projectivization by quotients](#projectivization-by-quotients), the fibre over a one-dimensional quotient of $E_x$ is that quotient line itself. These lines glue to the universal quotient. Its restriction to a projective fibre has degree one. It is the dual of the relative tautological line after identifying quotient projectivization of $E$ with line projectivization of $E^*$.

##### Rational normal scroll

↑ **Parent:** [Projectivization by quotients](#projectivization-by-quotients)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rational_normal_scroll)

For this smooth [projective bundle](#projective-bundle), put $L=\pi^*\mathcal O_{\mathbb P^1}(1)$ and $M=\mathcal O_{\mathbb F}(1)$, using [projectivization by quotients](#projectivization-by-quotients). If every $a_i>0$, the complete system $|M|$ embeds it as a rational normal scroll. If every $a_i\ge0$, the same system defines a scroll image which may be singular. Allowing arbitrary integers gives an abstract scroll; a common twist makes an embedding available. Its [intersection numbers](algebraic-geometry.md#intersection-number-of-a-cartier-divisor-with-a-curve) are $L^2=0$, $LM^{n-1}=1$, $M^n=\sum_i a_i$, and its [canonical divisor](algebraic-geometry.md#canonical-divisor) is $-nM+(\sum_i a_i-2)L$.

###### Fiber class of a rational normal scroll

↑ **Parent:** [Rational normal scroll](#rational-normal-scroll)

The divisor class of a fibre of the ruling of a [rational normal scroll](#rational-normal-scroll) has square zero. Its complete pencil recovers the projection to $\mathbb P^1$, and its intersection with $M^{n-1}$ is one.

###### Isomorphism classification of abstract rational scrolls

↑ **Parent:** [Rational normal scroll](#rational-normal-scroll)

Two rank-$n$ abstract [rational normal scrolls](#rational-normal-scroll) are [isomorphic](algebra.md#isomorphism) exactly when their splitting degrees agree as multisets after a common integer shift. For $n\ge3$, the primitive nef class $L$ of the ruling is intrinsically identified by $L^2=0$: restriction to a projective fibre forces every other divisor class with square zero to have zero coefficient of $M$. An isomorphism therefore preserves the ruling, and its effect on $M$ is a twist by $cL$. Pushforward gives an isomorphism of the defining bundles up to this twist; uniqueness in the [Birkhoff–Grothendieck theorem](#birkhoff-grothendieck-theorem) recovers their splitting degrees. For surfaces the unique nef square-zero ray identifies the ruling except on $\mathbb P^1\times\mathbb P^1$, where exchanging the two rulings changes no normalized splitting type.

#### Chern classes of a tautological-line complement

↑ **Parent:** [Projective bundle](#projective-bundle)

For the line-projectivization of a rank-$n$ complex bundle, $p^*E=S\oplus S^\perp$. The [Whitney sum formula for Chern classes](algebraic-geometry.md#whitney-sum-formula-for-chern-classes) gives $c_t(S^\perp)=p^*c_t(E)/(1+xt)$ as a formal power series. Comparing coefficients proves the formula. Since $S^\perp$ has rank $n-1$, its degree-$n$ [Chern class](algebraic-geometry.md#chern-class) vanishes and yields the monic projective-bundle relation.

// Target: geometry-and-topology.bigb

#### Holomorphic projectivization by lines

↑ **Parent:** [Projective bundle](#projective-bundle)

For a [holomorphic vector bundle](complex-geometry.md#holomorphic-vector-bundle), projectivize each fibre using lines. The transition $g_{ij}(x)$ acts holomorphically by $[v]\mapsto[g_{ij}(x)v]$. Thus local products $U_i\times\mathbb P^{r-1}$ define a [complex manifold](complex-geometry.md#complex-manifold) with holomorphic projection to the base. The lines convention gives the [relative tautological line bundle](#relative-tautological-line-bundle) of fibre degree $-1$, and its dual has degree $+1$.

##### Relative tautological line bundle

↑ **Parent:** [Holomorphic projectivization by lines](#holomorphic-projectivization-by-lines)

On the [holomorphic projectivization by lines](#holomorphic-projectivization-by-lines), take the line itself as the fibre of $S$. The evaluation inclusion makes it a holomorphic line subbundle of $p^*E$. Its fibre restriction is $\mathcal O(-1)$; the dual is the [relative hyperplane line bundle](#relative-hyperplane-line-bundle).

###### Relative hyperplane line bundle

↑ **Parent:** [Relative tautological line bundle](#relative-tautological-line-bundle)

Dualize the [relative tautological line bundle](#relative-tautological-line-bundle) to obtain the positive relative hyperplane [line bundle](ringed-space.md#line-bundle). It restricts to $\mathcal O(1)$ on each projective fibre. This sign depends on the convention that projectivization parametrizes lines; fixing the convention avoids confusing it with the tautological line itself.

#### Sections of a projective bundle

↑ **Parent:** [Projective bundle](#projective-bundle)

A complex line subbundle $L\subset E$ defines a [section of a fiber bundle](#section-fiber-bundle) $s:X\to\mathbb P(E)$ selecting $L_x$ at each point. Pullback of the [tautological bundle](#tautological-bundle) along $s$ is $L$, so if $t$ is its [Euler class](#euler-class-of-a-vector-bundle), then $s^*t=e(L)$. For a decomposition $E=\bigoplus_iL_i$, the resulting sections and the open sets where coordinate projection is nonzero identify the tautological line with $\pi^*L_i$. These identifications support the projective-bundle factorization via a [vanishing cup product from an open cover](cohomology.md#vanishing-cup-product-from-an-open-cover).

#### Orthogonal complex line flag manifold

↑ **Parent:** [Projective bundle](#projective-bundle)

For $n\geq2$, ordered orthogonal complex lines in $\mathbb C^n$ form a [projective bundle](#projective-bundle) over $\mathbb{CP}^{n-1}$, with fiber $\mathbb{CP}^{n-2}$. Here $L$ is the first tautological line and the complement is formed using the standard [Hermitian inner product](linear-algebra.md#hermitian-form). Its real dimension is $4n-6$. It is also the partial complex flag space of a line contained in a two-plane: send an orthogonal pair to $(\ell_1,\ell_1\oplus\ell_2)$, and recover the second line by orthogonal complement inside the two-plane.

##### Cohomology ring of the orthogonal complex line flag manifold

↑ **Parent:** [Orthogonal complex line flag manifold](#orthogonal-complex-line-flag-manifold)

For the [orthogonal complex line flag manifold](#orthogonal-complex-line-flag-manifold), take $x,y$ to be the first [Chern classes](algebraic-geometry.md#chern-class) of the duals of its two tautological lines, both in degree two. The [Whitney sum formula for Chern classes](algebraic-geometry.md#whitney-sum-formula-for-chern-classes) gives $c_i(L^\perp)=x^i$. The [projective bundle definition of Chern classes](algebraic-geometry.md#projective-bundle-definition-of-chern-classes) gives the second relation, and [Leray-Hirsch theorem](#leray-hirsch-theorem) gives the integral basis $x^iy^j$ with $0\leq i<n$, $0\leq j<n-1$. Polynomial division by the monic relation in $y$ proves that there are no further relations. Multiplying that relation by $y-x$ also gives $y^n=0$.

#### Projective bundle formula for complex vector bundles

↑ **Parent:** [Projective bundle](#projective-bundle)

For a rank-$r$ complex [vector bundle](#vector-bundle) and $u=c_1(\lambda^*)$, the [cohomology](cohomology.md) of its [projective bundle](#projective-bundle) is free over the [cohomology](cohomology.md) of the base on $1,u,\ldots,u^{r-1}$. Consequently pullback is injective, which yields the [splitting principle for complex vector bundles](algebraic-topology.md#splitting-principle-for-complex-vector-bundles) by iteration.

### Complex line bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

A complex line bundle is a [vector bundle](#vector-bundle) whose fibers are one-dimensional complex vector spaces and whose transition maps are complex linear. Its underlying real bundle has rank two and a canonical orientation, and its Euler class equals its [First Chern class](complex-geometry.md#first-chern-class).

#### Smooth exponential sequence

↑ **Parent:** [Complex line bundle](#complex-line-bundle)

On a [smooth manifold](differential-geometry.md#smooth-manifold), the sequence of [sheaves of abelian groups](algebraic-geometry.md#sheaf-of-abelian-groups)

$$
0\to\underline{\mathbb Z}\to\mathcal C^\infty_{\mathbb C}\xrightarrow{\exp(2\pi i\,\cdot)}\mathcal C^{\infty,*}_{\mathbb C}\to1
$$

is exact. The additive smooth-function sheaf is a [fine sheaf](ringed-space.md#fine-sheaf), so the connecting map identifies $H^1(X,\mathcal C^{\infty,*}_{\mathbb C})$ with $H^2(X,\mathbb Z)$. The former classifies smooth [complex line bundles](#complex-line-bundle) and the connecting class is their [First Chern class](complex-geometry.md#first-chern-class).

#### Smooth classification of complex line bundles on the complex projective line

↑ **Parent:** [Complex line bundle](#complex-line-bundle)

Every smooth complex line bundle on $\mathbb{CP}^1$ is isomorphic to exactly one twisting bundle $\mathcal O(k)$. Trivializing on the two standard affine charts leaves a transition function on $\mathbb C^*$; its [winding number](complex-analysis.md#winding-number) determines $k$, and a [partition of unity](differential-geometry.md#partition-of-unity) removes the zero-winding factor.

### Real line bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

A real line bundle is a rank-one real [vector bundle](#vector-bundle). It is orientable exactly when it is trivial.

<h4 id="mobius-line-bundle">Möbius line bundle</h4>

↑ **Parent:** [Real line bundle](#real-line-bundle)

The Möbius line bundle over the circle is

$$
L=(\mathbb R\times\mathbb R)/((t+2\pi,a)\sim(t,-a)),
$$

with projection to $t$ modulo $2\pi$. It is a smooth rank-one [vector bundle](#vector-bundle). A section is represented by a function $s$ satisfying $s(t+2\pi)=-s(t)$, so the [intermediate value theorem](calculus.md#intermediate-value-theorem) forces every [continuous](calculus.md#continuous-function) section to vanish somewhere. Thus it has no [nowhere-zero section](#nowhere-zero-section) and is not isomorphic to the [trivial vector bundle](#trivial-vector-bundle) of rank one.

#### Classification of real line bundles

↑ **Parent:** [Real line bundle](#real-line-bundle)

Real line bundles over a paracompact space are classified up to isomorphism by their first [Stiefel–Whitney class](#stiefel-whitney-class) in $H^1(X;\mathbb F_2)$. Tensor product corresponds to addition of classes.

#### Mod-two Euler class of a real line bundle

↑ **Parent:** [Real line bundle](#real-line-bundle)

For a real line bundle, the mod-two Euler class is its top [Stiefel–Whitney class](#stiefel-whitney-class), namely $w_1(L)\in H^1(X;\mathbb F_2)$. Its evaluation on a closed curve records whether parallel transport reverses the fiber orientation.

### Vector subbundle

↑ **Parent:** [Vector bundle](#vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vector_subbundle)

A vector subbundle $F\subseteq E$ is a subset whose fibers are [vector subspaces](vector-space.md#vector-subspace) $F_x\subseteq E_x$ of constant dimension and which admits local frames extending to local frames of $E$.

#### Orthogonal splitting of a vector subbundle

↑ **Parent:** [Vector subbundle](#vector-subbundle)

A [fiber metric](#fiber-metric) on a smooth [vector bundle](#vector-bundle) $E$ gives a smooth [orthogonal projection](hilbert-space.md#orthogonal-projection) $P:E\to F$ onto any [vector subbundle](#vector-subbundle). In a [local frame](#frame-of-a-vector-bundle) of $E$, let $G$ be the metric [matrix](vector-space.md#matrix) and $A$ the columns of a frame of $F$. Then $P=A(A^tGA)^{-1}A^tG$, proving smoothness. The complementary subbundle $F^\perp=\ker P$ maps isomorphically onto the [quotient vector bundle](#quotient-vector-bundle). Explicitly $v\mapsto(Pv,[v])$ is a [vector bundle isomorphism](#vector-bundle-isomorphism) $E\to F\oplus(E/F)$, with inverse $(f,[v])\mapsto f+(I-P)v$. This inverse is independent of the representative $v$, but the splitting depends on the chosen metric.

#### Quotient vector bundle

↑ **Parent:** [Vector subbundle](#vector-subbundle)

For a smooth [vector subbundle](#vector-subbundle) $F\subset E$, the quotient has [fibers](function.md#fiber-of-a-function) $(E/F)_p=E_p/F_p$. Extend a local [frame of a vector bundle](#frame-of-a-vector-bundle) of $F$ to one of $E$; the classes of the complementary frame vectors trivialize the quotient. Adapted [transition functions of a vector bundle](#transition-function-of-a-vector-bundle) are block upper triangular, and their lower-right blocks give the quotient transitions. These are smooth and satisfy the cocycle identity, defining a smooth [vector bundle](#vector-bundle). The projection $E\to E/F$ is a smooth [vector bundle morphism](#vector-bundle-morphism).

##### Universal quotient bundle on a real Grassmannian

↑ **Parent:** [Quotient vector bundle](#quotient-vector-bundle)

Over $\operatorname{Gr}_k(\mathbb R^N)$, quotient the trivial bundle by the [tautological bundle](#tautological-bundle). The quotient is a vector bundle because it identifies continuously with the orthogonal-complement bundle via $[v]\mapsto P_{W^\perp}v$. Its rank is $N-k$.

###### Universal quotient bundle need not have a nowhere-zero section

↑ **Parent:** [Universal quotient bundle on a real Grassmannian](#universal-quotient-bundle-on-a-real-grassmannian)

Over $\operatorname{Gr}_1(\mathbb R^2)=\mathbb{RP}^1$, the universal quotient is the orthogonal-complement line bundle, a [Möbius line bundle](#mobius-line-bundle). Writing a section as $a(\theta)(-\sin\theta,\cos\theta)$ forces $a(\theta+\pi)=-a(\theta)$. Continuity then forces a zero, so no [nowhere-zero section](#nowhere-zero-section) exists.

###### Classification of vector bundles by a universal quotient bundle

↑ **Parent:** [Universal quotient bundle on a real Grassmannian](#universal-quotient-bundle-on-a-real-grassmannian)

On a compact base, finitely many global sections can be selected to span every fiber when evaluations of global sections are surjective. They give a surjective morphism $M\times\mathbb R^N\to E$. Its kernel is a [kernel bundle of a surjective vector bundle morphism](#kernel-bundle-of-a-surjective-vector-bundle-morphism), and its fibers give the displayed map $\phi$. The first isomorphism theorem on each fiber identifies the resulting pullback quotient with $E$, with continuously varying inverses. The finite selection follows by choosing a frame's values at each point, extending each value to a global section, then taking a finite cover of the regions where those sections remain independent.

### Trivial vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

A rank-$d$ vector bundle is trivial when it is isomorphic over its base $B$ to the product bundle $B\times\mathbb R^d\to B$. Equivalently, it admits a global frame of $d$ pointwise linearly independent sections.

### Section of a vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

This is a [section of a fiber bundle](#section-fiber-bundle) whose fibers are [vector spaces](vector-space.md).

A section of a vector bundle $\pi:E\to B$ is a map $s:B\to E$ satisfying $\pi\circ s=\operatorname{id}_B$.

#### Regular zero locus

↑ **Parent:** [Section of a vector bundle](#section-of-a-vector-bundle)

The zero locus of a holomorphic [section of a vector bundle](#section-of-a-vector-bundle) of a rank-$r$ bundle is regular when its derivative has rank $r$ along the locus. Its kernel is then the tangent bundle of the smooth zero set. Smoothness of the underlying set alone is insufficient: the square of a reduced defining function has the same set of zeros but zero derivative there.

#### Module of smooth sections

↑ **Parent:** [Section of a vector bundle](#section-of-a-vector-bundle)

The smooth [sections of a vector bundle](#section-of-a-vector-bundle) form a [module](module-theory.md#module-mathematics) over the [commutative ring](commutative-algebra.md#commutative-ring) $C^\infty(M)$ by pointwise multiplication. A [vector bundle morphism](#vector-bundle-morphism) over the identity induces a $C^\infty(M)$-linear map between these modules. [Bundle morphisms from maps of smooth sections](#bundle-morphisms-from-maps-of-smooth-sections) gives the converse, without assuming the bundle has a global frame.

#### Nowhere-zero section

↑ **Parent:** [Section of a vector bundle](#section-of-a-vector-bundle)

A nowhere-zero section of a vector bundle is a section $s$ with $s(x)\ne0$ in every fiber. Every trivial vector bundle of positive rank has one.

##### Nonvanishing tangent field on an odd-dimensional sphere

↑ **Parent:** [Nowhere-zero section](#nowhere-zero-section)

Identify $\mathbb R^{2m+2}$ with $\mathbb C^{m+1}$ and let $J$ be multiplication by $i$. On the unit sphere $S^{2m+1}$, the [vector field](calculus.md#vector-field) $V(x)=Jx$ has norm one and satisfies $\langle x,Jx\rangle=0$. It is therefore a continuous tangent [nowhere-zero section](#nowhere-zero-section), including on $S^1$.

##### Splitting a trivial line from a nowhere-zero section

↑ **Parent:** [Nowhere-zero section](#nowhere-zero-section)

A unit [nowhere-zero section](#nowhere-zero-section) $\sigma$ of a real [vector bundle](#vector-bundle) with a [fiber metric](#fiber-metric) defines a rank-one [trivial vector bundle](#trivial-vector-bundle). Its fiberwise [orthogonal complement](hilbert-space.md#orthogonal-complement) is a subbundle: locally complete $\sigma$ to an orthonormal frame. The [vector bundle isomorphism](#vector-bundle-isomorphism) $(v,t)\mapsto v+t\sigma$ has inverse $w\mapsto(w-\langle w,\sigma\rangle\sigma,\langle w,\sigma\rangle)$. For an oriented bundle, orient the complement so that its positive frame followed by $\sigma$ is positive.

##### Hairy ball theorem

↑ **Parent:** [Nowhere-zero section](#nowhere-zero-section)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hairy_ball_theorem)

The hairy ball theorem says that every continuous tangent vector field on an even-dimensional sphere vanishes somewhere. Equivalently, the tangent bundle of an even-dimensional sphere has no nowhere-zero section.

###### Degree proof of the hairy ball theorem

↑ **Parent:** [Hairy ball theorem](#hairy-ball-theorem)

A nowhere-zero tangent [vector field](calculus.md#vector-field) on $S^n$ can be normalized to a unit field $w(x)$ perpendicular to $x$. Then $\cos(\pi t)x+\sin(\pi t)w(x)$ is a homotopy from the identity to the [antipodal map](homology.md#antipodal-map). Their [mapping degrees](homology.md#degree-of-a-continuous-mapping) are $1$ and $(-1)^{n+1}$, respectively, contradicting [homotopy invariance of mapping degree](homology.md#homotopy-invariance-of-mapping-degree) when $n$ is positive and even. For $S^0$ the tangent spaces are zero, so every tangent field is zero directly.

### Sphere bundle

↑ **Parent:** [Vector bundle](#vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sphere_bundle)

After choosing a fiber metric on a rank-$d$ [vector bundle](#vector-bundle) $E\to B$, its sphere bundle consists of the unit vectors and has fiber $S^{d-1}$. Different choices of metric give isomorphic sphere bundles.

#### Three-sphere bundle over the four-sphere

↑ **Parent:** [Sphere bundle](#sphere-bundle)

For an oriented rank-four real [vector bundle](#vector-bundle) $E\to S^4$, its [sphere bundle](#sphere-bundle) has fibre $S^3$. Let $m=\langle e(E),[S^4]\rangle$ be its [Euler class](#euler-class-of-a-vector-bundle) evaluated on the orientation class. The [Gysin sequence](#gysin-sequence-of-a-sphere-bundle) gives integral [homology](homology.md) $\mathbb Z$ in degrees $0,7$, $\mathbb Z/m\mathbb Z$ in degree $3$, and a copy of $\mathbb Z$ in degree $4$ exactly when $m=0$, with all other groups zero. Here $\mathbb Z/0\mathbb Z=\mathbb Z$. A transition function $v\mapsto q^k vq^l$ on the [unit quaternions](algebra.md#unit-quaternion) has Euler number $k+l$, up to an overall orientation sign: evaluating it at a fixed unit vector gives the power map $q\mapsto q^{k+l}$, whose [mapping degree](homology.md#degree-of-a-continuous-mapping) is $k+l$. The same homology calculation follows by applying the [Mayer–Vietoris sequence](algebraic-topology.md#mayer-vietoris-sequence) to the two trivializations over the hemispheres.

#### Unit tangent bundle

↑ **Parent:** [Sphere bundle](#sphere-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unit_tangent_bundle)

The unit tangent bundle of a Riemannian manifold $M$ is the [sphere bundle](#sphere-bundle) of its [tangent bundle](#tangent-bundle). Its points are pairs $(x,v)$ with $x\in M$, $v\in T_xM$, and $\lVert v\rVert=1$.

##### Canonical coframe of a surface unit tangent bundle

↑ **Parent:** [Unit tangent bundle](#unit-tangent-bundle)

On an oriented Riemannian surface, set $\alpha(\xi)=\langle v,d\pi\xi\rangle$, $\theta(\xi)=\langle iv,d\pi\xi\rangle$, and let $\omega$ be the Levi-Civita connection form with $\omega(V)=1$. The dual frame is $(X,H,V)$ and

$$
d\alpha=\omega\wedge\theta,\qquad d\theta=\alpha\wedge\omega,\qquad d\omega=-K\alpha\wedge\theta.
$$

In a local oriented frame, $\omega=d\vartheta+\omega_0$ and $\alpha,\theta$ are the base coframe rotated through angle $\vartheta$; the torsion-free and curvature equations give these identities. Evaluating exterior derivatives on dual fields yields $[V,X]=H$, $[V,H]=-X$, $[X,H]=KV$.

###### Vertical vector field of a surface unit tangent bundle

↑ **Parent:** [Canonical coframe of a surface unit tangent bundle](#canonical-coframe-of-a-surface-unit-tangent-bundle)

On an oriented [Riemannian surface](riemannian-geometry.md#riemannian-surface), the vertical vector field generates positive rotation in each fibre of its [unit tangent bundle](#unit-tangent-bundle): $Vf(x,v)=\left.\partial_t f(x,\cos t\,v+\sin t\,iv)\right|_{t=0}$. Hence $V(v)=iv$ and $V(iv)=-v$. In the canonical frame, $[V,X]=H$, $[V,H]=-X$ and $[X,H]=KV$.

###### Liouville volume of a surface geodesic flow

↑ **Parent:** [Canonical coframe of a surface unit tangent bundle](#canonical-coframe-of-a-surface-unit-tangent-bundle)

The positive Liouville volume for the base-orientation/positive-fibre orientation is $\mu=\pi^*\Omega_a\wedge\omega$. Its fibre integral is $2\pi\Omega_a$, so its total volume is $2\pi\operatorname{Area}(M)$. With the stated coframe convention, $\alpha\wedge d\alpha=-\mu$; the signed contact volume and the positive measure should not be confused. The fields $X,H,V$ preserve this volume by their structure equations.

##### Stiefel manifold

↑ **Parent:** [Unit tangent bundle](#unit-tangent-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stiefel_manifold)

The real Stiefel manifold $V_k(\mathbb R^n)$ consists of ordered orthonormal $k$-frames in $\mathbb R^n$. In particular, $V_2(\mathbb R^{m+1})$ is naturally the [unit tangent bundle](#unit-tangent-bundle) of $S^m$.

###### Unordered Stiefel bundle

↑ **Parent:** [Stiefel manifold](#stiefel-manifold)

For a rank-$n$ Euclidean [vector bundle](#vector-bundle), take its ordered orthonormal $k$-frame bundle and quotient by the symmetric group permuting the $k$ vectors. The whole fiber is generally positive-dimensional. A prescribed global framing selects a finite subcover consisting of the unordered $k$-element subsets of its distinguished frame vectors.

###### Subset cover of a framed vector bundle

↑ **Parent:** [Unordered Stiefel bundle](#unordered-stiefel-bundle)

A global ordered framing selects the displayed $\binom nk$-sheeted cover inside the [unordered Stiefel bundle](#unordered-stiefel-bundle). It is a trivial cover because the frame labels are global. Selecting subsets of a direct-sum framing decomposes the cover as the disjoint union of fiber products of the two summands' subset covers.

###### Complex Stiefel manifold

↑ **Parent:** [Stiefel manifold](#stiefel-manifold)

The space of ordered orthonormal complex $k$-frames in $\mathbb C^n$, for $0\leq k\leq n$. It is a compact [smooth manifold](differential-geometry.md#smooth-manifold) of real dimension $2nk-k^2$. Completing a frame to a unitary basis gives the displayed homogeneous-space description; $V_0$ is a point and $V_n(\mathbb C^n)$ is the [unitary group](topological-group.md#unitary-group) $U(n)$.

###### Integral cohomology of a complex Stiefel manifold

↑ **Parent:** [Complex Stiefel manifold](#complex-stiefel-manifold)

Use the [complement bundle on a complex Stiefel manifold](#complement-bundle-on-a-complex-stiefel-manifold) inductively. If the ring for $V_k$ is exterior with smallest positive degree $2n-2k+1$, the complement bundle has Euler degree $2(n-k)$, in which base cohomology vanishes. Its Euler class is consequently zero. The [Gysin ring splitting for an odd-dimensional sphere bundle](#gysin-ring-splitting-for-an-odd-dimensional-sphere-bundle) adds one exterior generator of degree $2(n-k)-1$. The initial base $V_0$ is a point. This gives the full integral [cohomology ring](cohomology.md#cohomology-ring) and in particular its torsion-freeness. At $k=n$, the [unitary group](topological-group.md#unitary-group) has Poincare polynomial $\prod_{j=0}^{n-1}(1+t^{2j+1})$.

###### Complement bundle on a complex Stiefel manifold

↑ **Parent:** [Complex Stiefel manifold](#complex-stiefel-manifold)

The orthogonal complements of the universal frames define a [complex vector bundle](#complex-vector-bundle) of rank $n-k$ inside the trivial $\mathbb C^n$ bundle. The orthogonal projector $I-\sum_i v_iv_i^*$ is smooth of constant rank, giving local bundle frames. Its underlying real bundle has canonical orientation and rank $2(n-k)$. Its [sphere bundle](#sphere-bundle) is exactly $V_{k+1}(\mathbb C^n)$, by appending the unit vector in the complement to the frame.

##### Cohomology of the unit tangent bundle of an even-dimensional sphere

↑ **Parent:** [Unit tangent bundle](#unit-tangent-bundle)

The Euler class of $TS^{2n}$ evaluates to $2$. Its [Gysin sequence of a sphere bundle](#gysin-sequence-of-a-sphere-bundle) gives

$$
H^q(STS^{2n};\mathbb Z)\cong
\begin{cases}
\mathbb Z,&q=0,4n-1,\\
\mathbb Z/2,&q=2n,\\
0,&\text{otherwise}.
\end{cases}
$$

All products of positive-degree classes vanish.

### Disk bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

The disk bundle of a metric [vector bundle](#vector-bundle) consists of the vectors of norm at most one. Its boundary is the [sphere bundle](#sphere-bundle) $S(E)$, and radial contraction makes $D(E)$ homotopy equivalent to its zero section.

#### Plumbing of oriented disk bundles

↑ **Parent:** [Disk bundle](#disk-bundle)

Plumbing identifies a base disk times a fiber disk in one oriented rank-two [disk bundle](#disk-bundle) with such a neighborhood in another, exchanging base and fiber coordinates. Their zero sections then intersect transversely once. For disk bundles over $S^2$ arranged along a chain with Euler numbers $-a_i$, the [intersection form](homology.md#intersection-form) has diagonal entries $-a_i$, adjacent entries one and other entries zero. The same manifold has a [Kirby diagram](knot-theory.md#kirby-diagram) consisting of adjacent Hopf-linked unknots with framings $-a_i$. Its boundary is described by the corresponding [negative continued fraction](number-theory.md#negative-continued-fraction), with the orientation fixed by the surgery convention.

### Tangent bundle

↑ **Parent:** [Vector bundle](#vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tangent_bundle)

The tangent bundle of a [smooth manifold](differential-geometry.md#smooth-manifold) $M$ is the [vector bundle](#vector-bundle) whose fiber over $p$ is the tangent space $T_pM$.

#### Stabilized tangent bundle of real projective space

↑ **Parent:** [Tangent bundle](#tangent-bundle)

For the real [tautological bundle](#tautological-bundle) $\gamma$ over [Real projective space](algebraic-topology.md#real-projective-space), the tangent space at a line is $\operatorname{Hom}(\gamma,\gamma^\perp)$. Adding $\operatorname{Hom}(\gamma,\gamma)\cong\varepsilon^1$ gives $\operatorname{Hom}(\gamma,\varepsilon^{m+1})\cong(m+1)\gamma$, using a metric to identify a real line with its dual. Hence its total [Stiefel–Whitney class](#stiefel-whitney-class) is $(1+a)^{m+1}$, with $a=w_1(\gamma)$.

#### Tangent coordinate transition

↑ **Parent:** [Tangent bundle](#tangent-bundle)

A [coordinate chart](differential-geometry.md#manifold-chart) $x$ trivializes the [tangent bundle](#tangent-bundle) by expressing $v\in T_pM$ in the coordinate [basis](vector-space.md#basis). For $y=f(x)$, the [chain rule](calculus.md#chain-rule) gives the displayed transition. Smoothness and fibrewise linear invertibility of the [Jacobian matrix](calculus.md#jacobian-matrix) construct the natural smooth [vector bundle](#vector-bundle) structure. The chain rule also supplies the transition cocycle.

### Projectivization of a real vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

The projectivization $\mathbb P(E)\to B$ has fiber over $b$ equal to the space of one-dimensional linear subspaces of $E_b$.

#### Tangent bundle of a projectivized real vector bundle

↑ **Parent:** [Projectivization of a real vector bundle](#projectivization-of-a-real-vector-bundle)

Let $p:\mathbb P(E)\to M$, let $L_E$ be the tautological line, and let $\omega_E$ be its orthogonal complement in $p^*E$. Then

$$
T\mathbb P(E)\cong p^*TM\oplus\operatorname{Hom}(L_E,\omega_E).
$$

The second summand is the vertical tangent bundle.

#### Projectivization of copies of the real tautological line bundle

↑ **Parent:** [Projectivization of a real vector bundle](#projectivization-of-a-real-vector-bundle)

Tensoring a fixed line with $\mathbb R^k$ does not change its projective directions, so

$$
\mathbb P(k\gamma_{\mathbb R}^{1,n+1})
\cong\mathbb{RP}^n\times\mathbb{RP}^{k-1}.
$$

If $x$ and $v$ are the degree-one generators from the two factors, then the tautological line over this projective bundle has first Stiefel–Whitney class $x+v$.

### Dual bundle

↑ **Parent:** [Vector bundle](#vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_bundle)

The dual bundle $E^*$ has fibre $\operatorname{Hom}(E_x,\mathbb F)$ over $x$. Its transition matrices are the inverse transposes of those of $E$.

#### Canonical trivialization of a line bundle tensored with its dual

↑ **Parent:** [Dual bundle](#dual-bundle)

For a real or complex [line bundle](ringed-space.md#line-bundle) $L$, the evaluation isomorphism $L^*\otimes L\cong\operatorname{End}(L)$ identifies the identity endomorphisms with a nowhere-zero global section. Consequently $L^*\otimes L$ is trivial.

### Pullback vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pullback_vector_bundle)

For a smooth map $f:M\to B$ and a vector bundle $\pi:E\to B$, the pullback bundle is

$$
f^*E=\{(p,v)\in M\times E:f(p)=\pi(v)\}.
$$

Pulling back local trivializations of $E$ makes it a vector bundle over $M$ whose transition functions are the original transition functions composed with $f$.

#### Pullback tangent bundle

↑ **Parent:** [Pullback vector bundle](#pullback-vector-bundle)

For a [smooth map between manifolds](differential-geometry.md#smooth-map-between-manifolds) $f:M\to N$, the [pullback vector bundle](#pullback-vector-bundle) $f^*TN$ has fibre $T_{f(p)}N$ at $p\in M$. A smooth section is a [vector field along a map](#vector-field-along-a-map). It allows one to differentiate maps and curves without requiring them to be invertible.

##### Vector field along a map

↑ **Parent:** [Pullback tangent bundle](#pullback-tangent-bundle)

A vector field along a [smooth map between manifolds](differential-geometry.md#smooth-map-between-manifolds) $f:M\to N$ assigns $Y_p\in T_{f(p)}N$ smoothly to each $p$. It is a section of the [pullback tangent bundle](#pullback-tangent-bundle), not necessarily a vector field on $N$. Along a curve $\gamma$, the velocity $\dot\gamma$ is such a section.

###### Local extension of a vector field along a submanifold

↑ **Parent:** [Vector field along a map](#vector-field-along-a-map)

For an embedded [submanifold](differential-geometry.md#submanifold) $i:M\hookrightarrow N$, a smooth [section of a vector bundle](#section-of-a-vector-bundle) $X\in\Gamma(i^*TN)$ locally extends to an ambient [vector field](calculus.md#vector-field). In an adapted chart $M=\{y=0\}$, extend each component $X^a(x)$ independently of the transverse coordinates $y$. If $X$ takes values in $TM$, the extension criterion is $(\widetilde XF)|_M=X(F|_M)$ for every local smooth function $F$ on $N$. Testing coordinate functions suffices. For tangent fields $X,Y$, this criterion also proves $[\widetilde X,\widetilde Y]|_M=[X,Y]$. General fields with normal components have no extension-independent ambient [Lie bracket](lie-algebra.md#lie-bracket).

// Target: riemannian-geometry.bigb

###### Vector field along a curve

↑ **Parent:** [Vector field along a map](#vector-field-along-a-map)

A vector field along a curve $\gamma:I\to M$ is a smooth [section of a vector bundle](#section-of-a-vector-bundle) with $V(t)\in T_{\gamma(t)}M$. Its values may differ at distinct times mapping to the same base point. The [covariant derivative along a curve](#covariant-derivative-along-a-curve) differentiates its time-dependent coefficients using the pulled-back [connection on a vector bundle](#connection-vector-bundle); it does not require extending it to one ambient vector field.

### Kernel bundle of a constant-rank family of linear maps

↑ **Parent:** [Vector bundle](#vector-bundle)

Let $A_b:V\to W$ vary smoothly with $b$ and have constant rank $r$. The spaces $\ker A_b$ form a [vector bundle](#vector-bundle) of rank $\dim V-r$. On a neighborhood where one $r$ by $r$ minor is invertible, the corresponding coordinates are smooth linear functions of the remaining coordinates, giving a local trivialization.

### Tensor product of vector bundles

↑ **Parent:** [Vector bundle](#vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tensor_product_of_vector_bundles)

The tensor product of vector bundles is formed fiberwise. Tensor products of local trivializations have transition functions given by tensor products of the original transition matrices.

#### Second Chern class of a tensor product of rank-two bundles

↑ **Parent:** [Tensor product of vector bundles](#tensor-product-of-vector-bundles)

The [splitting principle for complex vector bundles](algebraic-topology.md#splitting-principle-for-complex-vector-bundles) makes pullback injective in integral [cohomology](cohomology.md) and splits both bundles into lines with [Chern roots](algebraic-topology.md#chern-root) $x_1,x_2$ and $y_1,y_2$. The tensor product has roots $x_i+y_j$. Expanding their six pairwise products gives the displayed formula. This integral computation does not divide by two, so it remains valid when the [cohomology](cohomology.md) has two-torsion. In particular, taking $F$ trivial gives $c_2(E\oplus E)=c_1(E)^2+2c_2(E)$.

#### Tensor field

↑ **Parent:** [Tensor product of vector bundles](#tensor-product-of-vector-bundles)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tensor_field)

A [tensor field](#tensor-field) is a smooth [section of a vector bundle](#section-of-a-vector-bundle) formed from [tensor products](linear-algebra.md#tensor-product) of the [tangent bundle](#tangent-bundle) and [cotangent bundle](symplectic-geometry.md#cotangent-bundle). With $k$ covector factors and $l$ vector factors it belongs to

$$
\Gamma\bigl((T^*M)^{\otimes k}\otimes(TM)^{\otimes l}\bigr).
$$

Its coefficients in any local frame vary smoothly. Different conventions list the two counts in different orders, so the factor order should be specified. [Tensor contractions](linear-algebra.md#tensor-contraction) use the canonical evaluation of a covector on a vector and are independent of the frame.

##### Lie derivative of a covariant tensor field

↑ **Parent:** [Tensor field](#tensor-field)

For a covariant rank-two [tensor field](#tensor-field), pull back by the flow of a vector field $\xi$ and differentiate at zero flow time. Differentiating the evaluation point produces the first term above; differentiating the two coordinate Jacobians produces the remaining terms. In particular this formula gives the change in a [metric tensor](general-relativity.md#metric-tensor) under an infinitesimal coordinate displacement. A perturbation defined relative to a fixed background consequently transforms as $q_{\mu\nu}\mapsto q_{\mu\nu}-\mathcal L_\xi\bar g_{\mu\nu}$ in the passive displacement convention. The formula applies to symmetric tensors as well as differential forms; tensor symmetry does not make the antisymmetric differential-form formula its definition.

##### Tensoriality

↑ **Parent:** [Tensor field](#tensor-field)

A [multilinear](linear-algebra.md#multilinear-map) operation on [vector fields](calculus.md#vector-field) is [tensorial](#tensoriality) when it is [linear](vector-space.md#linearity) over [smooth functions](analysis.md#smooth-function) in every argument. Its value at a point then depends only on the argument [vectors](vector-space.md#vector) at that point. To see this, use a [smooth cutoff function](analysis.md#smooth-cutoff-function) to reduce to local fields, expand them in a [local frame](#frame-of-a-vector-bundle), and apply [linearity](vector-space.md#linearity) over [smooth functions](analysis.md#smooth-function) to their coefficients. A smoothly valued [tensorial](#tensoriality) operation therefore defines a [tensor field](#tensor-field). The [curvature](differential-geometry.md#curvature) of an [affine connection](#affine-connection) is [tensorial](#tensoriality), whereas a [covariant derivative](general-relativity.md#covariant-derivative) differentiates a [scalar](vector-space.md#scalar) coefficient in its second argument and is not [tensorial](#tensoriality) there.

##### Tensor derivation

↑ **Parent:** [Tensor field](#tensor-field)

A [tensor derivation](#tensor-derivation) is a real-linear operation preserving every tensor type, obeying the tensor-product [Leibniz rule](calculus.md#leibniz-rule), and commuting with every [tensor contraction](linear-algebra.md#tensor-contraction). A derivation $D$ of [smooth functions](analysis.md#smooth-function) and a real-linear operator on [vector fields](calculus.md#vector-field) satisfying $D(fY)=fDY+(Df)Y$ extend uniquely to a [tensor derivation](#tensor-derivation). On a [differential one-form](differential-form.md#one-form) it must satisfy

$$
(D\omega)(Y)=D(\omega(Y))-\omega(DY).
$$

This expression is linear over [smooth functions](analysis.md#smooth-function) in $Y$. In a local frame $De_a=A^b{}_ae_b$, the dual rule is $D\epsilon^a=-A^a{}_b\epsilon^b$. Apply the product rule to every coefficient and frame factor to define the extension; these dual signs cancel under contraction. Frame changes agree by differentiating the inverse [matrix](vector-space.md#matrix). Cutoffs prove locality and hence uniqueness from local expansions.

###### Lie derivative of a tensor field

↑ **Parent:** [Tensor derivation](#tensor-derivation)

For a smooth [vector field](calculus.md#vector-field) $X$, the Lie derivative is the [tensor derivation](#tensor-derivation) determined by $\mathcal L_Xf=X(f)$ and $\mathcal L_XY=[X,Y]$. The identity $[X,fY]=f[X,Y]+X(f)Y$ permits its unique extension. On a [differential one-form](differential-form.md#one-form),

$$
(\mathcal L_X\omega)(Y)=X(\omega(Y))-\omega([X,Y]).
$$

On [differential forms](differential-form.md) it agrees with the usual [Lie derivative of a differential form](differential-form.md#lie-derivative-of-a-differential-form) and [Cartan's magic formula](differential-form.md#cartan-s-magic-formula).

###### Lie derivative at a zero of its generator

↑ **Parent:** [Lie derivative of a tensor field](#lie-derivative-of-a-tensor-field)

The [tensor Lie derivative](#lie-derivative-of-a-tensor-field) need not vanish at a point where its generating [vector field](calculus.md#vector-field) vanishes. For $X=x\partial_x$, the local flow fixes zero but its differential rescales tangent vectors; $\mathcal L_Xdx=dx$ even there. Straightening coordinates exist only at nonzero generator points. The flow definition remains valid at zeros and includes derivatives of the generator acting on tensor slots.

###### Coordinate tensor Lie derivative

↑ **Parent:** [Lie derivative of a tensor field](#lie-derivative-of-a-tensor-field)

For every contravariant slot of a [tensor field](#tensor-field), the [tensor Lie derivative](#lie-derivative-of-a-tensor-field) contributes a negative derivative of its generating [vector field](calculus.md#vector-field); every covariant slot contributes a positive one. The remaining term differentiates the tensor's components along the generator. This follows from the [flow definition of the Lie derivative of a tensor field](#flow-definition-of-the-lie-derivative-of-a-tensor-field) and its product and contraction rules, without choosing a [affine connection](#affine-connection).

###### Commutator identity for Lie derivatives

↑ **Parent:** [Lie derivative of a tensor field](#lie-derivative-of-a-tensor-field)

The [Lie derivative of a tensor field](#lie-derivative-of-a-tensor-field) satisfies $[\mathcal L_X,\mathcal L_Y]=\mathcal L_{[X,Y]}$. On [smooth functions](analysis.md#smooth-function) this is the definition of the [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields); on [vector fields](calculus.md#vector-field) it follows from the [Jacobi identity](lie-algebra.md#jacobi-identity). The [Leibniz rule](calculus.md#leibniz-rule) and contraction compatibility extend the equality to [tensor fields](#tensor-field). The cyclic double-commutator identity also follows directly from associativity of operator composition.

###### Lie derivative of a vector field

↑ **Parent:** [Lie derivative of a tensor field](#lie-derivative-of-a-tensor-field)

For [vector fields](calculus.md#vector-field) $X,Y$, the Lie derivative is the [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields) $\mathcal L_XY=[X,Y]$. Pulling $Y$ back by the [local flow](differential-geometry.md#local-flow) of $X$ and differentiating gives $dY(X)-dX(Y)$. No [affine connection](#affine-connection) is needed.

###### Lie derivative of a function

↑ **Parent:** [Lie derivative of a tensor field](#lie-derivative-of-a-tensor-field)

For a [smooth function](analysis.md#smooth-function) $f$ and a [vector field](calculus.md#vector-field) $X$, the Lie derivative is $\mathcal L_Xf=X(f)=df(X)$. It is the derivative of $f$ along the [local flow](differential-geometry.md#local-flow) of $X$.

###### Flow definition of the Lie derivative of a tensor field

↑ **Parent:** [Lie derivative of a tensor field](#lie-derivative-of-a-tensor-field)

For the [local flow](differential-geometry.md#local-flow) $\phi_t$ of a smooth [vector field](calculus.md#vector-field) $X$, pull a [tensor field](#tensor-field) $T$ back to the fixed base point before differentiating. Pullback uses $d\phi_t^{-1}$ on vector factors and the dual of $d\phi_t$ on covector factors. The [chain rule](calculus.md#chain-rule) gives $\mathcal L_Xf=Xf$. In coordinates, $d\phi_t^{-1}Y(\phi_t(x))=Y+t(dY\,X-dX\,Y)+O(t^2)$, so $\mathcal L_XY=[X,Y]$. Differentiation of pullback preserves [tensor contractions](linear-algebra.md#tensor-contraction) and obeys the [Leibniz rule](calculus.md#leibniz-rule) for [tensor products](linear-algebra.md#tensor-product); hence this is the [tensor derivation](#tensor-derivation) defining the [Lie derivative of a tensor field](#lie-derivative-of-a-tensor-field).

###### Scaled Lie derivative defect identity

↑ **Parent:** [Lie derivative of a tensor field](#lie-derivative-of-a-tensor-field)

For a [smooth function](analysis.md#smooth-function) $f$ and [vector field](calculus.md#vector-field) $X$,

$$
f\mathcal L_X-\mathcal L_{fX}=D_{X\otimes df}
$$

on every [tensor field](#tensor-field), with $X\otimes df$ interpreted as the [endomorphism](algebra.md#endomorphism) $Y\mapsto Y(f)X$. Both sides vanish on functions; on [vector fields](calculus.md#vector-field) this follows from $[fX,Y]=f[X,Y]-Y(f)X$. Both are contraction-compatible [tensor derivations](#tensor-derivation), so agreement on functions and [vector fields](calculus.md#vector-field) proves equality on all tensor types. In particular $\mathcal L_{fX}\omega=f\mathcal L_X\omega+\omega(X)df$.

###### Endomorphism-induced tensor derivation

↑ **Parent:** [Tensor derivation](#tensor-derivation)

A smooth [endomorphism](algebra.md#endomorphism) $A$ of the [tangent bundle](#tangent-bundle) defines the [tensor derivation](#tensor-derivation) $D_A$ by $D_Af=0$ and $D_AY=A(Y)$. On a [differential one-form](differential-form.md#one-form), $D_A\omega=-\omega\circ A$. On a general [tensor field](#tensor-field), it acts by $A$ in each vector factor and by the negative dual action in each covector factor. The two actions cancel in each contracted pairing, proving compatibility with [tensor contraction](linear-algebra.md#tensor-contraction).

### Connection (vector bundle)

↑ **Parent:** [Vector bundle](#vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Connection_(vector_bundle))

A connection is a linear map $\nabla:\Gamma(E)\to\Omega^1(B;E)$ satisfying $\nabla(fs)=df\otimes s+f\nabla s$. In a local frame it has the form $d+A$ for a matrix-valued one-form $A$.

#### Parallel vector field

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

A [vector field](calculus.md#vector-field) is parallel for a specified [connection on a vector bundle](#connection-vector-bundle) on the [tangent bundle](#tangent-bundle) when its [covariant derivative](general-relativity.md#covariant-derivative) in every direction vanishes. Its values along every [smooth curve](differential-geometry.md#smooth-curve) are related by [parallel transport](#parallel-transport). For a [Levi-Civita connection](general-relativity.md#levi-civita-connection), its length is constant on each [connected component](geometry-and-topology.md#connected-component), since the connection preserves the [Riemannian metric](differential-geometry.md#riemannian-metric).

#### Projection connection

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

A smooth self-adjoint [projection](vector-space.md#projection-linear-algebra) $p:M\to M_N(\mathbb C)$ of locally constant rank defines the [Hermitian vector bundle](#hermitian-vector-bundle) $\operatorname{im}p$ inside the trivial bundle. Projecting the flat derivative gives the [unitary connection](#unitary-connection) $\nabla s=p\,ds$ for $ps=s$. Differentiating $p^2=p$ gives $p\,dp=dp(1-p)$ and $p\,dp\,p=0$. For a section $s$, $\nabla^2s=p\,dp\wedge ds=p(dp)^2s$, proving the curvature formula. Relative to $\operatorname{im}p\oplus\ker p$, $dp$ is off-diagonal and $(dp)^2$ is diagonal. Therefore $d\operatorname{tr}(p(dp)^{2k})=\operatorname{tr}(dp)^{2k+1}=0$. These are explicit closed representatives of the [Chern character](algebraic-topology.md#chern-character).

#### Connection difference as an endomorphism-valued one-form

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

The [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule) terms of two connections cancel, making their difference $C^\infty$-linear in the section. It is therefore an element of $A^1(\operatorname{End}E)$. Conversely adding any such form to a connection gives another connection, making the space of connections an [affine space](geometry-and-topology.md#affine-space).

#### Change of frame of a vector-bundle connection

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

With local frame written as a row $e$ and $D(eu)=e(du+Au)$, a change $e'=eg$ gives $A'=g^{-1}Ag+g^{-1}dg$. The [vector-bundle curvature](#curvature-form) transforms by conjugation. This convention makes the inhomogeneous derivative term and every subsequent [vector-bundle curvature](#curvature-form) sign explicit.

#### Affine space of vector-bundle connections

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

The difference of two [connections on a vector bundle](#connection-vector-bundle) is a smooth one-form with values in the endomorphism bundle: the Leibniz derivative terms cancel, leaving pointwise linearity in both the tangent vector and section value. Conversely every such form added to a connection gives another connection. Thus the collection is an [affine space](geometry-and-topology.md#affine-space) with this model vector space. Choosing $\nabla^0$ supplies a noncanonical origin; there is no distinguished zero connection.

#### Construction of a vector bundle connection by a partition of unity

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

A local trivialization of a smooth [vector bundle](#vector-bundle) gives a local connection by differentiating its component functions. Weight these connections by a subordinate locally finite [partition of unity](differential-geometry.md#partition-of-unity) and extend the weighted terms by zero. The weights sum to one, so the connection Leibniz rule survives. This proves existence on a paracompact smooth manifold. Averaging connections is valid with weights summing to one because the collection is the [affine space of vector-bundle connections](#affine-space-of-vector-bundle-connections).

#### Determinant connection

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

A [connection on a vector bundle](#connection-vector-bundle) induces a connection on its top [exterior power](linear-algebra.md#exterior-power) by differentiating each factor in turn. Its local [connection one-form](#connection-one-form) is $\operatorname{Tr}A$ and its [curvature form of a connection](#curvature-form) is $\operatorname{Tr}\Theta_D$.

#### Rough Laplacian

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

For a metric vector bundle connection over a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), the rough Laplacian is the formally nonnegative connection operator

$$
\nabla^*\nabla=-\sum_i\bigl(\nabla_{e_i}\nabla_{e_i}-\nabla_{\nabla_{e_i}e_i}\bigr),
$$

where $e_i$ is a local orthonormal frame. The correction term makes the expression independent of the orthonormal frame. On a [closed manifold](differential-geometry.md#closed-manifold), integration by parts gives $\langle\nabla^*\nabla s,s\rangle_{L^2}=\|\nabla s\|_{L^2}^2$.

#### Affine connection

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affine_connection)

An affine connection on a [smooth manifold](differential-geometry.md#smooth-manifold) is a [connection on a vector bundle](#connection-vector-bundle) for its [tangent bundle](#tangent-bundle). It satisfies $\nabla_{fX}Y=f\nabla_XY$ and $\nabla_X(fY)=X(f)Y+f\nabla_XY$. Its curvature is

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z.
$$

The [Leibniz rule](calculus.md#leibniz-rule) makes curvature tensorial in all three slots. An affine connection is also called a linear connection on the manifold; a [Levi-Civita connection](general-relativity.md#levi-civita-connection) is the distinguished torsion-free metric-compatible example.

##### Projective equivalence of affine connections

↑ **Parent:** [Affine connection](#affine-connection)

Two [torsion-free connections](#torsion-free-connection) are [projectively equivalent](#projective-equivalence-of-affine-connections) if they have the same unparametrized [geodesics](riemannian-geometry.md#geodesic). Their [difference of affine connections is a tensor](#difference-of-affine-connections-is-a-tensor) $S$. A change of parameter adds only tangential acceleration, so equality of curves requires $S(v,v)$ to be parallel to $v$ for every tangent vector. The [symmetric bilinear diagonal-parallel lemma](linear-algebra.md#symmetric-bilinear-diagonal-parallel-lemma) gives exactly the displayed condition. Conversely the [geodesic reparametrization under projective equivalence](#geodesic-reparametrization-under-projective-equivalence) absorbs this tangential term. Agreement with the same [affine parameters](riemannian-geometry.md#affine-parameter) instead forces $S=0$.

###### Geodesic reparametrization under projective equivalence

↑ **Parent:** [Projective equivalence of affine connections](#projective-equivalence-of-affine-connections)

Let $\tau$ be an [affine parameter](riemannian-geometry.md#affine-parameter) for a [geodesic](riemannian-geometry.md#geodesic) of $\nabla$ and suppose $\bar\nabla_XY-\nabla_XY=V(X)Y+V(Y)X$. Then $\bar\nabla_{\dot\gamma}\dot\gamma=2V(\dot\gamma)\dot\gamma$. For the new velocity $d\gamma/dt=\dot\gamma/t'$, the acceleration is $(t')^{-2}[\bar\nabla_{\dot\gamma}\dot\gamma-(t''/t')\dot\gamma]$, which vanishes under the displayed [differential equation](differential-equation.md). Its nonzero solution $t'=C\exp(2\int V(\dot\gamma)\,d\tau)$ changes the parameter while preserving the curve.

###### Projective covector from metric volume densities

↑ **Parent:** [Projective equivalence of affine connections](#projective-equivalence-of-affine-connections)

For two [projectively equivalent connections](#projective-equivalence-of-affine-connections) that are [Levi-Civita connections](general-relativity.md#levi-civita-connection), contraction of their difference gives $(n+1)V_c=\bar\Gamma^a{}_{ac}-\Gamma^a{}_{ac}$. The [Jacobi formula](linear-algebra.md#jacobi-s-formula) gives $\Gamma^a{}_{ac}=\partial_c\log\sqrt{|\det g|}$. Subtraction proves the displayed expression. The two [determinant](linear-algebra.md#determinant) densities transform by the same coordinate Jacobian factor, so their ratio is a [scalar](vector-space.md#scalar) and its [derivative](calculus.md#derivative) a [covector](linear-algebra.md#covector). The formula is a necessary consequence of projective equivalence, not a test asserting that arbitrary [metric tensors](general-relativity.md#metric-tensor) have identical [geodesics](riemannian-geometry.md#geodesic).

##### Bracket connection on a Lie group

↑ **Parent:** [Affine connection](#affine-connection)

Specify the displayed rule on [left-invariant vector fields](lie-theory.md#left-invariant-vector-field) and extend by the [Leibniz rule](calculus.md#leibniz-rule) to an [affine connection](#affine-connection) on the [Lie group](lie-theory.md#lie-group). In a [left-invariant vector field](lie-theory.md#left-invariant-vector-field) frame $L_i$, the extension is $\nabla_{L_i}(z^jL_j)=L_i(z^j)L_j+\lambda z^j[L_i,L_j]$. Applying the bare bracket formula to arbitrary vector fields instead would violate the [Leibniz rule](calculus.md#leibniz-rule) unless $\lambda=1$. With $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$, the [Jacobi identity](lie-algebra.md#jacobi-identity) gives

$$
T(X,Y)=(2\lambda-1)[X,Y],\qquad R(X,Y)Z=\lambda(\lambda-1)[[X,Y],Z],\qquad \operatorname{Ric}(X,Y)=\lambda(\lambda-1)B(X,Y),
$$

for left-invariant arguments, where $B$ is the [Killing form](lie-algebra.md#killing-form) and $\operatorname{Ric}(X,Y)=\operatorname{tr}(Z\mapsto R(Z,X)Y)$. These identities determine the [tensor fields](#tensor-field) everywhere. The endpoints $\lambda=0,1$ have zero curvature, with respectively left- and right-invariant [parallel frames](#parallel-frame-along-a-curve), and opposite [torsion tensors](#torsion-tensor). The midpoint $\lambda=1/2$ is torsion-free but need not have zero curvature.

##### Connection components

↑ **Parent:** [Affine connection](#affine-connection)

For a local [basis](vector-space.md#basis) $e_a$ of the [tangent bundle](#tangent-bundle), an [affine connection](#affine-connection) has components defined by $\nabla_{e_c}e_b=\Gamma^a{}_{bc}e_a$. If $V=V^be_b$, then $(\nabla_{e_c}V)^a=e_c(V^a)+\Gamma^a{}_{bc}V^b$. The [connection components](#connection-components) depend on the chosen [basis](vector-space.md#basis) and have an inhomogeneous transformation law; they are not themselves a [tensor field](#tensor-field). In a [coordinate basis](differential-geometry.md#coordinate-basis), a [torsion-free connection](#torsion-free-connection) has symmetry in the two lower indices.

##### Affine exponential map

↑ **Parent:** [Affine connection](#affine-connection)

For an [affine connection](#affine-connection), let $\gamma_X$ be the affinely parametrized [geodesic](riemannian-geometry.md#geodesic) starting at $p$ with velocity $X$. Define the exponential map by the displayed formula for initial velocities whose [geodesics](riemannian-geometry.md#geodesic) exist until parameter one. It is defined near zero, has differential equal to the identity there, and obeys $\exp_p(tX)=\gamma_X(t)$ wherever defined. This construction requires no metric and extends the metric [exponential map](riemannian-geometry.md#exponential-map-riemannian-geometry).

###### Affine normal coordinates

↑ **Parent:** [Affine exponential map](#affine-exponential-map)

Identify $T_pM$ with coordinate vectors using a basis and invert the [affine exponential map](#affine-exponential-map) near zero. Radial [geodesics](riemannian-geometry.md#geodesic) then have coordinates $sX$. Their equations imply $\Gamma^\lambda{}_{\mu\nu}(p)X^\mu X^\nu=0$ for every $X$, hence the displayed vanishing of the symmetric part. The antisymmetric part may survive when the [torsion tensor](#torsion-tensor) is nonzero. For a general connection the [Levi-Civita connection](general-relativity.md#levi-civita-connection) coefficients and first metric derivatives need not vanish in these coordinates.

##### Affine connection decomposition

↑ **Parent:** [Affine connection](#affine-connection)

Relative to a nondegenerate [metric tensor](general-relativity.md#metric-tensor), any [affine connection](#affine-connection) is uniquely the [Levi-Civita connection](general-relativity.md#levi-civita-connection) plus a [contorsion tensor](#contorsion-tensor) contribution and a [disformation tensor](#disformation-tensor) contribution. In derivative-last notation, with $T_{ab}{}^c=\Gamma^c{}_{ab}-\Gamma^c{}_{ba}$ and $N_{ab c}=\nabla_cg_{ab}$, the lowered difference is $A_{ab c}=\tfrac12(T_{ab c}+T_{bc a}-T_{ca b}+N_{ab c}-N_{bc a}-N_{ca b})$. This follows by solving $T_{ab c}=A_{ab c}-A_{ba c}$ and $N_{ab c}=-A_{ac b}-A_{bc a}$. The [difference of affine connections is a tensor](#difference-of-affine-connections-is-a-tensor).

##### Nonmetricity tensor

↑ **Parent:** [Affine connection](#affine-connection)

Given a [metric tensor](general-relativity.md#metric-tensor) and an [affine connection](#affine-connection), $N_{ab c}=\nabla_cg_{ab}$ measures failure of [metric compatibility](#metric-compatibility). It is symmetric in $a,b$. Some authors instead define nonmetricity as $-\nabla g$, so formulas must specify the sign. Together with the [torsion tensor](#torsion-tensor), it determines the difference from the [Levi-Civita connection](general-relativity.md#levi-civita-connection).

###### Disformation tensor

↑ **Parent:** [Nonmetricity tensor](#nonmetricity-tensor)

With derivative-last connection coefficients and $N_{ab c}=\nabla_cg_{ab}$, the displayed [tensor](linear-algebra.md#tensor) is the symmetric-in-$a,b$ correction associated with the [nonmetricity tensor](#nonmetricity-tensor). Raising its final slot gives the correction to connection coefficients. It vanishes for [metric compatibility](#metric-compatibility). Reversing the sign used to define nonmetricity reverses this formula.

##### Torsion tensor

↑ **Parent:** [Affine connection](#affine-connection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Torsion_tensor)

The torsion of an [affine connection](#affine-connection) is the displayed antisymmetric [tensor](linear-algebra.md#tensor). It measures the failure of the antisymmetrized [covariant derivative](general-relativity.md#covariant-derivative) to agree with the [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields). With derivative-last coefficients $\nabla_\mu Y^\rho=\partial_\mu Y^\rho+\Gamma^\rho{}_{\nu\mu}Y^\nu$, its components are $\mathcal T^\rho{}_{\mu\nu}=\Gamma^\rho{}_{\nu\mu}-\Gamma^\rho{}_{\mu\nu}$. Some conventions use the negative component tensor. Geodesic equations depend on the symmetric connection coefficients, so they alone cannot detect torsion.

###### Contorsion tensor

↑ **Parent:** [Torsion tensor](#torsion-tensor)

For a metric-compatible [affine connection](#affine-connection), its difference from the [Levi-Civita connection](general-relativity.md#levi-civita-connection) is the contorsion [tensor](linear-algebra.md#tensor). It is determined by the [torsion tensor](#torsion-tensor). In derivative-last notation let $T_{ab}{}^c=\Gamma^c{}_{ab}-\Gamma^c{}_{ba}$, the negative of geometric torsion, and lower the last slot with the [metric tensor](general-relativity.md#metric-tensor). Then $C_{ab c}=\tfrac12(T_{ab c}+T_{bc a}-T_{ca b})$. This is the actual correction added to the [Levi-Civita connection](general-relativity.md#levi-civita-connection); a convention writing $\Gamma=S-K$ has $K=-C$.

##### Parallel covector field

↑ **Parent:** [Affine connection](#affine-connection)

A one-form $k$ with $\nabla_bk_a=0$. If $\ell=d\phi$ satisfies $\nabla_b\ell_a+\ell_a\ell_b=0$, then $k=e^\phi\ell=d(e^\phi)$ is parallel.

##### Projected ambient connection

↑ **Parent:** [Affine connection](#affine-connection)

For a [Riemannian metric](differential-geometry.md#riemannian-metric) on an ambient manifold and an [embedded submanifold](differential-geometry.md#embedded-submanifold), let $\pi:TN|_M\to TM$ be [orthogonal projection](hilbert-space.md#orthogonal-projection). Project the [restriction of a connection to an embedded submanifold](#restriction-of-a-connection-to-an-embedded-submanifold) to obtain $D_XY=\pi\nabla_XY$. Since $\pi Y=Y$, the [Leibniz rule](calculus.md#leibniz-rule) and linearity over [smooth functions](analysis.md#smooth-function) hold, making $D$ an [affine connection](#affine-connection). If the ambient connection is the [Levi-Civita connection](general-relativity.md#levi-civita-connection), pairing with tangent vectors shows that $D$ is a [metric connection](#metric-connection); projecting the zero-torsion identity shows it is a [torsion-free connection](#torsion-free-connection). By uniqueness, $D$ is the induced [Levi-Civita connection](general-relativity.md#levi-civita-connection).

##### Difference of affine connections is a tensor

↑ **Parent:** [Affine connection](#affine-connection)

The difference of two [affine connections](#affine-connection) is a smooth [tensor field](#tensor-field) of type $(1,2)$. Linearity over [smooth functions](analysis.md#smooth-function) holds in the first slot by the connection axioms. In the second slot, the two extra terms $X(f)Y$ cancel, so $\Delta(X,fY)=f\Delta(X,Y)$. This [tensoriality](#tensoriality) makes the value depend only on $X_p,Y_p$. In coordinates its components are the differences of the [Christoffel symbols](riemannian-geometry.md#christoffel-symbol), although either collection of connection coefficients individually is not a tensor.

###### Parametrized geodesics determine the symmetric part of an affine connection

↑ **Parent:** [Difference of affine connections is a tensor](#difference-of-affine-connections-is-a-tensor)

Two [affine connections](#affine-connection) have exactly the same [geodesics](riemannian-geometry.md#geodesic) with the same parameters if and only if their difference tensor vanishes on every diagonal pair $(v,v)$. Indeed, their covariant accelerations differ by $\Delta(\dot\gamma,\dot\gamma)$; starting a [geodesic](riemannian-geometry.md#geodesic) at each arbitrary initial vector proves necessity. Polarization then says that the symmetric part of the difference is zero. This condition is stronger than agreement of [unparametrized geodesic equations](riemannian-geometry.md#unparametrized-geodesic-equation).

###### Torsion-free connections are determined by their parametrized geodesics

↑ **Parent:** [Parametrized geodesics determine the symmetric part of an affine connection](#parametrized-geodesics-determine-the-symmetric-part-of-an-affine-connection)

The difference of two [torsion-free connections](#torsion-free-connection) is symmetric, because subtracting their zero-torsion identities gives $\Delta(X,Y)=\Delta(Y,X)$. Agreement of parametrized [geodesics](riemannian-geometry.md#geodesic) makes this difference skew-symmetric as well, by [parametrized geodesics determine the symmetric part of an affine connection](#parametrized-geodesics-determine-the-symmetric-part-of-an-affine-connection). Over the real numbers it must therefore vanish. Without the torsion-free condition, an arbitrary skew-symmetric difference changes torsion without changing the parametrized [geodesics](riemannian-geometry.md#geodesic).

##### Affine connection for a velocity-linear force

↑ **Parent:** [Affine connection](#affine-connection)

For smooth spatial fields $E^i,C^i{}_j$, define a [torsion-free connection](#torsion-free-connection) on $\mathbb R\times\mathbb R^n$ by $\Gamma^i{}_{00}=-E^i$, $\Gamma^i{}_{0j}=\Gamma^i{}_{j0}=-C^i{}_j/2$ and all other coefficients zero. The time [geodesic equation](riemannian-geometry.md#geodesic-equation) is $\ddot t=0$. For $\dot t\ne0$, use $t$ as [affine parameter](riemannian-geometry.md#affine-parameter); the spatial geodesic equation becomes $d^2x^i/dt^2=E^i+C^i{}_jdx^j/dt$. In dimension three, $C^i{}_j=2\epsilon^i{}_{kj}B^k$ realizes $\ddot{\mathbf x}=\mathbf E+2\mathbf B\times\dot{\mathbf x}$. Such a connection need not preserve a metric; a spacetime description of these trajectories only needs affine geometry.

##### Product affine connection

↑ **Parent:** [Affine connection](#affine-connection)

Connections $\nabla^1,\nabla^2$ on $TM_1,TM_2$ give a connection on

$$
T(M_1\times M_2)\cong p_1^*TM_1\oplus p_2^*TM_2
$$

by taking the direct sum of their [pullback connections](#pullback-connection). In product coordinates its [Christoffel symbols](riemannian-geometry.md#christoffel-symbol) have the two factor blocks and zero mixed blocks. On arbitrary fields, the ordinary derivatives of their coefficients are still taken in both factors. On fields lifted separately from the factors it satisfies $\nabla_{Y_1+Y_2}(X_1+X_2)=\nabla^1_{Y_1}X_1+\nabla^2_{Y_2}X_2$.

###### Curvature splitting for a product connection

↑ **Parent:** [Product affine connection](#product-affine-connection)

For a [product affine connection](#product-affine-connection), its curvature satisfies

$$
R((u_1,u_2),(v_1,v_2))(w_1,w_2)
=(R^1(u_1,v_1)w_1,R^2(u_2,v_2)w_2).
$$

Expand the defining derivative commutator on lifted [vector fields](calculus.md#vector-field). Opposite-factor fields commute and have zero mixed covariant derivatives, leaving exactly the two factor curvatures. Tensoriality gives the formula for arbitrary tangent vectors. Thus the product connection is flat if the two factors are flat; for a [product Riemannian metric](differential-geometry.md#product-riemannian-metric) this applies to its [Levi-Civita connection](general-relativity.md#levi-civita-connection).

#### Covariant derivative along a curve

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

A [connection on a vector bundle](#connection-vector-bundle) pulls back along a smooth curve $\gamma$ to differentiate its time-dependent sections. For the [tangent bundle](#tangent-bundle), a section $V(t)$ of the [pullback tangent bundle](#pullback-tangent-bundle) has

$$
(D_tV)^i=\dot V^i+\Gamma^i{}_{jk}(\gamma(t))\dot\gamma^j V^k.
$$

The [Leibniz rule](calculus.md#leibniz-rule) under a change of frame proves independence of the coordinates. The derivative includes the time dependence of the coefficients, so it is meaningful even at a zero tangent velocity. A [vector field along a map](#vector-field-along-a-map) need not extend to one ambient field if the curve self-intersects. Parallel fields satisfy $D_tV=0$, a [linear ordinary differential equation](differential-equation.md#linear-ordinary-differential-equation) whose unique solutions define [parallel transport](#parallel-transport).

#### Connection one-form

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

In a local frame $e$, a [connection on a vector bundle](#connection-vector-bundle) is written $\nabla e=Ae$, where $A$ is a matrix-valued one-form. Under a change of frame $e'=eg$, it transforms as $A'=g^{-1}Ag+g^{-1}dg$.

#### Exterior covariant derivative

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exterior_covariant_derivative)

The covariant exterior derivative extends a connection to bundle-valued forms by

$$
d_A(s\otimes\alpha)=\nabla s\wedge\alpha+s\otimes d\alpha.
$$

Locally it is $d_A=d+A\wedge$.

##### Endomorphism-valued exterior product

↑ **Parent:** [Exterior covariant derivative](#exterior-covariant-derivative)

Exterior product of [differential forms](differential-form.md) combined with [endomorphism](algebra.md#endomorphism) composition is associative and generally noncommutative. For an endomorphism-valued one-form $a$, $(a\wedge a)(u,v)=[a(u),a(v)]$. The [endomorphism bundle connection](#endomorphism-bundle-connection) extends as a graded derivation of this algebra.

#### Horizontal subspace of a vector bundle connection

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

At $v\in E$, the vertical subspace is $V_vE=\ker(d\pi)_v$. A horizontal subspace is a complement $H_vE$ to $V_vE$. A linear connection is equivalently a smooth choice of such complements compatible with the vector-space structure in the fibres.

##### Linear horizontal distribution on a vector bundle

↑ **Parent:** [Horizontal subspace of a vector bundle connection](#horizontal-subspace-of-a-vector-bundle-connection)

In a local trivialization, a vector-bundle connection with matrix $A$ defines the displayed complement of the vertical tangent space. The frame-change law makes these complements independent of the trivialization. Their dependence on the fiber coordinate is linear; an arbitrary horizontal complement need not satisfy this condition and need not define a [connection on a vector bundle](#connection-vector-bundle). Horizontal lifts satisfy the ordinary differential equation defining [parallel transport](#parallel-transport).

##### Horizontal connection associated to a covariant derivative

↑ **Parent:** [Horizontal subspace of a vector bundle connection](#horizontal-subspace-of-a-vector-bundle-connection)

In a [frame of a vector bundle](#frame-of-a-vector-bundle), write a [vector bundle covariant derivative](#connection-vector-bundle) as $\nabla(e v)=e(dv+\Gamma v)$. The associated horizontal subspace at $(x,v)$ consists of tangent pairs $(\xi,-\Gamma_x(\xi)v)$. Under a frame change $e'=eg$, the [connection one-form](#connection-one-form) changes by $\Gamma'=g^{-1}\Gamma g+g^{-1}dg$, and this horizontal equation changes to the corresponding one in the new frame. Thus the subspaces glue to a unique smooth linear [connection on a vector bundle](#connection-vector-bundle). Its vertical projection gives back the original derivative. The [Leibniz rule](calculus.md#leibniz-rule) ensures locality, allowing this construction from an operator initially defined on global sections.

#### Pullback connection

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pullback_connection)

If a connection on $E\to B$ has connection matrix $A=A_i(y)dy^i$ in a local frame and $f:M\to B$, its pullback connection has matrix

$$
f^*A=A_i(f(x))\frac{\partial f^i}{\partial x^a}dx^a.
$$

It is characterized by $\nabla^{f^*A}_X(f^*s)=f^*(\nabla^A_{df(X)}s)$.

##### Curvature of a pullback connection

↑ **Parent:** [Pullback connection](#pullback-connection)

For a [smooth map](differential-geometry.md#smooth-map-between-manifolds) $\phi:M'\to M$ and a [connection on a vector bundle](#connection-vector-bundle) $E\to M$, the [curvature form of a connection](#curvature-form) on the [pullback vector bundle](#pullback-vector-bundle) satisfies

$$
R^{\phi^*\nabla}_p(u,v)=R^\nabla_{\phi(p)}(d\phi_pu,d\phi_pv)
$$

as an endomorphism of $E_{\phi(p)}$. In a [frame of a vector bundle](#frame-of-a-vector-bundle) written as a row, with section components written as columns, the [connection one-form](#connection-one-form) is $\Omega$ and its [curvature form of a connection](#curvature-form) is $d\Omega+\Omega\wedge\Omega$. The [pullback connection](#pullback-connection) has matrix $\phi^*\Omega$; commutation of the [pullback of a differential form](differential-form.md#pullback-of-a-differential-form) with the [exterior derivative](differential-form.md#exterior-derivative) and [wedge product of differential forms](differential-form.md#wedge-product-of-differential-forms) proves the identity. No pushforward to an ambient [vector field](calculus.md#vector-field) is required: $d\phi(X)$ is a [vector field along a map](#vector-field-along-a-map).

##### Restriction of a connection to an embedded submanifold

↑ **Parent:** [Pullback connection](#pullback-connection)

For an [embedded submanifold](differential-geometry.md#embedded-submanifold) $i:M\hookrightarrow N$, the ambient [affine connection](#affine-connection) induces a [pullback connection](#pullback-connection) on $i^*TN=TN|_M$. Extend a local section off $M$ and differentiate in a direction tangent to $M$. If two extensions agree on $M$, their difference has zero coefficients on $M$, whose tangential derivatives are zero. Thus the restricted derivative is independent of the extension. Its value may have a normal component, so obtaining a connection on $TM$ requires a further projection.

#### Dual connection

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

The [dual connection](#dual-connection) is induced by a [connection on a vector bundle](#connection-vector-bundle) through the evaluation pairing. A connection on $E$ induces one on $E^*$ by

$$
(\nabla_X\alpha)(s)=X(\alpha(s))-\alpha(\nabla_Xs).
$$

Its connection matrices are the negatives of the transposes of those for $E$.

#### Tensor product connection

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

Connections on $E$ and $F$ induce the connection on $E\otimes F$ determined by

$$
\nabla(s\otimes t)=(\nabla^Es)\otimes t+s\otimes(\nabla^Ft).
$$

In tensor-product local frames its connection matrix is $A_E\otimes I+I\otimes A_F$.

##### Curvature of a tensor product connection

↑ **Parent:** [Tensor product connection](#tensor-product-connection)

The curvature of a [tensor product connection](#tensor-product-connection) is

$$
F_{E\otimes F}=F_E\otimes I+I\otimes F_F.
$$

For [line bundles](ringed-space.md#line-bundle), this is simply $F_{E\otimes F}=F_E+F_F$.

#### Endomorphism bundle connection

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

A connection with local matrix $A$ induces on an endomorphism-valued $r$-form $\mu$ the covariant exterior derivative

$$
d^{\operatorname{End}(A)}\mu
=d\mu+A\wedge\mu-(-1)^r\mu\wedge A.
$$

##### Commutator identity for an endomorphism connection

↑ **Parent:** [Endomorphism bundle connection](#endomorphism-bundle-connection)

The [endomorphism bundle connection](#endomorphism-bundle-connection) is $\widetilde D_X\alpha=D_X\circ\alpha-\alpha\circ D_X$ on sections. Expanding twice makes the two middle terms cancel, proving the displayed [commutator](lie-algebra.md#commutator) identity. Subtracting the derivative along the [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields) gives $\widetilde R(X,Y)\alpha=[R(X,Y),\alpha]$. The operators $D_X$ are differential operators, rather than fibrewise endomorphisms; the corrected curvature operator is fibrewise linear.

##### Curvature of an endomorphism bundle connection

↑ **Parent:** [Endomorphism bundle connection](#endomorphism-bundle-connection)

For the [endomorphism bundle connection](#endomorphism-bundle-connection), $(\widetilde\nabla_X\phi)(s)=\nabla_X(\phi s)-\phi(\nabla_Xs)$. Expanding two derivatives and subtracting $\widetilde\nabla_{[X,Y]}$ gives

$$
F_{\operatorname{End}(A)}(X,Y)\phi
=F_A(X,Y)\circ\phi-\phi\circ F_A(X,Y).
$$

Thus its [curvature form of a connection](#curvature-form) is the commutator action of the original curvature.

###### Scalar-curvature criterion for a flat endomorphism connection

↑ **Parent:** [Curvature of an endomorphism bundle connection](#curvature-of-an-endomorphism-bundle-connection)

The [endomorphism bundle connection](#endomorphism-bundle-connection) of a rank-$r>0$ bundle is flat if and only if the original curvature satisfies $F_A=\omega\,\operatorname{id}$. By the [curvature of an endomorphism bundle connection](#curvature-of-an-endomorphism-bundle-connection), flatness means each $F_A(X,Y)$ commutes with every fiber endomorphism. The centre of the full matrix algebra consists of scalar matrices, and $\omega=r^{-1}\operatorname{tr}F_A$ is the required smooth two-form. The original connection can still have nonzero scalar curvature.

#### Solder form

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Solder_form)

The solder form on a smooth manifold is the identity $TX$-valued one-form $\theta(V)=V$. In a coordinate frame it is $\theta=dx^i\otimes\partial_i$.

##### Torsion form

↑ **Parent:** [Solder form](#solder-form)

The torsion form of a connection on $TX$ is the covariant exterior derivative of the [solder form](#solder-form). It satisfies

$$
T(U,V)=\nabla_UV-\nabla_VU-[U,V].
$$

###### Cartan first structure equation with input-first indices

↑ **Parent:** [Torsion form](#torsion-form)

If $\nabla_Xe_i=\sum_j\omega_{ij}(X)e_j$ and $\phi_i$ is the dual [coframe](#coframe), the first index of $\omega$ is the input frame vector. Expand the connection derivative of $Y=\sum_i\phi_i(Y)e_i$ and antisymmetrize in $X,Y$. The formula for the [exterior derivative of a one-form evaluated on vector fields](differential-form.md#exterior-derivative-of-a-one-form-evaluated-on-vector-fields) gives $\tau_j=d\phi_j-\sum_i\phi_i\wedge\omega_{ij}$. This is the first structure equation with the indicated index convention. Reversing the wedge order changes the sign.

###### Torsion-free connection

↑ **Parent:** [Torsion form](#torsion-form)

A connection on the tangent bundle is torsion-free when $\nabla_XY-\nabla_YX=[X,Y]$. Its Christoffel symbols are symmetric in their two lower indices.

#### Metric connection

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Metric_connection)

A connection on a Riemannian vector bundle is metric-compatible when

$$
d\langle s,t\rangle
=\langle\nabla s,t\rangle+\langle s,\nabla t\rangle.
$$

Equivalently, its parallel transport maps are isometries.

##### Metric compatibility

↑ **Parent:** [Metric connection](#metric-connection)

A [metric connection](#metric-connection) satisfies [metric compatibility](#metric-compatibility), $\nabla_\alpha g_{\mu\nu}=0$. This allows the [metric tensor](general-relativity.md#metric-tensor) to commute with [covariant derivatives](general-relativity.md#covariant-derivative) and index raising or lowering.

###### Lie derivative of a metric with nonmetricity

↑ **Parent:** [Metric compatibility](#metric-compatibility)

For any [torsion-free connection](#torsion-free-connection), expand the coordinate [Lie derivative of a tensor field](#lie-derivative-of-a-tensor-field) and cancel the symmetric connection terms to obtain the displayed identity. If the connection is [metric-compatible](#metric-connection), lowering the vector index commutes with the [covariant derivative](general-relativity.md#covariant-derivative) and it becomes $\mathcal L_\xi g_{ab}=2\nabla_{(a}\xi_{b)}$. Symmetry of the connection alone does not suffice: with $g=e^{2x}dx^2$, zero connection coefficients and $\xi=\partial_x$, the two expressions $\mathcal L_\xi g$ and $2\nabla_x\xi_x$ are $2e^{2x}$ and $4e^{2x}$, respectively.

##### Normal connection

↑ **Parent:** [Metric connection](#metric-connection)

The ambient [Levi-Civita connection](general-relativity.md#levi-civita-connection) induces this [metric connection](#metric-connection) on the [normal bundle](algebraic-geometry.md#normal-bundle) of an [embedded submanifold](differential-geometry.md#embedded-submanifold). Its tangential counterpart appears in the [Weingarten formula](second-fundamental-form.md#weingarten-formula). Projecting the derivative preserves the [connection on a vector bundle](#connection-vector-bundle) Leibniz rule and the fiber [inner product](linear-algebra.md#inner-product).

##### Skew-adjoint difference criterion for metric connections

↑ **Parent:** [Metric connection](#metric-connection)

Let $\nabla$ be a [metric connection](#metric-connection) for a [Riemannian metric](differential-geometry.md#riemannian-metric) $g$, and let $\nabla'$ be another [affine connection](#affine-connection) on the same [tangent bundle](#tangent-bundle). The [difference of affine connections is a tensor](#difference-of-affine-connections-is-a-tensor) $A=\nabla-\nabla'$. Expanding the derivative of the [metric tensor](general-relativity.md#metric-tensor) gives

$$
(\nabla'_Xg)(Y,Z)=g(A(X,Y),Z)+g(Y,A(X,Z)).
$$

Thus $\nabla'$ is a [metric connection](#metric-connection) precisely when each endomorphism $A(X,\cdot)$ is skew-adjoint. This imposes no antisymmetry in $X,Y$; that separate condition characterizes agreement of parametrized [geodesics](riemannian-geometry.md#geodesic). If both conditions hold, $g(A(X,Y),Z)$ is alternating in all three arguments.

##### Smooth unitary frame for a Hermitian connection

↑ **Parent:** [Metric connection](#metric-connection)

A smooth positive Hermitian bundle metric admits local orthonormal frames by the smooth [Gram-Schmidt process](linear-algebra.md#gram-schmidt-process). In such a frame, metric compatibility gives $A_{ji}(V)+\overline{A_{ij}(V)}=0$ for real [vector fields](calculus.md#vector-field) $V$, so the connection matrix is skew-Hermitian. The orthonormal frame is smooth; a holomorphic orthonormal frame is not generally available.

##### Parallel transport preserves a fibre metric

↑ **Parent:** [Metric connection](#metric-connection)

For a [metric connection](#metric-connection) on a [vector bundle](#vector-bundle), the [covariant derivative along a curve](#covariant-derivative-along-a-curve) satisfies $(d/dt)\langle u,v\rangle=\langle D_tu,v\rangle+\langle u,D_tv\rangle$. If both sections are parallel, the right side vanishes. Thus [parallel transport](#parallel-transport) preserves the fibre [inner product](linear-algebra.md#inner-product), not merely vector lengths, and is a linear isometry between the endpoint fibres.

##### Connection matrix in an orthonormal frame is skew-symmetric

↑ **Parent:** [Metric connection](#metric-connection)

In a local [orthonormal frame](general-relativity.md#orthonormal-frame-in-spacetime) $(e_i)$, write $\nabla e_j=A^i{}_j e_i$. [Metric compatibility](#metric-compatibility) and $d\langle e_i,e_j\rangle=0$ give

$$
A^i{}_j+A^j{}_i=0.
$$

Thus the connection one-form of a real metric connection takes values in the [skew-symmetric matrices](linear-algebra.md#skew-symmetric-matrix).

##### Koszul formula

↑ **Parent:** [Metric connection](#metric-connection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Koszul_formula)

The unique torsion-free metric connection satisfies

$$
2g(\nabla_XY,Z)
=Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)
-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
$$

This formula both proves uniqueness of the [Levi-Civita connection](general-relativity.md#levi-civita-connection) and computes it from the metric and [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields).

###### Existence and uniqueness of the Levi-Civita connection

↑ **Parent:** [Koszul formula](#koszul-formula)

The [Koszul formula](#koszul-formula) uniquely determines $g(\nabla_XY,Z)$ for all [vector fields](calculus.md#vector-field) $X,Y,Z$, so nondegeneracy of the [Riemannian metric](differential-geometry.md#riemannian-metric) determines $\nabla_XY$. The resulting operation is $C^\infty$-linear in $X$, obeys the [Leibniz rule](calculus.md#leibniz-rule) in $Y$, is compatible with the metric, and is [torsion-free](#torsion-free-connection). It is therefore the unique [Levi-Civita connection](general-relativity.md#levi-civita-connection).

##### Unitary connection

↑ **Parent:** [Metric connection](#metric-connection)

A connection on a complex vector bundle with [Hermitian metric](complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle) $h$ is unitary when

$$
d\,h(s,t)=h(\nabla s,t)+h(s,\nabla t).
$$

In a unitary local frame its connection matrix is skew-Hermitian, and so is its curvature matrix.

###### Uhlenbeck small-energy Coulomb gauge

↑ **Parent:** [Unitary connection](#unitary-connection)

For a connection with compact structure group on a four-dimensional ball, sufficiently small $L^2$ curvature permits a gauge with $d^*a=0$, suitable boundary condition and $\|a\|_{W^{1,2}}\leq C\|F\|_2$ after rescaling. For anti-self-dual connections, local elliptic regularity also gives scale-invariant curvature derivative estimates on smaller balls. These are local analytic inputs, not the global bubbling compactness conclusion.

// Destination: geometry-and-topology.bigb

###### Harmonic-curvature unitary line connection

↑ **Parent:** [Unitary connection](#unitary-connection)

The real curvature $iF_A$ of a unitary line connection has a fixed de Rham class. Let $\eta$ be its harmonic representative and write $\eta-iF_A=d\beta$. Then $A-i\beta$ has curvature $\eta$. Any two such connections differ by a closed imaginary one-form. If $b_1=0$, that form is exact and comes from a circle-valued gauge transformation. In general their gauge classes form a torsor for $H^1(X;\mathbb R)/(2\pi H^1(X;\mathbb Z))$.

// Destination: geometry-and-topology.bigb

###### Unitary bundle gauge transformation

↑ **Parent:** [Unitary connection](#unitary-connection)

A determinant-preserving unitary bundle automorphism covering the identity on the base. For an $SU(2)$ bundle its values are in the fiberwise special unitary group. We use $A^u=u^{-1}Au+u^{-1}du$. Its curvature transforms by $F_{A^u}=u^{-1}F_Au$. The automorphism is a change of unitary frame, not a change of the base point.

// Destination: geometry-and-topology.bigb

###### Unitary bundle gauge group

↑ **Parent:** [Unitary bundle gauge transformation](#unitary-bundle-gauge-transformation)

The group of [unitary bundle gauge transformations](#unitary-bundle-gauge-transformation) under composition. It acts on connections and their solution spaces. The stabilizer of a connection is the centralizer of its [holonomy](#holonomy) acting by parallel automorphisms, so a quotient can have singularities when this stabilizer increases.

// Destination: geometry-and-topology.bigb

###### Coulomb slice for unitary connections

↑ **Parent:** [Unitary bundle gauge group](#unitary-bundle-gauge-group)

Near a fixed connection $A$, impose $d_A^*a=0$ on perturbations. The linearized gauge-fixing equation is $d_A^*d_A\xi$, invertible on the orthogonal complement of its parallel kernel. In Sobolev completions above the multiplication threshold, the implicit function theorem gives a local slice; its remaining identifications are by the compact stabilizer of $A$. This reduces the gauge quotient to a finite-dimensional Kuranishi model when the curvature equation is elliptic.

// Destination: geometry-and-topology.bigb

###### Based unitary gauge group

↑ **Parent:** [Unitary bundle gauge group](#unitary-bundle-gauge-group)

The subgroup of [unitary bundle gauge transformations](#unitary-bundle-gauge-transformation) equal to the identity at a chosen framed base point. Quotienting flat connections by this subgroup retains the full [flat holonomy representation](relativistic-quantum-field.md#holonomy-representation-of-a-flat-connection); quotienting by the whole group also divides by simultaneous conjugation.

// Destination: geometry-and-topology.bigb

###### Anti-self-dual connection

↑ **Parent:** [Unitary connection](#unitary-connection)

A [unitary connection](#unitary-connection) $A$ on an oriented Riemannian four-manifold is anti-self-dual when $F_A^+=(F_A+*F_A)/2=0$. Its curvature is covariantly closed by the [Bianchi identity](#bianchi-identity) and solves the [Yang-Mills equations](relativistic-quantum-field.md#yang-mills-equations). With anti-Hermitian matrices and the fundamental trace, $k=c_2(E)[X]=(8\pi^2)^{-1}\int_X\operatorname{Tr}(F_A\wedge F_A)=\|F_A\|_2^2/(8\pi^2)$ for an $SU(2)$ bundle. Thus its charge is nonnegative.

// Destination: geometry-and-topology.bigb

###### Abelian anti-self-dual connections from harmonic scalar potentials

↑ **Parent:** [Anti-self-dual connection](#anti-self-dual-connection)

Locally a [U(1) connection](#u-1-connection) whose [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) has no $(2,0)$ or $(0,2)$ part can be written $A=\partial u+\bar\partial v$ by the [Dolbeault-Poincaré lemma](complex-geometry.md#dolbeault-poincare-lemma). Unitarity permits $v=-\bar u$. Writing $u=p+iq$, a [gauge transformation](electromagnetism.md#gauge-transformation) removes $i\,dq$ and leaves $A=\partial p-\bar\partial p$. Setting $f=-2p$ gives the displayed [unitary](#unitary-connection) form, whose [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) is $\partial\bar\partial f$. Its remaining [anti-self-duality of gauge curvature](classical-field-theory-soliton.md#anti-self-duality-of-gauge-curvature) condition is the scalar [Laplace equation](partial-differential-equation.md#laplace-equation). Alternatively a complex [gauge transformation](electromagnetism.md#gauge-transformation) by $e^{-u}$ gives $A=\bar\partial(v-u)$; this second gauge generally does not preserve unitarity.

// Destination: complex-geometry.bigb

###### ASD deformation complex

↑ **Parent:** [Anti-self-dual connection](#anti-self-dual-connection)

The infinitesimal gauge and curvature complex is $0\to\Omega^0(\operatorname{ad}E)\xrightarrow{d_A}\Omega^1(\operatorname{ad}E)\xrightarrow{d_A^+}\Omega^{2,+}(\operatorname{ad}E)\to0$. Its composite on $\xi$ is $[F_A^+,\xi]=0$. Its cohomology describes infinitesimal stabilizers, deformations and obstructions. The gauge-fixed operator is $D_A=d_A^*\oplus d_A^+$.

// Destination: geometry-and-topology.bigb

###### Local cone at an unobstructed reducible SU2 instanton

↑ **Parent:** [ASD deformation complex](#asd-deformation-complex)

On a simply connected negative-definite four-manifold, an ASD connection of full circle holonomy has $h_A^0=1$. If $h_A^2=0$, the index formula gives $h_A^1=8k-2$. The neutral diagonal deformation space vanishes because $b_1=0$, leaving a complex vector space of dimension $4k-1$ with stabilizer action $z\mapsto\lambda^2z$. Kuranishi reduction and the Coulomb slice give the local quotient $\mathbb C^{4k-1}/S^1$, equivalently the cone on $\mathbb{CP}^{4k-2}$.

// Destination: geometry-and-topology.bigb

###### ASD deformation index

↑ **Parent:** [ASD deformation complex](#asd-deformation-complex)

For an $SU(2)$ bundle of charge $k$ on a closed oriented four-manifold, $\operatorname{ind}D_A=h_A^1-h_A^0-h_A^2=8k-3(1-b_1+b^+)$. Equivalently it is $-2p_1(\operatorname{ad}E)[X]-3(\chi+\sigma)/2$, using $p_1(\operatorname{ad}E)=-4c_2(E)$. The Euler characteristic of the deformation complex has the opposite sign.

// Destination: analysis.bigb

###### Uhlenbeck-Donaldson compactness for charge-one ASD connections

↑ **Parent:** [Anti-self-dual connection](#anti-self-dual-connection)

On a closed oriented Riemannian four-manifold, a sequence of $SU(2)$ [anti-self-dual connections](#anti-self-dual-connection) of second Chern number one has, modulo gauge and subsequence, either smooth convergence with charge one or smooth convergence away from one point to a flat charge-zero connection. In the second case the curvature-energy measures converge to $8\pi^2\delta_x$. Small-energy gauges give convergence away from finitely many points; removable singularities extend the limit; Chern-Simons clutching integers quantize each positive defect. Total charge one leaves only the two stated cases. A flat limit need not have trivial holonomy on a nonsimply connected base.

// Destination: geometry-and-topology.bigb

###### Uhlenbeck removable singularity theorem for ASD connections

↑ **Parent:** [Anti-self-dual connection](#anti-self-dual-connection)

A smooth [anti-self-dual connection](#anti-self-dual-connection) with compact structure group on a punctured four-ball and finite $L^2$ curvature extends smoothly over the puncture after changing gauge and extending the bundle. The gauge on the punctured ball can carry nontrivial clutching degree; the extended bundle need not agree globally with the original one in a bubbling sequence.

// Destination: geometry-and-topology.bigb

###### Positive-square obstruction to ASD line connections

↑ **Parent:** [Anti-self-dual connection](#anti-self-dual-connection)

An [anti-self-dual connection](#anti-self-dual-connection) on a line bundle has $c_1(L)^2[X]=-\|iF_A/(2\pi)\|_2^2\leq0$. A line bundle with positive square therefore admits no such connection for any metric of the chosen orientation. The splitting $L\oplus L^{-1}$ has $c_2=-c_1(L)^2$, giving the equivalent nonnegative-instanton-charge obstruction.

// Destination: geometry-and-topology.bigb

#### Horizontal lift

↑ **Parent:** [Connection (vector bundle)](#connection-vector-bundle)

A [horizontal lift](#horizontal-lift) is determined by the horizontal distribution of a [principal connection](#connection-principal-bundle) or the corresponding [connection on a vector bundle](#connection-vector-bundle). A horizontal lift of a base curve is a curve in the bundle projecting to it and tangent to the horizontal distribution. In a local frame its fiber coordinate solves a linear ordinary differential equation.

##### Parallel transport

↑ **Parent:** [Horizontal lift](#horizontal-lift)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parallel_transport)

Parallel transport along a path $\gamma$ sends an initial fiber vector to the endpoint of the unique horizontal lift through that vector. Reversing the path gives the inverse linear map.

###### Parallel vector field along a curve

↑ **Parent:** [Parallel transport](#parallel-transport)

A [vector field](calculus.md#vector-field) along a smooth curve is parallel if its [covariant derivative](general-relativity.md#covariant-derivative) along that curve is zero. Its value is the [parallel transport](#parallel-transport) of its initial value. A [Levi-Civita connection](general-relativity.md#levi-civita-connection) preserves inner products under this transport, so the length of a parallel field is constant. Along a unit-speed curvature-one [geodesic](riemannian-geometry.md#geodesic), the normal [Jacobi field](general-relativity.md#jacobi-field) with zero initial value and initial derivative $a$ is $\sin t$ times the parallel transport of $a$.

###### Parallel transport around a spherical triangle

↑ **Parent:** [Parallel transport](#parallel-transport)

For the positively oriented boundary of a [spherical triangle](geometry-and-topology.md#spherical-triangle) on the unit sphere, [parallel transport](#parallel-transport) is rotation by its angle excess modulo $2\pi$. The tangent is parallel along each geodesic side and turns by $\pi-\alpha$ at a corner of angle $\alpha$. The three corner turns sum to $3\pi-\alpha-\beta-\gamma$, and combining them with parallel transport returns the initial tangent. Hence the transport angle is the negative of that sum modulo $2\pi$, giving the formula. The [spherical excess formula](differential-geometry.md#spherical-excess-formula) identifies the angle with enclosed area; reversing traversal changes its sign.

###### Global continuation of linear parallel transport

↑ **Parent:** [Parallel transport](#parallel-transport)

Along a smooth curve $\gamma:I\to M$, a [horizontal lift](#horizontal-lift) of a linear [connection on a vector bundle](#connection-vector-bundle) has fibre equation $v'=-\Gamma(\dot\gamma)v$. On each compact time interval the coefficient matrix is bounded, and the [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) prevents finite-time blowup. A finite cover by [vector bundle trivializations](#vector-bundle-trivialization) and ODE uniqueness patch local solutions. Exhausting the open interval gives a unique lift on all of $I$. Its endpoint map is linear, and reversal of the path gives its inverse; no completeness of the base manifold is needed.

###### Parallel frame along a curve

↑ **Parent:** [Parallel transport](#parallel-transport)

A parallel frame along a curve consists of a basis of [vector fields](calculus.md#vector-field) $E_a$ satisfying $D_tE_a=0$ for its [covariant derivative along a curve](#covariant-derivative-along-a-curve). Transporting a basis at the initial point constructs the frame. If the connection preserves the metric, an initially orthonormal basis stays orthonormal. In this frame the [Jacobi equation](calculus-of-variations.md#jacobi-equation) becomes a linear matrix [ordinary differential equation](differential-equation.md#ordinary-differential-equation).

###### Parallel transport on an endomorphism bundle

↑ **Parent:** [Parallel transport](#parallel-transport)

If $P=\mathcal P_\gamma^\nabla$, the induced transport on the endomorphism bundle is conjugation:

$$
\mathcal P_\gamma^{\operatorname{End}(\nabla)}(\mu)=P\mu P^{-1}.
$$

###### Parallel transport around a latitude of the unit sphere

↑ **Parent:** [Parallel transport](#parallel-transport)

For $ds^2=d\theta^2+\sin^2\theta\,d\phi^2$, a vector initially having coordinate components $(V^\theta,V^\phi)=(1,0)$ returns after one constant-$\theta$ circuit with

$$
(V^\theta,V^\phi)
=\left(
\cos(2\pi\cos\theta),
-\frac{\sin(2\pi\cos\theta)}{\sin\theta}
\right).
$$

### Orientation of a vector bundle

↑ **Parent:** [Vector bundle](#vector-bundle)

This is a fiberwise [orientation](algebraic-topology.md#orientation-of-a-simplex) compatible with local trivializations of a [vector bundle](#vector-bundle). An $R$-orientation of a rank-$d$ vector bundle is a coherent choice of generator of $H^d(E_b,E_b\setminus\{0\};R)$ for every fiber, equivalently a [Thom class](#thom-class) with the corresponding fiberwise restriction.

#### Orientability of a vector bundle total space

↑ **Parent:** [Orientation of a vector bundle](#orientation-of-a-vector-bundle)

The total space of a real [vector bundle](#vector-bundle) $E\to M$ has the exact sequence $0\to\pi^*E\to TE\to\pi^*TM\to0$. Taking [determinant line bundles](#determinant-line-bundle) gives the displayed identity. If $M$ is an [orientable smooth manifold](differential-geometry.md#orientable-smooth-manifold), the total space is orientable exactly when $\det E$ is trivial. Sufficiency follows by pullback; necessity follows by restricting the total-space determinant identity to the [zero section](#zero-section-of-a-vector-bundle). For the [cotangent bundle](symplectic-geometry.md#cotangent-bundle), base and fibre coordinate determinants cancel, giving an orientation even when the base is not orientable.

#### Canonical orientation of a complex vector bundle

↑ **Parent:** [Orientation of a vector bundle](#orientation-of-a-vector-bundle)

An ordered complex basis of a rank-$m$ complex vector space gives the real basis $(v_1,iv_1,\ldots,v_m,iv_m)$. Every complex change-of-basis matrix has positive real determinant $|\det_{\mathbb C}A|^2$, so these bases define a canonical integral orientation and hence an $R$-orientation for every commutative coefficient ring $R$.

#### Thom class

↑ **Parent:** [Orientation of a vector bundle](#orientation-of-a-vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thom_class)

A Thom class of an $R$-oriented rank-$d$ vector bundle is a class $u_E\in H^d(D(E),S(E);R)$ restricting to the chosen generator on every fiber pair $(D^d,S^{d-1})$.

##### Cohomology class of a cooriented submanifold

↑ **Parent:** [Thom class](#thom-class)

An oriented normal bundle of a compact embedded [submanifold](differential-geometry.md#submanifold) has a [Thom class](#thom-class). A [tubular neighborhood](differential-geometry.md#tubular-neighborhood) and excision identify it with a relative class in $H^d(X,X\setminus Y)$. Its image in absolute [cohomology](cohomology.md) is $\varepsilon_Y$. It restricts to zero off Y and, in an oriented closed ambient [manifold](topology.md#topological-manifold), represents the [Poincare dual](cohomology.md#poincare-dual) of Y with the normal-first induced orientation.

##### Thom class in a generalized cohomology theory

↑ **Parent:** [Thom class](#thom-class)

For an $h$-oriented rank-$r$ real [vector bundle](#vector-bundle), its [Thom class](#thom-class) restricts on each fiber to the suspension of the coefficient unit under the oriented identification $h^r(D^r,S^{r-1})\cong h^0(\mathrm{pt})$. [Cup product](cohomology.md#cup-product) with this class gives the Thom isomorphism. The associated [Euler class in a generalized cohomology theory](#euler-class-in-a-generalized-cohomology-theory) is the pullback along the [zero section](#zero-section-of-a-vector-bundle) after forgetting relative supports.

// Target: geometry-and-topology.bigb

##### Cup square of a Thom class

↑ **Parent:** [Thom class](#thom-class)

For an oriented rank-$r$ [vector bundle](#vector-bundle), let $U\in H^r(D(E),S(E);\mathbb Z)$ be its [Thom class](#thom-class). Forgetting relative supports sends $U$ to $\pi^*e(E)$, where $e(E)$ is the [Euler class](#euler-class-of-a-vector-bundle). Compatibility of relative and mixed [cup products](cohomology.md#cup-product) gives

$$
U\cup U=U\cup\pi^*e(E).
$$

For odd $r$, [graded commutativity of the cup product](cohomology.md#graded-commutativity-of-the-cup-product) makes $2U^2=0$. The [Thom isomorphism theorem](#thom-isomorphism-theorem) is injective, so $2e(E)=0$. This explains why an odd-rank [Euler class](#euler-class-of-a-vector-bundle) can have only two-torsion.

##### Thom isomorphism theorem

↑ **Parent:** [Thom class](#thom-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thom_isomorphism_theorem)

For an $R$-oriented rank-$d$ vector bundle, multiplication by the [Thom class](#thom-class) gives isomorphisms

$$
H^q(B;R)\xrightarrow{\ \cong\ }H^{q+d}(D(E),S(E);R),
\qquad a\longmapsto\pi^*a\smile u_E.
$$

###### Gysin sequence of an embedding

↑ **Parent:** [Thom isomorphism theorem](#thom-isomorphism-theorem)

For a closed smooth submanifold $M\subseteq N$ of codimension $c>0$, a [tubular neighborhood](differential-geometry.md#tubular-neighborhood) and the homological [Thom isomorphism theorem](#thom-isomorphism-theorem) identify

$$
H_j(N,N\setminus M;\mathbb F_2)\cong H_{j-c}(M;\mathbb F_2).
$$

Substitution in the [long exact sequence in relative homology](homology.md#long-exact-sequence-in-relative-homology) gives the displayed embedding Gysin sequence. It does not require orientability over $\mathbb F_2$.

###### Cohomological Gysin map of an embedding

↑ **Parent:** [Gysin sequence of an embedding](#gysin-sequence-of-an-embedding)

For a closed [smooth embedding](differential-geometry.md#smooth-embedding) $i:N\hookrightarrow M$ of codimension $r$ whose [normal bundle](algebraic-geometry.md#normal-bundle) is oriented over a coefficient ring $R$, a [tubular neighborhood](differential-geometry.md#tubular-neighborhood), [excision](homology.md#excision-theorem) and the [Thom isomorphism theorem](#thom-isomorphism-theorem) identify

$$
H^{q-r}(N;R)\cong H^q(M,M\setminus N;R).
$$

The relative-to-absolute map defines $i_!:H^j(N;R)\to H^{j+r}(M;R)$. For closed oriented $M,N$, it is characterized by

$$
\langle i_!b\smile c,[M]\rangle=\langle b\smile i^*c,[N]\rangle
$$

with compatible orientations. It obeys $i_!(b\smile i^*c)=i_!b\smile c$. If $j:M\setminus N\hookrightarrow M$ and $\delta:H^q(M\setminus N;R)\to H^{q+1-r}(N;R)$ is the connecting map followed by the inverse Thom isomorphism, then, over $\mathbb F_2$,

$$
\delta(j^*c\smile u)=i^*c\smile\delta u.
$$

These identities follow from naturality of the relative [cup product](cohomology.md#cup-product) and show how the exact sequence determines multiplication in complements. Over $\mathbb F_2$ every real [normal bundle](algebraic-geometry.md#normal-bundle) has the required orientation.

##### Euler class of a vector bundle

↑ **Parent:** [Thom class](#thom-class)

The Euler class of an oriented rank-$d$ vector bundle is the pullback $e(E)=s^*u_E\in H^d(B;R)$ of its [Thom class](#thom-class) along the zero section. Over $\mathbb F_2$ it equals the top Stiefel-Whitney class.

###### Euler class in a generalized cohomology theory

↑ **Parent:** [Euler class of a vector bundle](#euler-class-of-a-vector-bundle)

For an $h$-oriented real bundle $\xi$ of rank $r$, pull its [Thom class](#thom-class) back along the [zero section](#zero-section-of-a-vector-bundle) to obtain its Euler class in $h^r(X)$. It depends on the orientation and the actual bundle, not merely its stable isomorphism class. In [complex cobordism](geometry-and-topology.md#complex-cobordism) the orientation may be supplied by a [stable complex structure on a real vector bundle](#stable-complex-structure-on-a-real-vector-bundle).

###### A nowhere-zero section annihilates generalized Euler classes

↑ **Parent:** [Euler class in a generalized cohomology theory](#euler-class-in-a-generalized-cohomology-theory)

Normalize the section to the [sphere bundle](#sphere-bundle). Scaling it from zero to unit length gives a [homotopy](algebraic-topology.md#homotopy) within the [disk bundle](#disk-bundle) from the [zero section](#zero-section-of-a-vector-bundle) to this sphere-valued section. The image of the relative [Thom class](#thom-class) in absolute cohomology restricts to zero on the [sphere bundle](#sphere-bundle). [Homotopy](algebraic-topology.md#homotopy) invariance therefore makes its zero-section pullback vanish.

// Target: geometry-and-topology.bigb

###### Euler class of a complex vector bundle

↑ **Parent:** [Euler class of a vector bundle](#euler-class-of-a-vector-bundle)

A complex rank-$r$ [vector bundle](#vector-bundle) has a canonical real orientation, and its [Euler class](#euler-class-of-a-vector-bundle) equals its top [Chern class](algebraic-geometry.md#chern-class). For a complex line this is $e(L_{\mathbb R})=c_1(L)$. The [splitting principle for complex vector bundles](algebraic-topology.md#splitting-principle-for-complex-vector-bundles) gives an injective cohomology pullback on which the bundle splits into lines. The [Whitney product formula for Euler classes](#whitney-product-formula-for-euler-classes) and [Whitney sum formula for Chern classes](algebraic-geometry.md#whitney-sum-formula-for-chern-classes) then identify both sides with the product of those first Chern classes, proving the general equality.

###### Euler class of an oriented odd-rank vector bundle is two-torsion

↑ **Parent:** [Euler class of a vector bundle](#euler-class-of-a-vector-bundle)

For an oriented vector bundle $E$ of odd rank, multiplication by $-1$ on each fiber identifies $E$ with the oppositely oriented bundle. Naturality and reversal of the [Thom class](#thom-class) give

$$
e(E)=e(E^{\mathrm{op}})=-e(E),
$$

so $2e(E)=0$.

###### Whitney product formula for Euler classes

↑ **Parent:** [Euler class of a vector bundle](#euler-class-of-a-vector-bundle)

For oriented real vector bundles $E$ and $F$, the ordered direct-sum orientation satisfies

$$
e(E\oplus F)=e(E)\smile e(F).
$$

The formula follows because the [Thom class](#thom-class) of the direct sum is the fiberwise exterior product of the two Thom classes.

###### Euler number of a vector bundle

↑ **Parent:** [Euler class of a vector bundle](#euler-class-of-a-vector-bundle)

When an oriented rank-$d$ vector bundle $E$ has a closed oriented $d$-dimensional base $B$, its Euler number is the integer obtained by evaluating the [Euler class of a vector bundle](#euler-class-of-a-vector-bundle) on the [fundamental class](cohomology.md#fundamental-class) of $B$. A nonzero Euler number obstructs a nowhere-zero section and therefore obstructs a framing.

<h6 id="poincare-hopf-theorem">Poincaré-Hopf theorem</h6>

↑ **Parent:** [Euler class of a vector bundle](#euler-class-of-a-vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincaré-Hopf_theorem)

For a compact oriented [smooth manifold](differential-geometry.md#smooth-manifold) $M$, the Euler class of its [tangent bundle](#tangent-bundle) satisfies

$$
\langle e(TM),[M]\rangle=\chi(M).
$$

Equivalently, the sum of the indices of the isolated zeros of a vector field equals the [Euler characteristic](homology.md#euler-characteristic).

###### Euler class of a complex line bundle

↑ **Parent:** [Euler class of a vector bundle](#euler-class-of-a-vector-bundle)

The complex orientation turns a complex line bundle $L$ into an oriented real rank-two bundle, and

$$
e(L_\mathbb R)=c_1(L).
$$

Moreover $e(L^*)=-e(L)$ and $e(L_1\otimes_\mathbb C L_2)=e(L_1)+e(L_2)$.

###### Gysin sequence of a sphere bundle

↑ **Parent:** [Euler class of a vector bundle](#euler-class-of-a-vector-bundle)

A [Gysin sequence of a sphere bundle](#gysin-sequence-of-a-sphere-bundle) is the [long exact sequence](homology.md#long-exact-sequence) induced by the [Gysin homomorphism](cohomology.md#gysin-homomorphism) and the [Euler class of a vector bundle](#euler-class-of-a-vector-bundle).

For the unit sphere bundle $S(E)\to B$ of an oriented rank-$d$ vector bundle, the Gysin sequence contains

$$
\cdots\to H^{q-d}(B)\xrightarrow{\smile e(E)}H^q(B)\to H^q(S(E))\to H^{q-d+1}(B)\xrightarrow{\smile e(E)}H^{q+1}(B)\to\cdots.
$$

###### Gysin ring splitting for an odd-dimensional sphere bundle

↑ **Parent:** [Gysin sequence of a sphere bundle](#gysin-sequence-of-a-sphere-bundle)

Let $E$ be an oriented real [vector bundle](#vector-bundle) of positive even rank $r$, with zero [Euler class](#euler-class-of-a-vector-bundle), and suppose the integral [cohomology](cohomology.md) of $B$ is torsion-free. The [Gysin sequence](#gysin-sequence-of-a-sphere-bundle) gives $0\to H^j(B)\to H^j(S(E))\to H^{j-r+1}(B)\to0$. Choose an odd-degree class $a\in H^{r-1}(S(E))$ with $\pi_!a=1$. The [projection formula for sphere bundle integration](#projection-formula-for-sphere-bundle-integration) identifies the cohomology additively with $\pi^*H^*(B)\oplus\pi^*H^*(B)a$. It is torsion-free, so [graded commutativity of the cup product](cohomology.md#graded-commutativity-of-the-cup-product) gives $a^2=0$ from $2a^2=0$. These facts establish the displayed ring isomorphism, not just a decomposition of groups.

###### Projection formula for sphere bundle integration

↑ **Parent:** [Gysin sequence of a sphere bundle](#gysin-sequence-of-a-sphere-bundle)

For the [sphere bundle](#sphere-bundle) of an oriented rank-$r$ real [vector bundle](#vector-bundle), the integration map in the [Gysin sequence](#gysin-sequence-of-a-sphere-bundle) lowers degree by $r-1$. Its compatibility with the [cup product](cohomology.md#cup-product) is the displayed projection formula. The construction is the connecting map of the disk/sphere pair followed by the inverse [Thom isomorphism theorem](#thom-isomorphism-theorem); the connecting map has its graded module sign, and the degree sign in the conventional fibre-integration map gives the displayed left-module formula.

###### Unoriented Gysin sequence

↑ **Parent:** [Gysin sequence of a sphere bundle](#gysin-sequence-of-a-sphere-bundle)

For a real rank-$r$ [vector bundle](#vector-bundle) $E\to B$, the [Thom isomorphism theorem](#thom-isomorphism-theorem) with $\mathbb F_2$ coefficients identifies the [relative cohomology](cohomology.md#relative-cohomology) sequence of its [disk bundle](#disk-bundle) and [sphere bundle](#sphere-bundle) with

$$
\cdots\to H^{j-r}(B;\mathbb F_2)\xrightarrow{\cup w_r(E)}H^j(B;\mathbb F_2)\to H^j(S(E);\mathbb F_2)\to H^{j-r+1}(B;\mathbb F_2)\to\cdots.
$$

The multiplier is the top [Stiefel–Whitney class](#stiefel-whitney-class), also called the mod-two [Euler class](#euler-class-of-a-vector-bundle). No orientation of $E$ is required. For the [real tautological line bundle](#real-tautological-line-bundle), the [sphere bundle](#sphere-bundle) is the antipodal cover of [Real projective space](algebraic-topology.md#real-projective-space); this sequence proves that all powers of the degree-one generator through the dimension of the base are nonzero.

###### Three-dimensional lens space as a circle bundle

↑ **Parent:** [Gysin sequence of a sphere bundle](#gysin-sequence-of-a-sphere-bundle)

The diagonal quotient $L(p)=S^3/(\mathbb Z/p)$ is the unit [circle bundle](#circle-bundle) of a complex line bundle over $S^2$ whose [Euler class](#euler-class-of-a-vector-bundle) is $p$ times a generator. Its [Gysin sequence](#gysin-sequence-of-a-sphere-bundle) gives

$$
H^j(L(p);\mathbb Z)\cong
\begin{cases}
\mathbb Z,&j=0,3,\\
\mathbb Z/p,&j=2,\\
0,&\text{otherwise},
\end{cases}
$$

while $H^j(L(p);\mathbb F_p)\cong\mathbb F_p$ for $0\leq j\leq3$.

###### Integral cohomology of a circle bundle over a product of two spheres

↑ **Parent:** [Gysin sequence of a sphere bundle](#gysin-sequence-of-a-sphere-bundle)

Let $a,b$ be the standard basis of $H^2(S^2\times S^2;\mathbb Z)$ and let $E\to S^2\times S^2$ be an oriented circle bundle with Euler class $pa+qb\neq0$. If $d=\gcd(|p|,|q|)$, its [Gysin sequence](#gysin-sequence-of-a-sphere-bundle) gives

$$
H^i(E;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&i=0,3,5,\\
\mathbb Z\oplus\mathbb Z/d,&i=2,\\
\mathbb Z/d,&i=4,\\
0,&\text{otherwise}.
\end{cases}
$$

For zero Euler class the bundle is trivial and its cohomology is that of $(S^2\times S^2)\times S^1$.

### Tautological bundle

↑ **Parent:** [Vector bundle](#vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tautological_bundle)

The tautological bundle over a projective space has as its fiber over a line precisely that line. The real tautological line bundle over $\mathbb{RP}^m$ has first Stiefel-Whitney class equal to the degree-one generator.

#### Complex tautological bundle on a Grassmannian

↑ **Parent:** [Tautological bundle](#tautological-bundle)

Over $\operatorname{Gr}_k(\mathbb C^N)$ this rank-k [complex vector bundle](#complex-vector-bundle) has fibre W at the point W. In a chart of planes that are graphs of maps from a fixed k-plane, $(A,w)\mapsto(\operatorname{graph}A,w+Aw)$ gives a [local trivialization](#local-trivialization). The direct-limit bundle over the infinite [Grassmannian](differential-geometry.md#grassmannian) classifies rank-k bundles over compact Hausdorff spaces.

##### Classification of complex vector bundles by a Grassmannian

↑ **Parent:** [Complex tautological bundle on a Grassmannian](#complex-tautological-bundle-on-a-grassmannian)

A [partition of unity](differential-geometry.md#partition-of-unity) and local orthonormal frames embed a bundle over compact Hausdorff X in a finite trivial bundle. Its fibre images give a classifying map pulling back the [complex tautological bundle on a Grassmannian](#complex-tautological-bundle-on-a-grassmannian). Isomorphic bundles give homotopic maps by interpolating two embeddings in orthogonal coordinate blocks. Homotopic maps give isomorphic bundles because uniformly close orthogonal projections identify their image bundles along a finite subdivision of the homotopy interval.

###### Rank-two complex vector bundles over the four-sphere

↑ **Parent:** [Classification of complex vector bundles by a Grassmannian](#classification-of-complex-vector-bundles-by-a-grassmannian)

The contractible universal frame bundle gives $\pi_4(BU_2)\cong\pi_3(U_2)$ and simple connectedness of $BU_2$. The determinant fibration $SU_2\to U_2\to S^1$ identifies $\pi_3(U_2)$ with $\pi_3(SU_2)$. Since $SU_2\cong S^3$, this is $\mathbb Z$. Hence the [classification of complex vector bundles by a Grassmannian](#classification-of-complex-vector-bundles-by-a-grassmannian) gives the displayed bijection of isomorphism classes; fixed-rank classes do not acquire a group operation from Whitney sum.

###### Close orthogonal projections identify their image bundles

↑ **Parent:** [Classification of complex vector bundles by a Grassmannian](#classification-of-complex-vector-bundles-by-a-grassmannian)

Let P,Q be continuous orthogonal projection matrices of equal rank on a common trivial [complex vector bundle](#complex-vector-bundle), with the displayed bound at every base point. Restricting Q to the image of P is injective: if Qv=0, then $v=(P-Q)v$ contradicts the norm bound unless v=0. Equal dimensions give a continuously invertible [vector bundle isomorphism](#vector-bundle-isomorphism). Compactness applies this observation uniformly to a homotopy of image planes.

###### Finite-dimensional embedding of a complex vector bundle

↑ **Parent:** [Classification of complex vector bundles by a Grassmannian](#classification-of-complex-vector-bundles-by-a-grassmannian)

For finitely many orthonormal [local trivializations](#local-trivialization) $t_i$ and a subordinate [partition of unity](differential-geometry.md#partition-of-unity) $\rho_i$, the displayed map embeds a rank-k [complex vector bundle](#complex-vector-bundle) isometrically in $X\times\mathbb C^{kr}$. Outside the support of each $\rho_i$ its component is zero. Its continuous image planes give a finite-dimensional [Grassmannian](differential-geometry.md#grassmannian) map and identify the original bundle with a tautological pullback.

#### Complex tautological line bundle

↑ **Parent:** [Tautological bundle](#tautological-bundle)

Over complex [projective space](projective-space.md), its fibre at a line $\ell\subseteq\mathbb C^{n+1}$ is $\ell$ itself. It is a [holomorphic line bundle](complex-geometry.md#holomorphic-line-bundle) contained in the trivial bundle. Its dual is the [hyperplane line bundle](#hyperplane-line-bundle).

##### Punctured line bundles do not determine their duality sign

↑ **Parent:** [Complex tautological line bundle](#complex-tautological-line-bundle)

For any complex line bundle $L$, a nonzero dual vector $\phi\in L_b^*$ determines the unique $v\in L_b$ with $\phi(v)=1$. In local coordinates this is fiber inversion $a\mapsto a^{-1}$, giving a smooth projection-preserving diffeomorphism between the complements of the [zero sections](#zero-section-of-a-vector-bundle) of $L^*$ and $L$. It is not a fiber-linear bundle isomorphism. In particular this condition cannot distinguish the tautological line on the [complex projective line](algebraic-topology.md#complex-projective-line) from its dual.

##### Unitary transitions of the tautological line over the projective line

↑ **Parent:** [Complex tautological line bundle](#complex-tautological-line-bundle)

For $\zeta=z_2/z_1$ and $\eta=1/\zeta$, the tautological frames $(1,\zeta)$ and $(\eta,1)$ differ by $1/\zeta$. Normalize their ambient [Hermitian form](linear-algebra.md#hermitian-form) norms; the resulting frames differ by the displayed phase. The unit circle total space is $S^3\subset\mathbb C^2$ and its projection to the [complex projective line](algebraic-topology.md#complex-projective-line) is the [Hopf fibration](algebraic-topology.md#hopf-fibration). The transition of the dual line is the reciprocal phase.

##### Global holomorphic sections of the complex tautological line bundle vanish

↑ **Parent:** [Complex tautological line bundle](#complex-tautological-line-bundle)

The [complex tautological line bundle](#complex-tautological-line-bundle) is a [holomorphic subbundle](complex-geometry.md#holomorphic-subbundle) of the trivial bundle with fibre $\mathbb C^{n+1}$. A global [holomorphic section](complex-geometry.md#holomorphic-section) therefore gives $n+1$ global [holomorphic functions](complex-analysis.md#holomorphic-function) on compact connected [Complex projective space](algebraic-topology.md#complex-projective-space). The maximum modulus principle makes them constant. The constant vector must lie in every projective line through the origin, whose intersection is zero for $n\geq1$. For $n=0$, the base is one point and the section space is instead $\mathbb C$.

##### Hyperplane line bundle

↑ **Parent:** [Complex tautological line bundle](#complex-tautological-line-bundle)

The dual of the [complex tautological line bundle](#complex-tautological-line-bundle). On the [complex projective line](algebraic-topology.md#complex-projective-line) the induced frames satisfy $e_1=w e_0$ on the overlap of its standard affine charts.

###### Hyperplane class

↑ **Parent:** [Hyperplane line bundle](#hyperplane-line-bundle)

The [First Chern class](complex-geometry.md#first-chern-class) of the [hyperplane line bundle](#hyperplane-line-bundle). On [Complex projective space](algebraic-topology.md#complex-projective-space) it generates degree-two [integral cohomology](cohomology.md#integral-cohomology), and on $\mathbb{CP}^n$ its top power evaluates as one on the complex-oriented [fundamental class](cohomology.md#fundamental-class).

###### Nontrivial hyperplane powers on a compact projective submanifold

↑ **Parent:** [Hyperplane line bundle](#hyperplane-line-bundle)

Let $X$ be a nonempty positive-dimensional compact [complex submanifold](complex-geometry.md#complex-submanifold) of [Complex projective space](algebraic-topology.md#complex-projective-space). On a positive-dimensional connected component choose a hyperplane meeting, but not containing, that component. Its linear equation gives a [holomorphic section](complex-geometry.md#holomorphic-section) of $\mathcal O_X(1)$ with a zero and with a nonzero value. For $m>0$, its $m$th power cannot be a section of a trivial [holomorphic line bundle](complex-geometry.md#holomorphic-line-bundle), since such sections are constant on the compact connected component. Negative powers are also nontrivial by duality. Every positive-dimensional compact projective component meets every hyperplane: otherwise its affine coordinate functions would all be constant.

###### Tensor powers of the hyperplane line bundle

↑ **Parent:** [Hyperplane line bundle](#hyperplane-line-bundle)

For positive $k$ take the $k$th tensor power of the [hyperplane line bundle](#hyperplane-line-bundle); for negative $k$ take the corresponding power of its dual; for $k=0$ take the trivial line bundle. On the [complex projective line](algebraic-topology.md#complex-projective-line), global sections for $k\geq0$ correspond to polynomials of degree at most $k$ and form a space of dimension $k+1$.

#### Quaternionic tautological line bundle

↑ **Parent:** [Tautological bundle](#tautological-bundle)

Its fibre over a point of [quaternionic projective space](projective-space.md#quaternionic-projective-space) is the quaternionic line represented by that point. As a real vector bundle it has rank four, and its unit [sphere bundle](#sphere-bundle) is $S^{4n+3}\to\mathbb{HP}^n$. Right multiplication by a chosen imaginary unit equips it with complex rank two. Under the [complex inclusion into quaternionic projective space](projective-space.md#complex-inclusion-into-quaternionic-projective-space), it restricts to $L\oplus\overline L$, where $L$ is the complex [tautological bundle](#tautological-bundle). Thus its [Euler class](#euler-class-of-a-vector-bundle) restricts to $-c_1(L^*)^2$.

#### Real tautological line bundle

↑ **Parent:** [Tautological bundle](#tautological-bundle)

Over [Real projective space](algebraic-topology.md#real-projective-space) $\mathbb{RP}^n$, the real tautological line bundle is

$$
\gamma_n=\{(\ell,v):v\in\ell\}\subseteq\mathbb{RP}^n\times\mathbb R^{n+1}.
$$

On the standard chart $U_i=\{[x]:x_i\ne0\}$, let $s_i([x])=x/x_i$. A [local trivialization](#local-trivialization) sends $([x],t)$ to $([x],t s_i([x]))$, with inverse $([x],v)\mapsto([x],v_i)$. These maps prove that this is a [real line bundle](#real-line-bundle). Its unit [sphere bundle](#sphere-bundle) is the [antipodal map](homology.md#antipodal-map) quotient $S^n\to\mathbb{RP}^n$. Its [mod-two Euler class of a real line bundle](#mod-two-euler-class-of-a-real-line-bundle) is the degree-one generator of the [mod-two cohomology ring of real projective space](algebraic-topology.md#mod-two-cohomology-ring-of-real-projective-space).

<h3 id="stiefel-whitney-class">Stiefel–Whitney class</h3>

↑ **Parent:** [Vector bundle](#vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stiefel–Whitney_class)

The Stiefel–Whitney classes of a real rank-$d$ vector bundle are classes

$$
w_i(E)\in H^i(X;\mathbb F_2),
\qquad 0\leq i\leq d.
$$

Their total class is $w(E)=1+w_1(E)+\cdots+w_d(E)$.

#### Parity of zeros of a real line-bundle section

↑ **Parent:** [Stiefel–Whitney class](#stiefel-whitney-class)

For a real [line bundle](ringed-space.md#line-bundle) on a closed manifold, a transverse section has a hypersurface as its zero set. Along a closed loop transverse to this hypersurface, trivialize the pullback over the cut interval. Each simple zero reverses the sign of the component function. The total sign change is exactly the bundle's transition sign around the loop, detected by its first [Stiefel–Whitney class](#stiefel-whitney-class). Thus zero-set intersection parity with every loop equals the evaluation of $w_1(L)$, proving the displayed mod-two dual class. No orientability of the manifold or bundle is required.

<h4 id="codimension-one-stiefel-whitney-immersion-obstruction">Codimension-one Stiefel–Whitney immersion obstruction</h4>

↑ **Parent:** [Stiefel–Whitney class](#stiefel-whitney-class)

An [immersion](differential-geometry.md#immersion) of a smooth $d$-manifold in $\mathbb R^{d+1}$ supplies a rank-one [normal bundle](algebraic-geometry.md#normal-bundle) $\nu$ with $TM\oplus\nu\cong\varepsilon^{d+1}$. The [Whitney product formula for Stiefel–Whitney classes](#whitney-product-formula-for-stiefel-whitney-classes) therefore requires $w(\nu)=w(TM)^{-1}$. A [real line bundle](#real-line-bundle) has no positive-degree classes beyond $w_1$, so every higher-degree part of the inverse total class must vanish. For $\mathbb{RP}^2\times\mathbb{RP}^2$, the [stabilized tangent bundle of real projective space](#stabilized-tangent-bundle-of-real-projective-space) gives $w(TM)^{-1}=(1+a)(1+b)$ in $\mathbb F_2[a,b]/(a^3,b^3)$. Its nonzero degree-two part $ab$ excludes an [immersion](differential-geometry.md#immersion) in $\mathbb R^5$ even though the normal line need not be orientable.

<h4 id="stiefel-whitney-class-of-the-underlying-real-bundle-of-a-complex-line">Stiefel–Whitney class of the underlying real bundle of a complex line</h4>

↑ **Parent:** [Stiefel–Whitney class](#stiefel-whitney-class)

A [complex line bundle](#complex-line-bundle) has a canonically oriented underlying real [vector bundle](#vector-bundle) of rank two. Its first [Stiefel–Whitney class](#stiefel-whitney-class) vanishes, and its second [Stiefel–Whitney class](#stiefel-whitney-class) is the mod-two reduction of its [First Chern class](complex-geometry.md#first-chern-class).

<h4 id="projective-bundle-definition-of-stiefel-whitney-classes">Projective bundle definition of Stiefel–Whitney classes</h4>

↑ **Parent:** [Stiefel–Whitney class](#stiefel-whitney-class)

Let $p:\mathbb P(E)\to X$ and put $u=w_1(L_E)$. The mod-two projective bundle formula makes $H^*(\mathbb P(E);\mathbb F_2)$ free over $H^*(X;\mathbb F_2)$ on $1,u,\ldots,u^{d-1}$. The unique relation

$$
u^d+p^*w_1(E)u^{d-1}+\cdots+p^*w_d(E)=0
$$

defines the Stiefel–Whitney classes.

#### Splitting principle for real vector bundles

↑ **Parent:** [Stiefel–Whitney class](#stiefel-whitney-class)

After pulling a real vector bundle back along a suitable iterated projective or flag bundle, it splits into real line bundles, and the pullback on mod-two cohomology is injective. Identities among Stiefel–Whitney classes can therefore be checked after splitting.

<h5 id="whitney-product-formula-for-stiefel-whitney-classes">Whitney product formula for Stiefel–Whitney classes</h5>

↑ **Parent:** [Splitting principle for real vector bundles](#splitting-principle-for-real-vector-bundles)

For real vector bundles $E$ and $F$,

$$
w(E\oplus F)=w(E)w(F),
\qquad
w_k(E\oplus F)=\sum_{i+j=k}w_i(E)w_j(F).
$$

After applying the [splitting principle for real vector bundles](#splitting-principle-for-real-vector-bundles), both sides are the product of $1+w_1(L)$ over all line summands.

<h6 id="stiefel-whitney-obstruction-to-a-diagonal-projective-immersion">Stiefel–Whitney obstruction to a diagonal projective immersion</h6>

↑ **Parent:** [Whitney product formula for Stiefel–Whitney classes](#whitney-product-formula-for-stiefel-whitney-classes)

For a map $f:\mathbb{RP}^{2k+1}\to\mathbb{CP}^k$ nontrivial on degree-two mod-two [cohomology](cohomology.md), an [immersion](differential-geometry.md#immersion) in the [homotopy](algebraic-topology.md#homotopy) class of $(f,f)$ has a rank-$(2k-1)$ [normal bundle](algebraic-geometry.md#normal-bundle) with total [Stiefel–Whitney class](#stiefel-whitney-class) $(1+x)^{2k+2}$. Its forbidden degree-$2k$ [Stiefel–Whitney class](#stiefel-whitney-class) is $(k+1)x^{2k}$, so $k$ must be odd.

<h4 id="bockstein-of-a-stiefel-whitney-class">Bockstein of a Stiefel–Whitney class</h4>

↑ **Parent:** [Stiefel–Whitney class](#stiefel-whitney-class)

For the Bockstein associated with $0\to\mathbb Z/2\to\mathbb Z/4\to\mathbb Z/2\to0$,

$$
\beta(w_j(E))=w_1(E)w_j(E)+(j+1)w_{j+1}(E).
$$

For a real line bundle $L$, one first has $\beta(w_1(L))=w_1(L)^2$. The general identity follows from the [splitting principle for real vector bundles](#splitting-principle-for-real-vector-bundles), the [Bockstein derivation rule](homology.md#bockstein-derivation-rule), and the elementary-symmetric-polynomial identity obtained by separating whether an index lies in a chosen $j$-element subset.

<h4 id="first-stiefel-whitney-class-of-a-tensor-product-of-real-line-bundles">First Stiefel–Whitney class of a tensor product of real line bundles</h4>

↑ **Parent:** [Stiefel–Whitney class](#stiefel-whitney-class)

Real line bundles are classified by $H^1(X;\mathbb F_2)$, and tensor product corresponds to addition:

$$
w_1(L\otimes L')=w_1(L)+w_1(L').
$$

<h4 id="total-stiefel-whitney-class-of-the-projectivization-of-copies-of-the-tautological-line">Total Stiefel–Whitney class of the projectivization of copies of the tautological line</h4>

↑ **Parent:** [Stiefel–Whitney class](#stiefel-whitney-class)

Under

$$
\mathbb P(k\gamma_{\mathbb R}^{1,n+1})
\cong\mathbb{RP}^n\times\mathbb{RP}^{k-1},
$$

let $x$ and $v$ be the degree-one generators. Then

$$
w(T\mathbb P(k\gamma_{\mathbb R}^{1,n+1}))
=(1+x)^{n+1}(1+v)^k.
$$

## Curvature form

↑ **Parent:** [Fiber bundle](fiber-bundle.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Curvature_form)

The [curvature form](#curvature-form) of a [connection on a vector bundle](#connection-vector-bundle) is $F=dA+A\wedge A$ in a local frame. A [principal connection](#connection-principal-bundle) has the corresponding [Lie algebra](lie-algebra.md)-valued form $F=dA+\tfrac12[A\wedge A]$. It measures the failure of horizontal directions to be integrable.

The curvature is $F(A)=d_A^2$ and in a local frame satisfies $F(A)=dA+A\wedge A$.

### Curvature of a principal connection

↑ **Parent:** [Curvature form](#curvature-form)

This is the principal-bundle version of the [curvature form](#curvature-form). The curvature of a [principal connection](#connection-principal-bundle) is the horizontal equivariant two-form

$$
\mathcal F=d\mathcal A+\frac12[\mathcal A\wedge\mathcal A].
$$

For horizontal vector fields $X,Y$, it satisfies $\mathcal F(X,Y)=-\mathcal A([X,Y])$.

#### Flat principal connection

↑ **Parent:** [Curvature of a principal connection](#curvature-of-a-principal-connection)

A principal connection is flat when its [curvature](#curvature-of-a-principal-connection) vanishes. The identity $\mathcal F(X,Y)=-\mathcal A([X,Y])$ shows that this is equivalent to integrability of its [horizontal distribution](#horizontal-distribution-of-a-principal-connection).

### Trace of vector-bundle curvature

↑ **Parent:** [Curvature form](#curvature-form)

The [trace](linear-algebra.md#matrix-trace) of the [curvature form of a connection](#curvature-form) is a global [closed differential form](differential-form.md#closed-differential-form) of degree two. Under a frame change $e'=eg$, the [connection matrix](#connection-one-form) and curvature change by $A'=g^{-1}Ag+g^{-1}dg$ and $\Theta'=g^{-1}\Theta g$. Thus [trace](linear-algebra.md#matrix-trace) is independent of frame. The [Bianchi identity](#bianchi-identity) gives $d\Theta=\Theta\wedge A-A\wedge\Theta$. Taking the [trace](linear-algebra.md#matrix-trace) cancels the two terms: one-forms commute with two-forms in the graded sense, and renaming the [matrix](vector-space.md#matrix) indices gives equality of their [traces](linear-algebra.md#matrix-trace). Locally $\operatorname{tr}\Theta=d\operatorname{tr}A$, since the [trace](linear-algebra.md#matrix-trace) of $A\wedge A$ vanishes by pairing its off-diagonal terms. It is the curvature of the [determinant connection](#determinant-connection).

### Cartan curvature matrix equation

↑ **Parent:** [Curvature form](#curvature-form)

For a [connection on a vector bundle](#connection-vector-bundle) written $D=d+A\wedge$ in a local frame, its [curvature form of a connection](#curvature-form) is represented by $\Theta=dA+A\wedge A$. The products combine matrix multiplication with the [exterior product](linear-algebra.md#exterior-product). The formula follows by squaring $D$ and using the graded [Leibniz rule](calculus.md#leibniz-rule).

#### Cartan curvature equation with input indices

↑ **Parent:** [Cartan curvature matrix equation](#cartan-curvature-matrix-equation)

Write $De_i=\sum_j\theta_{ij}\otimes e_j$, with the differentiated input index first. The graded [Leibniz rule](calculus.md#leibniz-rule) gives $D^2e_i=\sum_j(d\theta_{ij}-\sum_k\theta_{ik}\wedge\theta_{kj})\otimes e_j$. For frames $e'=ge$, the [connection matrix](#connection-one-form) transforms as $\theta'=dg\,g^{-1}+g\theta g^{-1}$ and curvature by $\Theta'=g\Theta g^{-1}$. Transposing to the usual coefficient-column convention gives $A=\theta^t$ and $F=dA+A\wedge A=\Theta^t$; the opposite sign is an index convention, not a different curvature.

### Riemannian curvature two-form

↑ **Parent:** [Curvature form](#curvature-form)

For the [Levi-Civita connection](general-relativity.md#levi-civita-connection), the [curvature form of a connection](#curvature-form) is the endomorphism-valued two-form

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z.
$$

It has [tensoriality](#tensoriality) in all three arguments. Its [first Bianchi identity](general-relativity.md#first-bianchi-identity) follows from torsion-freeness: the cyclic sum is $\sum_{\mathrm{cyc}}(\nabla_X[Y,Z]-\nabla_{[Y,Z]}X)=\sum_{\mathrm{cyc}}[X,[Y,Z]]=0$ by the [Jacobi identity](lie-algebra.md#jacobi-identity).

### Curvature difference formula

↑ **Parent:** [Curvature form](#curvature-form)

If two objects $\nabla_1$ and $\nabla_2$ are each a [connection on a vector bundle](#connection-vector-bundle) and satisfy $\nabla_1=\nabla_2+a$ for an $\operatorname{End}(E)$-valued one-form $a$, then

$$
F_{\nabla_1}=F_{\nabla_2}+d_{\nabla_2}a+a\wedge a.
$$

This follows by expanding $(\nabla_2+a)^2$ with the [covariant exterior derivative](#exterior-covariant-derivative) on the [endomorphism bundle connection](#endomorphism-bundle-connection).

#### Trace curvature transgression

↑ **Parent:** [Curvature difference formula](#curvature-difference-formula)

The difference of two [connections on a vector bundle](#connection-vector-bundle) is a global endomorphism-valued one-form. Taking the [trace](linear-algebra.md#matrix-trace) of the [curvature difference formula](#curvature-difference-formula) cancels both the commutator terms and the trace of the square of that one-form. Consequently the trace curvatures represent the same [de Rham cohomology](differential-form.md#de-rham-cohomology) class.

##### Connection-independent curvature class of a line bundle

↑ **Parent:** [Trace curvature transgression](#trace-curvature-transgression)

For a real or complex [line bundle](ringed-space.md#line-bundle), its [endomorphism bundle](#endomorphism-bundle) is canonically trivial by scalar multiplication. The [Bianchi identity](#bianchi-identity) therefore reduces to $dF_A=0$. The difference of two [connections on a vector bundle](#connection-vector-bundle) is a global endomorphism-valued one-form, which here is an ordinary scalar one-form $a$. Since scalar one-forms have vanishing wedge square, the [curvature difference formula](#curvature-difference-formula) reduces to $F_{A+a}-F_A=da$. Thus the [de Rham cohomology](differential-form.md#de-rham-cohomology) class is independent of the [connection on a vector bundle](#connection-vector-bundle).

### Bianchi identity

↑ **Parent:** [Curvature form](#curvature-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bianchi_identity)

The curvature of a connection satisfies $d_AF(A)=0$. In a local frame this follows directly by expanding $d(dA+A\wedge A)+A\wedge F-F\wedge A$.

## ↑ Ancestors (5)

1. [Algebraic topology](algebraic-topology.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (29)

- [A sphere cannot fibre over a lower-dimensional odd sphere](algebraic-topology.md#a-sphere-cannot-fibre-over-a-lower-dimensional-odd-sphere)
- [Affine bundle](#affine-bundle)
- [Circle bundle](#circle-bundle)
- [Cohomological obstruction to a section of the twistor bundle](#cohomological-obstruction-to-a-section-of-the-twistor-bundle)
- [Compact first-cohomology obstruction to a Lagrangian fibration](symplectic-geometry.md#compact-first-cohomology-obstruction-to-a-lagrangian-fibration)
- [Ehresmann fibration theorem](#ehresmann-fibration-theorem)
- [Fiber-curve surgery](knot-theory.md#fiber-curve-surgery)
- [Lefschetz fibration](symplectic-geometry.md#lefschetz-fibration)
- [Leray-Hirsch theorem](#leray-hirsch-theorem)
- [Local basis criterion for Leray-Hirsch classes](#local-basis-criterion-for-leray-hirsch-classes)
- [Local trivialization](#local-trivialization)
- [Mapping torus](algebraic-topology.md#mapping-torus)
- [Mapping-torus homology from Mayer–Vietoris](algebraic-topology.md#mapping-torus-homology-from-mayer-vietoris)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-16.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-63.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-65.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-16.md#4/4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-16.md#5/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-17.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-14.md#2/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-114.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-114.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-115.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-127.md#2/solution)
- [Principal bundle](#principal-bundle)
- [Section (fiber bundle)](#section-fiber-bundle)
- [Special orthogonal sphere fibration](linear-algebra.md#special-orthogonal-sphere-fibration)
