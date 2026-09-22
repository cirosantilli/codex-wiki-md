# Lie theory

↑ **Parent:** [Diagonal dominance](algebra.md#diagonal-dominance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lie_theory)

[Lie theory](lie-theory.md) studies continuous symmetries through [Lie groups](#lie-group), [Lie algebras](lie-algebra.md), and their [representations](representation-theory.md).

**Table of contents**

- [Linear algebraic group](#linear-algebraic-group)
  - [Adjoint Chevalley group](#adjoint-chevalley-group)
    - [Adjoint Chevalley group of type A1](#adjoint-chevalley-group-of-type-a1)
  - [Algebraic one-parameter subgroup](#algebraic-one-parameter-subgroup)
  - [Geometrically reductive algebraic group](#geometrically-reductive-algebraic-group)
    - [Determinant separation for positive-characteristic SL2](#determinant-separation-for-positive-characteristic-sl2)
  - [Linearly reductive algebraic group](#linearly-reductive-algebraic-group)
  - [Rational structure on an algebraic group](#rational-structure-on-an-algebraic-group)
    - [Frobenius endomorphism of an algebraic group](#frobenius-endomorphism-of-an-algebraic-group)
      - [Lang theorem for algebraic groups](#lang-theorem-for-algebraic-groups)
        - [Lang map](#lang-map)
  - [Affine group](#affine-group)
  - [Rational representation](#rational-representation)
    - [Unstable vector in a rational representation](#unstable-vector-in-a-rational-representation)
      - [Hilbert-Mumford criterion for the affine null cone](#hilbert-mumford-criterion-for-the-affine-null-cone)
        - [Root-multiplicity criterion for unstable binary forms](#root-multiplicity-criterion-for-unstable-binary-forms)
    - [Complete reducibility of rational GL and SL representations](#complete-reducibility-of-rational-gl-and-sl-representations)
    - [Rational representation of the general linear group](#rational-representation-of-the-general-linear-group)
      - [Rational Schur module](#rational-schur-module)
        - [Dual of a rational Schur module](#dual-of-a-rational-schur-module)
      - [Highest-weight classification of rational GL representations](#highest-weight-classification-of-rational-gl-representations)
      - [Rational extension from SL to GL](#rational-extension-from-sl-to-gl)
      - [Determinant twist](#determinant-twist)
        - [One-dimensional rational characters of the general linear group](#one-dimensional-rational-characters-of-the-general-linear-group)
      - [Polynomial representation of the general linear group](#polynomial-representation-of-the-general-linear-group)
        - [Binary form](#binary-form)
          - [Binary quartic](#binary-quartic)
        - [Multiplicity-free symmetric-algebra model for polynomial GL representations](#multiplicity-free-symmetric-algebra-model-for-polynomial-gl-representations)
        - [Schur functor](#schur-functor)
          - [Schur module](#schur-module)
            - [Length bound for a Schur module](#length-bound-for-a-schur-module)
        - [Schur algebra](#schur-algebra)
          - [Invertible tensor powers span the Schur algebra](#invertible-tensor-powers-span-the-schur-algebra)
          - [Schur–Weyl duality](#schur-weyl-duality)
            - [Tensor cube of the defining unitary representation](#tensor-cube-of-the-defining-unitary-representation)
            - [Trace of a permuted tensor power](#trace-of-a-permuted-tensor-power)
            - [Young-symmetrizer tensor decomposition](#young-symmetrizer-tensor-decomposition)
  - [Lie algebra of an affine algebraic group](#lie-algebra-of-an-affine-algebraic-group)
  - [Descent of an irreducible SL2 representation to PGL2](#descent-of-an-irreducible-sl2-representation-to-pgl2)
  - [Faithful representation of an affine algebraic group](#faithful-representation-of-an-affine-algebraic-group)
  - [Left-right regular representation of an affine algebraic group](#left-right-regular-representation-of-an-affine-algebraic-group)
  - [Semisimple element of an affine algebraic group](#semisimple-element-of-an-affine-algebraic-group)
  - [Unipotent element of an affine algebraic group](#unipotent-element-of-an-affine-algebraic-group)
    - [Unipotent matrix](#unipotent-matrix)
  - [Jordan decomposition in an affine algebraic group](#jordan-decomposition-in-an-affine-algebraic-group)
  - [Derived subgroup of an affine algebraic group](#derived-subgroup-of-an-affine-algebraic-group)
    - [Solvable affine algebraic group](#solvable-affine-algebraic-group)
      - [Lie-Kolchin theorem](#lie-kolchin-theorem)
  - [Diagonalizable group](#diagonalizable-group)
  - [Reductive group](#reductive-group)
    - [Finite group of Lie type](#finite-group-of-lie-type)
      - [Harish-Chandra induction](#harish-chandra-induction)
        - [Mackey formula for Harish-Chandra induction](#mackey-formula-for-harish-chandra-induction)
        - [Harish-Chandra restriction](#harish-chandra-restriction)
          - [Cuspidal representation of a finite reductive group](#cuspidal-representation-of-a-finite-reductive-group)
      - [Deligne-Lusztig theory](#deligne-lusztig-theory)
        - [Deligne-Lusztig induction](#deligne-lusztig-induction)
          - [Harish-Chandra restriction of a Deligne-Lusztig character](#harish-chandra-restriction-of-a-deligne-lusztig-character)
          - [Principal series of a finite reductive group](#principal-series-of-a-finite-reductive-group)
            - [Irreducibility of the split SL3 principal series](#irreducibility-of-the-split-sl3-principal-series)
        - [Deligne-Lusztig variety](#deligne-lusztig-variety)
          - [Unipotent quotient in a Deligne-Lusztig variety](#unipotent-quotient-in-a-deligne-lusztig-variety)
    - [Borel subgroup](#borel-subgroup)
      - [Parabolic subgroup](#parabolic-subgroup)
        - [Levi subgroup](#levi-subgroup)
      - [Generalized flag variety](#generalized-flag-variety)
    - [Root datum](#root-datum)
    - [Bruhat decomposition](#bruhat-decomposition)
      - [Relative position of Borel subgroups](#relative-position-of-borel-subgroups)
      - [Bruhat decomposition of a BN-pair](#bruhat-decomposition-of-a-bn-pair)
  - [Algebraic-group torsor](#algebraic-group-torsor)
  - [Unipotent](#unipotent)
    - [Unipotent algebraic group](#unipotent-algebraic-group)
      - [Unipotent radical](#unipotent-radical)
      - [Kolchin theorem](#kolchin-theorem)
- [Lie group](#lie-group)
  - [Lie groups have no small subgroups](#lie-groups-have-no-small-subgroups)
  - [G2 (mathematics)](#g2-mathematics)
  - [Lie group–Lie algebra correspondence](#lie-group-lie-algebra-correspondence)
  - [Lie third theorem](#lie-third-theorem)
  - [Universal covering Lie group](#universal-covering-lie-group)
  - [Complex Lie group](#complex-lie-group)
    - [Compact connected complex Lie groups are complex tori](#compact-connected-complex-lie-groups-are-complex-tori)
  - [Abelian Lie group](#abelian-lie-group)
    - [Classification of connected abelian Lie groups](#classification-of-connected-abelian-lie-groups)
  - [Sol Lie group](#sol-lie-group)
  - [Semisimple Lie group](#semisimple-lie-group)
  - [Free step-N nilpotent Lie group](#free-step-n-nilpotent-lie-group)
    - [Step-2 planar group coordinates](#step-2-planar-group-coordinates)
  - [Loop group](#loop-group)
    - [Positive energy representation of the loop group of U(1)](#positive-energy-representation-of-the-loop-group-of-u-1)
      - [Loop group two-cocycle for U(1)](#loop-group-two-cocycle-for-u-1)
  - [Bi-invariant pseudo-Riemannian metric](#bi-invariant-pseudo-riemannian-metric)
    - [Neutral invariant metrics on the free two-step Lie algebra on three generators](#neutral-invariant-metrics-on-the-free-two-step-lie-algebra-on-three-generators)
    - [Killing-form Einstein metric](#killing-form-einstein-metric)
  - [Compact Lie group](#compact-lie-group)
    - [Real torus](#real-torus)
    - [Weyl integration formula](#weyl-integration-formula)
      - [Conjugation Jacobian for a compact Lie group](#conjugation-jacobian-for-a-compact-lie-group)
      - [Weyl integration formula for U(n)](#weyl-integration-formula-for-u-n)
  - [Translation-dilation group of the plane](#translation-dilation-group-of-the-plane)
    - [Left-invariant coframe of the translation-dilation group](#left-invariant-coframe-of-the-translation-dilation-group)
  - [Lie group homomorphism](#lie-group-homomorphism)
    - [Lie group isomorphism](#lie-group-isomorphism)
    - [Lie group homomorphism determined by its differential](#lie-group-homomorphism-determined-by-its-differential)
  - [Right-invariant Riemannian metric](#right-invariant-riemannian-metric)
  - [Right-invariant differential form](#right-invariant-differential-form)
  - [Maximal torus](#maximal-torus)
    - [Adjoint-orbit criterion for maximal-torus conjugacy](#adjoint-orbit-criterion-for-maximal-torus-conjugacy)
    - [Character lattice of a torus](#character-lattice-of-a-torus)
  - [Identity component of a Lie group](#identity-component-of-a-lie-group)
  - [Group manifold](#group-manifold)
  - [Lie subgroup](#lie-subgroup)
    - [Closed-subgroup theorem](#closed-subgroup-theorem)
      - [Local product coordinates for a closed subgroup](#local-product-coordinates-for-a-closed-subgroup)
      - [Lie algebra of a closed subgroup](#lie-algebra-of-a-closed-subgroup)
      - [Limit directions of a closed subgroup](#limit-directions-of-a-closed-subgroup)
    - [Lie algebra of a normal Lie subgroup](#lie-algebra-of-a-normal-lie-subgroup)
  - [Lie group action](#lie-group-action)
    - [Proper Lie group action](#proper-lie-group-action)
    - [Torus action](#torus-action)
    - [Special linear congruence action on symmetric matrices](#special-linear-congruence-action-on-symmetric-matrices)
    - [Coadjoint representation](#coadjoint-representation)
      - [Coadjoint orbit](#coadjoint-orbit)
        - [Kirillov–Kostant–Souriau symplectic form](#kirillov-kostant-souriau-symplectic-form)
    - [Fundamental vector field](#fundamental-vector-field)
      - [Infinitesimal left-action sign convention](#infinitesimal-left-action-sign-convention)
  - [Matrix Lie group](#matrix-lie-group)
    - [Lie algebra of a quadratic-form stabilizer](#lie-algebra-of-a-quadratic-form-stabilizer)
    - [Exponential map of a matrix Lie group](#exponential-map-of-a-matrix-lie-group)
      - [Exponential-surjectivity obstruction from distinct negative eigenvalues](#exponential-surjectivity-obstruction-from-distinct-negative-eigenvalues)
    - [Logarithmic chart of a matrix Lie group](#logarithmic-chart-of-a-matrix-lie-group)
  - [Simple Lie group](#simple-lie-group)
  - [Homogeneous space](#homogeneous-space)
  - [Left and right translation on a Lie group](#left-and-right-translation-on-a-lie-group)
    - [Flat translation connections on a Lie group](#flat-translation-connections-on-a-lie-group)
      - [Torsion contractions of a left-parallel Lie-group connection](#torsion-contractions-of-a-left-parallel-lie-group-connection)
      - [Canonical torsion-free connection on a Lie group](#canonical-torsion-free-connection-on-a-lie-group)
    - [Right-invariant vector field](#right-invariant-vector-field)
      - [Right-invariant vector fields realize the opposite Lie algebra](#right-invariant-vector-fields-realize-the-opposite-lie-algebra)
    - [Left-invariant vector field](#left-invariant-vector-field)
      - [Pauli-coordinate left-invariant vector fields on SU(2)](#pauli-coordinate-left-invariant-vector-fields-on-su-2)
      - [Parallelization of a Lie group by left translations](#parallelization-of-a-lie-group-by-left-translations)
      - [Differentiating left-invariant matrix fields](#differentiating-left-invariant-matrix-fields)
      - [Completeness of left-invariant vector fields](#completeness-of-left-invariant-vector-fields)
    - [Left-invariant differential form](#left-invariant-differential-form)
      - [Invariant volume form on a Lie group](#invariant-volume-form-on-a-lie-group)
      - [Bi-invariant differential form](#bi-invariant-differential-form)
        - [Cartan three-form](#cartan-three-form)
        - [Closed left-invariant 1-form](#closed-left-invariant-1-form)
  - [One-parameter subgroup](#one-parameter-subgroup)
    - [Classification of nontrivial one-parameter subgroups](#classification-of-nontrivial-one-parameter-subgroups)
      - [Compact one-parameter subgroups of SL2R](#compact-one-parameter-subgroups-of-sl2r)
  - [Circle group](#circle-group)
    - [Circle metric](#circle-metric)
  - [Lie-group representation](#lie-group-representation)
    - [Derived representation](#derived-representation)
  - [Adjoint representation of a Lie group](#adjoint-representation-of-a-lie-group)
    - [Normal subgroups of a compact group with irreducible adjoint action](#normal-subgroups-of-a-compact-group-with-irreducible-adjoint-action)
    - [Inverse conjugation and adjoint antirepresentations](#inverse-conjugation-and-adjoint-antirepresentations)
    - [Adjoint double cover from SU(2) to SO(3)](#adjoint-double-cover-from-su-2-to-so-3)
      - [Descent of an SU(2) representation to SO(3)](#descent-of-an-su-2-representation-to-so-3)
  - [Local group law](#local-group-law)
  - [Maurer-Cartan form](#maurer-cartan-form)
    - [Maurer-Cartan equation](#maurer-cartan-equation)
      - [Maurer-Cartan equation in a Lie-algebra basis](#maurer-cartan-equation-in-a-lie-algebra-basis)
        - [Symmetric-part ambiguity in Maurer-Cartan coefficients](#symmetric-part-ambiguity-in-maurer-cartan-coefficients)
  - [Orientation-preserving affine group of the real line](#orientation-preserving-affine-group-of-the-real-line)
    - [Invariant frames of the real affine group](#invariant-frames-of-the-real-affine-group)
    - [Maurer-Cartan coframe of the real affine group](#maurer-cartan-coframe-of-the-real-affine-group)
  - [Left-invariant metric](#left-invariant-metric)
    - [Bi-invariant Riemannian metric](#bi-invariant-riemannian-metric)
      - [Adjoint dilation obstruction to a bi-invariant Riemannian metric](#adjoint-dilation-obstruction-to-a-bi-invariant-riemannian-metric)
      - [Ricci curvature of a bi-invariant Riemannian metric](#ricci-curvature-of-a-bi-invariant-riemannian-metric)
      - [Geodesics of a bi-invariant metric are one-parameter subgroups](#geodesics-of-a-bi-invariant-metric-are-one-parameter-subgroups)
      - [Levi-Civita connection of a bi-invariant metric](#levi-civita-connection-of-a-bi-invariant-metric)
    - [Geodesic-vector criterion for a left-invariant metric](#geodesic-vector-criterion-for-a-left-invariant-metric)
  - [Exponential map of a Lie group](#exponential-map-of-a-lie-group)
    - [Additivity of the Lie exponential map](#additivity-of-the-lie-exponential-map)
    - [Lie product formula in a Lie group](#lie-product-formula-in-a-lie-group)
    - [Naturality of the Lie group exponential](#naturality-of-the-lie-group-exponential)
    - [Local exponential chart](#local-exponential-chart)
  - [Cayley transform (Lie theory)](#cayley-transform-lie-theory)
- [Lie algebra](lie-algebra.md)
  - [Cartan's criterion](lie-algebra.md#cartan-s-criterion)
  - [Loop algebra](lie-algebra.md#loop-algebra)
  - [Affine current algebra](lie-algebra.md#affine-current-algebra)
  - [Free Lie algebra](lie-algebra.md#free-lie-algebra)
    - [Lie polynomial](lie-algebra.md#lie-polynomial)
  - [Semidirect product of Lie algebras](lie-algebra.md#semidirect-product-of-lie-algebras)
  - [Lie algebra cohomology](lie-algebra.md#lie-algebra-cohomology)
    - [Lie algebra two-cocycle](lie-algebra.md#lie-algebra-two-cocycle)
  - [Compact Lie algebra](lie-algebra.md#compact-lie-algebra)
  - [Powerful Lie algebra over p-adic integers](lie-algebra.md#powerful-lie-algebra-over-p-adic-integers)
    - [Lie algebra of a uniform pro-p group](lie-algebra.md#lie-algebra-of-a-uniform-pro-p-group)
    - [BCH convergence on a powerful Lie lattice](lie-algebra.md#bch-convergence-on-a-powerful-lie-lattice)
  - [Cross-product Lie algebra](lie-algebra.md#cross-product-lie-algebra)
  - [Euclidean motion Lie algebra in two dimensions](lie-algebra.md#euclidean-motion-lie-algebra-in-two-dimensions)
    - [Killing form of the planar Euclidean motion Lie algebra](lie-algebra.md#killing-form-of-the-planar-euclidean-motion-lie-algebra)
  - [Graded Lie algebra](lie-algebra.md#graded-lie-algebra)
    - [Chevalley–Eilenberg cochains of a graded Lie algebra](lie-algebra.md#chevalley-eilenberg-cochains-of-a-graded-lie-algebra)
    - [Free graded Lie algebra](lie-algebra.md#free-graded-lie-algebra)
    - [Graded Lie bracket](lie-algebra.md#graded-lie-bracket)
  - [Central extension of a Lie algebra](lie-algebra.md#central-extension-of-a-lie-algebra)
  - [Witt algebra](lie-algebra.md#witt-algebra)
  - [Centralizer of an element of a Lie algebra](lie-algebra.md#centralizer-of-an-element-of-a-lie-algebra)
    - [Centralizer lower bound for a root vector](lie-algebra.md#centralizer-lower-bound-for-a-root-vector)
  - [Lie algebra generator](lie-algebra.md#lie-algebra-generator)
  - [Lie algebra of a matrix Lie group](lie-algebra.md#lie-algebra-of-a-matrix-lie-group)
    - [Matrix commutator from a logarithm chart](lie-algebra.md#matrix-commutator-from-a-logarithm-chart)
    - [General linear Lie algebra](lie-algebra.md#general-linear-lie-algebra)
    - [Unitary Lie algebra](lie-algebra.md#unitary-lie-algebra)
      - [Special unitary Lie algebra](lie-algebra.md#special-unitary-lie-algebra)
        - [Trace normalization of su(2)](lie-algebra.md#trace-normalization-of-su-2)
      - [SU(3) Lie algebra](lie-algebra.md#su-3-lie-algebra)
        - [Root SU(2) subalgebras of SU(3)](lie-algebra.md#root-su-2-subalgebras-of-su-3)
      - [Matrix-unit basis of the unitary Lie algebra](lie-algebra.md#matrix-unit-basis-of-the-unitary-lie-algebra)
  - [Lie algebra isomorphism](lie-algebra.md#lie-algebra-isomorphism)
  - [Direct sum of Lie algebras](lie-algebra.md#direct-sum-of-lie-algebras)
  - [Lie subalgebra](lie-algebra.md#lie-subalgebra)
    - [Normalizer of a Lie subalgebra](lie-algebra.md#normalizer-of-a-lie-subalgebra)
  - [Derivation of a Lie algebra](lie-algebra.md#derivation-of-a-lie-algebra)
    - [Exponential of a nilpotent Lie algebra derivation](lie-algebra.md#exponential-of-a-nilpotent-lie-algebra-derivation)
    - [Inner derivation of a Lie algebra](lie-algebra.md#inner-derivation-of-a-lie-algebra)
    - [Derivation Lie algebra](lie-algebra.md#derivation-lie-algebra)
    - [Outer derivation of a nilpotent Lie algebra](lie-algebra.md#outer-derivation-of-a-nilpotent-lie-algebra)
    - [Generalized-eigenspace bracket lemma](lie-algebra.md#generalized-eigenspace-bracket-lemma)
  - [Invariant bilinear form on a Lie algebra](lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra)
    - [Invariance of a bilinear form on a Lie algebra](lie-algebra.md#invariance-of-a-bilinear-form-on-a-lie-algebra)
    - [Positive invariant metric on a Lie algebra](lie-algebra.md#positive-invariant-metric-on-a-lie-algebra)
  - [Lie superalgebra](lie-algebra.md#lie-superalgebra)
    - [Lie superalgebra representation](lie-algebra.md#lie-superalgebra-representation)
    - [Graded Jacobi identity](lie-algebra.md#graded-jacobi-identity)
  - [Lie bracket](lie-algebra.md#lie-bracket)
    - [Antisymmetry of a Lie bracket](lie-algebra.md#antisymmetry-of-a-lie-bracket)
    - [Lie bracket from local group commutators](lie-algebra.md#lie-bracket-from-local-group-commutators)
    - [Commutator](lie-algebra.md#commutator)
      - [Identity commutator cyclic ladder](lie-algebra.md#identity-commutator-cyclic-ladder)
      - [Commutator expansion for exponential conjugation](lie-algebra.md#commutator-expansion-for-exponential-conjugation)
        - [Central-commutator exponential identity](lie-algebra.md#central-commutator-exponential-identity)
      - [Trace of a matrix commutator](lie-algebra.md#trace-of-a-matrix-commutator)
      - [Commutator derivation identity](lie-algebra.md#commutator-derivation-identity)
    - [Jacobi identity](lie-algebra.md#jacobi-identity)
  - [Abelian Lie algebra](lie-algebra.md#abelian-lie-algebra)
  - [Semidirect product of a Lie algebra and a module](lie-algebra.md#semidirect-product-of-a-lie-algebra-and-a-module)
    - [Killing form of a semidirect product with a module](lie-algebra.md#killing-form-of-a-semidirect-product-with-a-module)
  - [Ideal of a Lie algebra](lie-algebra.md#ideal-of-a-lie-algebra)
    - [Quotient Lie algebra](lie-algebra.md#quotient-lie-algebra)
  - [Derived series of a Lie algebra](lie-algebra.md#derived-series-of-a-lie-algebra)
    - [Derived algebra](lie-algebra.md#derived-algebra)
      - [Derived algebra nilpotence criterion](lie-algebra.md#derived-algebra-nilpotence-criterion)
    - [Solvable Lie algebra](lie-algebra.md#solvable-lie-algebra)
      - [Diamond Lie algebra](lie-algebra.md#diamond-lie-algebra)
      - [Affine Lie algebra of the line](lie-algebra.md#affine-lie-algebra-of-the-line)
      - [Radical of a Lie algebra](lie-algebra.md#radical-of-a-lie-algebra)
      - [Lie's theorem](lie-algebra.md#lie-s-theorem)
        - [Infinite-dimensional simple module for the two-dimensional affine Lie algebra](lie-algebra.md#infinite-dimensional-simple-module-for-the-two-dimensional-affine-lie-algebra)
        - [Simultaneous triangularization of a Lie algebra representation](lie-algebra.md#simultaneous-triangularization-of-a-lie-algebra-representation)
        - [Failure of Lie theorem in positive characteristic](lie-algebra.md#failure-of-lie-theorem-in-positive-characteristic)
      - [Cartan solvability criterion](lie-algebra.md#cartan-solvability-criterion)
        - [Conjugate-spectrum proof of Cartan solvability](lie-algebra.md#conjugate-spectrum-proof-of-cartan-solvability)
  - [Center of a Lie algebra](lie-algebra.md#center-of-a-lie-algebra)
    - [Central ideal](lie-algebra.md#central-ideal)
  - [Lower central series of a Lie algebra](lie-algebra.md#lower-central-series-of-a-lie-algebra)
    - [Nilpotent Lie algebra](lie-algebra.md#nilpotent-lie-algebra)
      - [Killing form of a nilpotent Lie algebra vanishes](lie-algebra.md#killing-form-of-a-nilpotent-lie-algebra-vanishes)
      - [Upper central series of a Lie algebra](lie-algebra.md#upper-central-series-of-a-lie-algebra)
      - [Two-dimensional subalgebra criterion for Lie algebra nilpotence](lie-algebra.md#two-dimensional-subalgebra-criterion-for-lie-algebra-nilpotence)
      - [Normalizer condition for a nilpotent Lie algebra](lie-algebra.md#normalizer-condition-for-a-nilpotent-lie-algebra)
      - [Engel's theorem](lie-algebra.md#engel-s-theorem)
        - [Proof of Engel theorem by induction and normalizers](lie-algebra.md#proof-of-engel-theorem-by-induction-and-normalizers)
        - [Engel lemma](lie-algebra.md#engel-lemma)
          - [Engel normalizer lemma](lie-algebra.md#engel-normalizer-lemma)
  - [Lie algebra homomorphism](lie-algebra.md#lie-algebra-homomorphism)
    - [Integration of a Lie algebra homomorphism](lie-algebra.md#integration-of-a-lie-algebra-homomorphism)
      - [Period obstruction to integration of a Lie algebra homomorphism](lie-algebra.md#period-obstruction-to-integration-of-a-lie-algebra-homomorphism)
    - [Differential of a Lie group homomorphism preserves Lie brackets](lie-algebra.md#differential-of-a-lie-group-homomorphism-preserves-lie-brackets)
    - [Lie algebra representation](lie-algebra.md#lie-algebra-representation)
      - [Representation ring of a semisimple Lie algebra](lie-algebra.md#representation-ring-of-a-semisimple-lie-algebra)
      - [Defining representation of a matrix Lie algebra](lie-algebra.md#defining-representation-of-a-matrix-lie-algebra)
      - [Hermitian quantum generator convention](lie-algebra.md#hermitian-quantum-generator-convention)
      - [Lie algebra representation homomorphism](lie-algebra.md#lie-algebra-representation-homomorphism)
      - [Exterior-power Lie algebra representation](lie-algebra.md#exterior-power-lie-algebra-representation)
      - [Nilpotent Lie algebras need not act nilpotently](lie-algebra.md#nilpotent-lie-algebras-need-not-act-nilpotently)
      - [Tensor product of Lie algebra representations](lie-algebra.md#tensor-product-of-lie-algebra-representations)
        - [SU(3) triplet-octet decomposition](lie-algebra.md#su-3-triplet-octet-decomposition)
        - [sl2 tensor product of cubic and quadratic symmetric powers](lie-algebra.md#sl2-tensor-product-of-cubic-and-quadratic-symmetric-powers)
        - [Action map of a Lie algebra representation](lie-algebra.md#action-map-of-a-lie-algebra-representation)
          - [Action summand can fail for an infinite-dimensional simple module](lie-algebra.md#action-summand-can-fail-for-an-infinite-dimensional-simple-module)
        - [Tensor product of the standard representation with its exterior square](lie-algebra.md#tensor-product-of-the-standard-representation-with-its-exterior-square)
        - [sl3 highest-weight tensor rule](lie-algebra.md#sl3-highest-weight-tensor-rule)
      - [Integration of a Lie-algebra representation](lie-algebra.md#integration-of-a-lie-algebra-representation)
      - [Lie-invariant bilinear form](lie-algebra.md#lie-invariant-bilinear-form)
      - [Dual Lie algebra representation](lie-algebra.md#dual-lie-algebra-representation)
        - [Highest weight of a dual representation](lie-algebra.md#highest-weight-of-a-dual-representation)
      - [Trivial Lie algebra representation](lie-algebra.md#trivial-lie-algebra-representation)
      - [Hom representation](lie-algebra.md#hom-representation)
      - [Automorphism of a Lie algebra](lie-algebra.md#automorphism-of-a-lie-algebra)
      - [Branching rule](lie-algebra.md#branching-rule)
        - [Adjoint branching to root sl2 subalgebras in rank two](lie-algebra.md#adjoint-branching-to-root-sl2-subalgebras-in-rank-two)
      - [Structure constant of a Lie algebra](lie-algebra.md#structure-constant-of-a-lie-algebra)
        - [Three-dimensional Lie algebra structure decomposition](lie-algebra.md#three-dimensional-lie-algebra-structure-decomposition)
        - [Antisymmetry of Killing-lowered structure constants](lie-algebra.md#antisymmetry-of-killing-lowered-structure-constants)
      - [Faithful Lie algebra representation](lie-algebra.md#faithful-lie-algebra-representation)
        - [Ado's theorem](lie-algebra.md#ado-s-theorem)
      - [Irreducible Lie algebra representation](lie-algebra.md#irreducible-lie-algebra-representation)
      - [Adjoint representation of a Lie algebra](lie-algebra.md#adjoint-representation-of-a-lie-algebra)
        - [Adjoint representation of SU(3)](lie-algebra.md#adjoint-representation-of-su-3)
          - [Tensor square of the SU(3) adjoint representation](lie-algebra.md#tensor-square-of-the-su-3-adjoint-representation)
        - [Killing form](lie-algebra.md#killing-form)
          - [Killing form of the general linear Lie algebra](lie-algebra.md#killing-form-of-the-general-linear-lie-algebra)
          - [Killing-form invariance under a Lie-group adjoint action](lie-algebra.md#killing-form-invariance-under-a-lie-group-adjoint-action)
          - [Killing form for cyclic three-generator brackets](lie-algebra.md#killing-form-for-cyclic-three-generator-brackets)
          - [Orthogonal ideal splitting for a nondegenerate Killing form](lie-algebra.md#orthogonal-ideal-splitting-for-a-nondegenerate-killing-form)
          - [Radical of the Killing form](lie-algebra.md#radical-of-the-killing-form)
          - [Compactness criterion from the Killing form](lie-algebra.md#compactness-criterion-from-the-killing-form)
          - [Abelian ideals lie in the radical of the Killing form](lie-algebra.md#abelian-ideals-lie-in-the-radical-of-the-killing-form)
          - [Solvability of the radical of the Killing form](lie-algebra.md#solvability-of-the-radical-of-the-killing-form)
          - [Cartan criterion for semisimplicity](lie-algebra.md#cartan-criterion-for-semisimplicity)
            - [Killing radical is a solvable ideal](lie-algebra.md#killing-radical-is-a-solvable-ideal)
          - [Uniqueness of an invariant bilinear form on a simple Lie algebra](lie-algebra.md#uniqueness-of-an-invariant-bilinear-form-on-a-simple-lie-algebra)
            - [Real-simple exception to uniqueness of the Killing form](lie-algebra.md#real-simple-exception-to-uniqueness-of-the-killing-form)
          - [Killing form of the special linear Lie algebra](lie-algebra.md#killing-form-of-the-special-linear-lie-algebra)
        - [Adjoint irreducibility of a simple Lie algebra](lie-algebra.md#adjoint-irreducibility-of-a-simple-lie-algebra)
      - [Trace form of a Lie algebra representation](lie-algebra.md#trace-form-of-a-lie-algebra-representation)
        - [Trace forms of solvable Lie algebras annihilate the derived algebra](lie-algebra.md#trace-forms-of-solvable-lie-algebras-annihilate-the-derived-algebra)
        - [Cubic trace tensor of a Lie algebra representation](lie-algebra.md#cubic-trace-tensor-of-a-lie-algebra-representation)
          - [Killing-normalized contraction of a cubic trace tensor](lie-algebra.md#killing-normalized-contraction-of-a-cubic-trace-tensor)
          - [Invariance identity for a cubic trace tensor](lie-algebra.md#invariance-identity-for-a-cubic-trace-tensor)
        - [Positive trace index for a compact simple Lie algebra](lie-algebra.md#positive-trace-index-for-a-compact-simple-lie-algebra)
      - [Trace trilinear form of a Lie algebra representation](lie-algebra.md#trace-trilinear-form-of-a-lie-algebra-representation)
  - [Heisenberg Lie algebra](lie-algebra.md#heisenberg-lie-algebra)
    - [Heisenberg group](lie-algebra.md#heisenberg-group)
      - [Center quotient of the real Heisenberg group](lie-algebra.md#center-quotient-of-the-real-heisenberg-group)
      - [Right-invariant coframe of the real Heisenberg group](lie-algebra.md#right-invariant-coframe-of-the-real-heisenberg-group)
        - [Killing frame for a right-invariant Heisenberg metric](lie-algebra.md#killing-frame-for-a-right-invariant-heisenberg-metric)
      - [Modular Heisenberg group](lie-algebra.md#modular-heisenberg-group)
      - [Left-invariant frame of the real Heisenberg group](lie-algebra.md#left-invariant-frame-of-the-real-heisenberg-group)
        - [Heisenberg horizontal distribution](lie-algebra.md#heisenberg-horizontal-distribution)
          - [Smooth horizontal reachability in the real Heisenberg group](lie-algebra.md#smooth-horizontal-reachability-in-the-real-heisenberg-group)
      - [Integer Heisenberg group](lie-algebra.md#integer-heisenberg-group)
        - [Scaled Heisenberg lattice](lie-algebra.md#scaled-heisenberg-lattice)
        - [Commutator identity in the integer Heisenberg group](lie-algebra.md#commutator-identity-in-the-integer-heisenberg-group)
      - [Schrödinger representation of the Heisenberg group](lie-algebra.md#schrodinger-representation-of-the-heisenberg-group)
    - [Polynomial representation of the Heisenberg Lie algebra](lie-algebra.md#polynomial-representation-of-the-heisenberg-lie-algebra)
  - [Complexification of a Lie algebra](lie-algebra.md#complexification-of-a-lie-algebra)
    - [Complexification preserves semisimplicity](lie-algebra.md#complexification-preserves-semisimplicity)
  - [Universal enveloping algebra](lie-algebra.md#universal-enveloping-algebra)
    - [Poincaré-Birkhoff-Witt theorem](lie-algebra.md#poincare-birkhoff-witt-theorem)
      - [Graded Poincaré–Birkhoff–Witt theorem](lie-algebra.md#graded-poincare-birkhoff-witt-theorem)
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
- [Coxeter group](#coxeter-group)
  - [Coxeter system](#coxeter-system)
    - [Coxeter matrix](#coxeter-matrix)
      - [Coxeter graph](#coxeter-graph)
        - [Admissible crystallographic Coxeter graph](#admissible-crystallographic-coxeter-graph)
        - [Irreducible Coxeter system](#irreducible-coxeter-system)
        - [Type E(p,q,k) Coxeter graph](#type-e-p-q-k-coxeter-graph)
    - [Reduced expression in a Coxeter group](#reduced-expression-in-a-coxeter-group)
      - [Deletion condition for involutory generators](#deletion-condition-for-involutory-generators)
        - [Folding-grid proof of the deletion condition](#folding-grid-proof-of-the-deletion-condition)
      - [Exchange condition for a Coxeter group](#exchange-condition-for-a-coxeter-group)
      - [Matsumoto theorem](#matsumoto-theorem)
        - [Tits word reduction theorem](#tits-word-reduction-theorem)
    - [Geometric representation of a Coxeter group](#geometric-representation-of-a-coxeter-group)
      - [Coxeter Gram matrix](#coxeter-gram-matrix)
      - [Dual geometric representation of a Coxeter group](#dual-geometric-representation-of-a-coxeter-group)
        - [Tits cone](#tits-cone)
        - [Coxeter complex](#coxeter-complex)
    - [Reflection of a Coxeter group](#reflection-of-a-coxeter-group)
      - [Wall of a Coxeter group](#wall-of-a-coxeter-group)
        - [Half-space of a Coxeter group](#half-space-of-a-coxeter-group)
    - [Standard parabolic subgroup](#standard-parabolic-subgroup)
      - [Spherical subset of a Coxeter system](#spherical-subset-of-a-coxeter-system)
      - [Davis complex](#davis-complex)
        - [Basic construction of a Coxeter group](#basic-construction-of-a-coxeter-group)
    - [Folding condition](#folding-condition)
      - [Braid relation in a Coxeter group](#braid-relation-in-a-coxeter-group)
    - [Coxeter element](#coxeter-element)
      - [Coxeter number](#coxeter-number)
  - [Finite Coxeter group](#finite-coxeter-group)
    - [Longest element of a Coxeter group](#longest-element-of-a-coxeter-group)
    - [E7 Coxeter group](#e7-coxeter-group)
    - [Hyperoctahedral group](#hyperoctahedral-group)
      - [Even signed symmetric group](#even-signed-symmetric-group)
  - [Affine Coxeter group](#affine-coxeter-group)
  - [Hyperbolic Coxeter group](#hyperbolic-coxeter-group)
  - [BN-pair](#bn-pair)
  - [Hecke algebra](#hecke-algebra)
    - [Iwahori-Hecke algebra](#iwahori-hecke-algebra)
      - [0-Hecke algebra](#0-hecke-algebra)
      - [Iwahori-Hecke algebra of a BN-pair](#iwahori-hecke-algebra-of-a-bn-pair)
        - [Hecke parameter of a BN-pair](#hecke-parameter-of-a-bn-pair)
- [Levi decomposition](#levi-decomposition)

## Linear algebraic group

↑ **Parent:** [Lie theory](lie-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_algebraic_group)

An affine algebraic group is an [affine variety](algebraic-geometry.md#affine-algebraic-set) $G$ whose multiplication and inversion are [regular maps](algebraic-geometry.md#morphism-of-algebraic-varieties). Equivalently, its [coordinate ring](algebraic-geometry.md#coordinate-ring) $k[G]$ is a commutative [Hopf algebra](algebra.md#hopf-algebra), with comultiplication induced by multiplication in $G$.

### Adjoint Chevalley group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

Fix a [Chevalley basis](semisimple-lie-algebra.md#chevalley-basis) and its integral lattice. The adjoint Chevalley group over a [field](algebra.md#field) is generated by the root operators obtained from the integral divided-power polynomials $x_\alpha(t)=\sum_j t^j(\operatorname{ad}e_\alpha)^j/j!$ on that lattice. The coefficients are first computed over the integers and then reduced to the field; factorials need not be invertible there. This is the adjoint construction; other weight lattices give other isogeny forms of [groups](group.md) of Lie type.

#### Adjoint Chevalley group of type A1

↑ **Parent:** [Adjoint Chevalley group](#adjoint-chevalley-group)

On the [sl2 Lie algebra](semisimple-lie-algebra.md#sl2-lie-algebra) with basis $e=E_{12},h=E_{11}-E_{22},f=E_{21}$, the integral adjoint root polynomials are

$$
\begin{aligned}
x_+(t)e&=e,&x_+(t)h&=h-2te,&x_+(t)f&=f+th-t^2e,\\
x_-(s)f&=f,&x_-(s)h&=h+2sf,&x_-(s)e&=e-sh-s^2f.
\end{aligned}
$$

These are conjugation by the upper and lower elementary matrices of the [special linear group](group-theory.md#special-linear-group). Those matrices generate $SL_2(K)$, and a matrix commuting with both $E_{12}$ and $E_{21}$ is scalar. Thus the kernel is precisely $\{aI:a^2=1\}$ over every field, even in characteristic two, and the image is the displayed quotient.

### Algebraic one-parameter subgroup

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

An algebraic one-parameter subgroup is a regular group homomorphism from the multiplicative algebraic group. In $SL_n$, a change of basis makes it $t\mapsto\operatorname{diag}(t^{a_1},\ldots,t^{a_n})$ for integers with sum zero. This is the algebraic multiplicative notion, distinct from an additive real-parameter subgroup of a Lie group.

### Geometrically reductive algebraic group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

For every finite-dimensional [rational representation](#rational-representation) $V$ and every nonzero $v\in V^G$, a geometrically reductive algebraic group admits a homogeneous invariant polynomial $F\in k[V]^G$ of positive degree with $F(v)\ne0$. A linearly reductive group can take degree one. In positive characteristic, higher degree is essential: a power $p^r$ can separate a fixed vector even when an invariant linear functional cannot.

#### Determinant separation for positive-characteristic SL2

↑ **Parent:** [Geometrically reductive algebraic group](#geometrically-reductive-algebraic-group)

Choose a torus-invariant functional nonzero on a fixed vector, and map the representation to right-torus-invariant matrix coefficients on $SL_2$. These functions lie in a finite filtration by polynomials of bidegree $(n,n)$ in the two matrix columns. For $n=q-1$, all binomial coefficients are nonzero in characteristic $p$, so the invariant tensor given by the determinant to power $n$ induces an invertible map from the symmetric power's dual to itself. The filtration piece becomes its endomorphism space, with the constant function corresponding to the identity. The endomorphism determinant is an invariant degree-$q$ polynomial equal to one there; composing it with the original representation map proves geometric reductivity.

### Linearly reductive algebraic group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

An [affine algebraic group](#linear-algebraic-group) is linearly reductive when every finite-dimensional [rational representation](#rational-representation) is completely reducible. Equivalently its invariants functor is exact. Over a field of characteristic zero, [reductive algebraic groups](#reductive-group) are linearly reductive; in positive characteristic this stronger property fails for many reductive groups. An [algebraic torus](toric-geometry.md#algebraic-torus) is linearly reductive in every characteristic because its rational representations decompose into character spaces.

### Rational structure on an algebraic group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

A rational structure over $\mathbb F_q$ is a model over that [finite field](algebra.md#finite-field) together with its identification after extension to $\overline{\mathbb F}_q$. It determines a [Frobenius endomorphism of an algebraic group](#frobenius-endomorphism-of-an-algebraic-group), whose fixed points are the rational points. Conjugating a standard Frobenius by an [algebraic group](algebraic-geometry.md#algebraic-group) automorphism transports the rational structure, even if the automorphism is not itself rational for the original structure.

#### Frobenius endomorphism of an algebraic group

↑ **Parent:** [Rational structure on an algebraic group](#rational-structure-on-an-algebraic-group)

For an [algebraic group](algebraic-geometry.md#algebraic-group) defined over $\mathbb F_q$, its Frobenius morphism acts as entrywise $q$th powers in a standard matrix realization. Its differential is zero, and its fixed-point group is finite. A conjugate $F'=\varphi F\varphi^{-1}$ defines an isomorphic rational structure. This group morphism must be distinguished from a field [Frobenius endomorphism](galois-theory.md#frobenius-endomorphism) alone and from the convention called geometric Frobenius in Galois theory, which is inverse to the arithmetic generator on field points.

##### Lang theorem for algebraic groups

↑ **Parent:** [Frobenius endomorphism of an algebraic group](#frobenius-endomorphism-of-an-algebraic-group)

For a connected smooth [algebraic group](algebraic-geometry.md#algebraic-group) and a finite-field Frobenius $F$, the [Lang map](#lang-map) $g\mapsto g^{-1}F(g)$ is surjective. One proof uses the twisted action $x\cdot y=xyF(x)^{-1}$. Since $dF=0$, every orbit map has surjective differential, so each orbit is open; connectedness leaves only one orbit. The same differential calculation makes the Lang map étale, with finite fibres equal to left cosets of $G^F$.

###### Lang map

↑ **Parent:** [Lang theorem for algebraic groups](#lang-theorem-for-algebraic-groups)

For the [Lang map](#lang-map), $\mathcal L_F(gh)=h^{-1}\mathcal L_F(g)F(h)$. This twisted right-translation identity determines which subgroups act on its inverse images. Fibres are left $G^F$-cosets, by the [Lang theorem for algebraic groups](#lang-theorem-for-algebraic-groups).

### Affine group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affine_group)

For a finite-dimensional [vector space](vector-space.md) $V$, the affine group consists of invertible [affine maps](geometry-and-topology.md#affine-map) $x\mapsto Ax+b$, where $A$ belongs to the [general linear group](group-theory.md#general-linear-group) and $b\in V$. Its product is $(A,b)(A',b')=(AA',b+Ab')$, making it the [semidirect product](group-theory.md#semidirect-product) of the translation vector space and its general linear group. On the real line the positive-dilation subgroup is the [real affine group](#orientation-preserving-affine-group-of-the-real-line) used in the adjacent article.

### Rational representation

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rational_representation)

A [rational representation](#rational-representation) is a [group homomorphism](group-theory.md#group-homomorphism) whose matrix coefficients are [regular functions](ringed-space.md#regular-function) on the [affine algebraic group](#linear-algebraic-group). For the [general linear group](group-theory.md#general-linear-group), those functions are [polynomials](polynomial.md) in matrix entries and the inverse [determinant](linear-algebra.md#determinant). The word rational does not permit poles at points of the group.

#### Unstable vector in a rational representation

↑ **Parent:** [Rational representation](#rational-representation)

A vector is unstable if zero lies in the Zariski closure of its orbit. For complex $SL_n$, this is equivalent to an [algebraic one-parameter subgroup](#algebraic-one-parameter-subgroup) taking it to zero as $t\to0$. In the subgroup's weight decomposition, exactly the positive-weight components can occur in such a vector.

##### Hilbert-Mumford criterion for the affine null cone

↑ **Parent:** [Unstable vector in a rational representation](#unstable-vector-in-a-rational-representation)

For complex $SL_n$, choose a sequence taking an unstable vector to zero and apply singular value decomposition to each group element. Compactness gives a limiting right-unitary factor. Every nonzero torus-weight component of the transformed vector forces a strict linear inequality on the diagonal exponents. A rational solution of these finitely many strict inequalities scales to integral exponents with sum zero, producing an [algebraic one-parameter subgroup](#algebraic-one-parameter-subgroup) that takes the vector to zero. The converse follows immediately from the subgroup limit.

###### Root-multiplicity criterion for unstable binary forms

↑ **Parent:** [Hilbert-Mumford criterion for the affine null cone](#hilbert-mumford-criterion-for-the-affine-null-cone)

For $\operatorname{diag}(t,t^{-1})$, the monomial $x^{d-i}y^i$ has weight $d-2i$. Positive weights force divisibility by $x^{\lfloor d/2\rfloor+1}$. Conjugating the subgroup replaces $x$ by any nonzero linear factor. Thus a nonzero [binary form](#binary-form) is unstable exactly when a projective root has multiplicity greater than half its degree. Equality gives zero weight and does not imply instability.

#### Complete reducibility of rational GL and SL representations

↑ **Parent:** [Rational representation](#rational-representation)

For finite-dimensional [rational representations](#rational-representation) of complex $GL_m$ or $SL_m$, average a Hermitian [inner product](linear-algebra.md#inner-product) over the [compact group](topological-group.md#compact-group) $U(m)$ or $SU(m)$ using normalized [Haar measure](measure-theory.md#haar-measure). [Orthogonal complements](hilbert-space.md#orthogonal-complement) become invariant under the compact group and its complexified [Lie algebra](lie-algebra.md). The latter generates the complex group, giving invariant complements and hence complete reducibility. This conclusion does not hold for arbitrary [affine algebraic groups](#linear-algebraic-group), such as the additive group.

#### Rational representation of the general linear group

↑ **Parent:** [Rational representation](#rational-representation)

The matrix coefficients of a rational $GL_m$ action belong to its [coordinate ring](algebraic-geometry.md#coordinate-ring) $\mathbb C[g_{ab},\det(g)^{-1}]$. Multiplying the action by a sufficiently large [determinant twist](#determinant-twist) clears all [determinant](linear-algebra.md#determinant) denominators and produces a [polynomial representation](#polynomial-representation-of-the-general-linear-group). Irreducible rational actions are indexed by decreasing integer highest weights, with negative coordinates allowed.

##### Rational Schur module

↑ **Parent:** [Rational representation of the general linear group](#rational-representation-of-the-general-linear-group)

For a dominant integer tuple $\lambda$, choose $k=\max(0,-\lambda_m)$ and define $D_\lambda=\det^{-k}\otimes D_{\lambda+k(1,\ldots,1)}$, using the [polynomial](polynomial.md) [Schur module](#schur-module) on the right. The [alternant character formula for the general linear group](semisimple-lie-algebra.md#alternant-character-formula-for-the-general-linear-group) shows that a larger admissible shift yields the same irreducible representation.

###### Dual of a rational Schur module

↑ **Parent:** [Rational Schur module](#rational-schur-module)

The dual of $D_\lambda$ has dominant label $-w_0\lambda=(-\lambda_m,\ldots,-\lambda_1)$. Substitution $x_i\mapsto x_i^{-1}$ in the [alternant character formula for the general linear group](semisimple-lie-algebra.md#alternant-character-formula-for-the-general-linear-group) and reversal of determinant columns gives that [character](representation-theory.md#character-of-a-representation). The numerator and denominator reversal signs and common [monomial](polynomial.md#monomial) factors cancel.

##### Highest-weight classification of rational GL representations

↑ **Parent:** [Rational representation of the general linear group](#rational-representation-of-the-general-linear-group)

The irreducible rational $GL_m$ [modules](module-theory.md#module-mathematics) are $D_\lambda(V)=(\det V)^{\lambda_m}\otimes D_{\lambda-\lambda_m(1,\ldots,1)}(V)$. The second factor is a [Schur module](#schur-module). Clearing [determinant](linear-algebra.md#determinant) denominators reduces completeness to the [Schur algebra](#schur-algebra) classification of [polynomial](polynomial.md) [modules](module-theory.md#module-mathematics). Distinct dominant integer tuples have distinct highest torus weights. Their [characters](representation-theory.md#character-of-a-representation) are symmetric [Laurent polynomials](polynomial.md#laurent-polynomial); only [polynomial](polynomial.md) [modules](module-theory.md#module-mathematics) have [characters](representation-theory.md#character-of-a-representation) defined at every singular endomorphism.

##### Rational extension from SL to GL

↑ **Parent:** [Rational representation of the general linear group](#rational-representation-of-the-general-linear-group)

Split a rational $SL_m$ representation by its finite scalar center: on $W_k$, $\rho(\zeta I)=\zeta^kI$ for $\zeta^m=1$. The displayed extension is independent of the scalar-root choice and is a [group homomorphism](group-theory.md#group-homomorphism). A matrix coefficient of $\rho|_{W_k}$ can be represented on $SL_m$ by a sum of homogeneous [polynomials](polynomial.md) $P_d$ with $d\equiv k\pmod m$, by averaging over the scalar center. Its extension is $\sum_d(\det g)^{(k-d)/m}P_d(g)$, a [regular function](ringed-space.md#regular-function) on $GL_m$. Every invariant subspace remains invariant under this extension, so irreducibility is preserved in both directions.

##### Determinant twist

↑ **Parent:** [Rational representation of the general linear group](#rational-representation-of-the-general-linear-group)

Tensoring a [rational representation](#rational-representation) of the [general linear group](group-theory.md#general-linear-group) with a [determinant](linear-algebra.md#determinant) power shifts every highest-weight coordinate by the same integer $r$. Positive twists can clear [determinant](linear-algebra.md#determinant) denominators; negative twists supply [rational representations](#rational-representation) that do not extend to singular matrices. Twisting preserves irreducibility and dimension.

###### One-dimensional rational characters of the general linear group

↑ **Parent:** [Determinant twist](#determinant-twist)

Every one-dimensional rational $GL_m$ representation is $\det^r$ for one integer $r$. Its restriction to the diagonal torus is a [Laurent monomial](polynomial.md#laurent-monomial). Invariance under conjugation by permutation matrices forces all its exponents to agree, and density of [diagonalizable](linear-operator-theory.md#diagonalizable-matrix) invertible matrices gives the result on the whole group. For $GL_1$, the [character](representation-theory.md#character-of-a-representation) identity $p(zw)=p(z)p(w)$ directly forces a [Laurent polynomial](polynomial.md#laurent-polynomial) to be one monomial with coefficient one.

##### Polynomial representation of the general linear group

↑ **Parent:** [Rational representation of the general linear group](#rational-representation-of-the-general-linear-group)

In a [polynomial representation](#polynomial-representation-of-the-general-linear-group), every matrix coefficient is a [polynomial](polynomial.md) in the matrix entries. The action extends to the monoid of all matrices. The scalar action splits it into homogeneous [polynomial](polynomial.md) degrees; each homogeneous degree-$n$ category is the [module](module-theory.md#module-mathematics) category of the [Schur algebra](#schur-algebra) $S(m,n)$. Its irreducibles are the [Schur modules](#schur-module) $D_\lambda(\mathbb C^m)$ with $\lambda\vdash n$ and at most $m$ rows.

###### Binary form

↑ **Parent:** [Polynomial representation of the general linear group](#polynomial-representation-of-the-general-linear-group)

A binary form is a homogeneous polynomial in two variables. Degree-$d$ binary forms give the symmetric-power representation of the standard two-dimensional representation of $SL_2$, after using its invariant alternating form to identify the standard representation with its dual.

###### Binary quartic

↑ **Parent:** [Binary form](#binary-form)

A [binary quartic](#binary-quartic) is a homogeneous degree-four [polynomial](polynomial.md) in two variables. Over the complex numbers it determines four points of the [projective line](finite-group-theory.md#projective-line), counted with multiplicity. Its [discriminant](polynomial.md#discriminant) is nonzero exactly when the four points are distinct; this is also its [geometric invariant theory](representation-theory.md#geometric-invariant-theory) stability condition under $SL_2$.

###### Multiplicity-free symmetric-algebra model for polynomial GL representations

↑ **Parent:** [Polynomial representation of the general linear group](#polynomial-representation-of-the-general-linear-group)

The [symmetric algebra](linear-algebra.md#symmetric-algebra) on $V\oplus\Lambda^2V$ contains every irreducible [polynomial representation](#polynomial-representation-of-the-general-linear-group) of $GL(V)$ exactly once. Its torus [character](representation-theory.md#character-of-a-representation) is $\prod_i(1-x_i)^{-1}\prod_{i<j}(1-x_ix_j)^{-1}$, which equals $\sum_\lambda s_\lambda(x)$ by the Schur identity. Complete reducibility and linear independence of Schur [characters](representation-theory.md#character-of-a-representation) identify the summands. This is a formal graded identity: each fixed scalar degree is finite, so no analytic convergence is needed. Multiplicity one refers to irreducible [modules](module-theory.md#module-mathematics), not arbitrary reducible representations.

###### Schur functor

↑ **Parent:** [Polynomial representation of the general linear group](#polynomial-representation-of-the-general-linear-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur_functor)

For a [partition of an integer](representation-theory-of-the-symmetric-group.md#partition-of-an-integer) $\lambda\vdash n$, applying a [Young symmetrizer](representation-theory-of-the-symmetric-group.md#young-symmetrizer) of that shape to the [tensor power](linear-algebra.md#tensor-power) of each [vector space](vector-space.md) gives a Schur functor. The construction respects [linear maps](vector-space.md#linear-map) because their [tensor powers](linear-algebra.md#tensor-power) commute with place permutations. For single rows it gives [symmetric powers](linear-algebra.md#symmetric-power), and for single columns [exterior powers](linear-algebra.md#exterior-power).

###### Schur module

↑ **Parent:** [Schur functor](#schur-functor)

A Schur [module](module-theory.md#module-mathematics) is the value of a [Schur functor](#schur-functor) on a [vector space](vector-space.md). Over the [complex numbers](complex-analysis.md#complex-number) it is either zero or an irreducible [polynomial representation](#polynomial-representation-of-the-general-linear-group) of the [general linear group](group-theory.md#general-linear-group). Its [character](representation-theory.md#character-of-a-representation) is the [Schur polynomial](combinatorics.md#schur-polynomial) $s_\lambda$ in the [eigenvalues](linear-operator-theory.md#eigenvalue), and its highest weight is $\lambda$ padded with zeros.

###### Length bound for a Schur module

↑ **Parent:** [Schur module](#schur-module)

A column of length greater than $m$ antisymmetrizes more than $m$ vectors, giving zero. When there are at most $m$ rows, place the $i$th [basis](vector-space.md#basis) vector in every tensor position of row $i$. Row symmetrization multiplies by a nonzero factorial product, and column antisymmetrization is nonzero because the vectors in every column are distinct. This proves the precise nonvanishing criterion for a [Schur module](#schur-module).

###### Schur algebra

↑ **Parent:** [Polynomial representation of the general linear group](#polynomial-representation-of-the-general-linear-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur_algebra)

The Schur algebra is the [commutant](group-theory.md#centralizer) of place permutations on a [tensor power](linear-algebra.md#tensor-power). It is the linear span of the diagonal [general linear group](group-theory.md#general-linear-group) action, by [Schur–Weyl duality](#schur-weyl-duality). [Modules](module-theory.md#module-mathematics) over $S(m,n)$ correspond to homogeneous degree-$n$ [polynomial representations](#polynomial-representation-of-the-general-linear-group). Over the [complex numbers](complex-analysis.md#complex-number) it is a [semisimple algebra](associative-algebra.md#semisimple-algebra): decompose the [tensor power](linear-algebra.md#tensor-power) as a [module](module-theory.md#module-mathematics) for the semisimple [group algebra](associative-algebra.md#group-algebra) $\mathbb CS_n$, and take its endomorphism algebra.

###### Invertible tensor powers span the Schur algebra

↑ **Parent:** [Schur algebra](#schur-algebra)

The commutant of the [permutation](combinatorics.md#permutation) action on $V^{\otimes n}$ identifies with the [symmetric tensors](linear-algebra.md#symmetric-tensor) in $\operatorname{End}(V)^{\otimes n}$. [Polarization spanning of symmetric tensors](linear-algebra.md#polarization-spanning-of-symmetric-tensors) spans it by $a^{\otimes n}$. Interpolating $(a+tI)^{\otimes n}$ at $n+1$ values where $a+tI$ is invertible expresses each such power using invertible ones. Hence the [Schur algebra](#schur-algebra) is the linear span of the diagonal general linear action.

<h6 id="schur-weyl-duality">Schur–Weyl duality</h6>

↑ **Parent:** [Schur algebra](#schur-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur–Weyl_duality)

The commuting actions of the [symmetric group](finite-group-theory.md#symmetric-group) and the [general linear group](group-theory.md#general-linear-group) on a [tensor power](linear-algebra.md#tensor-power) are mutual [commutants](group-theory.md#centralizer). The displayed sum ranges over partitions with at most $\dim V$ rows. The [Specht modules](representation-theory-of-the-symmetric-group.md#specht-module) and [Schur modules](#schur-module) are the simple factors for the two actions. In particular a primitive [Young symmetrizer](representation-theory-of-the-symmetric-group.md#young-symmetrizer) selects one copy of the matching Schur [module](module-theory.md#module-mathematics).

###### Tensor cube of the defining unitary representation

↑ **Parent:** [Schur–Weyl duality](#schur-weyl-duality)

For the [unitary group](topological-group.md#unitary-group) $U(n)$ with $n\geq3$, the third [tensor power](linear-algebra.md#tensor-power) of its [defining representation](lie-algebra.md#defining-representation-of-a-matrix-lie-algebra) decomposes as displayed. The first two summands have [highest weights](semisimple-lie-algebra.md#highest-weight-of-a-representation) $(3,0,\ldots)$ and $(1,1,1,0,\ldots)$ and [dimensions](vector-space.md#dimension-vector-space) $\binom{n+2}3$ and $\binom n3$. The mixed summand has [highest weight](semisimple-lie-algebra.md#highest-weight-of-a-representation) $(2,1,0,\ldots)$ and [dimension](vector-space.md#dimension-vector-space) $n(n^2-1)/3$. In the three-dimensional [weight space](semisimple-lie-algebra.md#weight-space) spanned by [permutations](combinatorics.md#permutation) of $e_1\otimes e_1\otimes e_2$, the vectors killed by all positive [root vectors](semisimple-lie-algebra.md#root-vector) have coefficient sum zero, giving multiplicity two. For $n=2$, the exterior cube vanishes and $V_{(2,1)}=\det\otimes\mathbb C^2$.

###### Trace of a permuted tensor power

↑ **Parent:** [Schur–Weyl duality](#schur-weyl-duality)

If $\sigma$ has $\alpha_r$ cycles of length $r$, contraction of matrix entries around its cycles gives $\operatorname{tr}(\sigma\xi^{\otimes n})=\prod_r\operatorname{tr}(\xi^r)^{\alpha_r}$. The formula holds for every [endomorphism](algebra.md#endomorphism), not only diagonalizable ones. The [Schur–Weyl duality](#schur-weyl-duality) decomposition equates it with a sum of products of Specht and Schur [characters](representation-theory.md#character-of-a-representation).

###### Young-symmetrizer tensor decomposition

↑ **Parent:** [Schur–Weyl duality](#schur-weyl-duality)

The standard-tableau right-ideal decomposition of $\mathbb CS_n$, tensored over that algebra with $V^{\otimes n}$, gives this direct sum of [general linear group](group-theory.md#general-linear-group) [modules](module-theory.md#module-mathematics). With $e_t=h_t/H_\lambda$, the map $e_t\mathbb CS_n\otimes T\to e_tT$ is an isomorphism. Individual summands generally need not be [symmetric group](finite-group-theory.md#symmetric-group) [submodules](module-theory.md#submodule); instead each is a [Schur module](#schur-module) for the commuting action.

### Lie algebra of an affine algebraic group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

The Lie algebra of an affine algebraic group $G$ is the tangent space $T_eG$ at its identity. Its bracket is the commutator of the corresponding left-invariant derivations of the coordinate ring.

### Descent of an irreducible SL2 representation to PGL2

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

The irreducible rational representations of $SL_2(\mathbb C)$ are $\operatorname{Sym}^n(\mathbb C^2)$. Such a representation descends through $SL_2\to PGL_2$ exactly when the central element $-I$ acts trivially, which holds exactly when $n$ is even.

### Faithful representation of an affine algebraic group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

Every affine algebraic group has a faithful finite-dimensional rational [group representation](representation-theory.md#group-representation). Choose algebra generators of $k[G]$ and place them in a finite-dimensional subspace stable under right translations. An element acting trivially on that subspace has the same coordinate values as the identity and therefore is the identity.

### Left-right regular representation of an affine algebraic group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

The group $G\times G$ acts on $k[G]$ by

$$
((a,b)f)(x)=f(a^{-1}xb).
$$

For $G=\mathbb G_m$, this gives $k[G]=\bigoplus_{r\in\mathbb Z}k_{(-r,r)}$. For $G=\mathbb G_a$, the action factors through $(a,b)\mapsto b-a$ and the degree filtration of $k[t]$ has trivial one-dimensional successive quotients.

### Semisimple element of an affine algebraic group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

An element of an affine algebraic group is semisimple when its image in one, equivalently every, faithful finite-dimensional representation is a diagonalizable linear map.

### Unipotent element of an affine algebraic group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

An element of an affine algebraic group is unipotent when its image in one, equivalently every, faithful finite-dimensional representation has every eigenvalue equal to one.

#### Unipotent matrix

↑ **Parent:** [Unipotent element of an affine algebraic group](#unipotent-element-of-an-affine-algebraic-group)

A square [matrix](vector-space.md#matrix) $U$ is unipotent when $U-I$ is nilpotent. Over an [algebraically closed field](algebra.md#algebraically-closed-field), this is equivalent to all [eigenvalues](linear-operator-theory.md#eigenvalue) being one. If $j$ belongs to a [nilpotent ideal](commutative-algebra.md#nilpotent-ideal) of an operator algebra, $I+j$ is a unipotent matrix. This realizes the radical factor in the [Levi decomposition of a quiver automorphism group](algebra.md#levi-decomposition-of-a-quiver-automorphism-group).

### Jordan decomposition in an affine algebraic group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

This is the multiplicative [Jordan–Chevalley decomposition](linear-operator-theory.md#jordan-chevalley-decomposition) in a [linear algebraic group](#linear-algebraic-group). Every element $g$ of an affine algebraic group has unique commuting semisimple and unipotent parts $g_s,g_u$ such that $g=g_sg_u$. The construction agrees with the multiplicative [Jordan decomposition](linear-operator-theory.md#jordan-normal-form) in every rational representation.

### Derived subgroup of an affine algebraic group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

The derived subgroup $[G,G]$ is the closed algebraic subgroup generated by the commutators $xyx^{-1}y^{-1}$. If $G$ is connected, images of finite products of commutators are connected and their closures stabilize by dimension, which shows that $[G,G]$ is connected.

#### Solvable affine algebraic group

↑ **Parent:** [Derived subgroup of an affine algebraic group](#derived-subgroup-of-an-affine-algebraic-group)

An affine algebraic group is solvable when its derived series reaches the identity. A connected solvable affine algebraic group can be conjugated into an upper triangular matrix group by the [Lie-Kolchin theorem](#lie-kolchin-theorem).

##### Lie-Kolchin theorem

↑ **Parent:** [Solvable affine algebraic group](#solvable-affine-algebraic-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lie–Kolchin_theorem)

Every connected solvable affine algebraic subgroup of $\operatorname{GL}(V)$ preserves a complete flag in $V$, equivalently it is conjugate to a subgroup of the upper triangular matrices.

### Diagonalizable group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diagonalizable_group)

A diagonalizable algebraic group is isomorphic to a closed subgroup of a product of copies of $\mathbb G_m$. Every rational representation of such a group decomposes into weight spaces.

### Reductive group

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reductive_group)

A reductive algebraic group is a smooth connected affine algebraic group whose largest connected normal [unipotent algebraic group](#unipotent-algebraic-group) is trivial.

#### Finite group of Lie type

↑ **Parent:** [Reductive group](#reductive-group)

A finite group of Lie type is obtained from rational points of a connected [reductive algebraic group](#reductive-group) with a suitable [Frobenius endomorphism of an algebraic group](#frobenius-endomorphism-of-an-algebraic-group), often followed by central quotient or passage to a derived subgroup. Its complex representations combine finite-group [character theory](representation-theory.md#character-theory) with the geometry of [Borel subgroups](#borel-subgroup), [maximal algebraic tori](toric-geometry.md#maximal-algebraic-torus), and the [Weyl group](semisimple-lie-algebra.md#weyl-group).

##### Harish-Chandra induction

↑ **Parent:** [Finite group of Lie type](#finite-group-of-lie-type)

For a rational [parabolic subgroup](#parabolic-subgroup) $P=L\ltimes U$, use [inflation of a group representation](representation-theory.md#inflation-of-a-group-representation) for a complex $L^F$-module across $P^F\to L^F$ and induce it to $G^F$. This is Harish-Chandra induction. Its adjoint, [Harish-Chandra restriction](#harish-chandra-restriction), takes $U^F$-invariants. These are ordinary finite-group [group representation](representation-theory.md#group-representation) functors and should not be confused with general [Deligne-Lusztig induction](#deligne-lusztig-induction) from a nonrational Borel.

###### Mackey formula for Harish-Chandra induction

↑ **Parent:** [Harish-Chandra induction](#harish-chandra-induction)

For rational [parabolic subgroups](#parabolic-subgroup) $P=LU$ and $Q=MV$, define $\mathcal S(M,L)=\{x:M\cap{}^xL\text{ contains a maximal algebraic torus of }G\}$. Then $\,{}^*R_M^G R_L^G$ is the sum over $M^F\backslash\mathcal S(M,L)^F/L^F$ of $R_{M\cap{}^xL}^{M}\,{}^*R_{M\cap{}^xL}^{{}^xL}\operatorname{ad}x$, with the intersection parabolics understood. It follows from ordinary finite-group [Mackey restriction formula](representation-theory.md#mackey-restriction-formula), taking $V^F$-invariants, and the compatible-Levi intersection lemma for parabolics.

###### Harish-Chandra restriction

↑ **Parent:** [Harish-Chandra induction](#harish-chandra-induction)

Restriction first views a $G^F$-module as a $P^F$-module, then takes the subspace fixed by the unipotent radical. The resulting $L^F$-module is adjoint to [Harish-Chandra induction](#harish-chandra-induction) by ordinary [Frobenius reciprocity](representation-theory.md#frobenius-reciprocity). Over characteristic zero, averaging makes invariants exact and identifies them with coinvariants.

###### Cuspidal representation of a finite reductive group

↑ **Parent:** [Harish-Chandra restriction](#harish-chandra-restriction)

An irreducible complex $G^F$-module is cuspidal if its [Harish-Chandra restriction](#harish-chandra-restriction) is zero for every proper rational [parabolic subgroup](#parabolic-subgroup). By adjunction, it occurs in no [Harish-Chandra induction](#harish-chandra-induction) from a proper rational [Levi subgroup](#levi-subgroup). This is a finite-group notion, distinct from a cuspidal automorphic representation.

##### Deligne-Lusztig theory

↑ **Parent:** [Finite group of Lie type](#finite-group-of-lie-type)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Deligne–Lusztig_theory)

Deligne-Lusztig theory constructs [virtual characters](representation-theory.md#virtual-character) of [finite groups of Lie type](#finite-group-of-lie-type) from compactly supported [étale cohomology](algebraic-geometry.md#etale-cohomology) of varieties associated with Frobenius and flags. [Rational maximal tori](toric-geometry.md#rational-maximal-torus) and their finite-group [characters](representation-theory.md#character-of-a-representation) provide induction data, while the geometry explains character orthogonality and cuspidality.

###### Deligne-Lusztig induction

↑ **Parent:** [Deligne-Lusztig theory](#deligne-lusztig-theory)

For a [rational maximal torus](toric-geometry.md#rational-maximal-torus) $T$, choose a [Borel subgroup](#borel-subgroup) containing it with [unipotent radical](#unipotent-radical) $U$. The alternating compactly supported [étale cohomology](algebraic-geometry.md#etale-cohomology) of $\mathcal L_F^{-1}(U)$, in the appropriate $T^F$-isotypic component, defines the [virtual character](representation-theory.md#virtual-character) of $G^F$ $R_T^G(\theta)$. It is independent of the chosen Borel. When the [Borel subgroup](#borel-subgroup) is rational, this is ordinary induction from its rational points after [inflation of a group representation](representation-theory.md#inflation-of-a-group-representation) from $T^F$.

###### Harish-Chandra restriction of a Deligne-Lusztig character

↑ **Parent:** [Deligne-Lusztig induction](#deligne-lusztig-induction)

For a rational [Levi subgroup](#levi-subgroup) $M$ of a rational [parabolic subgroup](#parabolic-subgroup) and a [rational maximal torus](toric-geometry.md#rational-maximal-torus) $T$, the torus case of the induction-restriction formula is

$$
{}^*R_M^G R_T^G(\theta)=\sum_{x\in M^F\backslash\{g\in G^F:{}^gT\subset M\}/T^F}R_{{}^xT}^{M}({}^x\theta).
$$

In particular it vanishes if there is no rational conjugate of $T$ in $M$. If $T\subset M$, transitivity gives $R_T^G=R_M^G R_T^M$. Together with adjunction these identities show that an irreducible character up to sign arising from $T$ is cuspidal exactly when $T$ is elliptic.

###### Principal series of a finite reductive group

↑ **Parent:** [Deligne-Lusztig induction](#deligne-lusztig-induction)

For a rational [Borel subgroup](#borel-subgroup) $B=TU$, the principal series is $\operatorname{Ind}_{B^F}^{G^F}\widetilde\theta$, with $\widetilde\theta$ inflated from a [linear character](representation-theory.md#linear-character) of $T^F$. The [Mackey restriction formula](representation-theory.md#mackey-restriction-formula) and rational [Bruhat decomposition](#bruhat-decomposition) give its self-inner-product as the size of the Weyl stabilizer of $\theta$. It is irreducible precisely when that stabilizer is trivial.

###### Irreducibility of the split SL3 principal series

↑ **Parent:** [Principal series of a finite reductive group](#principal-series-of-a-finite-reductive-group)

For $N=q-1$, write a diagonal-torus character as $\theta(\operatorname{diag}(a,b,(ab)^{-1}))=\chi(a)^r\chi(b)^s$, with $\chi$ a generator of the character group of $\mathbb F_q^\times$. Its Weyl stabilizer is trivial exactly when $r,s,r-s$ are all nonzero modulo $N$ and, if $3\mid N$, the unordered pair $\{r,s\}$ is not $\{N/3,2N/3\}$. The first conditions exclude transpositions; the exceptional pair excludes cyclic permutation of three characters modulo a common twist.

###### Deligne-Lusztig variety

↑ **Parent:** [Deligne-Lusztig theory](#deligne-lusztig-theory)

For a connected [reductive algebraic group](#reductive-group) and a [Weyl group](semisimple-lie-algebra.md#weyl-group) element $w$, this locally closed subset of the [flag variety](#generalized-flag-variety) consists of flags in relative position $w$ to their Frobenius image. For rational $B$ it is $\mathcal L_F^{-1}(B\dot wB)/B$, using the twisted right action identity of the [Lang map](#lang-map). Its dimension is the length of $w$.

###### Unipotent quotient in a Deligne-Lusztig variety

↑ **Parent:** [Deligne-Lusztig variety](#deligne-lusztig-variety)

Choose rational $B=TU$, a representative $\dot w$, and $x$ with $x^{-1}F(x)=\dot w$. Set $T'=xTx^{-1}$ and $U'=F(xUx^{-1})$. Then $T'$ is rational, and

$$
\mathcal L_F^{-1}(U')/[(U'\cap F^{-1}(U'))T'^F]\cong X(w).
$$

The map sends $h$ to $hxB$. Quotienting only by the finite group $T'^F$ leaves fibres isomorphic to the positive-dimensional unipotent intersection when that intersection is nontrivial. For $w=1$ in $\mathrm{SL}_2$, this is an affine-line fibre over each rational flag, so the missing quotient cannot be ignored in a variety isomorphism.

#### Borel subgroup

↑ **Parent:** [Reductive group](#reductive-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Borel_subgroup)

A Borel subgroup is a maximal closed connected solvable subgroup of an affine algebraic group.

##### Parabolic subgroup

↑ **Parent:** [Borel subgroup](#borel-subgroup)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parabolic_subgroup)

A parabolic subgroup of a connected reductive group is a closed subgroup containing a [Borel subgroup](#borel-subgroup). Its quotient in the group is projective.

###### Levi subgroup

↑ **Parent:** [Parabolic subgroup](#parabolic-subgroup)

A [Levi subgroup](#levi-subgroup) appears in a group version of a [Levi decomposition](#levi-decomposition). A Levi subgroup is a reductive complement to the unipotent radical of a parabolic subgroup.

##### Generalized flag variety

↑ **Parent:** [Borel subgroup](#borel-subgroup)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_flag_variety)

For a connected reductive algebraic group $G$ and a [Borel subgroup](#borel-subgroup) $B$, the quotient $G/B$ is its complete flag variety. Quotients $G/P$ by [parabolic subgroups](#parabolic-subgroup) are partial flag varieties.

#### Root datum

↑ **Parent:** [Reductive group](#reductive-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Root_datum)

A root datum is a quadruple $(X^*,\Phi,X_*,\Phi^\vee)$ of dual lattices, roots, and coroots with the natural perfect pairing and reflection axioms. A reductive group with maximal torus $T$ has $X^*=X^*(T)$ and $X_*=X_*(T)$.

#### Bruhat decomposition

↑ **Parent:** [Reductive group](#reductive-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bruhat_decomposition)

For a connected reductive algebraic group, a [Borel subgroup](#borel-subgroup) $B$, and a maximal torus $T\subseteq B$, the [Weyl group](semisimple-lie-algebra.md#weyl-group) $W=N_G(T)/T$ indexes the double cosets:

$$
G=\bigsqcup_{w\in W}B\dot wB.
$$

##### Relative position of Borel subgroups

↑ **Parent:** [Bruhat decomposition](#bruhat-decomposition)

The [relative position of Borel subgroups](#relative-position-of-borel-subgroups) $B_1,B_2$ is the [Weyl group](semisimple-lie-algebra.md#weyl-group) index of their simultaneous conjugacy orbit. After moving the first subgroup to a fixed $B$, the second has the form $gBg^{-1}$ and its index is the double coset $BgB$. This identifies the diagonal action on pairs of flags with the [Bruhat decomposition](#bruhat-decomposition).

##### Bruhat decomposition of a BN-pair

↑ **Parent:** [Bruhat decomposition](#bruhat-decomposition)

This is the [Bruhat decomposition](#bruhat-decomposition) associated with a [BN-pair](#bn-pair). The Bruhat decomposition is the disjoint union

$$
G=\bigsqcup_{w\in W}B\dot wB
$$

associated with a [BN-pair](#bn-pair).

### Algebraic-group torsor

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)

For an algebraic group $H$, a flat $H$-torsor over $Y$ is a faithfully flat morphism $X\to Y$ with a right $H$-action such that $X\times H\to X\times_YX$, $(x,h)\mapsto(x,xh)$, is an isomorphism. A Zariski torsor additionally becomes $U\times H$ on a Zariski open cover of $Y$.

### Unipotent

↑ **Parent:** [Linear algebraic group](#linear-algebraic-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unipotent)

An element $u$ of a [ring](commutative-algebra.md#ring) is [unipotent](#unipotent) when $u-1$ is [nilpotent](commutative-algebra.md#nilpotent). For a matrix, this says that every [eigenvalue](linear-operator-theory.md#eigenvalue) is one. A [unipotent algebraic group](#unipotent-algebraic-group) consists of unipotent elements in a faithful linear representation.

#### Unipotent algebraic group

↑ **Parent:** [Unipotent](#unipotent)

A [unipotent algebraic group](#unipotent-algebraic-group) is built from [unipotent](#unipotent) elements. A unipotent algebraic group is an affine algebraic group all of whose elements are unipotent. The [Kolchin theorem](#kolchin-theorem) embeds it into an upper unitriangular group.

##### Unipotent radical

↑ **Parent:** [Unipotent algebraic group](#unipotent-algebraic-group)

It is the largest connected normal unipotent subgroup of a [linear algebraic group](#linear-algebraic-group). A connected [reductive algebraic group](#reductive-group) has trivial unipotent radical. The subgroup $1+J(E)$ of a finite-dimensional algebra's unit group is closed, connected and unipotent.

##### Kolchin theorem

↑ **Parent:** [Unipotent algebraic group](#unipotent-algebraic-group)

Every unipotent algebraic subgroup of $\operatorname{GL}_n$ is conjugate to a subgroup of the upper unitriangular group. The filtration by vanishing initial superdiagonals then proves that every unipotent algebraic group is a [nilpotent group](group-theory.md#nilpotent-group).

## Lie group

↑ **Parent:** [Lie theory](lie-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lie_group)

A Lie group is a [group](group.md) that is also a [smooth manifold](differential-geometry.md#smooth-manifold), with smooth multiplication and inversion. Its tangent space at the identity carries a natural [Lie algebra](lie-algebra.md) structure.

### Lie groups have no small subgroups

↑ **Parent:** [Lie group](#lie-group)

Choose an injective [local exponential chart](#local-exponential-chart) on a ball of radius $r$ in the [Lie algebra](lie-algebra.md), and let $0<\varepsilon<r/2$. The neighborhood $\exp(B_\varepsilon)$ contains no nontrivial subgroup. Otherwise it contains an element $\exp X$ with $0<\|X\|<\varepsilon$. Choose the first integer $m$ with $m\|X\|\geq\varepsilon$. Then $\varepsilon\leq m\|X\|<2\varepsilon<r$, so chart injectivity puts $(\exp X)^m=\exp(mX)$ outside $\exp(B_\varepsilon)$, a contradiction. Zero-dimensional Lie groups have the singleton identity as such an open neighborhood.

### G2 (mathematics)

↑ **Parent:** [Lie group](#lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/G2_(mathematics))

$G_2$ denotes an exceptional [Lie group](#lie-group) and its associated [Lie algebra](lie-algebra.md), of rank two and dimension fourteen. Its roots form the [G2 root system](semisimple-lie-algebra.md#g2-root-system). The compact real form is the [automorphism group](group-theory.md#automorphism-group) of the octonion algebra; other real forms and the complex [Lie algebra](lie-algebra.md) have the same complex root-system type.

<h3 id="lie-group-lie-algebra-correspondence">Lie group–Lie algebra correspondence</h3>

↑ **Parent:** [Lie group](#lie-group)

Differentiation sends [Lie groups](#lie-group) to [Lie algebras](lie-algebra.md) and smooth [group homomorphisms](group-theory.md#group-homomorphism) to bracket-preserving [linear maps](vector-space.md#linear-map). On connected [simply connected](algebraic-topology.md#simply-connected-space) [Lie groups](#lie-group), this is an equivalence with finite-dimensional real [Lie algebras](lie-algebra.md): the [Lie third theorem](#lie-third-theorem) gives existence, and [integration of a Lie algebra homomorphism](lie-algebra.md#integration-of-a-lie-algebra-homomorphism) gives unique maps. General connected [groups](group.md) require discrete central quotient data, and disconnected [groups](group.md) additionally require component and conjugation data.

### Lie third theorem

↑ **Parent:** [Lie group](#lie-group)

Every finite-dimensional real [Lie algebra](lie-algebra.md) is the [Lie algebra](lie-algebra.md) of a connected [simply connected](algebraic-topology.md#simply-connected-space) [Lie group](#lie-group). One construction first uses the [Ado theorem](lie-algebra.md#ado-s-theorem) to embed it into a matrix [Lie algebra](lie-algebra.md), integrates the corresponding left-invariant distribution by the [Frobenius theorem](differential-geometry.md#frobenius-theorem) to a connected immersed [Lie subgroup](#lie-subgroup), and then takes a [universal covering Lie group](#universal-covering-lie-group). The immersed [subgroup](group.md#subgroup) need not be closed; taking its ambient closure may change its [Lie algebra](lie-algebra.md).

### Universal covering Lie group

↑ **Parent:** [Lie group](#lie-group)

The [universal cover](algebraic-topology.md#universal-cover) of a connected [Lie group](#lie-group) carries a unique lifted [Lie group](#lie-group) structure with a chosen identity, making its [covering map](algebraic-topology.md#covering-space) a [Lie group homomorphism](#lie-group-homomorphism). The kernel is a discrete central [subgroup](group.md#subgroup): conjugation of any kernel element is a continuous map from a connected [group](group.md) into a discrete set, hence constant. Every connected [Lie group](#lie-group) is therefore a quotient of its [simply connected](algebraic-topology.md#simply-connected-space) cover by a discrete central [subgroup](group.md#subgroup).

### Complex Lie group

↑ **Parent:** [Lie group](#lie-group)

A complex [Lie group](#lie-group) is a [complex manifold](complex-geometry.md#complex-manifold) whose multiplication and inversion are [holomorphic maps between complex manifolds](complex-geometry.md#holomorphic-map-between-complex-manifolds). Its [tangent space](differential-geometry.md#tangent-space) at the identity is a complex [Lie algebra](lie-algebra.md); the [Adjoint representation of a Lie group](#adjoint-representation-of-a-lie-group) and the [Lie exponential map](#exponential-map-of-a-lie-group) are holomorphic. Compatibility with a [complex manifold](complex-geometry.md#complex-manifold) structure is essential: an arbitrary even-dimensional real [Lie group](#lie-group) need not have holomorphic multiplication.

#### Compact connected complex Lie groups are complex tori

↑ **Parent:** [Complex Lie group](#complex-lie-group)

Every scalar [holomorphic function](complex-analysis.md#holomorphic-function) on a compact connected [complex manifold](complex-geometry.md#complex-manifold) is constant by the [maximum modulus principle](complex-analysis.md#maximum-modulus-principle). Apply this to each entry of the holomorphic [Adjoint representation of a Lie group](#adjoint-representation-of-a-lie-group); its value is constantly the identity. Differentiation makes the complex [Lie algebra](lie-algebra.md) abelian, hence connectedness makes the [group](group.md) abelian. The holomorphic [Lie exponential map](#exponential-map-of-a-lie-group) identifies it with $\mathbb C^n$ modulo a [discrete subgroup](topological-group.md#discrete-subgroup). Compactness forces that [subgroup](group.md#subgroup) to span the underlying [real vector space](vector-space.md#real-vector-space), giving a full-rank [Euclidean lattice](fourier-analysis.md#euclidean-lattice) and a [complex torus](complex-geometry.md#complex-torus).

### Abelian Lie group

↑ **Parent:** [Lie group](#lie-group)

An abelian [Lie group](#lie-group) has commutative multiplication. Its [Lie algebra](lie-algebra.md) is an [abelian Lie algebra](lie-algebra.md#abelian-lie-algebra), and its [Lie exponential map](#exponential-map-of-a-lie-group) is a [group homomorphism](group-theory.md#group-homomorphism) from the additive [Lie algebra](lie-algebra.md). Conversely, an additive [Lie exponential map](#exponential-map-of-a-lie-group) forces the [identity component of a Lie group](#identity-component-of-a-lie-group) to be abelian, but does not force all disconnected components to commute.

#### Classification of connected abelian Lie groups

↑ **Parent:** [Abelian Lie group](#abelian-lie-group)

For a connected [abelian Lie group](#abelian-lie-group), the [Lie exponential map](#exponential-map-of-a-lie-group) is an additive [group homomorphism](group-theory.md#group-homomorphism) and a local [diffeomorphism](geometry-and-topology.md#diffeomorphism) at zero. Its image is an open [subgroup](group.md#subgroup), hence the whole connected [group](group.md). Its kernel is a [discrete additive subgroup of a real vector space](topological-group.md#discrete-additive-subgroup-of-a-real-vector-space). A basis of that kernel identifies it with $\mathbb Z^r$ inside $\mathbb R^n$, giving the displayed classification. The compact factors record periods of [one-parameter subgroups](#one-parameter-subgroup).

### Sol Lie group

↑ **Parent:** [Lie group](#lie-group)

The multiplication $(x',y',z')(x,y,z)=(x'+e^{-z'}x,y'+e^{z'}y,z'+z)$ defines the three-dimensional Sol [Lie group](#lie-group). Its [left-invariant vector fields](#left-invariant-vector-field) $e^{-z}\partial_x,e^z\partial_y,\partial_z$ have dual [coframe](fiber-bundle.md#coframe) $e^zdx,e^{-z}dy,dz$. Their sum of squares is a [left-invariant metric](#left-invariant-metric), $ds^2=e^{2z}dx^2+e^{-2z}dy^2+dz^2$.

### Semisimple Lie group

↑ **Parent:** [Lie group](#lie-group)

A real or complex [Lie group](#lie-group) is semisimple when its [Lie algebra](lie-algebra.md) is semisimple. For a real group, the [Killing form](lie-algebra.md#killing-form) then defines a nondegenerate [bi-invariant pseudo-Riemannian metric](#bi-invariant-pseudo-riemannian-metric). Compact semisimple groups have negative-definite [Killing form](lie-algebra.md#killing-form); noncompact examples such as $SL(2,\mathbb R)$ have indefinite [Killing form](lie-algebra.md#killing-form). A disconnected group can also have a [semisimple Lie algebra](semisimple-lie-algebra.md), so connectedness is a separate hypothesis when integrating infinitesimal actions.

### Free step-N nilpotent Lie group

↑ **Parent:** [Lie group](#lie-group)

Inside the [truncated tensor algebra](linear-algebra.md#truncated-tensor-algebra), let $\mathfrak g^N(V)$ be the span of iterated [Lie brackets](lie-algebra.md#lie-bracket) of elements of $V$ of lengths at most $N$. Its exponential is the connected simply connected free nilpotent [Lie group](#lie-group) of step $N$, with tensor multiplication. The bracket is the commutator in the [tensor algebra](linear-algebra.md#tensor-algebra). Its grading defines dilations that multiply degree $k$ by $\lambda^k$.

#### Step-2 planar group coordinates

↑ **Parent:** [Free step-N nilpotent Lie group](#free-step-n-nilpotent-lie-group)

Write a group element as $\exp(v+a[e_1,e_2])$. The step-two Baker-Campbell-Hausdorff formula gives the displayed multiplication and inverse $(-v,-a)$. The scalar $a$ is the antisymmetric second signature coordinate, which equals the signed area for a closed planar path. The [Carnot-Carathéodory distance](differential-geometry.md#carnot-caratheodory-distance) is comparable to $|v|+|a|^{1/2}$ near the identity, with the same homogeneous scaling globally.

### Loop group

↑ **Parent:** [Lie group](#lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loop_group)

The loop group of a [Lie group](#lie-group) is the group of smooth maps from the circle to that group, with pointwise multiplication and the smooth-function topology. Rotation of the source circle acts by group automorphisms. For $G=U(1)$, every loop has the form $z^w e^{ih(z)}$, where $w\in\mathbb Z$ is its [winding number](complex-analysis.md#winding-number) and $h$ is a smooth real periodic function determined up to addition of an integer multiple of $2\pi$.

<h4 id="positive-energy-representation-of-the-loop-group-of-u-1">Positive energy representation of the loop group of U(1)</h4>

↑ **Parent:** [Loop group](#loop-group)

Such a continuous [projective unitary representation](quantum-mechanics.md#projective-unitary-representation) admits strongly continuous rotations whose self-adjoint generator is bounded below and whose adjoint action rotates the loops. In the basic fermionic construction, integer one-particle modes are filled below zero. The rotation energy counts nonnegative particle energies and positive hole energies. It has finite-dimensional integer eigenspaces and implements circle rotations. Tensor products give higher nonnegative integer levels.

<h5 id="loop-group-two-cocycle-for-u-1">Loop group two-cocycle for U(1)</h5>

↑ **Parent:** [Positive energy representation of the loop group of U(1)](#positive-energy-representation-of-the-loop-group-of-u-1)

Write a loop as $z^w e^{ih}$ with $h$ smooth real periodic and $h_0$ its mean. For the level-one representation with modes filled below zero and $\omega(h,k)=(2\pi)^{-1}\int_0^{2\pi}h'k$, choose implementers $U(w,h)=S^w e^{iA(h)}$, where $S$ increases charge by one, $SQS^*=Q-I$, and $[A(h),A(k)]=i\omega(h,k)I$. Their product differs from $U(w+v,h+k)$ by the displayed [two-cocycle](group-theory.md#two-cocycle). Its phase is bilinear, which verifies the cocycle identity; integer $v$ makes it independent of the $2\pi$ ambiguity in $h_0$. Rephasing implementers changes it by a [group coboundary](group-theory.md#group-coboundary).

### Bi-invariant pseudo-Riemannian metric

↑ **Parent:** [Lie group](#lie-group)

A nondegenerate invariant symmetric [bilinear form](linear-algebra.md#bilinear-form) on a [Lie algebra](lie-algebra.md) extends by translation to a metric preserved by both left and right translation. It may have indefinite signature. Its [Levi-Civita connection](general-relativity.md#levi-civita-connection) is $\nabla_XY=\frac12[X,Y]$ for [left-invariant vector fields](#left-invariant-vector-field), and its [Ricci tensor](general-relativity.md#ricci-tensor) is $-K/4$. Choosing the nondegenerate [Killing form](lie-algebra.md#killing-form) of a semisimple [Lie algebra](lie-algebra.md) yields a canonical indefinite [Einstein manifold](second-fundamental-form.md#einstein-manifold); compact groups instead admit the positive metric $-K$.

#### Neutral invariant metrics on the free two-step Lie algebra on three generators

↑ **Parent:** [Bi-invariant pseudo-Riemannian metric](#bi-invariant-pseudo-riemannian-metric)

Let $[e_1,e_2]=e_6$, $[e_1,e_3]=e_4$ and $[e_2,e_3]=e_5$, with $e_4,e_5,e_6$ central. The symmetric tensor $S=e_1\otimes e_5+e_5\otimes e_1+e_3\otimes e_6+e_6\otimes e_3-e_2\otimes e_4-e_4\otimes e_2$ is invariant under the [Adjoint representation of a Lie algebra](lie-algebra.md#adjoint-representation-of-a-lie-algebra): the derivation action of each of $e_1,e_2,e_3$ cancels in pairs. For $t\ne0$, $Q=tS+\sum_{j=4}^6a_j e_j\otimes e_j$ has determinant $-t^6$ and inverse metric $g=t^{-1}S(\lambda)-t^{-2}(a_5(\lambda^1)^2+a_4(\lambda^2)^2+a_6(\lambda^3)^2)$ in the dual coframe. Its three hyperbolic planes give the displayed [metric signature](topology.md#metric-signature). On a connected [Lie group](#lie-group) this supplies a four-parameter family of [bi-invariant pseudo-Riemannian metrics](#bi-invariant-pseudo-riemannian-metric). Disconnected components must preserve the tensor separately; the automorphism reversing $e_1,e_4,e_6$ while fixing the other generators reverses $S$ and prevents this extension.

#### Killing-form Einstein metric

↑ **Parent:** [Bi-invariant pseudo-Riemannian metric](#bi-invariant-pseudo-riemannian-metric)

On a real semisimple [Lie group](#lie-group), the nondegenerate invariant [Killing form](lie-algebra.md#killing-form) gives a [bi-invariant pseudo-Riemannian metric](#bi-invariant-pseudo-riemannian-metric). For left-invariant fields the [Koszul formula](fiber-bundle.md#koszul-formula) gives $\nabla_XY=[X,Y]/2$ and $R(X,Y)Z=-[[X,Y],Z]/4$. Taking the trace gives $\operatorname{Ric}(Y,Z)=-B(Y,Z)/4$, proving the Einstein property. On a compact [semisimple group](#semisimple-lie-group), $-B$ is positive definite and has Einstein constant $1/4$. The indefinite general construction is not a proof of existence of a positive-definite bi-invariant metric on a noncompact group.

### Compact Lie group

↑ **Parent:** [Lie group](#lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compact_Lie_group)

A compact Lie group is a [Lie group](#lie-group) whose underlying manifold is [compact](topology.md#compact-space). Averaging any positive inner product over its [Haar measure](measure-theory.md#haar-measure) supplies an invariant inner product on each finite-dimensional representation, including the [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra).

#### Real torus

↑ **Parent:** [Compact Lie group](#compact-lie-group)

A real torus is the compact [Lie group](#lie-group) obtained by identifying real vectors differing by integer vectors, with addition induced from Euclidean addition. It is a finite product of circle groups and has normalized [Haar measure](measure-theory.md#haar-measure). Dimension two is the familiar surface [torus](topology.md#torus), but toral dynamics and Fourier characters naturally use arbitrary finite dimension.

#### Weyl integration formula

↑ **Parent:** [Compact Lie group](#compact-lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weyl_integration_formula)

Let $G$ be a [connected](geometry-and-topology.md#connected-space) [compact Lie group](#compact-lie-group), $T$ a [maximal torus](#maximal-torus), and $W$ its [Weyl group](semisimple-lie-algebra.md#weyl-group). With normalized [Haar measures](measure-theory.md#haar-measure) and $D(t)=\prod_{\alpha>0}(1-e^{-\alpha}(t))$, every [continuous](calculus.md#continuous-function) [class function](representation-theory.md#class-function) satisfies $\int_G f(g)\,dg=|W|^{-1}\int_T f(t)|D(t)|^2\,dt$. For a general [continuous function](calculus.md#continuous-function), replace $f(t)$ by its average $\int_{G/T}f(gtg^{-1})\,d(gT)$. [Conjugation](group-theory.md#conjugation) from $G/T\times T$ covers the regular elements $|W|$ times, and its real [Jacobian determinant](calculus.md#jacobian-determinant) is $|D(t)|^2$.

##### Conjugation Jacobian for a compact Lie group

↑ **Parent:** [Weyl integration formula](#weyl-integration-formula)

For a connected [compact Lie group](#compact-lie-group) with [maximal torus](#maximal-torus) $T$, the map $q:G/T\times T\to G$, $q(xT,t)=xtx^{-1}$, has the displayed real [Jacobian determinant](calculus.md#jacobian-determinant). Choose an invariant [inner product](linear-algebra.md#inner-product) and identify the tangent space of $G/T$ with $\mathfrak t^\perp$. Translation of the derivative at $(T,t)$ to the identity gives $(X,Y)\mapsto(\operatorname{Ad}(t^{-1})-I)X+Y$. Each pair of opposite [roots of a root system](semisimple-lie-algebra.md#root-of-a-root-system) corresponds to a real two-plane on which the determinant is $|1-\alpha(t)|^2$. The torus direction has determinant one. Normalized quotient and [Haar measures](measure-theory.md#haar-measure) have matching volume constants because the Riemannian submersion gives $\operatorname{vol}G=\operatorname{vol}(G/T)\operatorname{vol}T$. The map covers regular elements $|W|$ times, giving the [Weyl integration formula](#weyl-integration-formula) with conjugacy averaging for general functions.

<h5 id="weyl-integration-formula-for-u-n">Weyl integration formula for U(n)</h5>

↑ **Parent:** [Weyl integration formula](#weyl-integration-formula)

For the [unitary group](topological-group.md#unitary-group), the diagonal [maximal torus](#maximal-torus) has coordinates $z_i=e^{i\theta_i}$ and [Weyl group](semisimple-lie-algebra.md#weyl-group) $S_n$. The [Weyl integration formula](#weyl-integration-formula) [weights](semisimple-lie-algebra.md#weight-representation-theory) independent uniform angles by $n!^{-1}\prod_{i<j}|z_i-z_j|^2$. The [Vandermonde determinant](galois-theory.md#vandermonde-determinant) $\det(z_i^{n-j})$ has squared [torus](topology.md#torus) integral $n!$, by [Fourier orthogonality](fourier-series.md#fourier-orthogonality). Multiplying an [irreducible](representation-theory.md#irreducible-representation) [character](representation-theory.md#character-of-a-representation) of [highest weight](semisimple-lie-algebra.md#highest-weight-of-a-representation) $\lambda$ by this [determinant](linear-algebra.md#determinant) gives an alternating [Laurent polynomial](polynomial.md#laurent-polynomial). Its leading alternant has coefficient one; [character orthogonality for compact groups](representation-theory.md#character-orthogonality-for-compact-groups) forces every other alternant coefficient to vanish. This yields the quotient $\det(z_i^{\lambda_j+n-j})/\det(z_i^{n-j})$.

### Translation-dilation group of the plane

↑ **Parent:** [Lie group](#lie-group)

This [Lie group](#lie-group) acts on the plane by $v\mapsto x+\rho v$ with $\rho>0$. Its multiplication is $(\rho,x)(\rho',x')=(\rho\rho',x+\rho x')$, and its inverse is $(\rho^{-1},-\rho^{-1}x)$. It is a [semidirect product](group-theory.md#semidirect-product) in which positive dilation acts on the translation subgroup. A dilation generator $D$ and translation generators $T_1,T_2$ have [Lie brackets](lie-algebra.md#lie-bracket) $[D,T_a]=T_a$ and $[T_1,T_2]=0$.

#### Left-invariant coframe of the translation-dilation group

↑ **Parent:** [Translation-dilation group of the plane](#translation-dilation-group-of-the-plane)

The [Maurer-Cartan form](#maurer-cartan-form) of the [translation-dilation group of the plane](#translation-dilation-group-of-the-plane) has these coefficients in its dilation–translation basis, with $a=1,2$. Left multiplication rescales each coordinate differential and $\rho$ equally, proving they are [left-invariant differential forms](#left-invariant-differential-form). Their dual [left-invariant vector fields](#left-invariant-vector-field) are $\rho\partial_\rho$ and $\rho\partial_{x^a}$. The [Maurer-Cartan equation](#maurer-cartan-equation) is $d\lambda^0=0$, $d\lambda^a=-\lambda^0\wedge\lambda^a$. The tensor $\sum_j\lambda^j\otimes\lambda^j$ is a positive definite [left-invariant metric](#left-invariant-metric).

### Lie group homomorphism

↑ **Parent:** [Lie group](#lie-group)

A smooth homomorphism of [Lie groups](#lie-group) has differential $D_eF$ at the identity. Differentiating $F\circ L_g=L_{F(g)}\circ F$ makes the corresponding [left-invariant vector fields](#left-invariant-vector-field) $F$-related. Their commutator action on pulled-back functions shows that the [differential of a Lie group homomorphism preserves Lie brackets](lie-algebra.md#differential-of-a-lie-group-homomorphism-preserves-lie-brackets). The map need not be injective or surjective.

#### Lie group isomorphism

↑ **Parent:** [Lie group homomorphism](#lie-group-homomorphism)

An isomorphism of [Lie groups](#lie-group) is a [group isomorphism](algebra.md#group-isomorphism) that is also a [diffeomorphism](geometry-and-topology.md#diffeomorphism). Both the [homomorphism](algebra.md#homomorphism) and its inverse preserve the smooth structures. Its identity differential is a [Lie algebra isomorphism](lie-algebra.md#lie-algebra-isomorphism), but an isomorphism of [Lie algebras](lie-algebra.md) determines a global [Lie group isomorphism](#lie-group-isomorphism) without extra period data only for connected [simply connected](algebraic-topology.md#simply-connected-space) [groups](group.md).

#### Lie group homomorphism determined by its differential

↑ **Parent:** [Lie group homomorphism](#lie-group-homomorphism)

A [Lie group homomorphism](#lie-group-homomorphism) intertwines [one-parameter subgroups](#one-parameter-subgroup) and therefore obeys the displayed identity. A connected [Lie group](#lie-group) is generated by an identity neighbourhood in an exponential chart, so its [homomorphism](algebra.md#homomorphism) is uniquely determined by the differential at the identity. On a disconnected [group](group.md), only the restriction to its [identity component](geometry-and-topology.md#identity-component) is determined this way; the images of the other components require extra data.

### Right-invariant Riemannian metric

↑ **Parent:** [Lie group](#lie-group)

A [Riemannian metric](differential-geometry.md#riemannian-metric) on a [Lie group](#lie-group) is right-invariant when every right translation is an [isometry](riemannian-geometry.md#isometry). It is determined by a positive-definite [inner product](linear-algebra.md#inner-product) at the identity, extended with a coframe of [right-invariant differential forms](#right-invariant-differential-form). Its translation-generated [Killing vector fields](general-relativity.md#killing-vector-field) are left-invariant, rather than the right-invariant vector fields dual to that coframe.

### Right-invariant differential form

↑ **Parent:** [Lie group](#lie-group)

A [differential form](differential-form.md) $\alpha$ on a [Lie group](#lie-group) is right-invariant if $R_g^*\alpha=\alpha$ for every right translation $R_g(p)=pg$. A right [Maurer-Cartan form](#maurer-cartan-form) is represented in a matrix group by $dg\,g^{-1}$, whereas the left version is $g^{-1}dg$. Its components supply a right-invariant coframe.

### Maximal torus

↑ **Parent:** [Lie group](#lie-group)

A maximal torus is a connected compact abelian [Lie subgroup](#lie-subgroup) maximal among such subgroups. Restricting a finite-dimensional [unitary representation](representation-theory.md#unitary-representation) to it splits into one-dimensional weight characters. For [special unitary group](topological-group.md#special-unitary-group) $\mathrm{SU}(2)$ it is the diagonal circle $\operatorname{diag}(z,z^{-1})$.

#### Adjoint-orbit criterion for maximal-torus conjugacy

↑ **Parent:** [Maximal torus](#maximal-torus)

Give the [Lie algebra](lie-algebra.md) of a [compact Lie group](#compact-lie-group) an [inner product](linear-algebra.md#inner-product) invariant under the [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra). For a [maximal torus](#maximal-torus) $T$ with Lie algebra $\mathfrak t$, its Lie-algebra centralizer is $\mathfrak t$: any additional commuting vector would generate, together with $T$, a larger compact connected abelian subgroup. The torus weight decomposition therefore supplies $H\in\mathfrak t$ whose centralizer is exactly $\mathfrak t$, by avoiding finitely many nonzero-weight hyperplanes. For any $X$, maximize $\langle\operatorname{Ad}_gX,H\rangle$ on the group. Its directional derivative gives $\langle Z,[\operatorname{Ad}_gX,H]\rangle=0$ for every $Z$, so $\operatorname{Ad}_gX\in\mathfrak t$. For a connected compact group, the [bi-invariant Riemannian metric](#bi-invariant-riemannian-metric) and [Hopf-Rinow theorem](riemannian-geometry.md#hopf-rinow-theorem) make the exponential onto; exponentiating this conjugacy puts every element in a conjugate of $T$.

#### Character lattice of a torus

↑ **Parent:** [Maximal torus](#maximal-torus)

For a [compact](topology.md#compact-space) [torus](topology.md#torus) $T\cong U(1)^r$, its [continuous](calculus.md#continuous-function) one-dimensional [characters](representation-theory.md#character-of-a-representation) form a [free abelian group](group-theory.md#free-abelian-group) of rank $r$. They are precisely $z\mapsto z_1^{m_1}\cdots z_r^{m_r}$ with integer exponents. This follows from the classification of [representations of the circle group](representation-theory.md#representation-of-the-circle-group), applied to each factor. These [characters](representation-theory.md#character-of-a-representation) are the integral [group](group.md) [weights](semisimple-lie-algebra.md#weight-representation-theory) occurring upon restricting a [group representation](representation-theory.md#group-representation) to a [maximal torus](#maximal-torus); global integrality must be distinguished from integrality against coroots for a [simply connected](algebraic-topology.md#simply-connected-space) semisimple covering [group](group.md).

### Identity component of a Lie group

↑ **Parent:** [Lie group](#lie-group)

The [connected component](geometry-and-topology.md#connected-component) of the identity in a [Lie group](#lie-group) is an open [normal subgroup](group-theory.md#normal-subgroup). Connected coordinate neighbourhoods prove openness, and conjugation preserves the component of the identity. Every open identity neighbourhood generates it: the generated [subgroup](group.md#subgroup) is open, its other [cosets](group-theory.md#coset) are open, and connectedness forces it to be the whole component.

### Group manifold

↑ **Parent:** [Lie group](#lie-group)

The [group manifold](#group-manifold) is the underlying [smooth manifold](differential-geometry.md#smooth-manifold) of a [Lie group](#lie-group), with smooth multiplication and inversion. Its global topology need not be determined by its [Lie algebra](lie-algebra.md): the [SU(2) group](topological-group.md#su-2-group) and [SO(3) group](linear-algebra.md#so-3-group) have isomorphic [Lie algebras](lie-algebra.md) but different [fundamental groups](algebraic-topology.md#fundamental-group).

### Lie subgroup

↑ **Parent:** [Lie group](#lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lie_subgroup)

A Lie subgroup is a subgroup carrying a [Lie group](#lie-group) structure such that its inclusion is an injective [immersion](differential-geometry.md#immersion) and a [group homomorphism](group-theory.md#group-homomorphism). Its [Lie algebra](lie-algebra.md) includes in that of the ambient [Lie group](#lie-group).

#### Closed-subgroup theorem

↑ **Parent:** [Lie subgroup](#lie-subgroup)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed-subgroup_theorem)

Every closed [subgroup](group.md#subgroup) of a finite-dimensional [Lie group](#lie-group) is an [embedded submanifold](differential-geometry.md#embedded-submanifold) and a [Lie subgroup](#lie-subgroup). Closedness alone forces the compatible smooth structure; smoothness need not be assumed in advance. The proof constructs the [Lie algebra of a closed subgroup](#lie-algebra-of-a-closed-subgroup) from [one-parameter subgroups](#one-parameter-subgroup), then uses [local product coordinates for a closed subgroup](#local-product-coordinates-for-a-closed-subgroup).

##### Local product coordinates for a closed subgroup

↑ **Parent:** [Closed-subgroup theorem](#closed-subgroup-theorem)

Choose a [vector subspace](vector-space.md#vector-subspace) $\mathfrak m$ complementary to the [Lie algebra of a closed subgroup](#lie-algebra-of-a-closed-subgroup) $H$. The differential of $F$ at $(0,0)$ is $(U,V)\mapsto U+V$, so the [inverse function theorem](calculus.md#inverse-function-theorem) makes $F$ a local [diffeomorphism](geometry-and-topology.md#diffeomorphism). Sufficiently small nonzero $U\in\mathfrak m$ cannot satisfy $\exp U\in H$: otherwise [limit directions of a closed subgroup](#limit-directions-of-a-closed-subgroup) give a nonzero element of $\mathfrak m\cap\mathfrak h$. Consequently $H$ is locally exactly the coordinate slice $U=0$, proving that it is an [embedded submanifold](differential-geometry.md#embedded-submanifold).

##### Lie algebra of a closed subgroup

↑ **Parent:** [Closed-subgroup theorem](#closed-subgroup-theorem)

For a closed [subgroup](group.md#subgroup) $H$ of a [Lie group](#lie-group), this set is a real [Lie subalgebra](lie-algebra.md#lie-subalgebra). Scalar closure is immediate; the [Lie product formula in a Lie group](#lie-product-formula-in-a-lie-group) and closedness of $H$ give addition. It is a closed [vector subspace](vector-space.md#vector-subspace), also directly by continuity of the [Exponential map of a Lie group](#exponential-map-of-a-lie-group). Conjugating its [one-parameter subgroups](#one-parameter-subgroup) by elements of $H$ preserves it. Differentiating the [Adjoint representation of a Lie group](#adjoint-representation-of-a-lie-group) along $\exp(sX)$ gives $[X,Y]\in\mathfrak h$ for $X,Y\in\mathfrak h$. After the [closed-subgroup theorem](#closed-subgroup-theorem) establishes smoothness, $\mathfrak h$ is exactly the tangent space $T_eH$.

##### Limit directions of a closed subgroup

↑ **Parent:** [Closed-subgroup theorem](#closed-subgroup-theorem)

Let $H$ be a closed [subgroup](group.md#subgroup) of a [Lie group](#lie-group) $G$, and let nonzero vectors $X_j$ in the ambient [Lie algebra](lie-algebra.md) $\mathfrak g$ tend to zero with $\exp X_j\in H$ and $X_j/\|X_j\|\to X$. For any real $t$, choose [integers](number-theory.md#integer) $m_j$ with $m_j\|X_j\|\to t$. Then $(\exp X_j)^{m_j}=\exp(m_jX_j)\to\exp(tX)$. Closedness gives $\exp(tX)\in H$. [Compactness](topology.md#compact-space) of the unit sphere supplies a limit direction from every sequence approaching the identity through nonidentity subgroup elements.

#### Lie algebra of a normal Lie subgroup

↑ **Parent:** [Lie subgroup](#lie-subgroup)

Conjugation by every element of $G$ preserves a normal [Lie subgroup](#lie-subgroup) $H$. Its differential therefore preserves $\mathfrak h=T_eH$. Differentiate that invariance along $\exp(tX)$ to obtain $\operatorname{ad}(X)\mathfrak h\subseteq\mathfrak h$, proving that $\mathfrak h$ is an [ideal of a Lie algebra](lie-algebra.md#ideal-of-a-lie-algebra). Closed subgroups have a canonical Lie-subgroup structure; an arbitrary abstract subgroup need not.

### Lie group action

↑ **Parent:** [Lie group](#lie-group)

A Lie group action is a smooth [group action](group-theory.md#group-action) of a Lie group on a smooth manifold. Differentiating the action gives an infinitesimal action of its [Lie algebra](lie-algebra.md) by vector fields.

#### Proper Lie group action

↑ **Parent:** [Lie group action](#lie-group-action)

A Lie group action on $M$ is proper if $(g,x)\mapsto(gx,x)$ from $G\times M$ to $M\times M$ is a proper map. A free proper smooth action has a smooth quotient manifold, with the quotient map a submersion and principal bundle. Proper actions with stabilizers can have orbit-type strata and singular quotients. These qualifications are necessary before treating an orbit space as a smooth phase space.

#### Torus action

↑ **Parent:** [Lie group action](#lie-group-action)

A smooth action of the compact abelian [Lie group](#lie-group) $\mathbb R^n/(2\pi\mathbb Z)^n$. Commuting [vector fields](calculus.md#vector-field) with a common periodic normalization give such an action. In [action-angle variables](classical-mechanics.md#action-angle-variables), the torus acts by translation of the angles while leaving the actions fixed.

#### Special linear congruence action on symmetric matrices

↑ **Parent:** [Lie group action](#lie-group-action)

The [special linear group](group-theory.md#special-linear-group) acts on determinant-one real [symmetric matrices](linear-algebra.md#symmetric-matrix) by [matrix congruence](linear-algebra.md#matrix-congruence). Symmetry and determinant are preserved, and signatures are preserved by [Sylvester's law of inertia](linear-algebra.md#sylvester-s-law-of-inertia). The determinant-one set is a [regular level set](topology.md#regular-level-set) of dimension $n(n+1)/2-1$, with tangent directions $C=C^T$ satisfying $\operatorname{tr}(B^{-1}C)=0$. Its infinitesimal left-action fields are $XB+BX^T$; converting them to a [Lie algebra representation](lie-algebra.md#lie-algebra-representation) requires the [infinitesimal left-action sign convention](#infinitesimal-left-action-sign-convention).

#### Coadjoint representation

↑ **Parent:** [Lie group action](#lie-group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coadjoint_representation)

The coadjoint action of a [Lie group](#lie-group) on the [dual space](linear-algebra.md#dual-space) of its [Lie algebra](lie-algebra.md) is $(\operatorname{Ad}_g^*\eta)(X)=\eta(\operatorname{Ad}_{g^{-1}}X)$. The inverse in this formula makes it a left [group action](group-theory.md#group-action).

##### Coadjoint orbit

↑ **Parent:** [Coadjoint representation](#coadjoint-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coadjoint_orbit)

A [coadjoint orbit](#coadjoint-orbit) is the orbit of $\ell\in\mathfrak g^*$ under $\operatorname{Ad}^*_g\ell$, defined by $\langle\operatorname{Ad}^*_g\ell,\xi\rangle=\langle\ell,\operatorname{Ad}_{g^{-1}}\xi\rangle$. For a connected Lie group these orbits are the [symplectic leaves](symplectic-geometry.md#symplectic-leaf) of its Lie-Poisson manifold. Their tangent vectors are infinitesimal coadjoint actions, and their natural two-form is the [Kirillov–Kostant–Souriau symplectic form](#kirillov-kostant-souriau-symplectic-form).

<h6 id="kirillov-kostant-souriau-symplectic-form">Kirillov–Kostant–Souriau symplectic form</h6>

↑ **Parent:** [Coadjoint orbit](#coadjoint-orbit)

With $\langle\operatorname{ad}^*_\xi\ell,\eta\rangle=-\langle\ell,[\xi,\eta]\rangle$, the displayed form on a [coadjoint orbit](#coadjoint-orbit) is well-defined: changing a generator by an element of the stabilizer changes no pairing. It is nondegenerate on orbit tangents, and its closedness follows from the Jacobi identity. This sign agrees with the positive Lie-Poisson bracket when Hamiltonian vector fields act by $X_f(g)=\{g,f\}$. A negative Lie-Poisson convention reverses the orbit form as well.

#### Fundamental vector field

↑ **Parent:** [Lie group action](#lie-group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_vector_field)

For a [Lie group action](#lie-group-action) and $X$ in its [Lie algebra](lie-algebra.md), the fundamental [vector field](calculus.md#vector-field) is $X_M(p)=\left.\frac{d}{dt}\right|_{t=0}\exp(tX)\cdot p$.

##### Infinitesimal left-action sign convention

↑ **Parent:** [Fundamental vector field](#fundamental-vector-field)

For a smooth left [Lie group action](#lie-group-action), define the [fundamental vector field](#fundamental-vector-field) by $X^\#(p)=\left.\frac d{ds}\right|_0\exp(sX)\cdot p$. With the [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields) $[U,V]f=U(Vf)-V(Uf)$, this map is an anti-homomorphism. The map $X\mapsto v_X=-X^\#$ is a [Lie algebra representation](lie-algebra.md#lie-algebra-representation). A right action with the positive exponential has the opposite homomorphism convention, so specifying action side and bracket convention prevents a sign ambiguity.

### Matrix Lie group

↑ **Parent:** [Lie group](#lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_Lie_group)

A matrix Lie group is a subgroup of a [general linear group](group-theory.md#general-linear-group) that is also a [Lie group](#lie-group) for its matrix topology. Near the identity, the [matrix exponential](linear-operator-theory.md#matrix-exponential) and [matrix logarithm](vector-space.md#matrix-logarithm) give inverse coordinate charts whenever they are restricted to sufficiently small neighborhoods in the group and its tangent space.

#### Lie algebra of a quadratic-form stabilizer

↑ **Parent:** [Matrix Lie group](#matrix-lie-group)

For a real [quadratic form](linear-algebra.md#quadratic-form) $Q(v)=v^TAv$ with $A$ a [symmetric matrix](linear-algebra.md#symmetric-matrix), its stabilizer is $G_Q=\{g\in\operatorname{GL}_n(\mathbb R):g^TAg=A\}$. Its [Lie algebra](lie-algebra.md) consists exactly of $X$ satisfying $X^TA+AX=0$. Differentiation proves necessity; the [matrix exponential](linear-operator-theory.md#matrix-exponential) proves sufficiency because $e^{tX^T}Ae^{tX}=A$. The result holds even when the [quadratic form](linear-algebra.md#quadratic-form) is degenerate.

#### Exponential map of a matrix Lie group

↑ **Parent:** [Matrix Lie group](#matrix-lie-group)

For a [Matrix Lie group](#matrix-lie-group) $G$ with Lie algebra $\mathfrak g$, its exponential map is the restriction of the [matrix exponential](linear-operator-theory.md#matrix-exponential), $X\mapsto e^X$. It maps $\mathfrak g$ into $G$ and is a local diffeomorphism at zero, but it need not be surjective globally.

##### Exponential-surjectivity obstruction from distinct negative eigenvalues

↑ **Parent:** [Exponential map of a matrix Lie group](#exponential-map-of-a-matrix-lie-group)

A real matrix with at least one simple negative [eigenvalue](linear-operator-theory.md#eigenvalue) cannot be a [matrix exponential](linear-operator-theory.md#matrix-exponential) of a real matrix: a logarithm would commute with it and preserve each one-dimensional real negative-eigenvalue space, where exponentiation can only produce a positive [eigenvalue](linear-operator-theory.md#eigenvalue). In particular $\operatorname{diag}(-2,-1/2)$ belongs to the connected [special linear group](group-theory.md#special-linear-group) $\mathrm{SL}_2(\mathbb R)$ but has no real logarithm.

#### Logarithmic chart of a matrix Lie group

↑ **Parent:** [Matrix Lie group](#matrix-lie-group)

For a matrix Lie group $G$ with Lie algebra $\mathfrak g=T_I G$, choose neighborhoods on which $\exp:\mathfrak g\to G$ and $\log:G\to\mathfrak g$ are inverse. Left translation gives a chart near $g\in G$ by

$$
h\longmapsto\log(g^{-1}h).
$$

The [Baker--Campbell--Hausdorff formula](linear-operator-theory.md#baker-campbell-hausdorff-formula) expresses multiplication smoothly in these coordinates.

### Simple Lie group

↑ **Parent:** [Lie group](#lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simple_Lie_group)

A connected Lie group is simple when its [Lie algebra](lie-algebra.md) is nonabelian and simple. Some conventions additionally quotient out or exclude a discrete center; the infinitesimal gauge fields depend only on the Lie algebra.

### Homogeneous space

↑ **Parent:** [Lie group](#lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homogeneous_space)

A homogeneous space is a space on which a group acts transitively. After choosing a point, a transitive Lie-group action identifies the space with a quotient $G/H$ by the point stabilizer.

### Left and right translation on a Lie group

↑ **Parent:** [Lie group](#lie-group)

For a [Lie group](#lie-group) $G$, left and right translation are the [diffeomorphisms](geometry-and-topology.md#diffeomorphism) $L_g(h)=gh$ and $R_g(h)=hg$. They commute: $L_gR_h=R_hL_g$.

#### Flat translation connections on a Lie group

↑ **Parent:** [Left and right translation on a Lie group](#left-and-right-translation-on-a-lie-group)

Declare a global left-invariant, respectively right-invariant, frame parallel to obtain two flat [affine connections](fiber-bundle.md#affine-connection) on a [Lie group](#lie-group). For [left-invariant vector fields](#left-invariant-vector-field), their derivatives are as displayed and their [torsion tensors](fiber-bundle.md#torsion-tensor) are $-[X,Y]$ and $+[X,Y]$. The tensors vanish on Abelian groups; two genuinely torsionful connections are not asserted there.

##### Torsion contractions of a left-parallel Lie-group connection

↑ **Parent:** [Flat translation connections on a Lie group](#flat-translation-connections-on-a-lie-group)

Declare a global frame of [left-invariant vector fields](#left-invariant-vector-field) parallel on a [semisimple Lie group](#semisimple-lie-group). This [affine connection](fiber-bundle.md#affine-connection) is flat and preserves a left-invariant [metric tensor](general-relativity.md#metric-tensor) because its frame components are constant. If $[e_a,e_c]=C_a{}^b{}_ce_b$, its [torsion tensor](fiber-bundle.md#torsion-tensor) is $T_a{}^b{}_c=-C_a{}^b{}_c$. For fixed $c$, the matrix with entries $T_a{}^b{}_c$ is $\operatorname{ad}e_c$. Its trace vanishes because a semisimple [Lie algebra](lie-algebra.md) is perfect and adjoints of brackets are commutators. The trace of the product for $c,d$ is the [Killing form](lie-algebra.md#killing-form) $K_{cd}$, proving both contractions. This flat metric connection differs from the curved torsion-free [Levi-Civita connection](general-relativity.md#levi-civita-connection) of the Killing metric.

##### Canonical torsion-free connection on a Lie group

↑ **Parent:** [Flat translation connections on a Lie group](#flat-translation-connections-on-a-lie-group)

The average of the two [flat translation connections on a Lie group](#flat-translation-connections-on-a-lie-group) is a [torsion-free connection](fiber-bundle.md#torsion-free-connection). For [left-invariant vector fields](#left-invariant-vector-field), the [Jacobi identity](lie-algebra.md#jacobi-identity) gives $R(X,Y)Z=-\frac14[[X,Y],Z]$ with $R(X,Y)=[\nabla_X,\nabla_Y]-\nabla_{[X,Y]}$. Contracting gives $\operatorname{Ric}(X,Y)=-\frac14K(X,Y)$ for the [Killing form](lie-algebra.md#killing-form) $K$. It is flat exactly when all double Lie brackets vanish, including the case of a two-step nilpotent group. For a semisimple [Lie algebra](lie-algebra.md), $K$ is nondegenerate and supplies a bi-invariant indefinite metric whose [Levi-Civita connection](general-relativity.md#levi-civita-connection) is $\nabla^0$.

#### Right-invariant vector field

↑ **Parent:** [Left and right translation on a Lie group](#left-and-right-translation-on-a-lie-group)

The right-invariant [vector field](calculus.md#vector-field) associated with a [Lie algebra](lie-algebra.md) element $\xi$ is obtained by right translation of its value at the identity. Its flow is $g\mapsto\exp(t\xi)g$, hence consists of [left translations on a Lie group](#left-and-right-translation-on-a-lie-group). Right invariance follows because left and right multiplication commute.

##### Right-invariant vector fields realize the opposite Lie algebra

↑ **Parent:** [Right-invariant vector field](#right-invariant-vector-field)

For a [Matrix Lie group](#matrix-lie-group), the [right-invariant vector field](#right-invariant-vector-field) is $r_\xi(g)=\xi g$. Differentiating these ambient matrix-valued functions in the definition of the [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields) gives $[r_\xi,r_\eta](g)=(\eta\xi-\xi\eta)g$. Thus $\xi\mapsto r_\xi$ is an antihomomorphism, and $\xi\mapsto-r_\xi$ is a homomorphism. In contrast, $\xi\mapsto l_\xi$ for [left-invariant vector fields](#left-invariant-vector-field) is a homomorphism.

#### Left-invariant vector field

↑ **Parent:** [Left and right translation on a Lie group](#left-and-right-translation-on-a-lie-group)

For $\xi$ in the [Lie algebra](lie-algebra.md) of $G$, the left-invariant vector field is $l_\xi(g)=(dL_g)_e\xi$. Its global [flow](differential-geometry.md#local-flow) is right translation $\Phi^t=R_{\exp(t\xi)}$.

<h5 id="pauli-coordinate-left-invariant-vector-fields-on-su-2">Pauli-coordinate left-invariant vector fields on SU(2)</h5>

↑ **Parent:** [Left-invariant vector field](#left-invariant-vector-field)

On a hemisphere of [SU(2) as the three-sphere](topological-group.md#su-2-as-the-three-sphere), write $A=u_0I+i u_i\sigma_i$, with real coefficients satisfying $u_0^2+|\mathbf u|^2=1$. Right multiplication by $I+i v_j\sigma_j$ gives $du_i=(u_0\delta_{ij}+u_k\epsilon_{jki})v_j$. This right multiplication flow defines left-invariant tangent fields. With the displayed factor $i$, they obey $T_jA=-A\sigma_j$, since $\partial_{u_i}u_0=-u_i/u_0$. Applying the [commutator](lie-algebra.md#commutator) to $A$ and using the [Pauli matrix commutator identity](algebra.md#pauli-matrix-commutator-identity) gives $[T_i,T_j]=-2i\epsilon_{ijk}T_k$. The entries of $A$ contain every coordinate, so this determines the vector-field identity, not just its action in one isolated representation.

##### Parallelization of a Lie group by left translations

↑ **Parent:** [Left-invariant vector field](#left-invariant-vector-field)

A basis $T_a$ of the [Lie algebra](lie-algebra.md) of a [Lie group](#lie-group) gives a global [frame of a vector bundle](fiber-bundle.md#frame-of-a-vector-bundle) of its [tangent bundle](fiber-bundle.md#tangent-bundle) by $X_a(g)=(dL_g)_eT_a$. Left translation is a [diffeomorphism](geometry-and-topology.md#diffeomorphism), so the [left-invariant vector fields](#left-invariant-vector-field) are independent everywhere. Every [Lie group](#lie-group) is therefore a [parallelizable manifold](differential-geometry.md#parallelizable-manifold).

##### Differentiating left-invariant matrix fields

↑ **Parent:** [Left-invariant vector field](#left-invariant-vector-field)

On a [Matrix Lie group](#matrix-lie-group), the [left-invariant vector field](#left-invariant-vector-field) associated to a [tangent vector](differential-geometry.md#tangent-vector) $B$ at the identity is $X_B(Q)=QB$. Its ambient derivative is $DX_B(Q)[H]=HB$. Therefore the [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields) is $[X_{B_1},X_{B_2}](Q)=Q(B_1B_2-B_2B_1)$, and the induced [Lie algebra](lie-algebra.md) bracket is the [commutator](lie-algebra.md#commutator). This fixes the sign for left invariance; right-invariant fields induce the opposite sign when evaluated with the same matrix identification.

##### Completeness of left-invariant vector fields

↑ **Parent:** [Left-invariant vector field](#left-invariant-vector-field)

Every smooth [left-invariant vector field](#left-invariant-vector-field) on a [Lie group](#lie-group) is a [complete vector field](differential-geometry.md#complete-vector-field). Translate a local [integral curve of a vector field](calculus.md#integral-curve-of-a-vector-field) through the identity to every other point. The same positive local existence interval works at every initial point, so no maximal [integral curve of a vector field](calculus.md#integral-curve-of-a-vector-field) can have a finite endpoint. Uniqueness then makes the curve through the identity a [one-parameter subgroup](#one-parameter-subgroup).

#### Left-invariant differential form

↑ **Parent:** [Left and right translation on a Lie group](#left-and-right-translation-on-a-lie-group)

A differential form $\alpha$ on a [Lie group](#lie-group) is left-invariant when $L_g^*\alpha=\alpha$ for every $g$. It is determined by its value at the identity.

##### Invariant volume form on a Lie group

↑ **Parent:** [Left-invariant differential form](#left-invariant-differential-form)

Choose a nonzero element of $\Lambda^nT_e^*G$ for an $n$-dimensional [Lie group](#lie-group) and transport it by inverse left translations. This gives a smooth nowhere-zero [left-invariant differential form](#left-invariant-differential-form) of top degree, hence an [orientation](algebraic-topology.md#orientation-of-a-simplex). The identity $L_{(hg)^{-1}}L_h=L_{g^{-1}}$ proves invariance. The space of invariant top forms is one-dimensional, since evaluation at the identity identifies it with $\Lambda^nT_e^*G$.

##### Bi-invariant differential form

↑ **Parent:** [Left-invariant differential form](#left-invariant-differential-form)

A differential form on a [Lie group](#lie-group) is bi-invariant when it is invariant under both left and right translations.

###### Cartan three-form

↑ **Parent:** [Bi-invariant differential form](#bi-invariant-differential-form)

An adjoint-invariant symmetric [bilinear form](linear-algebra.md#bilinear-form) $B$ on a [Lie algebra](lie-algebra.md) makes the displayed tensor alternating. If $B$ is invariant under the full group [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra), its left-translated three-form is also right-invariant. On left-invariant fields, the [exterior derivative](differential-form.md#exterior-derivative) is $d\eta(W,X,Y,Z)=-2B(W,[X,[Y,Z]]+[Y,[Z,X]]+[Z,[X,Y]])=0$ by the [Jacobi identity](lie-algebra.md#jacobi-identity). The [Killing form](lie-algebra.md#killing-form) supplies such a $B$ on every semisimple [Lie group](#lie-group). An overall sign change in the lowered structure-constant convention negates the form but not its invariance or closedness.

###### Closed left-invariant 1-form

↑ **Parent:** [Bi-invariant differential form](#bi-invariant-differential-form)

On a connected [Lie group](#lie-group), a [left-invariant](#left-invariant-differential-form) [differential 1-form](differential-form.md#one-form) is [closed](differential-form.md#closed-differential-form) exactly when it is [bi-invariant](#bi-invariant-differential-form). Connectedness is essential: on $O(2)$ every left-invariant 1-form is closed because its Lie algebra is abelian, while reflection conjugation negates every nonzero one.

### One-parameter subgroup

↑ **Parent:** [Lie group](#lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/One-parameter_subgroup)

A one-parameter subgroup of a Lie group $G$ is a smooth homomorphism $\gamma:(\mathbb R,+)\to G$. Every such subgroup has the form $\gamma(t)=\exp(tX)$ for a unique $X$ in the Lie algebra of $G$.

#### Classification of nontrivial one-parameter subgroups

↑ **Parent:** [One-parameter subgroup](#one-parameter-subgroup)

For $X\ne0$, the image of $t\mapsto e^{tX}$, with its intrinsic immersed [Lie subgroup](#lie-subgroup) topology, is isomorphic to $(\mathbb R,+)$ or the [circle group](#circle-group). The kernel is respectively zero or $\tau\mathbb Z$ for a least positive period $\tau$. The case $X=0$ is the trivial group. An irrational winding in a two-dimensional torus need not be an embedded or closed subgroup, so its intrinsic topology must be distinguished from the subspace topology.

##### Compact one-parameter subgroups of SL2R

↑ **Parent:** [Classification of nontrivial one-parameter subgroups](#classification-of-nontrivial-one-parameter-subgroups)

For $X=\begin{pmatrix}a&b\\c&-a\end{pmatrix}$, the image of its [matrix exponential](linear-operator-theory.md#matrix-exponential) is compact precisely when $a^2+bc<0$ or $X=0$. If $a^2+bc=-\omega^2<0$, then $e^{tX}=\cos(\omega t)I_2+\sin(\omega t)X/\omega$ and its image is conjugate to the [circle group](#circle-group). A nonzero nilpotent generator or a generator with real nonzero eigenvalues produces an unbounded image.

### Circle group

↑ **Parent:** [Lie group](#lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circle_group)

The circle group is the unit complex numbers under multiplication, equivalently planar rotations or the quotient $\mathbb R/(2\pi\mathbb Z)$.

#### Circle metric

↑ **Parent:** [Circle group](#circle-group)

The quotient metric of circumference one uses the shorter distance around the circle: $\|x\|=\min_{m\in\mathbb Z}|\widetilde x-m|$. It also measures separation across the identified endpoints. This is the metric used by [circular spacing](analytic-number-theory.md#circular-spacing) in the [analytic large sieve inequality](analytic-number-theory.md#exponential-sum-large-sieve).

### Lie-group representation

↑ **Parent:** [Lie group](#lie-group)

A Lie-group representation is a smooth [group representation](representation-theory.md#group-representation) $D:G\to GL(V)$.

#### Derived representation

↑ **Parent:** [Lie-group representation](#lie-group-representation)

The derived representation of a smooth Lie-group representation is $dD(X)=\left.\frac d{dt}\right|_{0}D(\exp(tX))$. It is a [Lie algebra representation](lie-algebra.md#lie-algebra-representation) because $dD([X,Y])=[dD(X),dD(Y)]$.

### Adjoint representation of a Lie group

↑ **Parent:** [Lie group](#lie-group)

The adjoint representation of a Lie group is its action on its Lie algebra by differentiating conjugation. For a matrix Lie group, $\operatorname{Ad}_gX=gXg^{-1}$.

#### Normal subgroups of a compact group with irreducible adjoint action

↑ **Parent:** [Adjoint representation of a Lie group](#adjoint-representation-of-a-lie-group)

Let $G$ be [connected](geometry-and-topology.md#connected-space) and [compact](topology.md#compact-space) with nonzero [irreducible](representation-theory.md#irreducible-representation) real [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra). Its [Lie algebra](lie-algebra.md) has no proper invariant [Lie algebra ideal](lie-algebra.md#ideal-of-a-lie-algebra). If it is [Abelian](group.md#abelian-group), irreducibility forces [dimension](vector-space.md#dimension-vector-space) one, so $G$ is the [circle group](#circle-group). Otherwise its centre has zero-dimensional [Lie algebra](lie-algebra.md) and is finite. A proper closed [normal subgroup](group-theory.md#normal-subgroup) likewise has zero-dimensional [Lie algebra](lie-algebra.md), hence is finite; connectedness of $G$ makes [conjugation](group-theory.md#conjugation) on that finite subgroup trivial, so the subgroup is central. A [Lie group homomorphism](#lie-group-homomorphism) onto a nontrivial [connected](geometry-and-topology.md#connected-space) target with [surjective](algebra.md#surjective-function) differential consequently has finite central [group kernel](group-theory.md#kernel-of-a-group-homomorphism). The qualifications “proper” and “nontrivial” are essential.

#### Inverse conjugation and adjoint antirepresentations

↑ **Parent:** [Adjoint representation of a Lie group](#adjoint-representation-of-a-lie-group)

With [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra) convention $\operatorname{ad}_X(Y)=[X,Y]$, the [matrix exponential](linear-operator-theory.md#matrix-exponential) identity is $e^{-X}Ye^X=e^{-\operatorname{ad}_X}Y$. Inverse conjugation reverses product order, so it is a right action or antirepresentation, whereas $\operatorname{Ad}_g(Y)=gYg^{-1}$ is an ordinary left [group representation](representation-theory.md#group-representation). The first-order terms $Y\mp[X,Y]$ detect a sign mismatch immediately. Negating every adjoint generator without reversing the Lie bracket does not give a new Lie-algebra homomorphism.

<h4 id="adjoint-double-cover-from-su-2-to-so-3">Adjoint double cover from SU(2) to SO(3)</h4>

↑ **Parent:** [Adjoint representation of a Lie group](#adjoint-representation-of-a-lie-group)

Conjugation by $SU(2)$ on its three-dimensional real Lie algebra of traceless skew-Hermitian matrices preserves $-\operatorname{tr}(AB)$ and defines a surjection

$$
SU(2)\longrightarrow SO(3)
$$

with kernel $\{\pm I_2\}$. It is the universal double covering of $SO(3)$.

<h5 id="descent-of-an-su-2-representation-to-so-3">Descent of an SU(2) representation to SO(3)</h5>

↑ **Parent:** [Adjoint double cover from SU(2) to SO(3)](#adjoint-double-cover-from-su-2-to-so-3)

A [SU(2) representation](representation-theory.md#representation-theory-of-su-2) descends to the [SO(3) group](linear-algebra.md#so-3-group) exactly when $-I$ acts trivially. In $\operatorname{Sym}^n(\mathbb C^2)$ it acts by $(-1)^n$, so descent holds precisely for even $n$, or integer spin $j=n/2$. This is the [inflation of a group representation](representation-theory.md#inflation-of-a-group-representation) criterion for the kernel $\{\pm I\}$. Half-integer-spin representations instead remain representations of the covering group.

### Local group law

↑ **Parent:** [Lie group](#lie-group)

A local group law is the coordinate expression $z=F(y,x)$ of multiplication near the identity of a [Lie group](#lie-group). The identity, inverse, and associativity equations for $F$ encode the group structure locally.

### Maurer-Cartan form

↑ **Parent:** [Lie group](#lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maurer–Cartan_form)

For a matrix Lie group, the left-invariant Maurer-Cartan form is $\rho=g^{-1}dg$. It identifies each tangent space with the Lie algebra and obeys $d\rho+\rho\wedge\rho=0$.

#### Maurer-Cartan equation

↑ **Parent:** [Maurer-Cartan form](#maurer-cartan-form)

The Maurer-Cartan equation is $d\rho+\rho\wedge\rho=0$ for the left-invariant form $\rho=g^{-1}dg$.

##### Maurer-Cartan equation in a Lie-algebra basis

↑ **Parent:** [Maurer-Cartan equation](#maurer-cartan-equation)

If $\rho=\sigma^\alpha T_\alpha$ and $[T_\alpha,T_\beta]=c^\gamma{}_{\alpha\beta}T_\gamma$, then

$$
d\sigma^\gamma=-\frac12c^\gamma{}_{\alpha\beta}
\sigma^\alpha\wedge\sigma^\beta.
$$

###### Symmetric-part ambiguity in Maurer-Cartan coefficients

↑ **Parent:** [Maurer-Cartan equation in a Lie-algebra basis](#maurer-cartan-equation-in-a-lie-algebra-basis)

When $d\sigma^\gamma=\sum_{\alpha,\beta}f^\gamma{}_{\alpha\beta}\sigma^\alpha\wedge\sigma^\beta$ sums over ordered pairs, the [Maurer-Cartan equation](#maurer-cartan-equation) determines only $f^\gamma{}_{[\alpha\beta]}=-c^\gamma{}_{\alpha\beta}/2$. Symmetric additions vanish in the [exterior product](linear-algebra.md#exterior-product). The usual coefficients are the unique antisymmetric representatives; summing instead over $\alpha<\beta$ removes the factor one half.

### Orientation-preserving affine group of the real line

↑ **Parent:** [Lie group](#lie-group)

The [real affine group](#orientation-preserving-affine-group-of-the-real-line) used here is the orientation-preserving subgroup of the [affine group](#affine-group) on the real line. It acts by $x\mapsto e^ax+b$ and has multiplication $(a,b)(a',b')=(a+a',b+e^ab')$. The positive dilation distinguishes this connected component from the full group, which also contains negative dilations.

#### Invariant frames of the real affine group

↑ **Parent:** [Orientation-preserving affine group of the real line](#orientation-preserving-affine-group-of-the-real-line)

In exponential scale coordinates, the [real affine group](#orientation-preserving-affine-group-of-the-real-line) has matrices $\begin{pmatrix}e^\alpha&\beta\\0&1\end{pmatrix}$. The left and right [Maurer-Cartan forms](#maurer-cartan-form) are respectively $D\,d\alpha+T\,e^{-\alpha}d\beta$ and $D\,d\alpha+T(d\beta-\beta\,d\alpha)$. Their dual [vector fields](calculus.md#vector-field) obey $[D_L,T_L]=T_L$ and $[D_R,T_R]=-T_R$, displaying the opposite bracket sign for [right-invariant vector fields](#right-invariant-vector-field).

#### Maurer-Cartan coframe of the real affine group

↑ **Parent:** [Orientation-preserving affine group of the real line](#orientation-preserving-affine-group-of-the-real-line)

In the faithful matrices $g=\begin{pmatrix}a&b\\0&1\end{pmatrix}$ with $a>0$, the [Maurer-Cartan form](#maurer-cartan-form) has entries $da/a$ and $db/a$. Thus the [left-invariant differential forms](#left-invariant-differential-form) $\sigma^D=da/a$, $\sigma^T=db/a$ obey $d\sigma^D=0$ and $d\sigma^T=-\sigma^D\wedge\sigma^T$. The [Lie algebra](lie-algebra.md) generators satisfy $[D,T]=T$.

### Left-invariant metric

↑ **Parent:** [Lie group](#lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Left-invariant_metric)

A left-invariant Riemannian metric is preserved by every left translation. Its Killing fields generated by left translations are right-invariant vector fields.

#### Bi-invariant Riemannian metric

↑ **Parent:** [Left-invariant metric](#left-invariant-metric)

A [Riemannian metric](differential-geometry.md#riemannian-metric) on a [Lie group](#lie-group) is bi-invariant if both left and right translations are isometries. Its identity inner product is invariant under the [Adjoint representation of a Lie group](#adjoint-representation-of-a-lie-group); infinitesimally,

$$
\langle[X,Y],Z\rangle+\langle Y,[X,Z]\rangle=0.
$$

This skew-adjointness is the key additional property beyond left invariance.

##### Adjoint dilation obstruction to a bi-invariant Riemannian metric

↑ **Parent:** [Bi-invariant Riemannian metric](#bi-invariant-riemannian-metric)

If a [Lie group](#lie-group) has an [Adjoint representation of a Lie group](#adjoint-representation-of-a-lie-group) element with a real eigenvector of eigenvalue whose modulus differs from one, it has no [bi-invariant Riemannian metric](#bi-invariant-riemannian-metric). Conjugation is a composition of left and right translations, hence would preserve the positive identity inner product. Applying it to that eigenvector gives $\|v\|=|\lambda|\|v\|$, a contradiction. The [orientation-preserving affine group of the real line](#orientation-preserving-affine-group-of-the-real-line) supplies a connected example: conjugation by dilation of factor two multiplies the infinitesimal translation by two.

##### Ricci curvature of a bi-invariant Riemannian metric

↑ **Parent:** [Bi-invariant Riemannian metric](#bi-invariant-riemannian-metric)

For a [bi-invariant Riemannian metric](#bi-invariant-riemannian-metric) on a [Lie group](#lie-group), the induced inner product on its [Lie algebra](lie-algebra.md) makes every adjoint operator skew-adjoint. The [Levi-Civita connection of a bi-invariant metric](#levi-civita-connection-of-a-bi-invariant-metric) gives $R(X,Y)Z=-\tfrac14[[X,Y],Z]$. Thus $K(X,Y)=\tfrac14\|[X,Y]\|^2$ for orthonormal $X,Y$, and

$$
\operatorname{Ric}(X,X)=\frac14\sum_i\|[X,e_i]\|^2.
$$

The nullspace of this quadratic form is exactly the [center of a Lie algebra](lie-algebra.md#center-of-a-lie-algebra). A zero center therefore gives positive [Ricci curvature](second-fundamental-form.md#ricci-curvature), uniformly bounded below by a positive constant times the metric through left invariance and compactness of the unit sphere in the [Lie algebra](lie-algebra.md).

##### Geodesics of a bi-invariant metric are one-parameter subgroups

↑ **Parent:** [Bi-invariant Riemannian metric](#bi-invariant-riemannian-metric)

Integral curves through the identity of [left-invariant vector fields](#left-invariant-vector-field) are [one-parameter subgroups](#one-parameter-subgroup), by flow uniqueness and left translation. They extend for all time because a fixed local existence interval translates to every point. Under a [bi-invariant Riemannian metric](#bi-invariant-riemannian-metric) they are [geodesics](riemannian-geometry.md#geodesic) by the [Levi-Civita connection of a bi-invariant metric](#levi-civita-connection-of-a-bi-invariant-metric). Geodesic uniqueness proves that these are all geodesics through the identity.

##### Levi-Civita connection of a bi-invariant metric

↑ **Parent:** [Bi-invariant Riemannian metric](#bi-invariant-riemannian-metric)

For [left-invariant vector fields](#left-invariant-vector-field), the [Koszul formula](fiber-bundle.md#koszul-formula) and the adjoint invariance of a [bi-invariant Riemannian metric](#bi-invariant-riemannian-metric) give the displayed [Levi-Civita connection](general-relativity.md#levi-civita-connection). In particular $\nabla_XX=0$.

#### Geodesic-vector criterion for a left-invariant metric

↑ **Parent:** [Left-invariant metric](#left-invariant-metric)

For a [left-invariant metric](#left-invariant-metric) on a [Lie group](#lie-group), the one-parameter subgroup $\gamma_\xi(t)=\exp(t\xi)$ is a [geodesic](riemannian-geometry.md#geodesic) exactly when

$$
\langle\xi,[\xi,\eta]\rangle=0
$$

for every $\eta$ in the [Lie algebra](lie-algebra.md). The [Koszul formula](fiber-bundle.md#koszul-formula) gives $\langle\nabla_\xi\xi,\eta\rangle=-\langle\xi,[\xi,\eta]\rangle$.

### Exponential map of a Lie group

↑ **Parent:** [Lie group](#lie-group)

For a matrix Lie group, the exponential map is the matrix exponential $\exp X=\sum_{n\geq0}X^n/n!$ and sends one-parameter additive subgroups of the Lie algebra to one-parameter subgroups of the group.

#### Additivity of the Lie exponential map

↑ **Parent:** [Exponential map of a Lie group](#exponential-map-of-a-lie-group)

The [Exponential map of a Lie group](#exponential-map-of-a-lie-group) is a [group homomorphism](group-theory.md#group-homomorphism) from the additive [Lie algebra](lie-algebra.md) exactly when its [identity component of a Lie group](#identity-component-of-a-lie-group) is abelian. If it is additive, its image is an abelian subgroup containing an identity neighborhood by the [local exponential chart](#local-exponential-chart); connectedness makes that image the entire identity component. Conversely, in an abelian identity component the product $\exp(tX)\exp(tY)$ is a [one-parameter subgroup](#one-parameter-subgroup) with derivative $X+Y$, giving the identity by uniqueness. The disconnected [Lie group](#lie-group) $S_3\times\mathbb R$ shows that the full group need not be abelian.

#### Lie product formula in a Lie group

↑ **Parent:** [Exponential map of a Lie group](#exponential-map-of-a-lie-group)

The [Lie product formula](numerical-analysis.md#lie-product-formula) extends from [matrices](vector-space.md#matrix) to any finite-dimensional [Lie group](#lie-group). In a [local exponential chart](#local-exponential-chart), smooth multiplication and its differential give $\log(\exp(sX)\exp(sY))=s(X+Y)+O(s^2)$. Taking $s=t/m$ and using the [one-parameter subgroup](#one-parameter-subgroup) identity shows that the $m$th power is $\exp(t(X+Y)+O(m^{-1}))$, proving the displayed [limit](calculus.md#limit-of-a-function). This proof needs only the first-order expansion, rather than convergence of the full [Baker--Campbell--Hausdorff formula](linear-operator-theory.md#baker-campbell-hausdorff-formula).

#### Naturality of the Lie group exponential

↑ **Parent:** [Exponential map of a Lie group](#exponential-map-of-a-lie-group)

For a [Lie group homomorphism](#lie-group-homomorphism) $F$, the image of the integral curve through the identity of a [left-invariant vector field](#left-invariant-vector-field) is the integral curve of the field induced by its differential. Uniqueness of [integral curves of a vector field](calculus.md#integral-curve-of-a-vector-field) identifies the curves for all times. Evaluating at time one gives the formula. Completeness of invariant fields follows from left translation and repetition of a local integral curve, independently of a matrix-series formula.

#### Local exponential chart

↑ **Parent:** [Exponential map of a Lie group](#exponential-map-of-a-lie-group)

Since the differential of the [Exponential map of a Lie group](#exponential-map-of-a-lie-group) at zero is the identity, the [inverse function theorem](calculus.md#inverse-function-theorem) makes it a [diffeomorphism](geometry-and-topology.md#diffeomorphism) on a sufficiently small neighborhood of zero. Its local inverse is a logarithm near the group identity. It need not extend to a global logarithm, even for the real [general linear group](group-theory.md#general-linear-group).

### Cayley transform (Lie theory)

↑ **Parent:** [Lie group](#lie-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cayley_transform_(Lie_theory))

The Cayley transform is a rational local parametrization of a matrix Lie group from its Lie algebra wherever $I-X$ is invertible. Unlike the exponential map, its image can meet nonidentity components.

## Lie algebra

↑ **Parent:** [Lie theory](lie-theory.md)

[This section is present in another page, follow this link to view it.](lie-algebra.md)

## Coxeter group

↑ **Parent:** [Lie theory](lie-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coxeter_group)

A Coxeter group is a [group](group.md) with a presentation

$$
W=\langle x_i\ (i\in I): (x_ix_j)^{m_{ij}}=1\rangle,
$$

where $m_{ii}=1$ and $m_{ij}=m_{ji}\in\{2,3,\ldots,\infty\}$ for $i\ne j$. The pair consisting of $W$ and its distinguished generating reflections is a [Coxeter system](#coxeter-system).

### Coxeter system

↑ **Parent:** [Coxeter group](#coxeter-group)

A Coxeter system $(W,I,M)$ records a [Coxeter group](#coxeter-group) $W$, its set $I$ of simple generators, and its [Coxeter matrix](#coxeter-matrix) $M=(m_{ij})$.

#### Coxeter matrix

↑ **Parent:** [Coxeter system](#coxeter-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coxeter_matrix)

The Coxeter matrix of a [Coxeter system](#coxeter-system) is the symmetric matrix whose entry $m_{ij}$ is the order of $x_ix_j$.

##### Coxeter graph

↑ **Parent:** [Coxeter matrix](#coxeter-matrix)

The Coxeter graph has vertex set $I$, joins $i$ and $j$ when $m_{ij}\geq3$, and labels the edge by $m_{ij}$ when $m_{ij}>3$. A [Coxeter system](#coxeter-system) is [irreducible](#irreducible-coxeter-system) exactly when this graph is connected.

###### Admissible crystallographic Coxeter graph

↑ **Parent:** [Coxeter graph](#coxeter-graph)

In the crystallographic convention, a [Coxeter graph](#coxeter-graph) is admissible when it is realized by linearly independent unit [vectors](vector-space.md#vector) $v_i$ in a [Euclidean space](functional-analysis.md#euclidean-norm), with nonpositive mutual [inner products](linear-algebra.md#inner-product) and $4(v_i,v_j)^2=n_{ij}\in\{0,1,2,3\}$ for distinct vertices. The number $n_{ij}$ records a single, double or triple connection; equivalently, the displayed [Gram matrix](linear-algebra.md#gram-matrix) is [positive-definite](linear-algebra.md#positive-definite-bilinear-form). In edge-label notation the nonzero connections have labels $3,4,6$. Forgetting multiplicity, the underlying [graph](graph.md) is a [forest](combinatorics.md#forest): for any cycle of $k\geq3$ distinct vertices, the sum of the corresponding unit [vectors](vector-space.md#vector) would have squared [norm](functional-analysis.md#norm) at most $k-k=0$, contradicting their linear independence. Multiple lines on one connection are labels and are not length-two cycles. This is the convention of [Wehler's Lie algebra notes, section 6.3](https://www.mathematik.uni-muenchen.de/~wehler/LieAlgebrasScript.pdf).

###### Irreducible Coxeter system

↑ **Parent:** [Coxeter graph](#coxeter-graph)

An irreducible Coxeter system is one whose [Coxeter graph](#coxeter-graph) is connected. The connected components of a Coxeter graph give the direct-product decomposition of its Coxeter group.

<h6 id="type-e-p-q-k-coxeter-graph">Type E(p,q,k) Coxeter graph</h6>

↑ **Parent:** [Coxeter graph](#coxeter-graph)

The type $E(p,q,k)$ graph is a simply-laced tree with one trivalent vertex and arms containing $p$, $q$, and $k$ vertices beyond that vertex.

#### Reduced expression in a Coxeter group

↑ **Parent:** [Coxeter system](#coxeter-system)

A [reduced expression in a Coxeter group](#reduced-expression-in-a-coxeter-group) has the least possible [Coxeter length](semisimple-lie-algebra.md#coxeter-length) among expressions in the generators of its [Coxeter system](#coxeter-system).

A reduced expression for $w\in W$ is a product of the fewest possible simple generators representing $w$. The number of factors is its [Coxeter length](semisimple-lie-algebra.md#coxeter-length) $\ell(w)$.

##### Deletion condition for involutory generators

↑ **Parent:** [Reduced expression in a Coxeter group](#reduced-expression-in-a-coxeter-group)

For a group generated by involutions, the deletion condition says that every nonreduced word can be shortened without changing its value by deleting two of its letters.

###### Folding-grid proof of the deletion condition

↑ **Parent:** [Deletion condition for involutory generators](#deletion-condition-for-involutory-generators)

Arrange the lengths of all consecutive subwords of a word in a triangular grid. Under the [folding condition](#folding-condition), the boundary between length ascents and descents must contain a folding square. Its equal opposite vertices identify two letters that can be deleted. Induction proves the [deletion condition for involutory generators](#deletion-condition-for-involutory-generators).

##### Exchange condition for a Coxeter group

↑ **Parent:** [Reduced expression in a Coxeter group](#reduced-expression-in-a-coxeter-group)

If $w=s_1\cdots s_n$ is a reduced expression and $s$ is simple with $\ell(ws)<\ell(w)$, then

$$
ws=s_1\cdots\widehat{s_j}\cdots s_n
$$

for some index $j$. The analogous statement holds for multiplication on the left.

##### Matsumoto theorem

↑ **Parent:** [Reduced expression in a Coxeter group](#reduced-expression-in-a-coxeter-group)

Matsumoto's theorem says that any two reduced expressions for one element of a Coxeter group are connected by a finite sequence of braid moves.

###### Tits word reduction theorem

↑ **Parent:** [Matsumoto theorem](#matsumoto-theorem)

Every word in simple Coxeter generators can be reduced by braid moves and cancellations $ss\mapsto1$. Consequently, a word is reduced exactly when no sequence of braid moves can make a cancellation possible.

#### Geometric representation of a Coxeter group

↑ **Parent:** [Coxeter system](#coxeter-system)

For a finite-rank [Coxeter system](#coxeter-system), let $V$ have basis $(e_i)_{i\in I}$ and symmetric [bilinear form](linear-algebra.md#bilinear-form)

$$
\langle e_i,e_j\rangle=-2\cos(\pi/m_{ij}).
$$

Its geometric representation sends the generator $x_i$ to the reflection

$$
\sigma(x_i)v=v-\langle v,e_i\rangle e_i.
$$

##### Coxeter Gram matrix

↑ **Parent:** [Geometric representation of a Coxeter group](#geometric-representation-of-a-coxeter-group)

The Coxeter Gram matrix is the [Gram matrix](linear-algebra.md#gram-matrix) $G=(-2\cos(\pi/m_{ij}))_{i,j\in I}$ of the distinguished basis in the [Geometric representation of a Coxeter group](#geometric-representation-of-a-coxeter-group).

##### Dual geometric representation of a Coxeter group

↑ **Parent:** [Geometric representation of a Coxeter group](#geometric-representation-of-a-coxeter-group)

The dual geometric representation acts on $V^*$ by

$$
(\sigma^*(w)f)(v)=f(\sigma(w^{-1})v).
$$

The open fundamental chamber consists of the functionals positive on every simple basis vector.

###### Tits cone

↑ **Parent:** [Dual geometric representation of a Coxeter group](#dual-geometric-representation-of-a-coxeter-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tits_cone)

For the closed fundamental chamber $D\subseteq V^*$, the Tits cone is

$$
U=\bigcup_{w\in W}wD.
$$

It equals all of $V^*$ exactly when the finite-rank Coxeter group $W$ is finite.

###### Coxeter complex

↑ **Parent:** [Dual geometric representation of a Coxeter group](#dual-geometric-representation-of-a-coxeter-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coxeter_complex)

The Coxeter complex has faces represented by cosets $wW_J$ of [standard parabolic subgroups](#standard-parabolic-subgroup), ordered by reverse inclusion. Geometrically, its maximal simplices are the chambers of the Coxeter arrangement intersected with a sphere.

#### Reflection of a Coxeter group

↑ **Parent:** [Coxeter system](#coxeter-system)

A reflection of a Coxeter system $(W,S)$ is a conjugate $wsw^{-1}$ of a simple generator $s\in S$.

##### Wall of a Coxeter group

↑ **Parent:** [Reflection of a Coxeter group](#reflection-of-a-coxeter-group)

The wall associated with a reflection $r$ consists of the Cayley-graph edges fixed setwise and reversed by left multiplication by $r$. Its complement has two connected components.

###### Half-space of a Coxeter group

↑ **Parent:** [Wall of a Coxeter group](#wall-of-a-coxeter-group)

The two connected components of the complement of a [wall of a Coxeter group](#wall-of-a-coxeter-group) are its half-spaces. A wall separates two group elements when they lie in opposite half-spaces.

#### Standard parabolic subgroup

↑ **Parent:** [Coxeter system](#coxeter-system)

For $J\subseteq I$, the standard parabolic subgroup is $W_J=\langle s_j:j\in J\rangle$. Its cosets index faces of a fixed type in the [Coxeter complex](#coxeter-complex).

##### Spherical subset of a Coxeter system

↑ **Parent:** [Standard parabolic subgroup](#standard-parabolic-subgroup)

A subset $T\subseteq S$ is spherical when its [standard parabolic subgroup](#standard-parabolic-subgroup) $W_T$ is finite.

##### Davis complex

↑ **Parent:** [Standard parabolic subgroup](#standard-parabolic-subgroup)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Davis_complex)

The Davis complex is the geometric realization of the poset of cosets $wW_T$ for spherical subsets $T\subseteq S$. Equivalently, it is the [basic construction of a Coxeter group](#basic-construction-of-a-coxeter-group) obtained by gluing copies of the Davis chamber along mirrors. It is a contractible proper $W$-CW complex.

###### Basic construction of a Coxeter group

↑ **Parent:** [Davis complex](#davis-complex)

For a mirrored chamber $K$, the basic construction is

$$
U(W,K)=(W\times K)/\sim,
$$

where $(w,x)\sim(w',x)$ when $w^{-1}w'$ belongs to the subgroup generated by the mirrors containing $x$.

#### Folding condition

↑ **Parent:** [Coxeter system](#coxeter-system)

For involutory generators, the folding condition requires that simple multiplication never preserve length and that simultaneous left and right ascents either combine to a two-step ascent or fold: if both $s_iw$ and $ws_j$ have length $\ell(w)+1$, then either $\ell(s_iws_j)=\ell(w)+2$ or $w=s_iws_j$.

##### Braid relation in a Coxeter group

↑ **Parent:** [Folding condition](#folding-condition)

For generators $s_i,s_j$ with $m_{ij}<\infty$, the braid relation equates the two alternating words of length $m_{ij}$ beginning with $s_i$ and $s_j$, respectively. When $m_{ij}=2$, it says that the generators commute.

#### Coxeter element

↑ **Parent:** [Coxeter system](#coxeter-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coxeter_element)

A Coxeter element is a product of all simple generators in some order. For a finite irreducible [Coxeter group](#coxeter-group), all Coxeter elements are conjugate.

##### Coxeter number

↑ **Parent:** [Coxeter element](#coxeter-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coxeter_number)

The Coxeter number is the [order](group-theory.md#order-of-a-group-element) of a [Coxeter element](#coxeter-element) in a finite irreducible [Coxeter group](#coxeter-group).

### Finite Coxeter group

↑ **Parent:** [Coxeter group](#coxeter-group)

A finite Coxeter group is a [Coxeter group](#coxeter-group) with finitely many elements. Its [Coxeter Gram matrix](#coxeter-gram-matrix) is positive definite.

#### Longest element of a Coxeter group

↑ **Parent:** [Finite Coxeter group](#finite-coxeter-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Longest_element_of_a_Coxeter_group)

The longest element $w_0$ is the unique element of maximal [Coxeter length](semisimple-lie-algebra.md#coxeter-length) in a finite [Coxeter group](#coxeter-group). It is an involution and satisfies $\ell(w_0w)=\ell(w_0)-\ell(w)$.

#### E7 Coxeter group

↑ **Parent:** [Finite Coxeter group](#finite-coxeter-group)

The $E_7$ Coxeter graph is the simply-laced seven-vertex tree whose three arms have lengths $1$, $2$, and $3$. Its Coxeter Gram matrix is positive definite and has determinant $2$.

#### Hyperoctahedral group

↑ **Parent:** [Finite Coxeter group](#finite-coxeter-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperoctahedral_group)

The signed symmetric group consists of permutations of $\{\pm1,\ldots,\pm n\}$ commuting with sign change. It is the Coxeter group of type $B_n$.

##### Even signed symmetric group

↑ **Parent:** [Hyperoctahedral group](#hyperoctahedral-group)

The even signed symmetric group is the index-two subgroup of signed permutations with an even number of sign changes. It is the Coxeter group of type $D_n$.

### Affine Coxeter group

↑ **Parent:** [Coxeter group](#coxeter-group)

An [Affine Coxeter group](#affine-coxeter-group) is a [Coxeter group](#coxeter-group) acting by affine reflections with Euclidean fundamental alcoves. An irreducible affine Coxeter group has a positive-semidefinite [Coxeter Gram matrix](#coxeter-gram-matrix) with a one-dimensional [radical](linear-algebra.md#radical-of-a-bilinear-form).

### Hyperbolic Coxeter group

↑ **Parent:** [Coxeter group](#coxeter-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbolic_Coxeter_group)

A hyperbolic Coxeter group has a nondegenerate [Coxeter Gram matrix](#coxeter-gram-matrix) of Lorentzian signature in its standard geometric realization.

### BN-pair

↑ **Parent:** [Coxeter group](#coxeter-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/BN-pair)

A BN-pair in a group $G$ consists of subgroups $B,N$ such that $G=\langle B,N\rangle$, $H=B\cap N$ is normal in $N$, and $W=N/H$ has distinguished involutory generators satisfying the Bruhat multiplication axioms. The quotient $W$ is its [Weyl group](semisimple-lie-algebra.md#weyl-group).

### Hecke algebra

↑ **Parent:** [Coxeter group](#coxeter-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hecke_algebra)

A Hecke algebra is a deformation of the [group algebra](associative-algebra.md#group-algebra) of a [Coxeter group](#coxeter-group), obtained by deforming the quadratic relations for its simple generators while retaining the braid relations.

#### Iwahori-Hecke algebra

↑ **Parent:** [Hecke algebra](#hecke-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Iwahori–Hecke_algebra)

Over the polynomial parameter ring, the generic Hecke algebra has basis $(T_w)_{w\in W}$ and multiplication

$$
T_iT_w=
\begin{cases}
T_{x_iw},&\ell(x_iw)>\ell(w),\\
a_iT_{x_iw}+(a_i-1)T_w,&\ell(x_iw)<\ell(w).
\end{cases}
$$

The parameters must agree for conjugate simple generators; equivalently, $(T_i-a_i)(T_i+1)=0$ together with the braid relations presents the algebra.

##### 0-Hecke algebra

↑ **Parent:** [Iwahori-Hecke algebra](#iwahori-hecke-algebra)

The 0-Hecke algebra is the [specialization](associative-algebra.md#specialization-of-an-algebra) $a_i=0$ of a [Generic Hecke algebra of a Coxeter system](#iwahori-hecke-algebra). Its generators obey $T_i^2=-T_i$.

##### Iwahori-Hecke algebra of a BN-pair

↑ **Parent:** [Iwahori-Hecke algebra](#iwahori-hecke-algebra)

This is a finite-group realization of an [Iwahori-Hecke algebra](#iwahori-hecke-algebra). For a finite group $G$ with a [BN-pair](#bn-pair), the Iwahori-Hecke algebra over $k$ is the endomorphism algebra of the permutation module $k[G/B]$, up to the conventional opposite algebra. Its standard basis is indexed by the [Bruhat double cosets](#bruhat-decomposition-of-a-bn-pair).

###### Hecke parameter of a BN-pair

↑ **Parent:** [Iwahori-Hecke algebra of a BN-pair](#iwahori-hecke-algebra-of-a-bn-pair)

For a representative $\dot x_i\in N$, the Hecke parameter is

$$
q_i=[B:B\cap\dot x_iB\dot x_i^{-1}].
$$

The [Iwahori-Hecke algebra of a BN-pair](#iwahori-hecke-algebra-of-a-bn-pair) is obtained from the generic algebra by $a_i\mapsto q_i\cdot1_k$.

## Levi decomposition

↑ **Parent:** [Lie theory](lie-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Levi_decomposition)

In characteristic zero, a finite-dimensional [Lie algebra](lie-algebra.md) is a semidirect sum of its solvable radical and a semisimple [Lie subalgebra](lie-algebra.md#lie-subalgebra). The group analogue splits appropriate groups as a semidirect product with a [Levi subgroup](#levi-subgroup).

## ↑ Ancestors (5)

1. [Diagonal dominance](algebra.md#diagonal-dominance)
2. [Algebra](algebra.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Lie theory](lie-theory.md)
