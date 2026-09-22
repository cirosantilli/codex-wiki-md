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
- [Vector bundle](vector-bundle.md)
  - [Density bundle](vector-bundle.md#density-bundle)
    - [Riemannian volume density](vector-bundle.md#riemannian-volume-density)
  - [Tensor bundle](vector-bundle.md#tensor-bundle)
  - [G-structure on a vector bundle](vector-bundle.md#g-structure-on-a-vector-bundle)
  - [Globally generated vector bundle](vector-bundle.md#globally-generated-vector-bundle)
    - [Global generation of positive twists on a smooth curve](vector-bundle.md#global-generation-of-positive-twists-on-a-smooth-curve)
    - [Nowhere-vanishing section of a globally generated bundle on a curve](vector-bundle.md#nowhere-vanishing-section-of-a-globally-generated-bundle-on-a-curve)
  - [Whitney sum of vector bundles](vector-bundle.md#whitney-sum-of-vector-bundles)
  - [Symplectic vector bundle](vector-bundle.md#symplectic-vector-bundle)
    - [Lagrangian subbundle](vector-bundle.md#lagrangian-subbundle)
  - [Thom space](vector-bundle.md#thom-space)
    - [Projective-space quotient as a Thom space of conjugate tautological lines](vector-bundle.md#projective-space-quotient-as-a-thom-space-of-conjugate-tautological-lines)
  - [Line subbundle](vector-bundle.md#line-subbundle)
  - [Birkhoff–Grothendieck theorem](vector-bundle.md#birkhoff-grothendieck-theorem)
  - [Stable framing of a vector bundle](vector-bundle.md#stable-framing-of-a-vector-bundle)
  - [Endomorphism bundle](vector-bundle.md#endomorphism-bundle)
  - [Exterior power of a vector bundle](vector-bundle.md#exterior-power-of-a-vector-bundle)
  - [Clutching construction](vector-bundle.md#clutching-construction)
    - [Clutching function](vector-bundle.md#clutching-function)
      - [Section obstruction for a clutched vector bundle](vector-bundle.md#section-obstruction-for-a-clutched-vector-bundle)
  - [Clifford module bundle](vector-bundle.md#clifford-module-bundle)
  - [Determinant line bundle](vector-bundle.md#determinant-line-bundle)
  - [Zero section of a vector bundle](vector-bundle.md#zero-section-of-a-vector-bundle)
  - [Fiber metric](vector-bundle.md#fiber-metric)
    - [Orthogonal structure on a real vector bundle](vector-bundle.md#orthogonal-structure-on-a-real-vector-bundle)
      - [Euclidean orthonormal frame](vector-bundle.md#euclidean-orthonormal-frame)
      - [Orthogonal local trivialization](vector-bundle.md#orthogonal-local-trivialization)
  - [Eigenbundle](vector-bundle.md#eigenbundle)
  - [Hermitian vector bundle](vector-bundle.md#hermitian-vector-bundle)
  - [Complex vector bundle](vector-bundle.md#complex-vector-bundle)
    - [Hermitian metric on a smooth complex vector bundle](vector-bundle.md#hermitian-metric-on-a-smooth-complex-vector-bundle)
    - [Stable complex structure on a real vector bundle](vector-bundle.md#stable-complex-structure-on-a-real-vector-bundle)
    - [Conjugate vector bundle](vector-bundle.md#conjugate-vector-bundle)
      - [Conjugate connection](vector-bundle.md#conjugate-connection)
  - [Rank of a vector bundle](vector-bundle.md#rank-of-a-vector-bundle)
  - [Vector bundle morphism](vector-bundle.md#vector-bundle-morphism)
    - [Kernel bundle of a surjective vector bundle morphism](vector-bundle.md#kernel-bundle-of-a-surjective-vector-bundle-morphism)
    - [Vector bundle endomorphism](vector-bundle.md#vector-bundle-endomorphism)
    - [Holomorphic bundle map](vector-bundle.md#holomorphic-bundle-map)
    - [Bundle morphisms from maps of smooth sections](vector-bundle.md#bundle-morphisms-from-maps-of-smooth-sections)
    - [Vector bundle isomorphism](vector-bundle.md#vector-bundle-isomorphism)
  - [Vector bundle trivialization](vector-bundle.md#vector-bundle-trivialization)
    - [Frame of a vector bundle](vector-bundle.md#frame-of-a-vector-bundle)
      - [Pseudo-orthonormal frame](vector-bundle.md#pseudo-orthonormal-frame)
      - [Coframe](vector-bundle.md#coframe)
  - [Complexification of a real vector bundle](vector-bundle.md#complexification-of-a-real-vector-bundle)
  - [Projective bundle](vector-bundle.md#projective-bundle)
    - [Projectivization by quotients](vector-bundle.md#projectivization-by-quotients)
      - [Universal quotient line bundle](vector-bundle.md#universal-quotient-line-bundle)
      - [Rational normal scroll](vector-bundle.md#rational-normal-scroll)
        - [Fiber class of a rational normal scroll](vector-bundle.md#fiber-class-of-a-rational-normal-scroll)
        - [Isomorphism classification of abstract rational scrolls](vector-bundle.md#isomorphism-classification-of-abstract-rational-scrolls)
    - [Chern classes of a tautological-line complement](vector-bundle.md#chern-classes-of-a-tautological-line-complement)
    - [Holomorphic projectivization by lines](vector-bundle.md#holomorphic-projectivization-by-lines)
      - [Relative tautological line bundle](vector-bundle.md#relative-tautological-line-bundle)
        - [Relative hyperplane line bundle](vector-bundle.md#relative-hyperplane-line-bundle)
    - [Sections of a projective bundle](vector-bundle.md#sections-of-a-projective-bundle)
    - [Orthogonal complex line flag manifold](vector-bundle.md#orthogonal-complex-line-flag-manifold)
      - [Cohomology ring of the orthogonal complex line flag manifold](vector-bundle.md#cohomology-ring-of-the-orthogonal-complex-line-flag-manifold)
    - [Projective bundle formula for complex vector bundles](vector-bundle.md#projective-bundle-formula-for-complex-vector-bundles)
  - [Complex line bundle](vector-bundle.md#complex-line-bundle)
    - [Smooth exponential sequence](vector-bundle.md#smooth-exponential-sequence)
    - [Smooth classification of complex line bundles on the complex projective line](vector-bundle.md#smooth-classification-of-complex-line-bundles-on-the-complex-projective-line)
  - [Real line bundle](vector-bundle.md#real-line-bundle)
    - [Möbius line bundle](vector-bundle.md#mobius-line-bundle)
    - [Classification of real line bundles](vector-bundle.md#classification-of-real-line-bundles)
    - [Mod-two Euler class of a real line bundle](vector-bundle.md#mod-two-euler-class-of-a-real-line-bundle)
  - [Vector subbundle](vector-bundle.md#vector-subbundle)
    - [Orthogonal splitting of a vector subbundle](vector-bundle.md#orthogonal-splitting-of-a-vector-subbundle)
    - [Quotient vector bundle](vector-bundle.md#quotient-vector-bundle)
      - [Universal quotient bundle on a real Grassmannian](vector-bundle.md#universal-quotient-bundle-on-a-real-grassmannian)
        - [Universal quotient bundle need not have a nowhere-zero section](vector-bundle.md#universal-quotient-bundle-need-not-have-a-nowhere-zero-section)
        - [Classification of vector bundles by a universal quotient bundle](vector-bundle.md#classification-of-vector-bundles-by-a-universal-quotient-bundle)
  - [Trivial vector bundle](vector-bundle.md#trivial-vector-bundle)
  - [Section of a vector bundle](vector-bundle.md#section-of-a-vector-bundle)
    - [Regular zero locus](vector-bundle.md#regular-zero-locus)
    - [Module of smooth sections](vector-bundle.md#module-of-smooth-sections)
    - [Nowhere-zero section](vector-bundle.md#nowhere-zero-section)
      - [Nonvanishing tangent field on an odd-dimensional sphere](vector-bundle.md#nonvanishing-tangent-field-on-an-odd-dimensional-sphere)
      - [Splitting a trivial line from a nowhere-zero section](vector-bundle.md#splitting-a-trivial-line-from-a-nowhere-zero-section)
      - [Hairy ball theorem](vector-bundle.md#hairy-ball-theorem)
        - [Degree proof of the hairy ball theorem](vector-bundle.md#degree-proof-of-the-hairy-ball-theorem)
  - [Sphere bundle](vector-bundle.md#sphere-bundle)
    - [Three-sphere bundle over the four-sphere](vector-bundle.md#three-sphere-bundle-over-the-four-sphere)
    - [Unit tangent bundle](vector-bundle.md#unit-tangent-bundle)
      - [Canonical coframe of a surface unit tangent bundle](vector-bundle.md#canonical-coframe-of-a-surface-unit-tangent-bundle)
        - [Vertical vector field of a surface unit tangent bundle](vector-bundle.md#vertical-vector-field-of-a-surface-unit-tangent-bundle)
        - [Liouville volume of a surface geodesic flow](vector-bundle.md#liouville-volume-of-a-surface-geodesic-flow)
      - [Stiefel manifold](vector-bundle.md#stiefel-manifold)
        - [Unordered Stiefel bundle](vector-bundle.md#unordered-stiefel-bundle)
          - [Subset cover of a framed vector bundle](vector-bundle.md#subset-cover-of-a-framed-vector-bundle)
        - [Complex Stiefel manifold](vector-bundle.md#complex-stiefel-manifold)
          - [Integral cohomology of a complex Stiefel manifold](vector-bundle.md#integral-cohomology-of-a-complex-stiefel-manifold)
          - [Complement bundle on a complex Stiefel manifold](vector-bundle.md#complement-bundle-on-a-complex-stiefel-manifold)
      - [Cohomology of the unit tangent bundle of an even-dimensional sphere](vector-bundle.md#cohomology-of-the-unit-tangent-bundle-of-an-even-dimensional-sphere)
  - [Disk bundle](vector-bundle.md#disk-bundle)
    - [Plumbing of oriented disk bundles](vector-bundle.md#plumbing-of-oriented-disk-bundles)
  - [Tangent bundle](vector-bundle.md#tangent-bundle)
    - [Stabilized tangent bundle of real projective space](vector-bundle.md#stabilized-tangent-bundle-of-real-projective-space)
    - [Tangent coordinate transition](vector-bundle.md#tangent-coordinate-transition)
  - [Projectivization of a real vector bundle](vector-bundle.md#projectivization-of-a-real-vector-bundle)
    - [Tangent bundle of a projectivized real vector bundle](vector-bundle.md#tangent-bundle-of-a-projectivized-real-vector-bundle)
    - [Projectivization of copies of the real tautological line bundle](vector-bundle.md#projectivization-of-copies-of-the-real-tautological-line-bundle)
  - [Dual bundle](vector-bundle.md#dual-bundle)
    - [Canonical trivialization of a line bundle tensored with its dual](vector-bundle.md#canonical-trivialization-of-a-line-bundle-tensored-with-its-dual)
  - [Pullback vector bundle](vector-bundle.md#pullback-vector-bundle)
    - [Pullback tangent bundle](vector-bundle.md#pullback-tangent-bundle)
      - [Vector field along a map](vector-bundle.md#vector-field-along-a-map)
        - [Local extension of a vector field along a submanifold](vector-bundle.md#local-extension-of-a-vector-field-along-a-submanifold)
        - [Vector field along a curve](vector-bundle.md#vector-field-along-a-curve)
  - [Kernel bundle of a constant-rank family of linear maps](vector-bundle.md#kernel-bundle-of-a-constant-rank-family-of-linear-maps)
  - [Tensor product of vector bundles](vector-bundle.md#tensor-product-of-vector-bundles)
    - [Second Chern class of a tensor product of rank-two bundles](vector-bundle.md#second-chern-class-of-a-tensor-product-of-rank-two-bundles)
    - [Tensor field](vector-bundle.md#tensor-field)
      - [Lie derivative of a covariant tensor field](vector-bundle.md#lie-derivative-of-a-covariant-tensor-field)
      - [Tensoriality](vector-bundle.md#tensoriality)
      - [Tensor derivation](vector-bundle.md#tensor-derivation)
        - [Lie derivative of a tensor field](vector-bundle.md#lie-derivative-of-a-tensor-field)
          - [Lie derivative at a zero of its generator](vector-bundle.md#lie-derivative-at-a-zero-of-its-generator)
          - [Coordinate tensor Lie derivative](vector-bundle.md#coordinate-tensor-lie-derivative)
          - [Commutator identity for Lie derivatives](vector-bundle.md#commutator-identity-for-lie-derivatives)
          - [Lie derivative of a vector field](vector-bundle.md#lie-derivative-of-a-vector-field)
          - [Lie derivative of a function](vector-bundle.md#lie-derivative-of-a-function)
          - [Flow definition of the Lie derivative of a tensor field](vector-bundle.md#flow-definition-of-the-lie-derivative-of-a-tensor-field)
          - [Scaled Lie derivative defect identity](vector-bundle.md#scaled-lie-derivative-defect-identity)
        - [Endomorphism-induced tensor derivation](vector-bundle.md#endomorphism-induced-tensor-derivation)
  - [Connection (vector bundle)](vector-bundle.md#connection-vector-bundle)
    - [Parallel vector field](vector-bundle.md#parallel-vector-field)
    - [Projection connection](vector-bundle.md#projection-connection)
    - [Connection difference as an endomorphism-valued one-form](vector-bundle.md#connection-difference-as-an-endomorphism-valued-one-form)
    - [Change of frame of a vector-bundle connection](vector-bundle.md#change-of-frame-of-a-vector-bundle-connection)
    - [Affine space of vector-bundle connections](vector-bundle.md#affine-space-of-vector-bundle-connections)
    - [Construction of a vector bundle connection by a partition of unity](vector-bundle.md#construction-of-a-vector-bundle-connection-by-a-partition-of-unity)
    - [Determinant connection](vector-bundle.md#determinant-connection)
    - [Rough Laplacian](vector-bundle.md#rough-laplacian)
    - [Affine connection](vector-bundle.md#affine-connection)
      - [Projective equivalence of affine connections](vector-bundle.md#projective-equivalence-of-affine-connections)
        - [Geodesic reparametrization under projective equivalence](vector-bundle.md#geodesic-reparametrization-under-projective-equivalence)
        - [Projective covector from metric volume densities](vector-bundle.md#projective-covector-from-metric-volume-densities)
      - [Bracket connection on a Lie group](vector-bundle.md#bracket-connection-on-a-lie-group)
      - [Connection components](vector-bundle.md#connection-components)
      - [Affine exponential map](vector-bundle.md#affine-exponential-map)
        - [Affine normal coordinates](vector-bundle.md#affine-normal-coordinates)
      - [Affine connection decomposition](vector-bundle.md#affine-connection-decomposition)
      - [Nonmetricity tensor](vector-bundle.md#nonmetricity-tensor)
        - [Disformation tensor](vector-bundle.md#disformation-tensor)
      - [Torsion tensor](vector-bundle.md#torsion-tensor)
        - [Contorsion tensor](vector-bundle.md#contorsion-tensor)
      - [Parallel covector field](vector-bundle.md#parallel-covector-field)
      - [Projected ambient connection](vector-bundle.md#projected-ambient-connection)
      - [Difference of affine connections is a tensor](vector-bundle.md#difference-of-affine-connections-is-a-tensor)
        - [Parametrized geodesics determine the symmetric part of an affine connection](vector-bundle.md#parametrized-geodesics-determine-the-symmetric-part-of-an-affine-connection)
          - [Torsion-free connections are determined by their parametrized geodesics](vector-bundle.md#torsion-free-connections-are-determined-by-their-parametrized-geodesics)
      - [Affine connection for a velocity-linear force](vector-bundle.md#affine-connection-for-a-velocity-linear-force)
      - [Product affine connection](vector-bundle.md#product-affine-connection)
        - [Curvature splitting for a product connection](vector-bundle.md#curvature-splitting-for-a-product-connection)
    - [Covariant derivative along a curve](vector-bundle.md#covariant-derivative-along-a-curve)
    - [Connection one-form](vector-bundle.md#connection-one-form)
    - [Exterior covariant derivative](vector-bundle.md#exterior-covariant-derivative)
      - [Endomorphism-valued exterior product](vector-bundle.md#endomorphism-valued-exterior-product)
    - [Horizontal subspace of a vector bundle connection](vector-bundle.md#horizontal-subspace-of-a-vector-bundle-connection)
      - [Linear horizontal distribution on a vector bundle](vector-bundle.md#linear-horizontal-distribution-on-a-vector-bundle)
      - [Horizontal connection associated to a covariant derivative](vector-bundle.md#horizontal-connection-associated-to-a-covariant-derivative)
    - [Pullback connection](vector-bundle.md#pullback-connection)
      - [Curvature of a pullback connection](vector-bundle.md#curvature-of-a-pullback-connection)
      - [Restriction of a connection to an embedded submanifold](vector-bundle.md#restriction-of-a-connection-to-an-embedded-submanifold)
    - [Dual connection](vector-bundle.md#dual-connection)
    - [Tensor product connection](vector-bundle.md#tensor-product-connection)
      - [Curvature of a tensor product connection](vector-bundle.md#curvature-of-a-tensor-product-connection)
    - [Endomorphism bundle connection](vector-bundle.md#endomorphism-bundle-connection)
      - [Commutator identity for an endomorphism connection](vector-bundle.md#commutator-identity-for-an-endomorphism-connection)
      - [Curvature of an endomorphism bundle connection](vector-bundle.md#curvature-of-an-endomorphism-bundle-connection)
        - [Scalar-curvature criterion for a flat endomorphism connection](vector-bundle.md#scalar-curvature-criterion-for-a-flat-endomorphism-connection)
    - [Solder form](vector-bundle.md#solder-form)
      - [Torsion form](vector-bundle.md#torsion-form)
        - [Cartan first structure equation with input-first indices](vector-bundle.md#cartan-first-structure-equation-with-input-first-indices)
        - [Torsion-free connection](vector-bundle.md#torsion-free-connection)
    - [Metric connection](vector-bundle.md#metric-connection)
      - [Metric compatibility](vector-bundle.md#metric-compatibility)
        - [Lie derivative of a metric with nonmetricity](vector-bundle.md#lie-derivative-of-a-metric-with-nonmetricity)
      - [Normal connection](vector-bundle.md#normal-connection)
      - [Skew-adjoint difference criterion for metric connections](vector-bundle.md#skew-adjoint-difference-criterion-for-metric-connections)
      - [Smooth unitary frame for a Hermitian connection](vector-bundle.md#smooth-unitary-frame-for-a-hermitian-connection)
      - [Parallel transport preserves a fibre metric](vector-bundle.md#parallel-transport-preserves-a-fibre-metric)
      - [Connection matrix in an orthonormal frame is skew-symmetric](vector-bundle.md#connection-matrix-in-an-orthonormal-frame-is-skew-symmetric)
      - [Koszul formula](vector-bundle.md#koszul-formula)
        - [Existence and uniqueness of the Levi-Civita connection](vector-bundle.md#existence-and-uniqueness-of-the-levi-civita-connection)
      - [Unitary connection](vector-bundle.md#unitary-connection)
        - [Uhlenbeck small-energy Coulomb gauge](vector-bundle.md#uhlenbeck-small-energy-coulomb-gauge)
        - [Harmonic-curvature unitary line connection](vector-bundle.md#harmonic-curvature-unitary-line-connection)
        - [Unitary bundle gauge transformation](vector-bundle.md#unitary-bundle-gauge-transformation)
          - [Unitary bundle gauge group](vector-bundle.md#unitary-bundle-gauge-group)
            - [Coulomb slice for unitary connections](vector-bundle.md#coulomb-slice-for-unitary-connections)
            - [Based unitary gauge group](vector-bundle.md#based-unitary-gauge-group)
        - [Anti-self-dual connection](vector-bundle.md#anti-self-dual-connection)
          - [Abelian anti-self-dual connections from harmonic scalar potentials](vector-bundle.md#abelian-anti-self-dual-connections-from-harmonic-scalar-potentials)
          - [ASD deformation complex](vector-bundle.md#asd-deformation-complex)
            - [Local cone at an unobstructed reducible SU2 instanton](vector-bundle.md#local-cone-at-an-unobstructed-reducible-su2-instanton)
            - [ASD deformation index](vector-bundle.md#asd-deformation-index)
          - [Uhlenbeck-Donaldson compactness for charge-one ASD connections](vector-bundle.md#uhlenbeck-donaldson-compactness-for-charge-one-asd-connections)
          - [Uhlenbeck removable singularity theorem for ASD connections](vector-bundle.md#uhlenbeck-removable-singularity-theorem-for-asd-connections)
          - [Positive-square obstruction to ASD line connections](vector-bundle.md#positive-square-obstruction-to-asd-line-connections)
    - [Horizontal lift](vector-bundle.md#horizontal-lift)
      - [Parallel transport](vector-bundle.md#parallel-transport)
        - [Parallel vector field along a curve](vector-bundle.md#parallel-vector-field-along-a-curve)
        - [Parallel transport around a spherical triangle](vector-bundle.md#parallel-transport-around-a-spherical-triangle)
        - [Global continuation of linear parallel transport](vector-bundle.md#global-continuation-of-linear-parallel-transport)
        - [Parallel frame along a curve](vector-bundle.md#parallel-frame-along-a-curve)
        - [Parallel transport on an endomorphism bundle](vector-bundle.md#parallel-transport-on-an-endomorphism-bundle)
        - [Parallel transport around a latitude of the unit sphere](vector-bundle.md#parallel-transport-around-a-latitude-of-the-unit-sphere)
  - [Orientation of a vector bundle](vector-bundle.md#orientation-of-a-vector-bundle)
    - [Orientability of a vector bundle total space](vector-bundle.md#orientability-of-a-vector-bundle-total-space)
    - [Canonical orientation of a complex vector bundle](vector-bundle.md#canonical-orientation-of-a-complex-vector-bundle)
    - [Thom class](vector-bundle.md#thom-class)
      - [Cohomology class of a cooriented submanifold](vector-bundle.md#cohomology-class-of-a-cooriented-submanifold)
      - [Thom class in a generalized cohomology theory](vector-bundle.md#thom-class-in-a-generalized-cohomology-theory)
      - [Cup square of a Thom class](vector-bundle.md#cup-square-of-a-thom-class)
      - [Thom isomorphism theorem](vector-bundle.md#thom-isomorphism-theorem)
        - [Gysin sequence of an embedding](vector-bundle.md#gysin-sequence-of-an-embedding)
          - [Cohomological Gysin map of an embedding](vector-bundle.md#cohomological-gysin-map-of-an-embedding)
      - [Euler class of a vector bundle](vector-bundle.md#euler-class-of-a-vector-bundle)
        - [Euler class in a generalized cohomology theory](vector-bundle.md#euler-class-in-a-generalized-cohomology-theory)
          - [A nowhere-zero section annihilates generalized Euler classes](vector-bundle.md#a-nowhere-zero-section-annihilates-generalized-euler-classes)
        - [Euler class of a complex vector bundle](vector-bundle.md#euler-class-of-a-complex-vector-bundle)
        - [Euler class of an oriented odd-rank vector bundle is two-torsion](vector-bundle.md#euler-class-of-an-oriented-odd-rank-vector-bundle-is-two-torsion)
        - [Whitney product formula for Euler classes](vector-bundle.md#whitney-product-formula-for-euler-classes)
        - [Euler number of a vector bundle](vector-bundle.md#euler-number-of-a-vector-bundle)
        - [Poincaré-Hopf theorem](vector-bundle.md#poincare-hopf-theorem)
        - [Euler class of a complex line bundle](vector-bundle.md#euler-class-of-a-complex-line-bundle)
        - [Gysin sequence of a sphere bundle](vector-bundle.md#gysin-sequence-of-a-sphere-bundle)
          - [Gysin ring splitting for an odd-dimensional sphere bundle](vector-bundle.md#gysin-ring-splitting-for-an-odd-dimensional-sphere-bundle)
          - [Projection formula for sphere bundle integration](vector-bundle.md#projection-formula-for-sphere-bundle-integration)
          - [Unoriented Gysin sequence](vector-bundle.md#unoriented-gysin-sequence)
          - [Three-dimensional lens space as a circle bundle](vector-bundle.md#three-dimensional-lens-space-as-a-circle-bundle)
          - [Integral cohomology of a circle bundle over a product of two spheres](vector-bundle.md#integral-cohomology-of-a-circle-bundle-over-a-product-of-two-spheres)
  - [Tautological bundle](vector-bundle.md#tautological-bundle)
    - [Complex tautological bundle on a Grassmannian](vector-bundle.md#complex-tautological-bundle-on-a-grassmannian)
      - [Classification of complex vector bundles by a Grassmannian](vector-bundle.md#classification-of-complex-vector-bundles-by-a-grassmannian)
        - [Rank-two complex vector bundles over the four-sphere](vector-bundle.md#rank-two-complex-vector-bundles-over-the-four-sphere)
        - [Close orthogonal projections identify their image bundles](vector-bundle.md#close-orthogonal-projections-identify-their-image-bundles)
        - [Finite-dimensional embedding of a complex vector bundle](vector-bundle.md#finite-dimensional-embedding-of-a-complex-vector-bundle)
    - [Complex tautological line bundle](vector-bundle.md#complex-tautological-line-bundle)
      - [Punctured line bundles do not determine their duality sign](vector-bundle.md#punctured-line-bundles-do-not-determine-their-duality-sign)
      - [Unitary transitions of the tautological line over the projective line](vector-bundle.md#unitary-transitions-of-the-tautological-line-over-the-projective-line)
      - [Global holomorphic sections of the complex tautological line bundle vanish](vector-bundle.md#global-holomorphic-sections-of-the-complex-tautological-line-bundle-vanish)
      - [Hyperplane line bundle](vector-bundle.md#hyperplane-line-bundle)
        - [Hyperplane class](vector-bundle.md#hyperplane-class)
        - [Nontrivial hyperplane powers on a compact projective submanifold](vector-bundle.md#nontrivial-hyperplane-powers-on-a-compact-projective-submanifold)
        - [Tensor powers of the hyperplane line bundle](vector-bundle.md#tensor-powers-of-the-hyperplane-line-bundle)
    - [Quaternionic tautological line bundle](vector-bundle.md#quaternionic-tautological-line-bundle)
    - [Real tautological line bundle](vector-bundle.md#real-tautological-line-bundle)
  - [Stiefel–Whitney class](vector-bundle.md#stiefel-whitney-class)
    - [Parity of zeros of a real line-bundle section](vector-bundle.md#parity-of-zeros-of-a-real-line-bundle-section)
    - [Codimension-one Stiefel–Whitney immersion obstruction](vector-bundle.md#codimension-one-stiefel-whitney-immersion-obstruction)
    - [Stiefel–Whitney class of the underlying real bundle of a complex line](vector-bundle.md#stiefel-whitney-class-of-the-underlying-real-bundle-of-a-complex-line)
    - [Projective bundle definition of Stiefel–Whitney classes](vector-bundle.md#projective-bundle-definition-of-stiefel-whitney-classes)
    - [Splitting principle for real vector bundles](vector-bundle.md#splitting-principle-for-real-vector-bundles)
      - [Whitney product formula for Stiefel–Whitney classes](vector-bundle.md#whitney-product-formula-for-stiefel-whitney-classes)
        - [Stiefel–Whitney obstruction to a diagonal projective immersion](vector-bundle.md#stiefel-whitney-obstruction-to-a-diagonal-projective-immersion)
    - [Bockstein of a Stiefel–Whitney class](vector-bundle.md#bockstein-of-a-stiefel-whitney-class)
    - [First Stiefel–Whitney class of a tensor product of real line bundles](vector-bundle.md#first-stiefel-whitney-class-of-a-tensor-product-of-real-line-bundles)
    - [Total Stiefel–Whitney class of the projectivization of copies of the tautological line](vector-bundle.md#total-stiefel-whitney-class-of-the-projectivization-of-copies-of-the-tautological-line)
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

A [fiber bundle](fiber-bundle.md) whose fibers are [affine spaces](geometry-and-topology.md#affine-space) and whose transition functions are affine. Differences of points in one fiber lie in a corresponding model [vector bundle](vector-bundle.md), but there need not be a preferred zero in each fiber.

## Section (fiber bundle)

↑ **Parent:** [Fiber bundle](fiber-bundle.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Section_(fiber_bundle))

A section of a [fiber bundle](fiber-bundle.md) $\pi:E\to B$ is a continuous map $s:B\to E$ with $\pi\circ s=\mathrm{id}_B$. It chooses a point of each fibre continuously. A [section of a vector bundle](vector-bundle.md#section-of-a-vector-bundle) is the special case for vector fibres; a [projective bundle](vector-bundle.md#projective-bundle) section chooses a line in each fibre of the underlying [vector bundle](vector-bundle.md).

### Cohomological obstruction to a section of the twistor bundle

↑ **Parent:** [Section (fiber bundle)](#section-fiber-bundle)

If the displayed [fiber bundle](fiber-bundle.md) had a section $s$, its projection $p$ would satisfy $s^*p^*=1$. The [cohomology ring of complex projective space](algebraic-topology.md#cohomology-ring-of-complex-projective-space) is $\mathbb Z[h]/(h^4)$ with $|h|=2$. For a generator $u\in H^4(S^4;\mathbb Z)$, write $p^*u=mh^2$. But $s^*h=0$ since $H^2(S^4;\mathbb Z)=0$, giving $u=s^*p^*u=0$. This contradiction proves that no section exists, without needing the value of $m$.

## Leray-Hirsch theorem

↑ **Parent:** [Fiber bundle](fiber-bundle.md)

For a [fiber bundle](fiber-bundle.md) $\pi:E\to B$ admitting a finite trivializing open cover, whose fiber has finite free [cohomology](cohomology.md) over $R$, suppose classes $e_j\in H^*(E;R)$ restrict to a basis on every fiber. Then multiplication $a\otimes e_j\mapsto\pi^*a\smile e_j$ gives the indicated module isomorphism. A finite trivializing open cover suffices, by the local [Künneth theorem](cohomology.md#kunneth-theorem) and the [Mayer–Vietoris sequence](algebraic-topology.md#mayer-vietoris-sequence). This determines an additive module structure; multiplicative relations must still be computed. Powers of the hyperplane class on a complex [projective bundle](vector-bundle.md#projective-bundle) provide an important application.

### Finite-cover proof of the Leray-Hirsch theorem

↑ **Parent:** [Leray-Hirsch theorem](#leray-hirsch-theorem)

For global [cohomology classes](cohomology.md#cohomology-class) satisfying the [local basis criterion for Leray-Hirsch classes](#local-basis-criterion-for-leray-hirsch-classes), multiplication commutes with the [Mayer–Vietoris sequence](algebraic-topology.md#mayer-vietoris-sequence), including its connecting homomorphism: multiply cochains on the right by global cocycle representatives. Induct over a finite trivializing open cover. If $U$ is a union of $r-1$ patches and $V$ is the last patch, $U\cap V$ has a cover by at most $r-1$ trivialized intersections. The induction hypothesis on $U$, $V$ and $U\cap V$, followed by the [Five lemma](category-theory.md#five-lemma), proves the theorem on $U\cup V$. A [compact](topology.md#compact-space) base supplies the finite cover.

### Local basis criterion for Leray-Hirsch classes

↑ **Parent:** [Leray-Hirsch theorem](#leray-hirsch-theorem)

On a trivialized [fiber bundle](fiber-bundle.md) over $U$, assume the fiber has finite-dimensional total [cohomology](cohomology.md) over a [field](algebra.md#field). The [Künneth theorem](cohomology.md#kunneth-theorem) identifies the total-space cohomology with a finite free graded module over $H^*(U)$. Classes restricting to a basis on every fiber give an invertible change of generators: its degree-zero coefficient blocks are invertible on each path component, while its positive-base-degree terms strictly decrease fiber degree and are therefore nilpotent. Inverting the diagonal blocks and then using a finite geometric series proves that multiplication by the chosen classes is an [isomorphism](algebra.md#isomorphism) over $U$.

## Local trivialization

↑ **Parent:** [Fiber bundle](fiber-bundle.md)

A local trivialization of a [fiber bundle](fiber-bundle.md) $p:E\to B$ over an open set $U\subseteq B$ is a [homeomorphism](topology.md#homeomorphism) $p^{-1}(U)\cong U\times F$ commuting with the projections to $U$. For a [vector bundle](vector-bundle.md), it must be linear on each fiber. Compatible local trivializations specify the bundle structure and give its transition functions on overlaps.

### Transition function of a vector bundle

↑ **Parent:** [Local trivialization](#local-trivialization)

Two local frames of a [vector bundle](vector-bundle.md) differ on their overlap by an invertible matrix-valued function. These functions satisfy the [Čech cocycle condition](sheaf-of-modules.md#cech-cocycle-condition). For a [holomorphic vector bundle](complex-geometry.md#holomorphic-vector-bundle) they are [holomorphic](holomorphic-function.md), and for a [holomorphic line bundle](complex-geometry.md#holomorphic-line-bundle) they are scalar holomorphic units.

#### Structure group of a vector bundle

↑ **Parent:** [Transition function of a vector bundle](#transition-function-of-a-vector-bundle)

A [complex vector bundle](vector-bundle.md#complex-vector-bundle) has structure group $G$ when it admits fiber-linear [local trivializations](#local-trivialization) whose transition matrices take values in $G$. Replacing frames by $h_i$ changes transitions to $h_i^{-1}g_{ij}h_j$ in the frame convention. Reducing the structure group means choosing new trivializations with values in a specified subgroup. The same transitions glue $U_i\times G$ by left multiplication to a right [principal bundle](#principal-bundle).

## Circle bundle

↑ **Parent:** [Fiber bundle](fiber-bundle.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circle_bundle)

A circle bundle is a [fiber bundle](fiber-bundle.md) with fiber $S^1$. Oriented circle bundles over a paracompact base are classified by their [Euler class](vector-bundle.md#euler-class-of-a-vector-bundle) in $H^2(B;\mathbb Z)$.

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

Write a point of [Real projective space](algebraic-topology.md#real-projective-space) as a nonzero vector $(w_1,w_2)\in\mathbb C^2$ modulo real nonzero scaling. The map to [Complex projective space](algebraic-topology.md#complex-projective-space) sends its class to the complex line through that vector. A free right action of the [circle group](lie-theory.md#circle-group) is $[w]\cdot u=[\lambda w]$ where $\lambda^2=u$; the two possible roots differ by a real sign and therefore give the same projective point. Local smooth square-root branches prove smoothness. Over $[z:1]$, the fibre coordinate is $(w_2/|w_2|)^2$; over $[1:\zeta]$, it is $(w_1/|w_1|)^2$. On the overlap $\zeta=1/z$, the [transition function of a principal bundle](#transition-function-of-a-principal-bundle) is $u\mapsto(z/\overline z)u$. Its phase winds twice. Ordinary scalar multiplication by $u$ instead has a kernel of order two and is not a [free action of a group](group-action.md#free-action-of-a-group).

### Transition function of a principal bundle

↑ **Parent:** [Principal bundle](#principal-bundle)

For equivariant [local trivializations](#local-trivialization) of a right [principal bundle](#principal-bundle), the change of coordinates is left multiplication in the group coordinate. Indeed an equivariant change $H$ satisfies $H(x,gh)=H(x,g)h$, so evaluating at the identity gives $H(x,g)=(x,\psi(x)g)$. Its inverse shows that $\psi$ takes values in the [Lie group](lie-theory.md#lie-group), and restriction to $(x,e)$ makes it smooth. Composition on triple overlaps gives $\psi_{ki}=\psi_{kj}\psi_{ji}$.

### Frame bundle

↑ **Parent:** [Principal bundle](#principal-bundle)

The frame bundle of an $n$-dimensional [smooth manifold](smooth-manifold.md) has fiber over $x$ consisting of linear [isomorphisms](algebra.md#isomorphism) $u:\mathbb R^n\to T_xM$. Right composition by $GL(n,\mathbb R)$ makes it a [principal bundle](#principal-bundle). A global [frame of a vector bundle](vector-bundle.md#frame-of-a-vector-bundle) is a global [section of a fiber bundle](#section-fiber-bundle) and trivializes the [tangent bundle](vector-bundle.md#tangent-bundle). A metric restricts the allowed frames to the [orthonormal frame bundle](#orthonormal-frame-bundle).

### Orthonormal frame bundle

↑ **Parent:** [Principal bundle](#principal-bundle)

For a metric of signature $(r,s)$, the orthonormal frame bundle consists of all linear isometries $u:\mathbb R^{r,s}\to T_xM$. Right composition by $O(r,s)$ makes it a [principal bundle](#principal-bundle). Its standard [associated vector bundle](#associated-vector-bundle) is the [tangent bundle](vector-bundle.md#tangent-bundle), via $[u,v]\mapsto u(v)$. A global orthonormal frame is a global section and therefore trivializes this principal bundle. A [Lie group](lie-theory.md#lie-group) with a left-invariant metric has such a frame by left translating an orthonormal basis at the identity.

#### Oriented orthonormal frame bundle of anti-de Sitter spacetime

↑ **Parent:** [Orthonormal frame bundle](#orthonormal-frame-bundle)

Represent the [Anti-de Sitter spacetime](general-relativity.md#anti-de-sitter-spacetime) quadric by $x\cdot x=-\ell^2$ in $\mathbb R^{3,2}$. Appending its timelike unit normal $x/\ell$ to an oriented tangent pseudo-orthonormal frame identifies the frame bundle with $SO(3,2)$. The stabilizer of that normal is $SO(3,1)$, so projection realizes $SO(3,2)/SO(3,1)$ as the base of a [principal bundle](#principal-bundle). For the commonly used universal cover of the anti-de Sitter quadric, pull this bundle back along the covering map; the quadric itself has a periodic timelike coordinate.

#### Oriented orthonormal frame bundle of Minkowski spacetime

↑ **Parent:** [Orthonormal frame bundle](#orthonormal-frame-bundle)

An oriented pseudo-orthonormal frame in [Minkowski spacetime](special-relativity.md#minkowski-spacetime) consists of its base point $a$ and a Lorentz matrix $L$ acting on a fixed reference frame. The pairs $(a,L)$ form the [Poincaré group](special-relativity.md#poincare-group), and right multiplication by $(0,h)$ sends the frame to $(a,Lh)$ while fixing its base point. Thus the displayed projection is a [principal bundle](#principal-bundle) with group $SO(3,1)$. The full frame bundle uses $O(3,1)$; a specified time orientation restricts to the corresponding connected component.

#### Oriented frame bundle of de Sitter spacetime

↑ **Parent:** [Orthonormal frame bundle](#orthonormal-frame-bundle)

Represent unit-radius [de Sitter spacetime](general-relativity.md#de-sitter-spacetime) by the spacelike unit [hyperboloid](differential-geometry.md#hyperboloid) in five-dimensional [Minkowski spacetime](special-relativity.md#minkowski-spacetime). Appending its position vector as the last column of an oriented [pseudo-orthonormal frame](vector-bundle.md#pseudo-orthonormal-frame) produces a matrix in $SO(4,1)$. Projection to that last column identifies $SO(4,1)$ with the oriented [orthonormal frame bundle](#orthonormal-frame-bundle), a [principal bundle](#principal-bundle) with group $SO(3,1)$. The full bundle allowing both orientations is $O(4,1)$ with group $O(3,1)$. Requiring a time orientation as well selects the corresponding identity components.

##### Global frame on four-dimensional de Sitter spacetime

↑ **Parent:** [Oriented frame bundle of de Sitter spacetime](#oriented-frame-bundle-of-de-sitter-spacetime)

In global coordinates the [de Sitter spacetime](general-relativity.md#de-sitter-spacetime) metric is $-d\tau^2+\cosh^2\tau\,g_{S^3}$. A global [frame of a vector bundle](vector-bundle.md#frame-of-a-vector-bundle) orthonormal for the round metric $Y_1,Y_2,Y_3$ on $S^3$ gives the displayed global [pseudo-orthonormal frame](vector-bundle.md#pseudo-orthonormal-frame). For example, identify $S^3$ with the [unit quaternions](algebra-over-a-field.md#unit-quaternion) and use $qi,qj,qk$. Choosing the spatial orientation and the future direction consistently gives a [section of a fiber bundle](#section-fiber-bundle) for the oriented, time-oriented frame bundle. The [principal bundle trivialization by a global section](#principal-bundle-trivialization-by-a-global-section) then proves that bundle is trivial.

### Associated bundle

↑ **Parent:** [Principal bundle](#principal-bundle)

For a [principal bundle](#principal-bundle) $P\to B$ and a left action of its structure group on a manifold $F$, the associated bundle is $(P\times F)/\sim$, where $(pg,f)\sim(p,gf)$. Local sections identify it with $U\times F$; principal transition functions act on $F$. Linear actions give [associated vector bundles](#associated-vector-bundle).

### Principal bundle trivialization by a global section

↑ **Parent:** [Principal bundle](#principal-bundle)

A [principal bundle](#principal-bundle) is trivial exactly when it has a global [section of a fiber bundle](#section-fiber-bundle). Given such a section, the displayed map is a smooth equivariant isomorphism: the free transitive action on each fiber gives the unique inverse group coordinate, and local trivializations make it smooth. Conversely, a product trivialization has the section $x\mapsto(x,e)$.

### Associated vector bundle

↑ **Parent:** [Principal bundle](#principal-bundle)

A linear representation $\rho:G\to GL(V)$ of a [principal bundle](#principal-bundle)'s structure group defines the quotient of $P\times V$ by $(p,v)\sim(pg,\rho(g)^{-1}v)$. It is a [vector bundle](vector-bundle.md) over the same base. A [principal connection](#connection-principal-bundle) induces [parallel transport](vector-bundle.md#parallel-transport) and a local [covariant derivative](general-relativity.md#covariant-derivative) $d+\rho_*(A)$ on its sections.

#### Adjoint bundle

↑ **Parent:** [Associated vector bundle](#associated-vector-bundle)

The adjoint bundle is the [associated vector bundle](#associated-vector-bundle) for the [Adjoint representation of a Lie group](lie-theory.md#adjoint-representation-of-a-lie-group) on its [Lie algebra](lie-algebra.md). The [gauge curvature](relativistic-quantum-field.md#gauge-field-strength) of a [principal connection](#connection-principal-bundle) is globally a two-form with values in this bundle. Differences of [principal connections](#connection-principal-bundle) and their infinitesimal variations are one-forms with values in the same bundle.

### Classifying space

↑ **Parent:** [Principal bundle](#principal-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Classifying_space)

For a [topological group](topological-group.md) $G$, a universal [principal bundle](#principal-bundle) $EG\to BG$ has contractible total space and classifies numerable principal $G$-bundles by pullback. Over a paracompact base, isomorphism classes correspond to [homotopy classes](homotopy.md#homotopy-class) of maps to $BG$. For a discrete group, its [classifying space of a discrete group](#classifying-space-of-a-discrete-group) is a $K(G,1)$; for the circle, $BS^1\simeq\mathbb{CP}^\infty$.

#### Rational odd-rank stabilization of orthogonal classifying spaces

↑ **Parent:** [Classifying space](#classifying-space)

The stabilizer of a line in $O(n)$ is $O(1)\times O(n-1)$, giving the [homogeneous space](lie-theory.md#homogeneous-space) $\mathbb{RP}^{n-1}$. Its classifying-space [Serre fibration](homotopy.md#serre-fibration) has rationally acyclic fiber for odd $n$, so its cohomological [Serre spectral sequence](homotopy.md#serre-spectral-sequence) has only its degree-zero row and gives the displayed restriction isomorphism. The factor $BO(1)=\mathbb{RP}^\infty$ is itself rationally acyclic. For even $n$, the fiber has a top rational class, with determinant-sign monodromy, so the one-row argument fails. The top universal [Pontryagin class](geometry-and-topology.md#pontryagin-class) $p_{n/2}$ is nonzero on $BO(n)$ but vanishes on restriction to $BO(n-1)$, witnessing genuine failure of stabilization.

#### Classifying space of a discrete group

↑ **Parent:** [Classifying space](#classifying-space)

Give a discrete group $G$ a contractible free [CW complex](algebraic-topology.md#cw-complex) $EG$. The quotient $BG=EG/G$ has [universal cover](algebraic-topology.md#universal-cover) $EG$, so it has [fundamental group](algebraic-topology.md#fundamental-group) $G$ and no higher [homotopy groups](homotopy.md#homotopy-group). It is thus an [Eilenberg–MacLane space](homotopy.md#eilenberg-maclane-space) $K(G,1)$, even when $G$ is nonabelian. The cohomology of $BG$ with the appropriate local coefficients computes [group cohomology](group-cohomology.md).

### General linear group modulo the unitary group

↑ **Parent:** [Principal bundle](#principal-bundle)

Let $H(n)$ be the real [vector space](vector-space.md) of [Hermitian matrices](hilbert-space.md#hermitian-operator). The [polar decomposition of an invertible complex matrix](quadratic-form.md#polar-decomposition-of-an-invertible-complex-matrix) gives a diffeomorphism

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

If a [Lie group](lie-theory.md#lie-group) acts smoothly, freely, and properly on a [smooth manifold](smooth-manifold.md) $P$, then the quotient $P/G$ has a unique smooth structure for which $P\to P/G$ is a [principal bundle](#principal-bundle). An action by a compact Lie group is automatically proper.

### Connection (principal bundle)

↑ **Parent:** [Principal bundle](#principal-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Connection_(principal_bundle))

A principal connection can be specified by a $G$-equivariant horizontal distribution $H\subset TP$ complementary to the vertical bundle, or equivalently by a Lie-algebra-valued connection form $\mathcal A$ that reproduces infinitesimal generators and has $H=\ker\mathcal A$.

#### Translational connection for a convex body rolling on a plane

↑ **Parent:** [Connection (principal bundle)](#connection-principal-bundle)

For a smooth strictly convex [rigid body](rigid-body-dynamics.md) with a smooth unique contact point, a configuration consists of its orientation $R\in SO(3)$ and horizontal position $c_{\parallel}\in\mathbb R^2$; its height is fixed by contact. Translation makes this a [principal bundle](#principal-bundle) over $SO(3)$ with group $\mathbb R^2$. If $r(R)$ points from its reference point to contact and $\Omega$ is its spatial [angular velocity](rigid-body-dynamics.md#angular-velocity), [rolling without slipping](rigid-body-dynamics.md#rolling-without-slipping) requires $\dot c+\Omega\times r=0$. The displayed translation-valued [principal connection](#connection-principal-bundle) vanishes on precisely these velocities. It is translation-invariant and equals the identity on vertical translation vectors. A prescribed orientation curve consequently has a unique horizontal lift from a given initial position. No-slip alone leaves spin free and does not specify a connection over the plane with orientation as its fiber; an additional no-twist constraint is needed for that familiar spherical model.

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

In the round [real projective plane](differential-geometry.md#real-projective-plane), project the great-circle arc $(\cos t,\sin t,0)$ for $0\le t\le\pi$. Its endpoint and velocity match after antipodal identification, so it is a closed [geodesic](riemannian-geometry.md#geodesic). On the sphere its tangent and the constant vector $(0,0,1)$ are parallel. Endpoint identification fixes the returned tangent and reverses the returned transverse vector. Its [parallel transport](vector-bundle.md#parallel-transport) is therefore a reflection. Nonorientability permits determinant-minus-one holonomy.

###### Holonomy around circular fibres

↑ **Parent:** [Holonomy](#holonomy)

For the [Riemannian metric](riemannian-metric.md) $dr^2+f(r)^2d\phi^2$, where $f>0$ and $\phi$ has period $2\pi$, [parallel transport](vector-bundle.md#parallel-transport) around $r=r_0$ acts on the [orthonormal basis](inner-product.md#orthonormal-basis) components of a [tangent vector](tangent-vector.md) by a rotation through $-2\pi f'(r_0)$. Indeed, those components obey $u'=f'(r_0)v$ and $v'=-f'(r_0)u$ as functions of $\phi$. Thus all [tangent vectors](tangent-vector.md) return to themselves exactly when $f'(r_0)\in\mathbb Z$. The integer criterion concerns [holonomy](#holonomy) and is stronger than local flatness.

###### Flat circular metrics with trivial holonomy

↑ **Parent:** [Holonomy around circular fibres](#holonomy-around-circular-fibres)

On a connected regular radial interval, trivial [holonomy around circular fibres](#holonomy-around-circular-fibres) forces the continuous function $f'$ to be integer-valued, hence constant. The resulting [Riemannian metrics](riemannian-metric.md) have $f(r)=nr+b$, with $n\in\mathbb Z$ and $f>0$ on the interval. Their [Gaussian curvature](second-fundamental-form.md#gaussian-curvature) is $-f''/f=0$. For $n\ne0$, $\rho=f/|n|$ and $\theta=|n|\phi$ give a [local isometry](differential-geometry.md#local-isometry) to the [Euclidean plane](geometry-and-topology.md#euclidean-plane); for $n=0$, $r,b\phi$ give a flat cylindrical chart. The polar [developing map](differential-geometry.md#developing-map) is injective on the regular domain when $|n|=1$, and is a multiple covering when $|n|>1$. Trivial [holonomy](#holonomy) therefore does not imply a global Euclidean chart. The slope is a discrete parameter, not an unrestricted real one.

###### Riemannian holonomy group

↑ **Parent:** [Holonomy](#holonomy)

For a connected [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), the full holonomy group consists of [parallel transport](vector-bundle.md#parallel-transport) maps around all piecewise smooth loops based at $p$. Metric compatibility makes them orthogonal. Basepoint changes conjugate this group by parallel transport. This is full holonomy, not just the subgroup using contractible loops.

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

[This section is present in another page, follow this link to view it.](vector-bundle.md)

## Curvature form

↑ **Parent:** [Fiber bundle](fiber-bundle.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Curvature_form)

The [curvature form](#curvature-form) of a [connection on a vector bundle](vector-bundle.md#connection-vector-bundle) is $F=dA+A\wedge A$ in a local frame. A [principal connection](#connection-principal-bundle) has the corresponding [Lie algebra](lie-algebra.md)-valued form $F=dA+\tfrac12[A\wedge A]$. It measures the failure of horizontal directions to be integrable.

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

The [trace](linear-algebra.md#matrix-trace) of the [curvature form of a connection](#curvature-form) is a global [closed differential form](differential-form.md#closed-differential-form) of degree two. Under a frame change $e'=eg$, the [connection matrix](vector-bundle.md#connection-one-form) and curvature change by $A'=g^{-1}Ag+g^{-1}dg$ and $\Theta'=g^{-1}\Theta g$. Thus [trace](linear-algebra.md#matrix-trace) is independent of frame. The [Bianchi identity](#bianchi-identity) gives $d\Theta=\Theta\wedge A-A\wedge\Theta$. Taking the [trace](linear-algebra.md#matrix-trace) cancels the two terms: one-forms commute with two-forms in the graded sense, and renaming the [matrix](vector-space.md#matrix) indices gives equality of their [traces](linear-algebra.md#matrix-trace). Locally $\operatorname{tr}\Theta=d\operatorname{tr}A$, since the [trace](linear-algebra.md#matrix-trace) of $A\wedge A$ vanishes by pairing its off-diagonal terms. It is the curvature of the [determinant connection](vector-bundle.md#determinant-connection).

### Cartan curvature matrix equation

↑ **Parent:** [Curvature form](#curvature-form)

For a [connection on a vector bundle](vector-bundle.md#connection-vector-bundle) written $D=d+A\wedge$ in a local frame, its [curvature form of a connection](#curvature-form) is represented by $\Theta=dA+A\wedge A$. The products combine matrix multiplication with the [exterior product](multilinear-algebra.md#exterior-product). The formula follows by squaring $D$ and using the graded [Leibniz rule](calculus.md#leibniz-rule).

#### Cartan curvature equation with input indices

↑ **Parent:** [Cartan curvature matrix equation](#cartan-curvature-matrix-equation)

Write $De_i=\sum_j\theta_{ij}\otimes e_j$, with the differentiated input index first. The graded [Leibniz rule](calculus.md#leibniz-rule) gives $D^2e_i=\sum_j(d\theta_{ij}-\sum_k\theta_{ik}\wedge\theta_{kj})\otimes e_j$. For frames $e'=ge$, the [connection matrix](vector-bundle.md#connection-one-form) transforms as $\theta'=dg\,g^{-1}+g\theta g^{-1}$ and curvature by $\Theta'=g\Theta g^{-1}$. Transposing to the usual coefficient-column convention gives $A=\theta^t$ and $F=dA+A\wedge A=\Theta^t$; the opposite sign is an index convention, not a different curvature.

### Riemannian curvature two-form

↑ **Parent:** [Curvature form](#curvature-form)

For the [Levi-Civita connection](general-relativity.md#levi-civita-connection), the [curvature form of a connection](#curvature-form) is the endomorphism-valued two-form

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z.
$$

It has [tensoriality](vector-bundle.md#tensoriality) in all three arguments. Its [first Bianchi identity](riemann-curvature-tensor.md#first-bianchi-identity) follows from torsion-freeness: the cyclic sum is $\sum_{\mathrm{cyc}}(\nabla_X[Y,Z]-\nabla_{[Y,Z]}X)=\sum_{\mathrm{cyc}}[X,[Y,Z]]=0$ by the [Jacobi identity](lie-algebra.md#jacobi-identity).

### Curvature difference formula

↑ **Parent:** [Curvature form](#curvature-form)

If two objects $\nabla_1$ and $\nabla_2$ are each a [connection on a vector bundle](vector-bundle.md#connection-vector-bundle) and satisfy $\nabla_1=\nabla_2+a$ for an $\operatorname{End}(E)$-valued one-form $a$, then

$$
F_{\nabla_1}=F_{\nabla_2}+d_{\nabla_2}a+a\wedge a.
$$

This follows by expanding $(\nabla_2+a)^2$ with the [covariant exterior derivative](vector-bundle.md#exterior-covariant-derivative) on the [endomorphism bundle connection](vector-bundle.md#endomorphism-bundle-connection).

#### Trace curvature transgression

↑ **Parent:** [Curvature difference formula](#curvature-difference-formula)

The difference of two [connections on a vector bundle](vector-bundle.md#connection-vector-bundle) is a global endomorphism-valued one-form. Taking the [trace](linear-algebra.md#matrix-trace) of the [curvature difference formula](#curvature-difference-formula) cancels both the commutator terms and the trace of the square of that one-form. Consequently the trace curvatures represent the same [de Rham cohomology](differential-form.md#de-rham-cohomology) class.

##### Connection-independent curvature class of a line bundle

↑ **Parent:** [Trace curvature transgression](#trace-curvature-transgression)

For a real or complex [line bundle](sheaf-of-modules.md#line-bundle), its [endomorphism bundle](vector-bundle.md#endomorphism-bundle) is canonically trivial by scalar multiplication. The [Bianchi identity](#bianchi-identity) therefore reduces to $dF_A=0$. The difference of two [connections on a vector bundle](vector-bundle.md#connection-vector-bundle) is a global endomorphism-valued one-form, which here is an ordinary scalar one-form $a$. Since scalar one-forms have vanishing wedge square, the [curvature difference formula](#curvature-difference-formula) reduces to $F_{A+a}-F_A=da$. Thus the [de Rham cohomology](differential-form.md#de-rham-cohomology) class is independent of the [connection on a vector bundle](vector-bundle.md#connection-vector-bundle).

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

- [A sphere cannot fibre over a lower-dimensional odd sphere](homotopy.md#a-sphere-cannot-fibre-over-a-lower-dimensional-odd-sphere)
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
