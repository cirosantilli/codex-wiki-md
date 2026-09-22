# Group theory

↑ **Parent:** [Algebra](algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_theory)

A [group](group.md) records reversible operations that can be combined consistently. Group theory studies their [subgroups](group.md#subgroup), [group homomorphisms](#group-homomorphism), [group actions](group-action.md), and [quotient groups](#quotient-group). A [symmetry group](group-action.md#symmetry-group) makes the abstraction visible: transformations may change individual points while preserving a specified object or its structure. An [orbit of a group action](group-action.md#orbit-group-theory) records which positions can be exchanged, while a [stabilizer subgroup](group-action.md#stabilizer-subgroup) records which operations leave a selected feature fixed.

**Table of contents**

- [Transfer (group theory)](#transfer-group-theory)
  - [Burnside transfer theorem](#burnside-transfer-theorem)
    - [Cyclic Sylow subgroup at the least prime gives a normal complement](#cyclic-sylow-subgroup-at-the-least-prime-gives-a-normal-complement)
- [Prüfer rank](#prufer-rank)
  - [Prüfer rank bound for extensions](#prufer-rank-bound-for-extensions)
- [Maximal condition on subgroups](#maximal-condition-on-subgroups)
- [Group](group.md)
  - [Partially ordered group](partially-ordered-group.md)
    - [Positive cone of an ordered group](partially-ordered-group.md#positive-cone-of-an-ordered-group)
    - [Convex subgroup of an ordered group](partially-ordered-group.md#convex-subgroup-of-an-ordered-group)
    - [Lattice-ordered group](partially-ordered-group.md#lattice-ordered-group)
      - [Riesz decomposition in a lattice-ordered group](partially-ordered-group.md#riesz-decomposition-in-a-lattice-ordered-group)
      - [Lattice-ordered group homomorphism](partially-ordered-group.md#lattice-ordered-group-homomorphism)
      - [Absolute value in a lattice-ordered group](partially-ordered-group.md#absolute-value-in-a-lattice-ordered-group)
        - [Positive and negative parts in a lattice-ordered group](partially-ordered-group.md#positive-and-negative-parts-in-a-lattice-ordered-group)
      - [Convex lattice subgroup](partially-ordered-group.md#convex-lattice-subgroup)
        - [One-sided bounds for adjoining a positive element](partially-ordered-group.md#one-sided-bounds-for-adjoining-a-positive-element)
        - [Ordered right cosets of a convex lattice subgroup](partially-ordered-group.md#ordered-right-cosets-of-a-convex-lattice-subgroup)
        - [Lattice of convex lattice subgroups](partially-ordered-group.md#lattice-of-convex-lattice-subgroups)
        - [Principal convex lattice subgroup](partially-ordered-group.md#principal-convex-lattice-subgroup)
        - [Prime convex lattice subgroup](partially-ordered-group.md#prime-convex-lattice-subgroup)
        - [Value in a lattice-ordered group](partially-ordered-group.md#value-in-a-lattice-ordered-group)
          - [Squared bound from comparison at values](partially-ordered-group.md#squared-bound-from-comparison-at-values)
          - [Cover of a value in a lattice-ordered group](partially-ordered-group.md#cover-of-a-value-in-a-lattice-ordered-group)
            - [Power cofinality in the cover of a value](partially-ordered-group.md#power-cofinality-in-the-cover-of-a-value)
      - [Normal-valued lattice-ordered group](partially-ordered-group.md#normal-valued-lattice-ordered-group)
        - [Wolfenstein inequality for normal-valued lattice-ordered groups](partially-ordered-group.md#wolfenstein-inequality-for-normal-valued-lattice-ordered-groups)
      - [Linearly ordered group](partially-ordered-group.md#linearly-ordered-group)
        - [Archimedean ordered group](partially-ordered-group.md#archimedean-ordered-group)
          - [Archimedean linearly ordered groups are Abelian](partially-ordered-group.md#archimedean-linearly-ordered-groups-are-abelian)
        - [Lexicographically ordered group](partially-ordered-group.md#lexicographically-ordered-group)
        - [Convex subgroups of a finite-rank ordered Abelian group](partially-ordered-group.md#convex-subgroups-of-a-finite-rank-ordered-abelian-group)
        - [Ohnishi orderability criterion](partially-ordered-group.md#ohnishi-orderability-criterion)
      - [Abelian lattice-ordered group](partially-ordered-group.md#abelian-lattice-ordered-group)
        - [Hahn group](partially-ordered-group.md#hahn-group)
          - [Finite-support Hahn embedding along a countable convex chain](partially-ordered-group.md#finite-support-hahn-embedding-along-a-countable-convex-chain)
        - [Free Abelian lattice-ordered group](partially-ordered-group.md#free-abelian-lattice-ordered-group)
          - [Piecewise integer-linear representation of a free Abelian lattice-ordered group](partially-ordered-group.md#piecewise-integer-linear-representation-of-a-free-abelian-lattice-ordered-group)
            - [Integer-linear hinge functions have infinite independent rank](partially-ordered-group.md#integer-linear-hinge-functions-have-infinite-independent-rank)
      - [Lattice-ordered permutation group](partially-ordered-group.md#lattice-ordered-permutation-group)
        - [Order-primitive lattice permutation group](partially-ordered-group.md#order-primitive-lattice-permutation-group)
          - [McCleary trichotomy theorem](partially-ordered-group.md#mccleary-trichotomy-theorem)
        - [Holland representation theorem](partially-ordered-group.md#holland-representation-theorem)
        - [Order n-transitivity](partially-ordered-group.md#order-n-transitivity)
          - [Finite interpolation by lattice operations](partially-ordered-group.md#finite-interpolation-by-lattice-operations)
        - [Positive bump of an order automorphism](partially-ordered-group.md#positive-bump-of-an-order-automorphism)
          - [Conjugacy of positive real-line bumps](partially-ordered-group.md#conjugacy-of-positive-real-line-bumps)
            - [Conjugating positive bumps while preserving a fundamental interval](partially-ordered-group.md#conjugating-positive-bumps-while-preserving-a-fundamental-interval)
  - [Exact factorization of a group](group.md#exact-factorization-of-a-group)
  - [Shifted addition on odd integers](group.md#shifted-addition-on-odd-integers)
  - [Triangle group](group.md#triangle-group)
  - [Poly-(cyclic or finite) group](group.md#poly-cyclic-or-finite-group)
  - [Group element](group.md#group-element)
  - [Braid group](group.md#braid-group)
    - [Artin automorphism of a braid](group.md#artin-automorphism-of-a-braid)
    - [Braid group relations](group.md#braid-group-relations)
  - [Infinite group](group.md#infinite-group)
    - [Tarski monster group](group.md#tarski-monster-group)
      - [Tarski monster groups are two-generated and simple](group.md#tarski-monster-groups-are-two-generated-and-simple)
  - [Trivial group](group.md#trivial-group)
  - [Group of exponent two is abelian](group.md#group-of-exponent-two-is-abelian)
  - [Non-abelian group](group.md#non-abelian-group)
  - [Torsion-free group](group.md#torsion-free-group)
    - [Countable torsion-free embedding with two conjugacy classes](group.md#countable-torsion-free-embedding-with-two-conjugacy-classes)
  - [Divisible group](group.md#divisible-group)
    - [Divisibility by a prime](group.md#divisibility-by-a-prime)
    - [Torsion-free divisible Abelian group](group.md#torsion-free-divisible-abelian-group)
  - [Group axioms](group.md#group-axioms)
    - [Group axioms from two-sided local inverse identities](group.md#group-axioms-from-two-sided-local-inverse-identities)
  - [Finite group](group.md#finite-group)
    - [p-prime core of a finite group](group.md#p-prime-core-of-a-finite-group)
    - [p-core of a finite group](group.md#p-core-of-a-finite-group)
      - [p-constrained group](group.md#p-constrained-group)
    - [Pi-group](group.md#pi-group)
      - [Pi-element](group.md#pi-element)
    - [Elementary group](group.md#elementary-group)
      - [Prime-set decomposition of elementary groups](group.md#prime-set-decomposition-of-elementary-groups)
      - [p-elementary group](group.md#p-elementary-group)
    - [Ambivalent group](group.md#ambivalent-group)
    - [Monomial group](group.md#monomial-group)
      - [Abelian intersection of irreducible inducing subgroups](group.md#abelian-intersection-of-irreducible-inducing-subgroups)
      - [Dade's embedding theorem for monomial groups](group.md#dade-s-embedding-theorem-for-monomial-groups)
      - [Taketa's theorem](group.md#taketa-s-theorem)
    - [Frobenius group](group.md#frobenius-group)
      - [Frobenius kernel](group.md#frobenius-kernel)
        - [Frobenius kernel criterion by irreducible induction](group.md#frobenius-kernel-criterion-by-irreducible-induction)
        - [Commutator bijection from a fixed-point-free automorphism](group.md#commutator-bijection-from-a-fixed-point-free-automorphism)
        - [Frobenius kernel theorem](group.md#frobenius-kernel-theorem)
      - [Frobenius complement](group.md#frobenius-complement)
    - [Burnside's theorem](group.md#burnside-s-theorem)
      - [Prime-power conjugacy-class obstruction to simplicity](group.md#prime-power-conjugacy-class-obstruction-to-simplicity)
        - [Abelian subgroup cannot have prime-power index in a nonabelian simple group](group.md#abelian-subgroup-cannot-have-prime-power-index-in-a-nonabelian-simple-group)
    - [Order of a finite group](group.md#order-of-a-finite-group)
  - [Nontrivial group](group.md#nontrivial-group)
  - [Group operation](group.md#group-operation)
    - [Group commutator](group.md#group-commutator)
      - [Hall-Witt identity](group.md#hall-witt-identity)
      - [Hall-Petrescu formula](group.md#hall-petrescu-formula)
  - [Translation in a group](group.md#translation-in-a-group)
  - [Cyclic group](group.md#cyclic-group)
    - [Cyclic multiplicative group](group.md#cyclic-multiplicative-group)
    - [A group of prime order is cyclic](group.md#a-group-of-prime-order-is-cyclic)
    - [Groups with no proper nontrivial subgroups](group.md#groups-with-no-proper-nontrivial-subgroups)
    - [Subgroups and quotients of a cyclic group](group.md#subgroups-and-quotients-of-a-cyclic-group)
    - [Free translation action on nontrivial subsets of a prime cyclic group](group.md#free-translation-action-on-nontrivial-subsets-of-a-prime-cyclic-group)
    - [Cyclic subgroup](group.md#cyclic-subgroup)
      - [Counting cyclic subgroups by their generators](group.md#counting-cyclic-subgroups-by-their-generators)
    - [Finite cyclic group](group.md#finite-cyclic-group)
      - [Cyclic group of order four](group.md#cyclic-group-of-order-four)
        - [Faithfulness criterion for a block representation of the cyclic group of order four](group.md#faithfulness-criterion-for-a-block-representation-of-the-cyclic-group-of-order-four)
      - [Order of an element of a finite cyclic group](group.md#order-of-an-element-of-a-finite-cyclic-group)
      - [Homomorphism from a finite cyclic group](group.md#homomorphism-from-a-finite-cyclic-group)
    - [Infinite cyclic group](group.md#infinite-cyclic-group)
      - [Subgroup of an infinite cyclic group](group.md#subgroup-of-an-infinite-cyclic-group)
      - [Additive group of integers](group.md#additive-group-of-integers)
      - [Integer shear group](group.md#integer-shear-group)
    - [Finite subgroup of the multiplicative complex numbers](group.md#finite-subgroup-of-the-multiplicative-complex-numbers)
    - [Generator of a group](group.md#generator-of-a-group)
      - [Generators of a finite cyclic group](group.md#generators-of-a-finite-cyclic-group)
  - [Generating set of a group](group.md#generating-set-of-a-group)
    - [Minimal generating set of a group](group.md#minimal-generating-set-of-a-group)
    - [Complement of a proper subgroup generates the group](group.md#complement-of-a-proper-subgroup-generates-the-group)
    - [Finitely generated group](group.md#finitely-generated-group)
      - [Benign subgroup](group.md#benign-subgroup)
        - [Normal benign subgroup quotient embedding](group.md#normal-benign-subgroup-quotient-embedding)
        - [Intersection and join of benign subgroups](group.md#intersection-and-join-of-benign-subgroups)
      - [Unshifted rank gradients](group.md#unshifted-rank-gradients)
      - [Finite-index subgroup count for a finitely generated group](group.md#finite-index-subgroup-count-for-a-finitely-generated-group)
      - [Rank of a group](group.md#rank-of-a-group)
  - [Abelian group](group.md#abelian-group)
    - [Complex multiplicative group](group.md#complex-multiplicative-group)
    - [Abelian group of prime-square order](group.md#abelian-group-of-prime-square-order)
    - [Serre class](group.md#serre-class)
      - [Serre class of finitely generated abelian groups](group.md#serre-class-of-finitely-generated-abelian-groups)
    - [Torsion-free abelian group](group.md#torsion-free-abelian-group)
      - [Rational divisible hull](group.md#rational-divisible-hull)
    - [Abelian subgroup](group.md#abelian-subgroup)
    - [Finitely generated abelian group](group.md#finitely-generated-abelian-group)
      - [Finite generation detected by a prime quotient](group.md#finite-generation-detected-by-a-prime-quotient)
      - [Rank of an abelian group](group.md#rank-of-an-abelian-group)
      - [Fundamental theorem of finitely generated abelian groups](group.md#fundamental-theorem-of-finitely-generated-abelian-groups)
    - [Prüfer group](group.md#prufer-group)
    - [Additive group](group.md#additive-group)
      - [Finitely generated subgroup of the rational additive group](group.md#finitely-generated-subgroup-of-the-rational-additive-group)
    - [Infinitely divisible element of an abelian group](group.md#infinitely-divisible-element-of-an-abelian-group)
    - [Finite abelian group](group.md#finite-abelian-group)
      - [Cyclic group of order four and Klein four-group](group.md#cyclic-group-of-order-four-and-klein-four-group)
      - [Elementary abelian group](group.md#elementary-abelian-group)
        - [Order of a finite group of exponent two](group.md#order-of-a-finite-group-of-exponent-two)
    - [Pontryagin duality](group.md#pontryagin-duality)
      - [Pontryagin dual group](group.md#pontryagin-dual-group)
        - [Equicontinuity of compact families of characters](group.md#equicontinuity-of-compact-families-of-characters)
        - [Dual Haar measure](group.md#dual-haar-measure)
      - [Character group](group.md#character-group)
        - [Character group of a finite abelian group](group.md#character-group-of-a-finite-abelian-group)
          - [Multiplicative character of a finite field](group.md#multiplicative-character-of-a-finite-field)
            - [Jacobi sum of finite-field characters](group.md#jacobi-sum-of-finite-field-characters)
            - [Gauss sum of a finite-field character](group.md#gauss-sum-of-a-finite-field-character)
          - [Extension of a unitary character from a finite abelian subgroup](group.md#extension-of-a-unitary-character-from-a-finite-abelian-subgroup)
          - [Extension of a character across a cyclic quotient](group.md#extension-of-a-character-across-a-cyclic-quotient)
          - [Character of a finite abelian group](group.md#character-of-a-finite-abelian-group)
          - [Character-sum cancellation lemma](group.md#character-sum-cancellation-lemma)
          - [Annihilator of a subgroup of a finite abelian group](group.md#annihilator-of-a-subgroup-of-a-finite-abelian-group)
  - [Finite additive group](group.md#finite-additive-group)
  - [Subgroup](group.md#subgroup)
    - [Subgroup test](group.md#subgroup-test)
    - [Trivial subgroup](group.md#trivial-subgroup)
    - [Finitely generated subgroup](group.md#finitely-generated-subgroup)
    - [Membership problem for a subgroup](group.md#membership-problem-for-a-subgroup)
    - [Maximal subgroup](group.md#maximal-subgroup)
      - [Maximal symmetric-group subgroups containing a three-cycle](group.md#maximal-symmetric-group-subgroups-containing-a-three-cycle)
      - [Maximal subgroups of a finite soluble group](group.md#maximal-subgroups-of-a-finite-soluble-group)
      - [Maximal subgroup normalizer criterion](group.md#maximal-subgroup-normalizer-criterion)
    - [Hall subgroup](group.md#hall-subgroup)
      - [Schur-Zassenhaus theorem](group.md#schur-zassenhaus-theorem)
      - [Hall conjugacy and embedding in finite soluble groups](group.md#hall-conjugacy-and-embedding-in-finite-soluble-groups)
      - [Hall subgroup existence in soluble groups](group.md#hall-subgroup-existence-in-soluble-groups)
    - [Union of two subgroups](group.md#union-of-two-subgroups)
    - [Index of a subgroup](group.md#index-of-a-subgroup)
    - [Index-two subgroup is normal](group.md#index-two-subgroup-is-normal)
    - [Finite-index subgroup](group.md#finite-index-subgroup)
- [First isomorphism theorem](#first-isomorphism-theorem)
- [Direct product of groups](#direct-product-of-groups)
  - [Direct product of cyclic groups of orders four and two](#direct-product-of-cyclic-groups-of-orders-four-and-two)
    - [Subgroups of C4 times C2](#subgroups-of-c4-times-c2)
  - [Cyclicity of a product of two finite cyclic groups](#cyclicity-of-a-product-of-two-finite-cyclic-groups)
  - [Order of a direct-product element](#order-of-a-direct-product-element)
  - [Restricted direct sum of groups](#restricted-direct-sum-of-groups)
  - [Internal direct product theorem](#internal-direct-product-theorem)
- [Metacyclic group](#metacyclic-group)
- [Commutator subgroup](#commutator-subgroup)
  - [Commutator subgroup of the symmetric group on three letters](#commutator-subgroup-of-the-symmetric-group-on-three-letters)
  - [Perfect group](#perfect-group)
    - [Perfectness of the special linear group](#perfectness-of-the-special-linear-group)
  - [Abelianization](#abelianization)
    - [Universal property of abelianization](#universal-property-of-abelianization)
    - [Uniqueness of finite-index subgroups forces infinite cyclic abelianization](#uniqueness-of-finite-index-subgroups-forces-infinite-cyclic-abelianization)
      - [Residually finite group with one subgroup of each finite index is infinite cyclic](#residually-finite-group-with-one-subgroup-of-each-finite-index-is-infinite-cyclic)
    - [Abelianization of the square symmetry group](#abelianization-of-the-square-symmetry-group)
    - [Abelianization of an odd dihedral group](#abelianization-of-an-odd-dihedral-group)
- [Center of a group](#center-of-a-group)
  - [Central element of a group](#central-element-of-a-group)
  - [Cyclic quotient by the center](#cyclic-quotient-by-the-center)
- [Conjugate subgroup](#conjugate-subgroup)
- [Group action](group-action.md)
  - [Column group action](group-action.md#column-group-action)
  - [Row group action](group-action.md#row-group-action)
  - [n-transitive group action](group-action.md#n-transitive-group-action)
  - [Symmetry enlargement under group translates](group-action.md#symmetry-enlargement-under-group-translates)
  - [Subgroup factorization from coset transitivity](group-action.md#subgroup-factorization-from-coset-transitivity)
  - [Circle action](group-action.md#circle-action)
  - [Symmetry group](group-action.md#symmetry-group)
    - [Symmetry transformation](group-action.md#symmetry-transformation)
    - [Symmetry depends on preserved structure](group-action.md#symmetry-depends-on-preserved-structure)
    - [Colour-preserving symmetry group](group-action.md#colour-preserving-symmetry-group)
  - [Finite support in a permutation action](group-action.md#finite-support-in-a-permutation-action)
  - [Free action of a group](group-action.md#free-action-of-a-group)
  - [Free group action](group-action.md#free-group-action)
    - [Finite groups cannot act freely on Euclidean space](group-action.md#finite-groups-cannot-act-freely-on-euclidean-space)
    - [Free actions on even-dimensional spheres have order at most two](group-action.md#free-actions-on-even-dimensional-spheres-have-order-at-most-two)
    - [Free sphere actions exclude elementary abelian subgroups of rank two](group-action.md#free-sphere-actions-exclude-elementary-abelian-subgroups-of-rank-two)
  - [Fundamental domain](group-action.md#fundamental-domain)
  - [Multiply transitive group action](group-action.md#multiply-transitive-group-action)
    - [Three-transitive group action](group-action.md#three-transitive-group-action)
  - [Diagonal action on a centerless group](group-action.md#diagonal-action-on-a-centerless-group)
  - [Ring of invariants](group-action.md#ring-of-invariants)
    - [Normality of a ring of invariants](group-action.md#normality-of-a-ring-of-invariants)
  - [Primitive group action](group-action.md#primitive-group-action)
    - [Primitive group with a transposition](group-action.md#primitive-group-with-a-transposition)
    - [Even primitive groups of safe-prime degree](group-action.md#even-primitive-groups-of-safe-prime-degree)
    - [O'Nan–Scott theorem](group-action.md#o-nan-scott-theorem)
      - [Diagonal primitive permutation group](group-action.md#diagonal-primitive-permutation-group)
      - [Affine primitive permutation group](group-action.md#affine-primitive-permutation-group)
        - [General affine group](group-action.md#general-affine-group)
    - [Primitive three-cycle criterion](group-action.md#primitive-three-cycle-criterion)
  - [Variable-permutation action on polynomials](group-action.md#variable-permutation-action-on-polynomials)
  - [Fixed point of a group action](group-action.md#fixed-point-of-a-group-action)
  - [Left regular action](group-action.md#left-regular-action)
  - [Block system](group-action.md#block-system)
    - [Uniform subdegrees force an imprimitive action to be Frobenius](group-action.md#uniform-subdegrees-force-an-imprimitive-action-to-be-frobenius)
  - [Transitive group action](group-action.md#transitive-group-action)
    - [Simply transitive group action](group-action.md#simply-transitive-group-action)
    - [Regular group action](group-action.md#regular-group-action)
    - [Derangement in a transitive group action](group-action.md#derangement-in-a-transitive-group-action)
      - [Derangement counting formula](group-action.md#derangement-counting-formula)
    - [Rank of a transitive permutation group](group-action.md#rank-of-a-transitive-permutation-group)
    - [Regular permutation subgroup](group-action.md#regular-permutation-subgroup)
      - [Centralizer of a regular permutation subgroup](group-action.md#centralizer-of-a-regular-permutation-subgroup)
    - [Sharp t-transitivity](group-action.md#sharp-t-transitivity)
      - [Sharp three-transitivity](group-action.md#sharp-three-transitivity)
      - [Sharp two-transitivity](group-action.md#sharp-two-transitivity)
      - [Regular kernel of a finite sharply two-transitive group](group-action.md#regular-kernel-of-a-finite-sharply-two-transitive-group)
    - [One-point extension of a permutation group](group-action.md#one-point-extension-of-a-permutation-group)
      - [Double-coset criterion for a one-point extension](group-action.md#double-coset-criterion-for-a-one-point-extension)
    - [Prime-degree transposition criterion](group-action.md#prime-degree-transposition-criterion)
  - [Two-transitive group action](group-action.md#two-transitive-group-action)
    - [Elementary abelian regular kernels in doubly transitive groups](group-action.md#elementary-abelian-regular-kernels-in-doubly-transitive-groups)
    - [Degree-ten partition action of S6](group-action.md#degree-ten-partition-action-of-s6)
    - [Minimal normal subgroup dichotomy for two-transitive groups](group-action.md#minimal-normal-subgroup-dichotomy-for-two-transitive-groups)
    - [Affine two-transitive group](group-action.md#affine-two-transitive-group)
  - [Orbit map](group-action.md#orbit-map)
  - [Equivariant map](group-action.md#equivariant-map)
    - [Translation equivariance](group-action.md#translation-equivariance)
  - [Conjugation action](group-action.md#conjugation-action)
    - [Conjugates of a proper subgroup do not cover a finite group](group-action.md#conjugates-of-a-proper-subgroup-do-not-cover-a-finite-group)
    - [Conjugation](group-action.md#conjugation)
      - [Conjugate subset](group-action.md#conjugate-subset)
      - [Conjugate group elements](group-action.md#conjugate-group-elements)
        - [Conjugate permutation](group-action.md#conjugate-permutation)
    - [Conjugacy class](group-action.md#conjugacy-class)
      - [Conjugacy classes of the symmetric group on three letters](group-action.md#conjugacy-classes-of-the-symmetric-group-on-three-letters)
      - [Infinite conjugacy class group](group-action.md#infinite-conjugacy-class-group)
      - [Torsion-freeness from one nonidentity conjugacy class](group-action.md#torsion-freeness-from-one-nonidentity-conjugacy-class)
      - [Shortest conjugacy representative](group-action.md#shortest-conjugacy-representative)
        - [Cyclic reduction of a shortest conjugacy representative](group-action.md#cyclic-reduction-of-a-shortest-conjugacy-representative)
      - [Conjugacy class splitting in a prime-index normal subgroup](group-action.md#conjugacy-class-splitting-in-a-prime-index-normal-subgroup)
        - [Alternating conjugacy class splitting criterion](group-action.md#alternating-conjugacy-class-splitting-criterion)
          - [Inversion of an odd cycle in an alternating group](group-action.md#inversion-of-an-odd-cycle-in-an-alternating-group)
      - [Class equation](group-action.md#class-equation)
        - [Prime-to-p conjugacy class lemma](group-action.md#prime-to-p-conjugacy-class-lemma)
    - [Centralizer and normalizer](group-action.md#centralizer-and-normalizer)
      - [Centralizer](group-action.md#centralizer)
        - [Centralizer of a subset](group-action.md#centralizer-of-a-subset)
          - [Centralizer of a Hermitian matrix in SU(n)](group-action.md#centralizer-of-a-hermitian-matrix-in-su-n)
        - [Centraliser of a fixed-point-free involution](group-action.md#centraliser-of-a-fixed-point-free-involution)
        - [Centraliser of a transposition](group-action.md#centraliser-of-a-transposition)
      - [Normalizer](group-action.md#normalizer)
        - [Normalizer of a diagonal subgroup of GL2](group-action.md#normalizer-of-a-diagonal-subgroup-of-gl2)
  - [Orbit-stabilizer theorem](group-action.md#orbit-stabilizer-theorem)
    - [Orbit dimension formula](group-action.md#orbit-dimension-formula)
  - [Symmetry group of a cube](group-action.md#symmetry-group-of-a-cube)
    - [Body-diagonal stabilizer in the cube symmetry group](group-action.md#body-diagonal-stabilizer-in-the-cube-symmetry-group)
    - [Axial isotropy types of the full cube symmetry group](group-action.md#axial-isotropy-types-of-the-full-cube-symmetry-group)
    - [Axis stabilizer in the full octahedral symmetry group](group-action.md#axis-stabilizer-in-the-full-octahedral-symmetry-group)
    - [Cube symmetry action on edges](group-action.md#cube-symmetry-action-on-edges)
    - [Direct-product decomposition of the cube symmetry group](group-action.md#direct-product-decomposition-of-the-cube-symmetry-group)
    - [Rotational symmetry group of a cube](group-action.md#rotational-symmetry-group-of-a-cube)
      - [Tetrahedron stabilizer in the cube rotation group](group-action.md#tetrahedron-stabilizer-in-the-cube-rotation-group)
      - [Kernel of the cube face-axis action](group-action.md#kernel-of-the-cube-face-axis-action)
      - [Face-pair orbits of cube rotations](group-action.md#face-pair-orbits-of-cube-rotations)
  - [Faithful group action](group-action.md#faithful-group-action)
    - [Nonfaithful coset action of the symmetric group on three letters](group-action.md#nonfaithful-coset-action-of-the-symmetric-group-on-three-letters)
    - [Faithful quotient of a group action](group-action.md#faithful-quotient-of-a-group-action)
    - [Normal subgroup orbits in a faithful prime-degree action](group-action.md#normal-subgroup-orbits-in-a-faithful-prime-degree-action)
  - [Orbit (group theory)](group-action.md#orbit-group-theory)
    - [Equality-pattern orbits of ordered pairs](group-action.md#equality-pattern-orbits-of-ordered-pairs)
    - [Real rotation orbits on a complex unit quadric](group-action.md#real-rotation-orbits-on-a-complex-unit-quadric)
    - [Equality-pattern orbits of projective triples](group-action.md#equality-pattern-orbits-of-projective-triples)
  - [Stabilizer subgroup](group-action.md#stabilizer-subgroup)
    - [Pointwise stabilizer](group-action.md#pointwise-stabilizer)
    - [Axial subgroup](group-action.md#axial-subgroup)
      - [Complex axial isotropy subgroup](group-action.md#complex-axial-isotropy-subgroup)
  - [Symmetric group action on subsets](group-action.md#symmetric-group-action-on-subsets)
  - [Coset action](group-action.md#coset-action)
    - [Faithful coset action of the symmetric group on three letters](group-action.md#faithful-coset-action-of-the-symmetric-group-on-three-letters)
- [Coset](#coset)
  - [Left coset](#left-coset)
  - [Right coset](#right-coset)
  - [Right coset transversal](#right-coset-transversal)
  - [Double coset](#double-coset)
    - [Double-coset counts need not divide group order](#double-coset-counts-need-not-divide-group-order)
    - [Double-coset sizes not dividing group order](#double-coset-sizes-not-dividing-group-order)
    - [Double-coset Hecke algebra](#double-coset-hecke-algebra)
    - [Sylow subgroup of a subgroup from double cosets](#sylow-subgroup-of-a-subgroup-from-double-cosets)
- [Lagrange's theorem](#lagrange-s-theorem)
  - [Failure of the converse to Lagrange's theorem](#failure-of-the-converse-to-lagrange-s-theorem)
- [Group embedding](#group-embedding)
  - [Two-generator HNN embedding](#two-generator-hnn-embedding)
  - [Alternating-group embedding of a finite group](#alternating-group-embedding-of-a-finite-group)
  - [Cayley's theorem](#cayley-s-theorem)
    - [Symmetric-group embedding at one less than the group order](#symmetric-group-embedding-at-one-less-than-the-group-order)
- [Generalized dihedral group](#generalized-dihedral-group)
  - [Two-involution characterization of a dihedral group](#two-involution-characterization-of-a-dihedral-group)
    - [Nontrivial-quotient closure of two-involution groups](#nontrivial-quotient-closure-of-two-involution-groups)
- [Order of a group element](#order-of-a-group-element)
  - [An element and its inverse have the same order](#an-element-and-its-inverse-have-the-same-order)
  - [Conjugation preserves element order](#conjugation-preserves-element-order)
  - [Product of commuting elements of coprime order](#product-of-commuting-elements-of-coprime-order)
  - [Infinite order](#infinite-order)
  - [Involution](#involution)
    - [Eigenspace decomposition of a linear involution](#eigenspace-decomposition-of-a-linear-involution)
      - [Involution exponential formula](#involution-exponential-formula)
- [Quotient group](#quotient-group)
  - [Quotient map of groups](#quotient-map-of-groups)
  - [Coset multiplication is well-defined exactly for normal subgroups](#coset-multiplication-is-well-defined-exactly-for-normal-subgroups)
  - [Universal property of a quotient group](#universal-property-of-a-quotient-group)
  - [Subgroup correspondence for a surjective group homomorphism](#subgroup-correspondence-for-a-surjective-group-homomorphism)
  - [Finite quotient of a group](#finite-quotient-of-a-group)
  - [Abelian quotient](#abelian-quotient)
- [General linear group](#general-linear-group)
  - [Orientation-preserving general linear group](#orientation-preserving-general-linear-group)
  - [Monomial matrix](#monomial-matrix)
  - [Integral general linear group](#integral-general-linear-group)
  - [Matrix group](#matrix-group)
    - [Classical group](#classical-group)
    - [Orthogonal group over a finite field](#orthogonal-group-over-a-finite-field)
- [Special linear group](#special-linear-group)
  - [Real special linear group of degree two](#real-special-linear-group-of-degree-two)
    - [Elementary unipotent generators of SL2R](#elementary-unipotent-generators-of-sl2r)
  - [Projective special linear group](#projective-special-linear-group)
    - [Scalar kernel of the projective linear action](#scalar-kernel-of-the-projective-linear-action)
  - [Complex special linear group in dimension two](#complex-special-linear-group-in-dimension-two)
  - [Triangular-rotation factorization of real determinant-one matrices](#triangular-rotation-factorization-of-real-determinant-one-matrices)
  - [Congruence subgroup](#congruence-subgroup)
    - [Principal congruence subgroup](#principal-congruence-subgroup)
    - [Gamma 0 congruence subgroup](#gamma-0-congruence-subgroup)
    - [Gamma 1 congruence subgroup](#gamma-1-congruence-subgroup)
      - [Number of cusps of Gamma 1 of prime level](#number-of-cusps-of-gamma-1-of-prime-level)
        - [Prime Gamma 1 cusp counts and widths](#prime-gamma-1-cusp-counts-and-widths)
- [Group homomorphism](#group-homomorphism)
  - [Homomorphism of abelian groups](#homomorphism-of-abelian-groups)
  - [Surjective group homomorphism](#surjective-group-homomorphism)
  - [Covering homomorphism](#covering-homomorphism)
  - [Homomorphism between cyclic groups](#homomorphism-between-cyclic-groups)
  - [Kernel of a group homomorphism](#kernel-of-a-group-homomorphism)
    - [Fibres of a group homomorphism are cosets of its kernel](#fibres-of-a-group-homomorphism-are-cosets-of-its-kernel)
  - [Image of a group homomorphism](#image-of-a-group-homomorphism)
- [Automorphism group](#automorphism-group)
  - [Holomorph](#holomorph)
  - [Inner automorphism](#inner-automorphism)
  - [Outer automorphism group](#outer-automorphism-group)
    - [Outer automorphism of a group](#outer-automorphism-of-a-group)
- [Group cohomology](group-cohomology.md)
  - [Cellular free resolution from a contractible universal cover](group-cohomology.md#cellular-free-resolution-from-a-contractible-universal-cover)
  - [Integral cohomological dimension of a group](group-cohomology.md#integral-cohomological-dimension-of-a-group)
    - [Stallings-Swan theorem](group-cohomology.md#stallings-swan-theorem)
  - [Poincare duality group](group-cohomology.md#poincare-duality-group)
    - [Normal finitely presented subgroups of three-dimensional duality groups](group-cohomology.md#normal-finitely-presented-subgroups-of-three-dimensional-duality-groups)
    - [Classification of two-dimensional Poincare duality groups](group-cohomology.md#classification-of-two-dimensional-poincare-duality-groups)
    - [Strebel infinite-index subgroup theorem](group-cohomology.md#strebel-infinite-index-subgroup-theorem)
    - [Extension rule for Poincare duality groups](group-cohomology.md#extension-rule-for-poincare-duality-groups)
    - [Finite-index invariance of Poincare duality for torsion-free groups](group-cohomology.md#finite-index-invariance-of-poincare-duality-for-torsion-free-groups)
  - [Mod-p cohomology ring of a cyclic group](group-cohomology.md#mod-p-cohomology-ring-of-a-cyclic-group)
  - [Dimension shifting in group cohomology](group-cohomology.md#dimension-shifting-in-group-cohomology)
  - [Tate cohomology of a finite group](group-cohomology.md#tate-cohomology-of-a-finite-group)
  - [Continuous cochains with topological coefficients](group-cohomology.md#continuous-cochains-with-topological-coefficients)
  - [Tate cohomology of a cyclic group](group-cohomology.md#tate-cohomology-of-a-cyclic-group)
    - [Cyclic cohomology of a regular lattice](group-cohomology.md#cyclic-cohomology-of-a-regular-lattice)
    - [Herbrand quotient](group-cohomology.md#herbrand-quotient)
      - [Herbrand quotient of a finite module](group-cohomology.md#herbrand-quotient-of-a-finite-module)
      - [Herbrand quotient of the local multiplicative group](group-cohomology.md#herbrand-quotient-of-the-local-multiplicative-group)
  - [Corestriction map in group cohomology](group-cohomology.md#corestriction-map-in-group-cohomology)
  - [Continuous cohomology of a profinite group](group-cohomology.md#continuous-cohomology-of-a-profinite-group)
    - [Cohomology continuity at closed subgroups](group-cohomology.md#cohomology-continuity-at-closed-subgroups)
    - [Cohomological dimension at a prime](group-cohomology.md#cohomological-dimension-at-a-prime)
      - [Trivial coefficients detect the cohomological dimension of a pro-p group](group-cohomology.md#trivial-coefficients-detect-the-cohomological-dimension-of-a-pro-p-group)
      - [Characteristic p Galois dimension bound](group-cohomology.md#characteristic-p-galois-dimension-bound)
  - [Nonabelian first cohomology](group-cohomology.md#nonabelian-first-cohomology)
  - [Periodic group cohomology](group-cohomology.md#periodic-group-cohomology)
    - [Cohomology ring of a finite cyclic group over its prime field](group-cohomology.md#cohomology-ring-of-a-finite-cyclic-group-over-its-prime-field)
    - [Periodic group cohomology from a free sphere action](group-cohomology.md#periodic-group-cohomology-from-a-free-sphere-action)
  - [Projective-resolution definition of group cohomology](group-cohomology.md#projective-resolution-definition-of-group-cohomology)
    - [Group cohomology commutes with finite direct sums](group-cohomology.md#group-cohomology-commutes-with-finite-direct-sums)
    - [Koszul resolution for a rank-two free abelian group](group-cohomology.md#koszul-resolution-for-a-rank-two-free-abelian-group)
      - [Second cohomology of a rank-two free abelian group with truncated group-ring coefficients](group-cohomology.md#second-cohomology-of-a-rank-two-free-abelian-group-with-truncated-group-ring-coefficients)
  - [Coinduced module](group-cohomology.md#coinduced-module)
    - [Shapiro's lemma](group-cohomology.md#shapiro-s-lemma)
      - [Hom functor adjunction for a coinduced module](group-cohomology.md#hom-functor-adjunction-for-a-coinduced-module)
  - [Conjugation module of a group ring](group-cohomology.md#conjugation-module-of-a-group-ring)
    - [Group cohomology of a conjugation module](group-cohomology.md#group-cohomology-of-a-conjugation-module)
  - [Integral cohomology of a finite cyclic group](group-cohomology.md#integral-cohomology-of-a-finite-cyclic-group)
    - [Periodic resolution of a finite cyclic group](group-cohomology.md#periodic-resolution-of-a-finite-cyclic-group)
  - [Group extension](group-cohomology.md#group-extension)
    - [Torsion-free finite extension of a lattice](group-cohomology.md#torsion-free-finite-extension-of-a-lattice)
    - [Split group extension](group-cohomology.md#split-group-extension)
      - [Section normal form for a split group extension](group-cohomology.md#section-normal-form-for-a-split-group-extension)
    - [Equivalent group extensions](group-cohomology.md#equivalent-group-extensions)
    - [Fiber product of groups](group-cohomology.md#fiber-product-of-groups)
      - [Mihailova subgroup](group-cohomology.md#mihailova-subgroup)
    - [Second group cohomology classifies group extensions](group-cohomology.md#second-group-cohomology-classifies-group-extensions)
      - [Integral central extensions of a rank-two free abelian group](group-cohomology.md#integral-central-extensions-of-a-rank-two-free-abelian-group)
      - [Extension cocycle](group-cohomology.md#extension-cocycle)
  - [Group cocycle](group-cohomology.md#group-cocycle)
    - [One-cocycle](group-cohomology.md#one-cocycle)
      - [Galois 1-cocycle](group-cohomology.md#galois-1-cocycle)
      - [Crossed homomorphism](group-cohomology.md#crossed-homomorphism)
        - [Principal crossed homomorphism](group-cohomology.md#principal-crossed-homomorphism)
    - [Two-cocycle](group-cohomology.md#two-cocycle)
      - [Normalized two-cocycle](group-cohomology.md#normalized-two-cocycle)
  - [Group coboundary](group-cohomology.md#group-coboundary)
  - [Group cochain](group-cohomology.md#group-cochain)
  - [Long exact sequence in group cohomology](group-cohomology.md#long-exact-sequence-in-group-cohomology)
  - [Finite-group cohomology is annihilated by the group order](group-cohomology.md#finite-group-cohomology-is-annihilated-by-the-group-order)
    - [Restriction-corestriction identity in group cohomology](group-cohomology.md#restriction-corestriction-identity-in-group-cohomology)
  - [Mac Lane exact sequence for a free presentation](group-cohomology.md#mac-lane-exact-sequence-for-a-free-presentation)
  - [Lyndon–Hochschild–Serre spectral sequence](group-cohomology.md#lyndon-hochschild-serre-spectral-sequence)
    - [Cyclic-extension shift of group-ring cohomology](group-cohomology.md#cyclic-extension-shift-of-group-ring-cohomology)
    - [Five-term exact sequence in group cohomology](group-cohomology.md#five-term-exact-sequence-in-group-cohomology)
      - [Inflation-restriction exact sequence](group-cohomology.md#inflation-restriction-exact-sequence)
      - [Inflation map in group cohomology](group-cohomology.md#inflation-map-in-group-cohomology)
      - [Restriction map in group cohomology](group-cohomology.md#restriction-map-in-group-cohomology)
      - [Transgression in group cohomology](group-cohomology.md#transgression-in-group-cohomology)
    - [Integral cohomology of the dihedral group of order ten](group-cohomology.md#integral-cohomology-of-the-dihedral-group-of-order-ten)
- [Group homology](#group-homology)
  - [Homology of a finite cyclic group](#homology-of-a-finite-cyclic-group)
  - [Schur multiplier](#schur-multiplier)
    - [Hopf's formula](#hopf-s-formula)
    - [Schur multiplier of an abelian group](#schur-multiplier-of-an-abelian-group)
- [Finite group theory](finite-group-theory.md)
  - [Group of order six](finite-group-theory.md#group-of-order-six)
  - [Fitting subgroup](finite-group-theory.md#fitting-subgroup)
    - [Fitting subgroup is self-centralizing in soluble groups](finite-group-theory.md#fitting-subgroup-is-self-centralizing-in-soluble-groups)
    - [Fitting subgroup centralizes the socle](finite-group-theory.md#fitting-subgroup-centralizes-the-socle)
    - [Nilpotent normal subgroup](finite-group-theory.md#nilpotent-normal-subgroup)
    - [p-core](finite-group-theory.md#p-core)
  - [Classification of groups of order ten](finite-group-theory.md#classification-of-groups-of-order-ten)
  - [Almost simple group](finite-group-theory.md#almost-simple-group)
  - [Heisenberg group over a prime field](finite-group-theory.md#heisenberg-group-over-a-prime-field)
    - [Abelian plane subgroup of a finite Heisenberg group](finite-group-theory.md#abelian-plane-subgroup-of-a-finite-heisenberg-group)
  - [Tetrahedral symmetry](finite-group-theory.md#tetrahedral-symmetry)
    - [Tetrahedral quotient onto the cyclic group of order three](finite-group-theory.md#tetrahedral-quotient-onto-the-cyclic-group-of-order-three)
    - [Tetrahedral rotation conjugacy classes](finite-group-theory.md#tetrahedral-rotation-conjugacy-classes)
  - [Group of order eight](finite-group-theory.md#group-of-order-eight)
  - [Feit–Thompson theorem](finite-group-theory.md#feit-thompson-theorem)
  - [Alternating group](finite-group-theory.md#alternating-group)
    - [Maximal subgroups of A5](finite-group-theory.md#maximal-subgroups-of-a5)
    - [Automorphisms of alternating groups from triple supports](finite-group-theory.md#automorphisms-of-alternating-groups-from-triple-supports)
    - [Connected triple supports generate an alternating group](finite-group-theory.md#connected-triple-supports-generate-an-alternating-group)
    - [Conjugacy classes of the alternating group on six letters](finite-group-theory.md#conjugacy-classes-of-the-alternating-group-on-six-letters)
  - [P-group](finite-group-theory.md#p-group)
  - [Symmetric group](finite-group-theory.md#symmetric-group)
    - [Symmetric group on three points](finite-group-theory.md#symmetric-group-on-three-points)
    - [Normal subgroups and quotients of the symmetric group on three letters](finite-group-theory.md#normal-subgroups-and-quotients-of-the-symmetric-group-on-three-letters)
    - [Automorphisms of the symmetric group](finite-group-theory.md#automorphisms-of-the-symmetric-group)
      - [Symmetric-group involution class-size collision](finite-group-theory.md#symmetric-group-involution-class-size-collision)
    - [Permutation group](finite-group-theory.md#permutation-group)
      - [Oligomorphic permutation group](finite-group-theory.md#oligomorphic-permutation-group)
    - [A cycle and a transposition generate the symmetric group exactly at coprime separation](finite-group-theory.md#a-cycle-and-a-transposition-generate-the-symmetric-group-exactly-at-coprime-separation)
    - [Transpositions on a connected graph generate the symmetric group](finite-group-theory.md#transpositions-on-a-connected-graph-generate-the-symmetric-group)
    - [Parity of a permutation](finite-group-theory.md#parity-of-a-permutation)
      - [Sign homomorphism](finite-group-theory.md#sign-homomorphism)
    - [Permutation cycle](finite-group-theory.md#permutation-cycle)
      - [Cycle type](finite-group-theory.md#cycle-type)
        - [Permutation order and sign do not determine conjugacy](finite-group-theory.md#permutation-order-and-sign-do-not-determine-conjugacy)
        - [Permutation conjugate to its square](finite-group-theory.md#permutation-conjugate-to-its-square)
        - [Transposition changes the cycle count by one](finite-group-theory.md#transposition-changes-the-cycle-count-by-one)
      - [Three-cycle](finite-group-theory.md#three-cycle)
      - [Disjoint permutation cycles](finite-group-theory.md#disjoint-permutation-cycles)
    - [Support of a permutation](finite-group-theory.md#support-of-a-permutation)
    - [Sign of a permutation](finite-group-theory.md#sign-of-a-permutation)
      - [Odd permutation](finite-group-theory.md#odd-permutation)
      - [Even permutation](finite-group-theory.md#even-permutation)
  - [Quaternion group](finite-group-theory.md#quaternion-group)
    - [Quaternion group modulo its centre](finite-group-theory.md#quaternion-group-modulo-its-centre)
    - [Character table of the quaternion group](finite-group-theory.md#character-table-of-the-quaternion-group)
    - [Minimal faithful permutation degree of the quaternion group](finite-group-theory.md#minimal-faithful-permutation-degree-of-the-quaternion-group)
  - [Dicyclic group](finite-group-theory.md#dicyclic-group)
    - [Order-twelve dicyclic character table](finite-group-theory.md#order-twelve-dicyclic-character-table)
    - [Dicyclic character table](finite-group-theory.md#dicyclic-character-table)
  - [Finite p-group](finite-group-theory.md#finite-p-group)
    - [p-subgroup](finite-group-theory.md#p-subgroup)
      - [p-radical subgroup](finite-group-theory.md#p-radical-subgroup)
    - [Lower p-series](finite-group-theory.md#lower-p-series)
    - [Powerful p-group](finite-group-theory.md#powerful-p-group)
      - [Minimal cyclic factorization criterion for powerful p-groups](finite-group-theory.md#minimal-cyclic-factorization-criterion-for-powerful-p-groups)
      - [Subgroup generator bound for a powerful finite p-group](finite-group-theory.md#subgroup-generator-bound-for-a-powerful-finite-p-group)
      - [Power lifting in a powerful p-group](finite-group-theory.md#power-lifting-in-a-powerful-p-group)
      - [Powerfully embedded subgroup](finite-group-theory.md#powerfully-embedded-subgroup)
    - [Classification of groups of order p squared](finite-group-theory.md#classification-of-groups-of-order-p-squared)
    - [Normalizer condition for finite p-groups](finite-group-theory.md#normalizer-condition-for-finite-p-groups)
    - [Central intersection property of normal subgroups of finite p-groups](finite-group-theory.md#central-intersection-property-of-normal-subgroups-of-finite-p-groups)
    - [Nontrivial center of a finite p-group](finite-group-theory.md#nontrivial-center-of-a-finite-p-group)
    - [Frattini subgroup](finite-group-theory.md#frattini-subgroup)
      - [Frattini lifting of nilpotence](finite-group-theory.md#frattini-lifting-of-nilpotence)
      - [Non-generator of a finite group](finite-group-theory.md#non-generator-of-a-finite-group)
      - [Frattini quotient](finite-group-theory.md#frattini-quotient)
        - [Burnside basis theorem](finite-group-theory.md#burnside-basis-theorem)
  - [Simple group](finite-group-theory.md#simple-group)
    - [Finite simple group](finite-group-theory.md#finite-simple-group)
    - [Simple groups with order a power of two times fifteen](finite-group-theory.md#simple-groups-with-order-a-power-of-two-times-fifteen)
    - [Iwasawa simplicity lemma](finite-group-theory.md#iwasawa-simplicity-lemma)
    - [Simplicity of the alternating group on six letters](finite-group-theory.md#simplicity-of-the-alternating-group-on-six-letters)
    - [Simplicity of alternating groups](finite-group-theory.md#simplicity-of-alternating-groups)
    - [Finite nonabelian simple group](finite-group-theory.md#finite-nonabelian-simple-group)
      - [Least-prime divisibility constraint for a finite simple group](finite-group-theory.md#least-prime-divisibility-constraint-for-a-finite-simple-group)
      - [Mathieu group](finite-group-theory.md#mathieu-group)
      - [Ree group of type G2](finite-group-theory.md#ree-group-of-type-g2)
      - [Suzuki group of Lie type](finite-group-theory.md#suzuki-group-of-lie-type)
    - [Simplicity of the alternating group A5](finite-group-theory.md#simplicity-of-the-alternating-group-a5)
    - [Smallest nonabelian simple group](finite-group-theory.md#smallest-nonabelian-simple-group)
  - [General linear group over a finite field](finite-group-theory.md#general-linear-group-over-a-finite-field)
    - [Conjugacy-class generating function for finite general linear groups](finite-group-theory.md#conjugacy-class-generating-function-for-finite-general-linear-groups)
    - [Unitary group over a finite field](finite-group-theory.md#unitary-group-over-a-finite-field)
    - [Projective special unitary group over a finite field](finite-group-theory.md#projective-special-unitary-group-over-a-finite-field)
    - [Parabolic stabilizer of a subspace](finite-group-theory.md#parabolic-stabilizer-of-a-subspace)
    - [Symplectic group over a finite field](finite-group-theory.md#symplectic-group-over-a-finite-field)
      - [Symplectic quotient of the binary subset module](finite-group-theory.md#symplectic-quotient-of-the-binary-subset-module)
      - [Perfectness of finite symplectic groups](finite-group-theory.md#perfectness-of-finite-symplectic-groups)
      - [Symplectic transvection](finite-group-theory.md#symplectic-transvection)
      - [Projective symplectic group over a finite field](finite-group-theory.md#projective-symplectic-group-over-a-finite-field)
    - [Inverse-transpose automorphism](finite-group-theory.md#inverse-transpose-automorphism)
    - [Maximal subgroups of GL3 over F2](finite-group-theory.md#maximal-subgroups-of-gl3-over-f2)
      - [Elementary abelian subgroups in GL3 over F2](finite-group-theory.md#elementary-abelian-subgroups-in-gl3-over-f2)
    - [Singer cycle](finite-group-theory.md#singer-cycle)
    - [Order-p matrices in GL2 over the prime field](finite-group-theory.md#order-p-matrices-in-gl2-over-the-prime-field)
    - [Faithful four-point action of GL2 over F2](finite-group-theory.md#faithful-four-point-action-of-gl2-over-f2)
    - [Order of a general linear group over a finite field](finite-group-theory.md#order-of-a-general-linear-group-over-a-finite-field)
    - [Upper unitriangular group](finite-group-theory.md#upper-unitriangular-group)
      - [Center of an upper unitriangular group](finite-group-theory.md#center-of-an-upper-unitriangular-group)
      - [Unitriangular matrix power formula](finite-group-theory.md#unitriangular-matrix-power-formula)
      - [Unitriangular group of degree three over F3](finite-group-theory.md#unitriangular-group-of-degree-three-over-f3)
    - [Projective general linear group action on the projective line](finite-group-theory.md#projective-general-linear-group-action-on-the-projective-line)
      - [Sharply three-transitive on a projective line](finite-group-theory.md#sharply-three-transitive-on-a-projective-line)
      - [Projective line](finite-group-theory.md#projective-line)
      - [Sylow 2-subgroup of PGL2 over F4](finite-group-theory.md#sylow-2-subgroup-of-pgl2-over-f4)
    - [Special linear group over a finite field](finite-group-theory.md#special-linear-group-over-a-finite-field)
      - [Unique involution in SL2 over an odd field](finite-group-theory.md#unique-involution-in-sl2-over-an-odd-field)
      - [SL2 over F2 as a permutation group](finite-group-theory.md#sl2-over-f2-as-a-permutation-group)
      - [Projective special linear group over a finite field](finite-group-theory.md#projective-special-linear-group-over-a-finite-field)
        - [Exterior-square realization of PSL4 over F2](finite-group-theory.md#exterior-square-realization-of-psl4-over-f2)
        - [Projective special linear group over the field with five elements](finite-group-theory.md#projective-special-linear-group-over-the-field-with-five-elements)
          - [Quaternion construction of an index-five subgroup of PSL2 over F5](finite-group-theory.md#quaternion-construction-of-an-index-five-subgroup-of-psl2-over-f5)
      - [Unipotent conjugacy in SL2 over a finite field](finite-group-theory.md#unipotent-conjugacy-in-sl2-over-a-finite-field)
      - [SL2 action on a finite projective line](finite-group-theory.md#sl2-action-on-a-finite-projective-line)
  - [Dihedral group](finite-group-theory.md#dihedral-group)
    - [Dihedral symmetry](finite-group-theory.md#dihedral-symmetry)
    - [Symmetry group of a square](finite-group-theory.md#symmetry-group-of-a-square)
      - [Character table of the symmetry group of a square](finite-group-theory.md#character-table-of-the-symmetry-group-of-a-square)
      - [Conjugacy classes of the symmetry group of a square](finite-group-theory.md#conjugacy-classes-of-the-symmetry-group-of-a-square)
    - [Conjugacy classes of a finite dihedral group](finite-group-theory.md#conjugacy-classes-of-a-finite-dihedral-group)
    - [Dihedral splitting when the half-rotation order is odd](finite-group-theory.md#dihedral-splitting-when-the-half-rotation-order-is-odd)
    - [Classification of subgroups of a dihedral group](finite-group-theory.md#classification-of-subgroups-of-a-dihedral-group)
    - [Dihedral subgroups of every divisor order](finite-group-theory.md#dihedral-subgroups-of-every-divisor-order)
    - [Involutions in an even dihedral group](finite-group-theory.md#involutions-in-an-even-dihedral-group)
  - [Sylow theorems](finite-group-theory.md#sylow-theorems)
    - [Sylow basis](finite-group-theory.md#sylow-basis)
      - [Counting Sylow bases in a coprime elementary abelian extension](finite-group-theory.md#counting-sylow-bases-in-a-coprime-elementary-abelian-extension)
    - [Sylow existence by subset action](finite-group-theory.md#sylow-existence-by-subset-action)
    - [A group of order 56 has a normal Sylow subgroup](finite-group-theory.md#a-group-of-order-56-has-a-normal-sylow-subgroup)
    - [Frattini argument](finite-group-theory.md#frattini-argument)
    - [Groups of order p squared q are not simple](finite-group-theory.md#groups-of-order-p-squared-q-are-not-simple)
    - [Sylow subgroup](finite-group-theory.md#sylow-subgroup)
    - [Nonabelian group of order pq](finite-group-theory.md#nonabelian-group-of-order-pq)
      - [Nonabelian group of order 21](finite-group-theory.md#nonabelian-group-of-order-21)
    - [Conjugation action on Sylow subgroups](finite-group-theory.md#conjugation-action-on-sylow-subgroups)
      - [Strengthened Sylow congruence from intersections](finite-group-theory.md#strengthened-sylow-congruence-from-intersections)
      - [Simple group embedding from Sylow conjugation](finite-group-theory.md#simple-group-embedding-from-sylow-conjugation)
    - [Sylow subgroups of S3, S4 and A5](finite-group-theory.md#sylow-subgroups-of-s3-s4-and-a5)
    - [Sylow containment from a coset fixed point](finite-group-theory.md#sylow-containment-from-a-coset-fixed-point)
    - [Sylow counts in a faithful degree-seven action with S4 point stabilizers](finite-group-theory.md#sylow-counts-in-a-faithful-degree-seven-action-with-s4-point-stabilizers)
    - [Even-involution coset fixed-point lemma](finite-group-theory.md#even-involution-coset-fixed-point-lemma)
  - [Cauchy theorem for groups](finite-group-theory.md#cauchy-theorem-for-groups)
    - [Cyclic-tuple proof of Cauchy theorem](finite-group-theory.md#cyclic-tuple-proof-of-cauchy-theorem)
  - [Power-map criterion for a finite group](finite-group-theory.md#power-map-criterion-for-a-finite-group)
  - [Composition series](finite-group-theory.md#composition-series)
    - [Composition chains in products with S5](finite-group-theory.md#composition-chains-in-products-with-s5)
    - [Composition length](finite-group-theory.md#composition-length)
    - [Jordan–Hölder factor](finite-group-theory.md#jordan-holder-factor)
      - [Jordan–Hölder theorem](finite-group-theory.md#jordan-holder-theorem)
  - [Klein four-group](finite-group-theory.md#klein-four-group)
    - [Character table of the Klein four-group](finite-group-theory.md#character-table-of-the-klein-four-group)
    - [Group generated by sign reversal and reciprocation](finite-group-theory.md#group-generated-by-sign-reversal-and-reciprocation)
    - [Equivalent sheared representations of the Klein four-group](finite-group-theory.md#equivalent-sheared-representations-of-the-klein-four-group)
- [Residually finite group](#residually-finite-group)
  - [Finite residual](#finite-residual)
    - [Finite residual contains surjective endomorphism kernels](#finite-residual-contains-surjective-endomorphism-kernels)
  - [Residual finiteness of semidirect products](#residual-finiteness-of-semidirect-products)
  - [Conjugacy separable group](#conjugacy-separable-group)
  - [Subgroup of a residually finite group](#subgroup-of-a-residually-finite-group)
  - [Reduction modulo a prime in an integral matrix group](#reduction-modulo-a-prime-in-an-integral-matrix-group)
  - [Infinite residually finite group is not simple](#infinite-residually-finite-group-is-not-simple)
- [Hopfian group](#hopfian-group)
  - [Non-Hopfian group](#non-hopfian-group)
- [Torsion element](#torsion-element)
  - [Torsion group](#torsion-group)
    - [Infinite residually finite torsion group](#infinite-residually-finite-torsion-group)
    - [Locally finite group](#locally-finite-group)
      - [Local finiteness is closed under extensions](#local-finiteness-is-closed-under-extensions)
  - [Torsion subgroup](#torsion-subgroup)
    - [Torsion subgroup killed by an integer](#torsion-subgroup-killed-by-an-integer)
    - [Primary torsion subgroup at a prime](#primary-torsion-subgroup-at-a-prime)
- [Free abelian group](#free-abelian-group)
  - [Saturated sublattice](#saturated-sublattice)
  - [Primitive lattice element](#primitive-lattice-element)
- [Normal subgroup](#normal-subgroup)
  - [p-residual of a finite group](#p-residual-of-a-finite-group)
  - [Complement of a normal subgroup](#complement-of-a-normal-subgroup)
  - [Normal subgroups of coprime order commute](#normal-subgroups-of-coprime-order-commute)
  - [Normal p-complement](#normal-p-complement)
    - [p-nilpotent group](#p-nilpotent-group)
      - [Thompson's character-degree normal complement theorem](#thompson-s-character-degree-normal-complement-theorem)
      - [Isaacs' character-degree criterion for p-nilpotency](#isaacs-character-degree-criterion-for-p-nilpotency)
  - [Maximal normal subgroup](#maximal-normal-subgroup)
    - [Finitely generated groups have maximal proper normal subgroups](#finitely-generated-groups-have-maximal-proper-normal-subgroups)
  - [Subnormal series](#subnormal-series)
    - [Schreier refinement theorem](#schreier-refinement-theorem)
    - [Zassenhaus butterfly lemma](#zassenhaus-butterfly-lemma)
    - [Normal series of a group](#normal-series-of-a-group)
      - [Chief series](#chief-series)
        - [Chief factor](#chief-factor)
  - [Minimal normal subgroup](#minimal-normal-subgroup)
    - [Minimal normal subgroups of finite solvable groups are elementary abelian](#minimal-normal-subgroups-of-finite-solvable-groups-are-elementary-abelian)
    - [Direct-product structure of a finite minimal normal subgroup](#direct-product-structure-of-a-finite-minimal-normal-subgroup)
    - [Socle of a finite group](#socle-of-a-finite-group)
  - [Normal subgroup of order two is central](#normal-subgroup-of-order-two-is-central)
  - [Core (group theory)](#core-group-theory)
  - [Normal closure](#normal-closure)
  - [Preimage of a normal subgroup](#preimage-of-a-normal-subgroup)
  - [Image of a normal subgroup](#image-of-a-normal-subgroup)
- [Dedekind group](#dedekind-group)
- [Projective linear group](#projective-linear-group)
  - [Möbius group](#mobius-group)
    - [Möbius pointwise stabilizer of two points](#mobius-pointwise-stabilizer-of-two-points)
    - [Möbius transformations permuting three points](#mobius-transformations-permuting-three-points)
    - [Subgroup generated by complex scalings and reciprocal inversion](#subgroup-generated-by-complex-scalings-and-reciprocal-inversion)
    - [Finite abelian subgroup of the Möbius group](#finite-abelian-subgroup-of-the-mobius-group)
  - [Möbius transformation](#mobius-transformation)
    - [Möbius translation-scaling-inversion factorization](#mobius-translation-scaling-inversion-factorization)
    - [Antipodal fixed-point classification of Möbius transformations](#antipodal-fixed-point-classification-of-mobius-transformations)
    - [Möbius conjugacy normal forms](#mobius-conjugacy-normal-forms)
      - [Iteration of a one-fixed-point Möbius transformation](#iteration-of-a-one-fixed-point-mobius-transformation)
      - [Finite-order Möbius orbit sizes](#finite-order-mobius-orbit-sizes)
    - [Cayley transform (complex analysis)](#cayley-transform-complex-analysis)
    - [Möbius transformations from the real axis to the unit circle](#mobius-transformations-from-the-real-axis-to-the-unit-circle)
    - [Möbius scaling generated by translations and reciprocal inversion](#mobius-scaling-generated-by-translations-and-reciprocal-inversion)
    - [Blaschke factor](#blaschke-factor)
    - [Antipodal fixed points do not characterize sphere rotations](#antipodal-fixed-points-do-not-characterize-sphere-rotations)
    - [Loxodromic Möbius transformation](#loxodromic-mobius-transformation)
    - [Real determinant-one Möbius orbits](#real-determinant-one-mobius-orbits)
    - [Concentric normalization of disjoint circles](#concentric-normalization-of-disjoint-circles)
    - [Cross-ratio](#cross-ratio)
      - [Cross-ratio construction of generalized-circle reflection](#cross-ratio-construction-of-generalized-circle-reflection)
      - [Ptolemy's theorem](#ptolemy-s-theorem)
      - [Möbius invariance of the cross-ratio](#mobius-invariance-of-the-cross-ratio)
      - [Cross-ratio with second point mapped to zero](#cross-ratio-with-second-point-mapped-to-zero)
      - [Real cross-ratio criterion for a generalized circle](#real-cross-ratio-criterion-for-a-generalized-circle)
    - [Generalized circle under a Möbius transformation](#generalized-circle-under-a-mobius-transformation)
      - [Reciprocal transformation of a generalized circle](#reciprocal-transformation-of-a-generalized-circle)
      - [Inversion in a circle](#inversion-in-a-circle)
    - [Affine subgroup of the Möbius group](#affine-subgroup-of-the-mobius-group)
    - [Fixed point of a Möbius transformation](#fixed-point-of-a-mobius-transformation)
      - [Conjugation of a Möbius transformation with two distinct fixed points](#conjugation-of-a-mobius-transformation-with-two-distinct-fixed-points)
      - [Prescribed fixed points of a Möbius transformation](#prescribed-fixed-points-of-a-mobius-transformation)
      - [Fixed points of a finite-order Möbius transformation](#fixed-points-of-a-finite-order-mobius-transformation)
    - [Constant-argument locus of a Möbius transformation](#constant-argument-locus-of-a-mobius-transformation)
    - [Classification of Möbius transformations by trace](#classification-of-mobius-transformations-by-trace)
    - [Möbius maps commuting with reflection in the unit circle](#mobius-maps-commuting-with-reflection-in-the-unit-circle)
  - [Matrix representative of a Möbius transformation](#matrix-representative-of-a-mobius-transformation)
- [Semidirect product](#semidirect-product)
  - [Central translations in a linear semidirect product](#central-translations-in-a-linear-semidirect-product)
  - [Finite presentation of a semidirect product](#finite-presentation-of-a-semidirect-product)
  - [Coprime splitting over an elementary abelian normal subgroup](#coprime-splitting-over-an-elementary-abelian-normal-subgroup)
  - [Twisted cyclic pair group](#twisted-cyclic-pair-group)
  - [Presentation of a semidirect product](#presentation-of-a-semidirect-product)
  - [Affine group of the complex line](#affine-group-of-the-complex-line)
    - [Commutator subgroup of the affine group of the complex line](#commutator-subgroup-of-the-affine-group-of-the-complex-line)
  - [Wreath product](#wreath-product)
    - [Product action of a wreath product](#product-action-of-a-wreath-product)
    - [Permutation wreath product](#permutation-wreath-product)
    - [Lamplighter group](#lamplighter-group)
  - [Abelianization of a semidirect product by the integers](#abelianization-of-a-semidirect-product-by-the-integers)
  - [Affine group over a finite field](#affine-group-over-a-finite-field)
    - [Involution orbits in an affine group of odd prime degree](#involution-orbits-in-an-affine-group-of-odd-prime-degree)
    - [Affine Galois group of a prime-radical splitting field](#affine-galois-group-of-a-prime-radical-splitting-field)
    - [Affine Galois group of the splitting field of x to the p minus two](#affine-galois-group-of-the-splitting-field-of-x-to-the-p-minus-two)
    - [Affine semidirect product of cyclic groups of orders eleven and five](#affine-semidirect-product-of-cyclic-groups-of-orders-eleven-and-five)
      - [Conjugacy classes in the affine semidirect product of orders eleven and five](#conjugacy-classes-in-the-affine-semidirect-product-of-orders-eleven-and-five)
- [Virtually cyclic group](#virtually-cyclic-group)
- [Solvable group](#solvable-group)
  - [Supersolvable group](#supersolvable-group)
  - [Finitely generated soluble torsion groups are finite](#finitely-generated-soluble-torsion-groups-are-finite)
  - [Virtually solvable group](#virtually-solvable-group)
    - [Finite-index characteristic soluble subgroup](#finite-index-characteristic-soluble-subgroup)
  - [Derived series](#derived-series)
  - [Metabelian group](#metabelian-group)
    - [Finite metabelian groups are monomial](#finite-metabelian-groups-are-monomial)
  - [Polycyclic group](#polycyclic-group)
    - [Polycyclic groups are virtually poly-infinite cyclic](#polycyclic-groups-are-virtually-poly-infinite-cyclic)
    - [Hirsch length](#hirsch-length)
    - [Poly-infinite cyclic group](#poly-infinite-cyclic-group)
  - [Nilpotent group](#nilpotent-group)
    - [Nilpotence criterion for an abelian-by-cyclic group](#nilpotence-criterion-for-an-abelian-by-cyclic-group)
    - [Malcev completion of a torsion-free nilpotent group](#malcev-completion-of-a-torsion-free-nilpotent-group)
    - [Commutator collection with fixed generators in nilpotent groups](#commutator-collection-with-fixed-generators-in-nilpotent-groups)
    - [Fixed-generator commutator collection in nilpotent groups](#fixed-generator-commutator-collection-in-nilpotent-groups)
    - [Finite nilpotent group decomposition](#finite-nilpotent-group-decomposition)
    - [Normalizer condition for nilpotent groups](#normalizer-condition-for-nilpotent-groups)
    - [Upper central series](#upper-central-series)
    - [Nilpotency class](#nilpotency-class)
      - [Nilpotency class of a direct product](#nilpotency-class-of-a-direct-product)
    - [Two-step nilpotent group](#two-step-nilpotent-group)
      - [Word collection in a two-step nilpotent group](#word-collection-in-a-two-step-nilpotent-group)
    - [Virtually nilpotent group](#virtually-nilpotent-group)
    - [Lower central series](#lower-central-series)
      - [Bounded-exponent finitely generated nilpotent group order bound](#bounded-exponent-finitely-generated-nilpotent-group-order-bound)
    - [Free nilpotent group](#free-nilpotent-group)
      - [Central nonsplit extension of the integer Heisenberg group by $\mathbb Z^2$](#central-nonsplit-extension-of-the-integer-heisenberg-group-by-mathbb-z-2)
    - [Central series](#central-series)
      - [Central-series comparison theorem](#central-series-comparison-theorem)
- [Exponential growth of a group](#exponential-growth-of-a-group)
- [Exponent of a finite group](#exponent-of-a-finite-group)
  - [Finite group of prime exponent has prime-power order](#finite-group-of-prime-exponent-has-prime-power-order)
  - [Finite subgroup of a field multiplicative group is cyclic](#finite-subgroup-of-a-field-multiplicative-group-is-cyclic)
- [Order of an element of a finite group](#order-of-an-element-of-a-finite-group)
- [Order (group theory)](#order-group-theory)

## Transfer (group theory)

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transfer_(group_theory))

For a subgroup $H$ of finite index, choose representatives $t$ of right cosets $Ht$. Write $tg=h(t,g)t_g$ with $h(t,g)\in H$. The transfer is $V_{G,H}(g)=\prod_t h(t,g)\pmod{H'}$. Replacing $t$ by $a_tt$ multiplies each factor by $a_t$ on the left and $a_{t_g}^{-1}$ on the right; these cancel in the [abelianization](#abelianization) because $t\mapsto t_g$ is a permutation. The identity $h(t,g_1g_2)=h(t,g_1)h(t_{g_1},g_2)$ proves the [group homomorphism](#group-homomorphism) property after multiplying all factors.

### Burnside transfer theorem

↑ **Parent:** [Transfer (group theory)](#transfer-group-theory)

The hypothesis makes $P$ abelian and makes any two conjugate elements of $P$ equal. For the latter assertion, Sylow conjugacy inside the centralizer of the target element adjusts a conjugating element into $N_G(P)$, where it centralizes $P$. Evaluating [group transfer](#transfer-group-theory) to $P$ on an element $u\in P$, each coset cycle contributes a conjugate of $u$ raised to the cycle length, hence that same power of $u$. The restriction is consequently $u\mapsto u^{[G:P]}$, an automorphism of the abelian $p$-group. Transfer is surjective, and its kernel is the required [normal p-complement](#normal-p-complement).

#### Cyclic Sylow subgroup at the least prime gives a normal complement

↑ **Parent:** [Burnside transfer theorem](#burnside-transfer-theorem)

Let $p$ be the smallest prime dividing the order of a [finite group](group.md#finite-group), and suppose its [Sylow subgroup](finite-group-theory.md#sylow-subgroup) $P$ is cyclic of order $p^a$. [Conjugation](group-action.md#conjugation) embeds $N_G(P)/C_G(P)$ into $\operatorname{Aut}(P)$, of order $p^{a-1}(p-1)$. Since $P\subseteq C_G(P)$, this quotient has order prime to $p$. Its remaining possible prime divisors are smaller than $p$ and cannot divide $|G|$. Thus $N_G(P)=C_G(P)$, and the [Burnside transfer theorem](#burnside-transfer-theorem) gives a [normal p-complement](#normal-p-complement).

<h2 id="prufer-rank">Prüfer rank</h2>

↑ **Parent:** [Group theory](group-theory.md)

The Prüfer rank bounds the number of [generators of a group](group.md#generator-of-a-group) needed for each finitely generated subgroup, without requiring the ambient group to be finitely generated. The additive [group](group.md) $\mathbb Q$ has Prüfer rank one: any finitely generated subgroup has a common denominator and is cyclic, but no finite collection generates all rational numbers. Prüfer rank cannot increase under taking subgroups or quotients; for quotients, lift a finite generating set and apply the rank bound to the subgroup generated by its lifts.

<h3 id="prufer-rank-bound-for-extensions">Prüfer rank bound for extensions</h3>

↑ **Parent:** [Prüfer rank](#prufer-rank)

For a [normal subgroup](#normal-subgroup) $N$ with [Prüfer rank](#prufer-rank) $r$ and quotient of rank $s$, let $H=\langle h_1,\ldots,h_k\rangle\le G$. Choose at most $s$ elements $x_j\in H$ generating the image of $H$. Write $h_i=w_i(x_1,\ldots,x_s)n_i$ with $n_i\in N\cap H$. The finitely generated subgroup $\langle n_1,\ldots,n_k\rangle$ needs at most $r$ generators, so $H$ needs at most $r+s$. The full intersection $H\cap N$ need not be finitely generated.

## Maximal condition on subgroups

↑ **Parent:** [Group theory](group-theory.md)

A [group](group.md) has the maximal condition on subgroups when every ascending sequence of [subgroups](group.md#subgroup) eventually stabilizes. Equivalently, every subgroup is a [finitely generated group](group.md#finitely-generated-group). If a subgroup were not finitely generated, repeatedly adjoining an element outside the previously generated subgroup would give a strictly ascending sequence. Conversely, generators of the union of an ascending sequence all lie in one term, making that term the whole union. This condition is preserved by [group extensions](group-cohomology.md#group-extension) because each subgroup is an extension of its intersection with the kernel by its image in the quotient.

## Group

↑ **Parent:** [Group theory](group-theory.md)

[This section is present in another page, follow this link to view it.](group.md)

## First isomorphism theorem

↑ **Parent:** [Group theory](group-theory.md)

For a [group homomorphism](#group-homomorphism) $\varphi:G\to H$, the [group isomorphism](algebra.md#group-isomorphism) $g\ker\varphi\mapsto\varphi(g)$ gives

$$
G/\ker\varphi\cong\operatorname{im}\varphi.
$$

The [group kernel](#kernel-of-a-group-homomorphism) records which inputs become indistinguishable, and the image records which outputs actually occur. The [first isomorphism theorem](#first-isomorphism-theorem) says that identifying precisely those indistinguishable inputs gives a [group](group.md) isomorphic to the image. It is one of the general [isomorphism theorems](algebra.md#isomorphism-theorems). [McKernan, MIT 18.703, Theorem 10.1: the first isomorphism theorem](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/b40d60898322bbd1d63410b0a925946a_MIT18_703S13_pra_l_10.pdf).

For example, reduction modulo three gives a [surjective group homomorphism](#surjective-group-homomorphism) from the additive [cyclic group](group.md#cyclic-group) $\mathbb Z/6\mathbb Z$ to $\mathbb Z/3\mathbb Z$. Its [group kernel](#kernel-of-a-group-homomorphism) is $\{0,3\}$. The three [cosets](#coset) $\{0,3\}$, $\{1,4\}$, and $\{2,5\}$ become the three outputs zero, one, and two, respectively. Thus

$$
(\mathbb Z/6\mathbb Z)/\{0,3\}\cong\mathbb Z/3\mathbb Z.
$$

The [quotient group](#quotient-group) diagram shows both the identification and the resulting operation. More generally, [fibres of a group homomorphism are cosets of its kernel](#fibres-of-a-group-homomorphism-are-cosets-of-its-kernel) explains why this map is well-defined and [injective](algebra.md#injective-function); it is [surjective](algebra.md#surjective-function) onto the image by definition.

## Direct product of groups

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Direct_product_of_groups)

A direct product combines two [groups](group.md) into one while keeping their operations in separate coordinates. Its underlying [set](set.md) is the [Cartesian product](set-theory.md#cartesian-product) $G\times H$, and its [group operation](group.md#group-operation) is

$$
(g_1,h_1)(g_2,h_2)=(g_1g_2,h_1h_2).
$$

The [identity element](algebraic-operation.md#identity-element) is $(e_G,e_H)$, and the [inverse element](algebraic-operation.md#inverse-element) of $(g,h)$ is $(g^{-1},h^{-1})$. [Associativity](algebraic-operation.md#associative-property) follows coordinate by coordinate. For finite [groups](group.md), the [multiplication principle](combinatorics.md#rule-of-product) gives $|G\times H|=|G||H|$.

For example, write the [cyclic group](group.md#cyclic-group) $C_m$ as the additive [group](group.md) of [residue classes](modular-arithmetic.md#residue-class) modulo $m$. In $C_2\times C_3$,

$$
(1,2)+(1,2)=(0,1),
$$

since each coordinate reduces with its own [integer modulus](modular-arithmetic.md#modulus-in-modular-arithmetic). A pair can track two cyclic counters that advance independently. Updating the first coordinate does not alter the second, and vice versa.

This independence has an algebraic form. The embedded factor elements always [commute](algebraic-operation.md#commuting-elements):

$$
(g,e_H)(e_G,h)=(g,h)=(e_G,h)(g,e_H).
$$

The coordinate maps $(g,h)\mapsto g$ and $(g,h)\mapsto h$ are [group homomorphisms](#group-homomorphism), so one can analyze either component separately. This does not make the full product an [abelian group](group.md#abelian-group) when one of its factors is nonabelian: two arbitrary pairs need not [commute](algebraic-operation.md#commuting-elements).

The construction is useful in both directions. It builds a larger [group](group.md) from familiar pieces, while the [internal direct product theorem](#internal-direct-product-theorem) recognizes when an existing [group](group.md) can be separated into such pieces. A [cyclic group](group.md#cyclic-group) can sometimes be split this way; whether two finite cyclic factors combine into one [cyclic group](group.md#cyclic-group) is decided by the [cyclicity of a product of two finite cyclic groups](#cyclicity-of-a-product-of-two-finite-cyclic-groups). Definitions and the basic recognition theorems are developed in [Thomas Judson, Abstract Algebra: Theory and Applications, §9.2, Direct Products](https://judsonbooks.org/aata-files/aata-html/isomorph-section-direct-products.html).

### Direct product of cyclic groups of orders four and two

↑ **Parent:** [Direct product of groups](#direct-product-of-groups)

This [abelian group](group.md#abelian-group) has eight elements $c^ra^s$, with $r$ taken modulo four and $s$ modulo two. Its [group operation](group.md#group-operation) adds these exponent pairs separately. The elements of order two are $c^2,a,c^2a$, and the other four nonidentity elements $c,c^3,ca,c^3a$ have order four. It is a [direct product of groups](#direct-product-of-groups) rather than a [cyclic group](group.md#cyclic-group), since no element has order eight.

#### Subgroups of C4 times C2

↑ **Parent:** [Direct product of cyclic groups of orders four and two](#direct-product-of-cyclic-groups-of-orders-four-and-two)

With the generators $c,a$ of the [direct product of cyclic groups of orders four and two](#direct-product-of-cyclic-groups-of-orders-four-and-two), the [subgroups](group.md#subgroup) are the trivial group, the whole group, the three order-two groups $\langle c^2\rangle$, $\langle a\rangle$, $\langle c^2a\rangle$, and the three order-four groups $\langle c\rangle$, $\langle ca\rangle$, $\langle c^2,a\rangle$. These are exhaustive by [Lagrange's theorem](#lagrange-s-theorem): a proper nontrivial [subgroup](group.md#subgroup) has order two or four; an order-four [subgroup](group.md#subgroup) either contains an element of order four and is one of the two cyclic examples, or is precisely the four-element set killed by squaring. The latter is a [Klein four-group](finite-group-theory.md#klein-four-group).

### Cyclicity of a product of two finite cyclic groups

↑ **Parent:** [Direct product of groups](#direct-product-of-groups)

For positive [integers](integer.md) $m,n$, two finite [cyclic groups](group.md#cyclic-group) combine into one [cyclic group](group.md#cyclic-group) precisely when their [group orders](group.md#order-of-a-finite-group) are [coprime](divisibility.md#coprime-integers):

$$
C_m\times C_n\cong C_{mn}\quad\Longleftrightarrow\quad\gcd(m,n)=1.
$$

The reason is that both cyclic counters must return to their [identity elements](algebraic-operation.md#identity-element) simultaneously. If $a,b$ are [generators of a group](group.md#generator-of-a-group) for the two factors, the [order of a direct-product element](#order-of-a-direct-product-element) gives $\operatorname{ord}(a,b)=\operatorname{lcm}(m,n)$. The pair generates all $mn$ elements exactly when this [least common multiple](divisibility.md#least-common-multiple) is $mn$.

For $C_2\times C_3$, repeated addition of $(1,1)$ visits

$$
(0,0),(1,1),(0,2),(1,0),(0,1),(1,2),(0,0).
$$

All six pairs appear before the return, so $(1,1)$ is a generator. In contrast, in $C_2\times C_2$ the same step gives only $(0,0),(1,1),(0,0)$. Every nonidentity element has [order of a group element](#order-of-a-group-element) two, so none can generate all four pairs. This is the [Klein four-group](finite-group-theory.md#klein-four-group); there is no [group isomorphism](algebra.md#group-isomorphism) to $C_4$ even though both have four elements.

<a id="image-adding-the-same-pair-generates-all-of-c2-times-c3-but-only-a-two-element-subgroup-of-c2-times-c2"></a>
![](direct-product-cyclic-orbits.png)

**[Figure 1](#image-adding-the-same-pair-generates-all-of-c2-times-c3-but-only-a-two-element-subgroup-of-c2-times-c2). Adding the same pair generates all of C2 times C3 but only a two-element subgroup of C2 times C2**.

For a brief proof of the converse, each component [order of a group element](#order-of-a-group-element) divides the corresponding factor [group order](group.md#order-of-a-finite-group). Every pair's order therefore divides $\operatorname{lcm}(m,n)$. If $\gcd(m,n)>1$, this is smaller than $mn$, so no pair can generate the whole product. The [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) gives the explicit isomorphism in the [coprime](divisibility.md#coprime-integers) case: $t\bmod mn\mapsto(t\bmod m,t\bmod n)$.

### Order of a direct-product element

↑ **Parent:** [Direct product of groups](#direct-product-of-groups)

If the [order of a group element](#order-of-a-group-element) is $m$ for $g$ and $n$ for $h$, with both finite, then

$$
(g,h)^k=(g^k,h^k)=(e_G,e_H)
$$

exactly when both $m$ and $n$ divide $k$. The smallest positive such $k$ is their [least common multiple](divisibility.md#least-common-multiple), giving

$$
\operatorname{ord}(g,h)=\operatorname{lcm}(m,n).
$$

This concerns the orders of the selected elements, which need not equal the orders of their entire [groups](group.md). If either component has infinite [order of a group element](#order-of-a-group-element), no positive power can return the pair to the [identity element](algebraic-operation.md#identity-element), so the pair also has infinite order.

For example, in $C_4\times C_6$, the additive element $(2,3)$ has component orders $2,2$, hence pair order $2$. The element $(1,1)$ instead has order $\operatorname{lcm}(4,6)=12$. The product has $24$ elements, so even this latter element does not generate it. This distinguishes [group order](group.md#order-of-a-finite-group) from [order of a group element](#order-of-a-group-element) while exposing the simultaneous-return interpretation.

### Restricted direct sum of groups

↑ **Parent:** [Direct product of groups](#direct-product-of-groups)

The restricted direct sum of a family of [groups](group.md) $G_i$ is the subgroup of their [direct product of groups](#direct-product-of-groups) consisting of tuples with only finitely many nonidentity coordinates. Multiplication is coordinatewise. If every factor is a [finite group](group.md#finite-group), each [subgroup](group.md#subgroup) that is a [finitely generated group](group.md#finitely-generated-group) lies in a finite subproduct, so the restricted direct sum is a [locally finite group](#locally-finite-group). This gives concrete infinite [torsion groups](#torsion-group) without a uniform bound on element orders.

### Internal direct product theorem

↑ **Parent:** [Direct product of groups](#direct-product-of-groups)

An internal direct product finds independent coordinates already present inside a [group](group.md). Let $H,K$ be [normal subgroups](#normal-subgroup) of $G$ with

$$
H\cap K=\{e\},\qquad HK=G.
$$

Then the multiplication map

$$
\Phi:H\times K\longrightarrow G,\qquad \Phi(h,k)=hk
$$

is a [group isomorphism](algebra.md#group-isomorphism). Thus every element of $G$ has a unique factorization into one element of each subgroup. Conversely, the embedded factors $G\times\{e_H\}$ and $\{e_G\}\times H$ inside an external [direct product of groups](#direct-product-of-groups) satisfy these conditions.

For a concrete example, take the additive [cyclic group](group.md#cyclic-group) $C_6=\mathbb Z/6\mathbb Z$ and its [subgroups](group.md#subgroup) $H=\{0,3\}$ and $K=\{0,2,4\}$. They are [normal subgroups](#normal-subgroup) because $C_6$ is an [abelian group](group.md#abelian-group). Their intersection is $\{0\}$, and the sums $h+k$ give every [residue class](modular-arithmetic.md#residue-class) exactly once. For instance, $1=3+4\bmod6$. The table makes the unique decomposition visible.

<a id="image-each-element-of-c6-has-one-decomposition-as-an-element-of-the-subgroup-0-3-plus-one-of-0-2-4"></a>
![](internal-direct-product-c6-decomposition.png)

**[Figure 2](#image-each-element-of-c6-has-one-decomposition-as-an-element-of-the-subgroup-0-3-plus-one-of-0-2-4). Each element of C6 has one decomposition as an element of the subgroup $\{0,3\}$ plus one of $\{0,2,4\}$**.

The proof explains each hypothesis. Normality puts the [group commutator](group.md#group-commutator) $[h,k]=h^{-1}k^{-1}hk$ in both $H$ and $K$, so it is the [identity element](algebraic-operation.md#identity-element). Therefore the factors [commute](algebraic-operation.md#commuting-elements), and $\Phi$ preserves the [group operation](group.md#group-operation). The condition $HK=G$ makes it [surjective](algebra.md#surjective-function). If $hk=e$, then $h=k^{-1}$ belongs to the intersection, forcing both to be the [identity element](algebraic-operation.md#identity-element); thus its [group kernel](#kernel-of-a-group-homomorphism) is trivial and it is [injective](algebra.md#injective-function).

Normality cannot simply be omitted. In the [symmetric group](finite-group-theory.md#symmetric-group) $S_3$, take $H=\langle(123)\rangle$ and $K=\langle(12)\rangle$. Their intersection is trivial and $HK=S_3$, but $K$ is not a [normal subgroup](#normal-subgroup). With [permutations](combinatorics.md#permutation) composed right to left, $(123)(12)=(13)$ while $(12)(123)=(23)$, so the factors do not [commute](algebraic-operation.md#commuting-elements). The setwise decomposition is unique, but its multiplication map is not a [group homomorphism](#group-homomorphism) from $H\times K$. An independent-coordinate interpretation requires the group operations to agree, not merely a bijection of the underlying sets.

## Metacyclic group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Metacyclic_group)

A group is metacyclic when it has a cyclic normal subgroup whose quotient is cyclic. Every [dihedral group](finite-group-theory.md#dihedral-group) is metacyclic through its rotation subgroup.

## Commutator subgroup

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Commutator_subgroup)

The commutator subgroup of a [group](group.md) $G$ is the [subgroup](group.md#subgroup) generated by all its [group commutators](group.md#group-commutator):

$$
G'=[G,G]=\langle x^{-1}y^{-1}xy:x,y\in G\rangle.
$$

Here and throughout, $[x,y]=x^{-1}y^{-1}xy$. A [group commutator](group.md#group-commutator) is the [identity element](algebraic-operation.md#identity-element) precisely when $x$ and $y$ commute. The generated [subgroup](group.md#subgroup) includes finite products of [group commutators](group.md#group-commutator) and their [inverse elements](algebraic-operation.md#inverse-element); an element of $G'$ need not itself be a single [group commutator](group.md#group-commutator). Thus $G'=\{e\}$ precisely when $G$ is an [abelian group](group.md#abelian-group).

The useful idea is to record exactly what must disappear to make multiplication commutative. The identity $xy=yx[x,y]$ shows how a [group commutator](group.md#group-commutator) corrects a change in multiplication order. Setting every such correction equal to $e$ produces the [abelianization](#abelianization) $G/G'$, while preserving every piece of information that a [group homomorphism](#group-homomorphism) to an [abelian group](group.md#abelian-group) can detect. This connects a local comparison of two operations to a canonical [quotient group](#quotient-group) of the whole [group](group.md).

The commutator subgroup is a [characteristic subgroup](algebra.md#characteristic-subgroup), hence a [normal subgroup](#normal-subgroup): a [group automorphism](algebra.md#group-automorphism) $\alpha$ sends $[x,y]$ to $[\alpha(x),\alpha(y)]$. For any [normal subgroup](#normal-subgroup) $N$,

$$
G/N\text{ is abelian}\quad\Longleftrightarrow\quad G'\subseteq N.
$$

Indeed, the [group commutator](group.md#group-commutator) of $xN$ and $yN$ is $[x,y]N$. This makes $G'$ the smallest [normal subgroup](#normal-subgroup) whose [quotient group](#quotient-group) is an [abelian group](group.md#abelian-group). See [Conrad, Subgroup series I, section 4: commutators and abelian quotients](https://kconrad.math.uconn.edu/blurbs/grouptheory/subgpseries1.pdf).

### Commutator subgroup of the symmetric group on three letters

↑ **Parent:** [Commutator subgroup](#commutator-subgroup)

For the [symmetric group](finite-group-theory.md#symmetric-group) $S_3$, take the [transpositions](combinatorics.md#transposition-permutation) $x=(12)$ and $y=(23)$. Products of [permutations](combinatorics.md#permutation) apply the rightmost factor first. Then

$$
xy=(123),\qquad yx=(132),\qquad [x,y]=(12)(23)(12)(23)=(132).
$$

The last [permutation](combinatorics.md#permutation) sends $1\mapsto3$, $3\mapsto2$, and $2\mapsto1$: two swaps fail to commute by an entire three-cycle.

<a id="image-group-commutators-and-the-information-surviving-abelianization-in-the-symmetric-group-s-3"></a>
![](s3-commutator-and-abelianization.png)

**[Figure 3](#image-group-commutators-and-the-information-surviving-abelianization-in-the-symmetric-group-s-3). Group commutators and the information surviving abelianization in the symmetric group $S_3$**. The upper rows group the six [permutations](combinatorics.md#permutation) by [sign of a permutation](finite-group-theory.md#sign-of-a-permutation). Each triangle labels the original vertices in their new positions. The lower row applies $y,x,y^{-1},x^{-1}$ successively, giving $[x,y]=(132)$ under the rightmost-first convention. The [commutator subgroup](#commutator-subgroup) consists of the three [even permutations](finite-group-theory.md#even-permutation); the [center of a group](#center-of-a-group) here contains only $e$.

Every [group commutator](group.md#group-commutator) has [sign of a permutation](finite-group-theory.md#sign-of-a-permutation) $+1$, so $S_3'\subseteq A_3$, the [alternating group](finite-group-theory.md#alternating-group) of [even permutations](finite-group-theory.md#even-permutation). Conversely, the displayed [group commutator](group.md#group-commutator) generates $A_3=\{e,(123),(132)\}$. Therefore $S_3'=A_3$. The two [cosets](#coset) are the [even permutations](finite-group-theory.md#even-permutation) and the [odd permutations](finite-group-theory.md#odd-permutation), and their multiplication is just multiplication of signs:

$$
S_3^{\mathrm{ab}}=S_3/A_3\cong\{+1,-1\}\cong C_2.
$$

This is the [first isomorphism theorem](#first-isomorphism-theorem) applied to the [sign of a permutation](finite-group-theory.md#sign-of-a-permutation). Once [commutativity](algebraic-operation.md#commutativity) is forced, all three [transpositions](combinatorics.md#transposition-permutation) become indistinguishable, and both three-cycles become the [identity element](algebraic-operation.md#identity-element). The surviving information is exactly whether the [permutation](combinatorics.md#permutation) is even or odd. Compare the very different [center of a group](#center-of-a-group) $Z(S_3)=\{e\}$.

### Perfect group

↑ **Parent:** [Commutator subgroup](#commutator-subgroup)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perfect_group)

A group $G$ is perfect when $G'=G$, equivalently when its [abelianization](#abelianization) is trivial.

#### Perfectness of the special linear group

↑ **Parent:** [Perfect group](#perfect-group)

For dimension at least three, $[I+aE_{ik},I+E_{kj}]=I+aE_{ij}$ for distinct $i,j,k$, with $[x,y]=x^{-1}y^{-1}xy$. In dimension two over a field with more than three elements, choose $s$ with $s^2\ne1$ and commute an elementary matrix with $\operatorname{diag}(s,s^{-1})$. In both cases all generating [transvections](vector-space.md#transvection) lie in the [commutator subgroup](#commutator-subgroup), so the [special linear group over a finite field](finite-group-theory.md#special-linear-group-over-a-finite-field) is perfect outside $\operatorname{SL}_2(\mathbb F_2)$ and $\operatorname{SL}_2(\mathbb F_3)$.

// Target: algebra.bigb

### Abelianization

↑ **Parent:** [Commutator subgroup](#commutator-subgroup)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abelianization)

The abelianization of a [group](group.md) $G$ is the [quotient group](#quotient-group)

$$
G^{\mathrm{ab}}=G/G',\qquad q:G\longrightarrow G^{\mathrm{ab}},\quad q(g)=gG',
$$

where $G'$ is the [commutator subgroup](#commutator-subgroup). Its elements are [cosets](#coset), and its operation is $(gG')(hG')=ghG'$. The result is an [abelian group](group.md#abelian-group): the two products $gh$ and $hg$ differ by a [group commutator](group.md#group-commutator), which disappears in the [quotient group](#quotient-group).

For the [symmetric group](finite-group-theory.md#symmetric-group) $S_3$, the [sign of a permutation](finite-group-theory.md#sign-of-a-permutation) realizes $S_3^{\mathrm{ab}}\cong C_2$, as shown in [commutator subgroup of the symmetric group on three letters](#commutator-subgroup-of-the-symmetric-group-on-three-letters). For the [dihedral group](finite-group-theory.md#dihedral-group) of a [square](euclidean-geometry.md#square), [abelianization of the square symmetry group](#abelianization-of-the-square-symmetry-group) gives $C_2\times C_2$: two independent yes-or-no pieces of information survive. An [abelian group](group.md#abelian-group) already has $G'=\{e\}$, so its [abelianization](#abelianization) is isomorphic to itself. At the other extreme, a [perfect group](#perfect-group) has trivial [abelianization](#abelianization).

Calling this the largest [abelian quotient](#abelian-quotient) means that every [group homomorphism](#group-homomorphism) into any [abelian group](group.md#abelian-group) factors uniquely through $q$. It does not require $G$ to be finite, or compare the sizes of unrelated [abelian groups](group.md#abelian-group). The [universal property of abelianization](#universal-property-of-abelianization) makes this precise. It lets us solve all such mapping problems in one simpler [group](group.md): any invariant that respects multiplication and takes values in an [abelian group](group.md#abelian-group) sees only $G^{\mathrm{ab}}$.

#### Universal property of abelianization

↑ **Parent:** [Abelianization](#abelianization)

For every [abelian group](group.md#abelian-group) $A$ and [group homomorphism](#group-homomorphism) $f:G\to A$, there is a unique [group homomorphism](#group-homomorphism) $\bar f:G^{\mathrm{ab}}\to A$ such that

$$
f=\bar f\circ q,\qquad \bar f(gG')=f(g).
$$

This is a [universal property](category-theory.md#universal-property). To see why it holds, compute $f([x,y])=[f(x),f(y)]=e_A$, using [commutativity](algebraic-operation.md#commutativity) in $A$. Hence $G'\subseteq\ker f$, and $f$ is constant on each [coset](#coset) of $G'$. The displayed formula is therefore well-defined and preserves multiplication. It is unique because $q$ is [surjective](algebra.md#surjective-function). This is an instance of factoring a [group homomorphism](#group-homomorphism) through a [quotient group](#quotient-group); see [Conrad, Universal mapping properties, theorem 3.4](https://kconrad.math.uconn.edu/blurbs/linmultialg/universalmapping.pdf).

In particular, every [abelian quotient](#abelian-quotient) $G/N$ comes from a [surjective group homomorphism](#surjective-group-homomorphism) $G^{\mathrm{ab}}\to G/N$, $gG'\mapsto gN$. For $S_3$, any [group homomorphism](#group-homomorphism) to an [abelian group](group.md#abelian-group) is determined by the common image $a$ of its three [transpositions](combinatorics.md#transposition-permutation), with $a^2=e_A$. Every [even permutation](finite-group-theory.md#even-permutation) must map to $e_A$. Thus [sign of a permutation](finite-group-theory.md#sign-of-a-permutation) captures all possible information of this kind, including maps with infinite [abelian groups](group.md#abelian-group) as their targets.

#### Uniqueness of finite-index subgroups forces infinite cyclic abelianization

↑ **Parent:** [Abelianization](#abelianization)

If a finitely generated group $S$ has exactly one subgroup of each finite index, every such subgroup is normal. The quotients of prime order give surjections of its finitely generated abelianization onto $C_p$ for all primes, forcing positive free rank. A free rank of at least two gives two distinct index-$p$ subgroups. Positive finite torsion together with the free rank-one factor also gives two index-$p$ subgroups for a suitable prime. Hence $S_{\mathrm{ab}}\cong\mathbb Z$.

// Target: algebra.bigb

##### Residually finite group with one subgroup of each finite index is infinite cyclic

↑ **Parent:** [Uniqueness of finite-index subgroups forces infinite cyclic abelianization](#uniqueness-of-finite-index-subgroups-forces-infinite-cyclic-abelianization)

The epimorphism $S\to S_{\mathrm{ab}}\cong\mathbb Z$ has preimage of $n\mathbb Z$ as the unique index-$n$ subgroup. Thus every finite-index subgroup contains the commutator subgroup. Residual finiteness makes their intersection trivial, forcing the commutator subgroup to vanish and $S\cong\mathbb Z$.

// Target: geometry-and-topology.bigb

#### Abelianization of the square symmetry group

↑ **Parent:** [Abelianization](#abelianization)

Let $D_8$ denote the [dihedral group](finite-group-theory.md#dihedral-group) of [group order](group.md#order-of-a-finite-group) eight acting on a [square](euclidean-geometry.md#square). Here the subscript specifies [group order](group.md#order-of-a-finite-group); the same [group](group.md) is called $D_4$ in the convention that counts [vertices of a polygon](euclidean-geometry.md#vertex-of-a-polygon), as in the [group action](group-action.md) example. Let $r$ be a counterclockwise quarter-turn [rotation](riemannian-geometry.md#rotation-mathematics) and $s$ a [reflection](linear-algebra.md#reflection-mathematics) in a diagonal. Then

$$
D_8=\{e,r,r^2,r^3,s,rs,r^2s,r^3s\},\qquad r^4=s^2=e,\quad srs=r^{-1}.
$$

Products act rightmost first. The [group commutator](group.md#group-commutator) of the [generators of a group](group.md#generator-of-a-group) is

$$
[r,s]=r^{-1}s^{-1}rs=r^{-1}(srs)=r^{-2}=r^2.
$$

It is a half-turn [rotation](riemannian-geometry.md#rotation-mathematics), so forcing $r$ and $s$ to commute must identify a half-turn with $e$.

<a id="image-the-eight-square-symmetries-become-four-elements-under-abelianization"></a>
![](square-group-abelianization.png)

**[Figure 4](#image-the-eight-square-symmetries-become-four-elements-under-abelianization). The eight square symmetries become four elements under abelianization**. Each column is a [coset](#coset) of the [commutator subgroup](#commutator-subgroup) $N=\{e,r^2\}$ in the [dihedral group](finite-group-theory.md#dihedral-group) of [group order](group.md#order-of-a-finite-group) eight. Vertex labels show where each original vertex goes. The map $r^is^j\mapsto(i\bmod2,j)$ retains quarter-turn [integer parity](integer.md#parity-mathematics) and the presence of a [reflection](linear-algebra.md#reflection-mathematics). The table adds the two bits separately modulo two, giving the [Klein four-group](finite-group-theory.md#klein-four-group) $C_2\times C_2$.

More concretely, write each element uniquely as $r^is^j$, with $0\leq i<4$ and $j\in\{0,1\}$. The [function](function.md)

$$
\phi:D_8\longrightarrow C_2\times C_2,\qquad \phi(r^is^j)=(i\bmod2,j)
$$

is a [surjective group homomorphism](#surjective-group-homomorphism). Indeed, $srs=r^{-1}$ gives

$$
(r^is^j)(r^ks^\ell)=r^{i+(-1)^jk}s^{j+\ell},
$$

where the exponents are reduced modulo four and two. Modulo two, $-k$ and $k$ agree, so $\phi$ adds the two coordinates separately. Its [group kernel](#kernel-of-a-group-homomorphism) is $N=\{e,r^2\}$. Since the target is an [abelian group](group.md#abelian-group), $D_8'\subseteq N$; since $[r,s]=r^2$, also $N\subseteq D_8'$. Thus

$$
D_8'=\{e,r^2\},\qquad D_8^{\mathrm{ab}}\cong C_2\times C_2.
$$

The four [cosets](#coset) are $\{e,r^2\}$, $\{r,r^3\}$, $\{s,r^2s\}$, and $\{rs,r^3s\}$. Each [coset](#coset) forgets the difference of a half-turn. The [quotient group](#quotient-group) still distinguishes [rotations](riemannian-geometry.md#rotation-mathematics) from [reflections](linear-algebra.md#reflection-mathematics), and even from odd numbers of quarter-turns; the two surviving choices are independent. This is the [Klein four-group](finite-group-theory.md#klein-four-group), rather than the [cyclic group](group.md#cyclic-group) $C_4$, because each nonidentity element squares to the [identity element](algebraic-operation.md#identity-element). For the general [dihedral group](finite-group-theory.md#dihedral-group) calculation, see [Conrad, Dihedral groups I, theorem A.1](https://kconrad.math.uconn.edu/blurbs/grouptheory/dihedral.pdf); that source uses the vertex-count convention and $xyx^{-1}y^{-1}$ for individual [group commutators](group.md#group-commutator).

#### Abelianization of an odd dihedral group

↑ **Parent:** [Abelianization](#abelianization)

For odd $n\geq3$, the [dihedral group](finite-group-theory.md#dihedral-group) $D_{2n}$ of order $2n$ has rotation generator $r$ and reflection generator $s$, with $srs=r^{-1}$. The [group commutator](group.md#group-commutator) $[r,s]=r^{-2}$ generates the rotation [subgroup](group.md#subgroup), while the quotient by that [subgroup](group.md#subgroup) is $C_2$. Hence the [commutator subgroup](#commutator-subgroup) is exactly $\langle r\rangle$ and the [abelianization](#abelianization) is $C_2$. The only [abelian quotients](#abelian-quotient) are $C_2$ and the trivial group.

## Center of a group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Center_(group_theory))

The center of a [group](group.md) consists of the elements that commute with every element of that [group](group.md):

$$
Z(G)=\{z\in G:zg=gz\text{ for every }g\in G\}=\bigcap_{g\in G}C_G(g),
$$

where $C_G(g)$ is the [centralizer](group-action.md#centralizer) of $g$. These are operations whose position in any product can be changed freely. The center is an [abelian group](group.md#abelian-group) and a [characteristic subgroup](algebra.md#characteristic-subgroup), hence a [normal subgroup](#normal-subgroup). A [group](group.md) is an [abelian group](group.md#abelian-group) precisely when $Z(G)=G$.

For the [symmetric group](finite-group-theory.md#symmetric-group) $S_3$, the [conjugacy classes](group-action.md#conjugacy-class) are

$$
\{e\},\qquad\{(12),(13),(23)\},\qquad\{(123),(132)\}.
$$

An element belongs to the center precisely when its [conjugacy class](group-action.md#conjugacy-class) has one element, so $Z(S_3)=\{e\}$. Yet [commutator subgroup of the symmetric group on three letters](#commutator-subgroup-of-the-symmetric-group-on-three-letters) gives $S_3'=A_3$, with three elements. Thus belonging to the [commutator subgroup](#commutator-subgroup) does not mean commuting with everything. The [alternating group](finite-group-theory.md#alternating-group) $A_3$ is an [abelian group](group.md#abelian-group) as a [subgroup](group.md#subgroup), but its nonidentity elements do not commute with the [transpositions](combinatorics.md#transposition-permutation) in the surrounding $S_3$.

For the [dihedral group](finite-group-theory.md#dihedral-group) $D_8$ of [group order](group.md#order-of-a-finite-group) eight in [abelianization of the square symmetry group](#abelianization-of-the-square-symmetry-group), the center is $\{e,r^2\}$. A [rotation](riemannian-geometry.md#rotation-mathematics) $r^i$ commutes with $s$ precisely when $r^i=r^{-i}$, which requires $i$ even. No [reflection](linear-algebra.md#reflection-mathematics) $r^is$ commutes with $r$, since $(r^is)r=r^{i-1}s$ whereas $r(r^is)=r^{i+1}s$. Consequently

$$
Z(D_8)=\{e,r^2\}=D_8'.
$$

The half-turn can be performed before or after any [square](euclidean-geometry.md#square) symmetry with the same result. Its appearance both here and in the [commutator subgroup](#commutator-subgroup) is a feature of this example, rather than a general equality. See [Conrad, Dihedral groups I, theorem 3.4 and example 3.5](https://kconrad.math.uconn.edu/blurbs/grouptheory/dihedral.pdf).

The center and the [commutator subgroup](#commutator-subgroup) answer different useful questions: which operations already commute with everything, and which operations must disappear for the entire [group](group.md) to commute. In an [abelian group](group.md#abelian-group) these answers are $Z(G)=G$ and $G'=\{e\}$. Another way to use the center is through [conjugation](group-action.md#conjugation): the [group homomorphism](#group-homomorphism) $g\mapsto(h\mapsto ghg^{-1})$ has [group kernel](#kernel-of-a-group-homomorphism) $Z(G)$, so the [first isomorphism theorem](#first-isomorphism-theorem) gives $G/Z(G)\cong\operatorname{Inn}(G)$, the [inner automorphism group](#inner-automorphism). The [quotient group](#quotient-group) by the center thus records the distinct conjugation operations; it need not be an [abelian quotient](#abelian-quotient).

A nontrivial finite [p-group](finite-group-theory.md#p-group) always has a nontrivial center. In the [class equation](group-action.md#class-equation), each noncentral [conjugacy class](group-action.md#conjugacy-class) has size divisible by $p$, so $|Z(G)|\equiv|G|\equiv0\pmod p$. The [identity element](algebraic-operation.md#identity-element) ensures $Z(G)$ is nonempty, hence it has at least $p$ elements. See [McKernan, MIT 18.703, lemmas 23.6–23.7 and definition-lemma 23.10](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/96221ce2d5b1077b3e5d3c5e08c88afe_MIT18_703S13_pra_l_23.pdf).

### Central element of a group

↑ **Parent:** [Center of a group](#center-of-a-group)

An element of a [group](group.md) is central when it commutes with every element of that [group](group.md). The set of all such elements is the [center of a group](#center-of-a-group). Equivalently, its [conjugacy class](group-action.md#conjugacy-class) is a singleton: $xgx^{-1}=g$ for every $x$ is exactly the commutation condition. This lets centrality identify one-element [conjugacy classes](group-action.md#conjugacy-class) without enumerating every [conjugation](group-action.md#conjugation).

### Cyclic quotient by the center

↑ **Parent:** [Center of a group](#center-of-a-group)

If $G/Z(G)$ is cyclic, then $G$ is abelian. Indeed, if $gZ(G)$ generates the quotient, every element is $g^az$ with $z\in Z(G)$, and any two such elements commute.

## Conjugate subgroup

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugate_subgroup)

For a [subgroup](group.md#subgroup) $H$ of a [group](group.md) $G$ and $g\in G$, the conjugate subgroup is the [conjugate subset](group-action.md#conjugate-subset)

$$
gHg^{-1}=\{ghg^{-1}:h\in H\}.
$$

It is a [subgroup](group.md#subgroup) because [conjugation](group-action.md#conjugation) is a [group automorphism](algebra.md#group-automorphism). Restricting that [group automorphism](algebra.md#group-automorphism) gives a [group isomorphism](algebra.md#group-isomorphism) from $H$ to $gHg^{-1}$, so conjugate [subgroups](group.md#subgroup) have the same [group order](group.md#order-of-a-finite-group). This describes the same operations after moving their reference configuration. Conjugacy of [subgroups](group.md#subgroup) is an [equivalence relation](set-theory.md#equivalence-relation). [Structure of Groups](mathematics-bibliography.md#abstract-algebra-second-edition-by-john-a-beachy-and-others/structure-of-groups)

For an [equilateral triangle](euclidean-geometry.md#equilateral-triangle) with [vertices of a polygon](euclidean-geometry.md#vertex-of-a-polygon) labeled $1,2,3$ counterclockwise, its [symmetry group](group-action.md#symmetry-group) is the [symmetric group](finite-group-theory.md#symmetric-group) $S_3$, also the [dihedral group](finite-group-theory.md#dihedral-group) of [group order](group.md#order-of-a-finite-group) six. Let $r=(123)$ be the counterclockwise [rotation](riemannian-geometry.md#rotation-mathematics) through $120$ degrees, and let $s=(12)$ be the [reflection](linear-algebra.md#reflection-mathematics) fixing [vertex of a polygon](euclidean-geometry.md#vertex-of-a-polygon) $3$. Products apply the rightmost [permutation](combinatorics.md#permutation) first. The [cyclic subgroup](group.md#cyclic-subgroup) $K=\langle s\rangle=\{e,(12)\}$ contains the [identity element](algebraic-operation.md#identity-element) and one [reflection](linear-algebra.md#reflection-mathematics). Relabeling a [transposition](combinatorics.md#transposition-permutation) by [conjugation](group-action.md#conjugation) gives

$$
r(12)r^{-1}=(r(1)\ r(2))=(23),\qquad r^2(12)r^{-2}=(13).
$$

Thus the [conjugation action](group-action.md#conjugation-action) moves $K$ among the three [subgroups](group.md#subgroup) $\langle(12)\rangle$, $\langle(23)\rangle$, and $\langle(13)\rangle$. Geometrically, the [rotation](riemannian-geometry.md#rotation-mathematics) moves the axis of the [reflection](linear-algebra.md#reflection-mathematics) to the next axis. Each [reflection](linear-algebra.md#reflection-mathematics) fixes a different [vertex of a polygon](euclidean-geometry.md#vertex-of-a-polygon), although [group isomorphisms](algebra.md#group-isomorphism) relate all three [subgroups](group.md#subgroup).

<a id="image-the-conjugation-action-of-a-triangle-rotation-cycles-three-reflection-subgroups"></a>
![](triangle-reflection-subgroup-conjugation-orbit.png)

**[Figure 5](#image-the-conjugation-action-of-a-triangle-rotation-cycles-three-reflection-subgroups). The conjugation action of a triangle rotation cycles three reflection subgroups**. Each arrow sends a [subgroup](group.md#subgroup) $L$ to $rLr^{-1}$, rather than multiplying its elements by $r$ on one side. The three-node [group orbit](group-action.md#orbit-group-theory) has [stabilizer subgroup](group-action.md#stabilizer-subgroup) $N_{S_3}(K)=K$. The [cyclic subgroup](group.md#cyclic-subgroup) $H=\langle r\rangle$ has a one-node [group orbit](group-action.md#orbit-group-theory) even though [reflection](linear-algebra.md#reflection-mathematics) [conjugation](group-action.md#conjugation) exchanges its two nonidentity elements.

The [normalizer](group-action.md#normalizer) tells when this change of reference leaves the [subgroup](group.md#subgroup) unchanged. For any [group](group.md) $G$ and [subgroup](group.md#subgroup) $H\leq G$, there is a [bijection](function.md#bijection)

$$
\{gN_G(H):g\in G\}\longrightarrow\{gHg^{-1}:g\in G\},\qquad gN_G(H)\longmapsto gHg^{-1}.
$$

Two choices $g,k$ give the same conjugate [subgroup](group.md#subgroup) exactly when $k^{-1}g\in N_G(H)$. Consequently the [index of a subgroup](group.md#index-of-a-subgroup) $[G:N_G(H)]$ counts the distinct conjugate [subgroups](group.md#subgroup), even for an infinite [group](group.md). For a [finite group](group.md#finite-group) the count is $|G|/|N_G(H)|$. These are [cosets](#coset); they need not form a [quotient group](#quotient-group), since $N_G(H)$ need not be a [normal subgroup](#normal-subgroup) of $G$. In the triangle example there are $6/2=3$ conjugate [subgroups](group.md#subgroup), while the [cyclic subgroup](group.md#cyclic-subgroup) $\langle r\rangle$ has only one. [Group Theory (v4.01) by James S. Milne](mathematics-bibliography.md#group-theory-v4-01-by-james-s-milne)

## Group action

↑ **Parent:** [Group theory](group-theory.md)

[This section is present in another page, follow this link to view it.](group-action.md)

## Coset

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coset)

For a [subgroup](group.md#subgroup) $H\leq G$ of a [group](group.md) $G$, a left [coset](#coset) is $gH=\{gh:h\in H\}$; a right [coset](#coset) is $Hg=\{hg:h\in H\}$. The name refers to the side on which the representative $g$ multiplies $H$. Think of a [coset](#coset) as a translated copy of a [subgroup](group.md#subgroup): it remembers the relative differences allowed by $H$, while moving the whole collection to another location in the [group](group.md).

Two left [cosets](#coset) of the same [subgroup](group.md#subgroup) are either equal or disjoint. Thus distinct left [cosets](#coset) form a [partition of a set](set.md#partition-of-a-set) covering $G$; the same statement holds separately for right [cosets](#coset). The useful membership test is

$$
aH=bH\quad\Longleftrightarrow\quad b^{-1}a\in H.
$$

This also defines an [equivalence relation](set-theory.md#equivalence-relation): changing a representative by right multiplication with a member of $H$ leaves its left [coset](#coset) unchanged. These facts hold even for infinite [groups](group.md). See [MIT's coset notes, definitions 3.6 and 3.9](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/df580757da0149c376f1fda29bf82a91_MIT18_703S13_pra_l_3.pdf).

For an explicit additive example, take the [cyclic group](group.md#cyclic-group) $G=\mathbb Z/6\mathbb Z$, with [modular arithmetic](modular-arithmetic.md), and the [subgroup](group.md#subgroup) $H=\{0,3\}$. Adding each representative to both members gives exactly

$$
0+H=\{0,3\},\qquad 1+H=\{1,4\},\qquad 2+H=\{2,5\}.
$$

Representatives $3,4,5$ repeat these three [cosets](#coset), respectively. For example, $4+H=\{4,1\}=1+H$, since $4-1=3\in H$. Every residue appears once in the displayed [partition of a set](set.md#partition-of-a-set). Each [coset](#coset) has two members, so the [group order](group.md#order-of-a-finite-group) of $H$ is $2$ and its [index of a subgroup](group.md#index-of-a-subgroup) is $3$. Left and right [cosets](#coset) coincide here because $G$ is an [abelian group](group.md#abelian-group).

<a id="image-three-cosets-of-the-order-two-subgroup-of-the-additive-cyclic-group-of-order-six"></a>
![](cyclic-coset-partition.png)

**[Figure 6](#image-three-cosets-of-the-order-two-subgroup-of-the-additive-cyclic-group-of-order-six). Three cosets of the order-two subgroup of the additive cyclic group of order six**.

A [coset](#coset) need not be a [subgroup](group.md#subgroup). In this example, $\{1,4\}$ lacks the [identity element](algebraic-operation.md#identity-element) $0$, and $1+1=2$ leaves it. In fact, the only left or right [coset](#coset) of $H$ that is a [subgroup](group.md#subgroup) is $H$ itself: a [subgroup](group.md#subgroup) must contain the [identity element](algebraic-operation.md#identity-element), and the [coset](#coset) containing that element is $H$. Equal sizes come instead from the [bijection](function.md#bijection) $h\mapsto gh$, whose inverse is $x\mapsto g^{-1}x$; for right [cosets](#coset), use $h\mapsto hg$ and $x\mapsto xg^{-1}$.

The [nonabelian group](group.md#non-abelian-group) $S_3$, the [symmetric group](finite-group-theory.md#symmetric-group) on three letters, separates the two sides. Use [function composition](function.md#function-composition) with the rightmost [permutation](combinatorics.md#permutation) applied first, and let $H=\{e,(12)\}$. Then $(13)(12)=(123)$ but $(12)(13)=(132)$, giving the differing pair

$$
(13)H=\{(13),(123)\},\qquad H(13)=\{(13),(132)\}.
$$

The complete [partition of a set](set.md#partition-of-a-set) into left [cosets](#coset) consists of $H$, $\{(13),(123)\}$ and $\{(23),(132)\}$; the complete [partition of a set](set.md#partition-of-a-set) into right [cosets](#coset) consists of $H$, $\{(13),(132)\}$ and $\{(23),(123)\}$. Each lists all six [permutations](combinatorics.md#permutation) exactly once. Both have three parts of size two, although their parts differ.

<a id="image-left-and-right-coset-partitions-in-s3-with-rightmost-first-permutation-composition"></a>
![](permutation-left-right-cosets.png)

**[Figure 7](#image-left-and-right-coset-partitions-in-s3-with-rightmost-first-permutation-composition). Left and right coset partitions in S3 with rightmost-first permutation composition**.

Left [cosets](#coset) support a [group action](group-action.md) by $a\cdot(gH)=(ag)H$ for every [subgroup](group.md#subgroup), as in the [coset action](group-action.md#coset-action). Multiplication of representatives defines a [quotient group](#quotient-group) operation $(aH)(bH)=(ab)H$ precisely when $H$ is a [normal subgroup](#normal-subgroup). Otherwise the answer can depend on the representatives: in this $S_3$ example, $e$ and $(12)$ represent the same [coset](#coset) $H$, yet $e(13)H=(13)H$ and $(12)(13)H=(23)H$ differ. In the additive example, $H$ is a [normal subgroup](#normal-subgroup), making $(1+H)+(2+H)=3+H=H$ valid. See [MIT's quotient-group notes, theorem 9.1](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/ecdbd211f736b3ac92379dea05b34491_MIT18_703S13_pra_l_9.pdf).

### Left coset

↑ **Parent:** [Coset](#coset)

For a [subgroup](group.md#subgroup) $H$ of a [group](group.md) $G$ and $g\in G$, its left coset is $gH=\{gh:h\in H\}$. Left multiplication $h\mapsto gh$ is a [bijection](function.md#bijection) from $H$ onto $gH$. Left and [right cosets](#right-coset) agree for every $g$ exactly when $H$ is a [normal subgroup](#normal-subgroup).

### Right coset

↑ **Parent:** [Coset](#coset)

For a [subgroup](group.md#subgroup) $H$ of a [group](group.md) $G$ and $g\in G$, its right coset is $Hg=\{hg:h\in H\}$. The map $h\mapsto hg$ is a [bijection](function.md#bijection) from $H$ onto $Hg$, with inverse $x\mapsto xg^{-1}$; in particular all right cosets have the same [cardinality](cardinal-number.md#cardinality) as $H$. Multiplication by subgroup elements is on the left in this expression because $g$ is the factor on the right.

### Right coset transversal

↑ **Parent:** [Coset](#coset)

A right coset transversal for a [subgroup](group.md#subgroup) $A\le G$ chooses one representative $r$ for each right coset $Ar$. Every $g\in G$ then has a unique expression $g=ar$ with $a\in A$ and $r$ in the transversal. Choosing $1$ as the representative of $A$ makes membership in $A$ equivalent to having representative $1$.

### Double coset

↑ **Parent:** [Coset](#coset)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Double_coset)

For subgroups $H,P\leq G$, the double coset of $x\in G$ is

$$
HxP=\{hxp:h\in H,\ p\in P\}.
$$

The double cosets partition $G$. The action of $H$ on the left cosets of $P$ gives

$$
\frac{|HxP|}{|P|}
=\frac{|H|}{|H\cap xPx^{-1}|}
$$

by the [orbit-stabilizer theorem](group-action.md#orbit-stabilizer-theorem).

#### Double-coset counts need not divide group order

↑ **Parent:** [Double coset](#double-coset)

For the order-eight [dihedral group](finite-group-theory.md#dihedral-group) generated by $r$ of order four and $s$ of order two with $srs=r^{-1}$, let $H=K=\langle s\rangle$. There are exactly three [double cosets](#double-coset): $H$, $Hr^2H$, and $HrH$, of sizes two, two, and four. Their number does not divide eight. This differs from the number of ordinary [cosets](#coset), which divides group order by [Lagrange's theorem](#lagrange-s-theorem).

#### Double-coset sizes not dividing group order

↑ **Parent:** [Double coset](#double-coset)

A [double coset](#double-coset) is generally not a [subgroup](group.md#subgroup), so [Lagrange's theorem](#lagrange-s-theorem) does not force its size to divide the ambient group order. In $S_3$, take $H=K=\langle(12)\rangle$. Then $HeH$ has size two, while $H(13)H$ has size four, which does not divide six. The general size formula $|HgK|=|H||K|/|H\cap gKg^{-1}|$ explains why different double cosets can have different sizes.

#### Double-coset Hecke algebra

↑ **Parent:** [Double coset](#double-coset)

For a [group](group.md) $G$ and subgroup $\Gamma$ such that every [double coset](#double-coset) has finitely many orbits under left multiplication by $\Gamma$, this algebra consists of complex $\Gamma$-bi-invariant [functions](function.md) on $G$ supported on finitely many [double cosets](#double-coset). Its convolution is

$$
(h_1*h_2)(g)=\sum_{\Gamma x\in\Gamma\backslash G}h_1(gx^{-1})h_2(x).
$$

The [double coset](#double-coset) indicator functions form a basis. On invariant modular [functions](function.md) it acts on the right by $f*h=\sum_{\Gamma x}h(x)f|_kx$. For $G=GL_2(\mathbb Q)^+$ and $\Gamma=SL_2(\mathbb Z)$, [rational conjugation of finite-index modular subgroups](modular-function.md#rational-conjugation-of-finite-index-modular-subgroups) verifies the finiteness condition. The determinant-$n$ [Hecke operator](modular-function.md#hecke-operator) uses the indicator of all integral determinant-$n$ [matrices](vector-space.md#matrix), not only a single [double coset](#double-coset) when $n$ is composite.

#### Sylow subgroup of a subgroup from double cosets

↑ **Parent:** [Double coset](#double-coset)

If $P$ is a [Sylow subgroup](finite-group-theory.md#sylow-subgroup) of a finite group $G$ and $H\leq G$, some intersection $H\cap xPx^{-1}$ is a Sylow subgroup of $H$. Otherwise every double-coset size

$$
|HxP|=\frac{|H||P|}{|H\cap xPx^{-1}|}
$$

would be divisible by a larger power of $p$ than $|G|$, as would their sum $|G|$.

<h2 id="lagrange-s-theorem">Lagrange's theorem</h2>

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lagrange's_theorem_(group_theory))

For a [finite group](group.md#finite-group) $G$ and a [subgroup](group.md#subgroup) $H$, the [group order](group.md#order-of-a-finite-group) of $H$ divides the [group order](group.md#order-of-a-finite-group) of $G$:

$$
|G|=[G:H]|H|.
$$

Here $[G:H]$ is the [index of a subgroup](group.md#index-of-a-subgroup), the number of distinct left [cosets](#coset). It is also the number of distinct right [cosets](#coset): inversion gives a [bijection](function.md#bijection) $gH\mapsto Hg^{-1}$ between the two collections. No [normal subgroup](#normal-subgroup) assumption is needed for [Lagrange's theorem](#lagrange-s-theorem). The [normal subgroup](#normal-subgroup) condition matters when constructing a [quotient group](#quotient-group), rather than when counting a [partition of a set](set.md#partition-of-a-set).

The beauty of [Lagrange's theorem](#lagrange-s-theorem) is that an arithmetic restriction follows from a structural picture. A [group](group.md) can be tiled by equal-sized [cosets](#coset) of any [subgroup](group.md#subgroup). To see the count, choose one representative from each left [coset](#coset). Every [group element](group.md#group-element) has exactly one expression $g_i h$ for these chosen representatives and $h\in H$: different rows do not overlap, and multiplication by $g_i$ is a [bijection](function.md#bijection) from $H$ to its row. Counting rows times row size gives the formula. See [MIT's symmetries notes, section 2](https://math.mit.edu/~djk/18.310/Lecture-Notes/symmetries_2007.html).

The additive [cyclic group](group.md#cyclic-group) $\mathbb Z/6\mathbb Z$ above gives $6=3\times2$ from $H=\{0,3\}$. Another [subgroup](group.md#subgroup), $K=\{0,2,4\}$, has [cosets](#coset) $K$ and $1+K=\{1,3,5\}$, giving $6=2\times3$. In $S_3$, the [subgroup](group.md#subgroup) $\{e,(12)\}$ also gives $6=3\times2$, despite its distinct left and right [coset](#coset) partitions. Thus equal row sizes persist in a [nonabelian group](group.md#non-abelian-group). A proposed [subgroup](group.md#subgroup) of size four in either [group](group.md) is impossible: four does not divide six. This filters possible [subgroups](group.md#subgroup) before any search for [group generators](group.md#generator-of-a-group).

Apply [Lagrange's theorem](#lagrange-s-theorem) to the [cyclic subgroup](group.md#cyclic-subgroup) generated by a [group element](group.md#group-element) $g$. Its size is the [order of a group element](#order-of-a-group-element), so $\operatorname{ord}(g)\mid|G|$ and $g^{|G|}=e$. In the additive example, $2$ has [order of a group element](#order-of-a-group-element) $3$, since $2+2+2=0$ modulo six; the corresponding multiplicative statement becomes $6\cdot2=0$. A [group](group.md) of [prime](prime-number.md) [group order](group.md#order-of-a-finite-group) is consequently a [cyclic group](group.md#cyclic-group): any nonidentity [group element](group.md#group-element) generates a [subgroup](group.md#subgroup) whose size is greater than one and divides that [prime](prime-number.md), forcing it to be the whole [group](group.md). See [MIT's cyclic-group notes](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/50c134275caf32dbf4430ab097185157_MIT18_703S13_pra_l_4.pdf). The same counting idea underlies the [orbit-stabilizer theorem](group-action.md#orbit-stabilizer-theorem): the [orbit of a group action](group-action.md#orbit-group-theory) is parametrized by [cosets](#coset) of its [stabilizer subgroup](group-action.md#stabilizer-subgroup).

Historically, [Lagrange's theorem](#lagrange-s-theorem) grew from investigations of [permutations](combinatorics.md#permutation) of [roots of a polynomial](polynomial.md#root-of-a-polynomial); see [St Andrews' account of Lagrange's early work](https://mathshistory.st-andrews.ac.uk/Biographies/Lagrange/). The modern statement about arbitrary [finite groups](group.md#finite-group) should not be read back into the early work. Carmichael's 1921 review explicitly cautioned against attributing the full result to Lagrange; see [Carmichael's historical note, reproduced by St Andrews](https://mathshistory.st-andrews.ac.uk/Extras/Carmichael_Hardy_1/). Finally, [Lagrange's theorem](#lagrange-s-theorem) supplies a necessary size condition; the [failure of the converse to Lagrange's theorem](#failure-of-the-converse-to-lagrange-s-theorem) below explains its limit.

<h3 id="failure-of-the-converse-to-lagrange-s-theorem">Failure of the converse to Lagrange's theorem</h3>

↑ **Parent:** [Lagrange's theorem](#lagrange-s-theorem)

Divisibility of a proposed subgroup order is necessary by [Lagrange's theorem](#lagrange-s-theorem) but is not sufficient in arbitrary [finite groups](group.md#finite-group). The [alternating group](finite-group-theory.md#alternating-group) $A_4$ has order $12$ and no [subgroup](group.md#subgroup) of order $6$. Such a subgroup would have index two, hence be a [normal subgroup](#normal-subgroup). The quotient would have order two, so every element of order three would map to its identity. But $A_4$ has eight distinct three-cycles, which together with the identity cannot fit in a subgroup of order six. This obstruction contrasts with [cyclic groups](group.md#cyclic-group), which have a subgroup of every divisor order.

## Group embedding

↑ **Parent:** [Group theory](group-theory.md)

A group embedding is an injective [group homomorphism](#group-homomorphism). It identifies its domain with an isomorphic subgroup of its codomain.

### Two-generator HNN embedding

↑ **Parent:** [Group embedding](#group-embedding)

For $G=\langle g_i\mid R\rangle$, put $B=G*F(a,b)$, $u_0=a$, $v_0=b$, $u_i=b^{-i}ab^i$ and $v_i=g_i a^{-i}ba^i$ for $i\ge1$. The $u_i$ freely generate by [free conjugate bases in a rank-two free group](geometric-group-theory.md#free-conjugate-bases-in-a-rank-two-free-group). The $v_i$ do too: projection killing $G$ maps them to a free conjugate basis, so no reduced word in them is trivial. The [HNN extension](geometric-group-theory.md#hnn-extension) adjoining $t^{-1}u_it=v_i$ embeds $G$ by [Britton's lemma](geometric-group-theory.md#britton-s-lemma). Since $b=t^{-1}at$ and $g_i=t^{-1}u_it(a^{-i}ba^i)^{-1}$, its generators reduce to $a,t$. For finitely many $g_i$ and $R$ this is a [finite group presentation](geometric-group-theory.md#finite-group-presentation); for effective countably many generators and enumerable $R$ it is a two-generator [recursive presentation of a group](geometric-group-theory.md#recursive-presentation-of-a-group).

### Alternating-group embedding of a finite group

↑ **Parent:** [Group embedding](#group-embedding)

[Cayley theorem](#cayley-s-theorem) embeds a [finite group](group.md#finite-group) of order $n$ into $S_n$. Extend $\sigma\in S_n$ to $n+2$ letters and multiply it by the disjoint [transposition](combinatorics.md#transposition-permutation) $(n+1\ n+2)$ exactly when $\sigma$ is odd. Additivity of parity makes this an injective [group homomorphism](#group-homomorphism) into the [alternating group](finite-group-theory.md#alternating-group) $A_{n+2}$. Thus every [finite group](group.md#finite-group) is isomorphic to a [subgroup](group.md#subgroup) of some [alternating group](finite-group-theory.md#alternating-group).

<h3 id="cayley-s-theorem">Cayley's theorem</h3>

↑ **Parent:** [Group embedding](#group-embedding)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cayley's_theorem)

Every [group](group.md) $G$ is [isomorphic](algebra.md#isomorphism) to a [subgroup](group.md#subgroup) of the [symmetric group](finite-group-theory.md#symmetric-group) on its underlying [set](set.md). The construction uses the [left regular action](group-action.md#left-regular-action): each [group element](group.md#group-element) $g$ becomes a [permutation](combinatorics.md#permutation) of all the [group elements](group.md#group-element), given by

$$
L_g:G\longrightarrow G,\qquad L_g(x)=gx,\qquad \lambda:G\hookrightarrow\operatorname{Sym}(G),\quad g\longmapsto L_g.
$$

For a [finite group](group.md#finite-group) of [group order](group.md#order-of-a-finite-group) $n$, labeling these elements by $1,\ldots,n$ gives a [group embedding](#group-embedding) into $S_n$. The same construction works for an [infinite group](group.md#infinite-group), with the [symmetric group](finite-group-theory.md#symmetric-group) of all [bijections](function.md#bijection) of its underlying [set](set.md).[Theorem 1.22 and Corollary 1.23, printed page 16: left multiplication embeds a group into its symmetric group](mathematics-bibliography.md#group-theory-v4-01-by-james-s-milne)

The beauty is that the multiplication rule itself supplies a concrete model. Whatever the [group elements](group.md#group-element) originally represent, each one rearranges the entire [group](group.md) by multiplication. A product becomes [function composition](function.md#function-composition), and no distinctions between [group elements](group.md#group-element) are lost. For a [finite group](group.md#finite-group), a row of its [Cayley table](algebraic-operation.md#cayley-table) lists the images under one $L_g$: the multiplication table is already a catalogue of [permutations](combinatorics.md#permutation).

Throughout this construction, products of [permutations](combinatorics.md#permutation) act rightmost first:

$$
(\sigma\tau)(x)=(\sigma\circ\tau)(x)=\sigma(\tau(x)),\qquad L_gL_h=L_{gh}.
$$

Thus $L_gL_h$ first multiplies by $h$, then by $g$. This is a left [group action](group-action.md), not a license to reverse the multiplication order in a [nonabelian group](group.md#non-abelian-group). Ordinary right multiplication $R_g(x)=xg$ instead satisfies $R_gR_h=R_{hg}$ with this convention; replacing it by $x\mapsto xg^{-1}$ restores the [group homomorphism](#group-homomorphism) law.[Example 2.10, printed page 7: left multiplication and the reversed composition law for right multiplication](mathematics-bibliography.md#group-actions-by-keith-conrad)

For an explicit [cyclic group](group.md#cyclic-group) example, take $C_4=\mathbb Z/4\mathbb Z$ under addition, using [modular arithmetic](modular-arithmetic.md). Its [left regular action](group-action.md#left-regular-action) consists of $L_k(x)=k+x\pmod4$. In [permutation cycles](finite-group-theory.md#permutation-cycle) on the labels $0,1,2,3$,

$$
L_0=\operatorname{id},\qquad L_1=(0\ 1\ 2\ 3),\qquad L_2=(0\ 2)(1\ 3),\qquad L_3=(0\ 3\ 2\ 1).
$$

The [function composition](function.md#function-composition) $L_1L_1=L_2$ sends $0$ to $2$, $1$ to $3$, $2$ to $0$, and $3$ to $1$: squaring the four-point [permutation cycle](finite-group-theory.md#permutation-cycle) produces two [disjoint permutation cycles](finite-group-theory.md#disjoint-permutation-cycles). Also $L_1L_3=L_0$. These four [permutations](combinatorics.md#permutation) form a [cyclic subgroup](group.md#cyclic-subgroup) of $S_4$, reproducing addition in $C_4$ exactly.

For a [nonabelian group](group.md#non-abelian-group) example, let $G=S_3$, with $r=(123)$, $s=(12)$, and $e$ its [identity element](algebraic-operation.md#identity-element). The six [group elements](group.md#group-element) are $e,r,r^2,s,rs,r^2s$, where $r^3=s^2=e$ and $sr=r^2s$. Now the labels being permuted are themselves [permutations](combinatorics.md#permutation) of three points. Computing the [left regular action](group-action.md#left-regular-action) gives [permutations](combinatorics.md#permutation) of these six labels:

$$
L_r=(e\ r\ r^2)(s\ rs\ r^2s),\qquad L_s=(e\ s)(r\ r^2s)(r^2\ rs).
$$

For example, $L_s(r)=sr=r^2s$; putting $rs$ here would accidentally switch to right multiplication. Noncommutativity survives in the model:

$$
(L_rL_s)(e)=rs=(13),\qquad (L_sL_r)(e)=sr=(23).
$$

These different outputs prove that $L_rL_s\ne L_sL_r$. The [group generators](group.md#generator-of-a-group) $r,s$ become [group generators](group.md#generator-of-a-group) $L_r,L_s$ of a six-element [subgroup](group.md#subgroup) of $S_6$.

<a id="cayley-left-translation-cycles"></a>
![](cayley-left-translation-cycles.png)

**[Figure 8](#cayley-left-translation-cycles). Left regular action as permutation cycles for $C_4$ and $S_3$**. Each arrow sends a label $x$ to $gx$, or to $k+x$ in the additive [cyclic group](group.md#cyclic-group). The top panels show the translations by $1$ and $2$ in $C_4$; the bottom panels show multiplication by $r$ and $s$ in the [symmetric group](finite-group-theory.md#symmetric-group) $S_3$. Each panel depicts one [permutation](combinatorics.md#permutation), decomposed into [disjoint permutation cycles](finite-group-theory.md#disjoint-permutation-cycles).

Why does a [group action](group-action.md) here produce a [group embedding](#group-embedding)? Any [group action](group-action.md) on a [set](set.md) $X$ gives a [group homomorphism](#group-homomorphism) $\rho:G\to\operatorname{Sym}(X)$; it is a [group embedding](#group-embedding) precisely when it is a [faithful group action](group-action.md#faithful-group-action). The [group kernel](#kernel-of-a-group-homomorphism) consists of the [group elements](group.md#group-element) fixing every point of $X$. In the [left regular action](group-action.md#left-regular-action), $L_g(e)=g$, so fixing the [identity element](algebraic-operation.md#identity-element) already forces $g=e$. In fact every [stabilizer subgroup](group-action.md#stabilizer-subgroup) is trivial, since $gx=x$ forces $g=e$; this stronger property makes the [left regular action](group-action.md#left-regular-action) a [regular group action](group-action.md#regular-group-action).[Theorem 1.2, printed pages 1-2: injectivity by evaluating at the identity; Theorem 1.7 and following paragraph, printed page 3: actions as homomorphisms and their kernels](mathematics-bibliography.md#group-actions-by-keith-conrad)

Compare two [group actions](group-action.md) of the same [cyclic group](group.md#cyclic-group) $C_4$. Its [left regular action](group-action.md#left-regular-action) on four labels distinguishes all four [group elements](group.md#group-element). On $X=\{0,1\}$, the rule $k\cdot x=k+x\pmod2$ defines a [transitive group action](group-action.md#transitive-group-action), but $0$ and $2$ both fix both points, while $1$ and $3$ both exchange them. Its [group kernel](#kernel-of-a-group-homomorphism) is $\{0,2\}$, so it is not a [faithful group action](group-action.md#faithful-group-action). Its image is a two-element [subgroup](group.md#subgroup) of $S_2$, [isomorphic](algebra.md#isomorphism) to the [quotient group](#quotient-group) $C_4/\{0,2\}$ rather than to $C_4$.

<a id="cayley-faithful-and-nonfaithful-actions"></a>
![](cayley-faithful-and-nonfaithful-actions.png)

**[Figure 9](#cayley-faithful-and-nonfaithful-actions). A faithful group action preserves all four translations; a two-point group action merges them**. Both panels start with the same [cyclic group](group.md#cyclic-group) $C_4$. The arrows show the [group action](group-action.md) of its [group generator](group.md#generator-of-a-group) $1$, and the tables show all four resulting [permutations](combinatorics.md#permutation). On four points the [group kernel](#kernel-of-a-group-homomorphism) is $\{0\}$; on two points it is $\{0,2\}$. Reachability of every point does not imply a [faithful group action](group-action.md#faithful-group-action).

The guaranteed number $|G|$ of labels need not be the smallest possible for a [faithful group action](group-action.md#faithful-group-action). The [symmetric group](finite-group-theory.md#symmetric-group) $S_3$ naturally acts faithfully on $\{1,2,3\}$: a [permutation](combinatorics.md#permutation) fixing all three labels is the [identity element](algebraic-operation.md#identity-element). Its [left regular action](group-action.md#left-regular-action) uses six labels instead. Three is the smallest possible here, since $S_1$ and $S_2$ have fewer than six elements and cannot contain an [isomorphic](algebra.md#isomorphism) copy of $S_3$. Moreover, in the natural three-point [group action](group-action.md), the [stabilizer subgroup](group-action.md#stabilizer-subgroup) of $1$ is $\{e,(23)\}$: a [faithful group action](group-action.md#faithful-group-action) can have nontrivial point [stabilizer subgroups](group-action.md#stabilizer-subgroup). Cayley's construction supplies a universal model, while a smaller model can reveal particular [symmetries](physics.md#symmetry-physics).

The proof is short. Each $L_g$ is a [bijection](function.md#bijection) with inverse $L_{g^{-1}}$. [Associativity](algebraic-operation.md#associative-property) gives

$$
L_g(L_h(x))=g(hx)=(gh)x=L_{gh}(x),
$$

so $\lambda$ is a [group homomorphism](#group-homomorphism). If $L_g=L_h$, evaluating both at the [identity element](algebraic-operation.md#identity-element) gives $g=L_g(e)=L_h(e)=h$. Hence $\lambda$ is [injective](algebra.md#injective-function), and its image is the required [isomorphic](algebra.md#isomorphism) [subgroup](group.md#subgroup). No finiteness assumption entered the argument.

The historical connection is unusually close to the notation. The opening paragraph of [Arthur Cayley](mathematics-author.md#arthur-cayley)'s 1854 paper already treats [permutations](combinatorics.md#permutation) as one example of operations on a collection of quantities and explicitly performs the rightmost operation first in a product. It also allows noncommutativity while insisting on [associativity](algebraic-operation.md#associative-property). The modern [left regular action](group-action.md#left-regular-action) shows how that viewpoint reaches every abstract [group](group.md), by choosing the [group](group.md) itself as the [set](set.md) to be acted on.[Abstract awakenings in algebra: Early group theory in the works of Lagrange, Cauchy, and Cayley by Janet Heine Barnett, Section 3.1, printed page 50: reproduced opening paragraph of Arthur Cayley's On the theory of groups, as depending on the symbolic equation theta^n = 1; reference 5, printed page 91: original publication in 1854](mathematics-bibliography.md#abstract-awakenings-in-algebra-early-group-theory-in-the-works-of-lagrange-cauchy-and-cayley-by-janet-heine-barnett)

#### Symmetric-group embedding at one less than the group order

↑ **Parent:** [Cayley's theorem](#cayley-s-theorem)

For $n>1$, a cyclic group of prime-power order $n$ cannot embed in $S_{n-1}$, because a permutation of order $p^k$ requires a cycle of length at least $p^k$. If $n$ is not a prime power, every group of order $n$ embeds in $S_{n-1}$ by combining coset actions on subgroups of two distinct prime orders.

## Generalized dihedral group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_dihedral_group)

For an abelian group $A$, the generalized dihedral group is the semidirect product $A\rtimes C_2$ in which the nonidentity element of $C_2$ acts on $A$ by inversion.

### Two-involution characterization of a dihedral group

↑ **Parent:** [Generalized dihedral group](#generalized-dihedral-group)

A [group](group.md) generated by two [involutions](#involution) is dihedral in the extended convention allowing $C_2$ and the [infinite dihedral group](representation-theory.md#infinite-dihedral-group). If $a\ne b$, put $x=ab$, $y=b$; then $yxy^{-1}=x^{-1}$. Conversely, from the inversion relation, $y$ and $xy$ square to the identity and generate. If $xy=e$, the group is $C_2$ and the same nonidentity element is used twice. Exact order two, rather than merely a square equal to the identity, requires this exceptional case. This convention extends the usual finite [dihedral group](finite-group-theory.md#dihedral-group) definition.

#### Nontrivial-quotient closure of two-involution groups

↑ **Parent:** [Two-involution characterization of a dihedral group](#two-involution-characterization-of-a-dihedral-group)

Every nontrivial [quotient group](#quotient-group) of a [group](group.md) generated by two [involutions](#involution) is generated by two [involutions](#involution), allowing repeated generators. The two generator images have squares equal to the identity. If one image becomes trivial, the other generates $C_2$; if both become trivial, the quotient is trivial and is excluded. Thus the [two-involution characterization of a dihedral group](#two-involution-characterization-of-a-dihedral-group) is preserved by nontrivial quotients.

## Order of a group element

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Order_of_a_group_element)

The order of a group element $g$ is the least positive integer $n$ for which $g^n$ is the identity. If no such integer exists, $g$ has infinite order.

### An element and its inverse have the same order

↑ **Parent:** [Order of a group element](#order-of-a-group-element)

For every positive integer $m$, $(g^{-1})^m=(g^m)^{-1}$, hence $g^m=e$ if and only if $(g^{-1})^m=e$. The sets of positive powers returning to the [identity element](algebraic-operation.md#identity-element) are therefore equal. Taking the least positive exponent therefore gives the same finite [order of a group element](#order-of-a-group-element) for $g$ and $g^{-1}$; if the sets are empty, both elements have infinite order. Equivalently, $g$ and $g^{-1}$ generate the same [cyclic subgroup](group.md#cyclic-subgroup).

### Conjugation preserves element order

↑ **Parent:** [Order of a group element](#order-of-a-group-element)

For every positive integer $n$, cancellation gives $(hah^{-1})^n=ha^nh^{-1}$. Thus the power on one side is the [identity element](algebraic-operation.md#identity-element) exactly when $a^n=e$, proving preservation of the [order of a group element](#order-of-a-group-element), including infinite order. In particular, $ab$ and $ba$ are conjugate because $a^{-1}(ab)a=ba$, and hence have the same order.

### Product of commuting elements of coprime order

↑ **Parent:** [Order of a group element](#order-of-a-group-element)

Let commuting elements $a,b$ have finite coprime orders $m,n$. Their [cyclic subgroups](group.md#cyclic-subgroup) have trivial intersection by [Lagrange's theorem](#lagrange-s-theorem). If $(ab)^k=1$, then $a^k=b^{-k}$ belongs to this intersection, so $m\mid k$ and $n\mid k$. Thus $mn\mid k$. Conversely, $(ab)^{mn}=1$ because the elements commute. This proves the displayed order formula.

### Infinite order

↑ **Parent:** [Order of a group element](#order-of-a-group-element)

A group element has infinite order when no positive power of it is the [identity element](algebraic-operation.md#identity-element).

### Involution

↑ **Parent:** [Order of a group element](#order-of-a-group-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Involution)

An involution is a group element $s$ satisfying $s^2=1$. Some conventions require $s\ne1$.

#### Eigenspace decomposition of a linear involution

↑ **Parent:** [Involution](#involution)

Let $F$ be a [linear map](vector-space.md#linear-map) on a [vector space](vector-space.md) over a field of characteristic different from two, with $F^2=I$. Then

$$
V=\ker(F-I)\oplus\ker(F+I),\qquad
P_\pm=\tfrac12(I\pm F).
$$

The projections satisfy $P_+P_-=0$ and $P_++P_-=I$, giving existence and uniqueness of the decomposition. In characteristic two, the two signs coincide and the conclusion need not hold.

##### Involution exponential formula

↑ **Parent:** [Eigenspace decomposition of a linear involution](#eigenspace-decomposition-of-a-linear-involution)

For a linear operator with $A^2=I$, every even power is $I$ and every odd power is $A$. Separating the absolutely convergent [matrix exponential](linear-operator-theory.md#matrix-exponential) series into those powers proves the displayed identity without a Hermiticity assumption. If $A$ is also a [Hermitian operator](hilbert-space.md#hermitian-operator), the exponential is a [unitary operator](vector-space.md#unitary-operator).

## Quotient group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quotient_group)

For a [group](group.md) $G$ and a [normal subgroup](#normal-subgroup) $N$, the [quotient group](#quotient-group) $G/N$ is the [set](set.md) of [cosets](#coset) $gN$, with operation

$$
(gN)(hN)=(gh)N.
$$

Its [identity element](algebraic-operation.md#identity-element) is the [coset](#coset) $N$, and the [inverse element](algebraic-operation.md#inverse-element) of $gN$ is $g^{-1}N$. A [quotient group](#quotient-group) treats all elements within one [coset](#coset) as the same input while retaining a consistent operation on the classes. The [normal subgroup](#normal-subgroup) condition is what makes this operation independent of which representatives are chosen. [McKernan, MIT 18.703, Theorem 9.1: quotient-group construction](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/ecdbd211f736b3ac92379dea05b34491_MIT18_703S13_pra_l_9.pdf).

Take the additive [group](group.md) $G=\mathbb Z/6\mathbb Z$ and $N=\{0,3\}$. Since $G$ is an [abelian group](group.md#abelian-group), $N$ is a [normal subgroup](#normal-subgroup). There are three elements in the [quotient group](#quotient-group):

$$
N=\{0,3\},\qquad 1+N=\{1,4\},\qquad 2+N=\{2,5\}.
$$

Adding two copies of $2+N$ gives $4+N=1+N$; adding $1+N$ and $2+N$ gives $3+N=N$. Hence the [quotient group](#quotient-group) has the addition table of $\mathbb Z/3\mathbb Z$. It does not select one representative and discard the others: its elements are the entire [cosets](#coset).

<a id="image-identifying-residues-differing-by-three-turns-a-six-element-cyclic-group-into-a-three-element-quotient-group"></a>
![](quotient-group-mod-six.png)

**[Figure 10](#image-identifying-residues-differing-by-three-turns-a-six-element-cyclic-group-into-a-three-element-quotient-group). Identifying residues differing by three turns a six-element cyclic group into a three-element quotient group**.

This is useful whenever distinctions within a [normal subgroup](#normal-subgroup) should be ignored. For example, the [sign of a permutation](finite-group-theory.md#sign-of-a-permutation) retains only even or odd parity of a [permutation](combinatorics.md#permutation) in $S_3$. Its [group kernel](#kernel-of-a-group-homomorphism) is the [alternating group](finite-group-theory.md#alternating-group) $A_3$, and the [quotient group](#quotient-group) $S_3/A_3$ has two elements. The [first isomorphism theorem](#first-isomorphism-theorem) explains why a [group homomorphism](#group-homomorphism)'s image is a [quotient group](#quotient-group) of its domain.

### Quotient map of groups

↑ **Parent:** [Quotient group](#quotient-group)

The [quotient map of groups](#quotient-map-of-groups) sends each [group element](group.md#group-element) to its [coset](#coset) modulo a [normal subgroup](#normal-subgroup). It is a [surjective group homomorphism](#surjective-group-homomorphism), with [group kernel](#kernel-of-a-group-homomorphism) exactly $N$. In the additive six-element example, it sends $0,3$ to $N$, $1,4$ to $1+N$, and $2,5$ to $2+N$. The [quotient map of groups](#quotient-map-of-groups) records the identification that produces the new [group](group.md).

### Coset multiplication is well-defined exactly for normal subgroups

↑ **Parent:** [Quotient group](#quotient-group)

If $N$ is a [normal subgroup](#normal-subgroup), changing representatives to $gn$ and $hm$, where $n,m\in N$, gives

$$
(gn)(hm)=gh(h^{-1}nh)m\in ghN.
$$

The chosen representatives therefore give the same [coset](#coset). Conversely, suppose the rule defines an operation on left [cosets](#coset). Since $nN=N$ for $n\in N$, multiplying by $gN$ gives $ngN=gN$, hence $g^{-1}ng\in N$. Applying this inclusion for every $g$ and $g^{-1}$ proves $g^{-1}Ng=N$, so $N$ is a [normal subgroup](#normal-subgroup). This makes normality exactly the condition needed to carry [group operation](group.md#group-operation) to these classes.

### Universal property of a quotient group

↑ **Parent:** [Quotient group](#quotient-group)

Let $N$ be a [normal subgroup](#normal-subgroup) of $G$, and let $\pi:G\to G/N$ be the [quotient map of groups](#quotient-map-of-groups). If a [group homomorphism](#group-homomorphism) $\varphi:G\to H$ has [group kernel](#kernel-of-a-group-homomorphism) containing $N$, there is exactly one [group homomorphism](#group-homomorphism) $\bar\varphi:G/N\to H$ with $\varphi=\bar\varphi\circ\pi$. Its value is forced: $\bar\varphi(gN)=\varphi(g)$. Every measurement by a [group homomorphism](#group-homomorphism) that ignores $N$ can thus be performed on the [quotient group](#quotient-group) directly. This is the [universal property](category-theory.md#universal-property) of the construction.

### Subgroup correspondence for a surjective group homomorphism

↑ **Parent:** [Quotient group](#quotient-group)

For a surjection $\theta:G\to H$ with kernel $K$, inverse image and image give inverse order-preserving bijections between subgroups of $H$ and subgroups of $G$ containing $K$. They preserve index. For an arbitrary subgroup $A$, $\theta^{-1}(\theta(A))=AK$, so $[H:\theta(A)]=[G:AK]$.

// Target: algebra.bigb

### Finite quotient of a group

↑ **Parent:** [Quotient group](#quotient-group)

A finite quotient is the image of a [group](group.md) under a surjective [group homomorphism](#group-homomorphism) to a [finite group](group.md#finite-group). A group has no nontrivial finite quotients exactly when every homomorphism from it to a finite group is trivial. This property does not prohibit finite or finite-quotient-bearing subgroups.

### Abelian quotient

↑ **Parent:** [Quotient group](#quotient-group)

An abelian quotient is a [quotient group](#quotient-group) $G/N$ that is an [abelian group](group.md#abelian-group). It exists only for a [normal subgroup](#normal-subgroup) $N$, and it is abelian exactly when $N$ contains the [commutator subgroup](#commutator-subgroup). Thus every abelian quotient factors through the [abelianization](#abelianization) $G/[G,G]$.

## General linear group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/General_linear_group)

The general linear group $GL(V)$ is the [group](group.md) of invertible [linear maps](vector-space.md#linear-map) from a [vector space](vector-space.md) $V$ to itself, with composition as its operation.

### Orientation-preserving general linear group

↑ **Parent:** [General linear group](#general-linear-group)

The real invertible matrices with positive [determinant](multilinear-algebra.md#determinant) form a [subgroup](group.md#subgroup) of the [general linear group](#general-linear-group). The identity has determinant one, [multiplicativity of the determinant](multilinear-algebra.md#multiplicativity-of-the-determinant) preserves positivity under products, and $\det(A^{-1})=1/\det A>0$ preserves it under inversion. More precisely this is the [kernel of a group homomorphism](#kernel-of-a-group-homomorphism) $A\mapsto\operatorname{sgn}(\det A)$ to $\{1,-1\}$, so it is a [normal subgroup](#normal-subgroup) of index two for $n\geq1$. Its elements preserve an [orientation of a vector space](multilinear-algebra.md#orientation-of-a-vector-space).

### Monomial matrix

↑ **Parent:** [General linear group](#general-linear-group)

A monomial [matrix](vector-space.md#matrix) has exactly one nonzero entry in each row and column. It factors as an invertible diagonal [matrix](vector-space.md#matrix) times a permutation [matrix](vector-space.md#matrix). Such [matrices](vector-space.md#matrix) permute the coordinate axes and normalize the group of invertible diagonal [matrices](vector-space.md#matrix); over very small fields that normalizer can be larger if the diagonal [subgroup](group.md#subgroup) fails to distinguish the axes.

### Integral general linear group

↑ **Parent:** [General linear group](#general-linear-group)

The integral general linear group consists of integer matrices with determinant $\pm1$. These are exactly the integer matrices whose inverses also have integer entries, so they are the automorphisms of the free abelian group $\mathbb Z^n$.

### Matrix group

↑ **Parent:** [General linear group](#general-linear-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_group)

A matrix group is a [group](group.md) represented by invertible matrices, equivalently a subgroup of a [general linear group](#general-linear-group).

#### Classical group

↑ **Parent:** [Matrix group](#matrix-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Classical_group)

A [classical group](#classical-group) is a standard family of linear groups, principally the general/special linear groups and groups preserving nondegenerate alternating, symmetric, Hermitian or quadratic forms. Finite-field versions yield many [finite simple groups](finite-group-theory.md#finite-simple-group) after imposing the appropriate determinant or derived-subgroup condition and quotienting the scalar [center of a group](#center-of-a-group). Small dimensions and small fields have exceptional isomorphisms and nonsimple cases.

#### Orthogonal group over a finite field

↑ **Parent:** [Matrix group](#matrix-group)

The [group](group.md) of invertible [linear maps](vector-space.md#linear-map) preserving a specified [quadratic form](quadratic-form.md) over a [finite field](algebra.md#finite-field). In characteristic two one must preserve the [quadratic form](quadratic-form.md) itself, not merely its polar [alternating bilinear form](bilinear-form.md#alternating-bilinear-form). For a nonsingular form, any two nonzero [isotropic vectors](quadratic-form.md#isotropic-vector) can be incorporated into hyperbolic pairs and standard adapted bases, producing an isometry between them.

## Special linear group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Special_linear_group)

### Real special linear group of degree two

↑ **Parent:** [Special linear group](#special-linear-group)

This [Lie group](lie-theory.md#lie-group) consists of real two-by-two matrices of determinant one. Its [Lie algebra](lie-algebra.md) is the space of traceless real two-by-two matrices. Its [Exponential map of a Lie group](lie-theory.md#exponential-map-of-a-lie-group) is not onto: by the [Cayley-Hamilton theorem](cayley-hamilton-theorem.md), $A^2=-\det(A)I$ for traceless $A$, and its exponential has trace either $2\cosh s$ or $2\cos s$, hence never less than $-2$. The determinant-one matrix $\operatorname{diag}(-2,-1/2)$ is therefore outside its exponential image.

#### Elementary unipotent generators of SL2R

↑ **Parent:** [Real special linear group of degree two](#real-special-linear-group-of-degree-two)

The upper and lower [unipotent matrices](lie-theory.md#unipotent-matrix) generate [SL2R](#real-special-linear-group-of-degree-two). For $a\ne0$, let $w(a)=U(a)L(-a^{-1})U(a)$; multiplication gives $w(a)=\begin{pmatrix}0&a\\-a^{-1}&0\end{pmatrix}$ and $w(a)w(-1)=\operatorname{diag}(a,a^{-1})$. A determinant-one matrix with upper-left entry $a\ne0$ factors as $L(c/a)\operatorname{diag}(a,a^{-1})U(b/a)$. If that entry vanishes, first add the second row to the first by $U(1)$. Lower unipotents are conjugates of upper unipotents, so the latter also generate the whole group normally.

### Projective special linear group

↑ **Parent:** [Special linear group](#special-linear-group)

The quotient of the [special linear group](#special-linear-group) by its scalar center, acting faithfully on [projective space](projective-space.md). It is a [simple group](finite-group-theory.md#simple-group) for $n\ge3$, or for $n=2$ and $|F|>3$. [Elementary transvection matrices](vector-space.md#elementary-transvection-matrix) give generation and perfectness, and the [Iwasawa simplicity lemma](finite-group-theory.md#iwasawa-simplicity-lemma) applies to the abelian subgroup of transvections with a fixed center.

#### Scalar kernel of the projective linear action

↑ **Parent:** [Projective special linear group](#projective-special-linear-group)

A linear transformation fixing every one-dimensional subspace is scalar. Fixing the coordinate lines makes it diagonal, and fixing the lines spanned by $e_i+e_j$ makes all diagonal entries equal. Within determinant-one [matrices](vector-space.md#matrix) the scalar satisfies $\lambda^n=1$. Conversely scalars fix all projective points. Commutation with all elementary [transvections](vector-space.md#transvection) shows these scalars are exactly the center of the [special linear group](#special-linear-group), so its projective quotient acts faithfully.

### Complex special linear group in dimension two

↑ **Parent:** [Special linear group](#special-linear-group)

Complex two-by-two [matrices](vector-space.md#matrix) of [determinant](multilinear-algebra.md#determinant) one form a complex three-dimensional [Lie group](lie-theory.md#lie-group), or a real six-dimensional [Lie group](lie-theory.md#lie-group). Their congruence action on Hermitian two-by-two [matrices](vector-space.md#matrix) gives the [Lorentz spinor double cover](special-relativity.md#lorentz-spinor-double-cover) with kernel $\{I,-I\}$. The two [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) representations are $A$ and $(A^\dagger)^{-1}$. Treating the group as real is essential for the second, antiholomorphic representation.

### Triangular-rotation factorization of real determinant-one matrices

↑ **Parent:** [Special linear group](#special-linear-group)

Every $g\in SL_2(\mathbb R)$ factors into an upper triangular determinant-one matrix and a [rotation matrix](linear-algebra.md#rotation-matrix). This follows because the triangular subgroup acts transitively on the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), a [group orbit](group-action.md#orbit-group-theory) of the full group, while $SO(2)$ is the [stabilizer subgroup](group-action.md#stabilizer-subgroup) of $i$. The intersection of the two subgroups is $\{\pm I\}$, giving exactly two matrix pairs $(h,k)$ and $(-h,-k)$. Requiring the diagonal of $h$ to be positive gives uniqueness. For $g=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ and $q=\sqrt{c^2+d^2}$, the positive branch is $h=\begin{pmatrix}1/q&(ac+bd)/q\\0&q\end{pmatrix}$ and $k=q^{-1}\begin{pmatrix}d&-c\\c&d\end{pmatrix}$.

### Congruence subgroup

↑ **Parent:** [Special linear group](#special-linear-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Congruence_subgroup)

A congruence subgroup of $SL_n(\mathbb Z)$ contains the kernel of reduction modulo some positive integer.

#### Principal congruence subgroup

↑ **Parent:** [Congruence subgroup](#congruence-subgroup)

The principal congruence subgroup of level $N$ is

$$
\Gamma(N)=\ker\left(SL_n(\mathbb Z)\longrightarrow SL_n(\mathbb Z/N\mathbb Z)\right).
$$

It has finite index because the target is finite.

#### Gamma 0 congruence subgroup

↑ **Parent:** [Congruence subgroup](#congruence-subgroup)

The Gamma 0 congruence subgroup is

$$
\Gamma_0(N)=\left\{\begin{pmatrix}a&b\\c&d\end{pmatrix}\in SL_2(\mathbb Z):c\equiv0\pmod N\right\}.
$$

#### Gamma 1 congruence subgroup

↑ **Parent:** [Congruence subgroup](#congruence-subgroup)

The subgroup

$$
\Gamma_1(N)=
\left\{
\begin{pmatrix}a&b\\c&d\end{pmatrix}\in SL_2(\mathbb Z):
a\equiv d\equiv1\pmod N,\ c\equiv0\pmod N
\right\}
$$

is a congruence subgroup of the [modular group](modular-function.md#modular-group).

##### Number of cusps of Gamma 1 of prime level

↑ **Parent:** [Gamma 1 congruence subgroup](#gamma-1-congruence-subgroup)

For an odd prime $p$, the group $\Gamma_1(p)$ has $p-1$ cusps. The general primitive-vector count gives

$$
\frac12\sum_{d\mid p}\varphi(d)\varphi(p/d)=p-1.
$$

The exceptional group $\Gamma_1(2)=\Gamma_0(2)$ has two cusps, represented by infinity and zero.

###### Prime Gamma 1 cusp counts and widths

↑ **Parent:** [Number of cusps of Gamma 1 of prime level](#number-of-cusps-of-gamma-1-of-prime-level)

For $p\ge5$, the [Gamma 1 congruence subgroup](#gamma-1-congruence-subgroup) has $(p-1)/2$ [modular cusps](modular-function.md#cusp-of-a-modular-group) of [cusp width](modular-function.md#width-of-a-cusp) one and $(p-1)/2$ of [cusp width](modular-function.md#width-of-a-cusp) $p$. Primitive columns modulo $p$, taken up to sign, are acted on by $(a,c)\mapsto(a+bc,c)$. The classes with $c=0$ have [cusp width](modular-function.md#width-of-a-cusp) one, the others [cusp width](modular-function.md#width-of-a-cusp) $p$. There are no effective elliptic stabilizers. The [genus formula for a modular curve](modular-function.md#genus-formula-for-a-modular-curve) gives genus $(p-5)(p-7)/24$.

## Group homomorphism

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_homomorphism)

A [group homomorphism](#group-homomorphism) is a [map](function.md#function-class) $\varphi:G\to H$ preserving the [group operation](group.md#group-operation): $\varphi(gh)=\varphi(g)\varphi(h)$. It also preserves the [identity element](algebraic-operation.md#identity-element) and [inverse elements](algebraic-operation.md#inverse-element). In an additive [group](group.md), the same requirement reads $\varphi(g+h)=\varphi(g)+\varphi(h)$. A [group homomorphism](#group-homomorphism) preserves a way of combining inputs, even when several inputs have the same output.

Reduction modulo three from $\mathbb Z/6\mathbb Z$ to $\mathbb Z/3\mathbb Z$ is a [group homomorphism](#group-homomorphism): reducing a [sum](arithmetic.md#sum) agrees with adding the reduced residues. For example, $2+5=1$ modulo six, and both sides reduce to one modulo three; the outputs $2$ and $2$ also add to one modulo three. This [map](function.md#function-class) is [surjective](algebra.md#surjective-function) but not [injective](algebra.md#injective-function), since zero and three both map to zero.

The [sign of a permutation](finite-group-theory.md#sign-of-a-permutation) gives another example, from the [symmetric group](finite-group-theory.md#symmetric-group) $S_3$ to the multiplicative [group](group.md) $\{1,-1\}$. A product of two odd [permutations](combinatorics.md#permutation) is even, matching $(-1)(-1)=1$. Its [group kernel](#kernel-of-a-group-homomorphism) is $A_3$, the [alternating group](finite-group-theory.md#alternating-group) of even [permutations](combinatorics.md#permutation). This shows how a [group homomorphism](#group-homomorphism) can retain a useful feature while forgetting other details.

### Homomorphism of abelian groups

↑ **Parent:** [Group homomorphism](#group-homomorphism)

A [group homomorphism](#group-homomorphism) between [abelian groups](group.md#abelian-group), conventionally written additively. Its [kernel](kernel-of-a-linear-map.md) and [image](set-theory.md#image-of-a-function) are [subgroups](group.md#subgroup), and the additive formula implies preservation of zero, negation and every integer multiple. Maps on [Mordell-Weil groups](normalization-of-an-algebraic-curve.md#mordell-weil-group) induced by [isogenies of elliptic curves](normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) and by [good reduction](normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve) are examples.

### Surjective group homomorphism

↑ **Parent:** [Group homomorphism](#group-homomorphism)

A group homomorphism $f:G\to H$ is surjective when every element of $H$ is $f(g)$ for some $g\in G$.

### Covering homomorphism

↑ **Parent:** [Group homomorphism](#group-homomorphism)

A covering homomorphism is a surjective homomorphism of topological groups whose underlying map is a [covering space](algebraic-topology.md#covering-space). Its discrete kernel is the fiber over the identity.

### Homomorphism between cyclic groups

↑ **Parent:** [Group homomorphism](#group-homomorphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homomorphism_between_cyclic_groups)

A homomorphism from $C_n$ is determined by the image of one generator; a surjection $C_n\to C_m$ exists exactly when $m\mid n$.

### Kernel of a group homomorphism

↑ **Parent:** [Group homomorphism](#group-homomorphism)

The [kernel of a group homomorphism](#kernel-of-a-group-homomorphism) is the group version of a [kernel](algebra.md#kernel-algebra). For $\varphi:G\to H$, it is

$$
\ker\varphi=\{g\in G:\varphi(g)=e_H\}.
$$

It is a [normal subgroup](#normal-subgroup) of the domain: for $n$ in the [group kernel](#kernel-of-a-group-homomorphism), $\varphi(gng^{-1})=\varphi(g)e_H\varphi(g)^{-1}=e_H$. The [group kernel](#kernel-of-a-group-homomorphism) describes inputs whose effect disappears after mapping. For reduction modulo three from $\mathbb Z/6\mathbb Z$, it is $\{0,3\}$; for the [sign of a permutation](finite-group-theory.md#sign-of-a-permutation) on $S_3$, it is $A_3$. A [group homomorphism](#group-homomorphism) is [injective](algebra.md#injective-function) exactly when its [group kernel](#kernel-of-a-group-homomorphism) contains only the [identity element](algebraic-operation.md#identity-element).

#### Fibres of a group homomorphism are cosets of its kernel

↑ **Parent:** [Kernel of a group homomorphism](#kernel-of-a-group-homomorphism)

For a [group homomorphism](#group-homomorphism) $\varphi:G\to H$, two inputs give the same output exactly when $\varphi(h^{-1}g)=e_H$. Consequently the [fibre](function.md#fiber-of-a-function) over an output $\varphi(h)$ is the left [coset](#coset) $h\ker\varphi$. These [cosets](#coset) identify precisely the inputs indistinguishable to $\varphi$, which is the mechanism behind the [first isomorphism theorem](#first-isomorphism-theorem).

### Image of a group homomorphism

↑ **Parent:** [Group homomorphism](#group-homomorphism)

The image of a group homomorphism $\phi:G\to H$ is the subgroup $\{\phi(g):g\in G\}$ of $H$.

## Automorphism group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Automorphism_group)

The automorphism group of a [group](group.md) $G$ is the group of all isomorphisms $G\to G$ under composition.

### Holomorph

↑ **Parent:** [Automorphism group](#automorphism-group)

The holomorph acts on the underlying set of a [group](group.md) by $x\mapsto g\alpha(x)$. Its multiplication is $(g,\alpha)(h,\beta)=(g\alpha(h),\alpha\beta)$. This is exactly the [normalizer](group-action.md#normalizer) of the left regular [permutation](combinatorics.md#permutation) representation: a normalizing [permutation](combinatorics.md#permutation) fixing the identity is an [group automorphism](algebra.md#group-automorphism), and every normalizing [permutation](combinatorics.md#permutation) is a left translation followed by one. The embedded copy of $G$ is normal and the identity stabilizer is its [group automorphism](algebra.md#group-automorphism) [group](group.md).

### Inner automorphism

↑ **Parent:** [Automorphism group](#automorphism-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inner_automorphism)

An inner automorphism is conjugation by an element of the group. The inner automorphisms form a normal subgroup $\operatorname{Inn}(G)\triangleleft\operatorname{Aut}(G)$.

### Outer automorphism group

↑ **Parent:** [Automorphism group](#automorphism-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Outer_automorphism_group)

The outer automorphism group is

$$
\operatorname{Out}(G)=\operatorname{Aut}(G)/\operatorname{Inn}(G).
$$

It records automorphisms modulo conjugation by elements of $G$.

#### Outer automorphism of a group

↑ **Parent:** [Outer automorphism group](#outer-automorphism-group)

An outer [group automorphism](algebra.md#group-automorphism) is not [conjugation](group-action.md#conjugation) by any element of the [group](group.md). Its nonidentity class belongs to $\operatorname{Out}(G)=\operatorname{Aut}(G)/\operatorname{Inn}(G)$. A permutation-group example is the exceptional automorphism of $S_6$ that swaps its natural and transitive copies of $S_5$; it sends a [transposition](combinatorics.md#transposition-permutation) to a product of three disjoint [transpositions](combinatorics.md#transposition-permutation) and hence cannot be inner.

## Group cohomology

↑ **Parent:** [Group theory](group-theory.md)

[This section is present in another page, follow this link to view it.](group-cohomology.md)

## Group homology

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_homology)

Group homology is obtained by tensoring a [projective resolution](homological-algebra.md#projective-resolution) of the trivial $\mathbb ZG$-module with a coefficient module and taking [homology](homology.md).

### Homology of a finite cyclic group

↑ **Parent:** [Group homology](#group-homology)

For the cyclic group $C_m$ with trivial integral coefficients,

$$
H_0(C_m;\mathbb Z)=\mathbb Z,
\qquad H_{2k+1}(C_m;\mathbb Z)=\mathbb Z/m,
\qquad H_{2k}(C_m;\mathbb Z)=0
$$

for $k\geq0$ in the positive-degree formulas.

### Schur multiplier

↑ **Parent:** [Group homology](#group-homology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur_multiplier)

The Schur multiplier of a group $G$ is its second integral [group homology](#group-homology) group:

$$
M(G)=H_2(G,\mathbb Z).
$$

<h4 id="hopf-s-formula">Hopf's formula</h4>

↑ **Parent:** [Schur multiplier](#schur-multiplier)

For a [free presentation](geometric-group-theory.md#free-presentation) $G\cong F/R$, [Hopf's formula](#hopf-s-formula) is

$$
H_2(G,\mathbb Z)\cong\frac{R\cap[F,F]}{[F,R]}.
$$

#### Schur multiplier of an abelian group

↑ **Parent:** [Schur multiplier](#schur-multiplier)

For an [abelian group](group.md#abelian-group) $A$,

$$
M(A)\cong\bigwedge^2A.
$$

For a finite direct sum of cyclic groups this gives one summand $C_{\gcd(m,n)}$ for every pair $C_m,C_n$.

## Finite group theory

↑ **Parent:** [Group theory](group-theory.md)

[This section is present in another page, follow this link to view it.](finite-group-theory.md)

## Residually finite group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Residually_finite_group)

A group $G$ is residually finite when every nonidentity $g\in G$ survives in some finite quotient: there are a finite group $Q$ and a homomorphism $\phi:G\to Q$ with $\phi(g)\ne1$.

### Finite residual

↑ **Parent:** [Residually finite group](#residually-finite-group)

The finite residual consists of all elements killed by every homomorphism to a finite group. A [group](group.md) is a [residually finite group](#residually-finite-group) precisely when its finite residual is trivial. Intersecting all finite-index subgroups gives the same result: the [normal core](#core-group-theory) of each such subgroup is normal of finite index and lies inside it.

#### Finite residual contains surjective endomorphism kernels

↑ **Parent:** [Finite residual](#finite-residual)

Let $G$ be a [finitely generated group](group.md#finitely-generated-group) and $\theta:G\to G$ a surjective [endomorphism](algebra.md#endomorphism). Pullback by $\theta$ permutes the finite set of normal subgroups of any prescribed finite index. For each such $N$, some iterate satisfies $\theta^{-m}(N)=N$, so $\ker\theta\subseteq\ker\theta^m\subseteq N$. Intersecting proves the inclusion. Consequently every finitely generated [residually finite group](#residually-finite-group) is a [Hopfian group](#hopfian-group).

### Residual finiteness of semidirect products

↑ **Parent:** [Residually finite group](#residually-finite-group)

If $K$ is a [finitely generated group](group.md#finitely-generated-group), then the [semidirect product](#semidirect-product) $K\rtimes H$ is a [residually finite group](#residually-finite-group) exactly when both $K$ and $H$ are [residually finite groups](#residually-finite-group). To separate an element whose $H$ coordinate is nontrivial, use a finite quotient of $H$. For $1\ne k\in K$, choose a finite-index normal subgroup $U$ omitting $k$, and intersect all subgroups of index at most $[K:U]$ to obtain a characteristic finite-index subgroup $C\leq U$. The induced map into $(K/C)\rtimes\operatorname{im}(H\to\operatorname{Aut}(K/C))$ has finite target and separates $k$. More generally, finite generation can be replaced by a separating family of finite-index normal subgroups invariant under the given $H$ action.

### Conjugacy separable group

↑ **Parent:** [Residually finite group](#residually-finite-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugacy_separable_group)

A group $G$ is conjugacy separable when any two nonconjugate elements remain nonconjugate in some finite quotient. Equivalently, every [conjugacy class](group-action.md#conjugacy-class) is closed in the [profinite topology](topological-group.md#profinite-topology).

### Subgroup of a residually finite group

↑ **Parent:** [Residually finite group](#residually-finite-group)

Every subgroup of a residually finite group is residually finite, because a finite quotient separating an element of the ambient group also separates it after restriction to the subgroup.

### Reduction modulo a prime in an integral matrix group

↑ **Parent:** [Residually finite group](#residually-finite-group)

For a [prime number](prime-number.md) $p$, reducing every entry modulo $p$ defines a [group homomorphism](#group-homomorphism) from an integral matrix group to the corresponding matrix group over $\mathbb F_p$. The target is finite. If an integral matrix $M$ is not the identity, choosing $p$ not to divide one nonzero entry of $M-I$ ensures that its reduction is also nonidentity.

### Infinite residually finite group is not simple

↑ **Parent:** [Residually finite group](#residually-finite-group)

An infinite residually finite group is not a [simple group](finite-group-theory.md#simple-group). For a nonidentity element, residual finiteness supplies a map to a finite group in which it survives. Its kernel is proper and cannot be trivial, since an infinite group cannot inject into a finite group.

## Hopfian group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hopfian_group)

A group is Hopfian when every surjective endomorphism is an automorphism. Every finitely generated residually finite group is Hopfian.

### Non-Hopfian group

↑ **Parent:** [Hopfian group](#hopfian-group)

A non-Hopfian group admits a surjective [endomorphism](algebra.md#endomorphism) which is not injective. The [Baumslag-Solitar group](geometric-group-theory.md#baumslag-solitar-group) $BS(2,3)$ has such an endomorphism $a\mapsto a^2$, $t\mapsto t$: its image contains $a^2$ and $a^3$, while the nonidentity [commutator](lie-algebra.md#commutator) $[a,tat^{-1}]$ lies in its kernel by [Britton's lemma](geometric-group-theory.md#britton-s-lemma).

## Torsion element

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Torsion_element)

A torsion element has finite order.

### Torsion group

↑ **Parent:** [Torsion element](#torsion-element)

A [group](group.md) is a torsion group when every element is a [torsion element](#torsion-element), meaning that each element has finite order. The orders need not have a common finite bound. A torsion group has no nontrivial [torsion-free group](group.md#torsion-free-group) as a subgroup; in particular it cannot contain a nonabelian [free group](geometric-group-theory.md#free-group). Infinite [finitely generated groups](group.md#finitely-generated-group) of this kind can be constructed using a [torsion group construction by p-power relators](geometric-group-theory.md#torsion-group-construction-by-p-power-relators).

#### Infinite residually finite torsion group

↑ **Parent:** [Torsion group](#torsion-group)

Enumerate all words $w_i$ on two generators in a [free pro-p group](topological-group.md#free-pro-p-group). Choose powers $p^{e_i}$ so large that $\sum_i\tau^{p^{e_i}}<2\tau-1$ for some $1/2<\tau<1$, and impose the closed normal relations $w_i^{p^{e_i}}=1$. The [Golod-Shafarevich infinitude criterion for pro-p groups](topological-group.md#golod-shafarevich-infinitude-criterion-for-pro-p-groups) makes the resulting pro-$p$ group infinite. Its abstract subgroup generated by the two generator images is dense and infinite; each element is represented by an enumerated word and has finite order. The ambient finite quotients separate its elements, so it is also a [residually finite group](#residually-finite-group). The abstract subgroup, rather than the whole topological group, is the desired finitely generated [torsion group](#torsion-group).

#### Locally finite group

↑ **Parent:** [Torsion group](#torsion-group)

A [group](group.md) is locally finite when every [subgroup](group.md#subgroup) that is a [finitely generated group](group.md#finitely-generated-group) is finite. It is a [torsion group](#torsion-group), since the cyclic subgroup generated by one element must be finite. A [restricted direct sum of groups](#restricted-direct-sum-of-groups) with finite factors is locally finite. A locally finite group can be infinite, while a locally finite [finitely generated group](group.md#finitely-generated-group) is finite by definition.

##### Local finiteness is closed under extensions

↑ **Parent:** [Locally finite group](#locally-finite-group)

For $1\to N\to G\to Q\to1$ with $N,Q$ locally finite, take a finitely generated subgroup $L\leq G$. Its image in $Q$ is finite, so $L\cap N$ has finite index in $L$ and is finitely generated by [Schreier's lemma](geometric-group-theory.md#schreier-s-lemma). Local finiteness of $N$ makes that intersection finite. Thus $L$ itself is finite, proving local finiteness of $G$.

// Target: algebra.bigb

### Torsion subgroup

↑ **Parent:** [Torsion element](#torsion-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Torsion_subgroup)

The torsion subgroup of an [abelian group](group.md#abelian-group) consists of all elements of finite order. For a finitely generated abelian group, it is the finite direct summand complementary to the free abelian part.

#### Torsion subgroup killed by an integer

↑ **Parent:** [Torsion subgroup](#torsion-subgroup)

For an [abelian group](group.md#abelian-group) $G$ and an integer $m\geq1$, its $m$-torsion subgroup is $G[m]=\{x\in G:mx=0\}$, the kernel of multiplication by $m$. In a [finite abelian group](group.md#finite-abelian-group), every nonempty fiber of this homomorphism has [cardinality](cardinal-number.md#cardinality) $|G[m]|$, so $|G:mG|=|G[m]|$. This follows directly: if $mx=my$, then $x-y\in G[m]$, and conversely translating by an element of $G[m]$ leaves the image unchanged. On the [cyclic group](group.md#cyclic-group) $\mathbb Z_N$, the solutions of $mx=0$ number $\gcd(m,N)$; divide both integers by their greatest common divisor to see that $x$ must be a multiple of $N/\gcd(m,N)$.

#### Primary torsion subgroup at a prime

↑ **Parent:** [Torsion subgroup](#torsion-subgroup)

For an abelian group $A$, its $p$-primary torsion subgroup is $A\{p\}=\{a:p^ra=0\text{ for some }r\ge0\}$. It is zero exactly when $A[p]=0$, since a nonzero element of $p$-power order has a multiple of order $p$. Multiplication by an integer prime to $p$ is an automorphism on it.

## Free abelian group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Free_abelian_group)

A free abelian group has a basis over $\mathbb Z$ and is isomorphic to a direct sum of copies of $\mathbb Z$.

### Saturated sublattice

↑ **Parent:** [Free abelian group](#free-abelian-group)

A subgroup $L\subseteq M$ of a finitely generated free abelian group is saturated if $am\in L$ for a nonzero integer $a$ implies $m\in L$. Equivalently $M/L$ is torsion-free. It is then free abelian and the quotient map splits, so $L$ is a direct summand. Intersecting $M$ with a real linear subspace always gives a saturated sublattice.

// Target: algebra.bigb

### Primitive lattice element

↑ **Parent:** [Free abelian group](#free-abelian-group)

A nonzero element of a [free abelian group](#free-abelian-group) is primitive when it is part of an integral basis, equivalently when some homomorphism to $\mathbb Z$ takes it to one. Its coordinates have [greatest common divisor](divisibility.md#greatest-common-divisor) one. This lattice meaning differs from a [primitive homology class](homology.md#primitive-homology-class) in the coalgebra sense.

## Normal subgroup

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_subgroup)

A [subgroup](group.md#subgroup) $N\leq G$ is a [normal subgroup](#normal-subgroup) when $gNg^{-1}=N$ for every $g\in G$. In other words, [conjugation](group-action.md#conjugation) by any [group element](group.md#group-element) preserves the [subgroup](group.md#subgroup) as a [set](set.md), although it may exchange its individual elements. Equivalently, $gN=Ng$ for every $g$: the left and right [cosets](#coset) of $N$ agree. Write $N\trianglelefteq G$.

Every [subgroup](group.md#subgroup) of an [abelian group](group.md#abelian-group) is a [normal subgroup](#normal-subgroup), because [conjugation](group-action.md#conjugation) fixes each element. Normality can also hold in a nonabelian [group](group.md): in $S_3$, the three even [permutations](combinatorics.md#permutation) form the [alternating group](finite-group-theory.md#alternating-group) $A_3=\{e,(123),(132)\}$, a [normal subgroup](#normal-subgroup) as the [group kernel](#kernel-of-a-group-homomorphism) of the [sign of a permutation](finite-group-theory.md#sign-of-a-permutation). Its two [cosets](#coset) separate the even and odd [permutations](combinatorics.md#permutation).

In contrast, $H=\{e,(12)\}$ is a [subgroup](group.md#subgroup) of $S_3$ but is not a [normal subgroup](#normal-subgroup). With [function composition](function.md#function-composition) of [permutations](combinatorics.md#permutation) acting rightmost first, choose $g=(123)$. Then

$$
gH=\{(123),(13)\},\qquad Hg=\{(123),(23)\},
$$

which are different [cosets](#coset). Also $g(12)g^{-1}=(23)\notin H$, directly contradicting invariance under [conjugation](group-action.md#conjugation). Thus a [subgroup](group.md#subgroup) alone does not suffice for [quotient group](#quotient-group) multiplication.

<a id="image-a-normal-subgroup-gives-matching-left-and-right-cosets-while-a-nonnormal-subgroup-can-give-different-ones"></a>
![](normal-subgroup-coset-contrast.png)

**[Figure 11](#image-a-normal-subgroup-gives-matching-left-and-right-cosets-while-a-nonnormal-subgroup-can-give-different-ones). A normal subgroup gives matching left and right cosets, while a nonnormal subgroup can give different ones**.

The practical value of normality is [coset multiplication is well-defined exactly for normal subgroups](#coset-multiplication-is-well-defined-exactly-for-normal-subgroups). Each [coset](#coset) can act as one element of a [quotient group](#quotient-group), with results independent of representatives. Conversely every [normal subgroup](#normal-subgroup) is the [group kernel](#kernel-of-a-group-homomorphism) of its [quotient map of groups](#quotient-map-of-groups), so normality also identifies which distinctions a [group homomorphism](#group-homomorphism) can consistently forget.

### p-residual of a finite group

↑ **Parent:** [Normal subgroup](#normal-subgroup)

The p-residual is the smallest [normal subgroup](#normal-subgroup) with p-group quotient, equivalently the subgroup generated by all elements of order prime to $p$. It is [characteristic](algebra.md#characteristic-of-a-field) and satisfies $O^p(O^p(G))=O^p(G)$: an extension of two finite p-groups is a p-group. A finite group has a [normal p-complement](#normal-p-complement) exactly when its p-residual has order prime to $p$.

### Complement of a normal subgroup

↑ **Parent:** [Normal subgroup](#normal-subgroup)

A group complement to a [normal subgroup](#normal-subgroup) $N\triangleleft G$ is a subgroup $H$ with $G=NH$ and $N\cap H=1$. Projection identifies $H$ with $G/N$, and conjugation gives $G=N\rtimes H$. This is a subgroup notion, not the set-theoretic complement of $N$.

### Normal subgroups of coprime order commute

↑ **Parent:** [Normal subgroup](#normal-subgroup)

If finite [normal subgroups](#normal-subgroup) $H,K$ of a [group](group.md) have coprime orders, their intersection is trivial by [Lagrange's theorem](#lagrange-s-theorem). For $h\in H$ and $k\in K$, the [commutator](lie-algebra.md#commutator) $hkh^{-1}k^{-1}$ belongs to both subgroups: write it as $h(kh^{-1}k^{-1})$ to use normality of $H$, and as $(hkh^{-1})k^{-1}$ to use normality of $K$. Hence it is the identity and $hk=kh$. The product subgroup is therefore isomorphic to the [direct product of groups](#direct-product-of-groups) $H\times K$.

### Normal p-complement

↑ **Parent:** [Normal subgroup](#normal-subgroup)

For a finite group with Sylow $p$-subgroup $P$, a normal $p$-complement is a normal subgroup of order $|G|/|P|$. It consists exactly of the elements of order prime to $p$: every such element has trivial image in the $p$-group quotient, and every element of the complement has prime-to-$p$ order. Thus a normal $p$-complement, if it exists, is unique and a [characteristic subgroup](algebra.md#characteristic-subgroup).

#### p-nilpotent group

↑ **Parent:** [Normal p-complement](#normal-p-complement)

A finite group is p-nilpotent when it has a [normal p-complement](#normal-p-complement). This terminology is distinct from having a normal Sylow p-subgroup. A finite group is [nilpotent](commutative-algebra.md#nilpotent) exactly when it is p-nilpotent for every prime dividing its order.

<h5 id="thompson-s-character-degree-normal-complement-theorem">Thompson's character-degree normal complement theorem</h5>

↑ **Parent:** [P-nilpotent group](#p-nilpotent-group)

If a prime $p$ divides the degree of every [nonlinear irreducible character](representation-theory.md#nonlinear-irreducible-character) of a finite group, the group has a [normal p-complement](#normal-p-complement). Indeed, the p-prime-degree characters are exactly the linear characters. Their squared-degree sum is $|G:G'|$, whose p-part is $|G:G'|_p$; [Isaacs' character-degree criterion for p-nilpotency](#isaacs-character-degree-criterion-for-p-nilpotency) applies.

##### Isaacs' character-degree criterion for p-nilpotency

↑ **Parent:** [P-nilpotent group](#p-nilpotent-group)

The integer $h=|G:G'|_p$ divides $s=\sum_{\chi\in\operatorname{Irr}_{p'}(G)}\chi(1)^2$. The group is [p-nilpotent](#p-nilpotent-group) exactly when $p\nmid s/h$. To see this, let $N=O^p(G)$. Invariant p-prime-degree characters of $N$ extend, and each has exactly $h$ extensions of p-prime degree. Conjugation by the p-group $G/N$ then gives $s/h\equiv|N|\pmod p$. Thus the quotient is prime to $p$ precisely when $N$ is a [normal p-complement](#normal-p-complement).

### Maximal normal subgroup

↑ **Parent:** [Normal subgroup](#normal-subgroup)

A proper [normal subgroup](#normal-subgroup) maximal among proper normal subgroups. Its quotient is a nontrivial [simple group](finite-group-theory.md#simple-group). Maximality among normal subgroups does not imply maximality among all subgroups.

// Target: algebra.bigb

#### Finitely generated groups have maximal proper normal subgroups

↑ **Parent:** [Maximal normal subgroup](#maximal-normal-subgroup)

Above any proper normal subgroup of a finitely generated group, a chain of proper normal subgroups has proper union. Otherwise that union would contain the finite generating set, all of which would already lie in one member of the chain. The [Zorn lemma](set-theory.md#zorn-s-lemma) therefore provides a maximal proper normal subgroup containing the given one.

// Target: algebra.bigb

### Subnormal series

↑ **Parent:** [Normal subgroup](#normal-subgroup)

A subnormal series is a finite chain of [subgroups](group.md#subgroup) in which each is a [normal subgroup](#normal-subgroup) of the next. A member need not be normal in the whole [group](group.md). Requiring the factors to be [cyclic groups](group.md#cyclic-group) defines a [polycyclic group](#polycyclic-group); allowing finite factors as well defines a [poly-(cyclic or finite) group](group.md#poly-cyclic-or-finite-group).

#### Schreier refinement theorem

↑ **Parent:** [Subnormal series](#subnormal-series)

Any two finite [subnormal series](#subnormal-series) have refinements with the same successive factors up to ordering and [group isomorphism](algebra.md#group-isomorphism). For descending chains $A_i$ and $B_j$, insert $A_{i+1}(A_i\cap B_j)$ between $A_i$ and $A_{i+1}$ and insert $B_{j+1}(B_j\cap A_i)$ in the other chain. The [Zassenhaus butterfly lemma](#zassenhaus-butterfly-lemma) identifies the factor indexed by $(i,j)$ in the first refinement with the factor indexed by $(j,i)$ in the second. If both chains are [composition series](finite-group-theory.md#composition-series), their simple factors admit no nontrivial refinement, giving the [Jordan–Hölder theorem](finite-group-theory.md#jordan-holder-theorem).

#### Zassenhaus butterfly lemma

↑ **Parent:** [Subnormal series](#subnormal-series)

Let $A'\trianglelefteq A$ and $B'\trianglelefteq B$ be [subgroups](group.md#subgroup) of one [group](group.md). Put $C=A\cap B$ and $D=(A'\cap B)(A\cap B')$. Then $D\trianglelefteq C$ and the [first isomorphism theorem](#first-isomorphism-theorem) identifies both

$$
\frac{A'C}{A'(A\cap B')}\quad\text{and}\quad\frac{B'C}{B'(B\cap A')}
$$

with $C/D$. Indeed $C$ maps onto either displayed [quotient group](#quotient-group), and its kernel in either case is $D$. This gives the matching factors used in the [Schreier refinement theorem](#schreier-refinement-theorem).

#### Normal series of a group

↑ **Parent:** [Subnormal series](#subnormal-series)

A normal series is a chain $1=G_0\le G_1\le\cdots\le G_r=G$ whose terms are all [normal subgroups](#normal-subgroup) of the ambient group. A [subnormal series](#subnormal-series) only requires each term normal in the next. Confusing these conditions would incorrectly require every term of a composition series to be normal in the full group.

##### Chief series

↑ **Parent:** [Normal series of a group](#normal-series-of-a-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chief_series)

A chief series is a strict [normal series of a group](#normal-series-of-a-group) with no proper normal-series refinement. Its factors are [minimal normal subgroups](#minimal-normal-subgroup) of the appropriate quotient groups. A chief factor of a finite soluble group is elementary abelian, whereas a composition factor of a finite soluble group is cyclic of prime order. A chief factor can therefore have order larger than a prime.

###### Chief factor

↑ **Parent:** [Chief series](#chief-series)

A chief factor of $G$ is a quotient $N/M$ with $M,N$ normal in $G$ and no $G$-normal subgroup strictly between them. Equivalently, $N/M$ is a [minimal normal subgroup](#minimal-normal-subgroup) of $G/M$. Such factors are the successive factors of a [chief series](#chief-series), and are direct products of isomorphic simple groups when $G$ is finite.

### Minimal normal subgroup

↑ **Parent:** [Normal subgroup](#normal-subgroup)

A minimal normal subgroup is a nontrivial [normal subgroup](#normal-subgroup) containing no smaller nontrivial normal subgroup of the ambient group. It need not be a minimal nontrivial subgroup. In a finite [soluble group](#solvable-group), it is elementary abelian: its derived subgroup must be trivial, a characteristic Sylow subgroup selects one prime, and the characteristic subgroup of elements killed by that prime gives exponent $p$.

#### Minimal normal subgroups of finite solvable groups are elementary abelian

↑ **Parent:** [Minimal normal subgroup](#minimal-normal-subgroup)

A nontrivial [minimal normal subgroup](#minimal-normal-subgroup) $N$ of a finite [solvable group](#solvable-group) is abelian: its [commutator subgroup](#commutator-subgroup) is characteristic, and minimality plus solvability excludes $N'=N$. A nontrivial [Sylow subgroup](finite-group-theory.md#sylow-subgroup) of this [abelian group](group.md#abelian-group) is characteristic, so minimality makes $N$ a p-group. The [characteristic subgroup](algebra.md#characteristic-subgroup) of pth powers is proper, hence trivial by minimality. Therefore $N$ is an [elementary abelian group](group.md#elementary-abelian-group).

#### Direct-product structure of a finite minimal normal subgroup

↑ **Parent:** [Minimal normal subgroup](#minimal-normal-subgroup)

Choose a minimal nontrivial normal subgroup $L$ of $K$. Its conjugates under the ambient group are minimal normal subgroups of $K$; distinct ones intersect trivially and commute. Choose a maximal family whose product is direct. Any omitted conjugate either lies in that product or meets it trivially and could be adjoined, so all conjugates lie in it. Their product is ambient-normal and therefore is $K$. A normal subgroup of one factor is then normal in $K$, since the other factors commute with it; minimality makes each factor simple. All factors are isomorphic because they are conjugates of $L$. In the abelian case they are cyclic of one common prime order.

#### Socle of a finite group

↑ **Parent:** [Minimal normal subgroup](#minimal-normal-subgroup)

The socle is generated by all minimal nontrivial normal subgroups. Distinct minimal normal subgroups commute and meet trivially, although in the abelian case not every collection of them is an independent direct-product decomposition. It is a direct product of simple groups. In a faithful primitive permutation group each nontrivial normal subgroup is transitive; its minimal normal subgroups are either elementary abelian and regular, or direct powers of a nonabelian simple group. This is the starting point of the [O'Nan–Scott theorem](group-action.md#o-nan-scott-theorem).

### Normal subgroup of order two is central

↑ **Parent:** [Normal subgroup](#normal-subgroup)

If $N=\{1,z\}$ is a [normal subgroup](#normal-subgroup) of a [group](group.md) $G$, conjugation by any element of $G$ preserves $N$ and fixes $1$. It must therefore fix $z$ as well. Thus $N$ lies in the [center of a group](#center-of-a-group). This fact can turn a small [normal subgroup](#normal-subgroup) into a commuting factor without assuming the whole group is abelian.

### Core (group theory)

↑ **Parent:** [Normal subgroup](#normal-subgroup)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Core_(group_theory))

The core of a [subgroup](group.md#subgroup) $H\leq G$ is

$$
\operatorname{Core}_G(H)=\bigcap_{g\in G}gHg^{-1}.
$$

It is the largest [normal subgroup](#normal-subgroup) of $G$ contained in $H$. If $H$ has finite index $k$, the action on $G/H$ gives $[G:\operatorname{Core}_G(H)]\leq k!$.

### Normal closure

↑ **Parent:** [Normal subgroup](#normal-subgroup)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_closure)

The normal closure of a subset $S\subseteq G$ is the smallest [normal subgroup](#normal-subgroup) containing $S$, equivalently the subgroup generated by all conjugates $gsg^{-1}$ with $g\in G$ and $s\in S$.

### Preimage of a normal subgroup

↑ **Parent:** [Normal subgroup](#normal-subgroup)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Preimage_of_a_normal_subgroup)

The preimage of a normal subgroup under any group homomorphism is normal.

### Image of a normal subgroup

↑ **Parent:** [Normal subgroup](#normal-subgroup)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Image_of_a_normal_subgroup)

Under a surjective homomorphism, the image of a normal subgroup is normal.

## Dedekind group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dedekind_group)

A Dedekind group is a group in which every subgroup is normal.

## Projective linear group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_linear_group)

The projective linear group is $PGL_n(F)=GL_n(F)/F^\times$ and acts on projective space.

<h3 id="mobius-group">Möbius group</h3>

↑ **Parent:** [Projective linear group](#projective-linear-group)

The Möbius group is the [group](group.md) of all [Möbius transformations](#mobius-transformation) of the [Riemann sphere](riemann-surfaces.md#riemann-sphere), under [function composition](function.md#function-composition). An invertible $2\times2$ complex matrix represents $z\mapsto(az+b)/(cz+d)$, and nonzero scalar multiples represent the same transformation. Rescaling a representative to determinant one gives a surjective [group homomorphism](#group-homomorphism) $SL_2(\mathbb C)\to\mathcal M$ with [kernel of a group homomorphism](#kernel-of-a-group-homomorphism) $\{I,-I\}$. Thus it is also the [projective linear group](#projective-linear-group) $PGL_2(\mathbb C)$ and the quotient $PSL_2(\mathbb C)=SL_2(\mathbb C)/\{\pm I\}$.

<h4 id="mobius-pointwise-stabilizer-of-two-points">Möbius pointwise stabilizer of two points</h4>

↑ **Parent:** [Möbius group](#mobius-group)

For two distinct points of the [Riemann sphere](riemann-surfaces.md#riemann-sphere), conjugate by a [Möbius transformation](#mobius-transformation) sending them to zero and infinity. A transformation fixing those two points has the form $z\mapsto\lambda z$, $\lambda\ne0$. Composition multiplies the parameter, so the [pointwise stabilizer](group-action.md#pointwise-stabilizer) is isomorphic to the [complex multiplicative group](group.md#complex-multiplicative-group). For zero and one, conjugation by $z/(1-z)$ gives $z\mapsto\lambda z/[1+(\lambda-1)z]$.

<h4 id="mobius-transformations-permuting-three-points">Möbius transformations permuting three points</h4>

↑ **Parent:** [Möbius group](#mobius-group)

The [Möbius transformations](#mobius-transformation) preserving a three-point set act faithfully on it: one fixing all three is the identity. Every permutation is realized because a [Möbius transformation](#mobius-transformation) can send any ordered distinct triple to any other, by composing the two normalizations to $0,1,\infty$. For that normalized set the six maps are $z$, $1-z$, $1/z$, $1/(1-z)$, $z/(z-1)$ and $(z-1)/z$. Thus its setwise stabilizer is the [symmetric group](finite-group-theory.md#symmetric-group) $S_3$. Normalizing any other three-point set conjugates its stabilizer to this group.

#### Subgroup generated by complex scalings and reciprocal inversion

↑ **Parent:** [Möbius group](#mobius-group)

The [Möbius transformations](#mobius-transformation) generated by $D_\lambda(z)=\lambda z$ with $\lambda\ne0$ and $I(z)=1/z$ have exactly the two displayed forms. The relations $I^2=1$ and $ID_\lambda=D_{\lambda^{-1}}I$ reduce every word to $D_\lambda I^\epsilon$, $\epsilon\in\{0,1\}$. This is a [semidirect product](#semidirect-product) of $\mathbb C^\times$ with a cyclic group of order two acting by multiplicative inversion. It preserves the unordered pair $\{0,\infty\}$, and only its scaling elements fix zero.

<h4 id="finite-abelian-subgroup-of-the-mobius-group">Finite abelian subgroup of the Möbius group</h4>

↑ **Parent:** [Möbius group](#mobius-group)

A finite [abelian subgroup](group.md#abelian-subgroup) of the [Möbius group](#mobius-group) is cyclic or isomorphic to $C_2\times C_2$. If it contains an element of order greater than two, conjugate that element's two fixed points to $0,\infty$. Every commuting map must preserve these points individually: an interchange would conjugate the element to its inverse. All maps are then scalings, forming a cyclic finite subgroup of $\mathbb C^\times$. If every nonidentity element has order two, choose one with fixed points $0,\infty$; the subgroup acts on this pair with image of size at most two and kernel contained in $\{z,-z\}$. Its size is therefore at most four, giving the asserted possibilities.

<h3 id="mobius-transformation">Möbius transformation</h3>

↑ **Parent:** [Projective linear group](#projective-linear-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Möbius_transformation)

A Möbius transformation of the Riemann sphere has the form

$$
z\longmapsto\frac{az+b}{cz+d},
\qquad ad-bc\ne0.
$$

The group is generated by translations, nonzero complex scalings, and inversion $z\mapsto1/z$.

<h4 id="mobius-translation-scaling-inversion-factorization">Möbius translation-scaling-inversion factorization</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

Let $T_a(z)=z+a$, $S_k(z)=kz$ with $k\ne0$, and $I(z)=1/z$ on the [Riemann sphere](riemann-surfaces.md#riemann-sphere). For $F(z)=(az+b)/(cz+d)$ and $\Delta=ad-bc\ne0$, $c=0$ gives $F=T_{b/d}\circ S_{a/d}$. If $c\ne0$, division gives $F=T_{a/c}\circ S_{-\Delta/c^2}\circ I\circ T_{d/c}$. The expressions agree at poles and at infinity by the sphere conventions. These elementary maps therefore generate the [Möbius transformation](#mobius-transformation) group.

<h4 id="antipodal-fixed-point-classification-of-mobius-transformations">Antipodal fixed-point classification of Möbius transformations</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

For a nonidentity [Möbius transformation](#mobius-transformation) whose two fixed points are antipodal under [stereographic projection](riemann-surfaces.md#stereographic-projection), conjugate by a sphere rotation sending them to $0,\infty$. The conjugated map fixes both, hence is $z\mapsto az$ with $a\ne0$. If $|a|=1$ it is an axial rotation; if $|a|<1$ every finite orbit tends to zero; if $|a|>1$ every nonzero orbit tends to infinity. Undoing the rotation gives either a sphere rotation or one attracting fixed point with the other as the sole exceptional initial point.

<h4 id="mobius-conjugacy-normal-forms">Möbius conjugacy normal forms</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

A nonidentity [Möbius transformation](#mobius-transformation) has one or two distinct [fixed points](function.md#fixed-point) on the [Riemann sphere](riemann-surfaces.md#riemann-sphere). If there are two, send them to zero and infinity; the conjugated map fixes both and is a nonzero scaling. If there is one, send it to infinity; the resulting affine map cannot have slope different from one, since that would give another fixed point. It is a nonzero translation, which a scaling conjugates to $z+1$. The identity is the scaling $\mu=1$. Fixed-point sets are carried bijectively under conjugacy, so a translation is not conjugate to a scaling.

<h5 id="iteration-of-a-one-fixed-point-mobius-transformation">Iteration of a one-fixed-point Möbius transformation</h5>

↑ **Parent:** [Möbius conjugacy normal forms](#mobius-conjugacy-normal-forms)

A nonidentity [Möbius transformation](#mobius-transformation) with only one [fixed point](function.md#fixed-point) is conjugate to a nonzero translation of the [Riemann sphere](riemann-surfaces.md#riemann-sphere). Its translation iterates are $z+nb$, tending to infinity in the topology of the [Riemann sphere](riemann-surfaces.md#riemann-sphere) for finite $z$, with infinity itself fixed. Conjugating back proves that every point tends to the unique [fixed point](function.md#fixed-point). This is convergence on the [sphere](euclidean-geometry.md#sphere); if the [fixed point](function.md#fixed-point) is finite, intermediate iterates can still pass through infinity.

<h5 id="finite-order-mobius-orbit-sizes">Finite-order Möbius orbit sizes</h5>

↑ **Parent:** [Möbius conjugacy normal forms](#mobius-conjugacy-normal-forms)

A nonidentity [Möbius transformation](#mobius-transformation) of finite order $n$ is conjugate to multiplication by a primitive $n$th [root of unity](algebra.md#root-of-unity). Zero and infinity are fixed; for any other point, a return after $k$ iterates requires $\mu^k=1$, whose least positive solution is $n$. Thus its only orbit sizes are one and $n$. For the identity, every orbit has size one. This is a direct orbit computation, independent of an appeal to the orbit-stabilizer theorem.

#### Cayley transform (complex analysis)

↑ **Parent:** [Möbius transformation](#mobius-transformation)

This [Möbius transformation](#mobius-transformation) maps the [upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) onto the [unit disk](euclidean-geometry.md#unit-disk). For $\operatorname{Im}z>0$, the identity $1-|C(z)|^2=4\operatorname{Im}z/|z+i|^2$ puts the image inside the [unit disk](euclidean-geometry.md#unit-disk). Its inverse is $z=i(1+w)/(1-w)$, so the map is a [conformal bijection](riemann-surfaces.md#biholomorphism). On the extended real boundary it maps onto the [unit circle](complex-analysis.md#complex-unit-circle). It is the scalar complex-analytic version of a Cayley map, rather than the matrix parametrization used in [Cayley transform](lie-theory.md#cayley-transform-lie-theory).

<h4 id="mobius-transformations-from-the-real-axis-to-the-unit-circle">Möbius transformations from the real axis to the unit circle</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

A nonconstant [Möbius transformation](#mobius-transformation) mapping the [real line](real-analysis.md#real-line) into the [unit circle](complex-analysis.md#complex-unit-circle) has the displayed form with $|\lambda|=1$ and $k$ nonreal. Indeed $|ax+b|^2=|cx+d|^2$ for real $x$ yields $|a|=|c|\ne0$, $|b/a|=|d/c|$ and $\operatorname{Re}(b/a)=\operatorname{Re}(d/c)$. Thus $d/c$ is $b/a$ or its [complex conjugate](complex-analysis.md#complex-conjugate); the first possibility makes the map constant, so the second is necessary. Conjugate numerator and denominator have equal modulus on the [real line](real-analysis.md#real-line), proving the converse as well.

<h4 id="mobius-scaling-generated-by-translations-and-reciprocal-inversion">Möbius scaling generated by translations and reciprocal inversion</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

Let $T_b(z)=z+b$ and $I(z)=1/z$ on the [Riemann sphere](riemann-surfaces.md#riemann-sphere). For $s\ne0$, direct composition gives the displayed identity. Every nonzero complex scaling $z\mapsto\lambda z$ is obtained by choosing $s^2=-\lambda$. Since translations, scalings and reciprocal inversion generate the [Möbius group](#mobius-group), translations and reciprocal inversion alone also generate it.

#### Blaschke factor

↑ **Parent:** [Möbius transformation](#mobius-transformation)

For $|w|<R$, this [Möbius transformation](#mobius-transformation) maps the radius-$R$ disc to the unit disc, vanishes at $w$ and has modulus one on the boundary. Expanding gives $|R^2-\overline wz|^2=R^2|z-w|^2$ when $|z|=R$; its [pole](isolated-singularity.md#pole) lies outside the disc. Dividing a [holomorphic function](holomorphic-function.md) by factors corresponding to its interior zeros removes those zeros without changing its boundary modulus. This gives a direct factorization proof of [Jensen's formula](holomorphic-function.md#jensen-s-formula).

#### Antipodal fixed points do not characterize sphere rotations

↑ **Parent:** [Möbius transformation](#mobius-transformation)

The [Möbius transformation](#mobius-transformation) $M(z)=(3z-1)/(3-z)$ fixes the [antipodal pair](euclidean-geometry.md#antipodal-pair) $1,-1$ under [stereographic projection](riemann-surfaces.md#stereographic-projection). But $M'(1)=2$, so it multiplies infinitesimal spherical lengths at that fixed point by two, as follows from the round line element $2|dz|/(1+|z|^2)$. It is not an [isometry](riemannian-geometry.md#isometry) and hence not a sphere [rotation](riemannian-geometry.md#rotation-mathematics). Fixing an [antipodal pair](euclidean-geometry.md#antipodal-pair) is therefore necessary for a nontrivial rotational [Möbius transformation](#mobius-transformation), but is not sufficient.

<h4 id="loxodromic-mobius-transformation">Loxodromic Möbius transformation</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

A [Möbius transformation](#mobius-transformation) with two distinct fixed points is conjugate to $z\mapsto az$. It is loxodromic when $|a|\ne1$; on three-dimensional [hyperbolic space](hyperbolic-geometry.md#hyperbolic-space) it translates along the axis joining its fixed points and rotates around that axis by $\arg a$. The positive-real multiplier case has no rotation and is also called hyperbolic. When listing elliptic, parabolic, hyperbolic and loxodromic as separate types, loxodromic refers to the remaining case with nonzero rotation. A determinant-one matrix with nonreal [trace](linear-algebra.md#matrix-trace) has reciprocal [eigenvalues](linear-operator-theory.md#eigenvalue) that are neither real nor of modulus one, so it supplies this latter case.

<h4 id="real-determinant-one-mobius-orbits">Real determinant-one Möbius orbits</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

The [special linear group](#special-linear-group) $SL_2(\mathbb R)$ acting by [Möbius transformations](#mobius-transformation) has exactly three [group orbits](group-action.md#orbit-group-theory) on the [Riemann sphere](riemann-surfaces.md#riemann-sphere): the extended real line and the two open half-planes. The identity $\operatorname{Im}((az+b)/(cz+d))=\operatorname{Im}z/|cz+d|^2$ preserves these sets. Upper triangular determinant-one matrices send $i$ to any prescribed point of the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), and similarly send $-i$ through the lower half-plane. The [stabilizer subgroups](group-action.md#stabilizer-subgroup) of $i$ and $-i$ are both $SO(2)$.

#### Concentric normalization of disjoint circles

↑ **Parent:** [Möbius transformation](#mobius-transformation)

Two disjoint ordinary [circle](topology.md#circle) boundaries can be taken to distinct concentric [circles](topology.md#circle) by a [Möbius transformation](#mobius-transformation). After their centres are put at $0,d$ with radii $a,b$, the map $(z-s)/(z-t)$ works when $st=a^2$ and $s+t=(d^2+a^2-b^2)/d$. Disjointness makes the quadratic have distinct real roots. Already concentric [circles](topology.md#circle) require no transformation.

#### Cross-ratio

↑ **Parent:** [Möbius transformation](#mobius-transformation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cross-ratio)

For four distinct points of the [Riemann sphere](riemann-surfaces.md#riemann-sphere), their cross-ratio is

$$
[z_1,z_2,z_3,z_4]
=\frac{(z_4-z_2)(z_1-z_3)}
{(z_4-z_3)(z_1-z_2)},
$$

with the evident limiting conventions at infinity. Every Möbius transformation preserves it.

##### Cross-ratio construction of generalized-circle reflection

↑ **Parent:** [Cross-ratio](#cross-ratio)

Normalize three distinct points on a [generalized circle](#generalized-circle-under-a-mobius-transformation) by a [Möbius transformation](#mobius-transformation) $f$ taking them to $1,0,\infty$. The inverse image of the extended real line is their generalized circle, and $J=f^{-1}\circ c\circ f$, with $c(z)=\overline z$, fixes that circle pointwise and squares to the identity. Changing the three normalizing points replaces $f$ by $M\circ f$ with a real-coefficient Möbius map $M$. Since $M$ commutes with conjugation, $J$ is unchanged. Thus this construction depends only on the circle. It is [inversion in a circle](#inversion-in-a-circle) for an ordinary circle and [Euclidean reflection](linear-algebra.md#reflection-mathematics) for a straight line, each extended to the [Riemann sphere](riemann-surfaces.md#riemann-sphere).

<h5 id="ptolemy-s-theorem">Ptolemy's theorem</h5>

↑ **Parent:** [Cross-ratio](#cross-ratio)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ptolemy's_theorem)

For four vertices in cyclic order on a circle, the product of the diagonal lengths is the sum of the products of opposite side lengths. One proof uses the [cross-ratio with second point mapped to zero](#cross-ratio-with-second-point-mapped-to-zero): its negative sign gives $|r|+1=|1-r|$, which becomes the displayed length relation.

<h5 id="mobius-invariance-of-the-cross-ratio">Möbius invariance of the cross-ratio</h5>

↑ **Parent:** [Cross-ratio](#cross-ratio)

Every [Möbius transformation](#mobius-transformation) preserves the [cross-ratio](#cross-ratio). The identity $M(u)-M(v)=(ad-bc)(u-v)/[(cu+d)(cv+d)]$ makes all extra factors cancel in the ratio; limiting conventions handle points at infinity.

##### Cross-ratio with second point mapped to zero

↑ **Parent:** [Cross-ratio](#cross-ratio)

This [cross-ratio](#cross-ratio) convention is the value of $z_3$ under the [Möbius transformation](#mobius-transformation) sending $z_1,z_2,z_4$ to $1,0,\infty$. It is one minus the convention $(z_1-z_3)(z_2-z_4)/[(z_1-z_2)(z_3-z_4)]$. Exchanging the first two points replaces $r$ by $1-r$. For four points in cyclic order on a circle, this convention gives $r<0$ and $1-r>1$.

##### Real cross-ratio criterion for a generalized circle

↑ **Parent:** [Cross-ratio](#cross-ratio)

Normalize three distinct points of the [Riemann sphere](riemann-surfaces.md#riemann-sphere) by a [Möbius transformation](#mobius-transformation) $f$ sending them to $\infty,0,1$. A fourth point lies on their [generalized circle](#generalized-circle-under-a-mobius-transformation) exactly when $f$ takes a real value there: the image of that [generalized circle](#generalized-circle-under-a-mobius-transformation) is the extended real line. Other standard [cross-ratio](#cross-ratio) ordering conventions differ by real fractional-linear transformations and preserve this reality criterion.

<h4 id="generalized-circle-under-a-mobius-transformation">Generalized circle under a Möbius transformation</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

A generalized circle is either a Euclidean circle or a straight line together with the point at infinity. Every Möbius transformation maps generalized circles to generalized circles. A Euclidean circle becomes a line exactly when it contains the pole, the preimage of infinity.

##### Reciprocal transformation of a generalized circle

↑ **Parent:** [Generalized circle under a Möbius transformation](#generalized-circle-under-a-mobius-transformation)

Write a [generalized circle](#generalized-circle-under-a-mobius-transformation) equation as $a|z|^2+b\bar z+\bar bz+c=0$, where $a,c$ are real. Under the reciprocal [Möbius transformation](#mobius-transformation) $z=1/w$, with $w\ne0$, multiply by $|w|^2$ to obtain

$$
c|w|^2+\bar b\bar w+bw+a=0.
$$

Thus the coefficient triple transforms as $(a,b,c)\mapsto(c,\bar b,a)$. A nondegenerate [circle](topology.md#circle) through zero has $c=0$ and becomes a [straight line](euclidean-geometry.md#straight-line); a [straight line](euclidean-geometry.md#straight-line) missing zero becomes a [circle](topology.md#circle) through zero on the [Riemann sphere](riemann-surfaces.md#riemann-sphere). When working only with finite nonzero coordinates, retain the excluded point $w=0$ even if it satisfies the multiplied equation.

This reciprocal transformation is different from [inversion in a circle](#inversion-in-a-circle), whose unit-circle formula is $z\mapsto1/\bar z$. The latter reverses [orientation](algebraic-topology.md#orientation-of-a-simplex); the reciprocal transformation is holomorphic away from its pole.

##### Inversion in a circle

↑ **Parent:** [Generalized circle under a Möbius transformation](#generalized-circle-under-a-mobius-transformation)

[Inversion in a circle](#inversion-in-a-circle) of centre $a$ and radius $R$ is an orientation-reversing involution of the [Riemann sphere](riemann-surfaces.md#riemann-sphere) fixing that circle pointwise and exchanging its interior and exterior. It is an anti-[Möbius transformation](#mobius-transformation). Reflection in a line is the corresponding inversion for a [generalized circle](#generalized-circle-under-a-mobius-transformation) through infinity. A composition of two such inversions is a [Möbius transformation](#mobius-transformation).

<h4 id="affine-subgroup-of-the-mobius-group">Affine subgroup of the Möbius group</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

The transformations that take every Euclidean circle to a Euclidean circle are precisely

$$
z\longmapsto az+b,\qquad a\ne0.
$$

They form the stabilizer of infinity in the Möbius group and are not a normal subgroup.

<h4 id="fixed-point-of-a-mobius-transformation">Fixed point of a Möbius transformation</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fixed_point_of_a_Möbius_transformation)

A fixed point of a Möbius transformation satisfies a quadratic equation on the Riemann sphere.

<h5 id="conjugation-of-a-mobius-transformation-with-two-distinct-fixed-points">Conjugation of a Möbius transformation with two distinct fixed points</h5>

↑ **Parent:** [Fixed point of a Möbius transformation](#fixed-point-of-a-mobius-transformation)

For $f(z)=(az+b)/(cz+d)$ with distinct finite [fixed points of a Möbius transformation](#fixed-point-of-a-mobius-transformation) $\alpha,\beta$, the fixed-point equation gives $f(z)-\alpha=(a-c\alpha)(z-\alpha)/(cz+d)$. Dividing the two identities gives $k=(a-c\alpha)/(a-c\beta)$, which is nonzero because $(a-c\alpha)(a-c\beta)=ad-bc\ne0$. The identities extend over the [Riemann sphere](riemann-surfaces.md#riemann-sphere). This conjugates the transformation to a dilation.

<h5 id="prescribed-fixed-points-of-a-mobius-transformation">Prescribed fixed points of a Möbius transformation</h5>

↑ **Parent:** [Fixed point of a Möbius transformation](#fixed-point-of-a-mobius-transformation)

For $f(z)=(az+b)/(z+1)$, the finite fixed points are the roots of

$$
z^2+(1-a)z-b=0.
$$

Thus a repeated fixed point or two prescribed fixed points determine $a$ and $b$ by the usual sum and product of roots.

<h5 id="fixed-points-of-a-finite-order-mobius-transformation">Fixed points of a finite-order Möbius transformation</h5>

↑ **Parent:** [Fixed point of a Möbius transformation](#fixed-point-of-a-mobius-transformation)

Every nonidentity finite-order Möbius transformation has exactly two fixed points on the Riemann sphere. A transformation with one repeated fixed point is conjugate to a nontrivial translation and therefore has infinite order.

<h4 id="constant-argument-locus-of-a-mobius-transformation">Constant-argument locus of a Möbius transformation</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

A condition $\arg((z-z_1)/(z-z_2))=\theta$ fixes the oriented angle subtended by $z_1,z_2$. Its locus is an arc of a circle through those two points, with the endpoints excluded.

<h4 id="classification-of-mobius-transformations-by-trace">Classification of Möbius transformations by trace</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Classification_of_Möbius_transformations_by_trace)

For determinant-one real representatives, trace magnitude below, equal to, or above two gives elliptic, parabolic, or hyperbolic type.

<h4 id="mobius-maps-commuting-with-reflection-in-the-unit-circle">Möbius maps commuting with reflection in the unit circle</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

The Möbius transformations commuting with $J(z)=1/\overline z$ are exactly

$$
z\longmapsto\frac{az+b}{\overline bz+\overline a},
\qquad |a|^2-|b|^2\ne0.
$$

They preserve the open unit disc exactly when $|a|>|b|$. The identity

$$
|az+b|^2-|\overline bz+\overline a|^2
=(|a|^2-|b|^2)(|z|^2-1)
$$

proves the latter assertion.

<h3 id="matrix-representative-of-a-mobius-transformation">Matrix representative of a Möbius transformation</h3>

↑ **Parent:** [Projective linear group](#projective-linear-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_representative_of_a_Möbius_transformation)

A Möbius transformation is represented by an invertible two-by-two matrix, with nonzero scalar multiples representing the same map.

## Semidirect product

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semidirect_product)

A semidirect product combines a normal subgroup with a subgroup acting on it by automorphisms.

### Central translations in a linear semidirect product

↑ **Parent:** [Semidirect product](#semidirect-product)

Let an [abelian group](group.md#abelian-group) $V$ carry an action $\rho$ of a [group](group.md) $H$ by automorphisms, and use multiplication $(h,v)(k,w)=(hk,v+\rho(h)w)$. Comparing $(e,v)(h,w)$ and $(h,w)(e,v)$ shows that a translation is central precisely when its vector is fixed by the entire action. If $H$ is itself abelian, the whole semidirect product is abelian exactly when the action is trivial. For $H=(\mathbb R,+)$, $V=\mathbb R^2$, and determinant-one linear actions fixing the first coordinate vector, $\rho(x)=\begin{pmatrix}1&r(x)\\0&1\end{pmatrix}$, where $r$ is an [additive function](analysis.md#additive-function). Without a regularity assumption, it need not be $r(x)=cx$.

### Finite presentation of a semidirect product

↑ **Parent:** [Semidirect product](#semidirect-product)

If $N=\langle A\mid R\rangle$ and $H=\langle B\mid S\rangle$ have [finite group presentations](geometric-group-theory.md#finite-group-presentation) and $\phi:H\to\operatorname{Aut}(N)$ is an action, choose a word $w_{b,a}(A)$ representing $\phi(b)(a)$. Then $N\rtimes_\phi H$ has the finite presentation

$$
\langle A,B\mid R,S,\ bab^{-1}=w_{b,a}(A)\ (a\in A,b\in B)\rangle.
$$

The action automorphisms also let these relations rewrite conjugation by inverse generators. Every word becomes an $A$-word followed by a $B$-word. The natural map to the [semidirect product](#semidirect-product) is injective because its triviality forces the $B$-word to be trivial using $S$ and then the $A$-word to be trivial using $R$.

### Coprime splitting over an elementary abelian normal subgroup

↑ **Parent:** [Semidirect product](#semidirect-product)

If $N$ is an elementary abelian normal subgroup and $|G/N|$ is prime to its characteristic, the extension splits and its complements are conjugate by $N$. In additive notation an extension cocycle satisfies $f(h,k)+f(hk,t)=h f(k,t)+f(h,kt)$. Averaging over $t$ gives $f(h,k)=b(h)+h b(k)-b(hk)$, where $b(h)=|G/N|^{-1}\sum_t f(h,t)$. Changing the section by $b$ removes the cocycle. For two complements the difference cocycle has $d(hk)=d(h)+h d(k)$; averaging gives $d(h)=b-hb$, which is conjugation by an element of $N$. These arguments use invertibility of the group order on $N$ and underlie Hall conjugacy in soluble groups.

### Twisted cyclic pair group

↑ **Parent:** [Semidirect product](#semidirect-product)

Let $p$ be prime, $a\in\mathbb F_p^\times$, $x,y\in\mathbb Z/(p-1)\mathbb Z$ and $u,v\in\mathbb F_p$. [Fermat's little theorem](number-theory.md#fermat-little-theorem) makes the displayed multiplication well defined. Its identity is $(0,0)$ and inverse is $(-x,-a^{-x}u)$; associativity follows by expanding both bracketings. Projection onto the first coordinate is a [group homomorphism](#group-homomorphism) with normal cyclic kernel of order $p$. Under the change $U=a^{-x}u$, multiplication becomes $(x,U)(y,V)=(x+y,U+a^{-x}V)$, the [semidirect product](#semidirect-product) of the additive prime field by the cyclic group of order $p-1$. The group is abelian precisely when $a=1$; $a$ need not be a generator of the multiplicative field group.

### Presentation of a semidirect product

↑ **Parent:** [Semidirect product](#semidirect-product)

Let $G=\langle S\mid R\rangle$ and $H=\langle T\mid U\rangle$ be [group presentations](geometric-group-theory.md#group-presentation), and let $\phi:H\to\operatorname{Aut}(G)$ be a [group homomorphism](#group-homomorphism). Choose a word $w_{t,s}(S)$ representing $\phi(t)(s)$ for each pair of generators. Then the [semidirect product](#semidirect-product) has presentation

$$
G\rtimes_\phi H=\langle S\sqcup T\mid R,U,\ tst^{-1}=w_{t,s}\ (t\in T,s\in S)\rangle.
$$

The cross-relations allow every word to be written in factor order $gh$, and the multiplication rule matches the prescribed action. The natural homomorphisms to and from the [semidirect product](#semidirect-product) are inverse on the generators. Finite factor presentations yield a [finite group presentation](geometric-group-theory.md#finite-group-presentation).

### Affine group of the complex line

↑ **Parent:** [Semidirect product](#semidirect-product)

The affine group of the complex line consists of the maps

$$
f_{a,b}(z)=az+b,
\qquad a\in\mathbb C^\times,\quad b\in\mathbb C.
$$

Composition identifies it with the [semidirect product](#semidirect-product) $(\mathbb C,+)\rtimes\mathbb C^\times$, where $a$ acts on a translation coordinate by multiplication.

#### Commutator subgroup of the affine group of the complex line

↑ **Parent:** [Affine group of the complex line](#affine-group-of-the-complex-line)

For the [Affine group of the complex line](#affine-group-of-the-complex-line),

$$
[G,G]=\{f_{1,b}:b\in\mathbb C\}\cong(\mathbb C,+),
\qquad G/[G,G]\cong\mathbb C^\times.
$$

Indeed, the multiplier map $f_{a,b}\mapsto a$ has the displayed translation group as its kernel and abelian image, while

$$
[f_{a,1},f_{1,b}]=f_{1,b(1-a^{-1})}
$$

produces every translation.

### Wreath product

↑ **Parent:** [Semidirect product](#semidirect-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wreath_product)

The restricted wreath product of groups $H$ and $G$ is

$$
H\wr G=\left(\bigoplus_{g\in G}H_g\right)\rtimes G,
$$

where $G$ acts on the finitely supported functions $G\to H$ by translation.

#### Product action of a wreath product

↑ **Parent:** [Wreath product](#wreath-product)

The base group acts independently on each coordinate of a Cartesian power, and the top group permutes coordinates. This is distinct from the imprimitive action on a disjoint union of blocks. It is primitive when the base action is primitive and nonregular and the top group is transitive. The full product-action overgroup is $S_{|\Delta|}\wr S_r$. Socles of almost-simple, diagonal or holomorph bases produce respectively product-action, compound-diagonal or holomorph-compound types.

#### Permutation wreath product

↑ **Parent:** [Wreath product](#wreath-product)

If a [group](group.md) $K$ acts on a finite set $X$, it acts on the [direct product of groups](#direct-product-of-groups) $H^X$ by permuting its factors. The resulting [semidirect product](#semidirect-product) is the permutation wreath product. For $K=S_m$ acting on $m$ two-point blocks and $H=C_2$, it describes independent within-block swaps combined with a permutation of blocks, and has order $2^m m!$. The action on $X$ is part of the definition; it need not be the regular action used in a regular [wreath product](#wreath-product).

#### Lamplighter group

↑ **Parent:** [Wreath product](#wreath-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lamplighter_group)

The lamplighter group is the restricted wreath product $C_2\wr\mathbb Z$. It is generated by one lamp switch and the translation of the integer line.

### Abelianization of a semidirect product by the integers

↑ **Parent:** [Semidirect product](#semidirect-product)

Let $B\in\operatorname{GL}_d(\mathbb Z)$ and $\Gamma_B=\mathbb Z^d\rtimes_B\mathbb Z$. If $t$ generates the second factor, then the elements $tnt^{-1}n^{-1}$ fill $(B-I)\mathbb Z^d$, and hence

$$
\Gamma_B^{\mathrm{ab}}\cong
\mathbb Z\oplus\mathbb Z^d/(B-I)\mathbb Z^d.
$$

If $1$ is not an [eigenvalue](linear-operator-theory.md#eigenvalue) of $B$, the second summand is finite.

### Affine group over a finite field

↑ **Parent:** [Semidirect product](#semidirect-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affine_group_over_a_finite_field)

The one-dimensional affine group over $\mathbb F_q$ consists of maps $x\mapsto ax+b$ with $a\ne0$.

#### Involution orbits in an affine group of odd prime degree

↑ **Parent:** [Affine group over a finite field](#affine-group-over-a-finite-field)

A nonidentity [involution](#involution) in the [affine group over a finite field](#affine-group-over-a-finite-field) $\mathbb F_\ell$, for odd prime $\ell$, has linear coefficient $-1$: a translation has order $\ell$, while $u^2=1$ forces $u=\pm1$. Its unique fixed point is $b/2$, and its remaining orbits have size two. This orbit count computes [primes in an intermediate field as double cosets](non-archimedean-analysis.md#primes-in-an-intermediate-field-as-double-cosets) for an order-two [decomposition group](non-archimedean-analysis.md#decomposition-group) acting on the radical roots.

// Target: number-theory.bigb

#### Affine Galois group of a prime-radical splitting field

↑ **Parent:** [Affine group over a finite field](#affine-group-over-a-finite-field)

For distinct or equal [prime numbers](prime-number.md) $\ell,\lambda$, the polynomial $X^\ell-\lambda$ is [Eisenstein](commutative-algebra.md#eisenstein-criterion) at $\lambda$. Its [splitting field](galois-theory.md#splitting-field) over $\mathbb Q(\zeta_\ell)$ has [Galois group](galois-theory.md#galois-group) a subgroup of $C_\ell$, which is nontrivial because a degree-$\ell$ radical cannot belong to a degree-$(\ell-1)$ [cyclotomic field](galois-theory.md#cyclotomic-field). Thus the full [Galois group](galois-theory.md#galois-group) has order $\ell(\ell-1)$. On roots indexed by $j\in\mathbb F_\ell$, all automorphisms act as $j\mapsto uj+b$. Equality of orders identifies the group with the full [affine group over a finite field](#affine-group-over-a-finite-field).

// Target: algebra.bigb

#### Affine Galois group of the splitting field of x to the p minus two

↑ **Parent:** [Affine group over a finite field](#affine-group-over-a-finite-field)

For an odd prime $p$, the splitting field

$$
\mathbb Q(\zeta_p,2^{1/p})
$$

of $X^p-2$ has Galois group

$$
C_p\rtimes\mathbb F_p^\times
\cong\operatorname{AGL}_1(\mathbb F_p).
$$

The translation subgroup multiplies $2^{1/p}$ by powers of $\zeta_p$, while the multiplicative subgroup acts on $\zeta_p$ by cyclotomic automorphisms.

#### Affine semidirect product of cyclic groups of orders eleven and five

↑ **Parent:** [Affine group over a finite field](#affine-group-over-a-finite-field)

Let $Q$ be the subgroup of nonzero squares in $\mathbb F_{11}^\times$. The affine maps

$$
x\longmapsto rx+b,
\qquad r\in Q,\quad b\in\mathbb F_{11},
$$

form the nonabelian semidirect product $C_{11}\rtimes C_5$, with multiplication

$$
(r,b)(s,c)=(rs,b+rc).
$$

##### Conjugacy classes in the affine semidirect product of orders eleven and five

↑ **Parent:** [Affine semidirect product of cyclic groups of orders eleven and five](#affine-semidirect-product-of-cyclic-groups-of-orders-eleven-and-five)

This group has seven conjugacy classes: the identity; two classes of five nonidentity translations, distinguished by square class of the translation parameter; and, for each of the four $r\in Q\setminus\{1\}$, one class $\{(r,b):b\in\mathbb F_{11}\}$ of size eleven.

## Virtually cyclic group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Virtually_cyclic_group)

A group is virtually cyclic when it has a cyclic subgroup of finite index. A finitely generated abelian group is virtually cyclic exactly when its free abelian rank is one.

## Solvable group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Solvable_group)

A solvable group has a subnormal series whose factor groups are abelian.

### Supersolvable group

↑ **Parent:** [Solvable group](#solvable-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supersolvable_group)

A finite group is supersolvable if it has a [normal series of a group](#normal-series-of-a-group) whose nontrivial factors are cyclic of prime order. This is stronger than solubility, because the individual terms must be normal in the ambient group. For instance, $A_4$ is soluble via its normal Klein four-group, but is not supersolvable: it has no normal subgroup of order two or three with which such a series could begin.

### Finitely generated soluble torsion groups are finite

↑ **Parent:** [Solvable group](#solvable-group)

A finitely generated [abelian group](group.md#abelian-group) whose elements all have finite order is finite. Induct on derived length for a finitely generated [soluble group](#solvable-group) with this property. Its [abelianization](#abelianization) is finite, so its [commutator subgroup](#commutator-subgroup) has finite index and is finitely generated by [Schreier's lemma](geometric-group-theory.md#schreier-s-lemma). That subgroup is soluble of smaller derived length and is still a [torsion group](#torsion-group), hence finite by induction. The ambient group is a finite extension of it and is finite.

### Virtually solvable group

↑ **Parent:** [Solvable group](#solvable-group)

A [group](group.md) is virtually solvable, or virtually soluble, when it contains a [solvable group](#solvable-group) as a [finite-index subgroup](group.md#finite-index-subgroup). This is preserved under [subgroups](group.md#subgroup), quotients and [group extensions](group-cohomology.md#group-extension). The extension proof can use a [finite-index characteristic soluble subgroup](#finite-index-characteristic-soluble-subgroup) of the kernel, followed by centralizing the resulting finite normal kernel. Finite generation is not required for these closure properties.

#### Finite-index characteristic soluble subgroup

↑ **Parent:** [Virtually solvable group](#virtually-solvable-group)

Every [virtually soluble group](#virtually-solvable-group) $K$ has a soluble [characteristic subgroup](algebra.md#characteristic-subgroup) of finite index. First take a soluble [normal subgroup](#normal-subgroup) $K_0$ of finite index by the [subgroup core](#core-group-theory) construction. Choose a soluble normal subgroup $R\supseteq K_0$ maximizing its image size in the finite quotient $K/K_0$. For every soluble normal subgroup $S$, the product $RS$ is soluble, because its quotient by $R$ is a quotient of $S$. Maximality forces $S\leq R$. Hence $R$ is the unique largest soluble normal subgroup and is invariant under all [automorphisms](algebra.md#automorphism). This avoids incorrectly intersecting infinitely many conjugates when proving closure under [group extensions](group-cohomology.md#group-extension).

### Derived series

↑ **Parent:** [Solvable group](#solvable-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Derived_series)

The derived series is defined by

$$
G^{(0)}=G,\qquad G^{(n+1)}=[G^{(n)},G^{(n)}].
$$

A group is [solvable](#solvable-group) exactly when this series reaches the trivial group after finitely many steps.

### Metabelian group

↑ **Parent:** [Solvable group](#solvable-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Metabelian_group)

A group is metabelian when its [commutator subgroup](#commutator-subgroup) is [abelian](group.md#abelian-group), equivalently when its derived length is at most two.

#### Finite metabelian groups are monomial

↑ **Parent:** [Metabelian group](#metabelian-group)

Let $L\triangleleft G$ and both $L,G/L$ be abelian. For an irreducible $G$-module, choose a subgroup $A\supseteq L$ of maximal order whose restriction contains a [linear character](representation-theory.md#linear-character) $\varphi$. Every subgroup containing $L$ is normal. If an element $x\notin A$ stabilizes $\varphi$, its action on the nonzero $\varphi$-[isotypic component](module-theory.md#isotypic-component) has an eigenvector; that line is invariant under $\langle A,x\rangle$ and affords a larger linear constituent, contradicting maximality. Thus $I_G(\varphi)=A$, and the [Clifford correspondence](representation-theory.md#clifford-correspondence) gives $\chi=\varphi^G$.

### Polycyclic group

↑ **Parent:** [Solvable group](#solvable-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polycyclic_group)

A group is polycyclic when it has a subnormal series with cyclic factors. Every subgroup and quotient of a polycyclic group is finitely generated, and extensions of polycyclic groups are polycyclic.

#### Polycyclic groups are virtually poly-infinite cyclic

↑ **Parent:** [Polycyclic group](#polycyclic-group)

Every [polycyclic group](#polycyclic-group) has a finite-index subgroup with a series whose nontrivial factors are infinite cyclic. This is the polycyclic finite-index lemma; it also supplies torsion-free finite-index subgroups. Such a subgroup is a [poly-infinite cyclic group](#poly-infinite-cyclic-group). Combining its series with the extension rule for [Poincare duality groups](group-cohomology.md#poincare-duality-group) makes it a duality group of dimension its [Hirsch length](#hirsch-length).

#### Hirsch length

↑ **Parent:** [Polycyclic group](#polycyclic-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hirsch_length)

The Hirsch length of a [polycyclic group](#polycyclic-group) counts infinite cyclic factors in a polycyclic series. Refinement shows it is independent of the series, additive in extensions, and unchanged in finite-index subgroups. A finite-index [poly-infinite cyclic group](#poly-infinite-cyclic-group) has one infinite cyclic factor for each unit of Hirsch length.

#### Poly-infinite cyclic group

↑ **Parent:** [Polycyclic group](#polycyclic-group)

A poly-infinite cyclic group has a finite subnormal series all of whose nontrivial factors are [infinite cyclic groups](group.md#infinite-cyclic-group). Intersecting its series with a subgroup again gives trivial or infinite cyclic factors; repetitions may be deleted. Splicing a kernel series with the preimage of a quotient series proves closure under extensions. Such groups are [finitely presented groups](geometric-group-theory.md#finitely-presented-group): induct on the series, split the last extension by an infinite cyclic quotient, and use [finite presentation of a semidirect product](#finite-presentation-of-a-semidirect-product).

### Nilpotent group

↑ **Parent:** [Solvable group](#solvable-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nilpotent_group)

A group is nilpotent when it has a finite central series, equivalently when its lower central series reaches the identity.

#### Nilpotence criterion for an abelian-by-cyclic group

↑ **Parent:** [Nilpotent group](#nilpotent-group)

For $tvt^{-1}=Bv$, the commutator $[t,v]$ is $(B-I)v$ in additive notation. The lower central series from its second term is $(B-I)\mathbb Z^r,(B-I)^2\mathbb Z^r,\ldots$. It terminates exactly when $B-I$ is a [nilpotent matrix](linear-operator-theory.md#nilpotent-matrix). For rank two this means $(B-I)^2=0$, equivalently $\det B=1$ and $\operatorname{tr}B=2$. Nilpotence of a finite-index subgroup alone gives virtual nilpotence of the whole group.

#### Malcev completion of a torsion-free nilpotent group

↑ **Parent:** [Nilpotent group](#nilpotent-group)

Every finitely generated [torsion-free group](group.md#torsion-free-group) which is a [nilpotent group](#nilpotent-group) embeds as a discrete cocompact subgroup of a unique simply connected nilpotent real [Lie group](lie-theory.md#lie-group). Its dimension equals the group's [integral cohomological dimension of a group](group-cohomology.md#integral-cohomological-dimension-of-a-group). In dimension three the Lie algebra is either abelian or has a basis with a single nonzero bracket $[Y,T]=X$, giving the [real Heisenberg group](lie-algebra.md#heisenberg-group).

#### Commutator collection with fixed generators in nilpotent groups

↑ **Parent:** [Nilpotent group](#nilpotent-group)

If a [nilpotent group](#nilpotent-group) is generated by $a_1,\ldots,a_d$, every element of its [commutator subgroup](#commutator-subgroup) is a product $[x_1,a_1]\cdots[x_d,a_d]$. The sets in the displayed formula need not be [subgroups](group.md#subgroup). Induct on the nilpotency class $c$. Collection in $G/\gamma_c(G)$ gives the desired product with a central error. Since $\gamma_c(G)=[\gamma_{c-1}(G),G]$, that error is a product $[y_1,a_1]\cdots[y_d,a_d]$ with $y_i\in\gamma_{c-1}(G)$. These factors are central, and $\gamma_{c-1}(G)$ centralizes $G\prime$, so replacing $x_i$ by $x_iy_i$ absorbs the error. For a finitely generated [pro-p group](topological-group.md#pro-p-group), applying this formula in all finite quotients and using compactness makes its algebraically generated [commutator subgroup](#commutator-subgroup) closed.

#### Fixed-generator commutator collection in nilpotent groups

↑ **Parent:** [Nilpotent group](#nilpotent-group)

If a [nilpotent group](#nilpotent-group) is generated by $a_1,\ldots,a_d$, every element of its [commutator subgroup](#commutator-subgroup) is a product $[x_1,a_1]\cdots[x_d,a_d]$. The sets in the displayed formula need not be [subgroups](group.md#subgroup). Induct on the nilpotency class $c$. Collection in $G/\gamma_c(G)$ gives the desired product with a central error. Since $\gamma_c(G)=[\gamma_{c-1}(G),G]$, that error is a product $[y_1,a_1]\cdots[y_d,a_d]$ with $y_i\in\gamma_{c-1}(G)$. These factors are central, and $\gamma_{c-1}(G)$ centralizes $G\prime$, so replacing $x_i$ by $x_iy_i$ absorbs the error. For a finitely generated [pro-p group](topological-group.md#pro-p-group), applying this formula in all finite quotients and using compactness makes its algebraically generated [commutator subgroup](#commutator-subgroup) closed.

#### Finite nilpotent group decomposition

↑ **Parent:** [Nilpotent group](#nilpotent-group)

A finite group is nilpotent exactly when it is the [direct product of groups](#direct-product-of-groups) of its [Sylow subgroups](finite-group-theory.md#sylow-subgroup). The [normalizer condition for nilpotent groups](#normalizer-condition-for-nilpotent-groups) and Sylow conjugacy force each Sylow normalizer to be the whole group. Distinct normal Sylow subgroups commute because their commutators lie in their trivial intersection. Conversely finite p-groups are nilpotent by the nontrivial center and induction; direct products preserve nilpotence.

#### Normalizer condition for nilpotent groups

↑ **Parent:** [Nilpotent group](#nilpotent-group)

Choose the first term of the [upper central series](#upper-central-series) not contained in $H$. The preceding term lies in $H$, so an element of the new term outside $H$ commutes with $H$ modulo that preceding term and normalizes $H$.

#### Upper central series

↑ **Parent:** [Nilpotent group](#nilpotent-group)

Repeatedly take the [center of a group](#center-of-a-group) after quotienting by the preceding term. A [group](group.md) is a [nilpotent group](#nilpotent-group) exactly when a finite term is the whole group. This yields the [normalizer condition for nilpotent groups](#normalizer-condition-for-nilpotent-groups).

#### Nilpotency class

↑ **Parent:** [Nilpotent group](#nilpotent-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nilpotency_class)

The nilpotency class of a [nilpotent group](#nilpotent-group) $G$ is the least nonnegative integer $s$ for which $\gamma_{s+1}(G)=\{1\}$ in the [lower central series](#lower-central-series). Thus nontrivial [abelian groups](group.md#abelian-group) have class one.

##### Nilpotency class of a direct product

↑ **Parent:** [Nilpotency class](#nilpotency-class)

[Group commutators](group.md#group-commutator) are taken coordinatewise in a [direct product of groups](#direct-product-of-groups), giving $\Gamma_j(A\times B)=\Gamma_j(A)\times\Gamma_j(B)$. A finite direct product of [nilpotent groups](#nilpotent-group) is nilpotent, with class the maximum of the factor classes.

// Target: algebra.bigb

#### Two-step nilpotent group

↑ **Parent:** [Nilpotent group](#nilpotent-group)

A group $G$ is two-step nilpotent when

$$
[[G,G],G]=\{1\}.
$$

Equivalently, its [commutator subgroup](#commutator-subgroup) is contained in the [center of a group](#center-of-a-group) of $G$. This allows every word to be collected into powers of generators followed by powers of their pairwise commutators.

##### Word collection in a two-step nilpotent group

↑ **Parent:** [Two-step nilpotent group](#two-step-nilpotent-group)

In a two-generated [two-step nilpotent group](#two-step-nilpotent-group), use $c=[x,y]=x^{-1}y^{-1}xy$. Centrality of $c$ gives $yx=xyc^{-1}$, so every word collects to $x^ay^bc^r$. The multiplication of these collected expressions is $(a,b,r)(a',b',r')=(a+a',b+b',r+r'-a'b)$. Relations on the central commutator can reduce $r$ modulo its order. To turn collection into a [word problem for a group](geometric-group-theory.md#word-problem-for-groups) algorithm, one must also prove the independence of the remaining coordinates, for example by constructing a group with that cocycle multiplication.

#### Virtually nilpotent group

↑ **Parent:** [Nilpotent group](#nilpotent-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Virtually_nilpotent_group)

A group is virtually nilpotent when it has a nilpotent subgroup of finite index.

#### Lower central series

↑ **Parent:** [Nilpotent group](#nilpotent-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lower_central_series)

The lower central series of a group is defined by $\gamma_1(G)=G$ and $\gamma_{i+1}(G)=[\gamma_i(G),G]$. A group is nilpotent of class at most $c$ exactly when $\gamma_{c+1}(G)$ is trivial.

##### Bounded-exponent finitely generated nilpotent group order bound

↑ **Parent:** [Lower central series](#lower-central-series)

Let $G$ be a [nilpotent group](#nilpotent-group) of class at most $s$ in which every element has order at most $r$. A subgroup generated by $k$ elements has order at most

$$
r^{sk^s}.
$$

Indeed, collection by the [lower central series](#lower-central-series) expresses every element as an ordered product of simple [group commutators](group.md#group-commutator) in the generators of weights at most $s$. There are at most $k+k^2+\cdots+k^s\leq sk^s$ such commutators, and each exponent may be reduced to one of at most $r$ values.

#### Free nilpotent group

↑ **Parent:** [Nilpotent group](#nilpotent-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Free_nilpotent_group)

The free nilpotent group of rank $r$ and class $c$ is $F_r/\gamma_{c+1}(F_r)$, where $F_r$ is the free group of rank $r$ and $\gamma_i$ is its lower central series.

<h5 id="central-nonsplit-extension-of-the-integer-heisenberg-group-by-mathbb-z-2">Central nonsplit extension of the integer Heisenberg group by <span class="katex"><span class="katex-html" aria-hidden="true"><span class="base"><span class="strut" style="height:0.8141em;"></span><span class="mord"><span class="mord mathbb">Z</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height:0.8141em;"><span style="top:-3.063em;margin-right:0.05em;"><span class="pstrut" style="height:2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight">2</span></span></span></span></span></span></span></span></span></span></span></h5>

↑ **Parent:** [Free nilpotent group](#free-nilpotent-group)

The quotient map

$$
F_2/\gamma_4(F_2)\longrightarrow F_2/\gamma_3(F_2)
$$

is a central nonsplit extension of the [Integer Heisenberg group](lie-algebra.md#integer-heisenberg-group) by $\gamma_3(F_2)/\gamma_4(F_2)\cong\mathbb Z^2$. It cannot split because the source has abelianization $\mathbb Z^2$, whereas a central splitting would give an abelianization containing an additional direct factor $\mathbb Z^2$.

#### Central series

↑ **Parent:** [Nilpotent group](#nilpotent-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Central_series)

A central series is a chain of normal subgroups whose successive quotients lie in the centers of the corresponding quotient groups.

##### Central-series comparison theorem

↑ **Parent:** [Central series](#central-series)

For a length-$r$ [central series](#central-series) $1=G_0\le\cdots\le G_r=G$, induction from the top gives $\Gamma_{r-i+1}(G)\le G_i$, and induction from the bottom gives $G_i\le Z_i(G)$. Consequently the [lower central series](#lower-central-series) terminates at $\Gamma_{c+1}=1$ exactly when the [upper central series](#upper-central-series) reaches $Z_c=G$.

// Target: algebra.bigb

## Exponential growth of a group

↑ **Parent:** [Group theory](group-theory.md)

A finitely generated group has exponential growth when the number of elements represented by words of length at most $n$ is bounded below by $c^n$ for some $c>1$ and all sufficiently large $n$. The property is independent of the chosen finite generating set.

## Exponent of a finite group

↑ **Parent:** [Group theory](group-theory.md)

The exponent of a finite group is the least common multiple of the orders of all its elements.

Every [finite group](group.md#finite-group) is a [torsion group](#torsion-group); its exponent is a common multiple of the [order of a group element](#order-of-a-group-element) for every element.

### Finite group of prime exponent has prime-power order

↑ **Parent:** [Exponent of a finite group](#exponent-of-a-finite-group)

If every nonidentity element of a [finite group](group.md#finite-group) has order equal to a prime $p$, its order is a power of $p$. For any prime divisor $q$ of the [group](group.md) order, [Cauchy theorem for groups](finite-group-theory.md#cauchy-theorem-for-groups) gives an element of order $q$, forcing $q=p$. This statement does not imply that the [group](group.md) is abelian; odd-characteristic [upper unitriangular groups](finite-group-theory.md#upper-unitriangular-group) provide counterexamples.

### Finite subgroup of a field multiplicative group is cyclic

↑ **Parent:** [Exponent of a finite group](#exponent-of-a-finite-group)

Every finite subgroup of $K^\times$ is cyclic. If its exponent is $m$, all its elements are roots of $X^m-1$, so its size is at most $m$; finite abelian group theory supplies an element of order $m$, forcing equality.

## Order of an element of a finite group

↑ **Parent:** [Group theory](group-theory.md)

The order of an element is the least positive power equal to the identity and divides the order of a finite group.

This is the [order of a group element](#order-of-a-group-element) in the finite setting, one use of [order (group theory)](#order-group-theory).

## Order (group theory)

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Order_(group_theory))

In [group theory](group-theory.md), order can mean the cardinality of a [group](group.md) or the least positive $n$ for which a [group element](group.md#group-element) $g$ satisfies $g^n=e$. If no such $n$ exists, the element has infinite order. For a [finite group](group.md#finite-group), [Lagrange's theorem](#lagrange-s-theorem) implies that each element order divides the group order.

## ↑ Ancestors (4)

1. [Algebra](algebra.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Camille Jordan](mathematics.md#camille-jordan)
- [Fermat little theorem](number-theory.md#fermat-little-theorem)
- [Fiber of a function](function.md#fiber-of-a-function)
- [Order (group theory)](#order-group-theory)
- [Otto Hölder](mathematics.md#otto-holder)
