# Group theory

↑ **Parent:** [Algebra](algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_theory)

Group theory studies groups, homomorphisms, actions, quotients, and symmetry.

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
  - [Identity element](group.md#identity-element)
  - [Inverse element](group.md#inverse-element)
  - [Group operation](group.md#group-operation)
    - [Associative property](group.md#associative-property)
    - [Group commutator](group.md#group-commutator)
      - [Hall-Witt identity](group.md#hall-witt-identity)
      - [Hall-Petrescu formula](group.md#hall-petrescu-formula)
  - [Translation in a group](group.md#translation-in-a-group)
  - [Cyclic group](group.md#cyclic-group)
    - [Subgroups and quotients of a cyclic group](group.md#subgroups-and-quotients-of-a-cyclic-group)
    - [Free translation action on nontrivial subsets of a prime cyclic group](group.md#free-translation-action-on-nontrivial-subsets-of-a-prime-cyclic-group)
    - [Cyclic subgroup](group.md#cyclic-subgroup)
      - [Counting cyclic subgroups by their generators](group.md#counting-cyclic-subgroups-by-their-generators)
    - [Finite cyclic group](group.md#finite-cyclic-group)
      - [Homomorphism from a finite cyclic group](group.md#homomorphism-from-a-finite-cyclic-group)
    - [Infinite cyclic group](group.md#infinite-cyclic-group)
    - [Finite subgroup of the multiplicative complex numbers](group.md#finite-subgroup-of-the-multiplicative-complex-numbers)
    - [Generator of a group](group.md#generator-of-a-group)
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
  - [Cyclicity of a product of two finite cyclic groups](#cyclicity-of-a-product-of-two-finite-cyclic-groups)
  - [Order of a direct-product element](#order-of-a-direct-product-element)
  - [Restricted direct sum of groups](#restricted-direct-sum-of-groups)
  - [Internal direct product theorem](#internal-direct-product-theorem)
- [Metacyclic group](#metacyclic-group)
- [Commutator subgroup](#commutator-subgroup)
  - [Perfect group](#perfect-group)
    - [Perfectness of the special linear group](#perfectness-of-the-special-linear-group)
  - [Abelianization](#abelianization)
    - [Uniqueness of finite-index subgroups forces infinite cyclic abelianization](#uniqueness-of-finite-index-subgroups-forces-infinite-cyclic-abelianization)
      - [Residually finite group with one subgroup of each finite index is infinite cyclic](#residually-finite-group-with-one-subgroup-of-each-finite-index-is-infinite-cyclic)
    - [Abelianization of an odd dihedral group](#abelianization-of-an-odd-dihedral-group)
- [Center of a group](#center-of-a-group)
  - [Cyclic quotient by the center](#cyclic-quotient-by-the-center)
- [Conjugate subgroup](#conjugate-subgroup)
- [Group action](#group-action)
  - [n-transitive group action](#n-transitive-group-action)
  - [Symmetry enlargement under group translates](#symmetry-enlargement-under-group-translates)
  - [Subgroup factorization from coset transitivity](#subgroup-factorization-from-coset-transitivity)
  - [Circle action](#circle-action)
  - [Symmetry group](#symmetry-group)
  - [Finite support in a permutation action](#finite-support-in-a-permutation-action)
  - [Free action of a group](#free-action-of-a-group)
  - [Free group action](#free-group-action)
    - [Finite groups cannot act freely on Euclidean space](#finite-groups-cannot-act-freely-on-euclidean-space)
    - [Free actions on even-dimensional spheres have order at most two](#free-actions-on-even-dimensional-spheres-have-order-at-most-two)
    - [Free sphere actions exclude elementary abelian subgroups of rank two](#free-sphere-actions-exclude-elementary-abelian-subgroups-of-rank-two)
  - [Fundamental domain](#fundamental-domain)
  - [Multiply transitive group action](#multiply-transitive-group-action)
    - [Three-transitive group action](#three-transitive-group-action)
  - [Diagonal action on a centerless group](#diagonal-action-on-a-centerless-group)
  - [Ring of invariants](#ring-of-invariants)
    - [Normality of a ring of invariants](#normality-of-a-ring-of-invariants)
  - [Primitive group action](#primitive-group-action)
    - [Primitive group with a transposition](#primitive-group-with-a-transposition)
    - [Even primitive groups of safe-prime degree](#even-primitive-groups-of-safe-prime-degree)
    - [O'Nan–Scott theorem](#o-nan-scott-theorem)
      - [Diagonal primitive permutation group](#diagonal-primitive-permutation-group)
      - [Affine primitive permutation group](#affine-primitive-permutation-group)
        - [General affine group](#general-affine-group)
    - [Primitive three-cycle criterion](#primitive-three-cycle-criterion)
  - [Variable-permutation action on polynomials](#variable-permutation-action-on-polynomials)
  - [Fixed point of a group action](#fixed-point-of-a-group-action)
  - [Left regular action](#left-regular-action)
  - [Block system](#block-system)
    - [Uniform subdegrees force an imprimitive action to be Frobenius](#uniform-subdegrees-force-an-imprimitive-action-to-be-frobenius)
  - [Transitive group action](#transitive-group-action)
    - [Simply transitive group action](#simply-transitive-group-action)
    - [Regular group action](#regular-group-action)
    - [Derangement in a transitive group action](#derangement-in-a-transitive-group-action)
      - [Derangement counting formula](#derangement-counting-formula)
    - [Rank of a transitive permutation group](#rank-of-a-transitive-permutation-group)
    - [Regular permutation subgroup](#regular-permutation-subgroup)
      - [Centralizer of a regular permutation subgroup](#centralizer-of-a-regular-permutation-subgroup)
    - [Sharp t-transitivity](#sharp-t-transitivity)
      - [Sharp three-transitivity](#sharp-three-transitivity)
      - [Sharp two-transitivity](#sharp-two-transitivity)
      - [Regular kernel of a finite sharply two-transitive group](#regular-kernel-of-a-finite-sharply-two-transitive-group)
    - [One-point extension of a permutation group](#one-point-extension-of-a-permutation-group)
      - [Double-coset criterion for a one-point extension](#double-coset-criterion-for-a-one-point-extension)
    - [Prime-degree transposition criterion](#prime-degree-transposition-criterion)
  - [Two-transitive group action](#two-transitive-group-action)
    - [Elementary abelian regular kernels in doubly transitive groups](#elementary-abelian-regular-kernels-in-doubly-transitive-groups)
    - [Degree-ten partition action of S6](#degree-ten-partition-action-of-s6)
    - [Minimal normal subgroup dichotomy for two-transitive groups](#minimal-normal-subgroup-dichotomy-for-two-transitive-groups)
    - [Affine two-transitive group](#affine-two-transitive-group)
  - [Orbit map](#orbit-map)
  - [Equivariant map](#equivariant-map)
  - [Conjugation action](#conjugation-action)
    - [Conjugates of a proper subgroup do not cover a finite group](#conjugates-of-a-proper-subgroup-do-not-cover-a-finite-group)
    - [Conjugation](#conjugation)
      - [Conjugate subset](#conjugate-subset)
      - [Conjugate group elements](#conjugate-group-elements)
        - [Conjugate permutation](#conjugate-permutation)
    - [Conjugacy class](#conjugacy-class)
      - [Infinite conjugacy class group](#infinite-conjugacy-class-group)
      - [Torsion-freeness from one nonidentity conjugacy class](#torsion-freeness-from-one-nonidentity-conjugacy-class)
      - [Shortest conjugacy representative](#shortest-conjugacy-representative)
        - [Cyclic reduction of a shortest conjugacy representative](#cyclic-reduction-of-a-shortest-conjugacy-representative)
      - [Conjugacy class splitting in a prime-index normal subgroup](#conjugacy-class-splitting-in-a-prime-index-normal-subgroup)
        - [Alternating conjugacy class splitting criterion](#alternating-conjugacy-class-splitting-criterion)
          - [Inversion of an odd cycle in an alternating group](#inversion-of-an-odd-cycle-in-an-alternating-group)
      - [Class equation](#class-equation)
        - [Prime-to-p conjugacy class lemma](#prime-to-p-conjugacy-class-lemma)
    - [Centralizer and normalizer](#centralizer-and-normalizer)
      - [Centralizer](#centralizer)
        - [Centralizer of a subset](#centralizer-of-a-subset)
        - [Centraliser of a fixed-point-free involution](#centraliser-of-a-fixed-point-free-involution)
        - [Centraliser of a transposition](#centraliser-of-a-transposition)
      - [Normalizer](#normalizer)
        - [Normalizer of a diagonal subgroup of GL2](#normalizer-of-a-diagonal-subgroup-of-gl2)
  - [Orbit-stabilizer theorem](#orbit-stabilizer-theorem)
    - [Orbit dimension formula](#orbit-dimension-formula)
  - [Symmetry group of a cube](#symmetry-group-of-a-cube)
    - [Body-diagonal stabilizer in the cube symmetry group](#body-diagonal-stabilizer-in-the-cube-symmetry-group)
    - [Axial isotropy types of the full cube symmetry group](#axial-isotropy-types-of-the-full-cube-symmetry-group)
    - [Axis stabilizer in the full octahedral symmetry group](#axis-stabilizer-in-the-full-octahedral-symmetry-group)
    - [Cube symmetry action on edges](#cube-symmetry-action-on-edges)
    - [Direct-product decomposition of the cube symmetry group](#direct-product-decomposition-of-the-cube-symmetry-group)
    - [Rotational symmetry group of a cube](#rotational-symmetry-group-of-a-cube)
      - [Tetrahedron stabilizer in the cube rotation group](#tetrahedron-stabilizer-in-the-cube-rotation-group)
      - [Kernel of the cube face-axis action](#kernel-of-the-cube-face-axis-action)
      - [Face-pair orbits of cube rotations](#face-pair-orbits-of-cube-rotations)
  - [Faithful group action](#faithful-group-action)
    - [Normal subgroup orbits in a faithful prime-degree action](#normal-subgroup-orbits-in-a-faithful-prime-degree-action)
  - [Orbit of a group action](#orbit-of-a-group-action)
    - [Equality-pattern orbits of ordered pairs](#equality-pattern-orbits-of-ordered-pairs)
    - [Real rotation orbits on a complex unit quadric](#real-rotation-orbits-on-a-complex-unit-quadric)
    - [Equality-pattern orbits of projective triples](#equality-pattern-orbits-of-projective-triples)
  - [Stabilizer subgroup](#stabilizer-subgroup)
    - [Pointwise stabilizer](#pointwise-stabilizer)
    - [Axial subgroup](#axial-subgroup)
      - [Complex axial isotropy subgroup](#complex-axial-isotropy-subgroup)
  - [Symmetric group action on subsets](#symmetric-group-action-on-subsets)
  - [Coset action](#coset-action)
- [Coset](#coset)
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
  - [Product of commuting elements of coprime order](#product-of-commuting-elements-of-coprime-order)
  - [Infinite order](#infinite-order)
  - [Involution](#involution)
    - [Eigenspace decomposition of a linear involution](#eigenspace-decomposition-of-a-linear-involution)
      - [Involution exponential formula](#involution-exponential-formula)
- [Quotient group](#quotient-group)
  - [Subgroup correspondence for a surjective group homomorphism](#subgroup-correspondence-for-a-surjective-group-homomorphism)
  - [Finite quotient of a group](#finite-quotient-of-a-group)
  - [Abelian quotient](#abelian-quotient)
- [General linear group](#general-linear-group)
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
  - [Image of a group homomorphism](#image-of-a-group-homomorphism)
- [Automorphism group](#automorphism-group)
  - [Holomorph](#holomorph)
  - [Inner automorphism](#inner-automorphism)
  - [Outer automorphism group](#outer-automorphism-group)
    - [Outer automorphism of a group](#outer-automorphism-of-a-group)
- [Group cohomology](#group-cohomology)
  - [Cellular free resolution from a contractible universal cover](#cellular-free-resolution-from-a-contractible-universal-cover)
  - [Integral cohomological dimension of a group](#integral-cohomological-dimension-of-a-group)
    - [Stallings-Swan theorem](#stallings-swan-theorem)
  - [Poincare duality group](#poincare-duality-group)
    - [Normal finitely presented subgroups of three-dimensional duality groups](#normal-finitely-presented-subgroups-of-three-dimensional-duality-groups)
    - [Classification of two-dimensional Poincare duality groups](#classification-of-two-dimensional-poincare-duality-groups)
    - [Strebel infinite-index subgroup theorem](#strebel-infinite-index-subgroup-theorem)
    - [Extension rule for Poincare duality groups](#extension-rule-for-poincare-duality-groups)
    - [Finite-index invariance of Poincare duality for torsion-free groups](#finite-index-invariance-of-poincare-duality-for-torsion-free-groups)
  - [Mod-p cohomology ring of a cyclic group](#mod-p-cohomology-ring-of-a-cyclic-group)
  - [Dimension shifting in group cohomology](#dimension-shifting-in-group-cohomology)
  - [Tate cohomology of a finite group](#tate-cohomology-of-a-finite-group)
  - [Continuous cochains with topological coefficients](#continuous-cochains-with-topological-coefficients)
  - [Tate cohomology of a cyclic group](#tate-cohomology-of-a-cyclic-group)
    - [Cyclic cohomology of a regular lattice](#cyclic-cohomology-of-a-regular-lattice)
    - [Herbrand quotient](#herbrand-quotient)
      - [Herbrand quotient of a finite module](#herbrand-quotient-of-a-finite-module)
      - [Herbrand quotient of the local multiplicative group](#herbrand-quotient-of-the-local-multiplicative-group)
  - [Corestriction map in group cohomology](#corestriction-map-in-group-cohomology)
  - [Continuous cohomology of a profinite group](#continuous-cohomology-of-a-profinite-group)
    - [Cohomology continuity at closed subgroups](#cohomology-continuity-at-closed-subgroups)
    - [Cohomological dimension at a prime](#cohomological-dimension-at-a-prime)
      - [Trivial coefficients detect the cohomological dimension of a pro-p group](#trivial-coefficients-detect-the-cohomological-dimension-of-a-pro-p-group)
      - [Characteristic p Galois dimension bound](#characteristic-p-galois-dimension-bound)
  - [Nonabelian first cohomology](#nonabelian-first-cohomology)
  - [Periodic group cohomology](#periodic-group-cohomology)
    - [Cohomology ring of a finite cyclic group over its prime field](#cohomology-ring-of-a-finite-cyclic-group-over-its-prime-field)
    - [Periodic group cohomology from a free sphere action](#periodic-group-cohomology-from-a-free-sphere-action)
  - [Projective-resolution definition of group cohomology](#projective-resolution-definition-of-group-cohomology)
    - [Group cohomology commutes with finite direct sums](#group-cohomology-commutes-with-finite-direct-sums)
    - [Koszul resolution for a rank-two free abelian group](#koszul-resolution-for-a-rank-two-free-abelian-group)
      - [Second cohomology of a rank-two free abelian group with truncated group-ring coefficients](#second-cohomology-of-a-rank-two-free-abelian-group-with-truncated-group-ring-coefficients)
  - [Coinduced module](#coinduced-module)
    - [Shapiro's lemma](#shapiro-s-lemma)
      - [Hom functor adjunction for a coinduced module](#hom-functor-adjunction-for-a-coinduced-module)
  - [Conjugation module of a group ring](#conjugation-module-of-a-group-ring)
    - [Group cohomology of a conjugation module](#group-cohomology-of-a-conjugation-module)
  - [Integral cohomology of a finite cyclic group](#integral-cohomology-of-a-finite-cyclic-group)
    - [Periodic resolution of a finite cyclic group](#periodic-resolution-of-a-finite-cyclic-group)
  - [Group extension](#group-extension)
    - [Torsion-free finite extension of a lattice](#torsion-free-finite-extension-of-a-lattice)
    - [Split group extension](#split-group-extension)
      - [Section normal form for a split group extension](#section-normal-form-for-a-split-group-extension)
    - [Equivalent group extensions](#equivalent-group-extensions)
    - [Fiber product of groups](#fiber-product-of-groups)
      - [Mihailova subgroup](#mihailova-subgroup)
    - [Second group cohomology classifies group extensions](#second-group-cohomology-classifies-group-extensions)
      - [Integral central extensions of a rank-two free abelian group](#integral-central-extensions-of-a-rank-two-free-abelian-group)
      - [Extension cocycle](#extension-cocycle)
  - [Group cocycle](#group-cocycle)
    - [One-cocycle](#one-cocycle)
      - [Galois 1-cocycle](#galois-1-cocycle)
      - [Crossed homomorphism](#crossed-homomorphism)
        - [Principal crossed homomorphism](#principal-crossed-homomorphism)
    - [Two-cocycle](#two-cocycle)
      - [Normalized two-cocycle](#normalized-two-cocycle)
  - [Group coboundary](#group-coboundary)
  - [Group cochain](#group-cochain)
  - [Long exact sequence in group cohomology](#long-exact-sequence-in-group-cohomology)
  - [Finite-group cohomology is annihilated by the group order](#finite-group-cohomology-is-annihilated-by-the-group-order)
    - [Restriction-corestriction identity in group cohomology](#restriction-corestriction-identity-in-group-cohomology)
  - [Mac Lane exact sequence for a free presentation](#mac-lane-exact-sequence-for-a-free-presentation)
  - [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence)
    - [Cyclic-extension shift of group-ring cohomology](#cyclic-extension-shift-of-group-ring-cohomology)
    - [Five-term exact sequence in group cohomology](#five-term-exact-sequence-in-group-cohomology)
      - [Inflation-restriction exact sequence](#inflation-restriction-exact-sequence)
      - [Inflation map in group cohomology](#inflation-map-in-group-cohomology)
      - [Restriction map in group cohomology](#restriction-map-in-group-cohomology)
      - [Transgression in group cohomology](#transgression-in-group-cohomology)
    - [Integral cohomology of the dihedral group of order ten](#integral-cohomology-of-the-dihedral-group-of-order-ten)
- [Group homology](#group-homology)
  - [Homology of a finite cyclic group](#homology-of-a-finite-cyclic-group)
  - [Schur multiplier](#schur-multiplier)
    - [Hopf's formula](#hopf-s-formula)
    - [Schur multiplier of an abelian group](#schur-multiplier-of-an-abelian-group)
- [Finite group theory](finite-group-theory.md)
  - [Fitting subgroup](finite-group-theory.md#fitting-subgroup)
    - [Fitting subgroup is self-centralizing in soluble groups](finite-group-theory.md#fitting-subgroup-is-self-centralizing-in-soluble-groups)
    - [Fitting subgroup centralizes the socle](finite-group-theory.md#fitting-subgroup-centralizes-the-socle)
    - [Nilpotent normal subgroup](finite-group-theory.md#nilpotent-normal-subgroup)
    - [p-core](finite-group-theory.md#p-core)
  - [Classification of groups of order ten](finite-group-theory.md#classification-of-groups-of-order-ten)
  - [Almost simple group](finite-group-theory.md#almost-simple-group)
  - [Heisenberg group over a prime field](finite-group-theory.md#heisenberg-group-over-a-prime-field)
  - [Tetrahedral symmetry](finite-group-theory.md#tetrahedral-symmetry)
  - [Group of order eight](finite-group-theory.md#group-of-order-eight)
  - [Feit–Thompson theorem](finite-group-theory.md#feit-thompson-theorem)
  - [Alternating group](finite-group-theory.md#alternating-group)
    - [Maximal subgroups of A5](finite-group-theory.md#maximal-subgroups-of-a5)
    - [Automorphisms of alternating groups from triple supports](finite-group-theory.md#automorphisms-of-alternating-groups-from-triple-supports)
    - [Connected triple supports generate an alternating group](finite-group-theory.md#connected-triple-supports-generate-an-alternating-group)
    - [Conjugacy classes of the alternating group on six letters](finite-group-theory.md#conjugacy-classes-of-the-alternating-group-on-six-letters)
  - [P-group](finite-group-theory.md#p-group)
  - [Symmetric group](finite-group-theory.md#symmetric-group)
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

Let $p$ be the smallest prime dividing the order of a [finite group](group.md#finite-group), and suppose its [Sylow subgroup](finite-group-theory.md#sylow-subgroup) $P$ is cyclic of order $p^a$. [Conjugation](#conjugation) embeds $N_G(P)/C_G(P)$ into $\operatorname{Aut}(P)$, of order $p^{a-1}(p-1)$. Since $P\subseteq C_G(P)$, this quotient has order prime to $p$. Its remaining possible prime divisors are smaller than $p$ and cannot divide $|G|$. Thus $N_G(P)=C_G(P)$, and the [Burnside transfer theorem](#burnside-transfer-theorem) gives a [normal p-complement](#normal-p-complement).

<h2 id="prufer-rank">Prüfer rank</h2>

↑ **Parent:** [Group theory](group-theory.md)

The Prüfer rank bounds the number of [generators of a group](group.md#generator-of-a-group) needed for each finitely generated subgroup, without requiring the ambient group to be finitely generated. The additive [group](group.md) $\mathbb Q$ has Prüfer rank one: any finitely generated subgroup has a common denominator and is cyclic, but no finite collection generates all rational numbers. Prüfer rank cannot increase under taking subgroups or quotients; for quotients, lift a finite generating set and apply the rank bound to the subgroup generated by its lifts.

<h3 id="prufer-rank-bound-for-extensions">Prüfer rank bound for extensions</h3>

↑ **Parent:** [Prüfer rank](#prufer-rank)

For a [normal subgroup](#normal-subgroup) $N$ with [Prüfer rank](#prufer-rank) $r$ and quotient of rank $s$, let $H=\langle h_1,\ldots,h_k\rangle\le G$. Choose at most $s$ elements $x_j\in H$ generating the image of $H$. Write $h_i=w_i(x_1,\ldots,x_s)n_i$ with $n_i\in N\cap H$. The finitely generated subgroup $\langle n_1,\ldots,n_k\rangle$ needs at most $r$ generators, so $H$ needs at most $r+s$. The full intersection $H\cap N$ need not be finitely generated.

## Maximal condition on subgroups

↑ **Parent:** [Group theory](group-theory.md)

A [group](group.md) has the maximal condition on subgroups when every ascending sequence of [subgroups](group.md#subgroup) eventually stabilizes. Equivalently, every subgroup is a [finitely generated group](group.md#finitely-generated-group). If a subgroup were not finitely generated, repeatedly adjoining an element outside the previously generated subgroup would give a strictly ascending sequence. Conversely, generators of the union of an ascending sequence all lie in one term, making that term the whole union. This condition is preserved by [group extensions](#group-extension) because each subgroup is an extension of its intersection with the kernel by its image in the quotient.

## Group

↑ **Parent:** [Group theory](group-theory.md)

[This section is present in another page, follow this link to view it.](group.md)

## First isomorphism theorem

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/First_isomorphism_theorem)

For a group homomorphism $\phi:G\to H$, the map $g\ker\phi\mapsto\phi(g)$ gives an isomorphism

$$
G/\ker\phi\cong\operatorname{im}\phi.
$$

## Direct product of groups

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Direct_product_of_groups)

The direct product $G\times H$ has componentwise multiplication. An element $(g,h)$ of finite component orders has order $\operatorname{lcm}(\operatorname{ord}g,\operatorname{ord}h)$.

### Cyclicity of a product of two finite cyclic groups

↑ **Parent:** [Direct product of groups](#direct-product-of-groups)

Generators $a,b$ of the two [cyclic groups](group.md#cyclic-group) give a pair of order $\operatorname{lcm}(m,n)$. It generates the product precisely when this equals $mn$, namely when the orders are [coprime](number-theory.md#coprime-integers). If their greatest common divisor is larger than one, every element has order at most this smaller least common multiple, so no generator exists.

### Order of a direct-product element

↑ **Parent:** [Direct product of groups](#direct-product-of-groups)

If the two [group elements](group.md#group-element) have finite orders $m,n$, then $(g,h)^k=(1,1)$ exactly when both $m$ and $n$ divide $k$. Thus their pair has the displayed [order of a group element](#order-of-a-group-element). This elementary criterion detects when a finite product has a generator.

### Restricted direct sum of groups

↑ **Parent:** [Direct product of groups](#direct-product-of-groups)

The restricted direct sum of a family of [groups](group.md) $G_i$ is the subgroup of their [direct product of groups](#direct-product-of-groups) consisting of tuples with only finitely many nonidentity coordinates. Multiplication is coordinatewise. If every factor is a [finite group](group.md#finite-group), each [subgroup](group.md#subgroup) that is a [finitely generated group](group.md#finitely-generated-group) lies in a finite subproduct, so the restricted direct sum is a [locally finite group](#locally-finite-group). This gives concrete infinite [torsion groups](#torsion-group) without a uniform bound on element orders.

### Internal direct product theorem

↑ **Parent:** [Direct product of groups](#direct-product-of-groups)

If $H,K\trianglelefteq G$, $H\cap K=\{1\}$, and $HK=G$, then multiplication defines an isomorphism $H\times K\to G$. Conversely, the two canonical factors of a direct product satisfy these conditions.

## Metacyclic group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Metacyclic_group)

A group is metacyclic when it has a cyclic normal subgroup whose quotient is cyclic. Every [dihedral group](finite-group-theory.md#dihedral-group) is metacyclic through its rotation subgroup.

## Commutator subgroup

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Commutator_subgroup)

The commutator subgroup $G'$ is generated by all $[x,y]=x^{-1}y^{-1}xy$. It is characteristic, $G/G'$ is abelian, and every normal subgroup with abelian quotient contains $G'$.

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

The abelianization of a group is the quotient $G^{\mathrm{ab}}=G/G'$ by its [commutator subgroup](#commutator-subgroup). It is the largest abelian quotient of $G$.

#### Uniqueness of finite-index subgroups forces infinite cyclic abelianization

↑ **Parent:** [Abelianization](#abelianization)

If a finitely generated group $S$ has exactly one subgroup of each finite index, every such subgroup is normal. The quotients of prime order give surjections of its finitely generated abelianization onto $C_p$ for all primes, forcing positive free rank. A free rank of at least two gives two distinct index-$p$ subgroups. Positive finite torsion together with the free rank-one factor also gives two index-$p$ subgroups for a suitable prime. Hence $S_{\mathrm{ab}}\cong\mathbb Z$.

// Target: algebra.bigb

##### Residually finite group with one subgroup of each finite index is infinite cyclic

↑ **Parent:** [Uniqueness of finite-index subgroups forces infinite cyclic abelianization](#uniqueness-of-finite-index-subgroups-forces-infinite-cyclic-abelianization)

The epimorphism $S\to S_{\mathrm{ab}}\cong\mathbb Z$ has preimage of $n\mathbb Z$ as the unique index-$n$ subgroup. Thus every finite-index subgroup contains the commutator subgroup. Residual finiteness makes their intersection trivial, forcing the commutator subgroup to vanish and $S\cong\mathbb Z$.

// Target: geometry-and-topology.bigb

#### Abelianization of an odd dihedral group

↑ **Parent:** [Abelianization](#abelianization)

For odd $n\geq3$, the [dihedral group](finite-group-theory.md#dihedral-group) $D_{2n}$ of order $2n$ has rotation generator $r$ and reflection generator $s$, with $srs=r^{-1}$. The [group commutator](group.md#group-commutator) $[r,s]=r^{-2}$ generates the rotation [subgroup](group.md#subgroup), while the quotient by that [subgroup](group.md#subgroup) is $C_2$. Hence the [commutator subgroup](#commutator-subgroup) is exactly $\langle r\rangle$ and the [abelianization](#abelianization) is $C_2$. The only [abelian quotients](#abelian-quotient) are $C_2$ and the trivial group.

## Center of a group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Center_of_a_group)

The centre of a [group](group.md) is $Z(G)=\{z\in G:zg=gz\text{ for every }g\in G\}$. It is a [normal subgroup](#normal-subgroup). A nontrivial finite [p-group](finite-group-theory.md#p-group) has nontrivial centre: in the [class equation](#class-equation), each noncentral conjugacy class has size divisible by $p$, so $|Z(G)|\equiv|G|\equiv0\pmod p$.

### Cyclic quotient by the center

↑ **Parent:** [Center of a group](#center-of-a-group)

If $G/Z(G)$ is cyclic, then $G$ is abelian. Indeed, if $gZ(G)$ generates the quotient, every element is $g^az$ with $z\in Z(G)$, and any two such elements commute.

## Conjugate subgroup

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugate_subgroup)

## Group action

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_action)

### n-transitive group action

↑ **Parent:** [Group action](#group-action)

A [group action](#group-action) on a set is n-transitive when it can send any ordered tuple of $n$ distinct points to any other such tuple. Here ordered means a sequence of entries, not increasing in a [total order](set.md#total-order). For order-preserving actions the corresponding notion is [order n-transitivity](partially-ordered-group.md#order-n-transitivity).

### Symmetry enlargement under group translates

↑ **Parent:** [Group action](#group-action)

For a [group](group.md) of [Euclidean isometries](riemannian-geometry.md#euclidean-isometry), every element preserves the displayed union of images of a [set](set.md), because left multiplication permutes its [group](group.md) indices. Its full setwise [isometry group](riemannian-geometry.md#isometry-group) can be larger even when $T$ itself has no nonidentity symmetry. Take $G$ to be the [integer](number-theory.md#integer) [translations](geometry-and-topology.md#translation-geometry) of the plane and $T=\{(0,0),(1,0),(0,2)\}$. By [rigidity of a scalene triangle](riemannian-geometry.md#rigidity-of-a-scalene-triangle), $T$ has trivial [stabilizer subgroup](#stabilizer-subgroup). Yet $S=\mathbb Z^2$, whose quarter-turn about the origin is a symmetry outside the [translation](geometry-and-topology.md#translation-geometry) [group](group.md).

### Subgroup factorization from coset transitivity

↑ **Parent:** [Group action](#group-action)

In the right multiplication action, the orbit of the coset $H$ under $K$ is $\{Hk:k\in K\}$. It is the whole right coset space exactly when every $g$ has form $hk$, proving the displayed criterion. The factorization need not be unique; for finite groups $|HK|=|H||K|/|H\cap K|$.

### Circle action

↑ **Parent:** [Group action](#group-action)

A circle action is a [group action](#group-action) by $S^1$. Hamiltonian circle actions are especially useful in [symplectic reduction](symplectic-geometry.md#symplectic-reduction).

### Symmetry group

↑ **Parent:** [Group action](#group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetry_group)

The [group](group.md) of transformations preserving a specified geometric object or structure.

### Finite support in a permutation action

↑ **Parent:** [Group action](#group-action)

Suppose a permutation group $G$ acts on an underlying atom set $A$ and on a collection of objects built over it. A finite subset $S\subseteq A$ supports an object $x$ when every permutation fixing all members of $S$ fixes $x$. Pairing supported objects uses the union of their supports. A definable subset or functional image inherits a support from its domain and parameters. In a [hereditarily finite-supported Quine-atom model](set-theory.md#hereditarily-finite-supported-quine-atom-model), every member is recursively required to have such a support; symmetry then rules out a choice function on the pairs of atoms.

### Free action of a group

↑ **Parent:** [Group action](#group-action)

A [group action](#group-action) is free when only the identity fixes any given point, or equivalently every [stabilizer subgroup](#stabilizer-subgroup) is trivial. The trivial group acts freely on every space. A nontrivial [group](group.md) acting freely must act by a fixed-point-free map for each nonidentity element; the [fixed-point property of even-dimensional complex projective space](algebraic-topology.md#fixed-point-property-of-even-dimensional-complex-projective-space) obstructs such actions. For a [finite group](group.md#finite-group) acting freely on a Hausdorff [manifold](topology.md#topological-manifold), the quotient map is a [covering map](algebraic-topology.md#covering-space).

### Free group action

↑ **Parent:** [Group action](#group-action)

A [group action](#group-action) is free if the only element of the [group](group.md) fixing any point is the [identity element](group.md#identity-element). Thus every [stabilizer subgroup](#stabilizer-subgroup) is trivial. This is a property of an action of any [group](group.md), not an assertion that the acting group is a [free group](geometric-group-theory.md#free-group).

#### Finite groups cannot act freely on Euclidean space

↑ **Parent:** [Free group action](#free-group-action)

If a nontrivial finite group acted freely on $\mathbb R^n$, a prime-order cyclic subgroup $C_p$ would too. The quotient is an $n$-manifold with contractible universal cover. The singular version of [cellular free resolution from a contractible universal cover](#cellular-free-resolution-from-a-contractible-universal-cover) identifies its cohomology with [group cohomology](#group-cohomology) of $C_p$. The [periodic resolution of a finite cyclic group](#periodic-resolution-of-a-finite-cyclic-group) gives $H^{2j}(C_p;\mathbb Z)=\mathbb Z/p$ for every $j\geq1$. But [Poincaré duality for noncompact manifolds](cohomology.md#poincare-duality-for-noncompact-manifolds) makes the quotient cohomology zero above dimension $n$. This contradiction excludes the action, for arbitrary homeomorphisms, not only Euclidean isometries.

#### Free actions on even-dimensional spheres have order at most two

↑ **Parent:** [Free group action](#free-group-action)

For every nonidentity element of a [free group action](#free-group-action) on $S^{2r}$, its action map has no fixed point and hence degree minus one by [fixed-point-free sphere maps are homotopic to the antipodal map](homology.md#fixed-point-free-sphere-maps-are-homotopic-to-the-antipodal-map). Degree of homeomorphisms defines a homomorphism into $\{1,-1\}$, whose kernel is trivial, since no nonidentity action map can have degree one. Thus the acting group has order at most two. For $S^0$, freeness on its two points gives the same conclusion directly.

#### Free sphere actions exclude elementary abelian subgroups of rank two

↑ **Parent:** [Free group action](#free-group-action)

Suppose a finite [group](group.md) $G$ acts freely on $S^n$, $n>1$. The quotient has [fundamental group](algebraic-topology.md#fundamental-group) $G$ and higher [homotopy groups](algebraic-topology.md#homotopy-group) equal to those of $S^n$. Attach one $(n+1)$-cell killing a generator of $\pi_n\cong\mathbb Z$, then attach higher cells successively to kill all remaining higher [homotopy](algebraic-topology.md#homotopy). This constructs a [Eilenberg–MacLane space](algebraic-topology.md#eilenberg-maclane-space) $K(G,1)$ with only one $(n+1)$-cell. The [one-cell bound on next-degree cohomology](homology.md#one-cell-bound-on-next-degree-cohomology) gives dimension at most one in degree $n+1$. But if $G=C_p\times C_p$, the [mod-p cohomology ring of a cyclic group](#mod-p-cohomology-ring-of-a-cyclic-group) and [Künneth theorem](cohomology.md#kunneth-theorem) give dimension $n+2$ there. This contradiction excludes that group, and also excludes such a subgroup of any group acting freely on a sphere.

### Fundamental domain

↑ **Parent:** [Group action](#group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_domain)

For a [group action](#group-action), a fundamental domain selects one representative from each [orbit](dynamical-systems.md#orbit-dynamical-system). Geometric fundamental domains are often taken with their boundary included, allowing boundary overlaps while their interiors remain disjoint under the action. For translations of the real line by the [integers](number-theory.md#integer), $[0,1)$ is an exact representative set and $[0,1]$ is its closed geometric version. A [lattice](mathematical-logic.md#lattice) similarly gives a half-open fundamental parallelepiped.

### Multiply transitive group action

↑ **Parent:** [Group action](#group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiply_transitive_group_action)

A [group action](#group-action) is $t$-transitive if it acts transitively on ordered $t$-tuples of distinct points. In degree $n\ge t$ this implies $n(n-1)\cdots(n-t+1)\mid |G|$. It is [sharply t-transitive](#sharp-t-transitivity) when each such ordered tuple has trivial [stabilizer subgroup](#stabilizer-subgroup).

#### Three-transitive group action

↑ **Parent:** [Multiply transitive group action](#multiply-transitive-group-action)

Transitivity on ordered triples of distinct points. It implies a [two-transitive group action](#two-transitive-group-action), but is stronger: in projective dimension at least two, collinear and noncollinear triples distinguish two orbits, even though the projective action is two-transitive.

### Diagonal action on a centerless group

↑ **Parent:** [Group action](#group-action)

For nontrivial centerless $T$, this action of $T\times T$ is faithful and transitive. Its identity stabilizer is the diagonal subgroup. Subgroups above that diagonal are $\{(a,b):a^{-1}b\in N\}$ with $N\trianglelefteq T$: multiply by a diagonal element to isolate the second coordinate, then use diagonal conjugation. Thus the action is primitive exactly when $T$ is nonabelian simple.

### Ring of invariants

↑ **Parent:** [Group action](#group-action)

For a group acting on a [ring](commutative-algebra.md#ring) by [ring automorphisms](commutative-algebra.md#ring-automorphism), the elements fixed by every group element form a [subring](commutative-algebra.md#subring) containing $1$. For finite $G$ acting on a commutative [ring](commutative-algebra.md#ring), each $r$ satisfies the monic orbit equation $\prod_{g\in G}(T-g(r))$, whose coefficients are fixed. Thus $R$ is integral over its [invariant subring](#ring-of-invariants). This uses an orbit product, not division by the group order.

#### Normality of a ring of invariants

↑ **Parent:** [Ring of invariants](#ring-of-invariants)

A fraction of invariant elements is fixed by every automorphism. If that fraction is integral over $R^G$, its monic equation also makes it integral over $R$. A [normal domain](commutative-algebra.md#integrally-closed-domain) therefore places it in $R$, and fixedness places it in $R^G$. This proves integral closedness of the [invariant subring](#ring-of-invariants) in its own [fraction field](commutative-algebra.md#field-of-fractions). The proof works for any group and in every characteristic; no averaging or finiteness of the group is needed for normality.

### Primitive group action

↑ **Parent:** [Group action](#group-action)

A transitive group action is primitive if the only blocks are singletons and the whole set; a block has every translate either equal to it or disjoint from it. Orbits of a normal subgroup form blocks. Hence a nontrivial normal subgroup in a faithful primitive action is transitive. Two-transitivity implies primitivity. This normal-subgroup observation is a hypothesis engine for [Iwasawa's simplicity lemma](finite-group-theory.md#iwasawa-simplicity-lemma).

#### Primitive group with a transposition

↑ **Parent:** [Primitive group action](#primitive-group-action)

If a primitive subgroup of $S_n$ contains a [transposition](combinatorics.md#transposition-permutation), make a graph whose edges are the supports of its conjugate [transpositions](combinatorics.md#transposition-permutation). Connected components form blocks for the group. An edge exists, so primitivity forces the graph to be connected. Its edge [transpositions](combinatorics.md#transposition-permutation) generate all of $S_n$, proving that the original group is $S_n$.

#### Even primitive groups of safe-prime degree

↑ **Parent:** [Primitive group action](#primitive-group-action)

Every nontrivial normal subgroup of a faithful primitive group of prime degree is transitive and contains a Sylow $p$-subgroup $P$. Its normalizer in $A_p$ has order $pq$. For a proper normal subgroup $N$, the [Frattini argument](finite-group-theory.md#frattini-argument) gives $G=NN_G(P)$; unless $G=C_p$, its $P$-normalizer is the full order-$pq$ normalizer, while $N_N(P)=P$. The [Burnside transfer theorem](#burnside-transfer-theorem) gives a characteristic normal $p$-complement in $N$. This complement is normal in $G$ and cannot be transitive because its order is prime to $p$, so it is trivial. Thus $N=P$ and $|G|=pq$.

<h4 id="o-nan-scott-theorem">O'Nan–Scott theorem</h4>

↑ **Parent:** [Primitive group action](#primitive-group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/O'Nan–Scott_theorem)

The theorem classifies finite primitive permutation groups by their minimal normal subgroups and the action of their socle. The modern types are affine (HA), almost simple (AS), simple diagonal (SD), compound diagonal (CD), product action (PA), holomorph simple (HS), holomorph compound (HC), and twisted wreath (TW). A coarser version describes primitive maximal subgroups of symmetric groups by affine, almost-simple, diagonal and full product-action overgroups. Intransitive and imprimitive maxima are respectively unequal-part subset stabilizers and block-system stabilizers. Primitivity alone is not maximality in the symmetric group; parity can put an otherwise natural candidate entirely inside the alternating group.

##### Diagonal primitive permutation group

↑ **Parent:** [O'Nan–Scott theorem](#o-nan-scott-theorem)

For a nonabelian simple group $T$, act on cosets of its full diagonal in $T^r$. A suitable factor-permuting extension is primitive and has point stabilizer intersecting the socle in the diagonal. The full normalizer has order $|T|^r|\operatorname{Out}(T)|r!$. For $T=A_5,r=2$, it acts on the sixty elements of $A_5$ by left/right multiplication, automorphisms and inversion, and has order $14400$. Odd conjugation in $S_5$ induces an odd permutation of these sixty points, while inversion is even; the full group is a primitive maximal subgroup of $S_{60}$.

##### Affine primitive permutation group

↑ **Parent:** [O'Nan–Scott theorem](#o-nan-scott-theorem)

An elementary abelian regular minimal normal subgroup acts as translations of a vector space. Its point stabilizer acts faithfully and irreducibly on that space; invariant subspaces would be blocks. The full affine normalizer is $AGL_d(p)$. In degree sixteen it lies inside $A_{16}$: nonzero translations swap eight pairs, and elementary linear transvections swap four pairs. Thus it is not a maximal subgroup of $S_{16}$.

###### General affine group

↑ **Parent:** [Affine primitive permutation group](#affine-primitive-permutation-group)

The [group](group.md) of maps $x\mapsto Ax+b$ of a finite-dimensional [vector space](vector-space.md), with $A$ invertible. Identifying the underlying points with a regular [elementary abelian group](group.md#elementary-abelian-group) identifies its normalizer in the [symmetric group](finite-group-theory.md#symmetric-group) with this [semidirect product](#semidirect-product).

#### Primitive three-cycle criterion

↑ **Parent:** [Primitive group action](#primitive-group-action)

Conjugate the three-cycle throughout the group. Connected components of the support hypergraph form an invariant [block system](#block-system). Primitivity makes it connected, and [connected triple supports generate an alternating group](finite-group-theory.md#connected-triple-supports-generate-an-alternating-group) gives the conclusion.

### Variable-permutation action on polynomials

↑ **Parent:** [Group action](#group-action)

The [symmetric group](finite-group-theory.md#symmetric-group) acts on [multivariate polynomials](polynomial.md#multivariate-polynomial) by replacing each variable $x_i$ by $x_{\sigma(i)}$. With $(\sigma\tau)(i)=\sigma(\tau(i))$, substitution gives $\sigma\cdot(\tau\cdot f)=(\sigma\tau)\cdot f$. Thus it is a left [group action](#group-action). A polynomial encoding a combinatorial partition has a [group orbit](#orbit-of-a-group-action) encoding all relabelings and a [stabiliser subgroup](#stabilizer-subgroup) encoding its label symmetries.

### Fixed point of a group action

↑ **Parent:** [Group action](#group-action)

A fixed point of a [group action](#group-action) is an element fixed by every group element. The set $A^G=\{a:g\cdot a=a\text{ for all }g\in G\}$ is the [categorical limit](category.md#categorical-limit) of the action viewed as a [functor](category.md#functor) from the one-object [category](category.md) associated with $G$ to the [Category of sets](category.md#category-of-sets).

### Left regular action

↑ **Parent:** [Group action](#group-action)

The left regular action of a [group](group.md) on its own underlying set is left multiplication. It is faithful, because an element fixing the identity is itself the identity. For a finite group it gives the [permutation representation](representation-theory.md#permutation-representation) used in [Cayley theorem](#cayley-s-theorem).

### Block system

↑ **Parent:** [Group action](#group-action)

A block system for a [group action](#group-action) is a partition of the acted-on set such that every [group](group.md) element permutes its parts. For a transitive action, a nontrivial block system has more than one part and more than one element per part. The full [symmetric group](finite-group-theory.md#symmetric-group) preserves no such partition: a [transposition](combinatorics.md#transposition-permutation) exchanging one point in each of two parts breaks it.

#### Uniform subdegrees force an imprimitive action to be Frobenius

↑ **Parent:** [Block system](#block-system)

For a transitive finite [permutation group](finite-group-theory.md#permutation-group), suppose each point stabilizer has orbits of a common size $r$ on the other points. If a nontrivial [block system](#block-system) exists, all two-point stabilizers are trivial. Indeed for block size $b$, $r\mid n-1$ gives $\gcd(r,b)=1$. An orbit of a block not containing $\alpha$ has size at most $br$ and divisible by $br$, so its b point-orbits are disjoint. A stabilizer of $\alpha$ and a point of that block fixes the whole block. Interchanging the two points also fixes the block of $\alpha$. Equal two-point-stabilizer orders then show that each two-point stabilizer fixes every point, and faithfulness makes it trivial.

### Transitive group action

↑ **Parent:** [Group action](#group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transitive_group_action)

A [group action](#group-action) on a set $X$ is transitive when every two points lie in the same [orbit of a group action](#orbit-of-a-group-action), equivalently when for all $x,y\in X$ there is a group element $g$ with $gx=y$.

#### Simply transitive group action

↑ **Parent:** [Transitive group action](#transitive-group-action)

A [group action](#group-action) is simply transitive when exactly one element sends any chosen point to any other. Equivalently it is both a [transitive group action](#transitive-group-action) and a [free group action](#free-group-action). Choosing a base point identifies the space with the acting [group](group.md); a different base point changes that identification by translation.

#### Regular group action

↑ **Parent:** [Transitive group action](#transitive-group-action)

A transitive [group action](#group-action) is regular if every [point stabilizer](#stabilizer-subgroup) is trivial. Equivalently each ordered pair of points is connected by exactly one [group](group.md) element. Identifying one point with the identity identifies the action with left multiplication on the [group](group.md). A regular [normal subgroup](#normal-subgroup) inside a larger primitive [group](group.md) can supply translations or nonabelian left multiplication; the whole primitive [group](group.md) usually has a nontrivial stabilizer acting by automorphisms of this regular [subgroup](group.md#subgroup).

#### Derangement in a transitive group action

↑ **Parent:** [Transitive group action](#transitive-group-action)

A derangement is an element fixing none of the points of a [group action](#group-action). Every finite transitive action on at least two points has a derangement. Count pairs $(g,x)$ with $gx=x$: transitivity gives $\sum_g|\operatorname{Fix}(g)|=\sum_x|G_x|=|G|$. If every element fixed a point, the identity's extra fixed points would make this sum strictly larger than $|G|$. This is the [Burnside lemma](representation-theory.md#burnside-s-lemma) counting argument specialized to existence of a derangement.

##### Derangement counting formula

↑ **Parent:** [Derangement in a transitive group action](#derangement-in-a-transitive-group-action)

[Inclusion-exclusion](combinatorics.md#inclusion-exclusion-principle) applied to the events that a [permutation](combinatorics.md#permutation) fixes a specified point gives the displayed formula. There are $\binom nk$ choices of $k$ fixed points and $(n-k)!$ permutations fixing them. The probability that a uniformly chosen permutation is a [derangement](combinatorics.md#derangement-of-a-permutation) tends to $e^{-1}$.

// Target: analysis.bigb

#### Rank of a transitive permutation group

↑ **Parent:** [Transitive group action](#transitive-group-action)

The number of point-stabilizer orbits, equivalently the number of orbits on ordered pairs. On $k$-spaces of an $n$-space with $k\le n/2$, $GL_n(q)$ has rank $k+1$, indexed by intersection dimension.

#### Regular permutation subgroup

↑ **Parent:** [Transitive group action](#transitive-group-action)

A regular permutation subgroup acts transitively with trivial point stabilizers. Each ordered pair of points is related by exactly one subgroup element. A finite regular subgroup on $n$ points has order $n$. Normality and characteristicity are additional properties; they do not follow from regularity alone.

##### Centralizer of a regular permutation subgroup

↑ **Parent:** [Regular permutation subgroup](#regular-permutation-subgroup)

Identify a regular orbit with the [group](group.md) using a chosen base point. A [permutation](combinatorics.md#permutation) commuting with all left translations satisfies $c(x)=xc(1)$. Thus the [centralizer](#centralizer) consists of right translations. Defining $R_g(x)=xg^{-1}$ makes $R_gR_h=R_{gh}$ and gives an isomorphism to $G$, rather than an unmentioned reversal of multiplication.

#### Sharp t-transitivity

↑ **Parent:** [Transitive group action](#transitive-group-action)

An action is sharply $t$-transitive if each ordered $t$-tuple of distinct points is carried to any other by exactly one group element. For finite degree $n\geq t$, its order is $n(n-1)\cdots(n-t+1)$ and each ordered-tuple stabilizer is trivial. Sharp one-transitivity is a regular action. Finite sharp two-transitivity gives a [regular kernel of a finite sharply two-transitive group](#regular-kernel-of-a-finite-sharply-two-transitive-group).

##### Sharp three-transitivity

↑ **Parent:** [Sharp t-transitivity](#sharp-t-transitivity)

Exactly one element sends each ordered triple of distinct points to each other such triple. On a [projective line](finite-group-theory.md#projective-line), representatives of the first two target points form a [basis](vector-space.md#basis); scaling them so their sum represents the third point gives the unique projective transformation.

##### Sharp two-transitivity

↑ **Parent:** [Sharp t-transitivity](#sharp-t-transitivity)

A [group action](#group-action) is sharply two-transitive when exactly one element sends each ordered distinct pair to each other ordered distinct pair. The [affine group over a finite field](#affine-group-over-a-finite-field) provides an example: solve $ax+b=u$ and $ay+b=v$ uniquely, giving $a=(v-u)/(y-x)$.

##### Regular kernel of a finite sharply two-transitive group

↑ **Parent:** [Sharp t-transitivity](#sharp-t-transitivity)

In a finite sharply two-transitive group, the identity together with all fixed-point-free elements forms a regular normal subgroup. One proof constructs virtual characters from induced point-stabilizer characters and the augmentation character, proves their norms are one, and realizes this set as an intersection of representation kernels. Conjugation by the point stabilizer is transitive on the kernel's nonidentity elements. This forces the kernel to be elementary abelian, so it is a unique Sylow subgroup and is characteristic. Closure of the fixed-point-free set is a theorem, not something supplied merely by counting its size.

#### One-point extension of a permutation group

↑ **Parent:** [Transitive group action](#transitive-group-action)

Adjoin a new point $\omega$ fixed by a transitive group $G$. A one-point extension is a transitive group on the enlarged set whose stabilizer of $\omega$ is exactly $G$, acting on the remaining points in the prescribed way. Its order is $(n+1)|G|$ in the finite degree-$n$ case. The [double-coset criterion for a one-point extension](#double-coset-criterion-for-a-one-point-extension) gives a concrete generator test.

##### Double-coset criterion for a one-point extension

↑ **Parent:** [One-point extension of a permutation group](#one-point-extension-of-a-permutation-group)

If $x$ interchanges the new point and $\alpha$, put $H=G_\alpha$. Then $\langle G,x\rangle$ is a one-point extension exactly when $x^2\in H$, $xHx^{-1}=H$, and $xgx\in GxG$ for every $g\notin H$. These conditions make $G\cup GxG$ multiplication-closed, hence a group in the finite setting, with new-point stabilizer $G$. Necessity comes from the two double cosets in the extended two-transitive action.

#### Prime-degree transposition criterion

↑ **Parent:** [Transitive group action](#transitive-group-action)

A transitive subgroup $G\le S_p$ for prime $p$ that contains a transposition is $S_p$. Form a [graph](graph.md) on the $p$ letters with edges given by all conjugates in $G$ of that transposition. The transitive action permutes connected components, so their common size divides $p$. An edge rules out size one, hence the graph is connected. Its edge transpositions generate $S_p$: successive swaps along a path generate the swap of its endpoint with any chosen start. All these edge transpositions belong to $G$.

### Two-transitive group action

↑ **Parent:** [Group action](#group-action)

A group action on a set is two-transitive when it acts transitively on ordered pairs of distinct points. Equivalently, a point stabilizer acts transitively on the remaining points.

This is the $k=2$ case of a [multiply transitive group action](#multiply-transitive-group-action).

#### Elementary abelian regular kernels in doubly transitive groups

↑ **Parent:** [Two-transitive group action](#two-transitive-group-action)

A [point stabilizer](#stabilizer-subgroup) in a doubly transitive [group](group.md) acts transitively by conjugation on the nonidentity elements of a regular [normal subgroup](#normal-subgroup) $N$. All those elements have the same order; Cauchy's theorem makes this a prime p and excludes other primes from $|N|$. A finite p-group has a nontrivial characteristic center. Transitivity then forces all of $N$ into its center, so $N$ is elementary abelian. Choosing a vector-space [basis](vector-space.md#basis) identifies the original [permutation](combinatorics.md#permutation) [group](group.md) with a [subgroup](group.md#subgroup) of the corresponding general affine [group](group.md).

#### Degree-ten partition action of S6

↑ **Parent:** [Two-transitive group action](#two-transitive-group-action)

There are $\binom63/2=10$ partitions of six letters into two unordered triples. A stabilizer is $S_3\wr S_2$, also the [normalizer](#normalizer) of the [Sylow subgroup](finite-group-theory.md#sylow-subgroup) generated by one 3-cycle in each triple. Relative to one partition, all other partitions have intersection pattern $1+2$ up to interchange, giving one orbit of the stabilizer and hence a [two-transitive](#two-transitive-group-action) action. A natural $S_5$ fixing one letter is transitive on these partitions, giving $S_6=S_5(S_3\wr S_2)$.

#### Minimal normal subgroup dichotomy for two-transitive groups

↑ **Parent:** [Two-transitive group action](#two-transitive-group-action)

A [minimal normal subgroup](#minimal-normal-subgroup) of a finite faithful [two-transitive group action](#two-transitive-group-action) is either regular elementary abelian or primitive nonabelian simple. The imprimitive case reduces to two-point stabilizers being trivial, then counting derangements gives a characteristic regular Sylow subgroup. In the primitive nonregular case, each simple direct factor is transitive. Two commuting transitive factors are regular and are mutual full centralizers. Thus at most two factors occur and $|N|=n^2$. But the common subdegree of $N_\alpha$ then divides both $n$ and $n-1$, forcing $N_\alpha=1$, a contradiction. Only one factor remains.

#### Affine two-transitive group

↑ **Parent:** [Two-transitive group action](#two-transitive-group-action)

Translations are regular on $V$, and the zero stabilizer is $H$. Two-transitivity is equivalent to $H$ being transitive on nonzero vectors. Full affine linear groups and groups with special linear or symplectic linear parts give examples.

### Orbit map

↑ **Parent:** [Group action](#group-action)

For a group $G$ acting on a set $X$ and a point $x\in X$, the orbit map is $G\to X$, $g\mapsto gx$. Its image is the [orbit of a group action](#orbit-of-a-group-action) of $x$, and its fibres are cosets of the [stabilizer subgroup](#stabilizer-subgroup) of $x$.

### Equivariant map

↑ **Parent:** [Group action](#group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equivariant_map)

For $G$-sets $X$ and $Y$, a map $f:X\to Y$ is equivariant when $f(gx)=gf(x)$ for every $g\in G$ and $x\in X$.

### Conjugation action

↑ **Parent:** [Group action](#group-action)

A group acts on itself and on its subgroups by conjugation: $g\cdot x=gxg^{-1}$ and $g\cdot H=gHg^{-1}$.

#### Conjugates of a proper subgroup do not cover a finite group

↑ **Parent:** [Conjugation action](#conjugation-action)

For a proper [subgroup](group.md#subgroup) $B$ of a [finite group](group.md#finite-group) $G$, the number $m$ of its conjugates is $[G:N_G(B)]\leq[G:B]$, because its [normalizer](#normalizer) contains $B$. All conjugates contain the identity, so their union has size at most $1+m(|B|-1)\leq|G|-[G:B]+1<|G|$. Thus some element is not conjugate to any element of $B$. Finiteness is essential to this cardinal counting argument.

#### Conjugation

↑ **Parent:** [Conjugation action](#conjugation-action)

Conjugation by $g$ is the [group automorphism](algebra.md#group-automorphism) $x\mapsto gxg^{-1}$. Its orbits are the [conjugacy classes](#conjugacy-class).

##### Conjugate subset

↑ **Parent:** [Conjugation](#conjugation)

For a subset $S$ of a [group](group.md) and an element $g$, its conjugate subset is

$$
gSg^{-1}=\{gsg^{-1}:s\in S\}.
$$

Conjugation is a [bijection](function.md#bijection) and a [group automorphism](algebra.md#group-automorphism), so it preserves cardinality and every property expressed using the group operation.

##### Conjugate group elements

↑ **Parent:** [Conjugation](#conjugation)

Two group elements $x$ and $y$ are conjugate when $y=gxg^{-1}$ for some group element $g$, equivalently when they belong to the same [conjugacy class](#conjugacy-class). Conjugate elements have the same [order of a group element](#order-of-a-group-element).

###### Conjugate permutation

↑ **Parent:** [Conjugate group elements](#conjugate-group-elements)

Two [permutations](combinatorics.md#permutation) in the same [symmetric group](finite-group-theory.md#symmetric-group) are conjugate if $\tau=\pi\sigma\pi^{-1}$ for some permutation $\pi$. Conjugation relabels every [permutation cycle](finite-group-theory.md#permutation-cycle), so it preserves [cycle type](finite-group-theory.md#cycle-type). Conversely, equal cycle types permit a relabelling between corresponding cycles, establishing conjugacy.

#### Conjugacy class

↑ **Parent:** [Conjugation action](#conjugation-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugacy_class)

The conjugacy class of $x\in G$ is its orbit under the [conjugation action](#conjugation-action):

$$
\operatorname{Cl}_G(x)=\{gxg^{-1}:g\in G\}.
$$

##### Infinite conjugacy class group

↑ **Parent:** [Conjugacy class](#conjugacy-class)

A discrete [group](group.md) is ICC when every nonidentity element has an infinite [conjugacy class](#conjugacy-class). The trivial [group](group.md) satisfies this condition vacuously. It characterizes when the [group von Neumann algebra](functional-analysis.md#group-von-neumann-algebra) is a [Von Neumann factor](functional-analysis.md#von-neumann-factor).

##### Torsion-freeness from one nonidentity conjugacy class

↑ **Parent:** [Conjugacy class](#conjugacy-class)

If an infinite [group](group.md) has a single nonidentity [conjugacy class](#conjugacy-class), it is a [torsion-free group](group.md#torsion-free-group). Otherwise every nonidentity element has the same finite order $n$. Powers show $n$ is prime. For $n\geq3$, choose $xgx^{-1}=g^2$; then $x^n=1$ gives $g=g^{2^n}$, impossible by [Fermat's little theorem](number-theory.md#fermat-little-theorem). For $n=2$, the group has exponent two and is abelian, so every conjugacy class is a singleton and the hypothesis would force the group to have only two elements. Infinitude excludes this final case.

##### Shortest conjugacy representative

↑ **Parent:** [Conjugacy class](#conjugacy-class)

A [shortest conjugacy representative](#shortest-conjugacy-representative) is a word having the fewest written letters among all words representing elements of a fixed [conjugacy class](#conjugacy-class). This minimum equals the least group [word length](geometric-group-theory.md#word-length) of an element in the class; a longer spelling of that element is not itself a shortest representative. Such a word exists because lengths are nonnegative integers. It is freely and cyclically reduced: free cancellation shortens the same representative, while removing mutually inverse first and last letters shortens a conjugate. Every cyclic rotation has the same minimal length.

###### Cyclic reduction of a shortest conjugacy representative

↑ **Parent:** [Shortest conjugacy representative](#shortest-conjugacy-representative)

A nonempty [shortest conjugacy representative](#shortest-conjugacy-representative) is a [cyclically reduced word](geometric-group-theory.md#cyclically-reduced-word). If $w=s v s^{-1}$ with first and last letters inverse, $v$ is a shorter word representing a conjugate. Consequently $w^n$ has length exactly $n|w|$ as a [freely reduced word](geometric-group-theory.md#freely-reduced-word), and any segment of the periodic word of length at most $|w|$ fits in a cyclic rotation of $w$. This observation turns a Dehn shortening segment crossing copy boundaries into a shortening of a conjugacy representative.

##### Conjugacy class splitting in a prime-index normal subgroup

↑ **Parent:** [Conjugacy class](#conjugacy-class)

If $N\trianglelefteq G$ has prime index $p$, a [conjugacy class](#conjugacy-class) of $G$ lying in $N$ splits into one or $p$ [conjugacy classes](#conjugacy-class) of $N$. [Conjugation](#conjugation) by $G$ acts transitively on these smaller classes, while $N$ fixes every one. This factors through $G/N$, and the [orbit-stabilizer theorem](#orbit-stabilizer-theorem) makes the number of classes a divisor of $p$.

###### Alternating conjugacy class splitting criterion

↑ **Parent:** [Conjugacy class splitting in a prime-index normal subgroup](#conjugacy-class-splitting-in-a-prime-index-normal-subgroup)

For an even [permutation](combinatorics.md#permutation) $g$, its [symmetric group](finite-group-theory.md#symmetric-group) class splits into two equal [alternating group](finite-group-theory.md#alternating-group) classes exactly when its symmetric-group centralizer contains no odd permutation. If an odd commuting element exists, an odd conjugator can be multiplied by it to become even; otherwise the index-two subgroup has two conjugation orbits. In cycle notation the splitting types are precisely distinct odd cycle lengths, counting fixed points as length-one cycles: rotating odd cycles is even, whereas an even cycle or the exchange of two equal odd cycles supplies an odd centralizer element.

###### Inversion of an odd cycle in an alternating group

↑ **Parent:** [Alternating conjugacy class splitting criterion](#alternating-conjugacy-class-splitting-criterion)

For an odd $n$-cycle $g$, an inverting permutation fixes one point and swaps $(n-1)/2$ pairs, so its sign is $(-1)^{(n-1)/2}$. Its other inverting permutations differ by elements of $C_{S_n}(g)=\langle g\rangle$, all even. Thus inversion is possible inside $A_n$ exactly when that sign is positive. In particular $A_n$ is not an [ambivalent group](group.md#ambivalent-group) when $n\equiv3\pmod4$.

##### Class equation

↑ **Parent:** [Conjugacy class](#conjugacy-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Class_equation)

For a finite group,

$$
|G|=|Z(G)|+\sum_i[G:C_G(x_i)],
$$

where the $x_i$ represent the noncentral conjugacy classes.

###### Prime-to-p conjugacy class lemma

↑ **Parent:** [Class equation](#class-equation)

For a [finite group](group.md#finite-group) with trivial [centre of a group](#center-of-a-group) and a prime divisor $p$ of its order, some nonidentity [conjugacy class](#conjugacy-class) has size [coprime](number-theory.md#coprime-integers) to $p$. Otherwise the [class equation](#class-equation) would give $|G|\equiv1\pmod p$. Primality is essential: in the [symmetric group](finite-group-theory.md#symmetric-group) $S_3$, neither nonidentity class size is coprime to the composite divisor $6$.

#### Centralizer and normalizer

↑ **Parent:** [Conjugation action](#conjugation-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Centralizer_and_normalizer)

##### Centralizer

↑ **Parent:** [Centralizer and normalizer](#centralizer-and-normalizer)

The centralizer of $x\in G$ is the stabilizer of $x$ under the [conjugation action](#conjugation-action):

$$
C_G(x)=\{g\in G:gx=xg\}.
$$

###### Centralizer of a subset

↑ **Parent:** [Centralizer](#centralizer)

The centralizer of a subset $A$ of a [group](group.md) consists of the elements commuting with every member of $A$. It is the intersection of the element [centralizers](#centralizer), hence a [subgroup](group.md#subgroup). Directly, identity commutes with every element, products of two elements that each commute with every member of $A$ still have that property, and the same is true of inverses. For $A=G$ this is the [centre of a group](#center-of-a-group). For an empty subset the commutation condition is vacuous and the centralizer is all of $G$.

###### Centraliser of a fixed-point-free involution

↑ **Parent:** [Centralizer](#centralizer)

Commutation with a fixed-point-free involution preserves its partner relation. A commuting [permutation](combinatorics.md#permutation) can permute the $m$ pairs and independently swap each pair. This gives the [permutation wreath product](#permutation-wreath-product) with order $2^m m!$.

###### Centraliser of a transposition

↑ **Parent:** [Centralizer](#centralizer)

A [permutation](combinatorics.md#permutation) commutes with a transposition exactly when it preserves its two-element support as a set. It may swap those two points and independently permute the remaining points. Thus this [centraliser](#centralizer) has order $2(n-2)!$.

##### Normalizer

↑ **Parent:** [Centralizer and normalizer](#centralizer-and-normalizer)

The normalizer $N_G(H)=\{g\in G:gHg^{-1}=H\}$ is the stabilizer of a subgroup $H$ under the [conjugation action](#conjugation-action).

###### Normalizer of a diagonal subgroup of GL2

↑ **Parent:** [Normalizer](#normalizer)

Over the reals or a [finite field](algebra.md#finite-field) with more than two elements, the [normalizer](#normalizer) of all invertible diagonal [matrices](vector-space.md#matrix) in $GL_2$ consists of [monomial matrices](#monomial-matrix) and has quotient $C_2$ over that diagonal [subgroup](group.md#subgroup). Over $\mathbb F_p$ its size is $2(p-1)^2$ for $p>2$. For $p=2$ the diagonal [subgroup](group.md#subgroup) is trivial, so its normalizer is all of $GL_2(\mathbb F_2)$, of order six.

### Orbit-stabilizer theorem

↑ **Parent:** [Group action](#group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orbit-stabilizer_theorem)

For a finite group acting on a set and any point $x$,

$$
|G|=|Gx|\,|G_x|.
$$

Indeed, $gG_x\mapsto gx$ is a well-defined bijection from the left cosets of the stabilizer to the orbit.

#### Orbit dimension formula

↑ **Parent:** [Orbit-stabilizer theorem](#orbit-stabilizer-theorem)

For an [algebraic group action](algebraic-geometry.md#algebraic-group-action), the orbit dimension is the dimension of the group minus that of its stabilizer. For a finite-dimensional representation, the stabilizer is an automorphism group, open in its [endomorphism ring](module-theory.md#endomorphism-ring), so their dimensions agree. In a [quiver representation space](algebra.md#quiver-representation-space), the [Ringel form](algebra.md#ringel-form) turns the orbit codimension into the dimension of the self-extension group.

### Symmetry group of a cube

↑ **Parent:** [Group action](#group-action)

The full isometry group of a cube has order $48$. Its transitive actions on the $8$ vertices, $12$ edges, and $4$ main diagonals have stabilizers isomorphic respectively to

$$
S_3,\qquad C_2\times C_2,\qquad C_2\times S_3.
$$

The action on main diagonals has kernel $\{I,-I\}$.

#### Body-diagonal stabilizer in the cube symmetry group

↑ **Parent:** [Symmetry group of a cube](#symmetry-group-of-a-cube)

For vertices $(\pm1,\pm1,\pm1)$, the [symmetry group of a cube](#symmetry-group-of-a-cube) consists of [signed permutation matrices](vector-space.md#signed-permutation-matrix). A matrix preserving the unoriented line through $(1,1,1)$ must have all three signs equal, so it has the form $\varepsilon P$, where $P$ is a [permutation matrix](vector-space.md#permutation-matrix) and $\varepsilon\in\{1,-1\}$. Central inversion commutes with every $P$ and is not itself a permutation matrix. Consequently $(P,\varepsilon)\mapsto\varepsilon P$ identifies this twelve-element [stabilizer subgroup](#stabilizer-subgroup) with the [direct product of groups](#direct-product-of-groups) $S_3\times C_2$. A body diagonal is different from a face-normal coordinate axis, whose line stabilizer has order sixteen.

#### Axial isotropy types of the full cube symmetry group

↑ **Parent:** [Symmetry group of a cube](#symmetry-group-of-a-cube)

The full [symmetry group of a cube](#symmetry-group-of-a-cube) acts as all signed permutation [matrices](vector-space.md#matrix). The [stabilizer subgroups](#stabilizer-subgroup) of $(1,0,0)$, $(1,1,0)$ and $(1,1,1)$ have orders eight, four and six, respectively, and their [fixed-point subspaces of a group action](representation-theory.md#fixed-point-subspace-of-a-group-action) are the lines through those vectors. The three [group orbits](#orbit-of-a-group-action) have sizes six, twelve and eight. They therefore give distinct axial types for the [equivariant branching lemma](dynamical-systems.md#equivariant-branching-lemma). More generally the fixed-space dimension of a vector [stabilizer subgroup](#stabilizer-subgroup) equals the number of distinct nonzero absolute coordinate values, so these are precisely its one-dimensional types.

// Destination: dynamical-systems.bigb

#### Axis stabilizer in the full octahedral symmetry group

↑ **Parent:** [Symmetry group of a cube](#symmetry-group-of-a-cube)

An opposite-vertex line in the [full octahedral symmetry group](#symmetry-group-of-a-cube) is an unoriented coordinate axis. Its [stabilizer subgroup](#stabilizer-subgroup) has the block form $\operatorname{diag}(A,\varepsilon)$, where $A$ is a signed two-dimensional permutation matrix and $\varepsilon=\pm1$. The eight possibilities for $A$ form the [dihedral group](finite-group-theory.md#dihedral-group) of a square, of order eight; the independent axial sign gives a [cyclic group](group.md#cyclic-group) of order two. Thus the stabilizer is their direct product, of order sixteen. It is larger than the stabilizer of an individual vertex, because exchanging the two endpoints still fixes the line.

#### Cube symmetry action on edges

↑ **Parent:** [Symmetry group of a cube](#symmetry-group-of-a-cube)

The full [symmetry group of a cube](#symmetry-group-of-a-cube) acts transitively and faithfully on its twelve edges. For vertices $(\pm1,\pm1,\pm1)$, its [signed permutation matrices](vector-space.md#signed-permutation-matrix) act transitively on the edges. The [stabilizer subgroup](#stabilizer-subgroup) of $\{(1,1,z):-1\le z\le1\}$ consists of independently swapping $x,y$ and reversing $z$, and is a [Klein four-group](finite-group-theory.md#klein-four-group). The [orbit-stabilizer theorem](#orbit-stabilizer-theorem) gives order $12\cdot4=48$. Fixing every edge fixes every vertex, as each vertex is the unique intersection of its three incident edges, so the [group action](#group-action) is faithful. The resulting [subgroup](group.md#subgroup) of $S_{12}$ has index $12!/48$ and is not normal: central inversion has [cycle type](finite-group-theory.md#cycle-type) $2^6$, whose [conjugacy class](#conjugacy-class) in $S_{12}$ has $12!/(2^6 6!)=10395>48$ elements.

#### Direct-product decomposition of the cube symmetry group

↑ **Parent:** [Symmetry group of a cube](#symmetry-group-of-a-cube)

The [symmetry group of a cube](#symmetry-group-of-a-cube) splits into its central inversion and its [rotational symmetry group of a cube](#rotational-symmetry-group-of-a-cube). Inversion has [determinant](linear-algebra.md#determinant) $-1$, the rotation [subgroup](group.md#subgroup) has [determinant](linear-algebra.md#determinant) $1$, and together they generate the full [group](group.md) with trivial intersection. The rotation [subgroup](group.md#subgroup) acts faithfully on the four body diagonals and is isomorphic to $S_4$. Consequently the full [group](group.md) is this [direct product of groups](#direct-product-of-groups).

#### Rotational symmetry group of a cube

↑ **Parent:** [Symmetry group of a cube](#symmetry-group-of-a-cube)

The orientation-preserving symmetries of a cube are the $3\times3$ [signed permutation matrices](vector-space.md#signed-permutation-matrix) with [determinant](linear-algebra.md#determinant) one. There are $3!\,2^2=24$ of them. Their [group action](#group-action) on the four body diagonals identifies this [group](group.md) with the [symmetric group](finite-group-theory.md#symmetric-group) $S_4$. Indeed choose diagonal directions $(1,1,1),(1,-1,-1),(-1,1,-1),(-1,-1,1)$, whose sum is zero and whose only linear relation has all coefficients equal. A rotation fixing every diagonal sends each direction to itself or its negative; the relation forces all four signs equal. All negative would give $-I$, which has [determinant](linear-algebra.md#determinant) $-1$, so the [kernel of a group homomorphism](#kernel-of-a-group-homomorphism) is trivial. Both [groups](group.md) have order 24, giving the identification. Its face [permutations](combinatorics.md#permutation) have cycle types $1^6$, $1^24$, $1^22^2$, $2^3$ and $3^2$, occurring $1,6,3,6,8$ times respectively.

##### Tetrahedron stabilizer in the cube rotation group

↑ **Parent:** [Rotational symmetry group of a cube](#rotational-symmetry-group-of-a-cube)

For cube vertices $(\pm1,\pm1,\pm1)$, the four vertices of coordinate product $+1$ and the four of product $-1$ form the two inscribed [regular tetrahedra](geometry-and-topology.md#regular-tetrahedron). A cube [rotation](riemannian-geometry.md#rotation-mathematics) is a [signed permutation matrix](vector-space.md#signed-permutation-matrix) of [determinant](linear-algebra.md#determinant) one and maps each product class to one class. A quarter-turn about a coordinate axis exchanges the classes. The [orbit](dynamical-systems.md#orbit-dynamical-system) of either tetrahedron therefore has size two, while the [cube rotation group](#rotational-symmetry-group-of-a-cube) has order 24. The [orbit-stabilizer theorem](#orbit-stabilizer-theorem) gives its setwise [stabilizer subgroup](#stabilizer-subgroup) order 12; this is the tetrahedron's proper [rotation](riemannian-geometry.md#rotation-mathematics) [group](group.md).

##### Kernel of the cube face-axis action

↑ **Parent:** [Rotational symmetry group of a cube](#rotational-symmetry-group-of-a-cube)

Permuting the three pairs of opposite faces gives a [group homomorphism](#group-homomorphism) from the [rotational symmetry group of a cube](#rotational-symmetry-group-of-a-cube) to $S_3$. Its kernel consists of the identity and the half-turns about the three coordinate axes: these are precisely the diagonal sign matrices with [determinant](linear-algebra.md#determinant) one. Thus it is a [normal subgroup](#normal-subgroup) of order four, a [Klein four-group](finite-group-theory.md#klein-four-group).

##### Face-pair orbits of cube rotations

↑ **Parent:** [Rotational symmetry group of a cube](#rotational-symmetry-group-of-a-cube)

The [rotational symmetry group of a cube](#rotational-symmetry-group-of-a-cube) has three [group orbits](#orbit-of-a-group-action) on ordered pairs of faces: equal faces, opposite faces, and adjacent faces. Their sizes are respectively $6$, $6$ and $24$. Fixing one face leaves its cyclic group of four quarter-turns, which acts transitively on the four adjacent faces; this proves transitivity in the last orbit rather than merely counting its points.

### Faithful group action

↑ **Parent:** [Group action](#group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Faithful_group_action)

A group action is faithful when only the identity acts as the identity on every point.

#### Normal subgroup orbits in a faithful prime-degree action

↑ **Parent:** [Faithful group action](#faithful-group-action)

If a group acts transitively on a set of prime size and $N$ is normal, then the $N$-orbits form a $G$-invariant block system of equal size. They are therefore either singletons or the whole set. In a faithful action the singleton case forces $N=1$, so every nontrivial normal subgroup is transitive.

### Orbit of a group action

↑ **Parent:** [Group action](#group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orbit_of_a_group_action)

The orbit of $x$ is $Gx=\{gx:g\in G\}$.

#### Equality-pattern orbits of ordered pairs

↑ **Parent:** [Orbit of a group action](#orbit-of-a-group-action)

The diagonal [group action](#group-action) of the [symmetric group](finite-group-theory.md#symmetric-group) on ordered pairs has two [orbits of a group action](#orbit-of-a-group-action) when $n\geq2$: equal pairs, of size $n$, and distinct pairs, of size $n(n-1)$. Equality is preserved by a [bijection](function.md#bijection), and a prescribed bijection on one or two distinct letters extends to a [permutation](combinatorics.md#permutation) of all letters. At $n=1$ only the equal-pair orbit remains.

#### Real rotation orbits on a complex unit quadric

↑ **Parent:** [Orbit of a group action](#orbit-of-a-group-action)

For $z=x+iy\in\mathbb C^3$ satisfying $z^Tz=1$, the real and imaginary parts obey $|x|^2-|y|^2=1$ and $x\cdot y=0$. Simultaneous real rotations preserve $r=|y|$. At $r=0$ the [group orbit](#orbit-of-a-group-action) is the unit sphere, with [stabilizer subgroup](#stabilizer-subgroup) $SO(2)$. At each $r>0$, the normalized pair $(x,y)$ is an oriented two-frame, giving a free transitive [SO(3) group](linear-algebra.md#so-3-group) action. The [group orbit](#orbit-of-a-group-action) space is $[0,\infty)$, and the whole quadric is diffeomorphic to the [tangent bundle](fiber-bundle.md#tangent-bundle) of $S^2$. Its varying Hermitian norm prevents it from being a single [SU(3)](topological-group.md#su-3-group) [group orbit](#orbit-of-a-group-action).

#### Equality-pattern orbits of projective triples

↑ **Parent:** [Orbit of a group action](#orbit-of-a-group-action)

The [general linear group over a finite field](finite-group-theory.md#general-linear-group-over-a-finite-field) acting diagonally on projective triples has five [orbits of a group action](#orbit-of-a-group-action): all equal, three different positions for the repeated coordinate when exactly two are equal, and all distinct. The corresponding representative [stabilizer subgroups](#stabilizer-subgroup) are upper triangular, diagonal, and [scalar matrices](linear-algebra.md#scalar-matrix). Their orders are $p(p-1)^2$, $(p-1)^2$, and $p-1$, respectively; the orbit sizes are $p+1$, $p(p+1)$, and $p(p+1)(p-1)$. Transitivity follows from the action being [sharply three-transitive on a projective line](finite-group-theory.md#sharply-three-transitive-on-a-projective-line).

### Stabilizer subgroup

↑ **Parent:** [Group action](#group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stabilizer_subgroup)

The stabilizer of $x$ is the subgroup $\{g:gx=x\}$.

#### Pointwise stabilizer

↑ **Parent:** [Stabilizer subgroup](#stabilizer-subgroup)

For a [group action](#group-action), the pointwise stabilizer of a set $S$ is the [subgroup](group.md#subgroup) fixing each of its points individually. It is the intersection of their [stabilizer subgroups](#stabilizer-subgroup). This is stronger than merely mapping the set to itself.

#### Axial subgroup

↑ **Parent:** [Stabilizer subgroup](#stabilizer-subgroup)

For a steady-state [equivariant dynamical system](dynamical-systems.md#equivariant-dynamical-system), an axial subgroup has a one-dimensional real [fixed-point subspace of a group action](representation-theory.md#fixed-point-subspace-of-a-group-action). A complex axial subgroup for a Hopf problem has a one-dimensional complex fixed-point subspace under the spatial group combined with the common phase action. Distinct conjugacy classes may yield distinct types of bifurcating branches.

##### Complex axial isotropy subgroup

↑ **Parent:** [Axial subgroup](#axial-subgroup)

For the spatial group combined with the temporal phase circle in an equivariant Hopf problem, a complex axial isotropy subgroup is an actual stabilizer whose fixed-point space is one complex line. Its real dimension is two. One must include the kernel of the combined action when writing the full stabilizer, not just a generator having the right fixed space.

// Target: dynamical-systems.bigb

### Symmetric group action on subsets

↑ **Parent:** [Group action](#group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_group_action_on_subsets)

The symmetric group acts on $k$-element subsets by applying a permutation to every member.

### Coset action

↑ **Parent:** [Group action](#group-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coset_action)

A group acts on the left cosets of a subgroup by left multiplication; its kernel is the core of that subgroup.

## Coset

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coset)

For a subgroup $H\leq G$, a left coset is $gH=\{gh:h\in H\}$. The left cosets partition $G$ and all have cardinality $|H|$.

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

by the [orbit-stabilizer theorem](#orbit-stabilizer-theorem).

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

For a finite group $G$ and subgroup $H$, the order of $H$ divides the order of $G$, and the quotient is the number of left [cosets](#coset):

$$
|G|=[G:H]|H|.
$$

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

Every group $G$ embeds in the symmetric group on its underlying set through the left-regular action $g:x\mapsto gx$.

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

### Product of commuting elements of coprime order

↑ **Parent:** [Order of a group element](#order-of-a-group-element)

Let commuting elements $a,b$ have finite coprime orders $m,n$. Their [cyclic subgroups](group.md#cyclic-subgroup) have trivial intersection by [Lagrange's theorem](#lagrange-s-theorem). If $(ab)^k=1$, then $a^k=b^{-k}$ belongs to this intersection, so $m\mid k$ and $n\mid k$. Thus $mn\mid k$. Conversely, $(ab)^{mn}=1$ because the elements commute. This proves the displayed order formula.

### Infinite order

↑ **Parent:** [Order of a group element](#order-of-a-group-element)

A group element has infinite order when no positive power of it is the [identity element](group.md#identity-element).

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

The [group](group.md) of invertible [linear maps](vector-space.md#linear-map) preserving a specified [quadratic form](linear-algebra.md#quadratic-form) over a [finite field](algebra.md#finite-field). In characteristic two one must preserve the [quadratic form](linear-algebra.md#quadratic-form) itself, not merely its polar [alternating bilinear form](linear-algebra.md#alternating-bilinear-form). For a nonsingular form, any two nonzero [isotropic vectors](linear-algebra.md#isotropic-vector) can be incorporated into hyperbolic pairs and standard adapted bases, producing an isometry between them.

## Special linear group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Special_linear_group)

### Real special linear group of degree two

↑ **Parent:** [Special linear group](#special-linear-group)

This [Lie group](lie-theory.md#lie-group) consists of real two-by-two matrices of determinant one. Its [Lie algebra](lie-algebra.md) is the space of traceless real two-by-two matrices. Its [Exponential map of a Lie group](lie-theory.md#exponential-map-of-a-lie-group) is not onto: by the [Cayley-Hamilton theorem](mathematics.md#cayley-hamilton-theorem), $A^2=-\det(A)I$ for traceless $A$, and its exponential has trace either $2\cosh s$ or $2\cos s$, hence never less than $-2$. The determinant-one matrix $\operatorname{diag}(-2,-1/2)$ is therefore outside its exponential image.

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

Complex two-by-two [matrices](vector-space.md#matrix) of [determinant](linear-algebra.md#determinant) one form a complex three-dimensional [Lie group](lie-theory.md#lie-group), or a real six-dimensional [Lie group](lie-theory.md#lie-group). Their congruence action on Hermitian two-by-two [matrices](vector-space.md#matrix) gives the [Lorentz spinor double cover](special-relativity.md#lorentz-spinor-double-cover) with kernel $\{I,-I\}$. The two [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) representations are $A$ and $(A^\dagger)^{-1}$. Treating the group as real is essential for the second, antiholomorphic representation.

### Triangular-rotation factorization of real determinant-one matrices

↑ **Parent:** [Special linear group](#special-linear-group)

Every $g\in SL_2(\mathbb R)$ factors into an upper triangular determinant-one matrix and a [rotation matrix](linear-algebra.md#rotation-matrix). This follows because the triangular subgroup acts transitively on the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), a [group orbit](#orbit-of-a-group-action) of the full group, while $SO(2)$ is the [stabilizer subgroup](#stabilizer-subgroup) of $i$. The intersection of the two subgroups is $\{\pm I\}$, giving exactly two matrix pairs $(h,k)$ and $(-h,-k)$. Requiring the diagonal of $h$ to be positive gives uniqueness. For $g=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ and $q=\sqrt{c^2+d^2}$, the positive branch is $h=\begin{pmatrix}1/q&(ac+bd)/q\\0&q\end{pmatrix}$ and $k=q^{-1}\begin{pmatrix}d&-c\\c&d\end{pmatrix}$.

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

A group homomorphism preserves multiplication: $\phi(xy)=\phi(x)\phi(y)$.

### Homomorphism of abelian groups

↑ **Parent:** [Group homomorphism](#group-homomorphism)

A [group homomorphism](#group-homomorphism) between [abelian groups](group.md#abelian-group), conventionally written additively. Its [kernel](linear-algebra.md#kernel-of-a-linear-map) and [image](set-theory.md#image-of-a-function) are [subgroups](group.md#subgroup), and the additive formula implies preservation of zero, negation and every integer multiple. Maps on [Mordell-Weil groups](normalization-of-an-algebraic-curve.md#mordell-weil-group) induced by [isogenies of elliptic curves](normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) and by [good reduction](normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve) are examples.

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
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kernel_of_a_group_homomorphism)

The kernel $\{g:\phi(g)=1\}$ is a normal subgroup of the domain.

### Image of a group homomorphism

↑ **Parent:** [Group homomorphism](#group-homomorphism)

The image of a group homomorphism $\phi:G\to H$ is the subgroup $\{\phi(g):g\in G\}$ of $H$.

## Automorphism group

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Automorphism_group)

The automorphism group of a [group](group.md) $G$ is the group of all isomorphisms $G\to G$ under composition.

### Holomorph

↑ **Parent:** [Automorphism group](#automorphism-group)

The holomorph acts on the underlying set of a [group](group.md) by $x\mapsto g\alpha(x)$. Its multiplication is $(g,\alpha)(h,\beta)=(g\alpha(h),\alpha\beta)$. This is exactly the [normalizer](#normalizer) of the left regular [permutation](combinatorics.md#permutation) representation: a normalizing [permutation](combinatorics.md#permutation) fixing the identity is an [group automorphism](algebra.md#group-automorphism), and every normalizing [permutation](combinatorics.md#permutation) is a left translation followed by one. The embedded copy of $G$ is normal and the identity stabilizer is its [group automorphism](algebra.md#group-automorphism) [group](group.md).

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

An outer [group automorphism](algebra.md#group-automorphism) is not [conjugation](#conjugation) by any element of the [group](group.md). Its nonidentity class belongs to $\operatorname{Out}(G)=\operatorname{Aut}(G)/\operatorname{Inn}(G)$. A permutation-group example is the exceptional automorphism of $S_6$ that swaps its natural and transitive copies of $S_5$; it sends a [transposition](combinatorics.md#transposition-permutation) to a product of three disjoint [transpositions](combinatorics.md#transposition-permutation) and hence cannot be inner.

## Group cohomology

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_cohomology)

Group cohomology studies a [group](group.md) through cochain complexes built from its actions on abelian groups. In degree one, $H^1(G,M)$ identifies one-cocycles $c:G\to M$ modulo one-coboundaries.

### Cellular free resolution from a contractible universal cover

↑ **Parent:** [Group cohomology](#group-cohomology)

For a connected [CW complex](algebraic-topology.md#cw-complex) $X$ with contractible [universal cover](algebraic-topology.md#universal-cover), let $\Gamma=\pi_1(X)$ and $R=\mathbb Z\Gamma$. Lift each cell once and transport its orientation by [deck transformations](algebraic-topology.md#deck-transformation). Its translates form an $R$-basis of the cellular chains of the cover. The augmentation sends every vertex to one, and contractibility makes the augmented chain complex an exact [free resolution](algebra.md#free-resolution) of the trivial module $\mathbb Z$. An $R$-linear cochain with trivial coefficient action is constant on each orbit of lifts, identifying $\operatorname{Hom}_R(C_*(\widetilde X),\mathbb Z)$ with the [cellular cohomology](homology.md#cellular-cohomology) complex of $X$. Consequently $H^i(X;\mathbb Z)=\operatorname{Ext}_R^i(\mathbb Z,\mathbb Z)$. The same argument with singular simplex lifts works for spaces with a contractible universal cover.

### Integral cohomological dimension of a group

↑ **Parent:** [Group cohomology](#group-cohomology)

The integral cohomological dimension is the least length of a [projective resolution](algebra.md#projective-resolution) of the trivial [group ring](commutative-algebra.md#group-ring) module $\mathbb Z$, equivalently the largest degree in which [group cohomology](#group-cohomology) with some module can be nonzero. A group containing torsion has infinite integral cohomological dimension. For $\mathbb Z^r$ the dimension is $r$, realized by its [torus](topology.md#torus) classifying space and detected by its top cohomology.

#### Stallings-Swan theorem

↑ **Parent:** [Integral cohomological dimension of a group](#integral-cohomological-dimension-of-a-group)

A group has integral [cohomological dimension](#integral-cohomological-dimension-of-a-group) at most one precisely when it is a [free group](geometric-group-theory.md#free-group), including the trivial free group in dimension zero. This result concerns integral coefficients; a rational dimension-one statement has different conclusions.

### Poincare duality group

↑ **Parent:** [Group cohomology](#group-cohomology)

A Poincare duality group of dimension $n$ has a finite-length resolution of the trivial [group ring](commutative-algebra.md#group-ring) module $\mathbb Z$ by [finitely generated projective modules](module-theory.md#finite-projective-module), and $H^k(G,\mathbb ZG)$ vanishes except in degree $n$, where it is infinite cyclic as an abelian group. The top module $D$ can have an orientation-sign action. Reversing the dual projective resolution gives $H^k(G,V)\cong\operatorname{Tor}^{\mathbb ZG}_{n-k}(D,V)$, equivalently $H_{n-k}(G,D\otimes V)$ with the appropriate diagonal action. Untwisted duality requires trivial orientation action. In positive dimension $H^0(G,\mathbb ZG)=0$, since a finitely supported invariant element cannot exist for an infinite group.

#### Normal finitely presented subgroups of three-dimensional duality groups

↑ **Parent:** [Poincare duality group](#poincare-duality-group)

Let $N$ be a normal [finitely presented group](geometric-group-theory.md#finitely-presented-group) inside a dimension-three [Poincare duality group](#poincare-duality-group) $G$, with $G/N$ containing an element of infinite order. Then $N$ is either a [free group](geometric-group-theory.md#free-group) or a dimension-two [Poincare duality group](#poincare-duality-group). The [Strebel infinite-index subgroup theorem](#strebel-infinite-index-subgroup-theorem) gives $\operatorname{cd}N\leq2$. If the dimension is two, take the preimage of an infinite cyclic subgroup of the quotient. The [cyclic-extension shift of group-ring cohomology](#cyclic-extension-shift-of-group-ring-cohomology) gives dimension three, forcing this preimage to have finite index by Strebel. Its duality then gives $H^*(N;\mathbb ZN)$ concentrated in degree two with top group $\mathbb Z$. The quotient is virtually cyclic, and surface automorphism realization gives a finite-index surface mapping-torus group.

#### Classification of two-dimensional Poincare duality groups

↑ **Parent:** [Poincare duality group](#poincare-duality-group)

Every integral dimension-two [Poincare duality group](#poincare-duality-group) is the [fundamental group](algebraic-topology.md#fundamental-group) of a closed aspherical [topological surface](topology.md#topological-surface). Orientable examples are the torus and closed surfaces of genus at least two. Nonorientable aspherical closed surfaces supply the orientation-twisted examples.

#### Strebel infinite-index subgroup theorem

↑ **Parent:** [Poincare duality group](#poincare-duality-group)

An infinite-index subgroup of an integral dimension-$d$ [Poincare duality group](#poincare-duality-group) has integral [cohomological dimension](#integral-cohomological-dimension-of-a-group) at most $d-1$. No finiteness assumption on the subgroup is needed for this inequality. In dimension three it places every infinite-index subgroup in cohomological dimension at most two.

#### Extension rule for Poincare duality groups

↑ **Parent:** [Poincare duality group](#poincare-duality-group)

For an extension with kernel a dimension-$n$ [Poincare duality group](#poincare-duality-group) and quotient a dimension-$q$ [Poincare duality group](#poincare-duality-group), apply the [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence) to the ambient group ring. Kernel cohomology is concentrated in degree $n$ and is a regular quotient module with a rank-one orientation twist. Quotient cohomology is then concentrated in degree $q$ with underlying group $\mathbb Z$. The extension resolution supplies finiteness and gives cohomological dimension at most $n+q$, proving duality in that dimension. Orientation actions need not be trivial.

#### Finite-index invariance of Poincare duality for torsion-free groups

↑ **Parent:** [Poincare duality group](#poincare-duality-group)

For a [torsion-free group](group.md#torsion-free-group) $G$ and [finite-index subgroup](group.md#finite-index-subgroup) $H$, $G$ is a [Poincare duality group](#poincare-duality-group) of dimension $n$ if and only if $H$ is. Finite-index induction and coinduction of $\mathbb ZH$ coincide and give $\mathbb ZG$, so [Shapiro's lemma](#shapiro-s-lemma) identifies their group-ring cohomology as abelian groups. The finite-index finiteness and cohomological-dimension lemmas supply finite projective resolutions. Without torsion-freeness of $G$ the converse fails: $\mathbb Z\times C_2$ contains the index-two $PD^1$ subgroup $\mathbb Z$ but has infinite integral cohomological dimension.

### Mod-p cohomology ring of a cyclic group

↑ **Parent:** [Group cohomology](#group-cohomology)

For a prime $p$, a classifying [Eilenberg–MacLane space](algebraic-topology.md#eilenberg-maclane-space) for $C_p$ is the infinite lens space $S^\infty/C_p$, using scalar multiplication by a primitive $p$th root on the complex-coordinate sphere. Its contractible [universal cover](algebraic-topology.md#universal-cover) is $S^\infty$. The standard two-periodic free resolution has differentials $g-1$ and $1+g+\cdots+g^{p-1}$, both zero after applying [cochains](cohomology.md#singular-cochain) with trivial $\mathbb F_p$ coefficients. Thus every [cohomology](cohomology.md) degree has dimension one. If $p=2$, the ring is $\mathbb F_2[t]$, $|t|=1$. If $p$ is odd, it is $\Lambda(a)\otimes\mathbb F_p[b]$, with $|a|=1$, $|b|=2$: graded commutativity gives $a^2=0$ and the periodicity class $b$ induces the degree-two isomorphisms. The [Künneth theorem](cohomology.md#kunneth-theorem) gives two copies of these generators for $C_p\times C_p$; the dimension in degree $d$ is $d+1$ for every $p$.

### Dimension shifting in group cohomology

↑ **Parent:** [Group cohomology](#group-cohomology)

Embed a [module](module-theory.md#module-mathematics) $M$ over the [group ring](commutative-algebra.md#group-ring) $\mathbb Z[G]$ in a module $I$ with vanishing positive [group cohomology](#group-cohomology), and write $M'=I/M$. The connecting map in the long exact [group cohomology](#group-cohomology) sequence of $0\to M\to I\to M'\to0$ is an isomorphism $H^r(G,M')\to H^{r+1}(G,M)$ for $r\geq1$, since the groups involving $I$ on both sides vanish. For a finite [group](group.md) and a module $I$ with vanishing [Tate cohomology of a finite group](#tate-cohomology-of-a-finite-group) in every degree, the same argument shifts every Tate degree. Repeating this construction transports computations to a convenient resolution.

### Tate cohomology of a finite group

↑ **Parent:** [Group cohomology](#group-cohomology)

For a finite [group](group.md) $G$, Tate cohomology joins [group cohomology](#group-cohomology) and [group homology](#group-homology) through the norm map $N_G=\sum_{g\in G}g$. For $r\geq1$ it equals ordinary [group cohomology](#group-cohomology); for $r\leq-2$ it equals $H_{-r-1}(G,M)$. The middle terms are $\widehat H^0(G,M)=M^G/N_GM$ and $\widehat H^{-1}(G,M)=\ker(N_G)/I_GM$, where $I_GM$ is generated by $gm-m$. For the trivial module $\mathbb Z$, $\widehat H^{-2}(G,\mathbb Z)=G^{\mathrm{ab}}$. With multiplicative coefficients the norm is the product of the translates.

### Continuous cochains with topological coefficients

↑ **Parent:** [Group cohomology](#group-cohomology)

For a [topological group module](module-theory.md#topological-group-module), use continuous maps with pointwise addition and the inhomogeneous group-cohomology differential. The kernel modulo the image defines continuous [group cohomology](#group-cohomology) as an abelian group. With general topological coefficients the quotient topology need not be Hausdorff; the cohomology here is the algebraic quotient of continuous cocycles by continuous coboundaries. With trivial discrete coefficients in a [prime field](algebra.md#prime-field), its first cohomology is the space of continuous [group homomorphisms](#group-homomorphism) to that field's additive group.

### Tate cohomology of a cyclic group

↑ **Parent:** [Group cohomology](#group-cohomology)

For $G=\langle\sigma\rangle$, set $D=\sigma-1$ and $N=\sum_{g\in G}g$. The two periodic groups are $M^G/NM$ and $\ker N/DM$. A short exact sequence of modules gives a six-term periodic exact sequence. For multiplicative modules the norm operator is a product and $D(x)=\sigma(x)/x$.

#### Cyclic cohomology of a regular lattice

↑ **Parent:** [Tate cohomology of a cyclic group](#tate-cohomology-of-a-cyclic-group)

Let $G$ be cyclic and let $R[G]$ carry the regular [permutation action](#group-action). Invariants are constant coefficient vectors, which are the images of the norm operator. A vector with coefficient sum zero is the difference of a vector and its cyclic translate, by successively solving the coordinate differences. Thus the norm [group kernel](#kernel-of-a-group-homomorphism) equals $(\sigma-1)R[G]$. Both cyclic [Tate cohomology](#tate-cohomology-of-a-finite-group) [groups](group.md) vanish. This applies to $R=\mathbb Z$ and $R=\mathbb Z_p$, and to finite [direct sums](vector-space.md#direct-sum) of regular lattices.

#### Herbrand quotient

↑ **Parent:** [Tate cohomology of a cyclic group](#tate-cohomology-of-a-cyclic-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Herbrand_quotient)

When the two indicated groups are finite, their size ratio is multiplicative on short exact sequences. It is one for finite modules and therefore unchanged by finite-index modifications. A trivial integral module $\mathbb Z$ has quotient $|G|$, while an induced regular lattice $\mathbb Z_p[G]$ has both Tate groups zero and quotient one. These facts permit norm-index calculations without explicitly finding every norm.

##### Herbrand quotient of a finite module

↑ **Parent:** [Herbrand quotient](#herbrand-quotient)

For a finite [module](module-theory.md#module-mathematics) acted on by a cyclic [group](group.md), write $D=\sigma-1$ and $N=1+\sigma+\cdots+\sigma^{n-1}$. The two [Tate cohomology](#tate-cohomology-of-a-finite-group) [group](group.md) sizes are $|\ker D|/|NM|$ and $|\ker N|/|DM|$. The equalities $|NM|=|M|/|\ker N|$ and $|DM|=|M|/|\ker D|$ show that these sizes are equal. The exact-sequence multiplication rule for the [Herbrand quotient](#herbrand-quotient) consequently makes it unchanged by finite-index modifications of lattices.

##### Herbrand quotient of the local multiplicative group

↑ **Parent:** [Herbrand quotient](#herbrand-quotient)

For a cyclic extension of [p-adic fields](arithmetic.md#p-adic-field), sufficiently deep [principal units](arithmetic.md#principal-unit) are equivariantly isomorphic to an additive lattice by the [p-adic logarithm](arithmetic.md#p-adic-logarithm). The [normal basis theorem](galois-theory.md#normal-basis-theorem) makes its [Herbrand quotient](#herbrand-quotient) one. Passing across finite unit quotients preserves it. The valuation exact sequence with quotient $\mathbb Z$ therefore gives the displayed formula.

### Corestriction map in group cohomology

↑ **Parent:** [Group cohomology](#group-cohomology)

For an open finite-index subgroup $U$ of a [profinite group](topological-group.md#profinite-group) $G$ and a discrete $G$-module $M$, cohomological transfer gives $\operatorname{Cor}_U^G:H^q(U,M)\to H^q(G,M)$. In degree zero it is the sum over cosets, or the norm for multiplicative coefficients. It is transitive and satisfies $\operatorname{Cor}\operatorname{Res}=[G:U]$ and the cup-product projection formula.

### Continuous cohomology of a profinite group

↑ **Parent:** [Group cohomology](#group-cohomology)

For a [profinite group](topological-group.md#profinite-group) and a discrete module with continuous action, continuous cohomology is computed by continuous cochains. On a compact domain these cochains have finite image. Positive-degree classes become zero on a sufficiently small open subgroup and hence are torsion by restriction followed by corestriction.

#### Cohomology continuity at closed subgroups

↑ **Parent:** [Continuous cohomology of a profinite group](#continuous-cohomology-of-a-profinite-group)

For a closed subgroup $P$ of a [profinite group](topological-group.md#profinite-group) $G$ and a discrete $G$-module $M$, restriction gives $H^q(P,M)=\varinjlim_{U\supseteq P,\ U\ \mathrm{open}}H^q(U,M)$. Thus a class restricting to zero on $P$ already restricts to zero on one such open subgroup. The property follows by extending continuous finite-image cochains and their identities to a sufficiently small open neighborhood of $P$.

#### Cohomological dimension at a prime

↑ **Parent:** [Continuous cohomology of a profinite group](#continuous-cohomology-of-a-profinite-group)

The value $\operatorname{cd}_p(G)$ is the least $n$ such that all cohomology in degrees greater than $n$ vanishes for every discrete $p$-primary torsion module. Vanishing in degree $n+1$ for all such modules suffices by dimension shifting. Dimension does not increase on closed subgroups. For a field, use its [absolute Galois group](galois-theory.md#absolute-galois-group).

##### Trivial coefficients detect the cohomological dimension of a pro-p group

↑ **Parent:** [Cohomological dimension at a prime](#cohomological-dimension-at-a-prime)

For a [pro-p group](topological-group.md#pro-p-group) $P$, vanishing of $H^{n+1}(P,\mathbb F_p)$ implies vanishing in that degree for every discrete $p$-primary module. Finite such modules have composition factors equal to the trivial module $\mathbb F_p$, so the long exact sequence gives the result by induction. General modules are unions of finite stable submodules, and continuous cohomology commutes with filtered unions. Dimension shifting gives $\operatorname{cd}_p(P)\le n$. The converse is immediate from the definition.

##### Characteristic p Galois dimension bound

↑ **Parent:** [Cohomological dimension at a prime](#cohomological-dimension-at-a-prime)

A field of characteristic $p$ satisfies $\operatorname{cd}_p(K)\le1$. The Artin-Schreier sequence and vanishing of positive-degree cohomology of the additive separable-closure module yield the bound. It concerns discrete $p$-primary modules; it does not assert that the $p$-primary [Brauer group](associative-algebra.md#brauer-group) vanishes.

### Nonabelian first cohomology

↑ **Parent:** [Group cohomology](#group-cohomology)

For a group $G$ acting by automorphisms on a possibly noncommutative group $B$, $H^1(G,B)$ is the pointed set of maps satisfying $c_{\sigma\tau}=c_\sigma\sigma(c_\tau)$ modulo $c_\sigma\mapsto b c_\sigma\sigma(b)^{-1}$. It classifies twisting of a reference action. It need not be an abelian group.

### Periodic group cohomology

↑ **Parent:** [Group cohomology](#group-cohomology)

For a finite group, the usual integral notion asks for a class $\Delta\in H^n(G;\mathbb Z)$ whose [cup product](cohomology.md#cup-product) gives the displayed isomorphisms for every coefficient module $M$ and every $i>0$. The analogous claim for just trivial coefficients over a fixed field is weaker and should be stated as such. A free cohomologically orientation-preserving sphere action supplies that field-coefficient version through [periodic group cohomology from a free sphere action](#periodic-group-cohomology-from-a-free-sphere-action).

#### Cohomology ring of a finite cyclic group over its prime field

↑ **Parent:** [Periodic group cohomology](#periodic-group-cohomology)

The alternating resolution maps $g-1$ and $1+g+\cdots+g^{p-1}$ for a [cyclic group](group.md#cyclic-group) $C_p$ become zero after applying homomorphisms to its trivial [prime field](algebra.md#prime-field) module. Thus there is one class in every degree. A two-step shift of the resolution represents a degree-two periodicity class $u$. For odd $p$, a degree-one class $v$ squares to zero by graded commutativity, and

$$
H^*(BC_p;\mathbb F_p)=\Lambda_{\mathbb F_p}(v)\otimes\mathbb F_p[u],\qquad |v|=1,\ |u|=2.
$$

One can take $u=\beta(v)$ for the [Bockstein homomorphism](homology.md#bockstein-homomorphism). For $p=2$ the two maps agree over $\mathbb F_2[C_2]$, so a one-step shift gives $H^*(BC_2;\mathbb F_2)=\mathbb F_2[v]$ with $|v|=1$. The [Künneth theorem](cohomology.md#kunneth-theorem) then gives dimension $i+1$ in degree $i$ for $B(C_p\times C_p)$, obstructing [periodic group cohomology](#periodic-group-cohomology) and hence such a free sphere action.

#### Periodic group cohomology from a free sphere action

↑ **Parent:** [Periodic group cohomology](#periodic-group-cohomology)

Suppose a finite group acts freely on $S^{n-1}$ and trivially on its integral [cohomology](cohomology.md). The [Borel construction](cohomology.md#borel-construction) gives a sphere fibration over $BG$ whose total space is homotopy equivalent to the $(n-1)$-dimensional quotient. Its [Serre spectral sequence](algebraic-topology.md#serre-spectral-sequence) has just two rows with trivial local coefficients. Transgressing the fibre generator gives $\Delta$; the sole differential is multiplication by it up to sign. For $i>0$, both the source and target terms have total degrees above $n-1$, so their surviving kernel and cokernel must vanish. Hence multiplication by $\Delta$ gives period $n$ in positive-degree cohomology over any field.

### Projective-resolution definition of group cohomology

↑ **Parent:** [Group cohomology](#group-cohomology)

Choose a [projective resolution](algebra.md#projective-resolution) $P_\bullet\to\mathbb Z$ of the trivial $\mathbb ZG$-module. For a $\mathbb ZG$-module $M$, [group cohomology](#group-cohomology) is

$$
H^n(G,M)=H^n\!\left(\operatorname{Hom}_{\mathbb ZG}(P_\bullet,M)\right)
=\operatorname{Ext}_{\mathbb ZG}^n(\mathbb Z,M).
$$

Different [projective resolutions](algebra.md#projective-resolution) give naturally isomorphic groups.

#### Group cohomology commutes with finite direct sums

↑ **Parent:** [Projective-resolution definition of group cohomology](#projective-resolution-definition-of-group-cohomology)

For $\mathbb ZG$-modules $M_1,M_2$,

$$
H^n(G,M_1\oplus M_2)\cong H^n(G,M_1)\oplus H^n(G,M_2),
$$

because the [Hom functor](algebra.md#hom-functor) into a finite [direct sum](vector-space.md#direct-sum) splits degree by degree and taking [cohomology](cohomology.md) preserves that splitting.

#### Koszul resolution for a rank-two free abelian group

↑ **Parent:** [Projective-resolution definition of group cohomology](#projective-resolution-definition-of-group-cohomology)

For $G=\langle x,y\mid xy=yx\rangle$, the trivial $\mathbb ZG$-module has the free resolution

$$
0\longrightarrow\mathbb ZG\xrightarrow{\binom{1-y}{x-1}}(\mathbb ZG)^2
\xrightarrow{(x-1\quad y-1)}\mathbb ZG\longrightarrow\mathbb Z\longrightarrow0.
$$

##### Second cohomology of a rank-two free abelian group with truncated group-ring coefficients

↑ **Parent:** [Koszul resolution for a rank-two free abelian group](#koszul-resolution-for-a-rank-two-free-abelian-group)

If $G\cong\mathbb Z^2$, $I$ is the augmentation ideal, and $M=\mathbb ZG/I^2$, then

$$
H^2(G,M)\cong M/IM\cong\mathbb Z.
$$

The quotient map $M\to\mathbb ZG/I\cong\mathbb Z$ induces an isomorphism in second cohomology.

### Coinduced module

↑ **Parent:** [Group cohomology](#group-cohomology)

For a subgroup $K\leq G$ and a $\mathbb ZK$-module $X$, the coinduced module is

$$
\operatorname{Coind}_K^G X=\operatorname{Hom}_{\mathbb ZK}(\mathbb ZG,X),
\qquad (g f)(r)=f(rg).
$$

<h4 id="shapiro-s-lemma">Shapiro's lemma</h4>

↑ **Parent:** [Coinduced module](#coinduced-module)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shapiro's_lemma)

[Shapiro's lemma](#shapiro-s-lemma) gives a natural isomorphism

$$
H^n\!\left(G,\operatorname{Coind}_K^G X\right)\cong H^n(K,X).
$$

It follows by applying the [Hom functor adjunction for a coinduced module](#hom-functor-adjunction-for-a-coinduced-module) to a [projective resolution](algebra.md#projective-resolution) and observing that restriction from $G$ to $K$ preserves [projective modules](module-theory.md#projective-module).

##### Hom functor adjunction for a coinduced module

↑ **Parent:** [Shapiro's lemma](#shapiro-s-lemma)

For a $\mathbb ZG$-module $P$ and a $\mathbb ZK$-module $X$,

$$
\operatorname{Hom}_{\mathbb ZG}\!\left(P,\operatorname{Hom}_{\mathbb ZK}(\mathbb ZG,X)\right)
\cong\operatorname{Hom}_{\mathbb ZK}(P,X).
$$

Evaluation at $1\in G$ gives the forward map. If $a:P\to X$ is $\mathbb ZK$-linear, its inverse sends $a$ to $p\mapsto(r\mapsto a(rp))$.

### Conjugation module of a group ring

↑ **Parent:** [Group cohomology](#group-cohomology)

The [group ring](commutative-algebra.md#group-ring) $\mathbb ZG$ becomes a $\mathbb ZG$-module under the [conjugation action](#conjugation-action) $g\cdot x=gxg^{-1}$. Its basis splits into [conjugacy classes](#conjugacy-class), and the span of the class of $x$ is the permutation module on $G/C_G(x)$.

#### Group cohomology of a conjugation module

↑ **Parent:** [Conjugation module of a group ring](#conjugation-module-of-a-group-ring)

For a [finite group](group.md#finite-group) $G$ and representatives $g_i$ of its [conjugacy classes](#conjugacy-class), [Shapiro's lemma](#shapiro-s-lemma) gives

$$
H^n(G,\mathbb ZG_{\mathrm{conj}})
\cong\bigoplus_iH^n(C_G(g_i),\mathbb Z).
$$

### Integral cohomology of a finite cyclic group

↑ **Parent:** [Group cohomology](#group-cohomology)

For the trivial action of the [finite cyclic group](group.md#finite-cyclic-group) $C_m$ on $\mathbb Z$,

$$
H^0(C_m,\mathbb Z)=\mathbb Z,
\qquad H^{2k+1}(C_m,\mathbb Z)=0,
\qquad H^{2k}(C_m,\mathbb Z)=\mathbb Z/m\mathbb Z
$$

for $k\geq1$. The [periodic resolution of a finite cyclic group](#periodic-resolution-of-a-finite-cyclic-group) proves this directly.

#### Periodic resolution of a finite cyclic group

↑ **Parent:** [Integral cohomology of a finite cyclic group](#integral-cohomology-of-a-finite-cyclic-group)

If $C_m=\langle t\rangle$ and $N=1+t+\cdots+t^{m-1}$, a [free resolution](algebra.md#free-resolution) of the trivial $\mathbb ZC_m$-module alternates multiplication by $t-1$ and $N$. Applying $\operatorname{Hom}_{\mathbb ZC_m}(-,\mathbb Z)$ for the trivial action alternates the zero map and multiplication by $m$.

### Group extension

↑ **Parent:** [Group cohomology](#group-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_extension)

A group extension of $G$ by an abelian $G$-module $A$ is a [short exact sequence](module-theory.md#short-exact-sequence)

$$
1\longrightarrow A\longrightarrow E\longrightarrow G\longrightarrow1
$$

whose conjugation action on $A$ is the specified $G$-action.

#### Torsion-free finite extension of a lattice

↑ **Parent:** [Group extension](#group-extension)

For a specified [finite group](group.md#finite-group) action on $A=\mathbb Z^n$, extensions are classified by $e\in H^2(Q,A)$. For an element $q$ of prime order $p$, a lift $g$ satisfies $g^p=a\in A^q$; changing the lift changes $a$ by $N_qv=(1+q+\cdots+q^{p-1})v$. Thus the extension is torsion-free precisely when every restriction to a prime-order cyclic subgroup is nonzero in $A^q/N_qA$. Any finite-order element has a prime-order power, so this tests all torsion. An arbitrary finite quotient must not be confused with faithful holonomy on a maximal translation lattice.

#### Split group extension

↑ **Parent:** [Group extension](#group-extension)

A [group extension](#group-extension) is split when its quotient homomorphism admits a group-homomorphic section. Equivalently, the middle group is a [semidirect product](#semidirect-product) of the kernel by the quotient.

##### Section normal form for a split group extension

↑ **Parent:** [Split group extension](#split-group-extension)

If a [group homomorphism](#group-homomorphism) section $i:G/N\to G$ satisfies $\pi i=\mathrm{id}$, then each $g\in G$ has a unique form $i(q)n$ with $q\in G/N$ and $n\in N$: take $q=\pi(g)$ and $n=i(q)^{-1}g$. Thus $(q,n)\mapsto i(q)n$ is a bijection. It is a homomorphism for the ordinary [direct product of groups](#direct-product-of-groups) exactly when the section image centralizes $N$. In general it describes a [semidirect product](#semidirect-product) with a nontrivial conjugation action.

#### Equivalent group extensions

↑ **Parent:** [Group extension](#group-extension)

Two extensions of $G$ by the same $G$-module $M$ are equivalent when an isomorphism between their middle groups commutes with the inclusions of $M$ and the projections to $G$. Splitness is preserved under this equivalence.

#### Fiber product of groups

↑ **Parent:** [Group extension](#group-extension)

For homomorphisms $E\to H$ and $G\to H$, their fiber product is

$$
E\times_HG=\{(e,g)\in E\times G:\pi(e)=f(g)\}.
$$

It is a subgroup of $E\times G$. Pulling a [group extension](#group-extension) back along $G\to H$ uses this fiber product as its middle group.

##### Mihailova subgroup

↑ **Parent:** [Fiber product of groups](#fiber-product-of-groups)

For a [finite group presentation](geometric-group-theory.md#finite-group-presentation) $H=\langle x_1,\ldots,x_m\mid r_1,\ldots,r_n\rangle$, let $F$ be the free group on its generators and $\pi:F\to H$. The corresponding [fiber product of groups](#fiber-product-of-groups) is generated by $(x_i,x_i)$ and $(1,r_j)$. Conjugation by the diagonal pairs supplies every pair $(1,r)$ with $r$ in the [normal closure](#normal-closure) of the relators, and $(u,v)=(u,u)(1,u^{-1}v)$ proves the generating claim. Membership of $(1,w)$ is equivalent to $w=1$ in $H$, so this finitely generated subgroup can have undecidable membership even though $F\times F$ has soluble word problem.

#### Second group cohomology classifies group extensions

↑ **Parent:** [Group extension](#group-extension)

Equivalence classes of [group extensions](#group-extension) of $G$ by an abelian $G$-module $A$ correspond to $H^2(G,A)$. A section $s:G\to E$ produces the [extension cocycle](#extension-cocycle)

$$
c(g,h)=s(g)s(h)s(gh)^{-1},
$$

and changing the section changes $c$ by a [group coboundary](#group-coboundary).

##### Integral central extensions of a rank-two free abelian group

↑ **Parent:** [Second group cohomology classifies group extensions](#second-group-cohomology-classifies-group-extensions)

With a fixed identification of the kernel with $\mathbb Z$ and quotient with $\mathbb Z^2$, these central [group extensions](#group-extension) are classified by $n\in\mathbb Z$. Choose lifts $x,y$ of the quotient generators; their commutator is $z^n$ and is unchanged by central changes of lifts. Every element has unique normal form $z^my^bx^a$, proving this invariant is complete. A cocycle representative is $c((a,b),(c,d))=nad$, whose cocycle identity follows from bilinearity. Its extension multiplication is $(a,b,m)(c,d,l)=(a+c,b+d,m+l+nad)$. The zero parameter gives $\mathbb Z^3$ and parameter one gives the integer Heisenberg group. The [Koszul resolution for a rank-two free abelian group](#koszul-resolution-for-a-rank-two-free-abelian-group) independently computes $H^2(\mathbb Z^2,\mathbb Z)\cong\mathbb Z$.

##### Extension cocycle

↑ **Parent:** [Second group cohomology classifies group extensions](#second-group-cohomology-classifies-group-extensions)

An extension cocycle is the [two-cocycle](#two-cocycle) obtained from a section of a [group extension](#group-extension). It measures the failure of the section to be a [group homomorphism](#group-homomorphism).

### Group cocycle

↑ **Parent:** [Group cohomology](#group-cohomology)

A group cocycle is an element of the kernel of the coboundary map in the standard cochain complex computing [group cohomology](#group-cohomology).

#### One-cocycle

↑ **Parent:** [Group cocycle](#group-cocycle)

For a $G$-module $M$, a one-cocycle is a map $f:G\to M$ satisfying $f(gh)=f(g)+g\cdot f(h)$.

##### Galois 1-cocycle

↑ **Parent:** [One-cocycle](#one-cocycle)

A continuous one-cocycle for a Galois group acting on an abelian module $M$ is a map satisfying the displayed identity. Cocycles modulo maps $\sigma\mapsto\sigma u-u$ form $H^1(K,M)$ in [Galois cohomology](galois-theory.md#galois-cohomology). For an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve), choosing $mQ=P$ gives the cocycle $\sigma\mapsto\sigma Q-Q$ in $E[m]$, which represents the [Kummer map of an elliptic curve](normalization-of-an-algebraic-curve.md#kummer-map-of-an-elliptic-curve).

##### Crossed homomorphism

↑ **Parent:** [One-cocycle](#one-cocycle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Crossed_homomorphism)

A crossed homomorphism from $G$ to a $G$-module $M$ is a map $f:G\to M$ satisfying

$$
f(gh)=f(g)+g\cdot f(h).
$$

Thus crossed homomorphisms are precisely [one-cocycles](#one-cocycle).

###### Principal crossed homomorphism

↑ **Parent:** [Crossed homomorphism](#crossed-homomorphism)

For $m\in M$, the map $g\mapsto g\cdot m-m$ is a principal crossed homomorphism. It is the [group coboundary](#group-coboundary) of the zero-cochain $m$, so first [group cohomology](#group-cohomology) is the quotient of crossed homomorphisms by principal crossed homomorphisms.

#### Two-cocycle

↑ **Parent:** [Group cocycle](#group-cocycle)

For a $G$-module $M$, a two-cocycle is a map $c:G\times G\to M$ satisfying

$$
g\cdot c(h,k)-c(gh,k)+c(g,hk)-c(g,h)=0.
$$

##### Normalized two-cocycle

↑ **Parent:** [Two-cocycle](#two-cocycle)

A two-cocycle is normalized when $c(1,g)=c(g,1)=0$ in additive notation, or $c(1,g)=c(g,1)=1$ in multiplicative notation.

### Group coboundary

↑ **Parent:** [Group cohomology](#group-cohomology)

A group coboundary is a cochain in the image of the preceding coboundary map. Quotienting [group cocycles](#group-cocycle) by group coboundaries gives [group cohomology](#group-cohomology).

### Group cochain

↑ **Parent:** [Group cohomology](#group-cohomology)

An inhomogeneous group $n$-cochain with values in a $G$-module $M$ is a function $G^n\to M$. The standard alternating [group coboundary](#group-coboundary) turns these groups into the cochain complex whose cohomology is $H^n(G,M)$.

### Long exact sequence in group cohomology

↑ **Parent:** [Group cohomology](#group-cohomology)

A [short exact sequence](module-theory.md#short-exact-sequence) $0\to M_1\to M_2\to M_3\to0$ of $G$-modules induces a natural long exact sequence

$$
0\to H^0(G,M_1)\to H^0(G,M_2)\to H^0(G,M_3)
\to H^1(G,M_1)\to\cdots.
$$

It follows by applying the cochain functor and the long exact cohomology sequence of a short exact sequence of cochain complexes.

### Finite-group cohomology is annihilated by the group order

↑ **Parent:** [Group cohomology](#group-cohomology)

If $G$ is finite and $n>0$, multiplication by $|G|$ annihilates $H^n(G,M)$. Indeed, restriction to the trivial subgroup is zero in positive degree, while the restriction-corestriction composite is multiplication by $|G|$.

#### Restriction-corestriction identity in group cohomology

↑ **Parent:** [Finite-group cohomology is annihilated by the group order](#finite-group-cohomology-is-annihilated-by-the-group-order)

For a subgroup $K\leq G$, restriction followed by corestriction acts on group cohomology as the sum over coset translates. For $K$ trivial, inner automorphisms act trivially on cohomology, so this sum is multiplication by $|G|$.

### Mac Lane exact sequence for a free presentation

↑ **Parent:** [Group cohomology](#group-cohomology)

For a free presentation $G=F/R$ and a $\mathbb ZG$-module $M$, restriction of derivations to $R$ gives an exact sequence

$$
H^1(F,M)\longrightarrow\operatorname{Hom}_G(R/[R,R],M)
\longrightarrow H^2(G,M)\longrightarrow0.
$$

It follows by applying $\operatorname{Hom}_{\mathbb ZG}(-,M)$ to the presentation relation sequence.

<h3 id="lyndon-hochschild-serre-spectral-sequence">Lyndon–Hochschild–Serre spectral sequence</h3>

↑ **Parent:** [Group cohomology](#group-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lyndon–Hochschild–Serre_spectral_sequence)

For a [normal subgroup](#normal-subgroup) $H\triangleleft G$, quotient $Q=G/H$, and a $G$-module $M$, the Lyndon–Hochschild–Serre spectral sequence has

$$
E_2^{p,q}=H^p(Q,H^q(H,M))\Longrightarrow H^{p+q}(G,M).
$$

#### Cyclic-extension shift of group-ring cohomology

↑ **Parent:** [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence)

If $N$ has a finite resolution by finitely generated projective modules, restriction of the semidirect-product group ring gives a direct sum of copies of $\mathbb ZN$, indexed by the integers. On its kernel cohomology the cyclic generator shifts those copies, possibly twisting each copy by an automorphism. Invariants are zero because elements have finite support; coinvariants identify with a single copy. The two-column [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence) therefore gives the displayed isomorphism of abelian groups. A group with such a finite resolution and cohomological dimension $d$ has $H^d(N;\mathbb ZN)\ne0$, so the cyclic extension has dimension $d+1$.

#### Five-term exact sequence in group cohomology

↑ **Parent:** [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence)

The low-degree edge maps of the [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence) give

$$
0\to H^1(Q,M^H)\xrightarrow{\mathrm{inf}}H^1(G,M)
\xrightarrow{\mathrm{res}}H^1(H,M)^Q
\xrightarrow{d_2}H^2(Q,M^H)
\xrightarrow{\mathrm{inf}}H^2(G,M).
$$

##### Inflation-restriction exact sequence

↑ **Parent:** [Five-term exact sequence in group cohomology](#five-term-exact-sequence-in-group-cohomology)

For a normal subgroup $N$ of $G$ and a $G$-module $M$, the low-degree exact sequence begins $0\to H^1(G/N,M^N)\to H^1(G,M)\to H^1(N,M)^{G/N}\to H^2(G/N,M^N)$. The first map inflates cocycles along $G\to G/N$; the second restricts them. If the restriction is trivial, subtract a coboundary to make the cocycle vanish on $N$ and descend to the quotient. Thus for a finite Galois extension, the kernel of restriction on [Galois cohomology](galois-theory.md#galois-cohomology) with finite coefficients is finite.

##### Inflation map in group cohomology

↑ **Parent:** [Five-term exact sequence in group cohomology](#five-term-exact-sequence-in-group-cohomology)

Inflation composes a cocycle on the quotient $Q=G/H$ with the quotient map $G\to Q$ and regards its values in the invariant submodule $M^H$ as values in $M$.

##### Restriction map in group cohomology

↑ **Parent:** [Five-term exact sequence in group cohomology](#five-term-exact-sequence-in-group-cohomology)

Restriction sends a cocycle on $G$ to its restriction to a subgroup $H$. If $H$ is normal, its image in $H^1(H,M)$ is fixed by the induced $G/H$-action.

##### Transgression in group cohomology

↑ **Parent:** [Five-term exact sequence in group cohomology](#five-term-exact-sequence-in-group-cohomology)

The transgression $d_2:H^1(H,M)^Q\to H^2(Q,M^H)$ is the first differential crossing from the vertical to the horizontal edge of the [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence). If a representative on $H$ is extended to a cochain on $G$, its coboundary descends to the representing two-cocycle on $Q$.

#### Integral cohomology of the dihedral group of order ten

↑ **Parent:** [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence)

For the dihedral group $D_{10}=C_5\rtimes C_2$,

$$
H^n(D_{10},\mathbb Z)\cong
\begin{cases}
\mathbb Z,&n=0,\\
0,&n\text{ odd},\\
\mathbb Z/2,&n\equiv2\pmod4,\\
\mathbb Z/10,&n>0\text{ and }n\equiv0\pmod4.
\end{cases}
$$

The Lyndon–Hochschild–Serre spectral sequence proves this from the inversion action of $C_2$ on $H^2(C_5,\mathbb Z)$.

## Group homology

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_homology)

Group homology is obtained by tensoring a [projective resolution](algebra.md#projective-resolution) of the trivial $\mathbb ZG$-module with a coefficient module and taking [homology](homology.md).

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

A group $G$ is conjugacy separable when any two nonconjugate elements remain nonconjugate in some finite quotient. Equivalently, every [conjugacy class](#conjugacy-class) is closed in the [profinite topology](topological-group.md#profinite-topology).

### Subgroup of a residually finite group

↑ **Parent:** [Residually finite group](#residually-finite-group)

Every subgroup of a residually finite group is residually finite, because a finite quotient separating an element of the ambient group also separates it after restriction to the subgroup.

### Reduction modulo a prime in an integral matrix group

↑ **Parent:** [Residually finite group](#residually-finite-group)

For a [prime number](number-theory.md#prime-number) $p$, reducing every entry modulo $p$ defines a [group homomorphism](#group-homomorphism) from an integral matrix group to the corresponding matrix group over $\mathbb F_p$. The target is finite. If an integral matrix $M$ is not the identity, choosing $p$ not to divide one nonzero entry of $M-I$ ensures that its reduction is also nonidentity.

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

For an [abelian group](group.md#abelian-group) $G$ and an integer $m\geq1$, its $m$-torsion subgroup is $G[m]=\{x\in G:mx=0\}$, the kernel of multiplication by $m$. In a [finite abelian group](group.md#finite-abelian-group), every nonempty fiber of this homomorphism has [cardinality](set-theory.md#cardinality) $|G[m]|$, so $|G:mG|=|G[m]|$. This follows directly: if $mx=my$, then $x-y\in G[m]$, and conversely translating by an element of $G[m]$ leaves the image unchanged. On the [cyclic group](group.md#cyclic-group) $\mathbb Z_N$, the solutions of $mx=0$ number $\gcd(m,N)$; divide both integers by their greatest common divisor to see that $x$ must be a multiple of $N/\gcd(m,N)$.

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

A nonzero element of a [free abelian group](#free-abelian-group) is primitive when it is part of an integral basis, equivalently when some homomorphism to $\mathbb Z$ takes it to one. Its coordinates have [greatest common divisor](number-theory.md#greatest-common-divisor) one. This lattice meaning differs from a [primitive homology class](homology.md#primitive-homology-class) in the coalgebra sense.

## Normal subgroup

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_subgroup)

A subgroup $N\le G$ is normal when $gNg^{-1}=N$ for every $g\in G$.

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

The socle is generated by all minimal nontrivial normal subgroups. Distinct minimal normal subgroups commute and meet trivially, although in the abelian case not every collection of them is an independent direct-product decomposition. It is a direct product of simple groups. In a faithful primitive permutation group each nontrivial normal subgroup is transitive; its minimal normal subgroups are either elementary abelian and regular, or direct powers of a nonabelian simple group. This is the starting point of the [O'Nan–Scott theorem](#o-nan-scott-theorem).

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

The Möbius group is the [group](group.md) of all [Möbius transformations](#mobius-transformation) of the [Riemann sphere](complex-analysis.md#riemann-sphere), under [function composition](algebra.md#function-composition). An invertible $2\times2$ complex matrix represents $z\mapsto(az+b)/(cz+d)$, and nonzero scalar multiples represent the same transformation. Rescaling a representative to determinant one gives a surjective [group homomorphism](#group-homomorphism) $SL_2(\mathbb C)\to\mathcal M$ with [kernel of a group homomorphism](#kernel-of-a-group-homomorphism) $\{I,-I\}$. Thus it is also the [projective linear group](#projective-linear-group) $PGL_2(\mathbb C)$ and the quotient $PSL_2(\mathbb C)=SL_2(\mathbb C)/\{\pm I\}$.

<h4 id="mobius-pointwise-stabilizer-of-two-points">Möbius pointwise stabilizer of two points</h4>

↑ **Parent:** [Möbius group](#mobius-group)

For two distinct points of the [Riemann sphere](complex-analysis.md#riemann-sphere), conjugate by a [Möbius transformation](#mobius-transformation) sending them to zero and infinity. A transformation fixing those two points has the form $z\mapsto\lambda z$, $\lambda\ne0$. Composition multiplies the parameter, so the [pointwise stabilizer](#pointwise-stabilizer) is isomorphic to the [complex multiplicative group](group.md#complex-multiplicative-group). For zero and one, conjugation by $z/(1-z)$ gives $z\mapsto\lambda z/[1+(\lambda-1)z]$.

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

Let $T_a(z)=z+a$, $S_k(z)=kz$ with $k\ne0$, and $I(z)=1/z$ on the [Riemann sphere](complex-analysis.md#riemann-sphere). For $F(z)=(az+b)/(cz+d)$ and $\Delta=ad-bc\ne0$, $c=0$ gives $F=T_{b/d}\circ S_{a/d}$. If $c\ne0$, division gives $F=T_{a/c}\circ S_{-\Delta/c^2}\circ I\circ T_{d/c}$. The expressions agree at poles and at infinity by the sphere conventions. These elementary maps therefore generate the [Möbius transformation](#mobius-transformation) group.

<h4 id="antipodal-fixed-point-classification-of-mobius-transformations">Antipodal fixed-point classification of Möbius transformations</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

For a nonidentity [Möbius transformation](#mobius-transformation) whose two fixed points are antipodal under [stereographic projection](complex-analysis.md#stereographic-projection), conjugate by a sphere rotation sending them to $0,\infty$. The conjugated map fixes both, hence is $z\mapsto az$ with $a\ne0$. If $|a|=1$ it is an axial rotation; if $|a|<1$ every finite orbit tends to zero; if $|a|>1$ every nonzero orbit tends to infinity. Undoing the rotation gives either a sphere rotation or one attracting fixed point with the other as the sole exceptional initial point.

<h4 id="mobius-conjugacy-normal-forms">Möbius conjugacy normal forms</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

A nonidentity [Möbius transformation](#mobius-transformation) has one or two distinct [fixed points](function.md#fixed-point) on the [Riemann sphere](complex-analysis.md#riemann-sphere). If there are two, send them to zero and infinity; the conjugated map fixes both and is a nonzero scaling. If there is one, send it to infinity; the resulting affine map cannot have slope different from one, since that would give another fixed point. It is a nonzero translation, which a scaling conjugates to $z+1$. The identity is the scaling $\mu=1$. Fixed-point sets are carried bijectively under conjugacy, so a translation is not conjugate to a scaling.

<h5 id="iteration-of-a-one-fixed-point-mobius-transformation">Iteration of a one-fixed-point Möbius transformation</h5>

↑ **Parent:** [Möbius conjugacy normal forms](#mobius-conjugacy-normal-forms)

A nonidentity [Möbius transformation](#mobius-transformation) with only one [fixed point](function.md#fixed-point) is conjugate to a nonzero translation of the [Riemann sphere](complex-analysis.md#riemann-sphere). Its translation iterates are $z+nb$, tending to infinity in the topology of the [Riemann sphere](complex-analysis.md#riemann-sphere) for finite $z$, with infinity itself fixed. Conjugating back proves that every point tends to the unique [fixed point](function.md#fixed-point). This is convergence on the [sphere](geometry-and-topology.md#sphere); if the [fixed point](function.md#fixed-point) is finite, intermediate iterates can still pass through infinity.

<h5 id="finite-order-mobius-orbit-sizes">Finite-order Möbius orbit sizes</h5>

↑ **Parent:** [Möbius conjugacy normal forms](#mobius-conjugacy-normal-forms)

A nonidentity [Möbius transformation](#mobius-transformation) of finite order $n$ is conjugate to multiplication by a primitive $n$th [root of unity](algebra.md#root-of-unity). Zero and infinity are fixed; for any other point, a return after $k$ iterates requires $\mu^k=1$, whose least positive solution is $n$. Thus its only orbit sizes are one and $n$. For the identity, every orbit has size one. This is a direct orbit computation, independent of an appeal to the orbit-stabilizer theorem.

#### Cayley transform (complex analysis)

↑ **Parent:** [Möbius transformation](#mobius-transformation)

This [Möbius transformation](#mobius-transformation) maps the [upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) onto the [unit disk](geometry-and-topology.md#unit-disk). For $\operatorname{Im}z>0$, the identity $1-|C(z)|^2=4\operatorname{Im}z/|z+i|^2$ puts the image inside the [unit disk](geometry-and-topology.md#unit-disk). Its inverse is $z=i(1+w)/(1-w)$, so the map is a [conformal bijection](complex-analysis.md#biholomorphism). On the extended real boundary it maps onto the [unit circle](complex-analysis.md#complex-unit-circle). It is the scalar complex-analytic version of a Cayley map, rather than the matrix parametrization used in [Cayley transform](lie-theory.md#cayley-transform-lie-theory).

<h4 id="mobius-transformations-from-the-real-axis-to-the-unit-circle">Möbius transformations from the real axis to the unit circle</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

A nonconstant [Möbius transformation](#mobius-transformation) mapping the [real line](real-analysis.md#real-line) into the [unit circle](complex-analysis.md#complex-unit-circle) has the displayed form with $|\lambda|=1$ and $k$ nonreal. Indeed $|ax+b|^2=|cx+d|^2$ for real $x$ yields $|a|=|c|\ne0$, $|b/a|=|d/c|$ and $\operatorname{Re}(b/a)=\operatorname{Re}(d/c)$. Thus $d/c$ is $b/a$ or its [complex conjugate](complex-analysis.md#complex-conjugate); the first possibility makes the map constant, so the second is necessary. Conjugate numerator and denominator have equal modulus on the [real line](real-analysis.md#real-line), proving the converse as well.

<h4 id="mobius-scaling-generated-by-translations-and-reciprocal-inversion">Möbius scaling generated by translations and reciprocal inversion</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

Let $T_b(z)=z+b$ and $I(z)=1/z$ on the [Riemann sphere](complex-analysis.md#riemann-sphere). For $s\ne0$, direct composition gives the displayed identity. Every nonzero complex scaling $z\mapsto\lambda z$ is obtained by choosing $s^2=-\lambda$. Since translations, scalings and reciprocal inversion generate the [Möbius group](#mobius-group), translations and reciprocal inversion alone also generate it.

#### Blaschke factor

↑ **Parent:** [Möbius transformation](#mobius-transformation)

For $|w|<R$, this [Möbius transformation](#mobius-transformation) maps the radius-$R$ disc to the unit disc, vanishes at $w$ and has modulus one on the boundary. Expanding gives $|R^2-\overline wz|^2=R^2|z-w|^2$ when $|z|=R$; its [pole](isolated-singularity.md#pole) lies outside the disc. Dividing a [holomorphic function](complex-analysis.md#holomorphic-function) by factors corresponding to its interior zeros removes those zeros without changing its boundary modulus. This gives a direct factorization proof of [Jensen's formula](complex-analysis.md#jensen-s-formula).

#### Antipodal fixed points do not characterize sphere rotations

↑ **Parent:** [Möbius transformation](#mobius-transformation)

The [Möbius transformation](#mobius-transformation) $M(z)=(3z-1)/(3-z)$ fixes the [antipodal pair](geometry-and-topology.md#antipodal-pair) $1,-1$ under [stereographic projection](complex-analysis.md#stereographic-projection). But $M'(1)=2$, so it multiplies infinitesimal spherical lengths at that fixed point by two, as follows from the round line element $2|dz|/(1+|z|^2)$. It is not an [isometry](riemannian-geometry.md#isometry) and hence not a sphere [rotation](riemannian-geometry.md#rotation-mathematics). Fixing an [antipodal pair](geometry-and-topology.md#antipodal-pair) is therefore necessary for a nontrivial rotational [Möbius transformation](#mobius-transformation), but is not sufficient.

<h4 id="loxodromic-mobius-transformation">Loxodromic Möbius transformation</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

A [Möbius transformation](#mobius-transformation) with two distinct fixed points is conjugate to $z\mapsto az$. It is loxodromic when $|a|\ne1$; on three-dimensional [hyperbolic space](geometry-and-topology.md#hyperbolic-space) it translates along the axis joining its fixed points and rotates around that axis by $\arg a$. The positive-real multiplier case has no rotation and is also called hyperbolic. When listing elliptic, parabolic, hyperbolic and loxodromic as separate types, loxodromic refers to the remaining case with nonzero rotation. A determinant-one matrix with nonreal [trace](linear-algebra.md#matrix-trace) has reciprocal [eigenvalues](linear-operator-theory.md#eigenvalue) that are neither real nor of modulus one, so it supplies this latter case.

<h4 id="real-determinant-one-mobius-orbits">Real determinant-one Möbius orbits</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

The [special linear group](#special-linear-group) $SL_2(\mathbb R)$ acting by [Möbius transformations](#mobius-transformation) has exactly three [group orbits](#orbit-of-a-group-action) on the [Riemann sphere](complex-analysis.md#riemann-sphere): the extended real line and the two open half-planes. The identity $\operatorname{Im}((az+b)/(cz+d))=\operatorname{Im}z/|cz+d|^2$ preserves these sets. Upper triangular determinant-one matrices send $i$ to any prescribed point of the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), and similarly send $-i$ through the lower half-plane. The [stabilizer subgroups](#stabilizer-subgroup) of $i$ and $-i$ are both $SO(2)$.

#### Concentric normalization of disjoint circles

↑ **Parent:** [Möbius transformation](#mobius-transformation)

Two disjoint ordinary [circle](topology.md#circle) boundaries can be taken to distinct concentric [circles](topology.md#circle) by a [Möbius transformation](#mobius-transformation). After their centres are put at $0,d$ with radii $a,b$, the map $(z-s)/(z-t)$ works when $st=a^2$ and $s+t=(d^2+a^2-b^2)/d$. Disjointness makes the quadratic have distinct real roots. Already concentric [circles](topology.md#circle) require no transformation.

#### Cross-ratio

↑ **Parent:** [Möbius transformation](#mobius-transformation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cross-ratio)

For four distinct points of the [Riemann sphere](complex-analysis.md#riemann-sphere), their cross-ratio is

$$
[z_1,z_2,z_3,z_4]
=\frac{(z_4-z_2)(z_1-z_3)}
{(z_4-z_3)(z_1-z_2)},
$$

with the evident limiting conventions at infinity. Every Möbius transformation preserves it.

##### Cross-ratio construction of generalized-circle reflection

↑ **Parent:** [Cross-ratio](#cross-ratio)

Normalize three distinct points on a [generalized circle](#generalized-circle-under-a-mobius-transformation) by a [Möbius transformation](#mobius-transformation) $f$ taking them to $1,0,\infty$. The inverse image of the extended real line is their generalized circle, and $J=f^{-1}\circ c\circ f$, with $c(z)=\overline z$, fixes that circle pointwise and squares to the identity. Changing the three normalizing points replaces $f$ by $M\circ f$ with a real-coefficient Möbius map $M$. Since $M$ commutes with conjugation, $J$ is unchanged. Thus this construction depends only on the circle. It is [inversion in a circle](#inversion-in-a-circle) for an ordinary circle and [Euclidean reflection](linear-algebra.md#reflection-mathematics) for a straight line, each extended to the [Riemann sphere](complex-analysis.md#riemann-sphere).

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

Normalize three distinct points of the [Riemann sphere](complex-analysis.md#riemann-sphere) by a [Möbius transformation](#mobius-transformation) $f$ sending them to $\infty,0,1$. A fourth point lies on their [generalized circle](#generalized-circle-under-a-mobius-transformation) exactly when $f$ takes a real value there: the image of that [generalized circle](#generalized-circle-under-a-mobius-transformation) is the extended real line. Other standard [cross-ratio](#cross-ratio) ordering conventions differ by real fractional-linear transformations and preserve this reality criterion.

<h4 id="generalized-circle-under-a-mobius-transformation">Generalized circle under a Möbius transformation</h4>

↑ **Parent:** [Möbius transformation](#mobius-transformation)

A generalized circle is either a Euclidean circle or a straight line together with the point at infinity. Every Möbius transformation maps generalized circles to generalized circles. A Euclidean circle becomes a line exactly when it contains the pole, the preimage of infinity.

##### Inversion in a circle

↑ **Parent:** [Generalized circle under a Möbius transformation](#generalized-circle-under-a-mobius-transformation)

[Inversion in a circle](#inversion-in-a-circle) of centre $a$ and radius $R$ is an orientation-reversing involution of the [Riemann sphere](complex-analysis.md#riemann-sphere) fixing that circle pointwise and exchanging its interior and exterior. It is an anti-[Möbius transformation](#mobius-transformation). Reflection in a line is the corresponding inversion for a [generalized circle](#generalized-circle-under-a-mobius-transformation) through infinity. A composition of two such inversions is a [Möbius transformation](#mobius-transformation).

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

For $f(z)=(az+b)/(cz+d)$ with distinct finite [fixed points of a Möbius transformation](#fixed-point-of-a-mobius-transformation) $\alpha,\beta$, the fixed-point equation gives $f(z)-\alpha=(a-c\alpha)(z-\alpha)/(cz+d)$. Dividing the two identities gives $k=(a-c\alpha)/(a-c\beta)$, which is nonzero because $(a-c\alpha)(a-c\beta)=ad-bc\ne0$. The identities extend over the [Riemann sphere](complex-analysis.md#riemann-sphere). This conjugates the transformation to a dilation.

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

A nonidentity [involution](#involution) in the [affine group over a finite field](#affine-group-over-a-finite-field) $\mathbb F_\ell$, for odd prime $\ell$, has linear coefficient $-1$: a translation has order $\ell$, while $u^2=1$ forces $u=\pm1$. Its unique fixed point is $b/2$, and its remaining orbits have size two. This orbit count computes [primes in an intermediate field as double cosets](arithmetic.md#primes-in-an-intermediate-field-as-double-cosets) for an order-two [decomposition group](arithmetic.md#decomposition-group) acting on the radical roots.

// Target: number-theory.bigb

#### Affine Galois group of a prime-radical splitting field

↑ **Parent:** [Affine group over a finite field](#affine-group-over-a-finite-field)

For distinct or equal [prime numbers](number-theory.md#prime-number) $\ell,\lambda$, the polynomial $X^\ell-\lambda$ is [Eisenstein](commutative-algebra.md#eisenstein-criterion) at $\lambda$. Its [splitting field](galois-theory.md#splitting-field) over $\mathbb Q(\zeta_\ell)$ has [Galois group](galois-theory.md#galois-group) a subgroup of $C_\ell$, which is nontrivial because a degree-$\ell$ radical cannot belong to a degree-$(\ell-1)$ [cyclotomic field](galois-theory.md#cyclotomic-field). Thus the full [Galois group](galois-theory.md#galois-group) has order $\ell(\ell-1)$. On roots indexed by $j\in\mathbb F_\ell$, all automorphisms act as $j\mapsto uj+b$. Equality of orders identifies the group with the full [affine group over a finite field](#affine-group-over-a-finite-field).

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

A [group](group.md) is virtually solvable, or virtually soluble, when it contains a [solvable group](#solvable-group) as a [finite-index subgroup](group.md#finite-index-subgroup). This is preserved under [subgroups](group.md#subgroup), quotients and [group extensions](#group-extension). The extension proof can use a [finite-index characteristic soluble subgroup](#finite-index-characteristic-soluble-subgroup) of the kernel, followed by centralizing the resulting finite normal kernel. Finite generation is not required for these closure properties.

#### Finite-index characteristic soluble subgroup

↑ **Parent:** [Virtually solvable group](#virtually-solvable-group)

Every [virtually soluble group](#virtually-solvable-group) $K$ has a soluble [characteristic subgroup](algebra.md#characteristic-subgroup) of finite index. First take a soluble [normal subgroup](#normal-subgroup) $K_0$ of finite index by the [subgroup core](#core-group-theory) construction. Choose a soluble normal subgroup $R\supseteq K_0$ maximizing its image size in the finite quotient $K/K_0$. For every soluble normal subgroup $S$, the product $RS$ is soluble, because its quotient by $R$ is a quotient of $S$. Maximality forces $S\leq R$. Hence $R$ is the unique largest soluble normal subgroup and is invariant under all [automorphisms](algebra.md#automorphism). This avoids incorrectly intersecting infinitely many conjugates when proving closure under [group extensions](#group-extension).

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

Every [polycyclic group](#polycyclic-group) has a finite-index subgroup with a series whose nontrivial factors are infinite cyclic. This is the polycyclic finite-index lemma; it also supplies torsion-free finite-index subgroups. Such a subgroup is a [poly-infinite cyclic group](#poly-infinite-cyclic-group). Combining its series with the extension rule for [Poincare duality groups](#poincare-duality-group) makes it a duality group of dimension its [Hirsch length](#hirsch-length).

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

Every finitely generated [torsion-free group](group.md#torsion-free-group) which is a [nilpotent group](#nilpotent-group) embeds as a discrete cocompact subgroup of a unique simply connected nilpotent real [Lie group](lie-theory.md#lie-group). Its dimension equals the group's [integral cohomological dimension of a group](#integral-cohomological-dimension-of-a-group). In dimension three the Lie algebra is either abelian or has a basis with a single nonzero bracket $[Y,T]=X$, giving the [real Heisenberg group](lie-algebra.md#heisenberg-group).

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

## ← Incoming links (1)

- [Order (group theory)](#order-group-theory)
