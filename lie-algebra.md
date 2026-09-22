# Lie algebra

↑ **Parent:** [Lie theory](lie-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lie_algebra)

A Lie algebra over a [field](algebra.md#field) is a [vector space](vector-space.md) $\mathfrak g$ with a bilinear operation $[x,y]$, called the [Lie bracket](#lie-bracket), that is alternating and satisfies the [Jacobi identity](#jacobi-identity).

**Table of contents**

- [Cartan's criterion](#cartan-s-criterion)
- [Loop algebra](#loop-algebra)
- [Affine current algebra](#affine-current-algebra)
- [Free Lie algebra](#free-lie-algebra)
  - [Lie polynomial](#lie-polynomial)
- [Semidirect product of Lie algebras](#semidirect-product-of-lie-algebras)
- [Lie algebra cohomology](#lie-algebra-cohomology)
  - [Lie algebra two-cocycle](#lie-algebra-two-cocycle)
- [Compact Lie algebra](#compact-lie-algebra)
- [Powerful Lie algebra over p-adic integers](#powerful-lie-algebra-over-p-adic-integers)
  - [Lie algebra of a uniform pro-p group](#lie-algebra-of-a-uniform-pro-p-group)
  - [BCH convergence on a powerful Lie lattice](#bch-convergence-on-a-powerful-lie-lattice)
- [Cross-product Lie algebra](#cross-product-lie-algebra)
- [Euclidean motion Lie algebra in two dimensions](#euclidean-motion-lie-algebra-in-two-dimensions)
  - [Killing form of the planar Euclidean motion Lie algebra](#killing-form-of-the-planar-euclidean-motion-lie-algebra)
- [Graded Lie algebra](#graded-lie-algebra)
  - [Chevalley–Eilenberg cochains of a graded Lie algebra](#chevalley-eilenberg-cochains-of-a-graded-lie-algebra)
  - [Free graded Lie algebra](#free-graded-lie-algebra)
  - [Graded Lie bracket](#graded-lie-bracket)
- [Central extension of a Lie algebra](#central-extension-of-a-lie-algebra)
- [Witt algebra](#witt-algebra)
- [Centralizer of an element of a Lie algebra](#centralizer-of-an-element-of-a-lie-algebra)
  - [Centralizer lower bound for a root vector](#centralizer-lower-bound-for-a-root-vector)
- [Lie algebra generator](#lie-algebra-generator)
- [Lie algebra of a matrix Lie group](#lie-algebra-of-a-matrix-lie-group)
  - [Matrix commutator from a logarithm chart](#matrix-commutator-from-a-logarithm-chart)
  - [General linear Lie algebra](#general-linear-lie-algebra)
  - [Unitary Lie algebra](#unitary-lie-algebra)
    - [Special unitary Lie algebra](#special-unitary-lie-algebra)
      - [Trace normalization of su(2)](#trace-normalization-of-su-2)
    - [SU(3) Lie algebra](#su-3-lie-algebra)
      - [Root SU(2) subalgebras of SU(3)](#root-su-2-subalgebras-of-su-3)
    - [Matrix-unit basis of the unitary Lie algebra](#matrix-unit-basis-of-the-unitary-lie-algebra)
- [Lie algebra isomorphism](#lie-algebra-isomorphism)
- [Direct sum of Lie algebras](#direct-sum-of-lie-algebras)
- [Lie subalgebra](#lie-subalgebra)
  - [Normalizer of a Lie subalgebra](#normalizer-of-a-lie-subalgebra)
- [Derivation of a Lie algebra](#derivation-of-a-lie-algebra)
  - [Exponential of a nilpotent Lie algebra derivation](#exponential-of-a-nilpotent-lie-algebra-derivation)
  - [Inner derivation of a Lie algebra](#inner-derivation-of-a-lie-algebra)
  - [Derivation Lie algebra](#derivation-lie-algebra)
  - [Outer derivation of a nilpotent Lie algebra](#outer-derivation-of-a-nilpotent-lie-algebra)
  - [Generalized-eigenspace bracket lemma](#generalized-eigenspace-bracket-lemma)
- [Invariant bilinear form on a Lie algebra](#invariant-bilinear-form-on-a-lie-algebra)
  - [Invariance of a bilinear form on a Lie algebra](#invariance-of-a-bilinear-form-on-a-lie-algebra)
  - [Positive invariant metric on a Lie algebra](#positive-invariant-metric-on-a-lie-algebra)
- [Lie superalgebra](#lie-superalgebra)
  - [Lie superalgebra representation](#lie-superalgebra-representation)
  - [Graded Jacobi identity](#graded-jacobi-identity)
- [Lie bracket](#lie-bracket)
  - [Antisymmetry of a Lie bracket](#antisymmetry-of-a-lie-bracket)
  - [Lie bracket from local group commutators](#lie-bracket-from-local-group-commutators)
  - [Commutator](#commutator)
    - [Identity commutator cyclic ladder](#identity-commutator-cyclic-ladder)
    - [Commutator expansion for exponential conjugation](#commutator-expansion-for-exponential-conjugation)
      - [Central-commutator exponential identity](#central-commutator-exponential-identity)
    - [Trace of a matrix commutator](#trace-of-a-matrix-commutator)
    - [Commutator derivation identity](#commutator-derivation-identity)
  - [Jacobi identity](#jacobi-identity)
- [Abelian Lie algebra](#abelian-lie-algebra)
- [Semidirect product of a Lie algebra and a module](#semidirect-product-of-a-lie-algebra-and-a-module)
  - [Killing form of a semidirect product with a module](#killing-form-of-a-semidirect-product-with-a-module)
- [Ideal of a Lie algebra](#ideal-of-a-lie-algebra)
  - [Quotient Lie algebra](#quotient-lie-algebra)
- [Derived series of a Lie algebra](#derived-series-of-a-lie-algebra)
  - [Derived algebra](#derived-algebra)
    - [Derived algebra nilpotence criterion](#derived-algebra-nilpotence-criterion)
  - [Solvable Lie algebra](#solvable-lie-algebra)
    - [Diamond Lie algebra](#diamond-lie-algebra)
    - [Affine Lie algebra of the line](#affine-lie-algebra-of-the-line)
    - [Radical of a Lie algebra](#radical-of-a-lie-algebra)
    - [Lie's theorem](#lie-s-theorem)
      - [Infinite-dimensional simple module for the two-dimensional affine Lie algebra](#infinite-dimensional-simple-module-for-the-two-dimensional-affine-lie-algebra)
      - [Simultaneous triangularization of a Lie algebra representation](#simultaneous-triangularization-of-a-lie-algebra-representation)
      - [Failure of Lie theorem in positive characteristic](#failure-of-lie-theorem-in-positive-characteristic)
    - [Cartan solvability criterion](#cartan-solvability-criterion)
      - [Conjugate-spectrum proof of Cartan solvability](#conjugate-spectrum-proof-of-cartan-solvability)
- [Center of a Lie algebra](#center-of-a-lie-algebra)
  - [Central ideal](#central-ideal)
- [Lower central series of a Lie algebra](#lower-central-series-of-a-lie-algebra)
  - [Nilpotent Lie algebra](#nilpotent-lie-algebra)
    - [Killing form of a nilpotent Lie algebra vanishes](#killing-form-of-a-nilpotent-lie-algebra-vanishes)
    - [Upper central series of a Lie algebra](#upper-central-series-of-a-lie-algebra)
    - [Two-dimensional subalgebra criterion for Lie algebra nilpotence](#two-dimensional-subalgebra-criterion-for-lie-algebra-nilpotence)
    - [Normalizer condition for a nilpotent Lie algebra](#normalizer-condition-for-a-nilpotent-lie-algebra)
    - [Engel's theorem](#engel-s-theorem)
      - [Proof of Engel theorem by induction and normalizers](#proof-of-engel-theorem-by-induction-and-normalizers)
      - [Engel lemma](#engel-lemma)
        - [Engel normalizer lemma](#engel-normalizer-lemma)
- [Lie algebra homomorphism](#lie-algebra-homomorphism)
  - [Integration of a Lie algebra homomorphism](#integration-of-a-lie-algebra-homomorphism)
    - [Period obstruction to integration of a Lie algebra homomorphism](#period-obstruction-to-integration-of-a-lie-algebra-homomorphism)
  - [Differential of a Lie group homomorphism preserves Lie brackets](#differential-of-a-lie-group-homomorphism-preserves-lie-brackets)
  - [Lie algebra representation](#lie-algebra-representation)
    - [Representation ring of a semisimple Lie algebra](#representation-ring-of-a-semisimple-lie-algebra)
    - [Defining representation of a matrix Lie algebra](#defining-representation-of-a-matrix-lie-algebra)
    - [Hermitian quantum generator convention](#hermitian-quantum-generator-convention)
    - [Lie algebra representation homomorphism](#lie-algebra-representation-homomorphism)
    - [Exterior-power Lie algebra representation](#exterior-power-lie-algebra-representation)
    - [Nilpotent Lie algebras need not act nilpotently](#nilpotent-lie-algebras-need-not-act-nilpotently)
    - [Tensor product of Lie algebra representations](#tensor-product-of-lie-algebra-representations)
      - [SU(3) triplet-octet decomposition](#su-3-triplet-octet-decomposition)
      - [sl2 tensor product of cubic and quadratic symmetric powers](#sl2-tensor-product-of-cubic-and-quadratic-symmetric-powers)
      - [Action map of a Lie algebra representation](#action-map-of-a-lie-algebra-representation)
        - [Action summand can fail for an infinite-dimensional simple module](#action-summand-can-fail-for-an-infinite-dimensional-simple-module)
      - [Tensor product of the standard representation with its exterior square](#tensor-product-of-the-standard-representation-with-its-exterior-square)
      - [sl3 highest-weight tensor rule](#sl3-highest-weight-tensor-rule)
    - [Integration of a Lie-algebra representation](#integration-of-a-lie-algebra-representation)
    - [Lie-invariant bilinear form](#lie-invariant-bilinear-form)
    - [Dual Lie algebra representation](#dual-lie-algebra-representation)
      - [Highest weight of a dual representation](#highest-weight-of-a-dual-representation)
    - [Trivial Lie algebra representation](#trivial-lie-algebra-representation)
    - [Hom representation](#hom-representation)
    - [Automorphism of a Lie algebra](#automorphism-of-a-lie-algebra)
    - [Branching rule](#branching-rule)
      - [Adjoint branching to root sl2 subalgebras in rank two](#adjoint-branching-to-root-sl2-subalgebras-in-rank-two)
    - [Structure constant of a Lie algebra](#structure-constant-of-a-lie-algebra)
      - [Three-dimensional Lie algebra structure decomposition](#three-dimensional-lie-algebra-structure-decomposition)
      - [Antisymmetry of Killing-lowered structure constants](#antisymmetry-of-killing-lowered-structure-constants)
    - [Faithful Lie algebra representation](#faithful-lie-algebra-representation)
      - [Ado's theorem](#ado-s-theorem)
    - [Irreducible Lie algebra representation](#irreducible-lie-algebra-representation)
    - [Adjoint representation of a Lie algebra](#adjoint-representation-of-a-lie-algebra)
      - [Adjoint representation of SU(3)](#adjoint-representation-of-su-3)
        - [Tensor square of the SU(3) adjoint representation](#tensor-square-of-the-su-3-adjoint-representation)
      - [Killing form](#killing-form)
        - [Killing form of the general linear Lie algebra](#killing-form-of-the-general-linear-lie-algebra)
        - [Killing-form invariance under a Lie-group adjoint action](#killing-form-invariance-under-a-lie-group-adjoint-action)
        - [Killing form for cyclic three-generator brackets](#killing-form-for-cyclic-three-generator-brackets)
        - [Orthogonal ideal splitting for a nondegenerate Killing form](#orthogonal-ideal-splitting-for-a-nondegenerate-killing-form)
        - [Radical of the Killing form](#radical-of-the-killing-form)
        - [Compactness criterion from the Killing form](#compactness-criterion-from-the-killing-form)
        - [Abelian ideals lie in the radical of the Killing form](#abelian-ideals-lie-in-the-radical-of-the-killing-form)
        - [Solvability of the radical of the Killing form](#solvability-of-the-radical-of-the-killing-form)
        - [Cartan criterion for semisimplicity](#cartan-criterion-for-semisimplicity)
          - [Killing radical is a solvable ideal](#killing-radical-is-a-solvable-ideal)
        - [Uniqueness of an invariant bilinear form on a simple Lie algebra](#uniqueness-of-an-invariant-bilinear-form-on-a-simple-lie-algebra)
          - [Real-simple exception to uniqueness of the Killing form](#real-simple-exception-to-uniqueness-of-the-killing-form)
        - [Killing form of the special linear Lie algebra](#killing-form-of-the-special-linear-lie-algebra)
      - [Adjoint irreducibility of a simple Lie algebra](#adjoint-irreducibility-of-a-simple-lie-algebra)
    - [Trace form of a Lie algebra representation](#trace-form-of-a-lie-algebra-representation)
      - [Trace forms of solvable Lie algebras annihilate the derived algebra](#trace-forms-of-solvable-lie-algebras-annihilate-the-derived-algebra)
      - [Cubic trace tensor of a Lie algebra representation](#cubic-trace-tensor-of-a-lie-algebra-representation)
        - [Killing-normalized contraction of a cubic trace tensor](#killing-normalized-contraction-of-a-cubic-trace-tensor)
        - [Invariance identity for a cubic trace tensor](#invariance-identity-for-a-cubic-trace-tensor)
      - [Positive trace index for a compact simple Lie algebra](#positive-trace-index-for-a-compact-simple-lie-algebra)
    - [Trace trilinear form of a Lie algebra representation](#trace-trilinear-form-of-a-lie-algebra-representation)
- [Heisenberg Lie algebra](#heisenberg-lie-algebra)
  - [Heisenberg group](#heisenberg-group)
    - [Center quotient of the real Heisenberg group](#center-quotient-of-the-real-heisenberg-group)
    - [Right-invariant coframe of the real Heisenberg group](#right-invariant-coframe-of-the-real-heisenberg-group)
      - [Killing frame for a right-invariant Heisenberg metric](#killing-frame-for-a-right-invariant-heisenberg-metric)
    - [Modular Heisenberg group](#modular-heisenberg-group)
    - [Left-invariant frame of the real Heisenberg group](#left-invariant-frame-of-the-real-heisenberg-group)
      - [Heisenberg horizontal distribution](#heisenberg-horizontal-distribution)
        - [Smooth horizontal reachability in the real Heisenberg group](#smooth-horizontal-reachability-in-the-real-heisenberg-group)
    - [Integer Heisenberg group](#integer-heisenberg-group)
      - [Scaled Heisenberg lattice](#scaled-heisenberg-lattice)
      - [Commutator identity in the integer Heisenberg group](#commutator-identity-in-the-integer-heisenberg-group)
    - [Schrödinger representation of the Heisenberg group](#schrodinger-representation-of-the-heisenberg-group)
  - [Polynomial representation of the Heisenberg Lie algebra](#polynomial-representation-of-the-heisenberg-lie-algebra)
- [Complexification of a Lie algebra](#complexification-of-a-lie-algebra)
  - [Complexification preserves semisimplicity](#complexification-preserves-semisimplicity)
- [Universal enveloping algebra](#universal-enveloping-algebra)
  - [Poincaré-Birkhoff-Witt theorem](#poincare-birkhoff-witt-theorem)
    - [Graded Poincaré–Birkhoff–Witt theorem](#graded-poincare-birkhoff-witt-theorem)
- [Semisimple Lie algebra](semisimple-lie-algebra.md)
  - [Chevalley basis](semisimple-lie-algebra.md#chevalley-basis)
    - [Serre relations](semisimple-lie-algebra.md#serre-relations)
      - [SU(2) proof of the Serre relations](semisimple-lie-algebra.md#su-2-proof-of-the-serre-relations)
    - [Simply laced Chevalley commutator formula](semisimple-lie-algebra.md#simply-laced-chevalley-commutator-formula)
  - [Jordan decomposition in an abstract semisimple Lie algebra](semisimple-lie-algebra.md#jordan-decomposition-in-an-abstract-semisimple-lie-algebra)
  - [Split semisimple Lie algebra](semisimple-lie-algebra.md#split-semisimple-lie-algebra)
  - [Compact real form of a complex semisimple Lie algebra](semisimple-lie-algebra.md#compact-real-form-of-a-complex-semisimple-lie-algebra)
  - [Perfect Lie algebra](semisimple-lie-algebra.md#perfect-lie-algebra)
  - [Weyl complete reducibility theorem](semisimple-lie-algebra.md#weyl-complete-reducibility-theorem)
    - [Haar averaging produces invariant complements](semisimple-lie-algebra.md#haar-averaging-produces-invariant-complements)
    - [Invariant complement from an equivariant projection](semisimple-lie-algebra.md#invariant-complement-from-an-equivariant-projection)
    - [Casimir splitting of a trivial quotient](semisimple-lie-algebra.md#casimir-splitting-of-a-trivial-quotient)
  - [Borel subalgebra](semisimple-lie-algebra.md#borel-subalgebra)
  - [Simple Lie algebra](semisimple-lie-algebra.md#simple-lie-algebra)
    - [Special linear Lie algebra](semisimple-lie-algebra.md#special-linear-lie-algebra)
      - [sl2 triple](semisimple-lie-algebra.md#sl2-triple)
        - [Finite sl2 lowest-weight ladder](semisimple-lie-algebra.md#finite-sl2-lowest-weight-ladder)
      - [Symmetric powers of the defining sln representation](semisimple-lie-algebra.md#symmetric-powers-of-the-defining-sln-representation)
        - [Contraction splitting of a defining module tensor a dual symmetric square](semisimple-lie-algebra.md#contraction-splitting-of-a-defining-module-tensor-a-dual-symmetric-square)
        - [sl3 decomposition of the symmetric-square dual tensor product](semisimple-lie-algebra.md#sl3-decomposition-of-the-symmetric-square-dual-tensor-product)
          - [Weight basis of the trace-free symmetric-square dual tensor module](semisimple-lie-algebra.md#weight-basis-of-the-trace-free-symmetric-square-dual-tensor-module)
          - [Exterior square of the sl3 representation of highest weight (2,1)](semisimple-lie-algebra.md#exterior-square-of-the-sl3-representation-of-highest-weight-2-1)
      - [Symmetric square of the sl3 representation of highest weight (2,1)](semisimple-lie-algebra.md#symmetric-square-of-the-sl3-representation-of-highest-weight-2-1)
      - [Matrix-unit extraction lemma for special linear ideals](semisimple-lie-algebra.md#matrix-unit-extraction-lemma-for-special-linear-ideals)
      - [Fundamental representations of sl3](semisimple-lie-algebra.md#fundamental-representations-of-sl3)
        - [Two conjugate SU(3) triplets with a triplet](semisimple-lie-algebra.md#two-conjugate-su-3-triplets-with-a-triplet)
        - [Tensor cube of the defining SU(3) representation](semisimple-lie-algebra.md#tensor-cube-of-the-defining-su-3-representation)
        - [Fundamental weights of sl3](semisimple-lie-algebra.md#fundamental-weights-of-sl3)
        - [Triple tensor decomposition for the defining sl3 representation](semisimple-lie-algebra.md#triple-tensor-decomposition-for-the-defining-sl3-representation)
      - [sl2 Lie algebra](semisimple-lie-algebra.md#sl2-lie-algebra)
        - [Weyl reflection lift in an sl2 representation](semisimple-lie-algebra.md#weyl-reflection-lift-in-an-sl2-representation)
        - [Explicit weight basis of the exterior square of Sym4 for sl2](semisimple-lie-algebra.md#explicit-weight-basis-of-the-exterior-square-of-sym4-for-sl2)
        - [sl2R Lie algebra](semisimple-lie-algebra.md#sl2r-lie-algebra)
        - [SU(2) Lie algebra](semisimple-lie-algebra.md#su-2-lie-algebra)
          - [Killing form of the SU(2) Lie algebra](semisimple-lie-algebra.md#killing-form-of-the-su-2-lie-algebra)
            - [Killing-normalized SU(2) quadratic Casimir](semisimple-lie-algebra.md#killing-normalized-su-2-quadratic-casimir)
        - [Classification of finite-dimensional sl2 representations](semisimple-lie-algebra.md#classification-of-finite-dimensional-sl2-representations)
          - [Clebsch-Gordan splitting of a defining module and its cubic symmetric power](semisimple-lie-algebra.md#clebsch-gordan-splitting-of-a-defining-module-and-its-cubic-symmetric-power)
          - [Parity unimodality of an sl2 character](semisimple-lie-algebra.md#parity-unimodality-of-an-sl2-character)
          - [sl2 highest-weight lowering formula](semisimple-lie-algebra.md#sl2-highest-weight-lowering-formula)
            - [Trace of a raising-lowering product in an irreducible sl2 module](semisimple-lie-algebra.md#trace-of-a-raising-lowering-product-in-an-irreducible-sl2-module)
          - [Invariant form on an irreducible sl2 module](semisimple-lie-algebra.md#invariant-form-on-an-irreducible-sl2-module)
          - [Injectivity of sl2 lowering above weight zero](semisimple-lie-algebra.md#injectivity-of-sl2-lowering-above-weight-zero)
        - [Reducibility of an sl2 Verma module](semisimple-lie-algebra.md#reducibility-of-an-sl2-verma-module)
          - [Nonsplit zero-weight Verma extension for sl2](semisimple-lie-algebra.md#nonsplit-zero-weight-verma-extension-for-sl2)
        - [Intermediate-series sl2 module](semisimple-lie-algebra.md#intermediate-series-sl2-module)
    - [Symplectic Lie algebra](semisimple-lie-algebra.md#symplectic-lie-algebra)
      - [Matrix root basis of the symplectic Lie algebra](semisimple-lie-algebra.md#matrix-root-basis-of-the-symplectic-lie-algebra)
      - [Tensor-square decomposition of the defining symplectic representation](semisimple-lie-algebra.md#tensor-square-decomposition-of-the-defining-symplectic-representation)
      - [Compact symplectic Lie algebra](semisimple-lie-algebra.md#compact-symplectic-lie-algebra)
        - [Matrix-unit basis of the compact symplectic Lie algebra](semisimple-lie-algebra.md#matrix-unit-basis-of-the-compact-symplectic-lie-algebra)
      - [Symplectic root sl2 triple](semisimple-lie-algebra.md#symplectic-root-sl2-triple)
      - [Exceptional isomorphism between sp4 and so5](semisimple-lie-algebra.md#exceptional-isomorphism-between-sp4-and-so5)
      - [Tensor-square decomposition of the defining sp4 representation](semisimple-lie-algebra.md#tensor-square-decomposition-of-the-defining-sp4-representation)
      - [Cn root system](semisimple-lie-algebra.md#cn-root-system)
        - [Cn Dynkin diagrams](semisimple-lie-algebra.md#cn-dynkin-diagrams)
        - [Positive-root data for Cn](semisimple-lie-algebra.md#positive-root-data-for-cn)
        - [Cn Weyl group](semisimple-lie-algebra.md#cn-weyl-group)
        - [C2 root system](semisimple-lie-algebra.md#c2-root-system)
        - [C3 root system](semisimple-lie-algebra.md#c3-root-system)
          - [Rank-two subsystems of a C3 root system](semisimple-lie-algebra.md#rank-two-subsystems-of-a-c3-root-system)
          - [Weyl chamber geometry of C3](semisimple-lie-algebra.md#weyl-chamber-geometry-of-c3)
          - [Cartan matrix convention for C3](semisimple-lie-algebra.md#cartan-matrix-convention-for-c3)
    - [Special orthogonal Lie algebra](semisimple-lie-algebra.md#special-orthogonal-lie-algebra)
      - [Exterior square realization of the orthogonal adjoint representation](semisimple-lie-algebra.md#exterior-square-realization-of-the-orthogonal-adjoint-representation)
      - [Exterior square of the defining orthogonal representation](semisimple-lie-algebra.md#exterior-square-of-the-defining-orthogonal-representation)
      - [Dn root system](semisimple-lie-algebra.md#dn-root-system)
        - [Weyl group of Dn](semisimple-lie-algebra.md#weyl-group-of-dn)
        - [Fundamental weights of Dn](semisimple-lie-algebra.md#fundamental-weights-of-dn)
        - [Matrix root basis of the even orthogonal Lie algebra](semisimple-lie-algebra.md#matrix-root-basis-of-the-even-orthogonal-lie-algebra)
      - [Real four-dimensional rotation algebra splitting](semisimple-lie-algebra.md#real-four-dimensional-rotation-algebra-splitting)
      - [SO(3) Lie algebra](semisimple-lie-algebra.md#so-3-lie-algebra)
      - [Bn root system](semisimple-lie-algebra.md#bn-root-system)
        - [Bn Dynkin diagram and affine extension](semisimple-lie-algebra.md#bn-dynkin-diagram-and-affine-extension)
        - [B3 root system](semisimple-lie-algebra.md#b3-root-system)
      - [so4 Lie algebra](semisimple-lie-algebra.md#so4-lie-algebra)
        - [Chiral decomposition of the complexified so4 Lie algebra](semisimple-lie-algebra.md#chiral-decomposition-of-the-complexified-so4-lie-algebra)
      - [Spin group](semisimple-lie-algebra.md#spin-group)
        - [Exterior-square double cover of SO0(3,2)](semisimple-lie-algebra.md#exterior-square-double-cover-of-so0-3-2)
        - [Hermitian-matrix double cover of SO0(3,1)](semisimple-lie-algebra.md#hermitian-matrix-double-cover-of-so0-3-1)
        - [Symmetric-matrix double cover of SO0(2,1)](semisimple-lie-algebra.md#symmetric-matrix-double-cover-of-so0-2-1)
        - [Exterior-square double cover of SO(3,3)](semisimple-lie-algebra.md#exterior-square-double-cover-of-so-3-3)
        - [Spin(4) double cover](semisimple-lie-algebra.md#spin-4-double-cover)
        - [Spin representation](semisimple-lie-algebra.md#spin-representation)
          - [Spinor dimension in arbitrary spacetime dimension](semisimple-lie-algebra.md#spinor-dimension-in-arbitrary-spacetime-dimension)
      - [Lorentz algebra](semisimple-lie-algebra.md#lorentz-algebra)
        - [Lorentz generator](semisimple-lie-algebra.md#lorentz-generator)
        - [Rotation and boost commutators with a fixed metric signature](semisimple-lie-algebra.md#rotation-and-boost-commutators-with-a-fixed-metric-signature)
        - [Chiral decomposition of the complex Lorentz algebra](semisimple-lie-algebra.md#chiral-decomposition-of-the-complex-lorentz-algebra)
          - [Lorentz reality condition on chiral generators](semisimple-lie-algebra.md#lorentz-reality-condition-on-chiral-generators)
          - [Finite-dimensional complex Lorentz representations](semisimple-lie-algebra.md#finite-dimensional-complex-lorentz-representations)
          - [Parity action on a Lorentz representation](semisimple-lie-algebra.md#parity-action-on-a-lorentz-representation)
          - [Lorentz Casimir invariants](semisimple-lie-algebra.md#lorentz-casimir-invariants)
      - [so5 Lie algebra](semisimple-lie-algebra.md#so5-lie-algebra)
        - [SO5 to SO4 branching](semisimple-lie-algebra.md#so5-to-so4-branching)
          - [Left SU(2) subgroup of SO(4)](semisimple-lie-algebra.md#left-su-2-subgroup-of-so-4)
            - [Diagonal-root SU(2) embedding in SO(5)](semisimple-lie-algebra.md#diagonal-root-su-2-embedding-in-so-5)
      - [B2 root system](semisimple-lie-algebra.md#b2-root-system)
        - [B2 adjoint representation weight diagram](semisimple-lie-algebra.md#b2-adjoint-representation-weight-diagram)
        - [B2 weight lattice](semisimple-lie-algebra.md#b2-weight-lattice)
        - [Isomorphism between so5 and sp4](semisimple-lie-algebra.md#isomorphism-between-so5-and-sp4)
        - [Fundamental representations of B2](semisimple-lie-algebra.md#fundamental-representations-of-b2)
          - [Weyl dimension formula for B2](semisimple-lie-algebra.md#weyl-dimension-formula-for-b2)
            - [Traceless symmetric square of the defining so5 representation](semisimple-lie-algebra.md#traceless-symmetric-square-of-the-defining-so5-representation)
              - [Tensor-square decomposition of the defining so5 representation](semisimple-lie-algebra.md#tensor-square-decomposition-of-the-defining-so5-representation)
  - [Cartan subalgebra](semisimple-lie-algebra.md#cartan-subalgebra)
    - [Self-centralizing property of a Cartan subalgebra](semisimple-lie-algebra.md#self-centralizing-property-of-a-cartan-subalgebra)
    - [Nondegeneracy of the Killing form on a Cartan subalgebra](semisimple-lie-algebra.md#nondegeneracy-of-the-killing-form-on-a-cartan-subalgebra)
      - [Euclidean subspace of a Cartan subalgebra](semisimple-lie-algebra.md#euclidean-subspace-of-a-cartan-subalgebra)
        - [Killing dual of a coroot](semisimple-lie-algebra.md#killing-dual-of-a-coroot)
    - [Rank of a semisimple Lie algebra](semisimple-lie-algebra.md#rank-of-a-semisimple-lie-algebra)
    - [Root-space decomposition](semisimple-lie-algebra.md#root-space-decomposition)
      - [Triangular decomposition of a Lie algebra](semisimple-lie-algebra.md#triangular-decomposition-of-a-lie-algebra)
      - [Root-space reducedness lemma](semisimple-lie-algebra.md#root-space-reducedness-lemma)
      - [Root space](semisimple-lie-algebra.md#root-space)
        - [Root bracket and the opposite-root exception](semisimple-lie-algebra.md#root-bracket-and-the-opposite-root-exception)
        - [Root vector](semisimple-lie-algebra.md#root-vector)
      - [Regular element of a semisimple Lie algebra](semisimple-lie-algebra.md#regular-element-of-a-semisimple-lie-algebra)
        - [Regular element criterion in a Cartan subalgebra](semisimple-lie-algebra.md#regular-element-criterion-in-a-cartan-subalgebra)
      - [Two-root decomposition with a nondegenerate trace form](semisimple-lie-algebra.md#two-root-decomposition-with-a-nondegenerate-trace-form)
      - [sl2 subalgebra associated with a root](semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root)
        - [Nonisotropic root lemma](semisimple-lie-algebra.md#nonisotropic-root-lemma)
      - [Root system](semisimple-lie-algebra.md#root-system)
        - [Root hyperplane](semisimple-lie-algebra.md#root-hyperplane)
        - [Root subsystem](semisimple-lie-algebra.md#root-subsystem)
        - [Negative root](semisimple-lie-algebra.md#negative-root)
        - [Obtuse nonopposite roots have a root sum](semisimple-lie-algebra.md#obtuse-nonopposite-roots-have-a-root-sum)
        - [Irreducible root system](semisimple-lie-algebra.md#irreducible-root-system)
          - [Weyl orbit spans an irreducible root space](semisimple-lie-algebra.md#weyl-orbit-spans-an-irreducible-root-space)
        - [Crystallographic root system](semisimple-lie-algebra.md#crystallographic-root-system)
        - [Root of a root system](semisimple-lie-algebra.md#root-of-a-root-system)
        - [Rank-one root system](semisimple-lie-algebra.md#rank-one-root-system)
        - [A2 root system](semisimple-lie-algebra.md#a2-root-system)
          - [A2 fundamental weights and weight lattice](semisimple-lie-algebra.md#a2-fundamental-weights-and-weight-lattice)
        - [Automorphism of a root system](semisimple-lie-algebra.md#automorphism-of-a-root-system)
        - [Long root](semisimple-lie-algebra.md#long-root)
        - [Short root](semisimple-lie-algebra.md#short-root)
        - [Root reflection](semisimple-lie-algebra.md#root-reflection)
        - [Cartan integer](semisimple-lie-algebra.md#cartan-integer)
        - [Reduced root system](semisimple-lie-algebra.md#reduced-root-system)
        - [A3 root system](semisimple-lie-algebra.md#a3-root-system)
          - [Cartan matrix of type A3](semisimple-lie-algebra.md#cartan-matrix-of-type-a3)
        - [Root string](semisimple-lie-algebra.md#root-string)
          - [Root-string theorem](semisimple-lie-algebra.md#root-string-theorem)
        - [Cartan matrix](semisimple-lie-algebra.md#cartan-matrix)
        - [Positive root](semisimple-lie-algebra.md#positive-root)
          - [Simple root](semisimple-lie-algebra.md#simple-root)
            - [Simple-root subtraction lemma](semisimple-lie-algebra.md#simple-root-subtraction-lemma)
            - [Action of a simple reflection on positive roots](semisimple-lie-algebra.md#action-of-a-simple-reflection-on-positive-roots)
          - [Highest root](semisimple-lie-algebra.md#highest-root)
          - [Half-sum of positive roots](semisimple-lie-algebra.md#half-sum-of-positive-roots)
        - [Coroot](semisimple-lie-algebra.md#coroot)
          - [Simple coroot](semisimple-lie-algebra.md#simple-coroot)
          - [Dual root system](semisimple-lie-algebra.md#dual-root-system)
        - [Root lattice](semisimple-lie-algebra.md#root-lattice)
          - [Kostant partition function](semisimple-lie-algebra.md#kostant-partition-function)
            - [Generating series of the Kostant partition function](semisimple-lie-algebra.md#generating-series-of-the-kostant-partition-function)
          - [Dominance order](semisimple-lie-algebra.md#dominance-order)
        - [Weight lattice](semisimple-lie-algebra.md#weight-lattice)
          - [Integrality of representation weights on coroots](semisimple-lie-algebra.md#integrality-of-representation-weights-on-coroots)
          - [Group ring of a weight lattice](semisimple-lie-algebra.md#group-ring-of-a-weight-lattice)
            - [Root-binomial divisibility of reflection anti-invariants](semisimple-lie-algebra.md#root-binomial-divisibility-of-reflection-anti-invariants)
          - [Dynkin label](semisimple-lie-algebra.md#dynkin-label)
          - [Dominant weight](semisimple-lie-algebra.md#dominant-weight)
          - [Dominant integral weight](semisimple-lie-algebra.md#dominant-integral-weight)
          - [Fundamental weight](semisimple-lie-algebra.md#fundamental-weight)
            - [Fundamental representation](semisimple-lie-algebra.md#fundamental-representation)
              - [Dynkin index](semisimple-lie-algebra.md#dynkin-index)
                - [Cubic anomaly coefficient](semisimple-lie-algebra.md#cubic-anomaly-coefficient)
              - [Two-index symmetric representation](semisimple-lie-algebra.md#two-index-symmetric-representation)
              - [Two-index antisymmetric representation](semisimple-lie-algebra.md#two-index-antisymmetric-representation)
                - [Real structure of the SU4 exterior square](semisimple-lie-algebra.md#real-structure-of-the-su4-exterior-square)
        - [Weyl reflection](semisimple-lie-algebra.md#weyl-reflection)
          - [Reflection group of a root system](semisimple-lie-algebra.md#reflection-group-of-a-root-system)
            - [Weyl group](semisimple-lie-algebra.md#weyl-group)
              - [Reflection representation of a Weyl group](semisimple-lie-algebra.md#reflection-representation-of-a-weyl-group)
              - [Longest Weyl-group element](semisimple-lie-algebra.md#longest-weyl-group-element)
              - [Coxeter length](semisimple-lie-algebra.md#coxeter-length)
                - [Weyl stabilizer of a dominant point](semisimple-lie-algebra.md#weyl-stabilizer-of-a-dominant-point)
                - [Inversion set of a Weyl-group element](semisimple-lie-algebra.md#inversion-set-of-a-weyl-group-element)
                - [Positive-root criterion for Coxeter length](semisimple-lie-algebra.md#positive-root-criterion-for-coxeter-length)
        - [Dynkin diagram](semisimple-lie-algebra.md#dynkin-diagram)
          - [Classification of finite crystallographic Dynkin diagrams](semisimple-lie-algebra.md#classification-of-finite-crystallographic-dynkin-diagrams)
          - [Acyclicity of a finite Dynkin diagram](semisimple-lie-algebra.md#acyclicity-of-a-finite-dynkin-diagram)
          - [G2 Dynkin diagram](semisimple-lie-algebra.md#g2-dynkin-diagram)
          - [F4 Dynkin diagram](semisimple-lie-algebra.md#f4-dynkin-diagram)
          - [En Dynkin diagram](semisimple-lie-algebra.md#en-dynkin-diagram)
          - [Dn Dynkin diagram](semisimple-lie-algebra.md#dn-dynkin-diagram)
          - [Cn Dynkin diagram](semisimple-lie-algebra.md#cn-dynkin-diagram)
          - [An Dynkin diagram](semisimple-lie-algebra.md#an-dynkin-diagram)
          - [Simply laced root system](semisimple-lie-algebra.md#simply-laced-root-system)
            - [ADE classification](semisimple-lie-algebra.md#ade-classification)
          - [D3 root system](semisimple-lie-algebra.md#d3-root-system)
            - [Isomorphism between so6 and sl4](semisimple-lie-algebra.md#isomorphism-between-so6-and-sl4)
          - [Extended Dynkin diagram](semisimple-lie-algebra.md#extended-dynkin-diagram)
        - [Long-root subsystem](semisimple-lie-algebra.md#long-root-subsystem)
        - [G2 root system](semisimple-lie-algebra.md#g2-root-system)
          - [Triple bond isolates a G2 component](semisimple-lie-algebra.md#triple-bond-isolates-a-g2-component)
          - [G2 adjoint branching to a short-root sl2 subalgebra](semisimple-lie-algebra.md#g2-adjoint-branching-to-a-short-root-sl2-subalgebra)
          - [Long-root A2 subsystem of G2](semisimple-lie-algebra.md#long-root-a2-subsystem-of-g2)
            - [Restriction of the seven-dimensional G2 representation to long-root A2](semisimple-lie-algebra.md#restriction-of-the-seven-dimensional-g2-representation-to-long-root-a2)
        - [Root-system finiteness lemma](semisimple-lie-algebra.md#root-system-finiteness-lemma)
          - [Classification of rank-two root systems](semisimple-lie-algebra.md#classification-of-rank-two-root-systems)
            - [Weyl group of a rank-two root system](semisimple-lie-algebra.md#weyl-group-of-a-rank-two-root-system)
        - [Fundamental system of a root system](semisimple-lie-algebra.md#fundamental-system-of-a-root-system)
          - [Positive system of a root system](semisimple-lie-algebra.md#positive-system-of-a-root-system)
          - [Fundamental chamber of a root system](semisimple-lie-algebra.md#fundamental-chamber-of-a-root-system)
            - [Closed dominant Weyl chamber](semisimple-lie-algebra.md#closed-dominant-weyl-chamber)
  - [Highest-weight representation](semisimple-lie-algebra.md#highest-weight-representation)
    - [Highest-weight classification of finite-dimensional semisimple Lie algebra modules](semisimple-lie-algebra.md#highest-weight-classification-of-finite-dimensional-semisimple-lie-algebra-modules)
    - [A2 representation of highest weight (2,0)](semisimple-lie-algebra.md#a2-representation-of-highest-weight-2-0)
      - [Tensor square of the A2 representation of highest weight (2,0)](semisimple-lie-algebra.md#tensor-square-of-the-a2-representation-of-highest-weight-2-0)
        - [Weight multiplicities in the A2 tensor square of highest weight (2,0)](semisimple-lie-algebra.md#weight-multiplicities-in-the-a2-tensor-square-of-highest-weight-2-0)
    - [Dominant root-lattice highest weights have zero weight](semisimple-lie-algebra.md#dominant-root-lattice-highest-weights-have-zero-weight)
    - [Minuscule representation](semisimple-lie-algebra.md#minuscule-representation)
      - [Formal character of a minuscule representation](semisimple-lie-algebra.md#formal-character-of-a-minuscule-representation)
      - [Minuscule weight](semisimple-lie-algebra.md#minuscule-weight)
        - [Minuscule weights in the root lattice are zero](semisimple-lie-algebra.md#minuscule-weights-in-the-root-lattice-are-zero)
    - [Highest weight of a representation](semisimple-lie-algebra.md#highest-weight-of-a-representation)
      - [Highest-weight coordinates](semisimple-lie-algebra.md#highest-weight-coordinates)
        - [SU(3) highest-weight coordinates](semisimple-lie-algebra.md#su-3-highest-weight-coordinates)
    - [Ladder operator](semisimple-lie-algebra.md#ladder-operator)
      - [Raising operator](semisimple-lie-algebra.md#raising-operator)
      - [Lowering operator](semisimple-lie-algebra.md#lowering-operator)
    - [Cartan-Weyl basis](semisimple-lie-algebra.md#cartan-weyl-basis)
      - [Disentangling identity](semisimple-lie-algebra.md#disentangling-identity)
    - [Weyl's theorem on complete reducibility](semisimple-lie-algebra.md#weyl-s-theorem-on-complete-reducibility)
    - [Generation by fundamental representations](semisimple-lie-algebra.md#generation-by-fundamental-representations)
    - [Weight multiplicity decreases away from a dominant weight](semisimple-lie-algebra.md#weight-multiplicity-decreases-away-from-a-dominant-weight)
    - [Weight vector](semisimple-lie-algebra.md#weight-vector)
      - [Highest-weight vector](semisimple-lie-algebra.md#highest-weight-vector)
      - [Weight of a representation](semisimple-lie-algebra.md#weight-of-a-representation)
      - [Weight space](semisimple-lie-algebra.md#weight-space)
        - [Weight decomposition](semisimple-lie-algebra.md#weight-decomposition)
        - [Generalized weight space of a Lie algebra representation](semisimple-lie-algebra.md#generalized-weight-space-of-a-lie-algebra-representation)
          - [Generalized-weight decomposition for a nilpotent Lie algebra](semisimple-lie-algebra.md#generalized-weight-decomposition-for-a-nilpotent-lie-algebra)
            - [Zero generalized weight space of a Cartan subalgebra](semisimple-lie-algebra.md#zero-generalized-weight-space-of-a-cartan-subalgebra)
        - [Weight string](semisimple-lie-algebra.md#weight-string)
          - [Weight-string enumeration algorithm](semisimple-lie-algebra.md#weight-string-enumeration-algorithm)
        - [Weight-space decomposition](semisimple-lie-algebra.md#weight-space-decomposition)
          - [Weight basis](semisimple-lie-algebra.md#weight-basis)
          - [Weight diagram](semisimple-lie-algebra.md#weight-diagram)
            - [Shell multiplicities in an SU(3) weight diagram](semisimple-lie-algebra.md#shell-multiplicities-in-an-su-3-weight-diagram)
            - [Weight diagram of the defining SU(3) representation](semisimple-lie-algebra.md#weight-diagram-of-the-defining-su-3-representation)
            - [Tensor-product weight diagram](semisimple-lie-algebra.md#tensor-product-weight-diagram)
        - [Extremal weight space](semisimple-lie-algebra.md#extremal-weight-space)
        - [Weight multiplicity](semisimple-lie-algebra.md#weight-multiplicity)
          - [Kostant multiplicity formula](semisimple-lie-algebra.md#kostant-multiplicity-formula)
          - [Cyclic trace identity between adjacent weight spaces](semisimple-lie-algebra.md#cyclic-trace-identity-between-adjacent-weight-spaces)
          - [Freudenthal multiplicity formula](semisimple-lie-algebra.md#freudenthal-multiplicity-formula)
      - [Singular vector](semisimple-lie-algebra.md#singular-vector)
    - [Verma module](semisimple-lie-algebra.md#verma-module)
      - [Universal property of a Verma module](semisimple-lie-algebra.md#universal-property-of-a-verma-module)
      - [Irreducible quotient of a Verma module](semisimple-lie-algebra.md#irreducible-quotient-of-a-verma-module)
        - [Maximal proper submodule of a dominant integral Verma module](semisimple-lie-algebra.md#maximal-proper-submodule-of-a-dominant-integral-verma-module)
    - [Formal character of a weight module](semisimple-lie-algebra.md#formal-character-of-a-weight-module)
      - [Highest-weight character subtraction](semisimple-lie-algebra.md#highest-weight-character-subtraction)
      - [sl3 interlacing character formula](semisimple-lie-algebra.md#sl3-interlacing-character-formula)
        - [Dominant weight multiplicity formula for sl3](semisimple-lie-algebra.md#dominant-weight-multiplicity-formula-for-sl3)
    - [Weyl character formula](semisimple-lie-algebra.md#weyl-character-formula)
      - [Weyl alternant](semisimple-lie-algebra.md#weyl-alternant)
      - [Alternant orthogonality on a unitary torus](semisimple-lie-algebra.md#alternant-orthogonality-on-a-unitary-torus)
      - [Alternant character formula for the general linear group](semisimple-lie-algebra.md#alternant-character-formula-for-the-general-linear-group)
      - [Character of a Weyl-vector multiple](semisimple-lie-algebra.md#character-of-a-weyl-vector-multiple)
      - [Weyl denominator formula](semisimple-lie-algebra.md#weyl-denominator-formula)
        - [Weyl denominator](semisimple-lie-algebra.md#weyl-denominator)
      - [Weyl dimension formula](semisimple-lie-algebra.md#weyl-dimension-formula)
        - [Lowest-degree alternant proof of the Weyl dimension formula](semisimple-lie-algebra.md#lowest-degree-alternant-proof-of-the-weyl-dimension-formula)
        - [G2 dimension polynomial](semisimple-lie-algebra.md#g2-dimension-polynomial)
        - [Weyl dimension formula for C2](semisimple-lie-algebra.md#weyl-dimension-formula-for-c2)
      - [q-character of a highest-weight representation](semisimple-lie-algebra.md#q-character-of-a-highest-weight-representation)
        - [Principal q-character of the G2 adjoint representation](semisimple-lie-algebra.md#principal-q-character-of-the-g2-adjoint-representation)
    - [Crystal basis](semisimple-lie-algebra.md#crystal-basis)
      - [B2 adjoint crystal](semisimple-lie-algebra.md#b2-adjoint-crystal)
      - [B2 spin crystal](semisimple-lie-algebra.md#b2-spin-crystal)
      - [Crystal of the defining symplectic representation](semisimple-lie-algebra.md#crystal-of-the-defining-symplectic-representation)
        - [Tensor square of the defining C2 crystal](semisimple-lie-algebra.md#tensor-square-of-the-defining-c2-crystal)
      - [Crystal of the seven-dimensional G2 representation](semisimple-lie-algebra.md#crystal-of-the-seven-dimensional-g2-representation)
        - [Exterior and symmetric squares of the seven-dimensional G2 representation](semisimple-lie-algebra.md#exterior-and-symmetric-squares-of-the-seven-dimensional-g2-representation)
      - [Crystal of the defining odd-orthogonal representation](semisimple-lie-algebra.md#crystal-of-the-defining-odd-orthogonal-representation)
      - [Root-string property of a crystal](semisimple-lie-algebra.md#root-string-property-of-a-crystal)
      - [Kashiwara operator](semisimple-lie-algebra.md#kashiwara-operator)
      - [Tensor product of crystals](semisimple-lie-algebra.md#tensor-product-of-crystals)
        - [A2 defining tensor crystals](semisimple-lie-algebra.md#a2-defining-tensor-crystals)
        - [Crystal tensor-product rule](semisimple-lie-algebra.md#crystal-tensor-product-rule)
  - [Casimir element](semisimple-lie-algebra.md#casimir-element)
    - [Quadratic Casimir operator](semisimple-lie-algebra.md#quadratic-casimir-operator)
      - [SU(3) Casimir in Chevalley generators](semisimple-lie-algebra.md#su-3-casimir-in-chevalley-generators)
      - [SU(3) quadratic Casimir eigenvalue](semisimple-lie-algebra.md#su-3-quadratic-casimir-eigenvalue)
      - [Tensor-product Casimir trace identity](semisimple-lie-algebra.md#tensor-product-casimir-trace-identity)
    - [Casimir eigenvalue](semisimple-lie-algebra.md#casimir-eigenvalue)
    - [Casimir eigenvalue for sl2](semisimple-lie-algebra.md#casimir-eigenvalue-for-sl2)
  - [Principal sl2 subalgebra](semisimple-lie-algebra.md#principal-sl2-subalgebra)
    - [Construction of a principal sl2 triple](semisimple-lie-algebra.md#construction-of-a-principal-sl2-triple)
    - [Principal nilpotent element](semisimple-lie-algebra.md#principal-nilpotent-element)
  - [Weight (representation theory)](semisimple-lie-algebra.md#weight-representation-theory)

<h2 id="cartan-s-criterion">Cartan's criterion</h2>

↑ **Parent:** [Lie algebra](lie-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cartan's_criterion)

For a finite-dimensional [Lie algebra](lie-algebra.md) over a field of characteristic zero, [Cartan's criterion](#cartan-s-criterion) characterizes a [solvable Lie algebra](#solvable-lie-algebra) by vanishing of its [Killing form](#killing-form) on $\mathfrak g\times[\mathfrak g,\mathfrak g]$, and a [semisimple Lie algebra](semisimple-lie-algebra.md) by nondegeneracy of that form. The [Cartan solvability criterion](#cartan-solvability-criterion) and [Cartan criterion for semisimplicity](#cartan-criterion-for-semisimplicity) state the two distinct tests.

## Loop algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loop_algebra)

The algebraic loop algebra of a [Lie algebra](lie-algebra.md) $\mathfrak g$ over a [field](algebra.md#field) $k$ consists of finite [Laurent polynomials](polynomial.md#laurent-polynomial) with coefficients in $\mathfrak g$. Its [Lie bracket](#lie-bracket) is $[x\otimes t^m,y\otimes t^n]=[x,y]\otimes t^{m+n}$, extended bilinearly. Alternation and the [Jacobi identity](#jacobi-identity) follow from those of $\mathfrak g$, since the [Laurent polynomial ring](commutative-algebra.md#laurent-polynomial-ring) is commutative. Appropriate smooth or formal completions give other loop-algebra variants; the [affine current algebra](#affine-current-algebra) adds a central extension to these Fourier modes. For the affine extension, see [Kac and Wakimoto, Section 0.2](https://math.mit.edu/~kac/not-easily-available/kac-and-wakimoto-1990.pdf).

## Affine current algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

The affine current algebra is the one-dimensional central extension of the [loop algebra](#loop-algebra) of a finite-dimensional [Lie algebra](lie-algebra.md), with central element acting as the level $k$. A restricted module has $J_n v=0$ for all sufficiently large $n$ for each vector $v$; this makes the [Sugawara construction](string-theory.md#sugawara-construction) finite on each vector after [normal ordering](perturbative-quantum-field-theory.md#normal-ordering). In a compact unitary positive-energy representation, the nontrivial integrable levels are positive integers in the standard basic normalization.

## Free Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

The [Lie algebra](lie-algebra.md) over a commutative ring $R$ generated by a set $X$ subject only to bilinearity, alternation and the [Jacobi identity](#jacobi-identity). Every map from $X$ to the underlying set of an $R$-[Lie algebra](lie-algebra.md) extends uniquely to a [Lie algebra homomorphism](#lie-algebra-homomorphism). It can be constructed from bracketed words by quotienting by those identities; elements are represented by [Lie polynomials](#lie-polynomial).

### Lie polynomial

↑ **Parent:** [Free Lie algebra](#free-lie-algebra)

A finite linear combination of iterated [Lie brackets](#lie-bracket) in formal variables. It evaluates naturally in every [Lie algebra](lie-algebra.md), and every [Lie algebra homomorphism](#lie-algebra-homomorphism) preserves its evaluation. The homogeneous terms of the [Baker--Campbell--Hausdorff formula](linear-operator-theory.md#baker-campbell-hausdorff-formula) are rational Lie polynomials; this permits the group law to be reconstructed from the bracket wherever the series converges.

## Semidirect product of Lie algebras

↑ **Parent:** [Lie algebra](lie-algebra.md)

If $D:\mathfrak b\to\operatorname{Der}(\mathfrak a)$ is a [Lie algebra homomorphism](#lie-algebra-homomorphism) into the [derivations of a Lie algebra](#derivation-of-a-lie-algebra), the semidirect product has underlying vector space $\mathfrak a\oplus\mathfrak b$ and bracket $[(a,b),(a',b')]=([a,a']+D_ba'-D_{b'}a,[b,b'])$. The homomorphism and derivation identities ensure the [Jacobi identity](#jacobi-identity). The first factor is an ideal; the second is a subalgebra whose action records the twisting. The [diamond Lie algebra](#diamond-lie-algebra) arises by letting a one-dimensional algebra act on a [Heisenberg Lie algebra](#heisenberg-lie-algebra).

// Target: linear-algebra.bigb

## Lie algebra cohomology

↑ **Parent:** [Lie algebra](lie-algebra.md)

The Chevalley-Eilenberg complex consists of alternating maps from $\mathfrak g^k$ to a [Lie algebra representation](#lie-algebra-representation) $V$, with differential built from the bracket and module action. For trivial real coefficients, a two-cocycle is an alternating bilinear form $\kappa$ satisfying $\kappa([X,Y],Z)+\kappa([Y,Z],X)+\kappa([Z,X],Y)=0$. Coboundaries have the form $b([X,Y])$, up to the differential's sign convention. Their quotient is $H^2(\mathfrak g,\mathbb R)$ and classifies [central extensions of a Lie algebra](#central-extension-of-a-lie-algebra).

### Lie algebra two-cocycle

↑ **Parent:** [Lie algebra cohomology](#lie-algebra-cohomology)

For trivial real coefficients, a Lie algebra two-cocycle is an alternating bilinear form satisfying $\kappa([X,Y],Z)+\kappa([Y,Z],X)+\kappa([Z,X],Y)=0$. Adding a form $b([X,Y])$ does not change its [Lie algebra cohomology](#lie-algebra-cohomology) class. The bracket $[(X,a),(Y,b)]=([X,Y],\kappa(X,Y))$ defines a [central extension of a Lie algebra](#central-extension-of-a-lie-algebra) by $\mathbb R$ precisely when this cocycle identity holds. The constant discrepancy in a [moment-map equivariance obstruction](symplectic-geometry.md#moment-map-equivariance-obstruction) is such a cocycle.

## Compact Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

A real Lie algebra is compact when it is the Lie algebra of some [compact Lie group](lie-theory.md#compact-lie-group). Equivalently, it has a positive-definite [invariant bilinear form on a Lie algebra](#invariant-bilinear-form-on-a-lie-algebra). It is a direct sum of an abelian center and a compact [semisimple Lie algebra](semisimple-lie-algebra.md). For its semisimple part, the [compactness criterion from the Killing form](#compactness-criterion-from-the-killing-form) is negative-definiteness of the [Killing form](#killing-form). This definition concerns the algebra; a global group with that algebra can still have a noncompact central covering direction.

## Powerful Lie algebra over p-adic integers

↑ **Parent:** [Lie algebra](lie-algebra.md)

A [Lie algebra](lie-algebra.md) over the [p-adic integers](number-theory.md#p-adic-integer) whose underlying [module](module-theory.md#module-mathematics) is free of finite rank and whose [Lie bracket](#lie-bracket) satisfies $[L,L]\subseteq p^\epsilon L$, where $\epsilon=1$ for odd $p$ and $\epsilon=2$ for $p=2$. Finite freeness is part of this convention: merely requiring a small [Lie bracket](#lie-bracket) on a torsion module would not correspond to [uniform pro-p groups](topological-group.md#uniform-pro-p-group).

### Lie algebra of a uniform pro-p group

↑ **Parent:** [Powerful Lie algebra over p-adic integers](#powerful-lie-algebra-over-p-adic-integers)

On the set underlying a [uniform pro-p group](topological-group.md#uniform-pro-p-group), define scalar multiplication by $\lambda x=x^\lambda$, and define addition and the [Lie bracket](#lie-bracket) by

$$
x+_Ly=\lim_{n\to\infty}(x^{p^n}y^{p^n})^{p^{-n}},\qquad [x,y]_L=\lim_{n\to\infty}[x^{p^n},y^{p^n}]^{p^{-2n}}.
$$

Roots are the unique roots in the appropriate power layers. The limits give a [powerful Lie lattice](#powerful-lie-algebra-over-p-adic-integers). In a suitable complete normed [group algebra](associative-algebra.md#group-algebra), the [p-adic logarithm](arithmetic.md#p-adic-logarithm) identifies these operations with ordinary addition and the associative-algebra commutator.

### BCH convergence on a powerful Lie lattice

↑ **Parent:** [Powerful Lie algebra over p-adic integers](#powerful-lie-algebra-over-p-adic-integers)

The [Baker--Campbell--Hausdorff formula](linear-operator-theory.md#baker-campbell-hausdorff-formula) converges integrally on a [powerful Lie lattice](#powerful-lie-algebra-over-p-adic-integers). A degree-$m$ Lie term has bracket divisibility $p^{\epsilon(m-1)}$; the standard integral coefficient bound loses at most $\lfloor(m-1)/(p-1)\rfloor$ powers of $p$. The remaining valuation tends to infinity. Associativity follows from the formal exponential identity, the identity is zero, the inverse is $-x$, and $x^{*n}=nx$. The resulting [pro-p group](topological-group.md#pro-p-group) is a [uniform pro-p group](topological-group.md#uniform-pro-p-group), with power subgroups $p^nL$.

## Cross-product Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

The [vector space](vector-space.md) $\mathbb R^3$ with the [cross product](vector-space.md#cross-product) as [Lie bracket](#lie-bracket). The vector triple-product identity proves the [Jacobi identity](#jacobi-identity). The map $x\mapsto-(i/2)x\cdot\sigma$ is a [Lie algebra isomorphism](#lie-algebra-isomorphism) to the compact real [SU(2) Lie algebra](semisimple-lie-algebra.md#su-2-lie-algebra), using the [Pauli matrix commutator identity](algebra.md#pauli-matrix-commutator-identity).

## Euclidean motion Lie algebra in two dimensions

↑ **Parent:** [Lie algebra](lie-algebra.md)

The real [Lie algebra](lie-algebra.md) $\mathfrak{iso}(2)$ is a semidirect product of planar translations with infinitesimal rotations. One orientation convention is $[J,E_1]=-E_2$, $[J,E_2]=E_1$, $[E_1,E_2]=0$. Its translation space is a two-dimensional abelian [ideal of a Lie algebra](#ideal-of-a-lie-algebra).

### Killing form of the planar Euclidean motion Lie algebra

↑ **Parent:** [Euclidean motion Lie algebra in two dimensions](#euclidean-motion-lie-algebra-in-two-dimensions)

In the ordered basis $(J,E_1,E_2)$ of the [Euclidean motion Lie algebra in two dimensions](#euclidean-motion-lie-algebra-in-two-dimensions), the [Killing form](#killing-form) has matrix $\operatorname{diag}(-2,0,0)$. Its radical is the translation ideal, and the algebra is solvable rather than semisimple.

## Graded Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

A [graded Lie algebra](#graded-lie-algebra) has a [graded Lie bracket](#graded-lie-bracket) preserving total degree, with $[u,v]=-(-1)^{|u||v|}[v,u]$ and $[u,[v,w]]=[[u,v],w]+(-1)^{|u||v|}[v,[u,w]]$ for homogeneous vectors in the indicated degrees. A [Gerstenhaber algebra](commutative-algebra.md#gerstenhaber-algebra) uses this sign rule after shifting degrees by one.

<h3 id="chevalley-eilenberg-cochains-of-a-graded-lie-algebra">Chevalley–Eilenberg cochains of a graded Lie algebra</h3>

↑ **Parent:** [Graded Lie algebra](#graded-lie-algebra)

For a positively [graded Lie algebra](#graded-lie-algebra) $L$ over $\mathbb Q$, finite-dimensional in each degree, its cochain algebra is free graded commutative on the graded dual of $sL$, with differential dual to the Lie bracket and its Koszul signs. The Jacobi identity gives $d^2=0$. A Lie element of degree $r$ contributes a cochain generator of degree $r+1$. Its [cohomology](cohomology.md) computes $\operatorname{Ext}_{U(L)}(\mathbb Q,\mathbb Q)$ with total grading; the standard free enveloping-algebra resolution gives this identification. For a [free graded Lie algebra](#free-graded-lie-algebra), the tensor-algebra augmentation has a length-one free resolution, explaining the square-zero [cohomology](cohomology.md) of a rational [wedge sum](topology.md#wedge-sum) of spheres.

### Free graded Lie algebra

↑ **Parent:** [Graded Lie algebra](#graded-lie-algebra)

For a positively graded [vector space](vector-space.md) $V$, the free [graded Lie algebra](#graded-lie-algebra) $\mathbb L(V)$ receives a linear map from $V$ and extends every graded linear map $V\to L$ uniquely to a Lie homomorphism. Over $\mathbb Q$, it is the Lie subalgebra generated by $V$ inside the [tensor algebra](linear-algebra.md#tensor-algebra) $T(V)$, using $[u,v]=uv-(-1)^{|u||v|}vu$. Its [universal enveloping algebra](#universal-enveloping-algebra) is $T(V)$: both have the same universal property for maps from $V$ into associative algebras. The primitives of the tensor [Hopf algebra](algebra.md#hopf-algebra) with primitive generators are exactly $\mathbb L(V)$.

### Graded Lie bracket

↑ **Parent:** [Graded Lie algebra](#graded-lie-algebra)

The bracket on a [graded Lie algebra](#graded-lie-algebra) is a bilinear operation satisfying graded antisymmetry and the graded [Jacobi identity](#jacobi-identity). For homogeneous elements of degrees $r,s$, $[u,v]=-(-1)^{rs}[v,u]$. A [Gerstenhaber bracket](associative-algebra.md#gerstenhaber-bracket) uses this convention on the shifted degrees $r=|u|-1$ and $s=|v|-1$.

## Central extension of a Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

A central extension is a [Lie algebra](lie-algebra.md) surjection whose [kernel](linear-algebra.md#kernel-of-a-linear-map) commutes with every element of the larger algebra. The [Virasoro central extension](string-theory.md#virasoro-central-extension) adds a central generator to the [Witt algebra](#witt-algebra).

## Witt algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Witt_algebra)

The Witt algebra is the [Lie algebra](lie-algebra.md) of vector fields on a circle with Laurent-polynomial coefficients. Its nontrivial [central extension of a Lie algebra](#central-extension-of-a-lie-algebra) is the [Virasoro algebra](string-theory.md#virasoro-algebra).

## Centralizer of an element of a Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

For an element $x$ of a [Lie algebra](lie-algebra.md) $\mathfrak g$, its centralizer is the [Lie subalgebra](#lie-subalgebra) $Z_{\mathfrak g}(x)=\{y\in\mathfrak g:[y,x]=0\}$, equivalently the [kernel](linear-algebra.md#kernel-of-a-linear-map) of $\operatorname{ad}x$ in the [Adjoint representation](#adjoint-representation-of-a-lie-algebra).

### Centralizer lower bound for a root vector

↑ **Parent:** [Centralizer of an element of a Lie algebra](#centralizer-of-an-element-of-a-lie-algebra)

In a complex [semisimple Lie algebra](semisimple-lie-algebra.md) whose [rank of a semisimple Lie algebra](semisimple-lie-algebra.md#rank-of-a-semisimple-lie-algebra) is $\ell$, a [root vector](semisimple-lie-algebra.md#root-vector) $x$ satisfies $\dim Z_{\mathfrak g}(x)\geq3\ell-2$. To see this, select $\ell-1$ roots whose images form a basis of the real root span modulo $\mathbb R\alpha$, where $x\in\mathfrak g_\alpha$. Take the highest endpoints of the [root strings](semisimple-lie-algebra.md#root-string) through both signs of each selected root. Their $2(\ell-1)$ distinct [root spaces](semisimple-lie-algebra.md#root-space) commute with $x$. Together with $\ker\alpha\subset\mathfrak t$ and $\mathbb Cx$, these give $2(\ell-1)+(\ell-1)+1$ independent vectors in the [Lie algebra centralizer](#centralizer-of-an-element-of-a-lie-algebra).

## Lie algebra generator

↑ **Parent:** [Lie algebra](lie-algebra.md)

A Lie algebra generator is an element of a chosen spanning or generating set for a Lie algebra. In a matrix representation, an infinitesimal group transformation has the form $1+i\alpha_at^a+O(\alpha^2)$ in terms of generator matrices $t^a$.

## Lie algebra of a matrix Lie group

↑ **Parent:** [Lie algebra](lie-algebra.md)

For a [Matrix Lie group](lie-theory.md#matrix-lie-group) $G$, its tangent space $\mathfrak g=T_I G$ is closed under the matrix [commutator](#commutator). Indeed, for $X,Y\in\mathfrak g$, the group commutator

$$
e^{tX}e^{sY}e^{-tX}e^{-sY}
$$

lies in $G$, and the mixed derivative at $(0,0)$ of its matrix logarithm is $XY-YX$. Thus $[X,Y]=XY-YX$ belongs to $\mathfrak g$.

### Matrix commutator from a logarithm chart

↑ **Parent:** [Lie algebra of a matrix Lie group](#lie-algebra-of-a-matrix-lie-group)

If the matrix logarithm identifies a neighborhood of the identity in a [Matrix Lie group](lie-theory.md#matrix-lie-group) with a neighborhood of zero in its tangent subspace, the logarithm of the displayed group commutator belongs to that subspace. Divide it by $t^2$ and take the limit. Finite-dimensional linear subspaces are closed, proving closure under the matrix [commutator](#commutator) without attempting to give a nonsmooth square-root reparametrization a velocity.

### General linear Lie algebra

↑ **Parent:** [Lie algebra of a matrix Lie group](#lie-algebra-of-a-matrix-lie-group)

The [endomorphisms](algebra.md#endomorphism) of a [vector space](vector-space.md) form a [Lie algebra](lie-algebra.md) under the [commutator](#commutator) $[A,B]=AB-BA$. It is the [Lie algebra](lie-algebra.md) of the [general linear group](group-theory.md#general-linear-group); the [Jacobi identity](#jacobi-identity) follows by expanding associative products.

### Unitary Lie algebra

↑ **Parent:** [Lie algebra of a matrix Lie group](#lie-algebra-of-a-matrix-lie-group)

The real [Lie algebra](lie-algebra.md) of the [unitary group](topological-group.md#unitary-group) is $\mathfrak u(N)=\{X:X^\dagger=-X\}$, of real dimension $N^2$. Differentiating unitarity gives necessity; exponentiating any [skew-Hermitian matrix](linear-operator-theory.md#skew-hermitian-matrix) gives a curve in the group, proving sufficiency.

#### Special unitary Lie algebra

↑ **Parent:** [Unitary Lie algebra](#unitary-lie-algebra)

The real [Lie algebra](lie-algebra.md) of the [special unitary group](topological-group.md#special-unitary-group) consists of traceless [skew-Hermitian matrices](linear-operator-theory.md#skew-hermitian-matrix). Differentiating unitarity and determinant one gives the two constraints; exponentiating any such matrix proves their sufficiency. The [commutator](#commutator) is again skew-Hermitian and traceless. Its real dimension is $n^2-1$, and its complexification is $\mathfrak{sl}_n(\mathbb C)$.

<h5 id="trace-normalization-of-su-2">Trace normalization of su(2)</h5>

↑ **Parent:** [Special unitary Lie algebra](#special-unitary-lie-algebra)

With the defining two-dimensional [matrix trace](linear-algebra.md#matrix-trace) and [inner product](linear-algebra.md#inner-product) $\langle X,Y\rangle=-\operatorname{tr}(XY)$, the displayed [Pauli matrix](algebra.md#pauli-matrices) basis is orthonormal. The [Pauli matrix multiplication law](algebra.md#pauli-matrix-multiplication-law) gives the indicated [structure constants of a Lie algebra](#structure-constant-of-a-lie-algebra). With the alternative form $-2\operatorname{tr}(XY)$, the orthonormal basis is $-i\sigma_a/2$ and the structure constant is one. The bracket and inner-product normalizations must be kept consistent in projected gauge-field formulas.

<h4 id="su-3-lie-algebra">SU(3) Lie algebra</h4>

↑ **Parent:** [Unitary Lie algebra](#unitary-lie-algebra)

The compact real [Lie algebra](lie-algebra.md) $\mathfrak{su}(3)$ consists of traceless anti-Hermitian $3\times3$ matrices. Physicists often specify Hermitian generators $t_a$ instead, so the genuine [Lie algebra](lie-algebra.md) elements are $it_a$. The compact real algebra and its complexification $\mathfrak{sl}_3(\mathbb C)$ should be distinguished.

<h5 id="root-su-2-subalgebras-of-su-3">Root SU(2) subalgebras of SU(3)</h5>

↑ **Parent:** [SU(3) Lie algebra](#su-3-lie-algebra)

Each [root](semisimple-lie-algebra.md#root-of-a-root-system) $\alpha$ of the [SU(3) Lie algebra](#su-3-lie-algebra) defines an [SU(2) Lie algebra](semisimple-lie-algebra.md#su-2-lie-algebra) generated by $J_3=\alpha\cdot H$ and $J_\pm=\sqrt2 E_{\pm\alpha}$ in the root-length-one convention. They obey $[J_3,J_\pm]=\pm J_\pm$ and $[J_+,J_-]=2J_3$. These subalgebras explain [root](semisimple-lie-algebra.md#root-of-a-root-system) strings, [Weyl group](semisimple-lie-algebra.md#weyl-group) reflections and the integer [Dynkin labels](semisimple-lie-algebra.md#dynkin-label) of [highest weights](semisimple-lie-algebra.md#highest-weight-of-a-representation).

// Target: lie-theory.bigb

#### Matrix-unit basis of the unitary Lie algebra

↑ **Parent:** [Unitary Lie algebra](#unitary-lie-algebra)

A real basis of the [unitary Lie algebra](#unitary-lie-algebra) is $iE_{ii}$, $E_{ij}-E_{ji}$ and $i(E_{ij}+E_{ji})$ for $i<j$, where $E_{ij}$ are [matrix units](vector-space.md#matrix-unit). These separately span the imaginary diagonal and real and imaginary upper off-diagonal entries.

## Lie algebra isomorphism

↑ **Parent:** [Lie algebra](lie-algebra.md)

A Lie algebra isomorphism is a bijective [linear map](vector-space.md#linear-map) $\varphi:\mathfrak g\to\mathfrak h$ satisfying $\varphi([x,y])=[\varphi(x),\varphi(y)]$. Its inverse automatically preserves the [Lie bracket](#lie-bracket).

## Direct sum of Lie algebras

↑ **Parent:** [Lie algebra](lie-algebra.md)

The direct sum $\mathfrak g\oplus\mathfrak h$ has componentwise bracket

$$
[(x,y),(x',y')]=([x,x'],[y,y']).
$$

The two summands are commuting [ideals](#ideal-of-a-lie-algebra).

## Lie subalgebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

A Lie subalgebra is a [vector subspace](vector-space.md#vector-subspace) closed under the [Lie bracket](#lie-bracket).

### Normalizer of a Lie subalgebra

↑ **Parent:** [Lie subalgebra](#lie-subalgebra)

The normalizer of a [Lie subalgebra](#lie-subalgebra) $H\subseteq L$ is

$$
N_L(H)=\{x\in L:[x,H]\subseteq H\}.
$$

It is the largest Lie subalgebra of $L$ in which $H$ is an [ideal of a Lie algebra](#ideal-of-a-lie-algebra).

## Derivation of a Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

A derivation of a [Lie algebra](lie-algebra.md) is an [algebraic derivation](algebra.md#derivation-differential-algebra), namely a [linear map](vector-space.md#linear-map) $D:L\to L$ satisfying

$$
D[x,y]=[Dx,y]+[x,Dy].
$$

Every adjoint map $\operatorname{ad}z:x\mapsto[z,x]$ is a derivation.

### Exponential of a nilpotent Lie algebra derivation

↑ **Parent:** [Derivation of a Lie algebra](#derivation-of-a-lie-algebra)

Over a [field](algebra.md#field) of characteristic zero, a [nilpotent operator](linear-operator-theory.md#nilpotent-linear-map) $D$ which is a [derivation of a Lie algebra](#derivation-of-a-lie-algebra) exponentiates to a [Lie algebra automorphism](#automorphism-of-a-lie-algebra). The iterated rule

$$
D^k[x,y]=\sum_{j=0}^k\binom{k}{j}[D^jx,D^{k-j}y]
$$

follows by induction using Pascal's identity. Regrouping the finite expansion of $[\exp(D)x,\exp(D)y]$ by total degree gives $\exp(D)[x,y]$. The inverse is $\exp(-D)$. This factorial construction must not be reduced naively to small positive characteristic.

### Inner derivation of a Lie algebra

↑ **Parent:** [Derivation of a Lie algebra](#derivation-of-a-lie-algebra)

An inner [derivation of a Lie algebra](#derivation-of-a-lie-algebra) is $\operatorname{ad}_x:y\mapsto[x,y]$. The [Jacobi identity](#jacobi-identity) makes this a [derivation of a Lie algebra](#derivation-of-a-lie-algebra). For every [derivation of a Lie algebra](#derivation-of-a-lie-algebra) $D$, $[D,\operatorname{ad}_x]=\operatorname{ad}_{Dx}$, so the inner derivations form an [ideal of a Lie algebra](#ideal-of-a-lie-algebra) in the [derivation Lie algebra](#derivation-lie-algebra). The [kernel](linear-algebra.md#kernel-of-a-linear-map) of $x\mapsto\operatorname{ad}_x$ is the [center of a Lie algebra](#center-of-a-lie-algebra).

### Derivation Lie algebra

↑ **Parent:** [Derivation of a Lie algebra](#derivation-of-a-lie-algebra)

The [derivations of a Lie algebra](#derivation-of-a-lie-algebra) form a [Lie subalgebra](#lie-subalgebra) of $\operatorname{End}(\mathfrak g)$ with the [commutator](#commutator) bracket. The identity $[D,\operatorname{ad}x]=\operatorname{ad}(Dx)$ makes the inner derivations an [ideal of a Lie algebra](#ideal-of-a-lie-algebra). For a complex [semisimple Lie algebra](semisimple-lie-algebra.md), the [Weyl complete reducibility theorem](semisimple-lie-algebra.md#weyl-complete-reducibility-theorem) and the vanishing [center of a Lie algebra](#center-of-a-lie-algebra) imply $\operatorname{Der}(\mathfrak g)=\operatorname{ad}\mathfrak g$.

### Outer derivation of a nilpotent Lie algebra

↑ **Parent:** [Derivation of a Lie algebra](#derivation-of-a-lie-algebra)

Every nonzero finite-dimensional nilpotent Lie algebra over a field of characteristic zero has a derivation outside its adjoint image. This remains true for characteristically nilpotent Lie algebras: all their derivations may be nilpotent, but they cannot all be inner.

### Generalized-eigenspace bracket lemma

↑ **Parent:** [Derivation of a Lie algebra](#derivation-of-a-lie-algebra)

If $D$ is a [derivation of a Lie algebra](#derivation-of-a-lie-algebra), then its [generalized eigenspaces](linear-operator-theory.md#generalized-eigenspace) satisfy

$$
[L_\lambda,L_\mu]\subseteq L_{\lambda+\mu}.
$$

Apply a sufficiently large power of $D-(\lambda+\mu)I$ and use the [binomial theorem](combinatorics.md#binomial-theorem) together with the derivation rule.

## Invariant bilinear form on a Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

A bilinear form $B$ on a Lie algebra is invariant when

$$
B([x,y],z)=B(x,[y,z]).
$$

For a symmetric form this says that every adjoint map is skew-adjoint with respect to $B$.

### Invariance of a bilinear form on a Lie algebra

↑ **Parent:** [Invariant bilinear form on a Lie algebra](#invariant-bilinear-form-on-a-lie-algebra)

For a symmetric [bilinear form](linear-algebra.md#bilinear-form) on a [Lie algebra](lie-algebra.md), invariance is the displayed identity. It equivalently says that each [Adjoint representation](#adjoint-representation-of-a-lie-algebra) endomorphism is skew-adjoint with respect to $B$. The [Killing form](#killing-form) has this property by cyclic invariance of the [trace](linear-algebra.md#matrix-trace).

### Positive invariant metric on a Lie algebra

↑ **Parent:** [Invariant bilinear form on a Lie algebra](#invariant-bilinear-form-on-a-lie-algebra)

A positive invariant metric is a positive-definite real symmetric [invariant bilinear form on a Lie algebra](#invariant-bilinear-form-on-a-lie-algebra). Each adjoint map is skew-adjoint. Invariance gives $[\mathfrak g,\mathfrak g]^\perp=\mathfrak z(\mathfrak g)$, so the algebra splits orthogonally into its Abelian center and its derived algebra. The latter has zero center, and $\kappa(X,X)=\operatorname{tr}(\operatorname{ad}_X^2)=-\|\operatorname{ad}_X\|^2$ is strictly negative for nonzero $X$. Thus it is compact semisimple; the whole algebra is compact reductive. Conversely, a compact semisimple summand has metric $-\kappa$ and the center can carry any positive metric. The [Killing form](#killing-form) alone vanishes on the center.

## Lie superalgebra

↑ **Parent:** [Lie algebra](lie-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lie_superalgebra)

A Lie superalgebra is a Z2-graded vector space with a graded-antisymmetric bracket satisfying the graded Jacobi identity. The bracket of two odd elements is symmetric and is conventionally written as an anticommutator.

### Lie superalgebra representation

↑ **Parent:** [Lie superalgebra](#lie-superalgebra)

A Lie superalgebra representation acts on a parity-graded vector space by linear operators preserving the graded brackets. Odd generators reverse parity, and their brackets are represented by [anticommutators](vector-space.md#anticommutator).

### Graded Jacobi identity

↑ **Parent:** [Lie superalgebra](#lie-superalgebra)

The [Jacobi identity](#jacobi-identity) of a [Lie superalgebra](#lie-superalgebra) includes parity signs. In particular, for odd $c$ and even $\phi$ it gives $[c,[c,\phi]]=\tfrac12[[c,c],\phi]$.

## Lie bracket

↑ **Parent:** [Lie algebra](lie-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lie_bracket)

The Lie bracket is the product in a [Lie algebra](lie-algebra.md). For matrix Lie algebras it is the [commutator](#commutator) $[X,Y]=XY-YX$.

### Antisymmetry of a Lie bracket

↑ **Parent:** [Lie bracket](#lie-bracket)

The relation $[x,y]=-[y,x]$ for a bilinear [Lie bracket](#lie-bracket). In characteristic zero it implies $[x,x]=0$. In characteristic two, the alternating identity must be required separately when defining a [Lie algebra](lie-algebra.md).

### Lie bracket from local group commutators

↑ **Parent:** [Lie bracket](#lie-bracket)

In a [local exponential chart](lie-theory.md#local-exponential-chart), the mixed second differential of the [group commutator](group.md#group-commutator) defines a [bilinear map](linear-algebra.md#bilinear-map) on the [tangent space](differential-geometry.md#tangent-space) at the identity. Inversion after swapping the two group elements proves antisymmetry. Differentiating conjugation gives $[X,Y]=\operatorname{ad}(X)Y$; applying [naturality of the Lie bracket](#differential-of-a-lie-group-homomorphism-preserves-lie-brackets) to the [Adjoint representation of a Lie group](lie-theory.md#adjoint-representation-of-a-lie-group) then proves the [Jacobi identity](#jacobi-identity). For a matrix group this recovers $XY-YX$ by expanding through the mixed term.

### Commutator

↑ **Parent:** [Lie bracket](#lie-bracket)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Commutator)

The commutator of two elements of an associative algebra is $[A,B]=AB-BA$. Matrix Lie algebras use the commutator as their [Lie bracket](#lie-bracket).

#### Identity commutator cyclic ladder

↑ **Parent:** [Commutator](#commutator)

For real-linear operators $[A,B]=I$ and a nonzero vector $y$ with $Ay=0$, induction gives $[A,B^i]=iB^{i-1}$, hence the displayed formula. Applying $A^n$ to a nontrivial finite dependence with highest term $c_nB^ny$ leaves $n!c_ny$, a contradiction. Thus $y,By,B^2y,\ldots$ are linearly independent, and their span is invariant under both operators. Characteristic zero is essential to the factorial argument.

#### Commutator expansion for exponential conjugation

↑ **Parent:** [Commutator](#commutator)

For bounded [linear operators](vector-space.md#linear-operator), or formally in an associative algebra,

$$
e^{\lambda A}Be^{-\lambda A}=\sum_{n\ge0}\frac{\lambda^n}{n!}\operatorname{ad}_A^n(B),\qquad \operatorname{ad}_A(B)=[A,B].
$$

Differentiate the two exponentials using the product rule: the result is $e^{\lambda A}[A,B]e^{-\lambda A}$. Induction gives the $n$th derivative $e^{\lambda A}\operatorname{ad}_A^n(B)e^{-\lambda A}$, and the [Taylor series](calculus.md#taylor-series) at zero proves the formula. For bounded operators convergence follows from $\|\operatorname{ad}_A^n(B)\|\le(2\|A\|)^n\|B\|$. For unbounded quantum operators, use a common invariant domain and justify the series there, or use the finite-dimensional system of commutators when their span closes.

##### Central-commutator exponential identity

↑ **Parent:** [Commutator expansion for exponential conjugation](#commutator-expansion-for-exponential-conjugation)

For finite-dimensional complex [linear operators](vector-space.md#linear-operator) with $C=[A,B]$ commuting with both $A$ and $B$, differentiating $e^{-vB}Ae^{vB}$ gives the constant derivative $C$. Hence $e^{-B}Ae^B=A+C$, and conjugating the [matrix exponential](linear-operator-theory.md#matrix-exponential) gives $e^{-B}e^{-A}e^B=e^{-A-C}$. Since $[A,C]=0$, multiplication by $e^A$ proves the identity. The commutator order determines the minus sign.

#### Trace of a matrix commutator

↑ **Parent:** [Commutator](#commutator)

The [matrix trace](linear-algebra.md#matrix-trace) of $[A,B]=AB-BA$ is zero, since $\operatorname{tr}(AB)=\sum_{i,j}A_{ij}B_{ji}=\operatorname{tr}(BA)$. This obstructs a matrix with nonzero trace from being a single [commutator](#commutator).

#### Commutator derivation identity

↑ **Parent:** [Commutator](#commutator)

Expand both sides using the definition of a [commutator](#commutator): the middle terms $BAC$ cancel, leaving $ABC-BCA$. Thus commutation with a fixed operator is a [derivation of an algebra](associative-algebra.md#derivation-of-an-algebra). In particular, $[A,[B,C]]=[[A,B],C]+[B,[A,C]]$, which gives a short way to derive a [Lie algebra](lie-algebra.md) representation from generator actions on an underlying algebra.

### Jacobi identity

↑ **Parent:** [Lie bracket](#lie-bracket)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobi_identity)

The Jacobi identity is

$$
[x,[y,z]]+[y,[z,x]]+[z,[x,y]]=0.
$$

## Abelian Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abelian_Lie_algebra)

A Lie algebra is abelian when every [Lie bracket](#lie-bracket) vanishes.

## Semidirect product of a Lie algebra and a module

↑ **Parent:** [Lie algebra](lie-algebra.md)

For a [Lie algebra representation](#lie-algebra-representation) of $\mathfrak g$ on $V$, the semidirect product $\mathfrak g\ltimes V$ is the vector space $\mathfrak g\oplus V$ with bracket

$$
[(x,v),(y,w)]=([x,y],xw-yv).
$$

The subspace $V$ is an abelian [ideal of a Lie algebra](#ideal-of-a-lie-algebra).

### Killing form of a semidirect product with a module

↑ **Parent:** [Semidirect product of a Lie algebra and a module](#semidirect-product-of-a-lie-algebra-and-a-module)

For a finite-dimensional representation $\rho:\mathfrak g\to\mathfrak{gl}(V)$,

$$
K_{\mathfrak g\ltimes V}((x,v),(y,w))
=K_{\mathfrak g}(x,y)+\operatorname{tr}(\rho(x)\rho(y)).
$$

In particular, $V$ lies in the radical of the Killing form.

## Ideal of a Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

A vector subspace $I\subseteq\mathfrak g$ is an ideal when $[\mathfrak g,I]\subseteq I$. It is therefore the kernel of a Lie-algebra quotient map.

### Quotient Lie algebra

↑ **Parent:** [Ideal of a Lie algebra](#ideal-of-a-lie-algebra)

For a [Lie algebra ideal](#ideal-of-a-lie-algebra) $I$, the quotient [vector space](vector-space.md) $\mathfrak g/I$ has [Lie bracket](#lie-bracket) $[x+I,y+I]=[x,y]+I$. The ideal condition makes this independent of representatives. Its [Lie algebra ideals](#ideal-of-a-lie-algebra) correspond to the ideals of $\mathfrak g$ containing $I$, by inverse image under the quotient [Lie algebra homomorphism](#lie-algebra-homomorphism).

## Derived series of a Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

The derived series is $\mathfrak g^{(0)}=\mathfrak g$ and $\mathfrak g^{(n+1)}=[\mathfrak g^{(n)},\mathfrak g^{(n)}]$.

### Derived algebra

↑ **Parent:** [Derived series of a Lie algebra](#derived-series-of-a-lie-algebra)

The derived algebra is the linear span of all [Lie brackets](#lie-bracket) $[x,y]$ in a [Lie algebra](lie-algebra.md). The [Jacobi identity](#jacobi-identity) makes it an [ideal of a Lie algebra](#ideal-of-a-lie-algebra). Its quotient is the largest [abelian Lie algebra](#abelian-lie-algebra) quotient of $\mathfrak g$.

#### Derived algebra nilpotence criterion

↑ **Parent:** [Derived algebra](#derived-algebra)

A finite-dimensional complex [Lie algebra](lie-algebra.md) is a [solvable Lie algebra](#solvable-lie-algebra) exactly when its [derived algebra](#derived-algebra) is a [nilpotent Lie algebra](#nilpotent-lie-algebra). The forward direction follows from the [Lie theorem](#lie-s-theorem) in the [Adjoint representation](#adjoint-representation-of-a-lie-algebra) and lifting nilpotence through its central kernel. The reverse direction follows because the [derived series of a Lie algebra](#derived-series-of-a-lie-algebra) after its first term is the [derived series of a Lie algebra](#derived-series-of-a-lie-algebra) of the [derived algebra](#derived-algebra).

### Solvable Lie algebra

↑ **Parent:** [Derived series of a Lie algebra](#derived-series-of-a-lie-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Solvable_Lie_algebra)

A Lie algebra is solvable when its derived series eventually becomes zero.

#### Diamond Lie algebra

↑ **Parent:** [Solvable Lie algebra](#solvable-lie-algebra)

The four-dimensional diamond Lie algebra is the [semidirect product of Lie algebras](#semidirect-product-of-lie-algebras) of the three-dimensional [Heisenberg Lie algebra](#heisenberg-lie-algebra) with a derivation having eigenvalues zero, one and minus one. With basis $c,d,p,q$, its nonzero brackets are $[d,p]=p$, $[d,q]=-q$, $[p,q]=c$. Its [derived series of a Lie algebra](#derived-series-of-a-lie-algebra) has dimensions four, three, one and zero. The symmetric form with $B(c,d)=B(p,q)=1$ and all other basis pairings zero is a [nondegenerate bilinear form](linear-algebra.md#nondegenerate-bilinear-form) and invariant. The alternating tensor $B([x,y],z)$ is the volume form on $\langle d,p,q\rangle$, verifying invariance.

#### Affine Lie algebra of the line

↑ **Parent:** [Solvable Lie algebra](#solvable-lie-algebra)

The two-dimensional [Lie algebra](lie-algebra.md) of infinitesimal dilations and translations of a line has a [basis](vector-space.md#basis) $h,e$ with $[h,e]=e$. Its [derived algebra](#derived-algebra) is the abelian line spanned by $e$, but every nontrivial term of its [lower central series of a Lie algebra](#lower-central-series-of-a-lie-algebra) is that same line. It is solvable and not nilpotent.

#### Radical of a Lie algebra

↑ **Parent:** [Solvable Lie algebra](#solvable-lie-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radical_of_a_Lie_algebra)

The solvable radical of a finite-dimensional [Lie algebra](lie-algebra.md) is its largest solvable [ideal of a Lie algebra](#ideal-of-a-lie-algebra). A Lie algebra is [semisimple](semisimple-lie-algebra.md) exactly when its solvable radical is zero.

<h4 id="lie-s-theorem">Lie's theorem</h4>

↑ **Parent:** [Solvable Lie algebra](#solvable-lie-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lie's_theorem)

Every finite-dimensional complex representation of a solvable Lie algebra has a common eigenvector. Equivalently, an irreducible finite-dimensional complex representation is one-dimensional; iterating gives simultaneous upper triangularization.

##### Infinite-dimensional simple module for the two-dimensional affine Lie algebra

↑ **Parent:** [Lie's theorem](#lie-s-theorem)

The [solvable Lie algebra](#solvable-lie-algebra) $\mathbb Cx\oplus\mathbb Cy$, with $[x,y]=y$, has an infinite-dimensional [Irreducible Lie algebra representation](#irreducible-lie-algebra-representation) on $\mathbb C[t]$: $xf(t)=tf(t)$ and $yf(t)=f(t-1)$. Indeed $[x,y]f=yf$. An [invariant subspace](representation-theory.md#invariant-subspace) is an ideal $p(t)\mathbb C[t]$ because it is invariant under multiplication by $t$. Shift invariance gives $p(t)\mid p(t-1)$, hence $p(t-1)=p(t)$ and $p$ is constant. This shows why the [Lie theorem](#lie-s-theorem) needs finite-dimensional representations, even when the algebra itself is finite-dimensional.

##### Simultaneous triangularization of a Lie algebra representation

↑ **Parent:** [Lie's theorem](#lie-s-theorem)

A [Lie algebra representation](#lie-algebra-representation) is simultaneously upper triangular precisely when it preserves a [complete flag](vector-space.md#complete-flag), with $\dim V_j=j$. A [basis](vector-space.md#basis) adapted to the invariant flag makes every representing matrix upper triangular. For a complex finite-dimensional representation of a [solvable Lie algebra](#solvable-lie-algebra), the [Lie theorem](#lie-s-theorem) provides a common [eigenvector](linear-operator-theory.md#eigenvector); iteration on the [quotient representations](representation-theory.md#quotient-representation) constructs the flag.

##### Failure of Lie theorem in positive characteristic

↑ **Parent:** [Lie's theorem](#lie-s-theorem)

In a [field](algebra.md#field) of [characteristic](algebra.md#characteristic-of-a-field) $p$, take a [basis](vector-space.md#basis) $e_0,\ldots,e_{p-1}$, and let $xe_j=e_{j-1}$ with indices modulo $p$, while $ye_j=je_j$. Then $[x,y]=x$, so $kx+ky$ is a [solvable Lie algebra](#solvable-lie-algebra), but the distinct [eigenvalues](linear-operator-theory.md#eigenvalue) of $y$ force any common [eigenvector](linear-operator-theory.md#eigenvector) to be a coordinate vector, and $x$ cyclically permutes those vectors. There is consequently no common [eigenvector](linear-operator-theory.md#eigenvector), even over an [algebraically closed field](algebra.md#algebraically-closed-field).

#### Cartan solvability criterion

↑ **Parent:** [Solvable Lie algebra](#solvable-lie-algebra)

This is the solvability test in [Cartan's criterion](#cartan-s-criterion), distinct from its semisimplicity test.

A complex Lie subalgebra $\mathfrak h\subseteq\mathfrak{gl}(V)$ is solvable if

$$
\operatorname{tr}(xy)=0
$$

for every $x\in[\mathfrak h,\mathfrak h]$ and $y\in\mathfrak h$. For an abstract Lie algebra, this is equivalent to $\kappa(\mathfrak h,[\mathfrak h,\mathfrak h])=0$.

##### Conjugate-spectrum proof of Cartan solvability

↑ **Parent:** [Cartan solvability criterion](#cartan-solvability-criterion)

For $x$ in the [derived algebra](#derived-algebra) of a complex matrix [Lie algebra](lie-algebra.md) $L$, define $y$ by multiplication by $\overline\lambda$ on each [generalized eigenspace](linear-operator-theory.md#generalized-eigenspace) $V_\lambda$ of $x$. [Polynomial interpolation](numerical-analysis.md#polynomial-interpolation) and [adjoint compatibility of additive Jordan decomposition](linear-operator-theory.md#adjoint-compatibility-of-additive-jordan-decomposition) make $\operatorname{ad}y$ a [polynomial](polynomial.md) in $\operatorname{ad}x$ with zero constant term, so $[y,L]\subseteq[L,L]$. Trace orthogonality of $[L,L]$ and $L$ forces the displayed sum to vanish. Thus $x$ is a [nilpotent endomorphism](linear-operator-theory.md#nilpotent-linear-map), and the [Engel theorem](#engel-s-theorem) implies solvability. The auxiliary $y$ and the Jordan components are not required to lie in $L$.

## Center of a Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

Like the [center of a group](group-theory.md#center-of-a-group), the Lie-algebra center consists of elements commuting with every element; here commutation means vanishing of the Lie bracket.

The center is $Z(\mathfrak g)=\{z:[z,x]=0\text{ for every }x\in\mathfrak g\}$.

### Central ideal

↑ **Parent:** [Center of a Lie algebra](#center-of-a-lie-algebra)

A central ideal is a [linear subspace](vector-space.md#vector-subspace) of the [center of a Lie algebra](#center-of-a-lie-algebra). It is a [Lie algebra ideal](#ideal-of-a-lie-algebra) because its [Lie bracket](#lie-bracket) with every element is zero. Passing to the [quotient Lie algebra](#quotient-lie-algebra) removes this central subspace. For $\mathfrak{sl}_p$ in [characteristic](algebra.md#characteristic-of-a-field) $p$, the identity matrix has zero [trace](linear-algebra.md#matrix-trace) and spans a central ideal.

## Lower central series of a Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

The lower central series is defined by $\gamma_1(\mathfrak g)=\mathfrak g$ and $\gamma_{i+1}(\mathfrak g)=[\mathfrak g,\gamma_i(\mathfrak g)]$.

### Nilpotent Lie algebra

↑ **Parent:** [Lower central series of a Lie algebra](#lower-central-series-of-a-lie-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nilpotent_Lie_algebra)

A [Lie algebra](lie-algebra.md) is nilpotent when its [lower central series](#lower-central-series-of-a-lie-algebra) eventually becomes zero.

#### Killing form of a nilpotent Lie algebra vanishes

↑ **Parent:** [Nilpotent Lie algebra](#nilpotent-lie-algebra)

Every [Adjoint representation](#adjoint-representation-of-a-lie-algebra) operator raises the [lower central series of a Lie algebra](#lower-central-series-of-a-lie-algebra) filtration. In a basis adapted to that finite filtration, all adjoint operators are strictly triangular. Their products have zero trace, so the [Killing form](#killing-form) vanishes. Consequently its [radical of the Killing form](#radical-of-the-killing-form) is the whole algebra. For strictly upper triangular matrices the filtration can be seen directly by the gap between the column and row indices.

// Target: algebra.bigb

#### Upper central series of a Lie algebra

↑ **Parent:** [Nilpotent Lie algebra](#nilpotent-lie-algebra)

Each term is the preimage of the [center of a Lie algebra](#center-of-a-lie-algebra) after quotienting by the preceding term. Equivalently, $Z_{i+1}=\{x:[\mathfrak g,x]\subseteq Z_i\}$. A [Lie algebra](lie-algebra.md) is nilpotent exactly when this series reaches the whole algebra after finitely many steps. For the [Heisenberg Lie algebra](#heisenberg-lie-algebra), the series is $0\subset\mathbb Cc\subset\mathfrak g$.

#### Two-dimensional subalgebra criterion for Lie algebra nilpotence

↑ **Parent:** [Nilpotent Lie algebra](#nilpotent-lie-algebra)

Over an [algebraically closed field](algebra.md#algebraically-closed-field), a finite-dimensional [Lie algebra](lie-algebra.md) is nilpotent exactly when every two-dimensional [Lie subalgebra](#lie-subalgebra) is abelian. A nonnilpotent [Adjoint representation](#adjoint-representation-of-a-lie-algebra) matrix has a nonzero [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda$ with [eigenvector](linear-operator-theory.md#eigenvector) $y$, so $[x,y]=\lambda y$ generates a nonabelian two-dimensional subalgebra. Conversely a subalgebra of a [nilpotent Lie algebra](#nilpotent-lie-algebra) is nilpotent, while a nonabelian two-dimensional algebra has a basis $u,v$ with $[u,v]=v$ and a nonnilpotent adjoint matrix. Algebraic closure is what guarantees the required eigenvector.

#### Normalizer condition for a nilpotent Lie algebra

↑ **Parent:** [Nilpotent Lie algebra](#nilpotent-lie-algebra)

Every proper [Lie subalgebra](#lie-subalgebra) $H$ of a finite-dimensional [nilpotent Lie algebra](#nilpotent-lie-algebra) is properly contained in its [normalizer](#normalizer-of-a-lie-subalgebra). Choose the first term of the lower central series contained in $H$; the preceding term contains an element outside $H$ that normalizes it.

<h4 id="engel-s-theorem">Engel's theorem</h4>

↑ **Parent:** [Nilpotent Lie algebra](#nilpotent-lie-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Engel's_theorem)

A finite-dimensional Lie algebra is nilpotent if and only if every adjoint map $\operatorname{ad}_x$ is nilpotent. A Lie algebra of nilpotent endomorphisms can be simultaneously represented by strictly upper triangular matrices.

##### Proof of Engel theorem by induction and normalizers

↑ **Parent:** [Engel's theorem](#engel-s-theorem)

First prove the [Engel lemma](#engel-lemma) by induction on the dimension of a [Lie algebra](lie-algebra.md) of [nilpotent endomorphisms](linear-operator-theory.md#nilpotent-linear-map). If $x^m=0$, then $\operatorname{ad}x=L_x-R_x$ on the endomorphism algebra has $(\operatorname{ad}x)^{2m-1}=0$, since left and right multiplication commute. Thus a proper [Lie subalgebra](#lie-subalgebra) $M$ acts nilpotently on $L/M$, and induction gives a nonzero class normalized by $M$. This proves the [Engel normalizer lemma](#engel-normalizer-lemma).

For a maximal proper $M$, its normalizer is all of $L$, so $M$ is an ideal. Maximality then forces $\dim L/M=1$, since every line in a Lie algebra is a subalgebra. Induction gives a nonzero common annihilator $W$ of $M$ in the representation space. Ideality makes $W$ stable under $L$. A generator $x$ of $L/M$ is nilpotent on $W$ and has nonzero kernel there, providing a vector killed by all of $L$. In the possibly nonfaithful quotient actions, apply induction to the image, whose dimension is at most $\dim M$.

Repeatedly apply this common-kernel statement to quotient representation spaces to obtain a complete flag with $xV_j\subseteq V_{j-1}$. Hence the operators are simultaneously strictly upper triangular. Applying this to the [Adjoint representation](#adjoint-representation-of-a-lie-algebra) shows that a finite-dimensional [Lie algebra](lie-algebra.md) whose every adjoint map is nilpotent has terminating [lower central series](group-theory.md#lower-central-series). Conversely, termination of that series immediately makes every adjoint map nilpotent. This proves [Engel theorem](#engel-s-theorem).

// Target: semisimple-lie-algebra.bigb

##### Engel lemma

↑ **Parent:** [Engel's theorem](#engel-s-theorem)

A finite-dimensional [Lie algebra representation](#lie-algebra-representation) in which every representing endomorphism is [nilpotent](linear-operator-theory.md#nilpotent-linear-map) has a nonzero vector annihilated by the entire Lie algebra. Applying this to the [Adjoint representation](#adjoint-representation-of-a-lie-algebra) is the key step in [Engel theorem](#engel-s-theorem).

###### Engel normalizer lemma

↑ **Parent:** [Engel lemma](#engel-lemma)

If $L$ is a finite-dimensional [Lie algebra](lie-algebra.md) of [nilpotent endomorphisms](linear-operator-theory.md#nilpotent-linear-map), every proper [Lie subalgebra](#lie-subalgebra) $M$ is strictly contained in its [normalizer of a Lie subalgebra](#normalizer-of-a-lie-subalgebra). The [Adjoint representation](#adjoint-representation-of-a-lie-algebra) of $M$ on $L/M$ consists of nilpotent maps by [nilpotence of commutation by a nilpotent endomorphism](linear-operator-theory.md#nilpotence-of-commutation-by-a-nilpotent-endomorphism). In the inductive proof of [Engel theorem](#engel-s-theorem), the lower-dimensional [Engel lemma](#engel-lemma) gives a nonzero class $y+M$ with $[M,y]\subseteq M$. A maximal proper $M$ is consequently an [ideal of a Lie algebra](#ideal-of-a-lie-algebra) of codimension one.

## Lie algebra homomorphism

↑ **Parent:** [Lie algebra](lie-algebra.md)

A Lie algebra homomorphism is a [linear map](vector-space.md#linear-map) $f$ satisfying $f([x,y])=[f(x),f(y)]$.

### Integration of a Lie algebra homomorphism

↑ **Parent:** [Lie algebra homomorphism](#lie-algebra-homomorphism)

For a connected [simply connected](algebraic-topology.md#simply-connected-space) source [Lie group](lie-theory.md#lie-group), every [Lie algebra homomorphism](#lie-algebra-homomorphism) integrates uniquely to a [Lie group homomorphism](lie-theory.md#lie-group-homomorphism). Along a path $\gamma$ from the identity, transport its left logarithmic velocity by $\theta$ and solve the corresponding left-invariant differential equation in the target. The [Maurer-Cartan equation](lie-theory.md#maurer-cartan-equation) and preservation of brackets make the endpoint invariant under fixed-endpoint [homotopies](algebraic-topology.md#homotopy). Simple connectedness removes path dependence, and path concatenation proves multiplicativity.

#### Period obstruction to integration of a Lie algebra homomorphism

↑ **Parent:** [Integration of a Lie algebra homomorphism](#integration-of-a-lie-algebra-homomorphism)

For a connected source, first integrate on its [universal covering Lie group](lie-theory.md#universal-covering-lie-group). The resulting map descends to the original [group](group.md) exactly when it kills the discrete kernel of the [covering map](algebraic-topology.md#covering-space). For the [circle group](lie-theory.md#circle-group), a real-linear map $t\mapsto ct$ integrates to a circle [endomorphism](algebra.md#endomorphism) exactly when $c\in\mathbb Z$, since $2\pi\mathbb Z$ must map into itself. This is a global period condition invisible to the zero bracket of the circle's [Lie algebra](lie-algebra.md).

### Differential of a Lie group homomorphism preserves Lie brackets

↑ **Parent:** [Lie algebra homomorphism](#lie-algebra-homomorphism)

For a smooth homomorphism of [Lie groups](lie-theory.md#lie-group), naturality gives $f(\exp X)=\exp(df_eX)$. Therefore $\log(f(g))=df_e(\log g)$ locally. Apply this to the [group commutator](group.md#group-commutator) and differentiate its two curve parameters to obtain the displayed identity for the [Lie bracket from local group commutators](#lie-bracket-from-local-group-commutators). In particular the differential of a group representation is a [Lie algebra representation](#lie-algebra-representation).

### Lie algebra representation

↑ **Parent:** [Lie algebra homomorphism](#lie-algebra-homomorphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lie_algebra_representation)

A representation of $\mathfrak g$ on a [vector space](vector-space.md) $V$ is a [Lie algebra homomorphism](#lie-algebra-homomorphism) $\rho:\mathfrak g\to\mathfrak{gl}(V)$.

#### Representation ring of a semisimple Lie algebra

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

The representation ring of finite-dimensional modules for a complex [semisimple Lie algebra](semisimple-lie-algebra.md) is the abelian group generated by module classes, with $[V\oplus U]=[V]+[U]$, and multiplication $[V][U]=[V\otimes U]$. [Weyl complete reducibility theorem](semisimple-lie-algebra.md#weyl-complete-reducibility-theorem) makes the classes of [irreducible representations](representation-theory.md#irreducible-representation) a free integral basis. The [formal character](semisimple-lie-algebra.md#formal-character-of-a-weight-module) map identifies this ring with the [Weyl group](semisimple-lie-algebra.md#weyl-group) invariant part of the [group ring of a weight lattice](semisimple-lie-algebra.md#group-ring-of-a-weight-lattice). Injectivity follows from distinct [highest weights](semisimple-lie-algebra.md#highest-weight-of-a-representation); surjectivity follows by subtracting the character with each maximal dominant weight, whose highest-weight coefficient is one, from a Weyl-invariant finite sum.

// Target: semisimple-lie-algebra.bigb

#### Defining representation of a matrix Lie algebra

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

For a [Lie subalgebra](#lie-subalgebra) $\mathfrak g\subseteq\mathfrak{gl}(V)$, its defining representation is its given action on the [vector space](vector-space.md) $V$. The [Lie bracket](#lie-bracket) identity $[X,Y]v=X(Yv)-Y(Xv)$ verifies the representation property. For the [special linear Lie algebra](semisimple-lie-algebra.md#special-linear-lie-algebra), diagonal trace-zero matrices have coordinate [weights of a representation](semisimple-lie-algebra.md#weight-of-a-representation) $L_i$ on the standard basis; for a [Special orthogonal Lie algebra](semisimple-lie-algebra.md#special-orthogonal-lie-algebra), the same action preserves the defining symmetric [bilinear form](linear-algebra.md#bilinear-form).

#### Hermitian quantum generator convention

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

For a unitary derived representation $\rho$, its generators are anti-Hermitian. Define Hermitian observables $H_X=i\rho(X)$; then their ordinary operator [commutator](#commutator) is $[H_X,H_Y]=iH_{[X,Y]}$. Thus real [Lie algebra](lie-algebra.md) structure constants and Hermitian-operator commutation relations differ by an $i$. Products in a [universal enveloping algebra](#universal-enveloping-algebra) require one conversion factor for every generator. In particular, the abstract bilinear Pauli-Lubanski element has representation image minus the pseudovector formed from the Hermitian physical generators.

#### Lie algebra representation homomorphism

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

A linear map between [Lie algebra representations](#lie-algebra-representation) is a representation homomorphism when it commutes with the action of every element. Its [kernel](linear-algebra.md#kernel-of-a-linear-map) and [image of a linear map](vector-space.md#image-of-a-linear-map) are invariant subspaces. This is a map of modules, distinct from a [Lie algebra homomorphism](#lie-algebra-homomorphism) between the acting algebras themselves.

#### Exterior-power Lie algebra representation

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

A [Lie algebra representation](#lie-algebra-representation) on $V$ induces one on each [exterior power](linear-algebra.md#exterior-power) by acting on every factor and summing. The [tensor product of Lie algebra representations](#tensor-product-of-lie-algebra-representations) preserves the defining alternating relations, so this descends to the quotient in every [characteristic of a field](algebra.md#characteristic-of-a-field). In [characteristic two](algebra.md#characteristic-two) define the [exterior algebra](linear-algebra.md#exterior-algebra) by the relations $v\wedge v=0$, rather than by dividing a tensor antisymmetrizer by $2$.

#### Nilpotent Lie algebras need not act nilpotently

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

The [abelian Lie algebra](#abelian-lie-algebra) $kI\subseteq\operatorname{End}(V)$, for $V\ne0$, is a [nilpotent Lie algebra](#nilpotent-lie-algebra) but contains the nonnilpotent [identity map](function.md#identity-function). Thus nilpotence of the abstract [Lie algebra](lie-algebra.md) does not imply that a particular [Lie algebra representation](#lie-algebra-representation) consists of [nilpotent endomorphisms](linear-operator-theory.md#nilpotent-linear-map). [Engel theorem](#engel-s-theorem) requires nilpotence of every represented endomorphism to obtain strict upper triangularity.

#### Tensor product of Lie algebra representations

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

The [tensor product](linear-algebra.md#tensor-product) of [Lie algebra representations](#lie-algebra-representation) has action $x(v\otimes w)=xv\otimes w+v\otimes xw$. The [Lie algebra representation](#lie-algebra-representation) identity follows because operators on the two different tensor factors commute. This action descends to [exterior powers](linear-algebra.md#exterior-power) and [symmetric powers](linear-algebra.md#symmetric-power).

<h5 id="su-3-triplet-octet-decomposition">SU(3) triplet-octet decomposition</h5>

↑ **Parent:** [Tensor product of Lie algebra representations](#tensor-product-of-lie-algebra-representations)

The summands have [Dynkin labels](semisimple-lie-algebra.md#dynkin-label) $(2,1)$, $(0,2)$ and $(1,0)$. Convolving the triplet and octet [weight diagrams](semisimple-lie-algebra.md#weight-diagram) and applying [highest-weight character subtraction](semisimple-lie-algebra.md#highest-weight-character-subtraction) removes these three characters in that order. Their dimensions $15+6+3=24$ match the product.

// Target: quantum-field-theory.bigb

##### sl2 tensor product of cubic and quadratic symmetric powers

↑ **Parent:** [Tensor product of Lie algebra representations](#tensor-product-of-lie-algebra-representations)

For the defining two-dimensional [sl2 Lie algebra](semisimple-lie-algebra.md#sl2-lie-algebra) module with coordinates $x,y$, put $u_{ij}=x^{3-i}y^i\otimes x^{2-j}y^j$. Its three [highest-weight vectors](semisimple-lie-algebra.md#highest-weight-vector) are $u_{00}$, $u_{10}-u_{01}$ and $u_{20}-2u_{11}+u_{02}$, of weights five, three and one. Lowering the last once gives $u_{30}-2u_{21}+u_{12}$, an explicit second vector of its two-dimensional irreducible summand.

##### Action map of a Lie algebra representation

↑ **Parent:** [Tensor product of Lie algebra representations](#tensor-product-of-lie-algebra-representations)

Give $\mathfrak g$ its [Adjoint representation](#adjoint-representation-of-a-lie-algebra). The representation identity gives $a(y\cdot(x\otimes v))=[y,x]v+xyv=y(xv)$, so the action map is a [Lie algebra representation homomorphism](#lie-algebra-representation-homomorphism). For a nontrivial simple module it is surjective. If the acting algebra is semisimple and the module is finite dimensional, [Weyl complete reducibility theorem](semisimple-lie-algebra.md#weyl-complete-reducibility-theorem) splits the surjection and makes $V$ a direct summand.

###### Action summand can fail for an infinite-dimensional simple module

↑ **Parent:** [Action map of a Lie algebra representation](#action-map-of-a-lie-algebra-representation)

Take the [Verma module](semisimple-lie-algebra.md#verma-module) for the [sl2 Lie algebra](semisimple-lie-algebra.md#sl2-lie-algebra) of highest weight $-2$, with basis $v_m$ and $fv_m=v_{m+1}$, $hv_m=(-2-2m)v_m$, $ev_m=-m(m+1)v_{m-1}$. It is simple. In $\mathfrak{sl}_2\otimes V$, the highest vectors of weight $-2$ are multiples of $w=e\otimes v_1-h\otimes v_0=f(e\otimes v_0)$. Every homomorphism to $V$ kills $e\otimes v_0$, whose weight is zero, and hence kills $w$. Every embedded copy of $V$ would have its highest vector proportional to $w$, so no projection onto such a copy can exist. Thus semisimplicity of the Lie algebra alone does not provide an action summand in infinite dimension.

##### Tensor product of the standard representation with its exterior square

↑ **Parent:** [Tensor product of Lie algebra representations](#tensor-product-of-lie-algebra-representations)

For $V=\mathbb C^n$, $n\ge3$, the [tensor product of Lie algebra representations](#tensor-product-of-lie-algebra-representations) for the [special linear Lie algebra](semisimple-lie-algebra.md#special-linear-lie-algebra) splits as displayed. The [exterior product](linear-algebra.md#exterior-product) map $v\otimes(u\wedge w)\mapsto v\wedge u\wedge w$ has an equivariant right inverse obtained by dividing its three-term alternating insertion by three. Its [kernel](linear-algebra.md#kernel-of-a-linear-map) is the [Schur functor](lie-theory.md#schur-functor) of shape $(2,1)$, with [highest weight](semisimple-lie-algebra.md#highest-weight-of-a-representation) $\omega_1+\omega_2$ and [dimension](vector-space.md#dimension-vector-space) $n(n^2-1)/3$. The other summand has [highest weight](semisimple-lie-algebra.md#highest-weight-of-a-representation) $\omega_3$ for $n\ge4$ and is trivial for $n=3$.

The [weight space](semisimple-lie-algebra.md#weight-space) of $2\varepsilon_i+\varepsilon_j$ has [dimension](vector-space.md#dimension-vector-space) one when $i\ne j$. The [weight space](semisimple-lie-algebra.md#weight-space) of $\varepsilon_i+\varepsilon_j+\varepsilon_k$ has [dimension](vector-space.md#dimension-vector-space) three for distinct indices. Restricting these functionals to the traceless diagonal [Cartan subalgebra](semisimple-lie-algebra.md#cartan-subalgebra) creates no additional coincidences; for $n=3$ the latter weight is zero.

##### sl3 highest-weight tensor rule

↑ **Parent:** [Tensor product of Lie algebra representations](#tensor-product-of-lie-algebra-representations)

For the complex [special linear Lie algebra](semisimple-lie-algebra.md#special-linear-lie-algebra) $\mathfrak{sl}_3$, tensoring an irreducible [highest-weight representation](semisimple-lie-algebra.md#highest-weight-representation) by the defining representation gives the displayed sum, omitting terms with negative [Dynkin labels](semisimple-lie-algebra.md#dynkin-label). It follows by multiplying its [Weyl character formula](semisimple-lie-algebra.md#weyl-character-formula) by $x_1+x_2+x_3$. In particular $\Gamma_{2,1}\otimes\Gamma_{1,0}=\Gamma_{3,1}\oplus\Gamma_{1,2}\oplus\Gamma_{2,0}$, with dimensions $24+15+6=45$.

#### Integration of a Lie-algebra representation

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

For a finite-dimensional real [Lie algebra](lie-algebra.md), a finite-dimensional [Lie algebra representation](#lie-algebra-representation) integrates uniquely to a smooth representation of the connected [simply connected](algebraic-topology.md#simply-connected-space) [Lie group](lie-theory.md#lie-group) with that [Lie algebra](lie-algebra.md). For another connected group with the same [Lie algebra](lie-algebra.md), integration is possible exactly when the representation of its universal cover is trivial on the covering kernel. This separates local Lie-algebra classification from global representation restrictions.

#### Lie-invariant bilinear form

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

A [bilinear form](linear-algebra.md#bilinear-form) on a [Lie algebra representation](#lie-algebra-representation) is invariant when it satisfies the displayed identity. Equivalently, $T_B(v)=B(v,-)$ is an [intertwining operator](representation-theory.md#intertwining-operator) from the representation to its [dual Lie algebra representation](#dual-lie-algebra-representation). For a finite-dimensional [irreducible representation](representation-theory.md#irreducible-representation) over an [algebraically closed field](algebra.md#algebraically-closed-field), any nonzero such form is [nondegenerate](linear-algebra.md#nondegenerate-bilinear-form), and the [Schur lemma](representation-theory.md#schur-s-lemma) makes all invariant forms proportional. In [characteristic](algebra.md#characteristic-of-a-field) different from two, transposing twice then proves that the form is a [symmetric bilinear form](linear-algebra.md#symmetric-bilinear-form) or an [alternating bilinear form](linear-algebra.md#alternating-bilinear-form).

#### Dual Lie algebra representation

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

The dual of a [Lie algebra representation](#lie-algebra-representation) on $V$ acts on its [dual space](linear-algebra.md#dual-space) by $(x\phi)(v)=-\phi(xv)$. The minus sign makes this a [Lie algebra homomorphism](#lie-algebra-homomorphism): taking transposes reverses the order in a [commutator](#commutator). It is the infinitesimal version of the [dual representation](representation-theory.md#dual-representation) of a [group](group.md).

##### Highest weight of a dual representation

↑ **Parent:** [Dual Lie algebra representation](#dual-lie-algebra-representation)

For a finite-dimensional irreducible representation $L(\lambda)$ of a complex [semisimple Lie algebra](semisimple-lie-algebra.md), its [dual Lie algebra representation](#dual-lie-algebra-representation) has [highest weight](semisimple-lie-algebra.md#highest-weight-of-a-representation) $-w_0\lambda$, where $w_0$ is the [longest Weyl-group element](semisimple-lie-algebra.md#longest-weyl-group-element). Indeed duality negates all [weights](semisimple-lie-algebra.md#weight-representation-theory), and $w_0\lambda$ is the lowest weight of the original module. In particular $w_0=-I$ makes every such irreducible module self-dual.

#### Trivial Lie algebra representation

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

The trivial representation sends every element of the [Lie algebra](lie-algebra.md) to the zero linear map. For a complex [semisimple Lie algebra](semisimple-lie-algebra.md), the irreducible representation of [highest weight](semisimple-lie-algebra.md#highest-weight-of-a-representation) zero is the one-dimensional trivial representation.

#### Hom representation

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

For [Lie algebra representations](#lie-algebra-representation) $V$ and $W$, the Hom representation on $\operatorname{Hom}(V,W)$ is

$$
(x\cdot f)(v)=x\cdot f(v)-f(x\cdot v).
$$

Its invariant vectors are exactly the intertwining maps.

#### Automorphism of a Lie algebra

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

An automorphism of a Lie algebra is an invertible linear map $f:\mathfrak g\to\mathfrak g$ satisfying $f([X,Y])=[f(X),f(Y)]$.

#### Branching rule

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Branching_rule)

A branching rule decomposes a representation into irreducible representations after restriction from a Lie group or Lie algebra to a subgroup or subalgebra.

##### Adjoint branching to root sl2 subalgebras in rank two

↑ **Parent:** [Branching rule](#branching-rule)

A [root string](semisimple-lie-algebra.md#root-string) of length $\Lambda+1$ gives an irreducible [sl2 Lie algebra](semisimple-lie-algebra.md#sl2-lie-algebra) module $R(\Lambda)$ when restricting the [Adjoint representation](#adjoint-representation-of-a-lie-algebra) to the [sl2 subalgebra associated with a root](semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root). Include also the root's own $R(2)$ and one commuting Cartan direction $R(0)$. For $A_2$ either simple root gives $R(2)\oplus2R(1)\oplus R(0)$. For $B_2$, the long root gives $R(2)\oplus2R(1)\oplus3R(0)$ and the short root gives $3R(2)\oplus R(0)$. For $G_2$, the long root gives $R(2)\oplus4R(1)\oplus3R(0)$ and the short root gives $R(2)\oplus2R(3)\oplus3R(0)$.

#### Structure constant of a Lie algebra

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

For a basis $(T_a)$ of a Lie algebra, its structure constants are defined by $[T_a,T_b]=f_{ab}{}^cT_c$.

##### Three-dimensional Lie algebra structure decomposition

↑ **Parent:** [Structure constant of a Lie algebra](#structure-constant-of-a-lie-algebra)

An oriented three-dimensional [Lie algebra](lie-algebra.md) has its antisymmetric structure constants encoded by the displayed matrix, whose symmetric part is $n^{bd}$ and whose antisymmetric part uniquely defines the covector $a_e$. In a volume-normalized basis, the inverse is $C_a{}^b{}_c=\frac12\epsilon_{acd}n^{bd}+\frac12(\delta_c^b a_a-\delta_a^b a_c)$. The only independent triple in the [Jacobi identity](#jacobi-identity) has coefficient $-\frac12n^{be}a_e$, so Jacobi holds exactly when $na=0$. This decomposition is useful in classifying three-dimensional [Lie algebras](lie-algebra.md).

##### Antisymmetry of Killing-lowered structure constants

↑ **Parent:** [Structure constant of a Lie algebra](#structure-constant-of-a-lie-algebra)

Lower the output index of the [structure constants of a Lie algebra](#structure-constant-of-a-lie-algebra) with its [Killing form](#killing-form). The [Lie bracket](#lie-bracket) makes the result antisymmetric in the first two indices, while invariance gives $\kappa([t_a,t_b],t_c)=\kappa(t_a,[t_b,t_c])$, making it antisymmetric in the last two indices. These two adjacent transpositions imply total antisymmetry. Nondegeneracy of the [Killing form](#killing-form) is unnecessary.

// Target: lie-theory.bigb

#### Faithful Lie algebra representation

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

A [Lie algebra representation](#lie-algebra-representation) is faithful when its representing homomorphism is [injective](algebra.md#injective-function).

<h5 id="ado-s-theorem">Ado's theorem</h5>

↑ **Parent:** [Faithful Lie algebra representation](#faithful-lie-algebra-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ado's_theorem)

Every finite-dimensional [Lie algebra](lie-algebra.md) over a [field](algebra.md#field) of [characteristic zero](algebra.md#characteristic-zero) has a finite-dimensional faithful [Lie algebra representation](#lie-algebra-representation). Thus it embeds as a Lie subalgebra of a [matrix algebra](associative-algebra.md#matrix-algebra), using the [matrix commutator](#commutator) as bracket. Faithfulness is crucial for detecting central elements: the [Adjoint representation](#adjoint-representation-of-a-lie-algebra) alone kills the [center of a Lie algebra](#center-of-a-lie-algebra).

#### Irreducible Lie algebra representation

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

A nonzero [Lie algebra representation](#lie-algebra-representation) is irreducible when it has no proper nonzero invariant [subspace](vector-space.md#vector-subspace).

#### Adjoint representation of a Lie algebra

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

The adjoint representation is $\operatorname{ad}_x(y)=[x,y]$. For a semisimple [Lie algebra](lie-algebra.md), its nonzero weights are the roots and its zero-weight space is the [Cartan subalgebra](semisimple-lie-algebra.md#cartan-subalgebra).

<h5 id="adjoint-representation-of-su-3">Adjoint representation of SU(3)</h5>

↑ **Parent:** [Adjoint representation of a Lie algebra](#adjoint-representation-of-a-lie-algebra)

The complex [Adjoint representation](#adjoint-representation-of-a-lie-algebra) of [SU(3)](topological-group.md#su-3-group) is the action by conjugation on traceless $3\times3$ matrices. With $H_1=\operatorname{diag}(1,-1,0)$ and $H_2=\operatorname{diag}(0,1,-1)$, its [highest-weight vector](semisimple-lie-algebra.md#highest-weight-vector) is $E_{13}$ of [Dynkin labels](semisimple-lie-algebra.md#dynkin-label) $(1,1)$. The six off-diagonal matrix units have weights $(2,-1),(-2,1),(-1,2),(1,-2),(1,1),(-1,-1)$, and the two-dimensional [Cartan subalgebra](semisimple-lie-algebra.md#cartan-subalgebra) has weight zero. In coordinates $(h_1,(h_1+2h_2)/\sqrt3)$, the [weight diagram](semisimple-lie-algebra.md#weight-diagram) is a regular hexagon together with a central point of [weight multiplicity](semisimple-lie-algebra.md#weight-multiplicity) two. This representation describes both the [gluon](standard-model.md#gluon) colour multiplet and the approximate flavour [baryon octet](standard-model.md#baryon-octet), under different physical [SU(3)](topological-group.md#su-3-group) symmetries.

<h6 id="tensor-square-of-the-su-3-adjoint-representation">Tensor square of the SU(3) adjoint representation</h6>

↑ **Parent:** [Adjoint representation of SU(3)](#adjoint-representation-of-su-3)

For traceless matrices $T,S$ transforming by conjugation under [SU(3)](topological-group.md#su-3-group), the [trace](linear-algebra.md#matrix-trace) $\operatorname{tr}(TS)$ supplies a singlet, the [commutator](#commutator) $[T,S]$ an antisymmetric octet, and the traceless anticommutator a symmetric octet. Symmetrizing the two upper and two lower indices and removing traces supplies the 27. Contracting an antisymmetric lower pair with the invariant alternating tensor and symmetrizing the remaining three upper indices supplies the 10, and the conjugate construction supplies the conjugate 10. These nonzero equivariant maps exhaust the dimensions: the symmetric part has $36=1+8+27$, the antisymmetric part $28=8+10+10$.

##### Killing form

↑ **Parent:** [Adjoint representation of a Lie algebra](#adjoint-representation-of-a-lie-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Killing_form)

The Killing form is

$$
\kappa(X,Y)=\operatorname{Tr}(\operatorname{ad}_X\operatorname{ad}_Y).
$$

It is symmetric and invariant: $\kappa([X,Y],Z)=\kappa(X,[Y,Z])$.

###### Killing form of the general linear Lie algebra

↑ **Parent:** [Killing form](#killing-form)

For the [general linear Lie algebra](#general-linear-lie-algebra) of all $n\times n$ matrices over a [field](algebra.md#field) of [characteristic zero](algebra.md#characteristic-zero), write $\operatorname{ad}_X=L_X-R_X$ on the matrix space. The traces of $L_XL_Y$ and $R_XR_Y$ are $n\operatorname{tr}(XY)$, whereas both mixed traces are $\operatorname{tr}X\operatorname{tr}Y$. Expanding gives the displayed [Killing form](#killing-form). Its radical is the scalar matrices because $\kappa(X,Y)=0$ for every $Y$ forces $nX-\operatorname{tr}(X)I=0$. Thus the full general linear algebra is not semisimple, even though its traceless summand is semisimple for $n\ge2$.

// Target: lie-theory.bigb

###### Killing-form invariance under a Lie-group adjoint action

↑ **Parent:** [Killing form](#killing-form)

Every Lie algebra automorphism $S$ obeys $\operatorname{ad}_{SX}=S\operatorname{ad}_XS^{-1}$. The [cyclic property of the trace](linear-algebra.md#cyclic-property-of-the-trace) therefore makes the [Killing form](#killing-form) invariant under $S$. For a matrix [Lie group](lie-theory.md#lie-group), $S=\operatorname{Ad}_g$ is conjugation by $g$, proving the displayed identity even when the group is disconnected. This directly proves [gauge invariance](relativistic-quantum-field.md#gauge-invariance) of Killing-form contractions of adjoint fields.

###### Killing form for cyclic three-generator brackets

↑ **Parent:** [Killing form](#killing-form)

For $[e_1,e_2]=ae_3$, $[e_2,e_3]=be_1$, and $[e_3,e_1]=ce_2$, the [Adjoint representation](#adjoint-representation-of-a-lie-algebra) [matrices](vector-space.md#matrix) give the displayed [Killing form](#killing-form). Cross traces vanish. Nonzero $a,b,c$ make it nondegenerate and hence the algebra semisimple. If the three constants have the same sign it is negative-definite; mixed signs give signature $(2,1)$. In particular $(a,b,c)=(2,2,2)$ is the compact $\mathfrak{su}(2)$ case, whereas $(2,2,-2)$ is the split real traceless two-by-two algebra. This gives a direct [compactness criterion from the Killing form](#compactness-criterion-from-the-killing-form) in a small explicit example.

###### Orthogonal ideal splitting for a nondegenerate Killing form

↑ **Parent:** [Killing form](#killing-form)

For an [ideal of a Lie algebra](#ideal-of-a-lie-algebra) $I$ and nondegenerate [Killing form](#killing-form), invariance makes $I^\perp$ an ideal. An element of $I\cap I^\perp$ commutes with $I$, so the intersection is an abelian ideal. [Abelian ideals lie in the radical of the Killing form](#abelian-ideals-lie-in-the-radical-of-the-killing-form), forcing the intersection to vanish. Thus $\mathfrak g=I\oplus I^\perp$ as commuting ideals. Iterating minimal nonzero ideals gives the direct-sum formulation of a [semisimple Lie algebra](semisimple-lie-algebra.md).

###### Radical of the Killing form

↑ **Parent:** [Killing form](#killing-form)

The [radical of a bilinear form](linear-algebra.md#radical-of-a-bilinear-form) of the [Killing form](#killing-form) is the [ideal of a Lie algebra](#ideal-of-a-lie-algebra) $\{x:B(x,y)=0\text{ for all }y\}$. It is zero for a complex [semisimple Lie algebra](semisimple-lie-algebra.md). Every element of the [center of a Lie algebra](#center-of-a-lie-algebra) lies in this radical.

###### Compactness criterion from the Killing form

↑ **Parent:** [Killing form](#killing-form)

A finite-dimensional real [Lie algebra](lie-algebra.md) has negative-definite [Killing form](#killing-form) exactly when it is compact semisimple. In the compact direction, average an [inner product](linear-algebra.md#inner-product) over a compact group; all adjoint maps are skew, so $\kappa(X,X)=-\|\operatorname{ad}_X\|^2$, and semisimplicity removes the center. Conversely, negative-definiteness gives the positive invariant metric $-\kappa$, embeds the faithful adjoint algebra in an orthogonal algebra, and nondegeneracy gives semisimplicity. This is an algebraic compactness criterion, not a claim that every global group with an Abelian compact-type algebra is compact.

###### Abelian ideals lie in the radical of the Killing form

↑ **Parent:** [Killing form](#killing-form)

If $\mathfrak a$ is an abelian [ideal of a Lie algebra](#ideal-of-a-lie-algebra), then $\operatorname{ad}_x\operatorname{ad}_y$ maps $\mathfrak g$ into $\mathfrak a$ and vanishes on $\mathfrak a$ whenever $x\in\mathfrak a$. Its trace is zero, so $\kappa(\mathfrak a,\mathfrak g)=0$. Every nonzero solvable ideal has a last nonzero term in its [derived series of a Lie algebra](#derived-series-of-a-lie-algebra), which is such an abelian ideal. Consequently a nondegenerate [Killing form](#killing-form) forces the [solvable radical](#radical-of-a-lie-algebra) to vanish.

###### Solvability of the radical of the Killing form

↑ **Parent:** [Killing form](#killing-form)

The radical $\mathfrak g^\perp=\{x:\kappa(x,\mathfrak g)=0\}$ of the Killing form is a solvable ideal. Invariance makes it an ideal, and the [Cartan solvability criterion](#cartan-solvability-criterion) applied to its adjoint image proves solvability.

###### Cartan criterion for semisimplicity

↑ **Parent:** [Killing form](#killing-form)

A finite-dimensional complex [Lie algebra](lie-algebra.md) is [semisimple](semisimple-lie-algebra.md) if and only if its [Killing form](#killing-form) is [nondegenerate](linear-algebra.md#nondegenerate-bilinear-form).

###### Killing radical is a solvable ideal

↑ **Parent:** [Cartan criterion for semisimplicity](#cartan-criterion-for-semisimplicity)

For a finite-dimensional complex [Lie algebra](lie-algebra.md) $L$, the radical $R$ of its [Killing form](#killing-form) is a [Lie algebra ideal](#ideal-of-a-lie-algebra) by invariance. For $x,y\in R$, their adjoint actions vanish on $L/R$, so $B_R(x,y)=B_L(x,y)=0$. The [Cartan solvability criterion](#cartan-solvability-criterion) makes the image $\operatorname{ad}_R(R)$ solvable; its kernel is the abelian center, so $R$ is solvable. A [semisimple Lie algebra](semisimple-lie-algebra.md) has no nonzero solvable ideal, forcing its Killing radical to vanish.

###### Uniqueness of an invariant bilinear form on a simple Lie algebra

↑ **Parent:** [Killing form](#killing-form)

Every invariant bilinear form on a finite-dimensional complex simple Lie algebra is a scalar multiple of its Killing form. A nondegenerate invariant form identifies the algebra with its dual; comparing this identification with the Killing form gives an endomorphism of the irreducible adjoint representation, so [Schur lemma](representation-theory.md#schur-s-lemma) makes it scalar.

###### Real-simple exception to uniqueness of the Killing form

↑ **Parent:** [Uniqueness of an invariant bilinear form on a simple Lie algebra](#uniqueness-of-an-invariant-bilinear-form-on-a-simple-lie-algebra)

The usual uniqueness theorem assumes a complex simple [Lie algebra](lie-algebra.md), or a real form with simple complexification. For a complex simple algebra regarded as real, both $\operatorname{Re}\kappa_{\mathbb C}$ and $\operatorname{Im}\kappa_{\mathbb C}$ define a real symmetric [invariant bilinear form on a Lie algebra](#invariant-bilinear-form-on-a-lie-algebra), and they are linearly independent. The real [Killing form](#killing-form) is $2\operatorname{Re}\kappa_{\mathbb C}$. For $\mathfrak{sl}_2(\mathbb C)$ and $H=\operatorname{diag}(1,-1)$, $\kappa_{\mathbb C}(H,H)=8$ and $\kappa_{\mathbb C}(H,iH)=8i$, proving the independence. This real algebra is simple: its real complexification is two complex simple ideals exchanged by conjugation, and a real ideal would complexify to a conjugation-stable sum of these ideals, hence either zero or the whole algebra.

###### Killing form of the special linear Lie algebra

↑ **Parent:** [Killing form](#killing-form)

For $\mathfrak{sl}_n(\mathbb C)$,

$$
\kappa(X,Y)=2n\operatorname{tr}(XY).
$$

##### Adjoint irreducibility of a simple Lie algebra

↑ **Parent:** [Adjoint representation of a Lie algebra](#adjoint-representation-of-a-lie-algebra)

Every invariant subspace of the [Adjoint representation of a Lie algebra](#adjoint-representation-of-a-lie-algebra) is an ideal. Hence the adjoint representation of a [simple Lie algebra](semisimple-lie-algebra.md#simple-lie-algebra) is irreducible.

#### Trace form of a Lie algebra representation

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

For a finite-dimensional [Lie algebra representation](#lie-algebra-representation) $\rho:\mathfrak g\to\mathfrak{gl}(V)$, its trace form is the symmetric bilinear form

$$
(x,y)_V=\operatorname{tr}(\rho(x)\rho(y)).
$$

It is invariant: $([x,y],z)_V=(x,[y,z])_V$.

##### Trace forms of solvable Lie algebras annihilate the derived algebra

↑ **Parent:** [Trace form of a Lie algebra representation](#trace-form-of-a-lie-algebra-representation)

For a finite-dimensional complex representation of a [solvable Lie algebra](#solvable-lie-algebra), the [Lie theorem](#lie-s-theorem) gives a basis in which all representing matrices are upper triangular. Commutators are strictly upper triangular, and their products with upper triangular matrices have zero [trace](linear-algebra.md#matrix-trace). Thus the [derived algebra](#derived-algebra) lies in the [radical of a bilinear form](linear-algebra.md#radical-of-a-bilinear-form). In particular, a nonabelian [solvable Lie algebra](#solvable-lie-algebra) can carry an [invariant bilinear form on a Lie algebra](#invariant-bilinear-form-on-a-lie-algebra) that is [nondegenerate](linear-algebra.md#nondegenerate-bilinear-form) without that form coming from a finite-dimensional representation trace.

// Target: semisimple-lie-algebra.bigb

##### Cubic trace tensor of a Lie algebra representation

↑ **Parent:** [Trace form of a Lie algebra representation](#trace-form-of-a-lie-algebra-representation)

The [cubic trace tensor of a Lie algebra representation](#cubic-trace-tensor-of-a-lie-algebra-representation) is cyclic by the [cyclic property of the trace](linear-algebra.md#cyclic-property-of-the-trace). It need not be fully antisymmetric. Its antisymmetric part in the first two arguments is fixed by the [Trace form of a Lie algebra representation](#trace-form-of-a-lie-algebra-representation):

$$
B(X,Y,Z)-B(Y,X,Z)=H([X,Y],Z).
$$

// Target: lie-theory.bigb

###### Killing-normalized contraction of a cubic trace tensor

↑ **Parent:** [Cubic trace tensor of a Lie algebra representation](#cubic-trace-tensor-of-a-lie-algebra-representation)

Lowering and raising [structure constants](algebra.md#structure-constant) with the [Killing form](#killing-form) gives $c_a{}^{mn}c_{mn}{}^r=-\delta_a{}^r$. Since $c_a{}^{mn}$ is antisymmetric in $m,n$, only the [commutator](#commutator) part of the [cubic trace tensor of a Lie algebra representation](#cubic-trace-tensor-of-a-lie-algebra-representation) contributes, proving $c_a{}^{mn}B_{mnb}=-H_{ab}/2$. In an adapted compact basis with $\kappa_{ab}=-\delta_{ab}$ and $H_{ab}=-\mu\delta_{ab}$, the resulting sign is positive: $+\mu\delta_{ab}/2$. Defining the lowered structure constants with a positive Euclidean metric instead would reverse this sign.

// Target: lie-theory.bigb

###### Invariance identity for a cubic trace tensor

↑ **Parent:** [Cubic trace tensor of a Lie algebra representation](#cubic-trace-tensor-of-a-lie-algebra-representation)

The [trace](linear-algebra.md#matrix-trace) of a [commutator](#commutator) gives

$$
B([W,X],Y,Z)+B(X,[W,Y],Z)+B(X,Y,[W,Z])=0.
$$

In a basis, cyclicity converts this to $c_{da}{}^\ell B_{bc\ell}+c_{db}{}^\ell B_{ca\ell}+c_{dc}{}^\ell B_{ab\ell}=0$.

// Target: lie-theory.bigb

##### Positive trace index for a compact simple Lie algebra

↑ **Parent:** [Trace form of a Lie algebra representation](#trace-form-of-a-lie-algebra-representation)

For a nontrivial finite-dimensional [anti-Hermitian](linear-operator-theory.md#skew-hermitian-matrix) [Lie algebra representation](#lie-algebra-representation) of a [compact Lie algebra](#compact-lie-algebra) that is simple, its [Trace form of a Lie algebra representation](#trace-form-of-a-lie-algebra-representation) is a positive multiple of the [Killing form](#killing-form). Define $T$ by $H(X,Y)=\kappa(TX,Y)$. Invariance makes $T$ commute with the [Adjoint representation of a Lie algebra](#adjoint-representation-of-a-lie-algebra). Symmetry makes $T$ self-adjoint for $-\kappa$, so its [eigenspaces](linear-operator-theory.md#eigenspace) are ideals. Simplicity implies $T=\mu I$. The kernel of the representation is an ideal and hence vanishes; therefore $H(X,X)=-\operatorname{Tr}(d(X)^\dagger d(X))<0$ for nonzero $X$, proving $\mu>0$.

// Target: lie-theory.bigb

#### Trace trilinear form of a Lie algebra representation

↑ **Parent:** [Lie algebra representation](#lie-algebra-representation)

For a finite-dimensional representation $d$, the trilinear form $B(X,Y,Z)=\operatorname{Tr}(d(X)d(Y)d(Z))$ is invariant under simultaneous adjoint action. This follows by writing the sum of its three infinitesimal variations as the trace of a commutator.

## Heisenberg Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

The three-dimensional Heisenberg Lie algebra has a basis $a,b,c$ with $[a,b]=c$ and $c$ central. It is a two-step [nilpotent Lie algebra](#nilpotent-lie-algebra).

### Heisenberg group

↑ **Parent:** [Heisenberg Lie algebra](#heisenberg-lie-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heisenberg_group)

The real Heisenberg group consists of upper-unitriangular $3\times3$ real matrices. In coordinates $(q,r,s)$ its multiplication is $(q,r,s)(q',r',s')=(q+q',r+r',s+s'+qr')$.

#### Center quotient of the real Heisenberg group

↑ **Parent:** [Heisenberg group](#heisenberg-group)

In coordinates $h(x,y,z)=\left(\begin{smallmatrix}1&x&y\\0&1&z\\0&0&1\end{smallmatrix}\right)$, the [Heisenberg group](#heisenberg-group) law is $h(x,y,z)h(a,b,c)=h(x+a,y+b+xc,z+c)$. Commutation for every $(a,b,c)$ forces $xc=az$, hence $x=z=0$. The [center of a group](group-theory.md#center-of-a-group) is therefore the $y$-axis. The surjective [group homomorphism](group-theory.md#group-homomorphism) $h(x,y,z)\mapsto(x,z)$ has exactly this [kernel of a group homomorphism](group-theory.md#kernel-of-a-group-homomorphism), giving the stated [quotient group](group-theory.md#quotient-group) by the [first isomorphism theorem](group-theory.md#first-isomorphism-theorem).

#### Right-invariant coframe of the real Heisenberg group

↑ **Parent:** [Heisenberg group](#heisenberg-group)

For the [Heisenberg group](#heisenberg-group) law $(x,y,z)(a,b,c)=(x+a,y+b,z+c+xb)$, the right [Maurer-Cartan form](lie-theory.md#maurer-cartan-form) has coefficients $dx,dy,dz-y\,dx$. They satisfy $d\sigma^1=d\sigma^2=0$ and $d\sigma^3=\sigma^1\wedge\sigma^2$. A general [right-invariant Riemannian metric](lie-theory.md#right-invariant-riemannian-metric) is a constant positive-definite symmetric matrix in this coframe.

##### Killing frame for a right-invariant Heisenberg metric

↑ **Parent:** [Right-invariant coframe of the real Heisenberg group](#right-invariant-coframe-of-the-real-heisenberg-group)

Every [right-invariant Riemannian metric](lie-theory.md#right-invariant-riemannian-metric) on the [Heisenberg group](#heisenberg-group) has [Killing vector fields](general-relativity.md#killing-vector-field) $\partial_x$, $\partial_y+x\partial_z$ and $\partial_z$. Their [Lie brackets of vector fields](differential-geometry.md#lie-bracket-of-vector-fields) reproduce $[X,Y]=Z$ and the central relations. Their flows are right translations. The dual frame of the right-invariant coframe is different and has the opposite Lie-bracket sign.

#### Modular Heisenberg group

↑ **Parent:** [Heisenberg group](#heisenberg-group)

The modular Heisenberg group consists of upper-unitriangular $3\times3$ matrices over the [finite field](algebra.md#finite-field) $\mathbb F_p$. In coordinates $M(x,y,z)$, multiplication is $M(x,y,z)M(x\prime,y\prime,z\prime)=M(x+x\prime,y+y\prime+xz\prime,z+z\prime)$, and its order is $p^3$. Its [center of a group](group-theory.md#center-of-a-group) is $\{M(0,y,0)\}\cong C_p$; the [quotient group](group-theory.md#quotient-group) by the centre is $C_p\times C_p$, represented by the $x,z$ coordinates. The elementary generators $a=M(1,0,0)$, $b=M(0,0,1)$, $c=M(0,1,0)$ satisfy $a^p=b^p=c^p=e$, $aba^{-1}b^{-1}=c$, and $c$ central. For $p=2$, $(ab)^2=c$, so the whole group does not have exponent two.

#### Left-invariant frame of the real Heisenberg group

↑ **Parent:** [Heisenberg group](#heisenberg-group)

For multiplication $(x,y,z)(a,b,c)=(x+a,y+b,z+c+xb)$, the left-invariant frame is

$$
E_1=\partial_x,\qquad E_2=\partial_y+x\partial_z,\qquad E_3=\partial_z.
$$

Its [Lie brackets of vector fields](differential-geometry.md#lie-bracket-of-vector-fields) satisfy $[E_1,E_2]=E_3$ and the other basis brackets vanish.

##### Heisenberg horizontal distribution

↑ **Parent:** [Left-invariant frame of the real Heisenberg group](#left-invariant-frame-of-the-real-heisenberg-group)

The horizontal [smooth distribution](differential-geometry.md#distribution-differential-geometry) on the [real Heisenberg group](#heisenberg-group) is spanned by $E_1=\partial_x$ and $E_2=\partial_y+x\partial_z$. It is not an [involutive distribution](differential-geometry.md#involutive-distribution) because their bracket is $\partial_z$, but their brackets span the full tangent space. A horizontal curve satisfies $\dot x=\alpha$, $\dot y=\beta$, and $\dot z=x\beta$.

###### Smooth horizontal reachability in the real Heisenberg group

↑ **Parent:** [Heisenberg horizontal distribution](#heisenberg-horizontal-distribution)

Every point $(P_x,P_y,P_z)$ can be reached from the identity by a smooth curve tangent to the [Heisenberg horizontal distribution](#heisenberg-horizontal-distribution). Put $a=2(P_z-P_xP_y/2+P_x)$ and choose

$$
\alpha(t)=P_x+a\cos(2\pi t),\qquad
\beta(t)=P_y+2\pi\sin(2\pi t).
$$

Their integrals give $x(1)=P_x$, $y(1)=P_y$, and $z(1)=\int_0^1x(t)\beta(t)dt=P_xP_y/2-P_x+a/2=P_z$. The third coordinate measures the effect of the noncommuting horizontal directions; integrability would instead confine horizontal curves to a two-dimensional leaf.

#### Integer Heisenberg group

↑ **Parent:** [Heisenberg group](#heisenberg-group)

The integer Heisenberg group consists of upper-unitriangular three-by-three integer matrices. In coordinates $(x,y,z)$ its multiplication is

$$
(x,y,z)(x',y',z')=(x+x',y+y',z+z'+xy').
$$

It is the semidirect product $\mathbb Z^2\rtimes_A\mathbb Z$ for

$$
A=\begin{pmatrix}1&0\\1&1\end{pmatrix},
$$

and its [abelianization](group-theory.md#abelianization) is $\mathbb Z^2$.

##### Scaled Heisenberg lattice

↑ **Parent:** [Integer Heisenberg group](#integer-heisenberg-group)

In the [real Heisenberg group](#heisenberg-group) with multiplication $(x,y,z)(x',y',z')=(x+x',y+y',z+z'+xy')$, the displayed set is a discrete cocompact subgroup. Writing $a=(k,0,0)$, $b=(0,k,0)$, $c=(0,0,k)$ gives $[a,b]=c^k$ and $c$ central. Hence its [abelianization](group-theory.md#abelianization) is $\mathbb Z^2\oplus\mathbb Z/k$. The right quotient maps to $\mathbb R^2/k\mathbb Z^2$ by its first two coordinates; each fibre is the central circle $\mathbb R/k\mathbb Z$.

##### Commutator identity in the integer Heisenberg group

↑ **Parent:** [Integer Heisenberg group](#integer-heisenberg-group)

Write the [Integer Heisenberg group](#integer-heisenberg-group) with central generator $c=[a,b]$, so $ab=cba$. Moving $a$ successively past powers of $b$ gives

$$
a^r b^s a^{-r}b^{-s}=c^{rs}\qquad(r,s\in\mathbb Z).
$$

For positive exponents this follows by two inductions; inverses give the remaining signs. The representation $a=I+E_{12}$, $b=I+E_{23}$, $c=I+E_{13}$ checks the identity and shows $c$ has infinite order.

<h4 id="schrodinger-representation-of-the-heisenberg-group">Schrödinger representation of the Heisenberg group</h4>

↑ **Parent:** [Heisenberg group](#heisenberg-group)

On $L^2(\mathbb R)$, translations and multiplication by phases give the Schrödinger representation of the Heisenberg group. The central coordinate acts by an overall phase.

### Polynomial representation of the Heisenberg Lie algebra

↑ **Parent:** [Heisenberg Lie algebra](#heisenberg-lie-algebra)

On $\mathbb C[x]$, the operators $d/dx$, multiplication by $x$, and the identity satisfy $[d/dx,x]=1$. Sending $a,b,c$ to these operators gives a faithful irreducible infinite-dimensional representation of the [Heisenberg Lie algebra](#heisenberg-lie-algebra).

## Complexification of a Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

For a real Lie algebra $\mathfrak g$, its complexification is $\mathfrak g_{\mathbb C}=\mathfrak g\otimes_{\mathbb R}\mathbb C$ with the bracket extended complex-bilinearly.

### Complexification preserves semisimplicity

↑ **Parent:** [Complexification of a Lie algebra](#complexification-of-a-lie-algebra)

For a finite-dimensional real [Lie algebra](lie-algebra.md) $\mathfrak g$, the [solvable radical](#radical-of-a-lie-algebra) of its [complexification of a Lie algebra](#complexification-of-a-lie-algebra) is invariant under complex conjugation. Its real fixed subspace is a solvable ideal of $\mathfrak g$, and complexifying that fixed subspace recovers the whole radical. Conversely the complexification of any real solvable ideal is solvable. These inclusions prove the displayed identity; in particular $\mathfrak g$ is semisimple if and only if $\mathfrak g_{\mathbb C}$ is semisimple.

## Universal enveloping algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Universal_enveloping_algebra)

The universal enveloping algebra $U(\mathfrak g)$ is the associative algebra generated by $\mathfrak g$ subject to $xy-yx=[x,y]$. Its modules are the same as [Lie algebra representations](#lie-algebra-representation).

<h3 id="poincare-birkhoff-witt-theorem">Poincaré-Birkhoff-Witt theorem</h3>

↑ **Parent:** [Universal enveloping algebra](#universal-enveloping-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincaré–Birkhoff–Witt_theorem)

For an ordered basis $(x_i)$ of a [Lie algebra](lie-algebra.md) $\mathfrak g$, the ordered monomials $x_1^{a_1}\cdots x_n^{a_n}$ form a basis of $U(\mathfrak g)$. In particular, a triangular decomposition $\mathfrak g=\mathfrak n^-\oplus\mathfrak t\oplus\mathfrak n^+$ gives $U(\mathfrak g)\cong U(\mathfrak n^-)\otimes U(\mathfrak t)\otimes U(\mathfrak n^+)$ as vector spaces.

## Semisimple Lie algebra

↑ **Parent:** [Lie algebra](lie-algebra.md)

[This section is present in another page, follow this link to view it.](semisimple-lie-algebra.md)

<h4 id="graded-poincare-birkhoff-witt-theorem">Graded Poincaré–Birkhoff–Witt theorem</h4>

↑ **Parent:** [Poincaré-Birkhoff-Witt theorem](#poincare-birkhoff-witt-theorem)

For a [graded Lie algebra](#graded-lie-algebra) over [characteristic zero](algebra.md#characteristic-zero), the associated graded algebra of its [universal enveloping algebra](#universal-enveloping-algebra) under the word-length filtration is its [graded symmetric algebra](commutative-algebra.md#graded-symmetric-algebra). Ordered homogeneous monomials form a [basis](vector-space.md#basis), with exponent at most one on each odd Lie [basis](vector-space.md#basis) element. The defining graded commutation relations reorder every word, and the Jacobi identity resolves the triple-reordering ambiguities. In particular the [primitive elements of a Hopf algebra](algebra.md#primitive-element-of-a-hopf-algebra) of $U(L)$ are precisely $L$: in its associated graded algebra, a primitive polynomial of symmetric length greater than one would have a nonzero mixed term under the diagonal, which is impossible in [characteristic zero](algebra.md#characteristic-zero).

## ↑ Ancestors (6)

1. [Lie theory](lie-theory.md)
2. [Diagonal dominance](algebra.md#diagonal-dominance)
3. [Algebra](algebra.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (299)

- [Abelian Lie group](lie-theory.md#abelian-lie-group)
- [Additivity of the Lie exponential map](lie-theory.md#additivity-of-the-lie-exponential-map)
- [ADE gauge enhancement](string-theory.md#ade-gauge-enhancement)
- [Adjoint bundle](fiber-bundle.md#adjoint-bundle)
- [Adjoint-orbit criterion for maximal-torus conjugacy](lie-theory.md#adjoint-orbit-criterion-for-maximal-torus-conjugacy)
- [Adjoint representation of a Lie algebra](#adjoint-representation-of-a-lie-algebra)
- [Ado's theorem](#ado-s-theorem)
- [Affine current algebra](#affine-current-algebra)
- [Affine Lie algebra of the line](#affine-lie-algebra-of-the-line)
- [Alternating trilinear form](linear-algebra.md#alternating-trilinear-form)
- [Antisymmetry of a Lie bracket](#antisymmetry-of-a-lie-bracket)
- [Associated graded Lie algebra of a filtered group](associative-algebra.md#associated-graded-lie-algebra-of-a-filtered-group)
- [B2 weight lattice](semisimple-lie-algebra.md#b2-weight-lattice)
- [Bi-invariant pseudo-Riemannian metric](lie-theory.md#bi-invariant-pseudo-riemannian-metric)
- [Canonical torsion-free connection on a Lie group](lie-theory.md#canonical-torsion-free-connection-on-a-lie-group)
- [Carnot-Carathéodory distance](differential-geometry.md#carnot-caratheodory-distance)
- [Cartan criterion for semisimplicity](#cartan-criterion-for-semisimplicity)
- [Cartan's criterion](#cartan-s-criterion)
- [Cartan subalgebra](semisimple-lie-algebra.md#cartan-subalgebra)
- [Cartan three-form](lie-theory.md#cartan-three-form)
- [Central extension of a Lie algebra](#central-extension-of-a-lie-algebra)
- [Centralizer of an element of a Lie algebra](#centralizer-of-an-element-of-a-lie-algebra)
- [Coadjoint representation](lie-theory.md#coadjoint-representation)
- [Commutator derivation identity](#commutator-derivation-identity)
- [Compact connected complex Lie groups are complex tori](lie-theory.md#compact-connected-complex-lie-groups-are-complex-tori)
- [Compact symplectic Lie algebra](semisimple-lie-algebra.md#compact-symplectic-lie-algebra)
- [Compactness criterion from the Killing form](#compactness-criterion-from-the-killing-form)
- [Complete reducibility of rational GL and SL representations](lie-theory.md#complete-reducibility-of-rational-gl-and-sl-representations)
- [Complex Lie group](lie-theory.md#complex-lie-group)
- [Complexification preserves semisimplicity](#complexification-preserves-semisimplicity)
- [Conjugate-spectrum proof of Cartan solvability](#conjugate-spectrum-proof-of-cartan-solvability)
- [Constraint algebra](classical-mechanics.md#constraint-algebra)
- [Cross-product model of su(2)](linear-operator-theory.md#cross-product-model-of-su-2)
- [Curvature form](fiber-bundle.md#curvature-form)
- [Degree-one almost commutative algebra](module-theory.md#degree-one-almost-commutative-algebra)
- [Derivation of a Lie algebra](#derivation-of-a-lie-algebra)
- [Derivation of an algebra](associative-algebra.md#derivation-of-an-algebra)
- [Derived algebra](#derived-algebra)
- [Derived algebra nilpotence criterion](#derived-algebra-nilpotence-criterion)
- [Differentiating left-invariant matrix fields](lie-theory.md#differentiating-left-invariant-matrix-fields)
- [Engel normalizer lemma](#engel-normalizer-lemma)
- [Euclidean motion Lie algebra in two dimensions](#euclidean-motion-lie-algebra-in-two-dimensions)
- [Exceptional isomorphism between sp4 and so5](semisimple-lie-algebra.md#exceptional-isomorphism-between-sp4-and-so5)
- [Fayet–Iliopoulos terms require an Abelian gauge factor](supersymmetry.md#fayet-iliopoulos-terms-require-an-abelian-gauge-factor)
- [Fixed-point normalization removes the moment-map cocycle](symplectic-geometry.md#fixed-point-normalization-removes-the-moment-map-cocycle)
- [Free Lie algebra](#free-lie-algebra)
- [Fundamental vector field](lie-theory.md#fundamental-vector-field)
- [G2 (mathematics)](lie-theory.md#g2-mathematics)
- [Gauge-boson mass rank from a real scalar vacuum](relativistic-quantum-field.md#gauge-boson-mass-rank-from-a-real-scalar-vacuum)
- [Gauge generator](relativistic-quantum-field.md#gauge-generator)
- [Gauge group](relativistic-quantum-field.md#gauge-group)
- [General linear Lie algebra](#general-linear-lie-algebra)
- [Geodesic-vector criterion for a left-invariant metric](lie-theory.md#geodesic-vector-criterion-for-a-left-invariant-metric)
- [Group manifold](lie-theory.md#group-manifold)
- [Hamiltonian Lie algebra homomorphism](symplectic-geometry.md#hamiltonian-lie-algebra-homomorphism)
- [Hermitian quantum generator convention](#hermitian-quantum-generator-convention)
- [Identity augmentation in quantum controllability](control-theory.md#identity-augmentation-in-quantum-controllability)
- [Integration of a Lie-algebra representation](#integration-of-a-lie-algebra-representation)
- [Invariance of a bilinear form on a Lie algebra](#invariance-of-a-bilinear-form-on-a-lie-algebra)
- [Invariant bilinear-form construction of a Yang-Mills action](relativistic-quantum-field.md#invariant-bilinear-form-construction-of-a-yang-mills-action)
- [Invariant gauge kinetic form](relativistic-quantum-field.md#invariant-gauge-kinetic-form)
- [Kepler dynamical symmetry algebra](classical-mechanics.md#kepler-dynamical-symmetry-algebra)
- [Killing radical is a solvable ideal](#killing-radical-is-a-solvable-ideal)
- [Left-invariant vector field](lie-theory.md#left-invariant-vector-field)
- [Left-right double cover of SO0(2,2)](general-relativity.md#left-right-double-cover-of-so0-2-2)
- [Levi decomposition](lie-theory.md#levi-decomposition)
- [Lie algebra of a quadratic-form stabilizer](lie-theory.md#lie-algebra-of-a-quadratic-form-stabilizer)
- [Lie bracket](#lie-bracket)
- [Lie group](lie-theory.md#lie-group)
- [Lie group action](lie-theory.md#lie-group-action)
- [Lie group isomorphism](lie-theory.md#lie-group-isomorphism)
- [Lie group–Lie algebra correspondence](lie-theory.md#lie-group-lie-algebra-correspondence)
- [Lie groups have no small subgroups](lie-theory.md#lie-groups-have-no-small-subgroups)
- [Lie-Poisson bracket](symplectic-geometry.md#lie-poisson-bracket)
- [Lie polynomial](#lie-polynomial)
- [Lie subgroup](lie-theory.md#lie-subgroup)
- [Lie theory](lie-theory.md)
- [Lie third theorem](lie-theory.md#lie-third-theorem)
- [Limit directions of a closed subgroup](lie-theory.md#limit-directions-of-a-closed-subgroup)
- [Logarithm charts for the special unitary group](topological-group.md#logarithm-charts-for-the-special-unitary-group)
- [Loop algebra](#loop-algebra)
- [Maurer-Cartan coframe of the real affine group](lie-theory.md#maurer-cartan-coframe-of-the-real-affine-group)
- [Milnor–Moore theorem](algebraic-topology.md#milnor-moore-theorem)
- [Moment map](symplectic-geometry.md#moment-map)
- [Nilpotent Lie algebra](#nilpotent-lie-algebra)
- [Nilpotent Lie algebras need not act nilpotently](#nilpotent-lie-algebras-need-not-act-nilpotently)
- [Normal subgroups of a compact group with irreducible adjoint action](lie-theory.md#normal-subgroups-of-a-compact-group-with-irreducible-adjoint-action)
- [Parallelization of a Lie group by left translations](lie-theory.md#parallelization-of-a-lie-group-by-left-translations)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-1.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-1.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-2.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-62.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-63.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-71.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-18.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-18.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-63.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-63.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-74.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-1.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-1.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-16.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-28.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-45.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-45.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-51.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-54.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-57.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-19.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-3.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-4.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-4.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-4.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-45.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-48.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-51.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-58.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-58.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-58.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-19.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-2.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-24.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-50.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-56.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-63.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-85.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-1.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-1.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-19.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-19.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-19.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-31.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-50.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-64.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-64.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-64.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4.md#19h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-32.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-32.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-5.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-5.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-52.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-53.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-6.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-60.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-19.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-23.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-23.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-23.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-23.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-3.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-3.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-3.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-3.md#5/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-49.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-59.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-65.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-65.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#32b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-17.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-17.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-45.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-45.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-58.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-1.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-43.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-43.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-55.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-1.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-1.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-1.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-1.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-1.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-14.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-17.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-48.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-48.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-55.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-55.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-55.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-1.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-1.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-42.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-42.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-42.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-42.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-45.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-50.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-50.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-2.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-2.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-2.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-41.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-41.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-46.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-17.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-2.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-2.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-44.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-44.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-56.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-102.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-102.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-102.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-302.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-302.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-302.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-302.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-304.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-313.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-313.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-313.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-102.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-128.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-301.md#2/d/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-301.md#2/g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-302.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-302.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-302.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-302.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-102.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-302.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-302.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-305.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-306.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#19i/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-102.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-102.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-115.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-302.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-302.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-102.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-115.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-115.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-313.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-102.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-102.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-115.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-102.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-102.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-302.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-307.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-302.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-102.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-302.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-302.md#4/a/solution)
- [Perfect Lie algebra](semisimple-lie-algebra.md#perfect-lie-algebra)
- [Period obstruction to integration of a Lie algebra homomorphism](#period-obstruction-to-integration-of-a-lie-algebra-homomorphism)
- [Poincaré-Birkhoff-Witt theorem](#poincare-birkhoff-witt-theorem)
- [Powerful Lie algebra over p-adic integers](#powerful-lie-algebra-over-p-adic-integers)
- [Primitive element of a Hopf algebra](algebra.md#primitive-element-of-a-hopf-algebra)
- [Principal nilpotent element](semisimple-lie-algebra.md#principal-nilpotent-element)
- [Principal sl2 subalgebra](semisimple-lie-algebra.md#principal-sl2-subalgebra)
- [Proof of Engel theorem by induction and normalizers](#proof-of-engel-theorem-by-induction-and-normalizers)
- [Radical of a Lie algebra](#radical-of-a-lie-algebra)
- [Real-simple exception to uniqueness of the Killing form](#real-simple-exception-to-uniqueness-of-the-killing-form)
- [Real special linear group of degree two](group-theory.md#real-special-linear-group-of-degree-two)
- [Regular element of a semisimple Lie algebra](semisimple-lie-algebra.md#regular-element-of-a-semisimple-lie-algebra)
- [Restriction of a Hamiltonian group action](symplectic-geometry.md#restriction-of-a-hamiltonian-group-action)
- [Ricci curvature of a bi-invariant Riemannian metric](lie-theory.md#ricci-curvature-of-a-bi-invariant-riemannian-metric)
- [Right-invariant vector field](lie-theory.md#right-invariant-vector-field)
- [Root-space decomposition](semisimple-lie-algebra.md#root-space-decomposition)
- [Root system](semisimple-lie-algebra.md#root-system)
- [Semisimple Lie algebra](semisimple-lie-algebra.md)
- [Semisimple Lie group](lie-theory.md#semisimple-lie-group)
- [Semisimple moment-map equivariance](symplectic-geometry.md#semisimple-moment-map-equivariance)
- [Simple Lie algebra](semisimple-lie-algebra.md#simple-lie-algebra)
- [Simple Lie group](lie-theory.md#simple-lie-group)
- [Sl2 triple](semisimple-lie-algebra.md#sl2-triple)
- [Sl2R Lie algebra](semisimple-lie-algebra.md#sl2r-lie-algebra)
- [Special unitary Lie algebra](#special-unitary-lie-algebra)
- [Structure functions of a constraint algebra](classical-mechanics.md#structure-functions-of-a-constraint-algebra)
- [SU(3) group](topological-group.md#su-3-group)
- [SU(3) Lie algebra](#su-3-lie-algebra)
- [Ten-dimensional super Yang-Mills theory](supersymmetry.md#ten-dimensional-super-yang-mills-theory)
- [Tensor-product Casimir trace identity](semisimple-lie-algebra.md#tensor-product-casimir-trace-identity)
- [Three-dimensional Lie algebra structure decomposition](#three-dimensional-lie-algebra-structure-decomposition)
- [Torsion contractions of a left-parallel Lie-group connection](lie-theory.md#torsion-contractions-of-a-left-parallel-lie-group-connection)
- [Trivial Lie algebra representation](#trivial-lie-algebra-representation)
- [Two-dimensional Killing algebra with a periodic generator is abelian](general-relativity.md#two-dimensional-killing-algebra-with-a-periodic-generator-is-abelian)
- [Two-dimensional subalgebra criterion for Lie algebra nilpotence](#two-dimensional-subalgebra-criterion-for-lie-algebra-nilpotence)
- [Unitary Lie algebra](#unitary-lie-algebra)
- [Unitary orbit of a density operator](quantum-theory.md#unitary-orbit-of-a-density-operator)
- [Upper central series of a Lie algebra](#upper-central-series-of-a-lie-algebra)
- [Variation of the Chern-Simons 5-form](relativistic-quantum-field.md#variation-of-the-chern-simons-5-form)
- [Weight-transfer proof of irreducibility of symmetric powers](linear-algebra.md#weight-transfer-proof-of-irreducibility-of-symmetric-powers)
- [Witt algebra](#witt-algebra)
- [Zero generalized weight space of a Cartan subalgebra](semisimple-lie-algebra.md#zero-generalized-weight-space-of-a-cartan-subalgebra)
