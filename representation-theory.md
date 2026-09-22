# Representation theory

↑ **Parent:** [Algebra](algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Representation_theory)

Representation theory describes abstract symmetries by [linear maps](vector-space.md#linear-map) on [vector spaces](vector-space.md). A [group representation](#group-representation) assigns an invertible [linear map](vector-space.md#linear-map) to each [group](group.md) element, respecting multiplication. The payoff is that a symmetry problem becomes a problem about [matrices](vector-space.md#matrix), [invariant subspaces](#invariant-subspace), and [eigenvalues](linear-operator-theory.md#eigenvalue). Decomposing the action can reveal combinations of variables that a symmetric system cannot mix.

Take the [cyclic group](group.md#cyclic-group) $C_3=\{e,g,g^2\}$, with $g^3=e$. On three real coordinates, let $g$ send $(a,b,c)$ to $(c,a,b)$:

$$
\rho(g)=P=\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix},\qquad P^3=I.
$$

This [permutation representation](#permutation-representation) does more than relabel a list: it acts linearly on every possible assignment of values to the three positions. The [vector](vector-space.md#vector) $(1,1,1)$ stays fixed. The [vector subspace](vector-space.md#vector-subspace) $W=\{(a,b,c):a+b+c=0\}$ is also preserved, since a permutation does not change the sum.

Every [vector](vector-space.md#vector) separates uniquely into these two types:

$$
(a,b,c)=\bar a(1,1,1)+(a-\bar a,b-\bar a,c-\bar a),\qquad
\bar a=\frac{a+b+c}{3}.
$$

For example, $(4,1,1)=2(1,1,1)+(2,-1,-1)$. The first term belongs to a [trivial representation](#trivial-representation); the second is a contrast with zero coordinate sum. This is a [direct sum](vector-space.md#direct-sum) decomposition $\mathbb R^3=\mathbb R(1,1,1)\oplus W$. The symmetry preserves the mean and rotates the contrasts.

<a id="image-three-coordinate-cyclic-symmetry-preserves-the-mean-and-rotates-the-zero-sum-contrasts-by-120-degrees"></a>
![](cyclic-representation-decomposition.png)

**[Figure 1](#image-three-coordinate-cyclic-symmetry-preserves-the-mean-and-rotates-the-zero-sum-contrasts-by-120-degrees). Three-coordinate cyclic symmetry preserves the mean and rotates the zero-sum contrasts by 120 degrees**.

The rotation is literal after choosing the [orthonormal basis](inner-product.md#orthonormal-basis) $u=(2,-1,-1)/\sqrt6$, $v=(0,1,-1)/\sqrt2$ of $W$. In this basis,

$$
P|_W=\begin{pmatrix}-1/2&-\sqrt3/2\\\sqrt3/2&-1/2\end{pmatrix}.
$$

It is a rotation through $120$ degrees, and three applications return to the starting point. There is no nonzero invariant real line, because this rotation has no real [eigenvector](linear-operator-theory.md#eigenvector). Thus the two-dimensional action is an [irreducible representation](#irreducible-representation) over the [real numbers](arithmetic.md#real-number). Over the [complex numbers](complex-analysis.md#complex-number) it instead splits into two [eigenlines](linear-operator-theory.md#eigenline) with [eigenvalues](linear-operator-theory.md#eigenvalue) $e^{2\pi i/3}$ and $e^{-2\pi i/3}$. The coefficient [field](algebra.md#field) is part of an irreducibility claim.

Why would this decomposition matter for a physical calculation? Consider three equal masses with scalar displacements $x_i$ and the symmetric quadratic coupling energy

$$
V(x)=\frac{k}{2}\left[(x_1-x_2)^2+(x_2-x_3)^2+(x_3-x_1)^2\right],\qquad k>0.
$$

The [equations of motion](classical-mechanics.md#equation-of-motion) are $m\ddot x=-kLx$, where

$$
L=\begin{pmatrix}2&-1&-1\\-1&2&-1\\-1&-1&2\end{pmatrix}=3I-J
$$

is a [graph Laplacian](graph-theory.md#laplacian-matrix) and $J$ is the all-ones [matrix](vector-space.md#matrix). The constant [vector](vector-space.md#vector) has [eigenvalue](linear-operator-theory.md#eigenvalue) zero: translating all coordinates equally costs no coupling energy. On $W$, $J$ vanishes and $L=3I$, so both independent contrast directions have [angular frequency](lagrangian-mechanics.md#angular-frequency) $\sqrt{3k/m}$. A three-coordinate coupled problem reduces to a free mean and two identical [harmonic oscillators](classical-mechanics.md#simple-harmonic-motion).

<a id="image-equal-pair-couplings-leave-the-mean-fixed-and-make-two-independent-zero-sum-modes-oscillate-at-the-same-frequency"></a>
![](symmetry-separated-oscillations.png)

**[Figure 2](#image-equal-pair-couplings-leave-the-mean-fixed-and-make-two-independent-zero-sum-modes-oscillate-at-the-same-frequency). Equal pair couplings leave the mean fixed and make two independent zero-sum modes oscillate at the same frequency**.

For initial displacement $x(0)=(4,1,1)$ and initial [velocity](classical-mechanics.md#velocity) zero, the exact solution is $x(t)=2(1,1,1)+\cos(\sqrt{3k/m}\,t)(2,-1,-1)$. The fixed mean and oscillating contrast can be read directly from the decomposition. More generally, a [linear operator](vector-space.md#linear-operator) commuting with the group action carries its fixed-vector subspace into itself; with an invariant [inner product](inner-product.md), it preserves the corresponding orthogonal complement too.

For a [finite group](group.md#finite-group), averaging over the action constructs an invariant [inner product](inner-product.md) over the [real numbers](arithmetic.md#real-number) or [complex numbers](complex-analysis.md#complex-number). The resulting invariant complements explain [Maschke's theorem](#maschke-s-theorem): a finite-dimensional [group representation](#group-representation) decomposes into [irreducible representations](#irreducible-representation). [Characters](#character-of-a-representation) compress the action into traces and help identify those pieces. The assumptions matter; in [modular representation theory](modular-representation-theory.md) the coefficient [field](algebra.md#field) can have [characteristic](algebra.md#characteristic-of-a-field) dividing the group order, and such decompositions can fail. Chapter 4 of Pavel Etingof and coauthors' notes develops these mechanisms. [Etingof and coauthors: Introduction to representation theory](https://math.mit.edu/~etingof/reprbook.pdf).

**Table of contents**

- [Representation ring of a compact group](#representation-ring-of-a-compact-group)
  - [Representation ring of an odd-dimensional special orthogonal group](#representation-ring-of-an-odd-dimensional-special-orthogonal-group)
- [Subrepresentation](#subrepresentation)
  - [Quotient representation](#quotient-representation)
- [Group representation](#group-representation)
  - [Character projection operator](#character-projection-operator)
  - [Quarter-turn action on diagonal quadratic forms](#quarter-turn-action-on-diagonal-quadratic-forms)
  - [Equivalence of group representations](#equivalence-of-group-representations)
  - [Inverse-adjoint representation](#inverse-adjoint-representation)
  - [One-dimensional representation](#one-dimensional-representation)
  - [Projective representation](#projective-representation)
  - [Orthogonal representation](#orthogonal-representation)
  - [Representation over the rational numbers](#representation-over-the-rational-numbers)
  - [Scalar endomorphisms obstruct a split extension](#scalar-endomorphisms-obstruct-a-split-extension)
  - [Distinct-character extensions of an abelian group split](#distinct-character-extensions-of-an-abelian-group-split)
  - [Smooth representation of a locally profinite group](#smooth-representation-of-a-locally-profinite-group)
    - [Smooth vector](#smooth-vector)
    - [Smooth character](#smooth-character)
    - [Jacquet module](#jacquet-module)
    - [Smooth right regular representation](#smooth-right-regular-representation)
    - [Admissible representation of a locally profinite group](#admissible-representation-of-a-locally-profinite-group)
      - [Contraction and admissible fixed spaces](#contraction-and-admissible-fixed-spaces)
    - [Fixed-vector space](#fixed-vector-space)
  - [Galois representation](#galois-representation)
    - [Tate module](#tate-module)
      - [CM Tate module stabilizer](#cm-tate-module-stabilizer)
      - [Rational Tate module](#rational-tate-module)
    - [Galois character](#galois-character)
    - [Cyclotomic character](#cyclotomic-character)
      - [Tate twist](#tate-twist)
  - [Invariant theory](#invariant-theory)
    - [Geometric invariant theory](#geometric-invariant-theory)
      - [Hilbert-Mumford criterion for projective stability](#hilbert-mumford-criterion-for-projective-stability)
        - [Root-multiplicity criterion for stable binary forms](#root-multiplicity-criterion-for-stable-binary-forms)
      - [Stable projective point in geometric invariant theory](#stable-projective-point-in-geometric-invariant-theory)
      - [Affine null cone](#affine-null-cone)
        - [Nilpotent cone for conjugation of matrices](#nilpotent-cone-for-conjugation-of-matrices)
      - [Semistable projective point in geometric invariant theory](#semistable-projective-point-in-geometric-invariant-theory)
      - [Linearization of a line bundle](#linearization-of-a-line-bundle)
    - [Symbolic method for binary-form invariants](#symbolic-method-for-binary-form-invariants)
      - [Transvectant of binary forms](#transvectant-of-binary-forms)
    - [Polynomial invariant ring](#polynomial-invariant-ring)
      - [Determinant-one cyclic quotient of the affine plane](#determinant-one-cyclic-quotient-of-the-affine-plane)
      - [Hilbert finite generation for reductive invariants](#hilbert-finite-generation-for-reductive-invariants)
      - [Reynolds operator on a polynomial invariant ring](#reynolds-operator-on-a-polynomial-invariant-ring)
      - [Binary dihedral invariant hypersurface](#binary-dihedral-invariant-hypersurface)
      - [Quadratic cone invariant ring](#quadratic-cone-invariant-ring)
      - [Factorial invariant ring with no linear characters](#factorial-invariant-ring-with-no-linear-characters)
      - [Orbit product of polynomial factors](#orbit-product-of-polynomial-factors)
      - [Alternating-group polynomial invariants](#alternating-group-polynomial-invariants)
  - [Restriction of a representation](#restriction-of-a-representation)
    - [Restriction multiplicity bound](#restriction-multiplicity-bound)
  - [Sum of squares of irreducible representation dimensions](#sum-of-squares-of-irreducible-representation-dimensions)
  - [Intertwiner](#intertwiner)
  - [Matrix coefficient](#matrix-coefficient)
    - [Schur orthogonality relations](#schur-orthogonality-relations)
      - [Character orthogonality for compact groups](#character-orthogonality-for-compact-groups)
      - [Schur averaging of rectangular matrices](#schur-averaging-of-rectangular-matrices)
  - [Cyclic vector for a group representation](#cyclic-vector-for-a-group-representation)
    - [Cyclic eigenvector obstruction to invariant vectors](#cyclic-eigenvector-obstruction-to-invariant-vectors)
  - [Multiplicity-free restriction](#multiplicity-free-restriction)
  - [Pseudoreal representation](#pseudoreal-representation)
  - [Splitting field for finite group representations](#splitting-field-for-finite-group-representations)
  - [Tensor product of group representations](#tensor-product-of-group-representations)
    - [Symmetric square of a group representation](#symmetric-square-of-a-group-representation)
    - [Trivial representation in a tensor square](#trivial-representation-in-a-tensor-square)
    - [External tensor product of group representations](#external-tensor-product-of-group-representations)
    - [Fundamental-antifundamental decomposition for SU(N)](#fundamental-antifundamental-decomposition-for-su-n)
    - [SU(n) tensor transformation](#su-n-tensor-transformation)
    - [Invariant tensor](#invariant-tensor)
    - [Octet and singlet in a fundamental SU3 tensor product](#octet-and-singlet-in-a-fundamental-su3-tensor-product)
  - [Conjugation representation](#conjugation-representation)
  - [Trivial representation](#trivial-representation)
    - [Fully symmetric representation](#fully-symmetric-representation)
    - [Gauge singlet](#gauge-singlet)
    - [Scalar representation](#scalar-representation)
  - [Vector representation](#vector-representation)
  - [Matrix representation](#matrix-representation)
  - [Invariant subspace](#invariant-subspace)
    - [Fixed-point subspace of a group action](#fixed-point-subspace-of-a-group-action)
    - [Reducible representation](#reducible-representation)
  - [Semisimple representation](#semisimple-representation)
- [Maschke's theorem](#maschke-s-theorem)
- [Modular representation theory](modular-representation-theory.md)
  - [p-local module](modular-representation-theory.md#p-local-module)
  - [Splitting p-modular system](modular-representation-theory.md#splitting-p-modular-system)
  - [Indecomposable modules for a cyclic p-group](modular-representation-theory.md#indecomposable-modules-for-a-cyclic-p-group)
  - [Modular representation ring](modular-representation-theory.md#modular-representation-ring)
  - [Indecomposable modules of a cyclic p-group in characteristic p](modular-representation-theory.md#indecomposable-modules-of-a-cyclic-p-group-in-characteristic-p)
  - [Group algebra of a p-group in characteristic p is local](modular-representation-theory.md#group-algebra-of-a-p-group-in-characteristic-p-is-local)
  - [p-modular system](modular-representation-theory.md#p-modular-system)
    - [Integral form of a group representation](modular-representation-theory.md#integral-form-of-a-group-representation)
      - [Reduction of Hom from a projective group-algebra lattice](modular-representation-theory.md#reduction-of-hom-from-a-projective-group-algebra-lattice)
  - [p-regular element](modular-representation-theory.md#p-regular-element)
  - [Brauer character](modular-representation-theory.md#brauer-character)
    - [Brauer–Nesbitt theorem](modular-representation-theory.md#brauer-nesbitt-theorem)
      - [Brauer character basis theorem](modular-representation-theory.md#brauer-character-basis-theorem)
    - [Projective character](modular-representation-theory.md#projective-character)
    - [Brauer character inner product](modular-representation-theory.md#brauer-character-inner-product)
      - [Duality of simple and projective Brauer characters](modular-representation-theory.md#duality-of-simple-and-projective-brauer-characters)
        - [Column orthogonality for Brauer characters](modular-representation-theory.md#column-orthogonality-for-brauer-characters)
  - [Symmetric algebra (Frobenius algebra)](modular-representation-theory.md#symmetric-algebra-frobenius-algebra)
    - [Head-socle identity for a symmetric algebra](modular-representation-theory.md#head-socle-identity-for-a-symmetric-algebra)
    - [Group algebra is a symmetric algebra](modular-representation-theory.md#group-algebra-is-a-symmetric-algebra)
      - [Projective modules over a finite group algebra are injective](modular-representation-theory.md#projective-modules-over-a-finite-group-algebra-are-injective)
        - [Head and socle of an indecomposable projective group-algebra module](modular-representation-theory.md#head-and-socle-of-an-indecomposable-projective-group-algebra-module)
          - [Dual of a projective cover over a group algebra](modular-representation-theory.md#dual-of-a-projective-cover-over-a-group-algebra)
        - [Group norm element detects the trivial projective cover](modular-representation-theory.md#group-norm-element-detects-the-trivial-projective-cover)
  - [Relative projective module](modular-representation-theory.md#relative-projective-module)
    - [Relative trace](modular-representation-theory.md#relative-trace)
      - [Transfer ideal of conjugation-fixed elements](modular-representation-theory.md#transfer-ideal-of-conjugation-fixed-elements)
      - [D. Higman criterion](modular-representation-theory.md#d-higman-criterion)
        - [Projectivity detected on a subgroup of invertible index](modular-representation-theory.md#projectivity-detected-on-a-subgroup-of-invertible-index)
    - [Vertex of an indecomposable module](modular-representation-theory.md#vertex-of-an-indecomposable-module)
      - [Full-vertex modules for a noncyclic p-group](modular-representation-theory.md#full-vertex-modules-for-a-noncyclic-p-group)
      - [Green correspondence](modular-representation-theory.md#green-correspondence)
        - [Green correspondence from Mackey multiplicity](modular-representation-theory.md#green-correspondence-from-mackey-multiplicity)
        - [Green correspondent of a module](modular-representation-theory.md#green-correspondent-of-a-module)
        - [Green correspondence for blocks](modular-representation-theory.md#green-correspondence-for-blocks)
      - [Source of an indecomposable module](modular-representation-theory.md#source-of-an-indecomposable-module)
        - [Trivial source module](modular-representation-theory.md#trivial-source-module)
          - [Inflated quotient projectives have trivial source](modular-representation-theory.md#inflated-quotient-projectives-have-trivial-source)
          - [Permutation homomorphisms lift through modular reduction](modular-representation-theory.md#permutation-homomorphisms-lift-through-modular-reduction)
  - [Finite representation type of a group algebra](modular-representation-theory.md#finite-representation-type-of-a-group-algebra)
    - [Parameter family for an elementary abelian p-group](modular-representation-theory.md#parameter-family-for-an-elementary-abelian-p-group)
    - [Higman criterion for finite representation type of a group algebra](modular-representation-theory.md#higman-criterion-for-finite-representation-type-of-a-group-algebra)
  - [Defect-zero representation](modular-representation-theory.md#defect-zero-representation)
  - [Block of a group algebra](modular-representation-theory.md#block-of-a-group-algebra)
    - [Residue-content criterion for symmetric-group blocks](modular-representation-theory.md#residue-content-criterion-for-symmetric-group-blocks)
      - [Nakayama block theorem](modular-representation-theory.md#nakayama-block-theorem)
    - [Central character of a block](modular-representation-theory.md#central-character-of-a-block)
    - [Fong–Reynolds matrix decomposition](modular-representation-theory.md#fong-reynolds-matrix-decomposition)
    - [Principal block](modular-representation-theory.md#principal-block)
    - [Modular reduction of block idempotents](modular-representation-theory.md#modular-reduction-of-block-idempotents)
    - [Blocks and Cartan matrices under central p-quotients](modular-representation-theory.md#blocks-and-cartan-matrices-under-central-p-quotients)
    - [Block of S3 in characteristic three](modular-representation-theory.md#block-of-s3-in-characteristic-three)
      - [Indecomposable projectives of S3 in characteristic three](modular-representation-theory.md#indecomposable-projectives-of-s3-in-characteristic-three)
    - [2-modular blocks of S3](modular-representation-theory.md#2-modular-blocks-of-s3)
    - [Defect group of a block](modular-representation-theory.md#defect-group-of-a-block)
      - [Regular defect-group bimodule inside a block](modular-representation-theory.md#regular-defect-group-bimodule-inside-a-block)
      - [Defect groups are centralizer-conjugate Sylow intersections](modular-representation-theory.md#defect-groups-are-centralizer-conjugate-sylow-intersections)
      - [Modules in a block are projective relative to its defect group](modular-representation-theory.md#modules-in-a-block-are-projective-relative-to-its-defect-group)
      - [Central defect blocks are matrix algebras](modular-representation-theory.md#central-defect-blocks-are-matrix-algebras)
      - [Inertial quotient of a block](modular-representation-theory.md#inertial-quotient-of-a-block)
        - [Inertial index of a block](modular-representation-theory.md#inertial-index-of-a-block)
      - [Defect of a block](modular-representation-theory.md#defect-of-a-block)
      - [Brauer pair](modular-representation-theory.md#brauer-pair)
      - [Block with cyclic defect group](modular-representation-theory.md#block-with-cyclic-defect-group)
        - [Brauer tree algebra](modular-representation-theory.md#brauer-tree-algebra)
          - [Uniserial branch of a Brauer tree algebra](modular-representation-theory.md#uniserial-branch-of-a-brauer-tree-algebra)
          - [Brauer tree path presentation](modular-representation-theory.md#brauer-tree-path-presentation)
          - [Indecomposable count for a cyclic defect block](modular-representation-theory.md#indecomposable-count-for-a-cyclic-defect-block)
      - [2-modular defect groups of A5](modular-representation-theory.md#2-modular-defect-groups-of-a5)
      - [Trace criterion for defect groups](modular-representation-theory.md#trace-criterion-for-defect-groups)
      - [Brauer morphism](modular-representation-theory.md#brauer-morphism)
        - [Block idempotents centralize a normal p-subgroup](modular-representation-theory.md#block-idempotents-centralize-a-normal-p-subgroup)
        - [Brauer quotient of a module](modular-representation-theory.md#brauer-quotient-of-a-module)
        - [Brauer morphism on a defect transfer ideal](modular-representation-theory.md#brauer-morphism-on-a-defect-transfer-ideal)
        - [Brauer morphism and relative trace](modular-representation-theory.md#brauer-morphism-and-relative-trace)
      - [Brauer correspondence](modular-representation-theory.md#brauer-correspondence)
        - [Brauer correspondent of a block](modular-representation-theory.md#brauer-correspondent-of-a-block)
        - [Brauer third main theorem](modular-representation-theory.md#brauer-third-main-theorem)
        - [Block induction](modular-representation-theory.md#block-induction)
          - [Block induction requires the block's defect centralizer](modular-representation-theory.md#block-induction-requires-the-block-s-defect-centralizer)
        - [Nagao module theorem](modular-representation-theory.md#nagao-module-theorem)
          - [Juhász induction refinement](modular-representation-theory.md#juhasz-induction-refinement)
        - [Brauer first main theorem](modular-representation-theory.md#brauer-first-main-theorem)
          - [Brauer extended first main theorem](modular-representation-theory.md#brauer-extended-first-main-theorem)
        - [5-modular blocks of A5](modular-representation-theory.md#5-modular-blocks-of-a5)
    - [Decomposition matrix (modular representation theory)](modular-representation-theory.md#decomposition-matrix-modular-representation-theory)
      - [Dominance triangularity of modular symmetric-group decomposition](modular-representation-theory.md#dominance-triangularity-of-modular-symmetric-group-decomposition)
      - [Cartan matrix of a group algebra](modular-representation-theory.md#cartan-matrix-of-a-group-algebra)
  - [2-modular representation theory of GL3 of F2](modular-representation-theory.md#2-modular-representation-theory-of-gl3-of-f2)
- [Complex representation](#complex-representation)
  - [Continuous representation of a topological group](#continuous-representation-of-a-topological-group)
  - [Degree of a representation](#degree-of-a-representation)
  - [Isomorphic representations](#isomorphic-representations)
  - [Nonsemisimple translation representation of the infinite cyclic group](#nonsemisimple-translation-representation-of-the-infinite-cyclic-group)
  - [Faithful representation](#faithful-representation)
    - [Regular representation](#regular-representation)
      - [Four-point regular representation of the Klein four-group](#four-point-regular-representation-of-the-klein-four-group)
      - [Sum of squares of irreducible degrees](#sum-of-squares-of-irreducible-degrees)
      - [Faithful irreducible representation of a finite simple group](#faithful-irreducible-representation-of-a-finite-simple-group)
    - [Spectrum orbit bound for a faithful symmetric-group representation](#spectrum-orbit-bound-for-a-faithful-symmetric-group-representation)
    - [Finite-dimensional representation obstruction from elementary abelian subgroups](#finite-dimensional-representation-obstruction-from-elementary-abelian-subgroups)
    - [Real Heisenberg quotient has no faithful finite-dimensional representation](#real-heisenberg-quotient-has-no-faithful-finite-dimensional-representation)
  - [One-dimensional representation kills the commutator subgroup](#one-dimensional-representation-kills-the-commutator-subgroup)
  - [Inflation of a group representation](#inflation-of-a-group-representation)
  - [Irreducible representation of a finite abelian group](#irreducible-representation-of-a-finite-abelian-group)
    - [Complex irreducible representations of a finite cyclic group](#complex-irreducible-representations-of-a-finite-cyclic-group)
- [Real representation](#real-representation)
  - [Realification of a complex representation](#realification-of-a-complex-representation)
  - [Irreducible real representations of a finite cyclic group](#irreducible-real-representations-of-a-finite-cyclic-group)
  - [Real regular representation of a finite cyclic group](#real-regular-representation-of-a-finite-cyclic-group)
- [Representation theory of SU(2)](#representation-theory-of-su-2)
  - [Conjugate fundamental spinor of SU(2)](#conjugate-fundamental-spinor-of-su-2)
  - [Homogeneous polynomial representation of SU2](#homogeneous-polynomial-representation-of-su2)
    - [Character of the homogeneous polynomial representation of SU2](#character-of-the-homogeneous-polynomial-representation-of-su2)
  - [Classification of finite-dimensional representations of SU2](#classification-of-finite-dimensional-representations-of-su2)
  - [Self-duality of finite-dimensional SU2 representations](#self-duality-of-finite-dimensional-su2-representations)
  - [Central parity on SU2 tensor products](#central-parity-on-su2-tensor-products)
  - [Clebsch-Gordan coefficients](#clebsch-gordan-coefficients)
    - [Ladder recurrence for Clebsch-Gordan coefficients](#ladder-recurrence-for-clebsch-gordan-coefficients)
    - [3-j symbol](#3-j-symbol)
    - [Clebsch-Gordan decomposition for SU2](#clebsch-gordan-decomposition-for-su2)
      - [Tensor contractions in the SU2 Clebsch-Gordan decomposition](#tensor-contractions-in-the-su2-clebsch-gordan-decomposition)
        - [Decomposition of three SU(2) spinors](#decomposition-of-three-su-2-spinors)
      - [Flip parity in the SU2 tensor square](#flip-parity-in-the-su2-tensor-square)
        - [Exterior square of an SU2 irreducible representation](#exterior-square-of-an-su2-irreducible-representation)
          - [Second and third exterior powers of V4 of SU2](#second-and-third-exterior-powers-of-v4-of-su2)
- [Character of an exterior square](#character-of-an-exterior-square)
- [Character of an exterior cube](#character-of-an-exterior-cube)
- [Averaging over a finite group](#averaging-over-a-finite-group)
- [Unitary representation](#unitary-representation)
  - [Triviality of finite-dimensional unitary representations of SL2R](#triviality-of-finite-dimensional-unitary-representations-of-sl2r)
  - [Integrated unitary representation](#integrated-unitary-representation)
  - [Positive energy unitary representation of the circle](#positive-energy-unitary-representation-of-the-circle)
  - [Stone theorem for the circle group](#stone-theorem-for-the-circle-group)
  - [Peter-Weyl theorem](#peter-weyl-theorem)
    - [Finite faithful representation from point-separating representations](#finite-faithful-representation-from-point-separating-representations)
    - [Convolution proof of uniform Peter-Weyl approximation](#convolution-proof-of-uniform-peter-weyl-approximation)
    - [Frobenius reciprocity for compact groups](#frobenius-reciprocity-for-compact-groups)
  - [Unitary irreducible representation](#unitary-irreducible-representation)
  - [Unitarization of a finite-group representation](#unitarization-of-a-finite-group-representation)
  - [Unitarization of a compact-group representation](#unitarization-of-a-compact-group-representation)
    - [Complete reducibility of compact-group representations](#complete-reducibility-of-compact-group-representations)
    - [Orthogonalization of a compact-group representation](#orthogonalization-of-a-compact-group-representation)
  - [Representation of the circle group](#representation-of-the-circle-group)
    - [Central circle weight-space decomposition](#central-circle-weight-space-decomposition)
- [Class function](#class-function)
  - [Conjugation averaging on a compact group](#conjugation-averaging-on-a-compact-group)
- [Character orthogonality](#character-orthogonality)
  - [Irreducible characters separate conjugacy classes](#irreducible-characters-separate-conjugacy-classes)
  - [Character expansion of the identity delta](#character-expansion-of-the-identity-delta)
  - [Row orthogonality relations for a character table](#row-orthogonality-relations-for-a-character-table)
  - [Central character value of a conjugacy-class sum](#central-character-value-of-a-conjugacy-class-sum)
    - [Irreducible character degree divides the group order](#irreducible-character-degree-divides-the-group-order)
      - [No finite simple group has an irreducible character of degree two](#no-finite-simple-group-has-an-irreducible-character-of-degree-two)
      - [Irreducible character degrees of a group of order two p](#irreducible-character-degrees-of-a-group-of-order-two-p)
      - [Irreducible characters of a nonabelian group of order p q](#irreducible-characters-of-a-nonabelian-group-of-order-p-q)
  - [Character inner product](#character-inner-product)
- [Character table](#character-table)
  - [Integral character reconstruction from column orthogonality](#integral-character-reconstruction-from-column-orthogonality)
  - [Irreducible representations of G6n](#irreducible-representations-of-g6n)
    - [Character table of G6n](#character-table-of-g6n)
  - [Irreducible character degree](#irreducible-character-degree)
    - [Irreducible characters of degree coprime to p](#irreducible-characters-of-degree-coprime-to-p)
    - [Linear character](#linear-character)
      - [Trivial character](#trivial-character)
    - [Nonlinear irreducible character](#nonlinear-irreducible-character)
- [Character theory](#character-theory)
  - [Brauer's permutation lemma](#brauer-s-permutation-lemma)
  - [Artin induction](#artin-induction)
  - [Brauer induction](#brauer-induction)
  - [Character of a representation](#character-of-a-representation)
    - [Character of a localized orbital basis](#character-of-a-localized-orbital-basis)
    - [Ordinary character](#ordinary-character)
    - [Determinant character](#determinant-character)
      - [Central commutator has no torsion from an abelian Sylow subgroup](#central-commutator-has-no-torsion-from-an-abelian-sylow-subgroup)
    - [Kernel of a character](#kernel-of-a-character)
    - [Characters distinguish finite-dimensional complex semisimple representations](#characters-distinguish-finite-dimensional-complex-semisimple-representations)
    - [Character value of a representation](#character-value-of-a-representation)
    - [Irreducible character](#irreducible-character)
      - [Frobenius-Schur indicator](#frobenius-schur-indicator)
        - [Central average of representation matrices at squares](#central-average-of-representation-matrices-at-squares)
        - [Odd-order group conjugacy-class congruence](#odd-order-group-conjugacy-class-congruence)
      - [Odd-order groups have no nontrivial real irreducible characters](#odd-order-groups-have-no-nontrivial-real-irreducible-characters)
    - [Character constituent](#character-constituent)
    - [Restriction of a character](#restriction-of-a-character)
      - [Character extension](#character-extension)
        - [Thompson's coprime character extension theorem](#thompson-s-coprime-character-extension-theorem)
        - [Gluing determinant-normalized character extensions](#gluing-determinant-normalized-character-extensions)
        - [Coprime-degree determinant extension theorem](#coprime-degree-determinant-extension-theorem)
      - [Inertia group of a character](#inertia-group-of-a-character)
        - [Clifford correspondence](#clifford-correspondence)
      - [Character restriction norm bound](#character-restriction-norm-bound)
        - [Index-two character restriction dichotomy](#index-two-character-restriction-dichotomy)
    - [Virtual character](#virtual-character)
      - [Brauer's characterization of characters](#brauer-s-characterization-of-characters)
        - [Generalized character separating complementary prime elements](#generalized-character-separating-complementary-prime-elements)
      - [Positive-degree norm-one virtual characters are irreducible](#positive-degree-norm-one-virtual-characters-are-irreducible)
- [Burnside's lemma](#burnside-s-lemma)
  - [Cycle index](#cycle-index)
    - [Pattern inventory](#pattern-inventory)
  - [Weighted Burnside lemma](#weighted-burnside-lemma)
  - [Permutation representation of a two-transitive action](#permutation-representation-of-a-two-transitive-action)
    - [Steinberg representation of GL2 over a finite field](#steinberg-representation-of-gl2-over-a-finite-field)
- [Permutation representation](#permutation-representation)
  - [Rank of a permutation action](#rank-of-a-permutation-action)
  - [Permutation module](#permutation-module)
  - [Deleted permutation module in characteristic two](#deleted-permutation-module-in-characteristic-two)
  - [Permutation character](#permutation-character)
  - [Gassmann equivalence](#gassmann-equivalence)
    - [Point and hyperplane stabilizers are almost conjugate](#point-and-hyperplane-stabilizers-are-almost-conjugate)
    - [Order-sixteen Gassmann pair](#order-sixteen-gassmann-pair)
    - [Nonisomorphic Gassmann equivalent regular subgroups](#nonisomorphic-gassmann-equivalent-regular-subgroups)
  - [Permutation character of a coset action](#permutation-character-of-a-coset-action)
  - [Augmentation subrepresentation of a permutation representation](#augmentation-subrepresentation-of-a-permutation-representation)
    - [Irreducible augmentation criterion for a transitive group action](#irreducible-augmentation-criterion-for-a-transitive-group-action)
  - [Character norm of a permutation representation](#character-norm-of-a-permutation-representation)
  - [Symmetric-group subset permutation representation](#symmetric-group-subset-permutation-representation)
    - [Inclusion map between subset permutation modules](#inclusion-map-between-subset-permutation-modules)
  - [Standard representation of the symmetric group](#standard-representation-of-the-symmetric-group)
    - [Gelfand–Tsetlin basis of the standard representation](#gelfand-tsetlin-basis-of-the-standard-representation)
    - [Three-dimensional irreducible representation of the alternating group on four letters](#three-dimensional-irreducible-representation-of-the-alternating-group-on-four-letters)
- [Representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md)
  - [Induction ring of symmetric-group characters](representation-theory-of-the-symmetric-group.md#induction-ring-of-symmetric-group-characters)
  - [Symmetric-group characters are integer-valued](representation-theory-of-the-symmetric-group.md#symmetric-group-characters-are-integer-valued)
  - [Young subgroup](representation-theory-of-the-symmetric-group.md#young-subgroup)
  - [Skew representation of a symmetric group](representation-theory-of-the-symmetric-group.md#skew-representation-of-a-symmetric-group)
  - [Deletion projection for a symmetric group](representation-theory-of-the-symmetric-group.md#deletion-projection-for-a-symmetric-group)
  - [Gelfand–Tsetlin algebra](representation-theory-of-the-symmetric-group.md#gelfand-tsetlin-algebra)
    - [Jucys–Murphy element](representation-theory-of-the-symmetric-group.md#jucys-murphy-element)
      - [Jucys–Murphy description of the center of a symmetric-group algebra](representation-theory-of-the-symmetric-group.md#jucys-murphy-description-of-the-center-of-a-symmetric-group-algebra)
      - [Cycle-sum identity for Young–Jucys–Murphy elements](representation-theory-of-the-symmetric-group.md#cycle-sum-identity-for-young-jucys-murphy-elements)
      - [Local spectral rules for Young–Jucys–Murphy elements](representation-theory-of-the-symmetric-group.md#local-spectral-rules-for-young-jucys-murphy-elements)
      - [Olshanskii centralizer lemma](representation-theory-of-the-symmetric-group.md#olshanskii-centralizer-lemma)
    - [Gelfand–Tsetlin basis](representation-theory-of-the-symmetric-group.md#gelfand-tsetlin-basis)
      - [Young seminormal form](representation-theory-of-the-symmetric-group.md#young-seminormal-form)
        - [Young orthogonal form](representation-theory-of-the-symmetric-group.md#young-orthogonal-form)
  - [Sign representation](representation-theory-of-the-symmetric-group.md#sign-representation)
  - [Tensor identity for an induced character](representation-theory-of-the-symmetric-group.md#tensor-identity-for-an-induced-character)
    - [Prime-degree irreducible Kronecker product criterion for a symmetric group](representation-theory-of-the-symmetric-group.md#prime-degree-irreducible-kronecker-product-criterion-for-a-symmetric-group)
    - [Induced-tensor decomposition for the symmetric group on four points](representation-theory-of-the-symmetric-group.md#induced-tensor-decomposition-for-the-symmetric-group-on-four-points)
  - [Partition of an integer](representation-theory-of-the-symmetric-group.md#partition-of-an-integer)
    - [Reverse lexicographic order on partitions](representation-theory-of-the-symmetric-group.md#reverse-lexicographic-order-on-partitions)
    - [Glaisher partition bijection](representation-theory-of-the-symmetric-group.md#glaisher-partition-bijection)
    - [Dictionary order on integer partitions](representation-theory-of-the-symmetric-group.md#dictionary-order-on-integer-partitions)
    - [Young's lattice](representation-theory-of-the-symmetric-group.md#young-s-lattice)
      - [Young branching graph](representation-theory-of-the-symmetric-group.md#young-branching-graph)
        - [Oscillating path in the Young lattice](representation-theory-of-the-symmetric-group.md#oscillating-path-in-the-young-lattice)
    - [Generating function for partitions with bounded parts](representation-theory-of-the-symmetric-group.md#generating-function-for-partitions-with-bounded-parts)
    - [Self-conjugate partition and distinct odd parts](representation-theory-of-the-symmetric-group.md#self-conjugate-partition-and-distinct-odd-parts)
    - [Young diagram](representation-theory-of-the-symmetric-group.md#young-diagram)
      - [Durfee square](representation-theory-of-the-symmetric-group.md#durfee-square)
      - [Jeu de taquin](representation-theory-of-the-symmetric-group.md#jeu-de-taquin)
      - [Skew Young diagram](representation-theory-of-the-symmetric-group.md#skew-young-diagram)
        - [Standard skew Young tableau](representation-theory-of-the-symmetric-group.md#standard-skew-young-tableau)
          - [Standard skew tableau determinant](representation-theory-of-the-symmetric-group.md#standard-skew-tableau-determinant)
        - [Horizontal strip](representation-theory-of-the-symmetric-group.md#horizontal-strip)
        - [Totally disconnected skew Young diagram](representation-theory-of-the-symmetric-group.md#totally-disconnected-skew-young-diagram)
      - [Hook partition](representation-theory-of-the-symmetric-group.md#hook-partition)
      - [Addable node of a Young diagram](representation-theory-of-the-symmetric-group.md#addable-node-of-a-young-diagram)
      - [Removable node of a Young diagram](representation-theory-of-the-symmetric-group.md#removable-node-of-a-young-diagram)
      - [Conjugate partition](representation-theory-of-the-symmetric-group.md#conjugate-partition)
      - [Hook of a Young diagram](representation-theory-of-the-symmetric-group.md#hook-of-a-young-diagram)
        - [Arm of a Young-diagram cell](representation-theory-of-the-symmetric-group.md#arm-of-a-young-diagram-cell)
        - [Leg of a Young-diagram cell](representation-theory-of-the-symmetric-group.md#leg-of-a-young-diagram-cell)
        - [Hook length](representation-theory-of-the-symmetric-group.md#hook-length)
          - [Hook graph of a partition](representation-theory-of-the-symmetric-group.md#hook-graph-of-a-partition)
            - [Hook product of a partition](representation-theory-of-the-symmetric-group.md#hook-product-of-a-partition)
        - [Hook-interval decomposition at a Young-diagram cell](representation-theory-of-the-symmetric-group.md#hook-interval-decomposition-at-a-young-diagram-cell)
        - [Divisor closure of hook lengths](representation-theory-of-the-symmetric-group.md#divisor-closure-of-hook-lengths)
        - [Rim hook](representation-theory-of-the-symmetric-group.md#rim-hook)
          - [Border-strip tableau](representation-theory-of-the-symmetric-group.md#border-strip-tableau)
      - [Content of a Young-diagram cell](representation-theory-of-the-symmetric-group.md#content-of-a-young-diagram-cell)
      - [Principal hook lengths of a partition](representation-theory-of-the-symmetric-group.md#principal-hook-lengths-of-a-partition)
    - [Beta set of a partition](representation-theory-of-the-symmetric-group.md#beta-set-of-a-partition)
      - [Beta number of a partition](representation-theory-of-the-symmetric-group.md#beta-number-of-a-partition)
      - [Beta-set hook-product identity](representation-theory-of-the-symmetric-group.md#beta-set-hook-product-identity)
        - [Square-sum identity for shifted partition coordinates](representation-theory-of-the-symmetric-group.md#square-sum-identity-for-shifted-partition-coordinates)
      - [Hook criterion in a beta set](representation-theory-of-the-symmetric-group.md#hook-criterion-in-a-beta-set)
      - [Abacus of a partition](representation-theory-of-the-symmetric-group.md#abacus-of-a-partition)
        - [Core-quotient bijection for partitions](representation-theory-of-the-symmetric-group.md#core-quotient-bijection-for-partitions)
        - [Core of a partition](representation-theory-of-the-symmetric-group.md#core-of-a-partition)
          - [Weight of a partition](representation-theory-of-the-symmetric-group.md#weight-of-a-partition)
          - [Odd-minus-even hook count of a partition](representation-theory-of-the-symmetric-group.md#odd-minus-even-hook-count-of-a-partition)
        - [Quotient of a partition](representation-theory-of-the-symmetric-group.md#quotient-of-a-partition)
          - [Hooks divisible by the abacus modulus](representation-theory-of-the-symmetric-group.md#hooks-divisible-by-the-abacus-modulus)
        - [Quotient tower of a partition](representation-theory-of-the-symmetric-group.md#quotient-tower-of-a-partition)
          - [Four-quotient of the partition three-one](representation-theory-of-the-symmetric-group.md#four-quotient-of-the-partition-three-one)
          - [Two-quotient tower of the partition three-one](representation-theory-of-the-symmetric-group.md#two-quotient-tower-of-the-partition-three-one)
          - [Iterated quotient equals a power quotient up to permutation](representation-theory-of-the-symmetric-group.md#iterated-quotient-equals-a-power-quotient-up-to-permutation)
        - [Core tower of a partition](representation-theory-of-the-symmetric-group.md#core-tower-of-a-partition)
          - [Power-core truncation of a prime-core tower](representation-theory-of-the-symmetric-group.md#power-core-truncation-of-a-prime-core-tower)
          - [P-adic valuation of a symmetric-group character degree from the core tower](representation-theory-of-the-symmetric-group.md#p-adic-valuation-of-a-symmetric-group-character-degree-from-the-core-tower)
            - [Character degree coprime to p from the core tower](representation-theory-of-the-symmetric-group.md#character-degree-coprime-to-p-from-the-core-tower)
            - [Character-degree valuation does not increase on taking the p-core](representation-theory-of-the-symmetric-group.md#character-degree-valuation-does-not-increase-on-taking-the-p-core)
        - [Residue content of a partition](representation-theory-of-the-symmetric-group.md#residue-content-of-a-partition)
    - [Young tableau](representation-theory-of-the-symmetric-group.md#young-tableau)
      - [Young symmetrizer](representation-theory-of-the-symmetric-group.md#young-symmetrizer)
        - [Row-column collision lemma](representation-theory-of-the-symmetric-group.md#row-column-collision-lemma)
      - [Robinson–Schensted correspondence](representation-theory-of-the-symmetric-group.md#robinson-schensted-correspondence)
        - [Robinson-Schensted-Knuth correspondence](representation-theory-of-the-symmetric-group.md#robinson-schensted-knuth-correspondence)
          - [RSK insertion shape](representation-theory-of-the-symmetric-group.md#rsk-insertion-shape)
          - [RSK growth-diagram local rule](representation-theory-of-the-symmetric-group.md#rsk-growth-diagram-local-rule)
            - [Trace and odd columns in symmetric RSK](representation-theory-of-the-symmetric-group.md#trace-and-odd-columns-in-symmetric-rsk)
        - [Dual Robinson–Schensted–Knuth correspondence](representation-theory-of-the-symmetric-group.md#dual-robinson-schensted-knuth-correspondence)
      - [Row insertion](representation-theory-of-the-symmetric-group.md#row-insertion)
        - [Row-insertion bumping-path monotonicity](representation-theory-of-the-symmetric-group.md#row-insertion-bumping-path-monotonicity)
      - [Near Young tableau](representation-theory-of-the-symmetric-group.md#near-young-tableau)
      - [Standard Young tableau](representation-theory-of-the-symmetric-group.md#standard-young-tableau)
        - [Column-reading order of standard Young tableaux](representation-theory-of-the-symmetric-group.md#column-reading-order-of-standard-young-tableaux)
          - [Triangular vanishing of Young-symmetrizer products](representation-theory-of-the-symmetric-group.md#triangular-vanishing-of-young-symmetrizer-products)
        - [Admissible adjacent swap of a standard Young tableau](representation-theory-of-the-symmetric-group.md#admissible-adjacent-swap-of-a-standard-young-tableau)
        - [Content vector of a standard Young tableau](representation-theory-of-the-symmetric-group.md#content-vector-of-a-standard-young-tableau)
          - [Axial distance in a Young tableau](representation-theory-of-the-symmetric-group.md#axial-distance-in-a-young-tableau)
      - [Semistandard Young tableau](representation-theory-of-the-symmetric-group.md#semistandard-young-tableau)
        - [Bender-Knuth involution](representation-theory-of-the-symmetric-group.md#bender-knuth-involution)
        - [Lattice word](representation-theory-of-the-symmetric-group.md#lattice-word)
      - [Row and column stabilizers of a Young tableau](representation-theory-of-the-symmetric-group.md#row-and-column-stabilizers-of-a-young-tableau)
      - [Tabloid](representation-theory-of-the-symmetric-group.md#tabloid)
        - [Young permutation module](representation-theory-of-the-symmetric-group.md#young-permutation-module)
          - [Character of a Young permutation module](representation-theory-of-the-symmetric-group.md#character-of-a-young-permutation-module)
          - [Signed Young permutation module](representation-theory-of-the-symmetric-group.md#signed-young-permutation-module)
          - [Young's rule](representation-theory-of-the-symmetric-group.md#young-s-rule)
            - [Vershik linear relations](representation-theory-of-the-symmetric-group.md#vershik-linear-relations)
            - [Two-row Young permutation module decomposition](representation-theory-of-the-symmetric-group.md#two-row-young-permutation-module-decomposition)
            - [Kostka number](representation-theory-of-the-symmetric-group.md#kostka-number)
          - [Specht filtration of the ordered-pair permutation module](representation-theory-of-the-symmetric-group.md#specht-filtration-of-the-ordered-pair-permutation-module)
        - [Polytabloid](representation-theory-of-the-symmetric-group.md#polytabloid)
          - [Column antisymmetrizer of a Young tableau](representation-theory-of-the-symmetric-group.md#column-antisymmetrizer-of-a-young-tableau)
            - [Dominance from a nonzero column antisymmetrizer](representation-theory-of-the-symmetric-group.md#dominance-from-a-nonzero-column-antisymmetrizer)
            - [Nonzero column antisymmetrizer criterion](representation-theory-of-the-symmetric-group.md#nonzero-column-antisymmetrizer-criterion)
          - [Specht module](representation-theory-of-the-symmetric-group.md#specht-module)
            - [Standard polytabloid basis](representation-theory-of-the-symmetric-group.md#standard-polytabloid-basis)
              - [Garnir relation](representation-theory-of-the-symmetric-group.md#garnir-relation)
            - [Semistandard homomorphism theorem](representation-theory-of-the-symmetric-group.md#semistandard-homomorphism-theorem)
            - [Kernel intersection theorem for Specht modules](representation-theory-of-the-symmetric-group.md#kernel-intersection-theorem-for-specht-modules)
              - [Invariant vector criterion for a Specht module](representation-theory-of-the-symmetric-group.md#invariant-vector-criterion-for-a-specht-module)
            - [Alternating-group restriction of Specht modules](representation-theory-of-the-symmetric-group.md#alternating-group-restriction-of-specht-modules)
              - [Smallest non-linear ordinary degree of an alternating group](representation-theory-of-the-symmetric-group.md#smallest-non-linear-ordinary-degree-of-an-alternating-group)
            - [Generalized Specht module](representation-theory-of-the-symmetric-group.md#generalized-specht-module)
              - [Pair of partitions for a generalized Specht module](representation-theory-of-the-symmetric-group.md#pair-of-partitions-for-a-generalized-specht-module)
                - [Good-letter matching in a tableau word](representation-theory-of-the-symmetric-group.md#good-letter-matching-in-a-tableau-word)
            - [Specht filtration](representation-theory-of-the-symmetric-group.md#specht-filtration)
              - [Littlewood–Richardson rule](representation-theory-of-the-symmetric-group.md#littlewood-richardson-rule)
                - [Littlewood–Richardson coefficient](representation-theory-of-the-symmetric-group.md#littlewood-richardson-coefficient)
                - [Pieri rule](representation-theory-of-the-symmetric-group.md#pieri-rule)
            - [Specht modules as minimal left ideals](representation-theory-of-the-symmetric-group.md#specht-modules-as-minimal-left-ideals)
            - [James submodule theorem](representation-theory-of-the-symmetric-group.md#james-submodule-theorem)
            - [Conjugate Specht module as a sign-twisted dual](representation-theory-of-the-symmetric-group.md#conjugate-specht-module-as-a-sign-twisted-dual)
            - [Restriction branching rule for a symmetric group](representation-theory-of-the-symmetric-group.md#restriction-branching-rule-for-a-symmetric-group)
              - [Standard-character multiplicity in a Specht self-product](representation-theory-of-the-symmetric-group.md#standard-character-multiplicity-in-a-specht-self-product)
            - [Linear independence of standard polytabloids](representation-theory-of-the-symmetric-group.md#linear-independence-of-standard-polytabloids)
            - [Hook-length formula](representation-theory-of-the-symmetric-group.md#hook-length-formula)
              - [Least non-linear ordinary degree of a symmetric group](representation-theory-of-the-symmetric-group.md#least-non-linear-ordinary-degree-of-a-symmetric-group)
              - [Trace computation of Specht module dimension](representation-theory-of-the-symmetric-group.md#trace-computation-of-specht-module-dimension)
              - [Determinant formula for Specht module dimension](representation-theory-of-the-symmetric-group.md#determinant-formula-for-specht-module-dimension)
              - [Greene–Nijenhuis–Wilf hook walk](representation-theory-of-the-symmetric-group.md#greene-nijenhuis-wilf-hook-walk)
                - [Hook walk terminal probability](representation-theory-of-the-symmetric-group.md#hook-walk-terminal-probability)
            - [Murnaghan–Nakayama rule](representation-theory-of-the-symmetric-group.md#murnaghan-nakayama-rule)
              - [Power-sum border-strip multiplication](representation-theory-of-the-symmetric-group.md#power-sum-border-strip-multiplication)
                - [Staircase Schur functions use only odd power sums](representation-theory-of-the-symmetric-group.md#staircase-schur-functions-use-only-odd-power-sums)
              - [Maximal p-hook character formula](representation-theory-of-the-symmetric-group.md#maximal-p-hook-character-formula)
              - [Sign of an abacus hook-removal sequence](representation-theory-of-the-symmetric-group.md#sign-of-an-abacus-hook-removal-sequence)
              - [Two-row alternating character cancellation](representation-theory-of-the-symmetric-group.md#two-row-alternating-character-cancellation)
              - [Principal-hook character value of a symmetric group](representation-theory-of-the-symmetric-group.md#principal-hook-character-value-of-a-symmetric-group)
              - [Staircase-character vanishing criterion](representation-theory-of-the-symmetric-group.md#staircase-character-vanishing-criterion)
              - [Conjugate Specht character](representation-theory-of-the-symmetric-group.md#conjugate-specht-character)
              - [Straightening of a symmetric-group character indexed by a composition](representation-theory-of-the-symmetric-group.md#straightening-of-a-symmetric-group-character-indexed-by-a-composition)
            - [Modular Specht module](representation-theory-of-the-symmetric-group.md#modular-specht-module)
              - [Tabloid bilinear form](representation-theory-of-the-symmetric-group.md#tabloid-bilinear-form)
              - [Regular partition](representation-theory-of-the-symmetric-group.md#regular-partition)
                - [Regular label of the modular sign representation](representation-theory-of-the-symmetric-group.md#regular-label-of-the-modular-sign-representation)
                - [Simple symmetric-group module from a regular partition](representation-theory-of-the-symmetric-group.md#simple-symmetric-group-module-from-a-regular-partition)
                  - [Absolute irreducibility of the Specht radical quotient](representation-theory-of-the-symmetric-group.md#absolute-irreducibility-of-the-specht-radical-quotient)
                - [Endomorphism theorem for a regular Specht module](representation-theory-of-the-symmetric-group.md#endomorphism-theorem-for-a-regular-specht-module)
    - [Dominance order on partitions](representation-theory-of-the-symmetric-group.md#dominance-order-on-partitions)
      - [Single-box up-move](representation-theory-of-the-symmetric-group.md#single-box-up-move)
  - [Brauer defect-zero vanishing theorem](representation-theory-of-the-symmetric-group.md#brauer-defect-zero-vanishing-theorem)
  - [Symmetric-group character co-degree vanishing criterion](representation-theory-of-the-symmetric-group.md#symmetric-group-character-co-degree-vanishing-criterion)
- [Intertwining operator](#intertwining-operator)
  - [Reduced matrix element](#reduced-matrix-element)
    - [Wigner-Eckart theorem](#wigner-eckart-theorem)
    - [Two reduced octet matrix elements](#two-reduced-octet-matrix-elements)
- [Schur's lemma](#schur-s-lemma)
  - [Proof of Schur lemma](#proof-of-schur-lemma)
  - [Failure of the scalar conclusion of Schur lemma over the real numbers](#failure-of-the-scalar-conclusion-of-schur-lemma-over-the-real-numbers)
  - [Cyclic-center obstruction to a faithful irreducible representation](#cyclic-center-obstruction-to-a-faithful-irreducible-representation)
- [Dual representation](#dual-representation)
  - [Algebraic contragredient representation](#algebraic-contragredient-representation)
    - [Conjugate contragredient representation](#conjugate-contragredient-representation)
    - [Smooth dual](#smooth-dual)
      - [Conductors force finite support in a smooth dual](#conductors-force-finite-support-in-a-smooth-dual)
  - [Character of a Hom representation](#character-of-a-hom-representation)
    - [Two-sided regular representation decomposition](#two-sided-regular-representation-decomposition)
  - [Invariant bilinear form as an intertwiner](#invariant-bilinear-form-as-an-intertwiner)
    - [Symmetric-or-alternating dichotomy for invariant forms](#symmetric-or-alternating-dichotomy-for-invariant-forms)
- [Induced representation](#induced-representation)
  - [Extension of a faithful representation from an open normal subgroup](#extension-of-a-faithful-representation-from-an-open-normal-subgroup)
  - [Unnormalized parabolic induction](#unnormalized-parabolic-induction)
    - [Evaluation adjunction for unnormalized induction](#evaluation-adjunction-for-unnormalized-induction)
    - [Local principal series of GL2](#local-principal-series-of-gl2)
      - [Local Steinberg representation of GL2](#local-steinberg-representation-of-gl2)
      - [Equal-character Jacquet self-extension for GL2](#equal-character-jacquet-self-extension-for-gl2)
  - [Monomiality of irreducible representations of finite p-groups](#monomiality-of-irreducible-representations-of-finite-p-groups)
  - [Induced character](#induced-character)
    - [Monomial character](#monomial-character)
    - [Character induction norm bound](#character-induction-norm-bound)
    - [Irreducible characters across an index-two subgroup](#irreducible-characters-across-an-index-two-subgroup)
  - [Rotation content of induced Lorentz representations](#rotation-content-of-induced-lorentz-representations)
  - [Conjugate subgroup representation](#conjugate-subgroup-representation)
  - [Character formula for an induced representation](#character-formula-for-an-induced-representation)
  - [Induction from an abelian normal subgroup with a free character orbit](#induction-from-an-abelian-normal-subgroup-with-a-free-character-orbit)
    - [Irreducible characters of the affine semidirect product of orders eleven and five](#irreducible-characters-of-the-affine-semidirect-product-of-orders-eleven-and-five)
  - [Tensor identity for induced representations](#tensor-identity-for-induced-representations)
  - [Frobenius reciprocity](#frobenius-reciprocity)
  - [Mackey theory](#mackey-theory)
    - [Mackey restriction formula](#mackey-restriction-formula)
      - [Mackey irreducibility criterion](#mackey-irreducibility-criterion)
      - [Bruhat decomposition of SL2 over a finite field](#bruhat-decomposition-of-sl2-over-a-finite-field)
        - [Mackey inner product for the finite SL2 principal series](#mackey-inner-product-for-the-finite-sl2-principal-series)
          - [Irreducible principal series of finite SL2](#irreducible-principal-series-of-finite-sl2)
  - [Square orbits of additive characters of a finite field](#square-orbits-of-additive-characters-of-a-finite-field)
    - [Induction from the diagonal subgroup of upper-triangular SL2](#induction-from-the-diagonal-subgroup-of-upper-triangular-sl2)
- [Irreducible representation](#irreducible-representation)
  - [Totally symmetric representation](#totally-symmetric-representation)
  - [Absolute irreducibility of a group representation](#absolute-irreducibility-of-a-group-representation)
  - [Absolutely irreducible real representation](#absolutely-irreducible-real-representation)
  - [Eigenvalue orbit under conjugation](#eigenvalue-orbit-under-conjugation)
  - [Irreducible complex representations of a finite dihedral group](#irreducible-complex-representations-of-a-finite-dihedral-group)
    - [Two-dimensional representations of a finite dihedral group](#two-dimensional-representations-of-a-finite-dihedral-group)
      - [Faithful irreducible representation of D8](#faithful-irreducible-representation-of-d8)
- [Infinite dihedral group](#infinite-dihedral-group)
  - [Representation of the infinite dihedral group](#representation-of-the-infinite-dihedral-group)
    - [Nonfaithful representations of the infinite dihedral group](#nonfaithful-representations-of-the-infinite-dihedral-group)
    - [Quadratic-polynomial representation of the infinite dihedral group](#quadratic-polynomial-representation-of-the-infinite-dihedral-group)
    - [Induced two-dimensional dihedral representation](#induced-two-dimensional-dihedral-representation)
- [One-dimensional character](#one-dimensional-character)
  - [One-dimensional characters factor through the abelianization](#one-dimensional-characters-factor-through-the-abelianization)
- [Finite quotient representation](#finite-quotient-representation)
- [Indecomposable representation](#indecomposable-representation)
  - [Nonsplit extension of representations](#nonsplit-extension-of-representations)
    - [Split extension as a degeneration](#split-extension-as-a-degeneration)
  - [Unipotent representation](#unipotent-representation)

## Representation ring of a compact group

↑ **Parent:** [Representation theory](representation-theory.md)

The representation ring is the [Grothendieck group](algebraic-topology.md#grothendieck-group) of finite-dimensional complex [unitary representations](#unitary-representation) of a [compact group](topological-group.md#compact-group), with addition induced by [direct sum](vector-space.md#direct-sum) and multiplication by [tensor product](multilinear-algebra.md#tensor-product). As an abelian group it is freely generated by the irreducible [unitary representations](#unitary-representation). Taking dimension gives a ring homomorphism $R(G)\to\mathbb Z$.

### Representation ring of an odd-dimensional special orthogonal group

↑ **Parent:** [Representation ring of a compact group](#representation-ring-of-a-compact-group)

For the block-rotation [maximal torus](lie-theory.md#maximal-torus) in the [special orthogonal group](linear-algebra.md#special-orthogonal-group) $SO(2m+1)$, the [Weyl group](semisimple-lie-algebra.md#weyl-group) acts by permutations and independent inversions of $z_i$. Its invariant [Laurent polynomials](polynomial.md#laurent-polynomial) are the symmetric polynomials in $x_i=z_i+z_i^{-1}$, hence the polynomial ring in their [elementary symmetric polynomials](polynomial.md#elementary-symmetric-polynomial) $e_1,\ldots,e_m$. Restriction of the group [representation ring of a compact group](#representation-ring-of-a-compact-group) is injective because every group element is conjugate into the torus and [characters](#character-of-a-representation) distinguish virtual representations. For the defining complexified representation $V$, the exterior-power characters satisfy $\sum_k\chi_{\Lambda^kV}t^k=(1+t)\prod_i(1+x_it+t^2)$. For $k\leq m$, its coefficient is $e_k$ plus an integral linear combination of $e_j$ for $j<k$. Induction puts every $e_k$ in the restriction image, proving equality with the invariant ring and giving polynomial generators $[\Lambda^1V],\ldots,[\Lambda^mV]$.

## Subrepresentation

↑ **Parent:** [Representation theory](representation-theory.md)

A subrepresentation is an [invariant subspace](#invariant-subspace) of a [group representation](#group-representation) or [Lie algebra representation](lie-algebra.md#lie-algebra-representation), with the restricted action.

### Quotient representation

↑ **Parent:** [Subrepresentation](#subrepresentation)

For a [subrepresentation](#subrepresentation) $W\subseteq V$, the [quotient vector space](vector-space.md#quotient-vector-space) $V/W$ inherits the action. For a [Lie algebra representation](lie-algebra.md#lie-algebra-representation), the formula is $x(v+W)=xv+W$, well-defined because $W$ is invariant.

## Group representation

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_representation)

A group representation is a [group homomorphism](group-theory.md#group-homomorphism) from a [group](group.md) to the [general linear group](group-theory.md#general-linear-group) of a [vector space](vector-space.md). It realizes abstract group elements as invertible linear transformations.

The defining identities are $\rho(e)=I$ and $\rho(gh)=\rho(g)\rho(h)$, so an [inverse element](algebraic-operation.md#inverse-element) is represented by a [matrix inverse](matrix-inverse.md). A choice of [basis](vector-space.md#basis) gives a [matrix representation](#matrix-representation), but the underlying action does not depend on that choice. The action need not distinguish every group element: the [trivial representation](#trivial-representation) sends all of them to $I$.

### Character projection operator

↑ **Parent:** [Group representation](#group-representation)

For a finite [group](group.md) $G$ represented unitarily by $U(g)$, the central projector onto the isotypic subspace of an [irreducible representation](#irreducible-representation) $\lambda$ is $P_\lambda=(d_\lambda/|G|)\sum_g\chi_\lambda(g)^*U(g)$, where $d_\lambda$ is its [dimension](vector-space.md#dimension-vector-space). [Character orthogonality](#character-orthogonality) implies that the operator is identity on copies of $\lambda$ and zero on other irreducibles. For a one-dimensional irreducible, applying it to an [atomic orbital](chemistry.md#atomic-orbital) gives either zero or a [symmetry-adapted linear combination](chemistry.md#symmetry-adapted-linear-combination) of that [symmetry](physics.md#symmetry-physics), to be normalized afterward. A multidimensional central projector selects an entire isotypic component rather than one uniquely chosen component function.

### Quarter-turn action on diagonal quadratic forms

↑ **Parent:** [Group representation](#group-representation)

Let $J$ be the plane [rotation matrix](linear-algebra.md#rotation-matrix) through $\pi/2$, generating a [cyclic group](group.md#cyclic-group) of order four. A [quadratic form](quadratic-form.md) $ax^2+by^2$ has its two coefficients exchanged by a quarter-turn and unchanged by a half-turn. Thus the pullback action on this two-dimensional space gives the displayed [group representation](#group-representation): $D(J^k)=D(J)^k$, with $D(J)^2=I$. It is not a [faithful representation](#faithful-representation), because its [kernel of a group homomorphism](group-theory.md#kernel-of-a-group-homomorphism) is $\{I,J^2\}$. Its two invariant coefficient lines correspond to $x^2+y^2$ and $x^2-y^2$, on which a quarter-turn acts by $+1$ and $-1$, respectively. Restricting to this diagonal space is valid for these signed coordinate permutations; a general [linear transformation](vector-space.md#linear-map) can introduce an $xy$ term.

### Equivalence of group representations

↑ **Parent:** [Group representation](#group-representation)

Two finite-dimensional [group representations](#group-representation) $D,E$ over the same [field](algebra.md#field) are equivalent if there is one invertible linear map $S$ intertwining all their group actions, equivalently $E(g)=S^{-1}D(g)S$ for every $g$. The same change of basis must work simultaneously for all group elements. The [cyclic property of the trace](linear-algebra.md#cyclic-property-of-the-trace) implies that [equivalent representations](#equivalence-of-group-representations) have identical [characters](#character-of-a-representation): $\operatorname{tr}(S^{-1}D(g)S)=\operatorname{tr}D(g)$. Consequently a difference at a single group element proves inequivalence. This implication does not need the group to be finite, and the reverse implication is not asserted for arbitrary groups or fields.

### Inverse-adjoint representation

↑ **Parent:** [Group representation](#group-representation)

For a complex finite-dimensional [group representation](#group-representation), the displayed matrices give another [group representation](#group-representation): taking inverses and taking the [conjugate transpose](linear-operator-theory.md#conjugate-transpose) each reverse multiplication order, so their composition preserves it. This operation is involutive. With the standard [Hermitian inner product](linear-algebra.md#hermitian-inner-product), an invariant [vector subspace](vector-space.md#vector-subspace) $W$ for $D^\sharp$ has [orthogonal complement](hilbert-space.md#orthogonal-complement) invariant for $D$, because $D(g)^\dagger W=D^\sharp(g^{-1})W\subseteq W$. Thus $\langle w,D(g)v\rangle=\langle D(g)^\dagger w,v\rangle=0$ for $v\in W^\perp,w\in W$. It follows that $D^\sharp$ is an [irreducible representation](#irreducible-representation) exactly when $D$ is. No finiteness assumption on the [group](group.md) or unitarity assumption on the [group representation](#group-representation) is needed.

### One-dimensional representation

↑ **Parent:** [Group representation](#group-representation)

A one-dimensional complex [group representation](#group-representation) acts on a one-dimensional complex [vector space](vector-space.md), and is equivalently a [group homomorphism](group-theory.md#group-homomorphism) into the multiplicative [group](group.md) $\mathbb C^\times$. It is automatically an [irreducible representation](#irreducible-representation). Its [character of a representation](#character-of-a-representation) is its scalar value, a [one-dimensional character](#one-dimensional-character). A change of [basis](vector-space.md#basis) cannot change those scalar values, so two such [group representations](#group-representation) are equivalent exactly when their homomorphisms agree. For a [symmetric group](finite-group-theory.md#symmetric-group) $S_n$ with $n\geq2$, all [transpositions](combinatorics.md#transposition-permutation) are conjugate, square to the identity and generate the group. Their common scalar image is therefore $1$ or $-1$, giving exactly the [trivial representation](#trivial-representation) and the [sign representation](representation-theory-of-the-symmetric-group.md#sign-representation).

### Projective representation

↑ **Parent:** [Group representation](#group-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_representation)

A [projective representation](#projective-representation) is a [group homomorphism](group-theory.md#group-homomorphism) into the projective linear group of a [vector space](vector-space.md). Choosing invertible linear representatives makes multiplication hold up to nonzero scalar factors. A [projective unitary representation](wave-function.md#projective-unitary-representation) chooses [unitary operators](vector-space.md#unitary-operator) as representatives, whose scalar factors have modulus one.

### Orthogonal representation

↑ **Parent:** [Group representation](#group-representation)

An [orthogonal representation](#orthogonal-representation) is a real [group representation](#group-representation) preserving a positive-definite [inner product](inner-product.md), equivalently a [group homomorphism](group-theory.md#group-homomorphism) into an [orthogonal group](linear-algebra.md#orthogonal-group). Every finite-dimensional [continuous](calculus.md#continuous-function) [real representation](#real-representation) of a [compact group](topological-group.md#compact-group) has this form after averaging an [inner product](inner-product.md) over [Haar measure](measure.md#haar-measure), by [orthogonalization of a compact-group representation](#orthogonalization-of-a-compact-group-representation).

### Representation over the rational numbers

↑ **Parent:** [Group representation](#group-representation)

A [representation over the rational numbers](#representation-over-the-rational-numbers) is a [group representation](#group-representation) on a finite-dimensional rational [vector space](vector-space.md). Choosing a basis gives rational matrices. It differs from a [rational representation of an algebraic group](lie-theory.md#rational-representation), where rational refers to regular matrix-coefficient functions rather than the ground [field](algebra.md#field). Scalar extension yields [representations](#group-representation) over every characteristic-zero [field](algebra.md#field).

### Scalar endomorphisms obstruct a split extension

↑ **Parent:** [Group representation](#group-representation)

If a representation has one-dimensional endomorphism algebra, it cannot be a [direct sum](vector-space.md#direct-sum) of two nonzero invariant subspaces: the two coordinate projections would be independent endomorphisms. This obstruction does not require either summand to be irreducible, and does not assert that scalar endomorphisms alone imply irreducibility.

### Distinct-character extensions of an abelian group split

↑ **Parent:** [Group representation](#group-representation)

A two-dimensional representation of an [abelian group](group.md#abelian-group) fitting into an extension of two distinct [linear characters](#linear-character) splits. Choose an element on which the [linear characters](#linear-character) differ. Its matrix has two distinct [eigenvalues](linear-operator-theory.md#eigenvalue), and all commuting group operators preserve its two eigenlines. Those eigenlines supply the two invariant [linear character](#linear-character) summands. The argument does not apply when the two [linear characters](#linear-character) coincide.

### Smooth representation of a locally profinite group

↑ **Parent:** [Group representation](#group-representation)

A complex [group representation](#group-representation) $\pi:G\to\operatorname{GL}(V)$ is smooth when every vector is fixed by some [compact-open subgroup](topological-group.md#compact-open-subgroup). Equivalently each vector's stabilizer is open. Smoothness is local constancy of orbit maps with the vector space regarded discretely, not ordinary continuity into a finite-dimensional complex topology.

#### Smooth vector

↑ **Parent:** [Smooth representation of a locally profinite group](#smooth-representation-of-a-locally-profinite-group)

A [smooth vector](#smooth-vector) in any abstract group representation of a [locally profinite group](topological-group.md#locally-profinite-group) has an open stabilizer, equivalently is fixed by some [compact-open subgroup](topological-group.md#compact-open-subgroup). [Smooth vectors](#smooth-vector) form an invariant linear subspace: use intersections for addition and conjugation for translation. A [smooth representation](#smooth-representation-of-a-locally-profinite-group) is one in which every vector has this property.

#### Smooth character

↑ **Parent:** [Smooth representation of a locally profinite group](#smooth-representation-of-a-locally-profinite-group)

A smooth [linear character](#linear-character) is a one-dimensional [smooth representation](#smooth-representation-of-a-locally-profinite-group), equivalently a homomorphism whose kernel is open. On a local multiplicative group, each smooth [linear character](#linear-character) is trivial on some sufficiently deep principal-unit subgroup. Its inverse has the same kernel.

#### Jacquet module

↑ **Parent:** [Smooth representation of a locally profinite group](#smooth-representation-of-a-locally-profinite-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacquet_module)

The unnormalized [Jacquet module](#jacquet-module) is the space of coinvariants of a unipotent subgroup $U$. If a subgroup $T$ normalizes $U$, it acts on this quotient. Every [linear functional](dual-space.md#linear-functional) transforming by a [linear character](#linear-character) trivial on $U$ factors through it. Normalized Jacquet functors include an additional modulus twist; that convention must be specified.

#### Smooth right regular representation

↑ **Parent:** [Smooth representation of a locally profinite group](#smooth-representation-of-a-locally-profinite-group)

The right action on [compactly supported locally constant functions](calculus.md#compactly-supported-locally-constant-function) is a [smooth representation](#smooth-representation-of-a-locally-profinite-group). For a [compact-open subgroup](topological-group.md#compact-open-subgroup) $K$, its [fixed-vector space](#fixed-vector-space) has basis the characteristic functions of cosets in $G/K$, since compact support on that discrete quotient is finite support. Consequently this representation is admissible exactly when $G$ is compact.

#### Admissible representation of a locally profinite group

↑ **Parent:** [Smooth representation of a locally profinite group](#smooth-representation-of-a-locally-profinite-group)

An [admissible representation](#admissible-representation-of-a-locally-profinite-group) is a [smooth representation](#smooth-representation-of-a-locally-profinite-group) for which every [fixed-vector space](#fixed-vector-space) $V^K$ for a [compact-open subgroup](topological-group.md#compact-open-subgroup) has finite dimension. Admissibility can hold for an infinite-dimensional representation; it bounds each local fixed level, not their union.

##### Contraction and admissible fixed spaces

↑ **Parent:** [Admissible representation of a locally profinite group](#admissible-representation-of-a-locally-profinite-group)

For the upper-triangular subgroup of $\operatorname{GL}_n(F)$, conjugation by $\operatorname{diag}(\varpi^{-(n-1)},\ldots,1)$ expands the upper-unipotent coordinates. For a decomposed [compact-open subgroup](topological-group.md#compact-open-subgroup) $K=T_0U_0$, its conjugates eventually contain $K$, while their [fixed-vector spaces](#fixed-vector-space) are isomorphic. Finite dimension therefore forces those spaces to be equal. Inverse conjugation contracts any fixed unipotent element into $U_0$, proving that the unipotent radical acts trivially in every admissible representation of this triangular group.

#### Fixed-vector space

↑ **Parent:** [Smooth representation of a locally profinite group](#smooth-representation-of-a-locally-profinite-group)

The [fixed-vector space](#fixed-vector-space) is $V^K=\{v:\pi(k)v=v\text{ for all }k\in K\}$. Conjugation gives an isomorphism $V^K\to V^{gKg^{-1}}$, $v\mapsto\pi(g)v$. If $K\subseteq L$, then $V^L\subseteq V^K$.

### Galois representation

↑ **Parent:** [Group representation](#group-representation)

A Galois representation is a continuous [group representation](#group-representation) of an [absolute Galois group](galois-theory.md#absolute-galois-group), usually on a vector space or lattice over a local field. Examples include the [cyclotomic character](#cyclotomic-character) and the representations attached to [modular forms](modular-function.md#modular-form). The coefficient topology is part of the definition.

#### Tate module

↑ **Parent:** [Galois representation](#galois-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tate_module)

For an [abelian variety](abelian-variety.md) $A$ and a [prime number](prime-number.md) $\ell$ different from the characteristic, the inverse limit of its geometric $\ell^n$-torsion, with transition multiplication by $\ell$, is its Tate module. For an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve), it is free of rank two over the [p-adic integers](number-theory.md#p-adic-integer) and satisfies $T_\ell(E)/\ell^nT_\ell(E)\simeq E[\ell^n]$. The [absolute Galois group](galois-theory.md#absolute-galois-group) acts continuously and commutes with all base-defined [endomorphisms](algebra.md#endomorphism).

##### CM Tate module stabilizer

↑ **Parent:** [Tate module](#tate-module)

Let $R=K\cap\operatorname{End}_k(E)$. If $\alpha\in R$ maps the [Tate module](#tate-module) into $\ell^nT_\ell(E)$, it kills $E[\ell^n]$ and factors through the quotient isogeny $[\ell^n]$. The resulting [endomorphism](algebra.md#endomorphism) is $\alpha/\ell^n$, belongs to $K$ and is defined over $k$, hence belongs to $R$. Approximation in $R\otimes\mathbb Z_\ell$ now identifies the displayed stabilizer. This does not assume that the integral [Tate module](#tate-module) is free over a possibly nonmaximal CM order.

##### Rational Tate module

↑ **Parent:** [Tate module](#tate-module)

Tensoring a [Tate module](#tate-module) with the [P-adic numbers](non-archimedean-analysis.md#p-adic-number) gives its rational Tate module. For a [CM elliptic curve](algebraic-geometry.md#cm-elliptic-curve) with base-defined multiplication by $K$, it is free of rank one over $K\otimes\mathbb Q_\ell$, including when this algebra is a product of two [fields](algebra.md#field). In the split case the two distinct roots of a nonrational CM endomorphism each have a one-dimensional eigenspace.

#### Galois character

↑ **Parent:** [Galois representation](#galois-representation)

A Galois character is a continuous one-dimensional [Galois representation](#galois-representation): the [absolute Galois group](galois-theory.md#absolute-galois-group) acts by multiplication by a scalar in a coefficient [field](algebra.md#field) $F$. A quadratic character over a coefficient field of characteristic different from two has values in $\{1,-1\}$; after identifying this group with $\mathbb Z/2\mathbb Z$, its kernel fixes a [quadratic extension](algebra.md#quadratic-extension), or the base field for the trivial character. Its restriction to an [inertia group](non-archimedean-analysis.md#inertia-group) is trivial exactly when that extension is unramified at the corresponding place.

#### Cyclotomic character

↑ **Parent:** [Galois representation](#galois-representation)

The cyclotomic character is defined by $g(\zeta)=\zeta^{\kappa(g)}$ on compatible $p$-power [roots of unity](algebra.md#root-of-unity). On the full cyclotomic tower of $\mathbb Q$, it identifies the [Galois group](galois-theory.md#galois-group) with $\mathbb Z_p^\times$. Its finite-order part is the [Teichmüller character](non-archimedean-analysis.md#teichmuller-character) and its pro-$p$ part acts through $1+p\mathbb Z_p$, or $1+4\mathbb Z_2$.

##### Tate twist

↑ **Parent:** [Cyclotomic character](#cyclotomic-character)

The Tate twist $M(1)$ multiplies a [Galois representation](#galois-representation)'s action by the [cyclotomic character](#cyclotomic-character). Here $\mathbb Z_p(1)$ is the inverse limit of $p$-power [roots of unity](algebra.md#root-of-unity) under power maps. For a one-variable [Iwasawa module](algebraic-number-theory.md#iwasawa-module), twisting changes characteristic power series by the corresponding change in the generator's action.

### Invariant theory

↑ **Parent:** [Group representation](#group-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Invariant_theory)

[Invariant theory](#invariant-theory) studies functions and tensors unchanged by a [group action](group-action.md). For a linear representation, the [polynomial invariant ring](#polynomial-invariant-ring) records invariant [polynomial](polynomial.md) functions on the representation space. Tensor invariants and commuting algebra actions connect it with [Schur–Weyl duality](lie-theory.md#schur-weyl-duality).

#### Geometric invariant theory

↑ **Parent:** [Invariant theory](#invariant-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometric_invariant_theory)

[Geometric invariant theory](#geometric-invariant-theory) constructs algebraic quotients of [group actions](group-action.md) by a [reductive algebraic group](lie-theory.md#reductive-group) using invariant sections and a chosen [linearization of a line bundle](#linearization-of-a-line-bundle). An affine quotient is the spectrum of the [polynomial invariant ring](#polynomial-invariant-ring); a projective quotient uses homogeneous invariants and excludes the points where all positive-degree invariants vanish. Stability separates the orbits which give well-behaved [geometric quotient](toric-geometry.md#geometric-quotient) points.

##### Hilbert-Mumford criterion for projective stability

↑ **Parent:** [Geometric invariant theory](#geometric-invariant-theory)

For a complex [reductive algebraic group](lie-theory.md#reductive-group) acting linearly on $V$, decompose a nonzero vector into weights for each [algebraic one-parameter subgroup](lie-theory.md#algebraic-one-parameter-subgroup). With the displayed sign convention, semistability is equivalent to $\mu\ge0$ for every such subgroup, and stability is equivalent to strict positivity for every nontrivial subgroup. One must test conjugates of the subgroups as well as those diagonal in a single fixed coordinate system.

###### Root-multiplicity criterion for stable binary forms

↑ **Parent:** [Hilbert-Mumford criterion for projective stability](#hilbert-mumford-criterion-for-projective-stability)

Under $\operatorname{diag}(t,t^{-1})$, acting by inverse substitution, $X^{d-j}Y^j$ has weight $2j-d$. If $r$ is the smallest active exponent of $Y$, the multiplicity at $[1:0]$ is $r$ and the Hilbert-Mumford value is $d-2r$. Conjugating replaces this point by any projective point. Thus strict positivity is exactly the displayed condition; replacing the strict inequality by $m_p\le d/2$ gives semistability. A [binary quartic](lie-theory.md#binary-quartic) is stable precisely when it has no repeated projective root.

##### Stable projective point in geometric invariant theory

↑ **Parent:** [Geometric invariant theory](#geometric-invariant-theory)

A point is stable when a positive-degree homogeneous invariant is nonzero there and its orbit is closed in that invariant's nonvanishing affine open set, with finite [stabilizer](group-action.md#stabilizer-subgroup). This is stronger than merely having a closed orbit or a nonzero invariant. For [binary forms](lie-theory.md#binary-form) of degree four, the stable points have four distinct projective roots.

##### Affine null cone

↑ **Parent:** [Geometric invariant theory](#geometric-invariant-theory)

The [affine null cone](#affine-null-cone) is the set of vectors whose orbit closure contains the origin. For a reductive algebraic group it is also the common zero locus of all positive-degree homogeneous invariants. A nonzero vector in this set represents an unstable projective point. The [Hilbert-Mumford criterion for the affine null cone](lie-theory.md#hilbert-mumford-criterion-for-the-affine-null-cone) detects membership by a [algebraic one-parameter subgroup](lie-theory.md#algebraic-one-parameter-subgroup) with only positive active weights.

###### Nilpotent cone for conjugation of matrices

↑ **Parent:** [Affine null cone](#affine-null-cone)

For conjugation of $n$ by $n$ complex matrices by the [special linear group](group-theory.md#special-linear-group), the [affine null cone](#affine-null-cone) consists exactly of the [nilpotent matrices](linear-operator-theory.md#nilpotent-matrix). If a conjugate tends to zero along an [algebraic one-parameter subgroup](lie-theory.md#algebraic-one-parameter-subgroup), its constant [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) must be $T^n$. Conversely, put a nilpotent matrix in strictly upper triangular form and conjugate it by $\operatorname{diag}(t^{n-1},t^{n-3},\ldots,t^{1-n})$. Every active matrix entry has positive weight and tends to zero. The [Hilbert-Mumford criterion for projective stability](#hilbert-mumford-criterion-for-projective-stability) therefore identifies the semistable locus of the projective conjugation representation as the complement of the projectivized nilpotent cone.

##### Semistable projective point in geometric invariant theory

↑ **Parent:** [Geometric invariant theory](#geometric-invariant-theory)

For the natural [linearization of a line bundle](#linearization-of-a-line-bundle) of the action on lines in $V$, a point is semistable when some positive-degree homogeneous invariant on $V$ is nonzero on a representative. This condition is independent of the representative. The nonsemistable vectors form the [affine null cone](#affine-null-cone).

##### Linearization of a line bundle

↑ **Parent:** [Geometric invariant theory](#geometric-invariant-theory)

A linearization of a line bundle is a group action on its total space lifting the action on the base, linear on each fibre and obeying the group law. It induces actions on global sections of its tensor powers. For the projective space of lines in a linear representation $V$, the induced action on the dual of the tautological line bundle gives the natural linearization of $\mathcal O(1)$. Geometric invariant theory uses its invariant sections to define the semistable locus.

#### Symbolic method for binary-form invariants

↑ **Parent:** [Invariant theory](#invariant-theory)

Replace a degree-$d$ [binary form](lie-theory.md#binary-form) by the formal power $(a_0x+a_1y)^d$ and recover its coefficients with the linear rule $a_0^{d-i}a_1^i\mapsto f_i$. For a coefficient invariant of degree $r$, use $r$ symbolic letters, each of degree $d$, polarize and then apply this rule to each letter. Products of brackets $(ab)=a_0b_1-a_1b_0$ generate the invariant expressions before the final coefficient substitution.

##### Transvectant of binary forms

↑ **Parent:** [Symbolic method for binary-form invariants](#symbolic-method-for-binary-form-invariants)

For forms of degrees $m,n$, the $r$th transvectant contracts $r$ pairs of indices using the invariant alternating form. Explicitly it is a scalar normalization of $\sum_{j=0}^r(-1)^j\binom rj(\partial_x^{r-j}\partial_y^j f)(\partial_x^j\partial_y^{r-j}g)$. These contractions realize the irreducible summands in the symmetric-power tensor-product decomposition.

#### Polynomial invariant ring

↑ **Parent:** [Invariant theory](#invariant-theory)

For a group acting linearly on $W$, act on the [coordinate ring](algebraic-variety.md#coordinate-ring) by $(g\cdot f)(w)=f(g^{-1}w)$. The [polynomial invariant ring](#polynomial-invariant-ring) is the fixed subalgebra $\mathbb C[W]^G$. It inherits the degree grading. Even over the complex numbers it need not be a [unique factorization domain](algebra.md#unique-factorization-domain), as the [quadratic cone invariant ring](#quadratic-cone-invariant-ring) demonstrates.

##### Determinant-one cyclic quotient of the affine plane

↑ **Parent:** [Polynomial invariant ring](#polynomial-invariant-ring)

The action $(x,y)\mapsto(\zeta x,\zeta^{-1}y)$ has invariant [monomials](polynomial.md#monomial) exactly when their two exponents differ by a multiple of $n$. Every such [monomial](polynomial.md#monomial) is a product of $x^n,y^n,xy$. Reducing by $uv=w^n$ leaves the [monomials](polynomial.md#monomial) $w^j$, $u^iw^j$ and $v^iw^j$ with $i\ge1$; their images are distinct [monomials](polynomial.md#monomial) in $x,y$, proving that this is the only relation. The map $(x,y)\mapsto(x^n,y^n,xy)$ is finite and its fibres are the finite-group orbits, so the hypersurface is the [geometric quotient](toric-geometry.md#geometric-quotient).

// Destination: ringed-space.bigb

##### Hilbert finite generation for reductive invariants

↑ **Parent:** [Polynomial invariant ring](#polynomial-invariant-ring)

Choose finitely many homogeneous positive-degree invariants generating the ideal generated by all positive-degree invariants in the ambient polynomial ring. Such a finite set exists because a polynomial ring is Noetherian. Apply the [Reynolds operator on a polynomial invariant ring](#reynolds-operator-on-a-polynomial-invariant-ring) to an expression for any homogeneous invariant in that ideal. Its coefficients become invariants of smaller degree, so induction proves that the chosen set generates the entire invariant ring as an algebra.

##### Reynolds operator on a polynomial invariant ring

↑ **Parent:** [Polynomial invariant ring](#polynomial-invariant-ring)

In characteristic zero, averaging over a compact group, or over a Zariski-dense compact form of a complex reductive group, gives a degree-preserving projection onto the [polynomial invariant ring](#polynomial-invariant-ring). Its module property is $\mathcal R(af)=a\mathcal R(f)$ for invariant $a$. This property turns finite ideal generation in the ambient polynomial ring into finite algebra generation of the invariant subring.

##### Binary dihedral invariant hypersurface

↑ **Parent:** [Polynomial invariant ring](#polynomial-invariant-ring)

Let $\zeta=e^{\pi i/n}$ and let the [binary dihedral group](finite-group-theory.md#dicyclic-group) act on $\mathbb C^2$ by $(x,y)\mapsto(\zeta x,\zeta^{-1}y)$ and $(x,y)\mapsto(-y,x)$. For $n\ge2$, the invariants

$$
U=x^{2n}+y^{2n},\qquad V=x^2y^2,\qquad W=xy(x^{2n}-y^{2n})
$$

present the invariant ring as $\mathbb C[U,V,W]/(W^2-VU^2+4V^{n+1})$. First take the cyclic invariants $A=x^{2n},B=y^{2n},C=xy$ with $AB=C^{2n}$. The residual involution interchanges $A,B$ and negates $C$, so invariant normal forms are polynomials in $A+B,C^2$ plus $C(A-B)$ times such polynomials. For $n=3$ the group has order twelve and the equation is $W^2-VU^2+4V^4=0$.

##### Quadratic cone invariant ring

↑ **Parent:** [Polynomial invariant ring](#polynomial-invariant-ring)

The scalar sign action of a [cyclic group](group.md#cyclic-group) of order two on $\mathbb C^2$ has invariant ring $\mathbb C[X^2,XY,Y^2]\cong\mathbb C[a,b,c]/(ac-b^2)$. It is not factorial: $a,b,c$ are pairwise nonassociate irreducibles, since every nonconstant invariant has degree at least two, while $ac=b^2$ gives two distinct factorizations.

##### Factorial invariant ring with no linear characters

↑ **Parent:** [Polynomial invariant ring](#polynomial-invariant-ring)

If a [finite group](group.md#finite-group) has no nontrivial homomorphism to $\mathbb C^\times$, its [polynomial invariant ring](#polynomial-invariant-ring) is a [unique factorization domain](algebra.md#unique-factorization-domain). Factor an invariant in the ambient [polynomial ring](commutative-algebra.md#polynomial-ring) and collect its irreducible factors into orbit products. Each orbit product transforms by a [linear character](#linear-character), hence is invariant. It is prime in the invariant ring, and the invariant factorization is a product of these primes.

##### Orbit product of polynomial factors

↑ **Parent:** [Polynomial invariant ring](#polynomial-invariant-ring)

A [finite group](group.md#finite-group) permutes the associate classes of irreducible [polynomial](polynomial.md) factors of an invariant. The product of one representative from each orbit transforms by a scalar [character](#character-of-a-representation) of the group. If that [character](#character-of-a-representation) is trivial, the product is invariant. Its transitive factor orbit makes it prime in the invariant ring: an invariant [polynomial](polynomial.md) divisible by one orbit factor is divisible by all of them.

##### Alternating-group polynomial invariants

↑ **Parent:** [Polynomial invariant ring](#polynomial-invariant-ring)

For the [permutation](combinatorics.md#permutation) action on $n$ coordinates with $n\geq2$, every alternating-group invariant is a [symmetric polynomial](polynomial.md#symmetric-polynomial) plus the Vandermonde product $\Delta$ times a [symmetric polynomial](polynomial.md#symmetric-polynomial). Thus the invariant ring is $\mathbb C[e_1,\ldots,e_n,Z]/(Z^2-D(e_1,\ldots,e_n))$, where $D$ is the discriminant [polynomial](polynomial.md). The two summands are independent over the [symmetric polynomial](polynomial.md#symmetric-polynomial) ring.

### Restriction of a representation

↑ **Parent:** [Group representation](#group-representation)

For a [group representation](#group-representation) of $G$ and a subgroup $H$, restriction keeps the vector space and lets only the elements of $H$ act. It is denoted $\operatorname{Res}_H^G V$.

#### Restriction multiplicity bound

↑ **Parent:** [Restriction of a representation](#restriction-of-a-representation)

For an irreducible complex character $\chi$ of a finite group $G$ and subgroup $H$, write its restriction as $\sum_i d_i\psi_i$. Orthogonality gives $\sum_i d_i^2=|H|^{-1}\sum_{h\in H}|\chi(h)|^2\le|G|/|H|$, because $|G|^{-1}\sum_G|\chi|^2=1$. Equality holds exactly when $\chi$ vanishes outside $H$, since the omitted sum consists of nonnegative terms.

### Sum of squares of irreducible representation dimensions

↑ **Parent:** [Group representation](#group-representation)

The regular [group representation](#group-representation) of a finite group over the complex numbers contains each [irreducible representation](#irreducible-representation) with multiplicity equal to its dimension. Consequently the sum of the squared dimensions is the group order. Once a list of distinct irreducibles exhausts this sum, it is complete.

### Intertwiner

↑ **Parent:** [Group representation](#group-representation)

An intertwiner between [group representations](#group-representation) $\rho$ on $V$ and $\sigma$ on $W$ is a [linear map](vector-space.md#linear-map) $A:V\to W$ satisfying $A\rho(x)=\sigma(x)A$ for every group element. The [Schur lemma](#schur-s-lemma) controls these maps between [irreducible representations](#irreducible-representation).

### Matrix coefficient

↑ **Parent:** [Group representation](#group-representation)

A matrix coefficient of a finite-dimensional [group representation](#group-representation) is a scalar function obtained by applying a [linear functional](dual-space.md#linear-functional) to the translate of a fixed vector. In a chosen [basis](vector-space.md#basis) these functions include $x\mapsto\rho(x)_{ij}$. For a [finite group](group.md#finite-group), the [Schur orthogonality relations](#schur-orthogonality-relations) make the scaled coefficients of all inequivalent [unitary irreducible representations](#unitary-irreducible-representation) an [orthonormal basis](inner-product.md#orthonormal-basis) of its scalar functions.

#### Schur orthogonality relations

↑ **Parent:** [Matrix coefficient](#matrix-coefficient)

For inequivalent chosen [unitary irreducible representations](#unitary-irreducible-representation) of a [finite group](group.md#finite-group), uniform [expectation](expected-value.md) gives

$$
\mathbb E_x\rho(x)_{ij}\overline{\sigma(x)_{kl}}
=\begin{cases}d_\rho^{-1}\delta_{ik}\delta_{jl},&\rho=\sigma,\\0,&\rho\ne\sigma.\end{cases}
$$

The [Kronecker deltas](multilinear-algebra.md#kronecker-delta) in the first case refer to entries in the same chosen [basis](vector-space.md#basis). Averaging an [intertwiner](#intertwiner) and applying the [Schur lemma](#schur-s-lemma) proves the formula; summing diagonal entries gives [character orthogonality](#character-orthogonality).

##### Character orthogonality for compact groups

↑ **Parent:** [Schur orthogonality relations](#schur-orthogonality-relations)

For finite-dimensional [unitary representations](#unitary-representation) of a [compact group](topological-group.md#compact-group), average the action on $\operatorname{Hom}(W,V)$ against normalized [Haar measure](measure.md#haar-measure). This is the [orthogonal projection](hilbert-space.md#orthogonal-projection) onto the [intertwining operators](#intertwining-operator), and its [trace](linear-algebra.md#matrix-trace) is the displayed integral. The [Schur lemma](#schur-s-lemma) therefore makes distinct [irreducible](#irreducible-representation) [characters](#character-of-a-representation) [orthogonal](inner-product.md#orthogonal-vectors) and each [irreducible](#irreducible-representation) [character](#character-of-a-representation) of norm one.

##### Schur averaging of rectangular matrices

↑ **Parent:** [Schur orthogonality relations](#schur-orthogonality-relations)

For chosen inequivalent [unitary irreducible representations](#unitary-irreducible-representation) $\rho,\sigma$ of a [finite group](group.md#finite-group) and a $d_\rho\times d_\sigma$ matrix $M$, the average $\mathbb E_x\rho(x)M\sigma(x)^*$ is zero when $\rho\ne\sigma$. For $\rho=\sigma$, it is $(\operatorname{tr}M/d_\rho)I$. This follows from the [Schur lemma](#schur-s-lemma), since the average intertwines the two [group representations](#group-representation). Equivalent representations in different bases require the corresponding [intertwiner](#intertwiner); the identity-matrix formula assumes literally the same representative.

### Cyclic vector for a group representation

↑ **Parent:** [Group representation](#group-representation)

A vector $v$ is cyclic for a [group representation](#group-representation) $\rho:G\to GL(V)$ if the [linear span](vector-space.md#linear-span) of $\{\rho(g)v:g\in G\}$ is all of $V$. Equivalently $v$ generates $V$ as a module over the [group algebra](associative-algebra.md#group-algebra). Its projection to the invariant subspace generates that subspace, so a cyclic representation of a [finite group](group.md#finite-group) has at most one copy of the [trivial representation](#trivial-representation).

#### Cyclic eigenvector obstruction to invariant vectors

↑ **Parent:** [Cyclic vector for a group representation](#cyclic-vector-for-a-group-representation)

In a [unitary representation](#unitary-representation) of a [finite group](group.md#finite-group), if a cyclic vector $v$ satisfies $\rho(g)v=av$ for some $a\ne1$, then there are no invariant vectors. Indeed the averaging [orthogonal projection](hilbert-space.md#orthogonal-projection) $P=|G|^{-1}\sum_h\rho(h)$ satisfies $P\rho(g)=P$, so $Pv=aPv=0$. All translates of $v$ also project to zero, and they span the representation.

### Multiplicity-free restriction

↑ **Parent:** [Group representation](#group-representation)

Restriction of an [irreducible representation](#irreducible-representation) to a [subgroup](group.md#subgroup) is multiplicity-free when its [semisimple representation](#semisimple-representation) decomposition has no repeated irreducible summands. Over the [complex numbers](complex-analysis.md#complex-number), for [finite groups](group.md#finite-group), this is equivalent to the restricted module's endomorphism algebra being commutative. This follows by writing that algebra as a product of [matrix algebras](associative-algebra.md#matrix-algebra) of sizes equal to the multiplicities.

### Pseudoreal representation

↑ **Parent:** [Group representation](#group-representation)

A pseudoreal [complex representation](#complex-representation) is isomorphic to its conjugate but has an invariant antilinear map squaring to minus the identity. Such [group representations](#group-representation) admit antisymmetric invariant bilinear forms and can support half-[hypermultiplets](supersymmetry.md#hypermultiplet) in four-dimensional [extended supersymmetry](supersymmetry.md#extended-supersymmetry).

### Splitting field for finite group representations

↑ **Parent:** [Group representation](#group-representation)

A [field](algebra.md#field) $k$ is a splitting [field](algebra.md#field) for a finite [group](group.md) $G$ if every [simple module](module-theory.md#irreducible-module) over its [group algebra](associative-algebra.md#group-algebra) $kG$ is absolutely simple: it remains simple over every extension [field](algebra.md#field). Equivalently, the quotient by the [Jacobson radical](noncommutative-algebra.md#jacobson-radical) is a product of full [matrix algebras](associative-algebra.md#matrix-algebra) over $k$. In [characteristic](algebra.md#characteristic-of-a-field) $p$, containing all $m$th [roots of unity](algebra.md#root-of-unity), where $|G|=p^a m$ and $p\nmid m$, is sufficient. This is the modular splitting-field theorem; it is substantially stronger than merely having [eigenvalues](linear-operator-theory.md#eigenvalue) for one chosen group element.

### Tensor product of group representations

↑ **Parent:** [Group representation](#group-representation)

For representations $V$ and $W$ of a group $G$, the tensor product representation is the [tensor product](multilinear-algebra.md#tensor-product) $V\otimes W$ with diagonal action

$$
g(v\otimes w)=(gv)\otimes(gw).
$$

#### Symmetric square of a group representation

↑ **Parent:** [Tensor product of group representations](#tensor-product-of-group-representations)

The subrepresentation of $V\otimes V$ fixed by exchange of the two tensor factors. In characteristic zero the projector is $(I+\tau)/2$, and its character is $[\chi(g)^2+\chi(g^2)]/2$. Real coordinate-quadratic perturbations of a nonmagnetic electronic multiplet transform in this symmetric square.

#### Trivial representation in a tensor square

↑ **Parent:** [Tensor product of group representations](#tensor-product-of-group-representations)

For a finite-dimensional irreducible complex representation $V$, invariant tensors in $V\otimes V$ correspond to equivariant maps $V^*\to V$. [Schur's lemma](#schur-s-lemma) makes their dimension one if $V$ is self-dual and zero otherwise. In particular a real-character irreducible representation has precisely one trivial copy in its tensor square. For arbitrary complex irreducibles, the unconditional statement is that $V\otimes V^*$ contains the trivial representation once.

#### External tensor product of group representations

↑ **Parent:** [Tensor product of group representations](#tensor-product-of-group-representations)

For a $G$-[representation](#group-representation) $V$ and an $H$-[representation](#group-representation) $W$ over the same [field](algebra.md#field), $V\boxtimes W$ is the [representation](#group-representation) of $G\times H$ on $V\otimes W$ given by $(g,h)(v\otimes w)=gv\otimes hw$. Its [character](#character-of-a-representation) is $(g,h)\mapsto\chi_V(g)\chi_W(h)$. Over a splitting field in characteristic zero the external products of irreducible [representations](#group-representation) form all irreducible representations of $G\times H$: character orthogonality gives irreducibility, and their squared degrees sum to $|G||H|$, proving exhaustion. Unlike the tensor product of two representations of one group, the two factors here act independently.

<h4 id="fundamental-antifundamental-decomposition-for-su-n">Fundamental-antifundamental decomposition for SU(N)</h4>

↑ **Parent:** [Tensor product of group representations](#tensor-product-of-group-representations)

Identify the product with endomorphisms of the defining space. [Special unitary group](topological-group.md#special-unitary-group) conjugation fixes scalar matrices and preserves the complementary traceless subspace. For $N\ge2$, the latter is the complex [Adjoint representation of a Lie algebra](lie-algebra.md#adjoint-representation-of-a-lie-algebra), which is irreducible because $\mathfrak{sl}_N$ is simple. With fundamental [Dynkin index](semisimple-lie-algebra.md#dynkin-index) $1/2$, the trace-Casimir identity gives $C_2(\mathbf N)=(N^2-1)/(2N)$; the [tensor-product Casimir trace identity](semisimple-lie-algebra.md#tensor-product-casimir-trace-identity) then gives $C_2(\mathbf{Adj})=N$.

<h4 id="su-n-tensor-transformation">SU(n) tensor transformation</h4>

↑ **Parent:** [Tensor product of group representations](#tensor-product-of-group-representations)

A $(j,k)$ [tensor](multilinear-algebra.md#tensor) has one [fundamental representation](semisimple-lie-algebra.md#fundamental-representation) factor for every upper index and a dual factor for every lower index. Under $A\in SU(n)$, upper factors transform by $A$ and lower factors by $A^{-1}$; unitarity identifies the latter with conjugate fundamental [matrices](vector-space.md#matrix). Thus [complex conjugation](complex-analysis.md#complex-conjugation) exchanges $(j,k)$ and $(k,j)$. Index permutations and contraction with an [invariant tensor](#invariant-tensor) commute with the action, producing [invariant subspaces](#invariant-subspace) and decomposition maps.

#### Invariant tensor

↑ **Parent:** [Tensor product of group representations](#tensor-product-of-group-representations)

An invariant [tensor](multilinear-algebra.md#tensor) is fixed by every element of the represented group, so it spans or belongs to a trivial [group representation](#group-representation). The [special unitary group](topological-group.md#special-unitary-group) preserves its identity [tensor](multilinear-algebra.md#tensor) and the upper and lower volume [tensors](multilinear-algebra.md#tensor). Such [tensors](multilinear-algebra.md#tensor) make [tensor contraction](multilinear-algebra.md#tensor-contraction) equivariant and permit invariant inner products and real structures.

#### Octet and singlet in a fundamental SU3 tensor product

↑ **Parent:** [Tensor product of group representations](#tensor-product-of-group-representations)

The [tensor-product weight diagram](semisimple-lie-algebra.md#tensor-product-weight-diagram) has six distinct nonzero differences of the three defining weights and a zero weight of multiplicity three. Identify the tensor product with endomorphisms of $\mathbb C^3$ under conjugation. Its scalar line is a singlet, while the traceless matrices give the irreducible adjoint octet, with two zero weights. The root [commutators](lie-algebra.md#commutator) connect all of the traceless matrix units, proving irreducibility rather than inferring it solely from a drawing.

### Conjugation representation

↑ **Parent:** [Group representation](#group-representation)

If $G$ acts on a vector space $W$, it acts on $\operatorname{End}(W)$ by conjugation:

$$
g\cdot X=\rho(g)X\rho(g)^{-1}.
$$

Under $\operatorname{End}(W)\cong W\otimes W^*$, this is the [tensor product of group representations](#tensor-product-of-group-representations) $W\otimes W^*$.

### Trivial representation

↑ **Parent:** [Group representation](#group-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trivial_representation)

The trivial representation sends every [group](group.md) element to the [identity operator](vector-space.md#identity-operator). A one-dimensional constant-coordinate line in a [permutation representation](#permutation-representation) is an example: relabelling positions leaves a uniform assignment unchanged. A trivial action on a higher-dimensional [vector space](vector-space.md) has many [invariant subspaces](#invariant-subspace) and is therefore not an [irreducible representation](#irreducible-representation).

#### Fully symmetric representation

↑ **Parent:** [Trivial representation](#trivial-representation)

The [trivial representation](#trivial-representation) of a molecular point group: every symmetry operation is represented by $1$. Labels such as $A_1$ or $A_{1g}$ depend on the group and its labelling convention.

#### Gauge singlet

↑ **Parent:** [Trivial representation](#trivial-representation)

A field is a [gauge singlet](#gauge-singlet) if it transforms in the [trivial representation](#trivial-representation) of the entire [gauge group](relativistic-quantum-field.md#gauge-group): every gauge transformation leaves it unchanged. A singlet of only one factor need not be a gauge singlet of the product group. For example a [right-handed neutrino](standard-model.md#right-handed-neutrino) with representation $(\mathbf1,\mathbf1)_0$ is a [Standard Model](standard-model.md) gauge singlet, whereas a color-singlet charged [lepton](standard-model.md#lepton) is still acted on by the electroweak group. A singlet can have ordinary derivatives in its [kinetic term](classical-field-theory.md#kinetic-term) and gauge-invariant masses, subject to [Lorentz invariance](special-relativity.md#lorentz-invariance) and any additional global symmetries.

#### Scalar representation

↑ **Parent:** [Trivial representation](#trivial-representation)

A scalar representation is the one-dimensional [trivial representation](#trivial-representation): every group element acts as the identity. Scalar polarization labels are unchanged by the relevant rotation group.

### Vector representation

↑ **Parent:** [Group representation](#group-representation)

The vector representation is the defining action of a matrix group on the vector space on which its matrices act. For an orthogonal or Lorentz group, it preserves the corresponding symmetric bilinear form.

### Matrix representation

↑ **Parent:** [Group representation](#group-representation)

A matrix representation is a [group representation](#group-representation) together with a basis, so each group element is represented by an invertible matrix and multiplication is represented by matrix multiplication.

### Invariant subspace

↑ **Parent:** [Group representation](#group-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Invariant_subspace)

An invariant subspace of a [linear map](vector-space.md#linear-map) $A:V\to V$ is a [vector subspace](vector-space.md#vector-subspace) $W\subseteq V$ satisfying $A(W)\subseteq W$. For a [group representation](#group-representation), invariance means $\rho(g)W\subseteq W$ for every represented group element $g$.

Invariance of a [vector subspace](vector-space.md#vector-subspace) does not mean that each individual [vector](vector-space.md#vector) stays fixed. The zero-sum plane in the three-coordinate example is invariant even though the cyclic permutation rotates its nonzero [vectors](vector-space.md#vector). By contrast, the constant-coordinate line is pointwise fixed. Distinguishing these statements prevents a symmetry-preserved mode space from being mistaken for a static mode.

#### Fixed-point subspace of a group action

↑ **Parent:** [Invariant subspace](#invariant-subspace)

For a linear [group representation](#group-representation), the common fixed vectors of a subgroup form an [invariant subspace](#invariant-subspace) for any [equivariant map](group-action.md#equivariant-map) restricted to it. Its dimension is central to symmetry-based branching theorems. It need not be invariant under the entire group; conjugate subgroups have conjugate fixed-point subspaces.

#### Reducible representation

↑ **Parent:** [Invariant subspace](#invariant-subspace)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reducible_representation)

A nonzero representation is reducible when it has a nonzero proper [invariant subspace](#invariant-subspace); otherwise it is an [irreducible representation](#irreducible-representation).

### Semisimple representation

↑ **Parent:** [Group representation](#group-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semisimple_representation)

A representation is semisimple when it is a [direct sum](vector-space.md#direct-sum) of [irreducible representations](#irreducible-representation). Equivalently, every invariant subspace has an invariant complement.

<h2 id="maschke-s-theorem">Maschke's theorem</h2>

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maschke's_theorem)

Every [group representation](#group-representation) of a [finite group](group.md#finite-group) over a [field](algebra.md#field) whose [characteristic](algebra.md#characteristic-of-a-field) does not divide the number of elements of the group is [semisimple](#semisimple-representation). Given an invariant subspace, averaging any projection onto it over the group produces an equivariant projection, whose kernel is an invariant complement.

## Modular representation theory

↑ **Parent:** [Representation theory](representation-theory.md)

[This section is present in another page, follow this link to view it.](modular-representation-theory.md)

## Complex representation

↑ **Parent:** [Representation theory](representation-theory.md)

A complex representation of a group $G$ is a homomorphism $\rho:G\to\operatorname{GL}(V)$ for a complex vector space $V$.

### Continuous representation of a topological group

↑ **Parent:** [Complex representation](#complex-representation)

A finite-dimensional continuous representation of a topological group is a continuous homomorphism $\rho:G\to\operatorname{GL}(V)$, where $V$ is a finite-dimensional complex vector space.

### Degree of a representation

↑ **Parent:** [Complex representation](#complex-representation)

The degree of a finite-dimensional representation $\rho:G\to\operatorname{GL}(V)$ is $\dim V$.

### Isomorphic representations

↑ **Parent:** [Complex representation](#complex-representation)

Representations $\rho:G\to\operatorname{GL}(V)$ and $\rho':G\to\operatorname{GL}(V')$ are isomorphic when an invertible linear map $T:V\to V'$ intertwines the actions: $T\rho(g)=\rho'(g)T$ for every $g\in G$.

### Nonsemisimple translation representation of the infinite cyclic group

↑ **Parent:** [Complex representation](#complex-representation)

On polynomials of degree at most one, let the generator of $\mathbb Z$ act by $p(x)\mapsto p(x+1)$. In the basis $(1,x)$ its matrix is

$$
\begin{pmatrix}1&1\\0&1\end{pmatrix}.
$$

This nontrivial [Jordan block](linear-operator-theory.md#jordan-block) is not diagonalizable, so the representation is not a direct sum of one-dimensional subrepresentations.

### Faithful representation

↑ **Parent:** [Complex representation](#complex-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Faithful_representation)

A representation is faithful when its kernel is trivial.

#### Regular representation

↑ **Parent:** [Faithful representation](#faithful-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regular_representation)

The left regular representation acts on the basis $(e_h)_{h\in G}$ by $\rho(g)e_h=e_{gh}$. It is faithful.

##### Four-point regular representation of the Klein four-group

↑ **Parent:** [Regular representation](#regular-representation)

The [permutation matrices](vector-space.md#permutation-matrix) of the three displayed double transpositions, together with $I_4$, form a [faithful representation](#faithful-representation) of the [Klein four-group](finite-group-theory.md#klein-four-group). They satisfy $P^2=Q^2=I_4$ and $PQ=QP$. Every nonidentity element fixes no basis vector, so this is its four-dimensional [regular representation](#regular-representation).

The constant vector $(1,1,1,1)^T$ spans a nonzero proper [invariant subspace](#invariant-subspace), proving reducibility. More completely, the columns of

$$
S=\frac12\begin{pmatrix}1&1&1&1\\1&1&-1&-1\\1&-1&1&-1\\1&-1&-1&1\end{pmatrix}
$$

form a common [orthonormal basis](inner-product.md#orthonormal-basis) of [eigenvectors](linear-operator-theory.md#eigenvector). Direct multiplication gives $S^TPS=\operatorname{diag}(1,1,-1,-1)$ and $S^TQS=\operatorname{diag}(1,-1,1,-1)$. Thus the representation splits into the four distinct real one-dimensional characters, each once. The basis change is a normalized [Hadamard matrix](vector-space.md#hadamard-matrix).

##### Sum of squares of irreducible degrees

↑ **Parent:** [Regular representation](#regular-representation)

If $\rho_1,\ldots,\rho_k$ are the complex irreducible representations of a finite group $G$ and $n_j=\dim\rho_j$, decomposition of the [regular representation](#regular-representation) gives

$$
\sum_{j=1}^k n_j^2=|G|.
$$

##### Faithful irreducible representation of a finite simple group

↑ **Parent:** [Regular representation](#regular-representation)

By [Maschke's theorem](#maschke-s-theorem), the complex regular representation of a finite group is a direct sum of irreducibles. Its kernel is the intersection of their kernels. If the group is simple, each kernel is either trivial or the whole group; faithfulness of the regular representation therefore forces at least one irreducible constituent to be faithful.

#### Spectrum orbit bound for a faithful symmetric-group representation

↑ **Parent:** [Faithful representation](#faithful-representation)

For a $p$-cycle $g\in S_p$, each $g^k$ with $1\leq k<p$ is conjugate to $g$. In a faithful complex representation, $\rho(g)$ has a nontrivial $p$th-root eigenvalue $\lambda$, and similarity of $\rho(g)$ and $\rho(g)^k$ puts all $p-1$ values $\lambda^k$ in its spectrum. Hence the representation has dimension at least $p-1$.

#### Finite-dimensional representation obstruction from elementary abelian subgroups

↑ **Parent:** [Faithful representation](#faithful-representation)

Commuting complex involutions are simultaneously diagonalizable, so $(C_2)^n$ can act faithfully in dimension $d$ only if $n\leq d$. A group containing $(C_2)^n$ for arbitrarily large $n$, such as the full permutation group of $\mathbb N$, has no faithful finite-dimensional complex representation.

#### Real Heisenberg quotient has no faithful finite-dimensional representation

↑ **Parent:** [Faithful representation](#faithful-representation)

Let $G$ be the real upper unitriangular three-by-three group, let $Z$ be its centre, and let $Z_0$ be the integer subgroup of $Z$. Every finite-dimensional continuous complex representation of $G/Z_0$ kills the central circle $Z/Z_0$, and hence is not faithful.

### One-dimensional representation kills the commutator subgroup

↑ **Parent:** [Complex representation](#complex-representation)

The image of a one-dimensional representation lies in the abelian group $\mathbb C^\times$, so its kernel contains the [commutator subgroup](group-theory.md#commutator-subgroup) of the represented group.

### Inflation of a group representation

↑ **Parent:** [Complex representation](#complex-representation)

Given a [quotient group](group-theory.md#quotient-group) map $\pi:G\to G/N$ and a representation $\rho$ of $G/N$, its inflation to $G$ is the representation $\rho\circ\pi$. Conversely, a representation of $G$ factors through $G/N$ exactly when its kernel contains $N$.

### Irreducible representation of a finite abelian group

↑ **Parent:** [Complex representation](#complex-representation)

Every irreducible complex representation of a [finite abelian group](group.md#finite-abelian-group) is one-dimensional. After making the representation unitary, the commuting representing matrices are simultaneously diagonalizable; any common eigenspace is invariant, so irreducibility leaves only one dimension.

#### Complex irreducible representations of a finite cyclic group

↑ **Parent:** [Irreducible representation of a finite abelian group](#irreducible-representation-of-a-finite-abelian-group)

For $C_n=\langle g:g^n=e\rangle$, the complex [irreducible representations](#irreducible-representation) are precisely the $n$ one-dimensional maps $g\mapsto e^{2\pi ij/n}$, with $0\leq j<n$. Their [characters](#character-of-a-representation) have the displayed values, forming the discrete Fourier character table. Indeed a representing matrix $A$ satisfies $A^n=I$. Applying the [fundamental theorem of algebra](algebra.md#fundamental-theorem-of-algebra) to its [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) gives an [eigenvalue](linear-operator-theory.md#eigenvalue) and an [eigenvector](linear-operator-theory.md#eigenvector) over the [complex numbers](complex-analysis.md#complex-number). Its line is an [invariant subspace](#invariant-subspace) under every power of $A$; irreducibility therefore forces the entire space to be that line. Its [eigenvalue](linear-operator-theory.md#eigenvalue) is an $n$th [root of unity](algebra.md#root-of-unity). Different roots give inequivalent one-dimensional representations, and there are exactly $n$ possibilities.

All [conjugacy classes](group-action.md#conjugacy-class) are singletons because the [group](group.md) is [Abelian](group.md#abelian-group). The number of the displayed irreducibles equals the group order, and their squared dimensions sum to $n$, in agreement with the [sum of squares of irreducible representation dimensions](#sum-of-squares-of-irreducible-representation-dimensions). Over the real numbers, conjugate nonreal characters instead combine into the planes described by the [irreducible real representations of a finite cyclic group](#irreducible-real-representations-of-a-finite-cyclic-group).

## Real representation

↑ **Parent:** [Representation theory](representation-theory.md)

A real representation of a group $G$ is a homomorphism $G\to\operatorname{GL}(V)$ for a real vector space $V$.

### Realification of a complex representation

↑ **Parent:** [Real representation](#real-representation)

A complex [group representation](#group-representation) $\rho:G\to\operatorname{GL}(n,\mathbb C)$ defines a real representation on $\mathbb R^{2n}$ by viewing each complex coordinate as its real and imaginary parts. In grouped coordinates its matrices are the [realification of a complex matrix](vector-space.md#realification-of-a-complex-matrix) shown in the title. Direct block multiplication gives $\mathcal R(AB)=\mathcal R(A)\mathcal R(B)$ and $\mathcal R(I_n)=I_{2n}$, proving the representation property and preservation of invertibility.

Taking the [trace](linear-algebra.md#matrix-trace) gives its [character](#character-of-a-representation) $\chi_\mathbb R(g)=2\operatorname{Re}\chi_\mathbb C(g)$. After [complexification of a real vector space](vector-space.md#complexification-of-a-real-vector-space), this realification splits as the original representation and its conjugate. Realification need not preserve irreducibility: the answer depends on whether the irreducible complex representation has real, complex or [quaternionic representation](#pseudoreal-representation) type. The standard two-dimensional complex representation of the [quaternion group](finite-group-theory.md#quaternion-group) gives a four-dimensional real example with character four at the identity, minus four at its central negative identity, and zero at the other six elements.

### Irreducible real representations of a finite cyclic group

↑ **Parent:** [Real representation](#real-representation)

For $C_n=\langle g\rangle$, the irreducible real representations are the trivial line, the sign line $g\mapsto-1$ when $n$ is even, and the pairwise nonisomorphic real planes on which $g$ rotates through $2\pi k/n$ for $1\leq k<n/2$.

### Real regular representation of a finite cyclic group

↑ **Parent:** [Real representation](#real-representation)

The real regular representation of $C_n$ is the direct sum of the [irreducible real representations of a finite cyclic group](#irreducible-real-representations-of-a-finite-cyclic-group), each once. A real Fourier basis consists of the constant vector, the alternating vector when $n$ is even, and cosine-sine pairs for frequencies $1\leq k<n/2$.

<h2 id="representation-theory-of-su-2">Representation theory of SU(2)</h2>

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Representation_theory_of_SU(2))

Finite-dimensional complex representations of $SU_2$ are completely reducible, and their irreducibles are indexed by nonnegative integers.

<h3 id="conjugate-fundamental-spinor-of-su-2">Conjugate fundamental spinor of SU(2)</h3>

↑ **Parent:** [Representation theory of SU(2)](#representation-theory-of-su-2)

For the defining [SU(2)](topological-group.md#su-2-group) action $\eta'=A\eta$, the conjugate row $\bar\eta_\alpha=(\eta^\alpha)^*$ transforms by $A^\dagger=A^{-1}$. Thus $\bar\eta_\alpha\eta^\alpha$ is invariant. The alternating [invariant tensor](#invariant-tensor) $\epsilon_{12}=1$ satisfies $A^T\epsilon A=\epsilon$. Choose its inverse $\epsilon^{12}=-1$; then $\epsilon^{\alpha\gamma}\epsilon_{\gamma\beta}=\delta^\alpha{}_\beta$. Raising the conjugate index, $\widetilde\eta^\alpha=\epsilon^{\alpha\beta}\bar\eta_\beta$, gives another defining spinor. The resulting antilinear intertwiner squares to $-I$, so the defining representation is a [pseudoreal representation](#pseudoreal-representation).

### Homogeneous polynomial representation of SU2

↑ **Parent:** [Representation theory of SU(2)](#representation-theory-of-su-2)

The irreducible representation $V_n=\operatorname{Sym}^n(\mathbb C^2)$ consists of homogeneous degree-$n$ polynomials in two variables, with the action induced from the standard two-dimensional representation. It has dimension $n+1$.

#### Character of the homogeneous polynomial representation of SU2

↑ **Parent:** [Homogeneous polynomial representation of SU2](#homogeneous-polynomial-representation-of-su2)

If $g\in SU_2$ has eigenvalues $z,z^{-1}$, then

$$
\chi_{V_n}(g)=z^n+z^{n-2}+\cdots+z^{-n}.
$$

### Classification of finite-dimensional representations of SU2

↑ **Parent:** [Representation theory of SU(2)](#representation-theory-of-su-2)

Every finite-dimensional complex $SU_2$-representation is a direct sum of the pairwise nonisomorphic irreducibles $V_n=\operatorname{Sym}^n(\mathbb C^2)$.

### Self-duality of finite-dimensional SU2 representations

↑ **Parent:** [Representation theory of SU(2)](#representation-theory-of-su-2)

The standard invariant alternating form identifies $V_1$ with its dual. Its symmetric powers identify every $V_n$ with $V_n^*$, and complete reducibility then gives $V\cong V^*$ for every finite-dimensional complex $SU_2$-representation.

### Central parity on SU2 tensor products

↑ **Parent:** [Representation theory of SU(2)](#representation-theory-of-su-2)

On $V_n$, the central element $-I$ acts as $(-1)^n$. It therefore acts trivially on $V_n\otimes V_n$, although it need not act trivially on the tensor square of a representation containing irreducibles of both parities.

### Clebsch-Gordan coefficients

↑ **Parent:** [Representation theory of SU(2)](#representation-theory-of-su-2)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Clebsch–Gordan_coefficients)

Clebsch-Gordan coefficients are the change-of-basis coefficients between an uncoupled tensor-product basis and a basis adapted to the irreducible decomposition of the tensor product.

#### Ladder recurrence for Clebsch-Gordan coefficients

↑ **Parent:** [Clebsch-Gordan coefficients](#clebsch-gordan-coefficients)

Apply a total [ladder operator](semisimple-lie-algebra.md#ladder-operator) to a coupled state and evaluate against an uncoupled product state. The total operator is the sum of the two factor operators, so its one coupled ladder amplitude times the corresponding one of the [Clebsch-Gordan coefficients](#clebsch-gordan-coefficients) equals the sum of two factor ladder amplitudes times shifted coefficients. An overall common rescaling of the ladder operators cancels from the recurrence. Nonzero coefficients obey $m_1+m_2=m$, and the positive ladder amplitudes require a consistent phase convention within each irreducible summand.

// Target: lie-theory.bigb

#### 3-j symbol

↑ **Parent:** [Clebsch-Gordan coefficients](#clebsch-gordan-coefficients)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/3-j_symbol)

A symmetrized form of the [Clebsch-Gordan coefficients](#clebsch-gordan-coefficients) used for coupling three angular momenta. The relation is $\langle j_1m_1,j_2m_2|j_3m_3\rangle=(-1)^{j_1-j_2+m_3}\sqrt{2j_3+1}\begin{pmatrix}j_1&j_2&j_3\\m_1&m_2&-m_3\end{pmatrix}$. The symbol vanishes unless the magnetic indices sum to zero and the angular momenta obey the triangle and integrality conditions. Products of two such symbols express the [Gaunt integral](analysis.md#gaunt-integral); the zero-magnetic-index symbol enforces even total multipole for integer spherical harmonics.

#### Clebsch-Gordan decomposition for SU2

↑ **Parent:** [Clebsch-Gordan coefficients](#clebsch-gordan-coefficients)

For $m,n\geq0$,

$$
V_m\otimes V_n\cong
\bigoplus_{j=0}^{\min(m,n)}V_{m+n-2j}.
$$

The identity follows by multiplying the weight characters and comparing their nested weight strings.

##### Tensor contractions in the SU2 Clebsch-Gordan decomposition

↑ **Parent:** [Clebsch-Gordan decomposition for SU2](#clebsch-gordan-decomposition-for-su2)

Realize $V_n=\operatorname{Sym}^n\mathbb C^2$. Contract $r$ pairs of indices, one from each [symmetric tensor](multilinear-algebra.md#symmetric-tensor), with the alternating [invariant tensor](#invariant-tensor) $\epsilon$, and symmetrize the remaining indices. This is a nonzero [intertwining operator](#intertwining-operator) into $V_{m+n-2r}$. In the bihomogeneous polynomial realization, $(z_1w_2-z_2w_1)^rz_1^{m-r}w_1^{n-r}$ is a [highest-weight vector](semisimple-lie-algebra.md#highest-weight-vector) of weight $m+n-2r$. Its lowering string has length $m+n-2r+1$. These inequivalent irreducible summands exhaust the tensor product, since their dimensions sum to $(m+1)(n+1)$.

<h6 id="decomposition-of-three-su-2-spinors">Decomposition of three SU(2) spinors</h6>

↑ **Parent:** [Tensor contractions in the SU2 Clebsch-Gordan decomposition](#tensor-contractions-in-the-su2-clebsch-gordan-decomposition)

For $Q^{\alpha\beta\gamma}$, put $S=Q^{(\alpha\beta\gamma)}$, $d_1^\alpha=\epsilon_{\beta\gamma}Q^{\alpha\beta\gamma}$, $d_2^\alpha=\epsilon_{\beta\gamma}Q^{\beta\alpha\gamma}$ and $d_3^\alpha=\epsilon_{\beta\gamma}Q^{\beta\gamma\alpha}$. With $\epsilon_{12}=1$ and inverse $\epsilon^{12}=-1$, the two-dimensional alternating identity gives $d_1-d_2+d_3=0$. The inverse decomposition is $Q^{\alpha\beta\gamma}=S^{\alpha\beta\gamma}+\epsilon^{\alpha\beta}(2d_1^\gamma-d_2^\gamma)/3-\epsilon^{\alpha\gamma}(d_1^\beta+d_2^\beta)/3$. The symmetric part is the spin-$3/2$ [SU(2) representation](#representation-theory-of-su-2), and the two independent contractions are spin-$1/2$ representations. This is the spin coupling underlying ground-state three-quark [baryons](physics.md#baryon), before the [Pauli constraint on three-quark flavour multiplets](physics.md#pauli-constraint-on-three-quark-flavour-multiplets) is imposed.

// Target: quantum-field-theory.bigb

##### Flip parity in the SU2 tensor square

↑ **Parent:** [Clebsch-Gordan decomposition for SU2](#clebsch-gordan-decomposition-for-su2)

On the multiplicity-one summand $V_{2n-2j}\subset V_n\otimes V_n$, interchange of tensor factors acts by $(-1)^j$. A highest-weight vector exhibiting the sign is

$$
\sum_{k=0}^j(-1)^k\binom jk
x^{n-k}y^k\otimes x^{n-j+k}y^{j-k}.
$$

###### Exterior square of an SU2 irreducible representation

↑ **Parent:** [Flip parity in the SU2 tensor square](#flip-parity-in-the-su2-tensor-square)

The odd-parity summands give

$$
\bigwedge^2V_n\cong
\bigoplus_{k=0}^{\lfloor(n-1)/2\rfloor}V_{2n-4k-2}.
$$

###### Second and third exterior powers of V4 of SU2

↑ **Parent:** [Exterior square of an SU2 irreducible representation](#exterior-square-of-an-su2-irreducible-representation)

The alternating summands in the tensor square give $\bigwedge^2V_4\cong V_6\oplus V_2$. Since $V_4$ is self-dual and has trivial determinant,

$$
\bigwedge^3V_4\cong(\bigwedge^2V_4)^*\otimes\det V_4
\cong V_6\oplus V_2.
$$

## Character of an exterior square

↑ **Parent:** [Representation theory](representation-theory.md)

For any finite-dimensional complex representation,

$$
\chi_{\wedge^2V}(g)=
\frac{\chi_V(g)^2-\chi_V(g^2)}2.
$$

## Character of an exterior cube

↑ **Parent:** [Representation theory](representation-theory.md)

Newton's identities applied to the eigenvalues of $g$ give

$$
\chi_{\wedge^3V}(g)
=\frac{\chi_V(g)^3-3\chi_V(g)\chi_V(g^2)+2\chi_V(g^3)}6.
$$

## Averaging over a finite group

↑ **Parent:** [Representation theory](representation-theory.md)

Averaging any object over a finite group, $|G|^{-1}\sum_{g\in G}g\cdot x$, produces a group-invariant object whenever the relevant operations are linear.

## Unitary representation

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unitary_representation)

A complex representation is unitary when every representing matrix preserves a positive-definite Hermitian inner product.

### Triviality of finite-dimensional unitary representations of SL2R

↑ **Parent:** [Unitary representation](#unitary-representation)

The diagonal element $\operatorname{diag}(m,m^{-1})$ conjugates $U(t)$ to $U(m^2t)=U(t)^{m^2}$. In a finite-dimensional [unitary representation](#unitary-representation), conjugacy therefore makes its eigenvalue multiset invariant under every square power. [Square-power rigidity of a finite nonzero spectrum](algebra.md#square-power-rigidity-of-a-finite-nonzero-spectrum) makes the image of every upper unipotent the identity. Its kernel is a [normal subgroup](group-theory.md#normal-subgroup); [elementary unipotent generators of SL2R](group-theory.md#elementary-unipotent-generators-of-sl2r) then force the entire [group representation](#group-representation) to be trivial. This algebraic argument does not require continuity.

### Integrated unitary representation

↑ **Parent:** [Unitary representation](#unitary-representation)

For a strongly continuous [unitary representation](#unitary-representation), integration against $f\in L^1(G)$ defines an operator satisfying $\|\pi(f)\|\le\|f\|_1$. [Fubini's theorem](measure-theory.md#fubini-s-theorem) gives $\pi(f*g)=\pi(f)\pi(g)$, and the group-algebra involution gives $\pi(f^*)=\pi(f)^*$. On an Abelian group, the operator-norm closure is a commutative [C-star algebra](banach-algebra.md#c-star-algebra). Its [algebra characters](banach-algebra.md#character-of-an-algebra) produce continuous unitary [group characters](topological-group.md#continuous-unitary-character), allowing the [Commutative Gelfand--Naimark theorem](banach-algebra.md#commutative-gelfand-naimark-theorem) and [Riesz-Markov-Kakutani representation theorem](functional-analysis.md#riesz-markov-kakutani-representation-theorem) to turn a positive vector functional into a finite spectral measure.

### Positive energy unitary representation of the circle

↑ **Parent:** [Unitary representation](#unitary-representation)

A strongly continuous [unitary representation](#unitary-representation) of the circle has integer spectral weights: $H$ is the orthogonal sum of spaces on which $U_z=z^m$. Positive energy means that these weights are bounded below, equivalently its self-adjoint generator has spectrum bounded below. Multiplication by an integer character shifts the lower bound to zero. A unitary operator with a nonzero rotation weight cannot exist in its operator algebra: repeated application of it or its inverse would move a nonzero vector to arbitrarily low energy.

### Stone theorem for the circle group

↑ **Parent:** [Unitary representation](#unitary-representation)

A strongly continuous [unitary representation](#unitary-representation) of the [circle group](lie-theory.md#circle-group) splits as an orthogonal sum of character subspaces. The [projections](vector-space.md#projection-linear-algebra) are $P_n=\int_{\mathbb T}z^{-n}U_z\,dz$. Character [orthogonality](inner-product.md#orthogonal-vectors) makes them mutually orthogonal, and [Fejér sum](fourier-series.md#fejer-sum) shows their ranges span the represented [Hilbert space](hilbert-space.md). The [self-adjoint](linear-operator-theory.md#self-adjoint-operator) generator has integer [eigenvalues](linear-operator-theory.md#eigenvalue), with domain given by $\sum_n n^2\|P_n\xi\|^2<\infty$.

### Peter-Weyl theorem

↑ **Parent:** [Unitary representation](#unitary-representation)

For a [compact group](topological-group.md#compact-group), the matrix coefficients of its finite-dimensional irreducible [unitary representations](#unitary-representation) span a dense subspace of $C(G)$ and form a complete orthogonal decomposition of $L^2(G)$ with [Haar measure](measure.md#haar-measure). If $K$ is a closed subgroup and $W$ is a finite-dimensional unitary $K$-representation, the space of L2 sections of the associated homogeneous bundle has multiplicity $\dim\operatorname{Hom}_K(E|_K,W)$ for each irreducible $G$-representation $E$. This is the compact-group form of Frobenius reciprocity and determines homogeneous-bundle multiplicities from isotropy weights.

#### Finite faithful representation from point-separating representations

↑ **Parent:** [Peter-Weyl theorem](#peter-weyl-theorem)

Suppose finite-dimensional [continuous](calculus.md#continuous-function) [group representations](#group-representation) separate points of a [compact Lie group](lie-theory.md#compact-lie-group). Choose an identity neighborhood $U$ containing no nontrivial subgroup, using [Lie groups have no small subgroups](lie-theory.md#lie-groups-have-no-small-subgroups). For each $g\notin U$, choose a representation whose matrix at $g$ is not the identity. The corresponding open nonidentity sets cover the compact complement of $U$, so finitely many representations suffice there. Their [direct sum](vector-space.md#direct-sum) has kernel inside $U$ and therefore trivial kernel. [Unitarization of a compact-group representation](#unitarization-of-a-compact-group-representation) makes it a finite-dimensional faithful [unitary representation](#unitary-representation).

#### Convolution proof of uniform Peter-Weyl approximation

↑ **Parent:** [Peter-Weyl theorem](#peter-weyl-theorem)

A continuous symmetric approximate identity on a [compact group](topological-group.md#compact-group) gives a compact self-adjoint [convolution](fourier-analysis.md#convolution) operator $T$ on $L^2(G)$ which maps into $C(G)$ and commutes with [left translations](lie-theory.md#left-and-right-translation-on-a-lie-group). Its nonzero [eigenspaces](linear-operator-theory.md#eigenspace) are finite-dimensional invariant spaces of [continuous functions](calculus.md#continuous-function), hence consist of [matrix coefficients](#matrix-coefficient) of finite-dimensional [unitary representations](#unitary-representation). If $S_N$ projects onto increasing finite sums of these [eigenspaces](linear-operator-theory.md#eigenspace), $S_NTf\to Tf$ in $L^2$, and the bound $\|Th\|_\infty\leq\|k\|_2\|h\|_2$ gives $TS_NTf\to T^2f$ uniformly. Choosing the approximate identity narrow makes $T^2f$ uniformly close to $f$. This supplies uniform approximation without confusing an $L^2$ limit with a uniform limit.

#### Frobenius reciprocity for compact groups

↑ **Parent:** [Peter-Weyl theorem](#peter-weyl-theorem)

For a [compact group](topological-group.md#compact-group) $G$, closed subgroup $K$ and finite-dimensional unitary $K$-representation $W$, induced sections are functions satisfying $f(gk)=k^{-1}f(g)$. A $K$-intertwiner $\phi:E\to W$ produces the $G$-intertwiner $v\mapsto(g\mapsto\phi(g^{-1}v))$. Evaluation at the identity reverses this construction on each finite-dimensional continuous representation summand. Thus the multiplicity of an irreducible $E$ in the induced section space is $\dim\operatorname{Hom}_K(E|_K,W)$.

### Unitary irreducible representation

↑ **Parent:** [Unitary representation](#unitary-representation)

A unitary irreducible representation is both [unitary](#unitary-representation) and [irreducible](#irreducible-representation). Such representations are the building blocks in the harmonic analysis of groups and in quantum symmetry classifications.

### Unitarization of a finite-group representation

↑ **Parent:** [Unitary representation](#unitary-representation)

Average a positive-definite Hermitian form over a finite group and choose an orthonormal basis for the averaged form. In that basis every representing matrix is unitary.

### Unitarization of a compact-group representation

↑ **Parent:** [Unitary representation](#unitary-representation)

For a compact group with normalized [Haar measure](measure.md#haar-measure), averaging any positive-definite Hermitian form,

$$
\langle v,w\rangle_G
=\int_G\langle\rho(g)v,\rho(g)w\rangle\,dg,
$$

produces an invariant positive-definite Hermitian form.

#### Complete reducibility of compact-group representations

↑ **Parent:** [Unitarization of a compact-group representation](#unitarization-of-a-compact-group-representation)

A finite-dimensional [complex representation](#complex-representation) of a [compact group](topological-group.md#compact-group) is a [direct sum](vector-space.md#direct-sum) of [irreducible representations](#irreducible-representation). Average a positive [Hermitian inner product](linear-algebra.md#hermitian-inner-product) over normalized [Haar measure](measure.md#haar-measure). The [orthogonal complement](hilbert-space.md#orthogonal-complement) of an [invariant subspace](#invariant-subspace) is then invariant, so induction on [dimension](vector-space.md#dimension-vector-space) gives the decomposition. The same argument works for finite-dimensional [real representations](#real-representation) with a positive real [inner product](inner-product.md).

#### Orthogonalization of a compact-group representation

↑ **Parent:** [Unitarization of a compact-group representation](#unitarization-of-a-compact-group-representation)

For a continuous real representation $\rho:G\to GL(V)$ of a compact group, average any positive-definite real inner product against normalized [Haar measure](measure.md#haar-measure):

$$
(v,w)_G=\int_G(\rho(g)v,\rho(g)w)\,dg.
$$

The result is positive definite and $G$-invariant. An orthonormal basis for it conjugates the representation into an [orthogonal group](linear-algebra.md#orthogonal-group).

### Representation of the circle group

↑ **Parent:** [Unitary representation](#unitary-representation)

Every finite-dimensional continuous complex representation of $S^1$ is unitary and decomposes into one-dimensional weight spaces. Its continuous one-dimensional characters are $z\mapsto z^m$ for $m\in\mathbb Z$.

#### Central circle weight-space decomposition

↑ **Parent:** [Representation of the circle group](#representation-of-the-circle-group)

If a central subgroup is isomorphic to $S^1$, its weight spaces are invariant under the entire group, because every representing operator commutes with the central circle action.

## Class function

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Class_function)

A class function on a [group](group.md) is a function constant on every [conjugacy class](group-action.md#conjugacy-class). Equivalently, $f(hgh^{-1})=f(g)$ for all group elements $g,h$.

### Conjugation averaging on a compact group

↑ **Parent:** [Class function](#class-function)

Normalized [Haar measure](measure.md#haar-measure) makes this averaging a norm-one projection onto continuous [class functions](#class-function). Averaging a [trace](linear-algebra.md#matrix-trace) coefficient replaces its coefficient [endomorphism](algebra.md#endomorphism) by $\int\theta(h)^{-1}\alpha\theta(h)\,dh$. On an irreducible summand this average is $(\operatorname{tr}\alpha/\dim V)I$ by [Schur lemma](#schur-s-lemma). It follows that averaging finite-dimensional [matrix coefficients](#matrix-coefficient) yields finite linear combinations of [irreducible characters](#irreducible-character). Together with the [Peter-Weyl theorem](#peter-weyl-theorem), this proves uniform density of those characters among continuous [class functions](#class-function).

## Character orthogonality

↑ **Parent:** [Representation theory](representation-theory.md)

Irreducible characters are orthonormal for $\langle\chi,\psi\rangle=|G|^{-1}\sum_g\chi(g)\overline{\psi(g)}$, and $\sum_\chi\chi(1)^2=|G|$.

### Irreducible characters separate conjugacy classes

↑ **Parent:** [Character orthogonality](#character-orthogonality)

The [irreducible characters](#irreducible-character) of a [finite group](group.md#finite-group) form a basis of its complex [class functions](#class-function). Equality of every irreducible character value therefore forces equality of every class-function value, including indicators of [conjugacy classes](group-action.md#conjugacy-class), and hence conjugacy. The converse follows from the class-function property.

### Character expansion of the identity delta

↑ **Parent:** [Character orthogonality](#character-orthogonality)

For a [finite group](group.md#finite-group), the [regular representation](#regular-representation) contains $d_\rho$ copies of each [irreducible representation](#irreducible-representation) $\rho$. Its [character of a representation](#character-of-a-representation) is $|G|$ at the identity and zero elsewhere. Thus $\sum_\rho d_\rho\chi_\rho(x)=|G|1_{\{x=e\}}$, including the [trivial representation](#trivial-representation). This formula converts independent uniform [expectations](expected-value.md) into constrained configuration counts.

### Row orthogonality relations for a character table

↑ **Parent:** [Character orthogonality](#character-orthogonality)

For irreducible complex characters $\chi,\psi$ of a finite group,

$$
\sum_{g\in G}\chi(g)\overline{\psi(g)}
=|G|\delta_{\chi\psi}.
$$

Equivalently, summing over conjugacy classes $C$ with representatives $c$ gives

$$
\sum_C|C|\chi(c)\overline{\psi(c)}
=|G|\delta_{\chi\psi}.
$$

### Central character value of a conjugacy-class sum

↑ **Parent:** [Character orthogonality](#character-orthogonality)

For an irreducible character $\chi$ and a conjugacy class $C$ represented by $c$, the central group-algebra element $\sum_{x\in C}x$ acts as the scalar

$$
\omega_\chi(C)=\frac{|C|\chi(c)}{\chi(1)}.
$$

This scalar is an [algebraic integer](algebraic-number-theory.md#algebraic-integer), since the class sum acts by an integer matrix on the regular representation.

#### Irreducible character degree divides the group order

↑ **Parent:** [Central character value of a conjugacy-class sum](#central-character-value-of-a-conjugacy-class-sum)

For every irreducible complex character $\chi$ of a finite group $G$,

$$
\chi(1)\mid|G|.
$$

Indeed, row orthogonality expresses $|G|/\chi(1)$ as a sum of products of [algebraic integers](algebraic-number-theory.md#algebraic-integer):

$$
\frac{|G|}{\chi(1)}
=\sum_C\frac{|C|\chi(c)}{\chi(1)}
\overline{\chi(c)}.
$$

It is a rational algebraic integer and therefore an integer.

##### No finite simple group has an irreducible character of degree two

↑ **Parent:** [Irreducible character degree divides the group order](#irreducible-character-degree-divides-the-group-order)

A degree-two irreducible representation of a nonabelian finite simple group would be faithful. Its determinant is a linear character and hence trivial, so its image lies in $\operatorname{SL}_2(\mathbb C)$. Degree divisibility makes the group order even; an involution must map to the unique nonidentity involution $-I$ in $\operatorname{SL}_2(\mathbb C)$ and would therefore be central, a contradiction.

##### Irreducible character degrees of a group of order two p

↑ **Parent:** [Irreducible character degree divides the group order](#irreducible-character-degree-divides-the-group-order)

For a prime $p$, either a group of order $2p$ is abelian and all irreducible character degrees are one, or $p$ is odd and its degrees are

$$
1,1,\underbrace{2,\ldots,2}_{(p-1)/2}.
$$

##### Irreducible characters of a nonabelian group of order p q

↑ **Parent:** [Irreducible character degree divides the group order](#irreducible-character-degree-divides-the-group-order)

If $p>q$ are prime and $G$ is nonabelian of order $pq$, then it has $q$ linear characters and $(p-1)/q$ irreducible characters of degree $q$. It consequently has

$$
q+\frac{p-1}{q}
$$

conjugacy classes.

### Character inner product

↑ **Parent:** [Character orthogonality](#character-orthogonality)

For complex [class functions](#class-function) on a [finite group](group.md#finite-group) $G$, the character inner product is

$$
\langle\chi,\psi\rangle_G
=\frac1{|G|}\sum_{g\in G}\chi(g)\overline{\psi(g)}.
$$

If $\psi$ is [irreducible](#irreducible-character), this inner product is its multiplicity in the representation with character $\chi$.

## Character table

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Character_table)

The character table of a finite group lists its irreducible complex characters on its conjugacy classes. The number of rows equals the number of conjugacy classes, and the squared row degrees sum to the group order.

### Integral character reconstruction from column orthogonality

↑ **Parent:** [Character table](#character-table)

Column orthogonality and the regular character give quadratic and linear equations for missing character values once their degrees are known. These equations can admit spurious rational solutions. Every character value is an algebraic integer, so a rational candidate must be an ordinary integer. Applying this extra condition can remove ambiguities that orthogonality alone leaves.

### Irreducible representations of G6n

↑ **Parent:** [Character table](#character-table)

For

$$
G_{6n}=\langle a,b:a^{2n}=b^3=1,\ a^{-1}ba=b^{-1}\rangle,
$$

there are $2n$ [linear characters](#linear-character), given by $a\mapsto\xi^j$, $b\mapsto1$ for a primitive $(2n)$th [root of unity](algebra.md#root-of-unity) $\xi$, and $n$ two-dimensional irreducible representations

$$
a\mapsto\begin{pmatrix}0&\xi^k\\\xi^k&0\end{pmatrix},
\qquad
b\mapsto\begin{pmatrix}\omega&0\\0&\omega^2\end{pmatrix},
\qquad 0\leq k<n,
$$

where $\omega^3=1$ and $\omega\ne1$. The two-dimensional representations parametrized by $\varepsilon$ and $-\varepsilon$ are isomorphic. The [sum of squares of irreducible degrees](#sum-of-squares-of-irreducible-degrees) is $2n+4n=6n$, so this list is complete.

#### Character table of G6n

↑ **Parent:** [Irreducible representations of G6n](#irreducible-representations-of-g6n)

The conjugacy classes of $G_{6n}$ are

$$
C_r=\{a^{2r}\},\qquad
D_r=\{a^{2r}b,a^{2r}b^2\},\qquad
E_r=\{a^{2r+1},a^{2r+1}b,a^{2r+1}b^2\},
$$

for $0\leq r<n$. With $0\leq j<2n$ and $0\leq k<n$, the linear character $\lambda_j$ and two-dimensional character $\chi_k$ have values

$$
\begin{array}{c|ccc}
&C_r&D_r&E_r\\ \hline
\lambda_j&\xi^{2jr}&\xi^{2jr}&\xi^{j(2r+1)}\\
\chi_k&2\xi^{2kr}&-\xi^{2kr}&0.
\end{array}
$$

### Irreducible character degree

↑ **Parent:** [Character table](#character-table)

The degree of an irreducible character $\chi$ is $\chi(1)$, the dimension of the corresponding irreducible representation.

#### Irreducible characters of degree coprime to p

↑ **Parent:** [Irreducible character degree](#irreducible-character-degree)

For a [finite group](group.md#finite-group) $G$ and [prime number](prime-number.md) $p$, the notation

$$
\operatorname{Irr}_{p'}(G)=\{\chi\in\operatorname{Irr}(G):p\nmid\chi(1)\}
$$

denotes the [irreducible characters](#irreducible-character) whose [irreducible character degree](#irreducible-character-degree) is coprime to $p$.

#### Linear character

↑ **Parent:** [Irreducible character degree](#irreducible-character-degree)

A linear character is the character of a one-dimensional representation and therefore has degree one.

##### Trivial character

↑ **Parent:** [Linear character](#linear-character)

The trivial character takes the value $1$ on every group element and is afforded by the one-dimensional [trivial representation](#trivial-representation).

#### Nonlinear irreducible character

↑ **Parent:** [Irreducible character degree](#irreducible-character-degree)

A nonlinear irreducible character has degree greater than one.

## Character theory

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Character_theory)

Character theory studies representations through the traces of the representing linear transformations.

<h3 id="brauer-s-permutation-lemma">Brauer's permutation lemma</h3>

↑ **Parent:** [Character theory](#character-theory)

A group of [automorphisms](algebra.md#automorphism) of a [finite group](group.md#finite-group) permutes both its [conjugacy classes](group-action.md#conjugacy-class) and its [irreducible characters](#irreducible-character). The two [permutation representations](#permutation-representation) have the same [character](#character-of-a-representation): each automorphism fixes equally many conjugacy classes and irreducible characters. The invertible [character table](#character-table) intertwines the two permutation matrices, which have equal traces. The claim concerns fixed classes, not merely fixed elements.

### Artin induction

↑ **Parent:** [Character theory](#character-theory)

Every complex [character of a representation](#character-of-a-representation) of a [finite group](group.md#finite-group) $G$ is a rational linear combination of [characters](#character-of-a-representation) of [induced representations](#induced-representation) from one-dimensional [group representations](#group-representation) of [cyclic subgroups](group.md#cyclic-subgroup) $C_j$. One-dimensionality follows because the [irreducible representations](#irreducible-representation) of a finite [cyclic group](group.md#cyclic-group) over the complex numbers are one-dimensional. The rational coefficients distinguish this statement from [Brauer induction](#brauer-induction), which permits integer coefficients by allowing more general subgroups. For a rational-valued [character](#character-of-a-representation), another form of Artin induction uses rational combinations of [induced representations](#induced-representation) of trivial [group representations](#group-representation) of [cyclic subgroups](group.md#cyclic-subgroup).

### Brauer induction

↑ **Parent:** [Character theory](#character-theory)

Every complex [character of a representation](#character-of-a-representation) of a [finite group](group.md#finite-group) $G$ is an integer linear combination of [characters](#character-of-a-representation) of [induced representations](#induced-representation) from one-dimensional [group representations](#group-representation) of subgroups $H_j\leq G$. Negative coefficients are allowed. Unlike [Artin induction](#artin-induction), the subgroups need not be [cyclic groups](group.md#cyclic-group). Applied to an [Artin L-function](algebraic-number-theory.md#artin-l-function), compatibility with [induced representations](#induced-representation) turns this character identity into a product of one-dimensional [Artin L-functions](algebraic-number-theory.md#artin-l-function) with integer exponents, reducing the behavior at $s=1$ to abelian extensions.

### Character of a representation

↑ **Parent:** [Character theory](#character-theory)

The character of a finite-dimensional representation $\rho$ is the class function $\chi_\rho(g)=\operatorname{tr}(\rho(g))$. Isomorphic representations have the same character.

#### Character of a localized orbital basis

↑ **Parent:** [Character of a representation](#character-of-a-representation)

A [symmetry transformation](group-action.md#symmetry-transformation) acts on localized [atomic orbitals](chemistry.md#atomic-orbital) both by moving their centres and by transforming their angular shapes. Only centres left in place can contribute to the [trace](linear-algebra.md#matrix-trace) of the corresponding [group representation](#group-representation). At each fixed centre, sum the diagonal coefficients of the orbital transformation: a reversed [p orbital](chemistry.md#p-orbital) contributes $-1$, whereas a fixed [s orbital](chemistry.md#s-orbital) contributes $+1$. For Cartesian displacement vectors at a fixed atom, use the [trace](linear-algebra.md#matrix-trace) of the full polar-vector [matrix](vector-space.md#matrix), not merely the number of fixed components. This rule generates [characters of a representation](#character-of-a-representation) without writing its entire [matrix](vector-space.md#matrix).

#### Ordinary character

↑ **Parent:** [Character of a representation](#character-of-a-representation)

An [ordinary character](#ordinary-character) is the [trace](linear-algebra.md#matrix-trace) [character](#character-of-a-representation) of a finite-dimensional [group representation](#group-representation) in [characteristic](algebra.md#characteristic-of-a-field) zero, usually realized over the complex numbers. It contrasts with a Brauer [character](#character-of-a-representation) in positive [characteristic](algebra.md#characteristic-of-a-field), which lifts eigenvalues on p-regular elements to characteristic-zero roots of unity.

#### Determinant character

↑ **Parent:** [Character of a representation](#character-of-a-representation)

For a [group representation](#group-representation) $\rho$ with character $\theta$, its determinant character sends $g$ to $\det\rho(g)$. Multiplicativity makes it a [linear character](#linear-character), independent of the equivalent matrix realization of $\rho$.

##### Central commutator has no torsion from an abelian Sylow subgroup

↑ **Parent:** [Determinant character](#determinant-character)

If a [Sylow p-subgroup](finite-group-theory.md#sylow-subgroup) $P$ is abelian, a hypothetical central subgroup $Q\leq G'$ of order $p$ has a nontrivial linear character extending to $P$. Inducing this extension to $G$ gives a character of degree prime to $p$, hence an irreducible constituent of such degree. On $Q$ its [determinant character](#determinant-character) is a nontrivial power of the chosen linear character, but every determinant character is trivial on $G'$. This contradiction proves the displayed restriction.

#### Kernel of a character

↑ **Parent:** [Character of a representation](#character-of-a-representation)

For a complex character $\chi$ of a [finite group](group.md#finite-group), its kernel is the kernel of an affording [group representation](#group-representation). Averaging an inner product makes that representation unitary. If its degree is $d$, all eigenvalues of a group element have modulus one, so their sum equals $d$ only when every eigenvalue is one. Thus the displayed character-value criterion agrees with the representation kernel and defines a [normal subgroup](group-theory.md#normal-subgroup).

#### Characters distinguish finite-dimensional complex semisimple representations

↑ **Parent:** [Character of a representation](#character-of-a-representation)

For any group, take the group-algebra image on the [direct sum](vector-space.md#direct-sum) of two finite-dimensional complex semisimple representations. Its radical annihilates their simple summands and hence the faithful [direct sum](vector-space.md#direct-sum), so the image algebra is semisimple. Equality of traces on group elements gives equality on their linear span. Traces on primitive central blocks then recover every simple multiplicity, proving that equal [characters](#character-of-a-representation) imply isomorphism.

#### Character value of a representation

↑ **Parent:** [Character of a representation](#character-of-a-representation)

At an element $g$ of a [finite group](group.md#finite-group), a complex character value is the sum of the [roots of unity](algebra.md#root-of-unity) which are the [eigenvalues](linear-operator-theory.md#eigenvalue) of its representing [matrix](vector-space.md#matrix). It is therefore an [algebraic integer](algebraic-number-theory.md#algebraic-integer), and every [algebraic conjugate](algebra.md#conjugate-element-field-theory) has modulus at most the degree.

#### Irreducible character

↑ **Parent:** [Character of a representation](#character-of-a-representation)

An irreducible character is the character of an [irreducible representation](#irreducible-representation). Over the complex numbers, every finite-group character decomposes uniquely as a nonnegative integer combination of irreducible characters.

##### Frobenius-Schur indicator

↑ **Parent:** [Irreducible character](#irreducible-character)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frobenius–Schur_indicator)

For an irreducible complex [character of a representation](#character-of-a-representation), the indicator is $1$ for real type, $-1$ for quaternionic type and $0$ for complex type, the latter meaning $\chi\ne\overline\chi$. It detects the invariant bilinear form on an irreducible representation. For an odd-order group, squaring permutes its elements, so every nontrivial irreducible character has indicator zero by [character orthogonality](#character-orthogonality).

###### Central average of representation matrices at squares

↑ **Parent:** [Frobenius-Schur indicator](#frobenius-schur-indicator)

For a complex [irreducible representation](#irreducible-representation) $D$ of a [finite group](group.md#finite-group) $G$, the sum $A=\sum_gD(g^2)$ commutes with every $D(h)$: conjugation sends its summands to $D((hgh^{-1})^2)$, merely permuting the summation index. [Schur's lemma](#schur-s-lemma) gives $A=cI$. Taking the [trace](linear-algebra.md#matrix-trace) yields $c\dim D=\sum_g\chi(g^2)=|G|\nu(D)$, proving the identity. Here $\nu(D)$ is the [Frobenius-Schur indicator](#frobenius-schur-indicator). For a reducible representation the sum is still central in its image, but need not be one scalar on all irreducible constituents.

###### Odd-order group conjugacy-class congruence

↑ **Parent:** [Frobenius-Schur indicator](#frobenius-schur-indicator)

An odd-order [finite group](group.md#finite-group) has only odd irreducible degrees, by [irreducible character degree divides the group order](#irreducible-character-degree-divides-the-group-order). Its nontrivial characters occur in distinct conjugate pairs, by the [Frobenius-Schur indicator](#frobenius-schur-indicator). Therefore $|G|-k(G)=\sum_\chi(\chi(1)^2-1)$ is a sum of pairs $2(d^2-1)$ with $d$ odd. Since $d^2\equiv1\pmod8$, each pair is divisible by sixteen. Here $k(G)$ is the number of [conjugacy classes](group-action.md#conjugacy-class).

##### Odd-order groups have no nontrivial real irreducible characters

↑ **Parent:** [Irreducible character](#irreducible-character)

For a real-valued [irreducible character](#irreducible-character) of a finite odd-order group, pairing $g$ with $g^{-1}$ gives $\langle\chi,1_G\rangle=(\chi(1)+2A)/|G|$, with $A$ an [algebraic integer](algebraic-number-theory.md#algebraic-integer). If this inner product were zero, $\chi(1)$ would be even, since a rational [algebraic integer](algebraic-number-theory.md#algebraic-integer) is an integer. But an [irreducible character degree divides the group order](#irreducible-character-degree-divides-the-group-order), so it is odd. Therefore the character is trivial.

#### Character constituent

↑ **Parent:** [Character of a representation](#character-of-a-representation)

An irreducible character $\varphi$ is a constituent of a character $\chi$ when its multiplicity $\langle\chi,\varphi\rangle$ is positive.

#### Restriction of a character

↑ **Parent:** [Character of a representation](#character-of-a-representation)

For a subgroup $H\leq G$, the restriction of a $G$-character $\chi$ to $H$ is the $H$-character obtained by evaluating the same function only on elements of $H$.

##### Character extension

↑ **Parent:** [Restriction of a character](#restriction-of-a-character)

An extension of $\theta\in\operatorname{Irr}(N)$ from $N\triangleleft G$ is a character $\chi$ of $G$ whose restriction is exactly $\theta$. It is necessarily irreducible, because a nontrivial invariant subspace for $G$ would also be one for $N$. An ordinary extension can fail to exist even when $\theta$ is invariant under $G$.

<h6 id="thompson-s-coprime-character-extension-theorem">Thompson's coprime character extension theorem</h6>

↑ **Parent:** [Character extension](#character-extension)

Let $N\triangleleft G$ and let $\theta\in\operatorname{Irr}(N)$ be invariant under $G$. If $\theta(1)$ is coprime to $[G:N]$, then $\theta$ extends to $G$ if and only if its [determinant character](#determinant-character) extends to a linear character of $G$. In particular, if the determinant order is also coprime to the index, there is a unique extension whose determinant order is coprime to the index. When $G/N$ is a p-group and $N=O^p(N)$, every invariant irreducible character of degree prime to $p$ satisfies this latter determinant condition.

###### Gluing determinant-normalized character extensions

↑ **Parent:** [Character extension](#character-extension)

Under the invariant, coprime-degree and determinant hypotheses of the [coprime-degree determinant extension theorem](#coprime-degree-determinant-extension-theorem), without assuming $G/N$ solvable, each cyclic-quotient subgroup $N\langle g\rangle$ has a unique determinant-normalized extension. Use its value at $g$ to define $f$. Uniqueness makes $f$ conjugacy-invariant. On an [elementary subgroup](group.md#elementary-group) $E$, it agrees with the restriction of the extension to $NE$, since $NE/N$ is a solvable quotient of $E$. [Brauer's characterization of characters](#brauer-s-characterization-of-characters) therefore makes $f$ a [generalized character](#virtual-character), with $f_N=\theta$.

###### Coprime-degree determinant extension theorem

↑ **Parent:** [Character extension](#character-extension)

Suppose $N\triangleleft G$, $G/N$ is solvable, $\theta\in\operatorname{Irr}(N)$ is invariant under $G$, and $\theta(1)$ is coprime to $[G:N]$. If a [linear character](#linear-character) $\mu$ of $G$ restricts to the [determinant character](#determinant-character) $\det\theta$, then there is a unique [character extension](#character-extension) $\chi\in\operatorname{Irr}(G)$ with determinant $\mu$. This is the solvable-quotient extension result supplied for the exam's application.

##### Inertia group of a character

↑ **Parent:** [Restriction of a character](#restriction-of-a-character)

For $N\triangleleft G$ and $\theta\in\operatorname{Irr}(N)$, set $\theta^g(n)=\theta(g^{-1}ng)$. Its inertia group is its stabilizer under this conjugation action and contains $N$. Write $\operatorname{Irr}(G\mid\theta)$ for the [irreducible characters](#irreducible-character) of $G$ whose restriction to $N$ contains $\theta$.

###### Clifford correspondence

↑ **Parent:** [Inertia group of a character](#inertia-group-of-a-character)

For $N\triangleleft G$, $\theta\in\operatorname{Irr}(N)$ and $T=I_G(\theta)$, induction gives the displayed bijection. The inverse takes the $\theta$-[isotypic component](module-theory.md#isotypic-component) of an irreducible $G$-module, viewed as a $T$-module. Induction produces distinct $N$-isotypic components indexed by $G/T$. Any nonzero $G$-submodule meets one of them and hence, by translation and irreducibility over $T$, contains them all. The same argument shows that the inverse component is irreducible and determines the original inducing module uniquely.

##### Character restriction norm bound

↑ **Parent:** [Restriction of a character](#restriction-of-a-character)

If $\chi$ is an [irreducible character](#irreducible-character) of a finite group $G$ and $H\leq G$, then

$$
\left\langle\operatorname{Res}_H^G\chi,
\operatorname{Res}_H^G\chi\right\rangle_H\leq[G:H].
$$

Equality holds exactly when $\chi$ vanishes on $G\setminus H$.

###### Index-two character restriction dichotomy

↑ **Parent:** [Character restriction norm bound](#character-restriction-norm-bound)

Let $H\triangleleft G$ have index two, and let $\lambda$ be the nontrivial linear character of $G/H$ inflated to $G$. For an irreducible character $\chi$ of $G$, either $\operatorname{Res}_H^G\chi$ is irreducible and $\chi\ne\chi\lambda$, or the restriction is a sum of two distinct irreducible characters and $\chi=\chi\lambda$.

#### Virtual character

↑ **Parent:** [Character of a representation](#character-of-a-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Virtual_character)

A virtual character is an integer linear combination of characters, equivalently an element of the Grothendieck group of finite-dimensional representations.

<h5 id="brauer-s-characterization-of-characters">Brauer's characterization of characters</h5>

↑ **Parent:** [Virtual character](#virtual-character)

A complex [class function](#class-function) $f$ on a finite group is a [generalized character](#virtual-character) if and only if $f_E$ is a generalized character of every [elementary subgroup](group.md#elementary-group). Equivalently, $\langle f_E,\alpha\rangle_E\in\mathbb Z$ for every such $E$ and $\alpha\in\operatorname{Irr}(E)$. Ordinary characters additionally have nonnegative global irreducible multiplicities; integrality of the virtual-character lattice is the conclusion of this criterion.

###### Generalized character separating complementary prime elements

↑ **Parent:** [Brauer's characterization of characters](#brauer-s-characterization-of-characters)

Suppose every nonidentity element of a finite group $K$ is either a [pi-element](group.md#pi-element) or an element for complementary primes. An [elementary subgroup](group.md#elementary-group) cannot have nontrivial factors of both kinds, since the product of nonidentity commuting coprime-order elements would have mixed prime order. Choose an integer $d$ congruent to $1$ modulo $|K|_\pi$ and to $0$ modulo $|K|_{\pi'}$. Set $f(1)=d$, $f=1$ on nonidentity pi-elements and $f=0$ on the other nonidentity elements. On each elementary subgroup this is an integer combination of the trivial and regular characters. [Brauer's characterization of characters](#brauer-s-characterization-of-characters) supplies the asserted [generalized character](#virtual-character).

##### Positive-degree norm-one virtual characters are irreducible

↑ **Parent:** [Virtual character](#virtual-character)

Write the [virtual character](#virtual-character) as $\psi=\sum_\chi a_\chi\chi$ with integer coefficients and [irreducible characters](#irreducible-character) $\chi$. [Character orthogonality](#character-orthogonality) gives $\langle\psi,\psi\rangle=\sum_\chi a_\chi^2$. Norm one forces exactly one coefficient to be $1$ or $-1$, and positive degree selects the positive sign.

<h2 id="burnside-s-lemma">Burnside's lemma</h2>

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Burnside's_lemma)

For a finite group $G$ acting on a finite set $X$, the number of orbits is

$$
|X/G|=\frac1{|G|}\sum_{g\in G}|X^g|.
$$

It follows by counting pairs $(g,x)$ with $gx=x$ first by $g$ and then by $x$.

### Cycle index

↑ **Parent:** [Burnside's lemma](#burnside-s-lemma)

For a [permutation group](finite-group-theory.md#permutation-group), $c_r(g)$ is the number of length-$r$ cycles of $g$. The cycle index records the average cycle structure. On coloring a finite underlying set, a coloring fixed by $g$ is constant on each cycle. Replacing $t_r$ by the [power-sum symmetric polynomial](combinatorics.md#power-sum-symmetric-polynomial) $p_r(x)$ therefore gives the [pattern inventory](#pattern-inventory) by the [weighted Burnside lemma](#weighted-burnside-lemma).

#### Pattern inventory

↑ **Parent:** [Cycle index](#cycle-index)

This is the sum of content [monomials](polynomial.md#monomial) of colorings up to the [group action](group-action.md). It equals the [cycle index](#cycle-index) specialized at $t_r=p_r(x)$. One may first use finitely many colors; stabilization defines the corresponding homogeneous [symmetric function](combinatorics.md#symmetric-function). Calling the specialized cycle index a cycle indicator makes $Z_G=F_G$ an equality in the same variables.

### Weighted Burnside lemma

↑ **Parent:** [Burnside's lemma](#burnside-s-lemma)

For an orbit-invariant weight $w$ on a finite [group action](group-action.md) $G\curvearrowright X$, the sum of one weight per orbit is $|G|^{-1}\sum_g\sum_{x:gx=x}w(x)$. Double counting gives $\sum_x|G_x|w(x)$ before dividing by $|G|$; each orbit contributes $|G|$ copies of its common weight. Thus the usual [Burnside's lemma](#burnside-s-lemma) extends to weights in any commutative coefficient ring.

### Permutation representation of a two-transitive action

↑ **Parent:** [Burnside's lemma](#burnside-s-lemma)

If a finite group acts two-transitively on $X$, then

$$
\mathbb C[X]\cong\mathbf1\oplus V,
$$

where $V$ is irreducible and nontrivial. The character norm is the number of orbits on $X\times X$, namely the diagonal and its complement.

#### Steinberg representation of GL2 over a finite field

↑ **Parent:** [Permutation representation of a two-transitive action](#permutation-representation-of-a-two-transitive-action)

The action of $GL_2(\mathbb F_q)$ on $\mathbb P^1(\mathbb F_q)$ has permutation representation $\mathbf1\oplus\mathrm{St}$. The Steinberg constituent is irreducible of dimension $q$ and has character values $q,0,1,-1$ on scalar, nontrivial Jordan, split regular semisimple, and nonsplit semisimple elements respectively.

## Permutation representation

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Permutation_representation)

For a finite $G$-set $X$, the character of $\mathbb C[X]$ at $g$ is $|X^g|$. Its invariant dimension is the number of $G$-orbits.

### Rank of a permutation action

↑ **Parent:** [Permutation representation](#permutation-representation)

The rank is the number of orbits on ordered pairs under the diagonal [group action](group-action.md). Its fixed-pair count at $g$ is $\chi(g)^2$, since the [permutation character](#permutation-character) counts fixed points. [Burnside's lemma](#burnside-s-lemma) identifies its average with the orbit count, while real-valuedness makes that average the [character inner product](#character-inner-product) of $\chi$ with itself. For a transitive action on at least two points, rank two is equivalent to transitivity on distinct ordered pairs.

### Permutation module

↑ **Parent:** [Permutation representation](#permutation-representation)

For a finite [group action](group-action.md) on a finite set $X$, $R[X]$ is the free $R$-module with basis $X$, with the group permuting that basis. For a transitive set $G/H$ it is $\operatorname{Ind}_H^G R$. Disjoint unions of sets give [direct sums](vector-space.md#direct-sum) of permutation modules.

### Deleted permutation module in characteristic two

↑ **Parent:** [Permutation representation](#permutation-representation)

For even degree the augmentation hyperplane has an alternating dot product whose radical is the all-ones line. Quotienting by that line gives a nondegenerate symplectic space of dimension two less than the permutation degree. Coordinate permutations preserve the form. In degree at least six their quotient action is faithful, since two distinct weight-two coordinate vectors cannot differ by the all-ones vector. In degree six this gives $S_6\cong Sp_4(2)$; in degree four the quotient action instead has Klein-four kernel.

### Permutation character

↑ **Parent:** [Permutation representation](#permutation-representation)

The character of a permutation representation counts fixed points: $\chi(g)=|\{\omega:g\omega=\omega\}|$. Its self-inner-product counts orbits on ordered pairs, while its inner product with the trivial character counts orbits on the original set.

### Gassmann equivalence

↑ **Parent:** [Permutation representation](#permutation-representation)

Subgroups $H_1,H_2$ of a finite [group](group.md) $G$ are Gassmann equivalent if $|H_1\cap C|=|H_2\cap C|$ for every [conjugacy class](group-action.md#conjugacy-class) $C$. Equivalently their coset [permutation representations](#permutation-representation) have the same [character of a representation](#character-of-a-representation). They need not be conjugate subgroups. The [Sunada theorem](riemannian-geometry.md#sunada-theorem) turns this equality into equality of [Laplacian eigenfunction](partial-differential-equation.md#laplacian-eigenfunction) multiplicities.

#### Point and hyperplane stabilizers are almost conjugate

↑ **Parent:** [Gassmann equivalence](#gassmann-equivalence)

In a finite [general linear group](group-theory.md#general-linear-group), the [permutation representations](#permutation-representation) on nonzero vectors and on nonzero dual vectors have equal [characters](#character-of-a-representation): an element fixes $q^{\dim\ker(t-I)}-1$ vectors in each action because a matrix and its transpose have the same rank. In characteristic two the stabilizers of a nonzero vector and a hyperplane are therefore [almost conjugate subgroups](#gassmann-equivalence). In dimension three over $\mathbb F_2$, both have order $24$ and index $7$ in a group of order $168$, but they are not conjugate: a point stabilizer preserves no plane. A [triangle cover construction for Sunada surfaces](riemannian-geometry.md#triangle-cover-construction-for-sunada-surfaces) with generator orders $(7,7,7)$ gives quotient surfaces of [genus](topological-surface.md#genus-of-a-surface) three.

#### Order-sixteen Gassmann pair

↑ **Parent:** [Gassmann equivalence](#gassmann-equivalence)

Embed $C_4\times C_4$ and $Q_8\times C_2$ in $S_{16}$ by their [regular representations](#regular-representation). Both have one element of order one, three of order two, and twelve of order four. An order-$r$ element in a regular action has cycle type $r^{16/r}$. Their intersections with every [conjugacy class](group-action.md#conjugacy-class) of $S_{16}$ consequently have the same size, so they are [Gassmann equivalent](#gassmann-equivalence). The first group is abelian and the second is not, so their underlying groups are not isomorphic. Finite-cover constructions from the [Sunada theorem](riemannian-geometry.md#sunada-theorem) therefore give [isospectral manifolds](riemannian-geometry.md#isospectral-manifolds) with different [fundamental groups](algebraic-topology.md#fundamental-group).

#### Nonisomorphic Gassmann equivalent regular subgroups

↑ **Parent:** [Gassmann equivalence](#gassmann-equivalence)

For an odd prime $p$, embed the elementary abelian group $(C_p)^3$ and the [Heisenberg group over a prime field](finite-group-theory.md#heisenberg-group-over-a-prime-field) regularly in $S_{p^3}$. Every nonidentity element has order $p$ and hence regular permutation cycle type $p^{p^2}$. The two [subgroups](group.md#subgroup) have equal intersection counts with every symmetric-group [conjugacy class](group-action.md#conjugacy-class), so they are [Gassmann equivalent](#gassmann-equivalence), but they are not isomorphic because one is abelian and the other is not. Using a compact [simply connected](algebraic-topology.md#simply-connected-space) isometric cover with ambient deck group $S_{p^3}$ gives quotients with these nonisomorphic [fundamental groups](algebraic-topology.md#fundamental-group); [Sunada theorem](riemannian-geometry.md#sunada-theorem) makes them isospectral while their topology differs.

### Permutation character of a coset action

↑ **Parent:** [Permutation representation](#permutation-representation)

For a subgroup $H\leq G$, the permutation character of the [coset action](group-action.md#coset-action) on $G/H$ is the induced trivial character

$$
\pi_{G/H}=1_H\mathbin{\uparrow}^G,
$$

and

$$
\pi_{G/H}(g)
=|\{xH:gxH=xH\}|
=\frac1{|H|}|\{x\in G:x^{-1}gx\in H\}|.
$$

### Augmentation subrepresentation of a permutation representation

↑ **Parent:** [Permutation representation](#permutation-representation)

For a finite $G$-set $X$, the coefficient-sum map $\varepsilon:\mathbb C[X]\to\mathbb C$ is equivariant. Its kernel

$$
\mathbb C[X]_0
=\left\{\sum_{x\in X}a_xx:\sum_{x\in X}a_x=0\right\}
$$

is the augmentation subrepresentation. If $X$ is nonempty, then

$$
\mathbb C[X]
=\mathbb C\!\left(\sum_{x\in X}x\right)
\oplus\mathbb C[X]_0.
$$

#### Irreducible augmentation criterion for a transitive group action

↑ **Parent:** [Augmentation subrepresentation of a permutation representation](#augmentation-subrepresentation-of-a-permutation-representation)

For a transitive finite $G$-set $X$ with at least two points, the [augmentation subrepresentation of a permutation representation](#augmentation-subrepresentation-of-a-permutation-representation) is [irreducible](#irreducible-representation) if and only if the action is [two-transitive](group-action.md#two-transitive-group-action). Indeed, writing the permutation character as $\pi=1+\sum_i m_i\chi_i$ gives

$$
\langle\pi,\pi\rangle_G=1+\sum_i m_i^2.
$$

The augmentation subrepresentation is irreducible exactly when this norm is two. By the [character norm of a permutation representation](#character-norm-of-a-permutation-representation), that means that the diagonal and the off-diagonal are the only two orbits on $X\times X$, which is exactly two-transitivity.

### Character norm of a permutation representation

↑ **Parent:** [Permutation representation](#permutation-representation)

If $\pi$ is the character of $\mathbb C[X]$, then [Burnside lemma](#burnside-s-lemma) applied to the diagonal action on $X\times X$ gives

$$
\langle\pi,\pi\rangle_G
=\frac1{|G|}\sum_{g\in G}|X^g|^2
=|G\backslash(X\times X)|.
$$

For a transitive action $X\simeq G/H$, this also equals the number of [double cosets](group-theory.md#double-coset) in $H\backslash G/H$.

### Symmetric-group subset permutation representation

↑ **Parent:** [Permutation representation](#permutation-representation)

Let $S_n$ act on the $r$-element subsets of $\{1,\ldots,n\}$, with permutation character $\pi_r$. If $0\leq l\leq k\leq n/2$, then

$$
\langle\pi_k,\pi_l\rangle=l+1,
$$

because orbits of pairs are classified by intersection size $0,\ldots,l$.

#### Inclusion map between subset permutation modules

↑ **Parent:** [Symmetric-group subset permutation representation](#symmetric-group-subset-permutation-representation)

For $r\leq n/2$, the equivariant map from $(r-1)$-subsets to $r$-subsets that sends each subset to the sum of the $r$-subsets containing it is injective over $\mathbb C$. Hence $\pi_r-\pi_{r-1}$ is the character of a representation.

### Standard representation of the symmetric group

↑ **Parent:** [Permutation representation](#permutation-representation)

This representation is a distinguished example in the [representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md).

The permutation representation of $S_n$ on $\mathbb C^n$ decomposes as

$$
\mathbb C(1,\ldots,1)
\oplus
\{(x_1,\ldots,x_n):x_1+\cdots+x_n=0\}.
$$

The first summand is the trivial representation and the second is the $(n-1)$-dimensional standard representation.

<h4 id="gelfand-tsetlin-basis-of-the-standard-representation">Gelfand–Tsetlin basis of the standard representation</h4>

↑ **Parent:** [Standard representation of the symmetric group](#standard-representation-of-the-symmetric-group)

For the sum-zero [standard representation of the symmetric group](#standard-representation-of-the-symmetric-group), the vectors $v_j=e_1+\cdots+e_j-je_{j+1}$ form a [Gelfand–Tsetlin basis](representation-theory-of-the-symmetric-group.md#gelfand-tsetlin-basis). The [Young–Jucys–Murphy element](representation-theory-of-the-symmetric-group.md#jucys-murphy-element) $X_i$ has eigenvalue $i-1$ for $i\leq j$, $-1$ for $i=j+1$, and $i-2$ for $i>j+1$. Normalizing by $\sqrt{j(j+1)}$ gives an [orthonormal basis](inner-product.md#orthonormal-basis) corresponding to tableaux of shape $(n-1,1)$ whose second-row entry is $j+1$.

#### Three-dimensional irreducible representation of the alternating group on four letters

↑ **Parent:** [Standard representation of the symmetric group](#standard-representation-of-the-symmetric-group)

The [standard representation of the symmetric group](#standard-representation-of-the-symmetric-group) $S_4$ restricts irreducibly to $A_4$. Its character has value $3$ at the identity and $-1$ on each nonidentity element of the normal [Klein four-group](finite-group-theory.md#klein-four-group). Restricted to that subgroup, it is the sum of the three nontrivial linear characters.

## Representation theory of the symmetric group

↑ **Parent:** [Representation theory](representation-theory.md)

[This section is present in another page, follow this link to view it.](representation-theory-of-the-symmetric-group.md)

## Intertwining operator

↑ **Parent:** [Representation theory](representation-theory.md)

An intertwining operator between representations $\rho$ and $\sigma$ is a linear [equivariant map](group-action.md#equivariant-map) $T$ satisfying $T\rho(g)=\sigma(g)T$ for every group element $g$.

### Reduced matrix element

↑ **Parent:** [Intertwining operator](#intertwining-operator)

A tensor operator transforming in an [irreducible representation](#irreducible-representation) $R$ between states in $V$ defines an [intertwining operator](#intertwining-operator) $R\otimes V\to V$. In a basis of these intertwining maps, its scalar coefficients $g_\nu$ are reduced matrix elements, independent of the component indices. [Schur lemma](#schur-s-lemma) makes the number of independent coefficients the multiplicity of $V$ in $R\otimes V$. The component dependence is fixed by the associated [Clebsch-Gordan coefficients](#clebsch-gordan-coefficients).

#### Wigner-Eckart theorem

↑ **Parent:** [Reduced matrix element](#reduced-matrix-element)

The [Wigner-Eckart theorem](#wigner-eckart-theorem) separates the dependence of a [spherical tensor operator](angular-momentum-operator.md#spherical-tensor-operator) on [angular momentum](momentum.md#angular-momentum) projections from its dynamical content. In one standard convention,

$$
\langle\lambda'j'm'|T_q^{(k)}|\lambda jm\rangle
=\frac{\langle jm;kq|j'm'\rangle}{\sqrt{2j'+1}}
\langle\lambda'j'\Vert T^{(k)}\Vert\lambda j\rangle.
$$

The [reduced matrix element](#reduced-matrix-element) on the right is independent of $m,m',q$. The [Clebsch-Gordan coefficients](#clebsch-gordan-coefficients) impose $m'=m+q$ and $|j-k|\leq j'\leq j+k$; additional [selection rules](atomic-physics.md#selection-rule), including [parity](quantum-mechanics.md#parity), can make the [reduced matrix element](#reduced-matrix-element) vanish.

To see why the factorization holds, combine the rank-$k$ transformation law of the operator with the spin-$j$ transformation law of the initial state. This gives an [intertwining operator](#intertwining-operator) from the [tensor product representation](#tensor-product-of-group-representations) $j\otimes k$ to the final representation $j'$. The [Clebsch-Gordan decomposition](angular-momentum-operator.md#clebsch-gordan-decomposition) contains each allowed $j'$ once. Therefore the corresponding [intertwining operator](#intertwining-operator) is unique up to an overall scalar, which is the [reduced matrix element](#reduced-matrix-element) after the chosen normalization. Ratios within the same pair of multiplets depend only on [Clebsch-Gordan coefficients](#clebsch-gordan-coefficients), whenever the common [reduced matrix element](#reduced-matrix-element) is nonzero.

#### Two reduced octet matrix elements

↑ **Parent:** [Reduced matrix element](#reduced-matrix-element)

An octet operator between [baryon octet](standard-model.md#baryon-octet) states has two [reduced matrix elements](#reduced-matrix-element), because the [tensor square of the SU(3) adjoint representation](lie-algebra.md#tensor-square-of-the-su-3-adjoint-representation) contains two octets. The symmetric invariant $d_{ris}$ and antisymmetric invariant $f_{ris}$ give independent component tensors. Equivalently, represent baryons by traceless matrices $B$ and let the operator act as $F[t_i,B]+D(\{t_i,B\}-\tfrac23\operatorname{tr}(t_iB)I)$. Normalization choices are absorbed into $F,D$; Hermitian operators permit real coefficients in a Hermitian octet basis.

<h2 id="schur-s-lemma">Schur's lemma</h2>

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur's_lemma)

An intertwiner between irreducible complex representations is either zero or an isomorphism; an endomorphism of one irreducible is scalar.

### Proof of Schur lemma

↑ **Parent:** [Schur's lemma](#schur-s-lemma)

The kernel and image of an intertwiner are invariant subspaces. Irreducibility therefore makes a nonzero intertwiner injective and surjective. For an endomorphism $T$ of a finite-dimensional irreducible complex representation, choose an eigenvalue $\lambda$. The noninvertible intertwiner $T-\lambda I$ must be zero, so $T=\lambda I$.

### Failure of the scalar conclusion of Schur lemma over the real numbers

↑ **Parent:** [Schur's lemma](#schur-s-lemma)

Let a cyclic-group generator act on a real plane by a rotation through an angle other than zero or $\pi$. The representation is irreducible, but its commuting endomorphisms are

$$
\{aI+bJ:a,b\in\mathbb R,\ J^2=-I\}\cong\mathbb C.
$$

The non-scalar complex structure $J$ shows that the scalar endomorphism conclusion of [Schur lemma](#schur-s-lemma) fails over $\mathbb R$.

### Cyclic-center obstruction to a faithful irreducible representation

↑ **Parent:** [Schur's lemma](#schur-s-lemma)

If a finite group has a faithful irreducible complex representation, every central element acts as a scalar by [Schur lemma](#schur-s-lemma). Faithfulness embeds the centre into $\mathbb C^\times$, and every finite subgroup of $\mathbb C^\times$ is cyclic. Hence the group centre must be cyclic.

## Dual representation

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_representation)

For a representation on $V$, the dual action on $V^*$ is $(g\varphi)(v)=\varphi(g^{-1}v)$.

### Algebraic contragredient representation

↑ **Parent:** [Dual representation](#dual-representation)

The algebraic contragredient acts on the entire algebraic [dual space](dual-space.md). It need not be a [smooth representation](#smooth-representation-of-a-locally-profinite-group), even if the original representation is smooth. Taking the inverse in this formula is necessary to obtain a group action, and inverts a one-dimensional [linear character](#linear-character).

#### Conjugate contragredient representation

↑ **Parent:** [Algebraic contragredient representation](#algebraic-contragredient-representation)

For a finite-dimensional complex [group representation](#group-representation), combining inverse and [conjugate transpose](linear-operator-theory.md#conjugate-transpose) gives another representation: both operations reverse multiplication order. This is the complex conjugate of the algebraic [dual representation](#dual-representation) in matrices. If $W$ is invariant under $D^\#$, its orthogonal complement is invariant under $D$, because $\langle w,D(g)v\rangle=\langle D^\#(g^{-1})w,v\rangle=0$ for $w\in W$, $v\in W^\perp$. Thus irreducibility is preserved. Applying the construction twice returns $D$, so the equivalence of irreducibility works in both directions for arbitrary groups in finite dimension.

#### Smooth dual

↑ **Parent:** [Algebraic contragredient representation](#algebraic-contragredient-representation)

The smooth dual consists of the [smooth vectors](#smooth-vector) of the [algebraic contragredient representation](#algebraic-contragredient-representation). Their union is a vector subspace because finite intersections of open stabilizers remain open; it is invariant because translation conjugates stabilizers.

##### Conductors force finite support in a smooth dual

↑ **Parent:** [Smooth dual](#smooth-dual)

If one-dimensional smooth [linear characters](#linear-character) of a local multiplicative group have conductors tending to infinity, their [direct sum](vector-space.md#direct-sum) can be admissible. Its algebraic dual is the product of inverse [linear characters](#linear-character), but a [smooth vector](#smooth-vector) in this product has only finitely many nonzero coordinates. A common open stabilizer contains one fixed principal-unit subgroup, on which every sufficiently ramified [linear character](#linear-character) is nontrivial. Thus the smooth dual is again a [direct sum](vector-space.md#direct-sum).

### Character of a Hom representation

↑ **Parent:** [Dual representation](#dual-representation)

For complex representations $V,W$ of a finite group,

$$
\operatorname{Hom}_{\mathbb C}(V,W)\cong V^*\otimes W.
$$

Under the $G\times G$ action $(g,h)\alpha=\sigma(h)\alpha\rho(g^{-1})$, its character is

$$
\chi_{\operatorname{Hom}(V,W)}(g,h)
=\overline{\chi_V(g)}\,\chi_W(h).
$$

#### Two-sided regular representation decomposition

↑ **Parent:** [Character of a Hom representation](#character-of-a-hom-representation)

Let $G\times G$ act on $\mathbb C G$ by $(g,h)x=gxh^{-1}$. Its character is zero unless $g$ and $h$ are conjugate, in which case it equals $|C_G(g)|$. Character column orthogonality gives the same character for

$$
\bigoplus_i\operatorname{Hom}_{\mathbb C}(V_i,V_i),
$$

where the $V_i$ run through the irreducible complex representations. Maschke's theorem therefore gives an isomorphism of the two representations.

### Invariant bilinear form as an intertwiner

↑ **Parent:** [Dual representation](#dual-representation)

A bilinear form $B$ on $V$ is invariant exactly when $v\mapsto B(v,-)$ is a $G$-homomorphism $V\to V^*$. On an irreducible representation, Schur's lemma makes a nonzero such form [nondegenerate](bilinear-form.md#nondegenerate-bilinear-form) and unique up to scale.

#### Symmetric-or-alternating dichotomy for invariant forms

↑ **Parent:** [Invariant bilinear form as an intertwiner](#invariant-bilinear-form-as-an-intertwiner)

Transposing a nonzero invariant bilinear form on an irreducible complex representation gives a scalar multiple $B^T=\lambda B$. Transposing twice yields $\lambda^2=1$, so the form is symmetric or alternating.

## Induced representation

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Induced_representation)

Induction extends a representation of a subgroup to the whole group; Frobenius reciprocity computes its multiplicities.

### Extension of a faithful representation from an open normal subgroup

↑ **Parent:** [Induced representation](#induced-representation)

Let $H$ be an [open normal subgroup](topological-group.md#open-normal-subgroup) of a [compact topological group](topological-group.md#compact-group) $G$, and let $\tau:H\to\operatorname{GL}_m(\mathbb Z_p)$ be a continuous [faithful representation](#faithful-representation). Choose representatives $t_j$ for the finite left [cosets](group-theory.md#coset) $G/H$. Write $gt_j=t_i h_{ij}$ and act on the $j$-th summand of $\bigoplus_j\mathbb Z_p^m$ by $\tau(h_{ij})$ into the $i$-th summand. The cocycle identity proves this is a continuous [group representation](#group-representation). An element outside $H$ has a nontrivial coset permutation, while an element of $H$ acting trivially has $\tau(g)=1$ on the identity-coset summand. Hence the representation of $G$ is faithful and integral.

### Unnormalized parabolic induction

↑ **Parent:** [Induced representation](#induced-representation)

For a smooth [linear character](#linear-character) $\chi$ of a parabolic subgroup $B$, unnormalized induction consists of smooth functions satisfying $f(bg)=\chi(b)f(g)$, with right-translation action. The quotient $B\backslash G$ is compact for the local general linear groups in question. Normalized induction inserts a square root of the parabolic modulus in the covariance, changing formulas for the inducing [linear character](#linear-character).

#### Evaluation adjunction for unnormalized induction

↑ **Parent:** [Unnormalized parabolic induction](#unnormalized-parabolic-induction)

Evaluation of an intertwiner at the identity gives a $B$-equivariant functional. Conversely a functional $\ell$ gives $A(v)(g)=\ell(\pi(g)v)$, which has the required covariance and is fixed on the right by any [compact-open subgroup](topological-group.md#compact-open-subgroup) fixing $v$. These inverse constructions prove the displayed adjunction. If $\xi$ is trivial on the unipotent radical, it is equivalent to a character-valued functional on the [Jacquet module](#jacquet-module).

#### Local principal series of GL2

↑ **Parent:** [Unnormalized parabolic induction](#unnormalized-parabolic-induction)

The local principal series of GL2 induces a smooth [linear character](#linear-character) of its diagonal torus, inflated to its upper-triangular subgroup. Its unnormalized [Jacquet module](#jacquet-module) has two one-dimensional composition factors, $\chi$ and $\chi^w\delta^{-1}$, where $\delta(\operatorname{diag}(a,d))=|d/a|$. When these coincide, the module is a nonsplit self-extension, so one must not count the [linear character](#linear-character) twice as two independent quotients.

##### Local Steinberg representation of GL2

↑ **Parent:** [Local principal series of GL2](#local-principal-series-of-gl2)

The local Steinberg representation is the quotient of locally constant functions on the projective line by constant functions, with the action induced from GL2. In the unnormalized convention, $V(1)$ fits into $0\to1\to V(1)\to\operatorname{St}\to0$. Its scalar endomorphism algebra obstructs a splitting. This local infinite-dimensional representation differs from the finite-field Steinberg representation.

##### Equal-character Jacquet self-extension for GL2

↑ **Parent:** [Local principal series of GL2](#local-principal-series-of-gl2)

At $\chi=\chi^w\delta^{-1}$, a determinant-character twist reduces to $\chi(\operatorname{diag}(a,d))=|a|$. In the open Bruhat coordinate, a section $g_0(x)=1$ for $|x|\le1$ and $g_0(x)=|x|^{-1}$ otherwise has $\pi(\operatorname{diag}(\varpi,1))g_0-q^{-1}g_0=(1-q^{-1})1_{\varpi\mathfrak o}$. Its additive Haar integral is nonzero, whereas every unipotent translation difference has zero such integral. The difference therefore survives in the [Jacquet module](#jacquet-module), proving that this two-dimensional self-extension is nonsplit and has just one quotient functional of the common [linear character](#linear-character).

### Monomiality of irreducible representations of finite p-groups

↑ **Parent:** [Induced representation](#induced-representation)

Every complex [irreducible representation](#irreducible-representation) of a finite [p-group](finite-group-theory.md#p-group) is induced from a one-dimensional representation of a subgroup. Induct on the group order. Nonfaithful representations reduce to a smaller quotient. For a faithful representation of a nonabelian group, choose an abelian normal subgroup not contained in the centre. Restriction cannot be isotypic, since it would make that subgroup scalar and faithfulness would then force it central. The [Clifford correspondence](#clifford-correspondence) induces the representation from a proper subgroup; induction there and transitivity of induction complete the proof. Abelian groups have only one-dimensional complex irreducible representations.

### Induced character

↑ **Parent:** [Induced representation](#induced-representation)

For a character $\psi$ of $H\leq G$, the induced character is

$$
(\operatorname{Ind}_H^G\psi)(g)=\frac1{|H|}\sum_{x\in G:\,x^{-1}gx\in H}\psi(x^{-1}gx).
$$

This is the [character of a representation](#character-of-a-representation) of $\mathbb C[G]\otimes_{\mathbb C[H]}V_\psi$. Substituting this expression into the character inner product and putting $g=xhx^{-1}$ proves [Frobenius reciprocity](#frobenius-reciprocity).

#### Monomial character

↑ **Parent:** [Induced character](#induced-character)

A monomial character is a character induced from a [linear character](#linear-character) of a subgroup. When discussing monomial finite groups, this property is required for every [irreducible character](#irreducible-character).

#### Character induction norm bound

↑ **Parent:** [Induced character](#induced-character)

Extend a class function $\psi$ on $H$ by zero outside $H$. For coset representatives $x_1,\ldots,x_m$ of $G/H$, $\operatorname{Ind}_H^G\psi(g)=\sum_j\psi_0(x_j^{-1}gx_j)$. Each summand has squared normalized $G$-norm $\|\psi\|_H^2/m$. Pointwise [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and summation give $\|\operatorname{Ind}\psi\|_G^2\le m\|\psi\|_H^2$. If $\psi$ is an irreducible character, its norm is one, and the sum of squared induction multiplicities is at most the subgroup index.

#### Irreducible characters across an index-two subgroup

↑ **Parent:** [Induced character](#induced-character)

An index-two subgroup is normal. Conjugation by an outside element gives an involution on its irreducible characters. If $\psi^g\ne\psi$, the squared norm of induction is one, so induction is irreducible of twice the degree and restriction is $\psi+\psi^g$. If $\psi^g=\psi$, the squared norm is two, so induction has exactly two distinct constituents, each once. Each restricts to a representation containing $\psi$, and their total degree is twice that of $\psi$, forcing both degrees to equal that of $\psi$. This proves the fixed-orbit versus two-element-orbit classification without assuming extension of $\psi$ in advance.

### Rotation content of induced Lorentz representations

↑ **Parent:** [Induced representation](#induced-representation)

In the compact picture of a principal-series [group representation](#group-representation) of the [Lorentz spinor double cover](special-relativity.md#lorentz-spinor-double-cover), functions on [SU(2)](topological-group.md#su-2-group) have a fixed right-torus character $e^{-in\vartheta}$. Expanding into spin matrix coefficients leaves one right weight in each allowed spin, giving the displayed multiplicity-one rotation decomposition. The boost action couples these spaces. The central element acts by $(-1)^n$; even $n$ yields integer rotation spins and a [group representation](#group-representation) of the connected Lorentz group.

### Conjugate subgroup representation

↑ **Parent:** [Induced representation](#induced-representation)

For an $H$-representation $V$ and $g\in G$, the conjugate representation ${}^gV$ of $gHg^{-1}$ is defined by $(ghg^{-1})v=hv$. This transports the acting subgroup; it is distinct from conjugating complex matrix entries. It occurs in the [Mackey restriction formula](#mackey-restriction-formula).

### Character formula for an induced representation

↑ **Parent:** [Induced representation](#induced-representation)

For $H\leq G$ and an $H$-character $\chi$,

$$
(\operatorname{Ind}_H^G\chi)(g)=\frac1{|H|}
\sum_{\substack{x\in G\\x^{-1}gx\in H}}\chi(x^{-1}gx).
$$

### Induction from an abelian normal subgroup with a free character orbit

↑ **Parent:** [Induced representation](#induced-representation)

Let $N\triangleleft G$ be abelian and let a linear character $\theta$ of $N$ have stabilizer exactly $N$ under conjugation by $G$. Then $\operatorname{Ind}_N^G\theta$ is irreducible of degree $[G:N]$. Its value is zero outside $N$, while on $n\in N$ it is the sum of the characters in the $G$-orbit of $\theta$.

#### Irreducible characters of the affine semidirect product of orders eleven and five

↑ **Parent:** [Induction from an abelian normal subgroup with a free character orbit](#induction-from-an-abelian-normal-subgroup-with-a-free-character-orbit)

For $G=C_{11}\rtimes C_5$ with faithful action, the abelianization $G/C_{11}\cong C_5$ supplies five linear characters. The two orbits of size five on the nontrivial characters of $C_{11}$ induce two irreducible characters of degree five. Their squared degrees satisfy

$$
5\cdot1^2+2\cdot5^2=55,
$$

so these seven characters are all the irreducible characters of $G$.

### Tensor identity for induced representations

↑ **Parent:** [Induced representation](#induced-representation)

For a $G$-representation $W$ and an $H$-representation $V$,

$$
\operatorname{Ind}_H^G(\operatorname{Res}_H^G W\otimes V)
\cong W\otimes\operatorname{Ind}_H^G V.
$$

On group-algebra tensors the isomorphism sends $x\otimes(w\otimes v)$ to $xw\otimes(x\otimes v)$.

### Frobenius reciprocity

↑ **Parent:** [Induced representation](#induced-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frobenius_reciprocity)

For $H\leq G$, an $H$-representation $V$, and a $G$-representation $W$,

$$
\operatorname{Hom}_G(\operatorname{Ind}_H^GV,W)
\cong
\operatorname{Hom}_H(V,\operatorname{Res}_H^GW).
$$

Equivalently, induction and restriction are adjoint for character inner products.

### Mackey theory

↑ **Parent:** [Induced representation](#induced-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mackey_theory)

Mackey theory studies how induced representations behave under restriction and conjugation of subgroups.

#### Mackey restriction formula

↑ **Parent:** [Mackey theory](#mackey-theory)

For $H,K\leq G$ and a $K$-representation $V$,

$$
\operatorname{Res}_H^G\operatorname{Ind}_K^GV
\cong
\bigoplus_{x\in H\backslash G/K}
\operatorname{Ind}_{H\cap xKx^{-1}}^H
\operatorname{Res}_{H\cap xKx^{-1}}^{xKx^{-1}}({}^xV),
$$

where ${}^xV(xkx^{-1})=V(k)$.

To prove the formula, write induction as $\mathbb C[G]\otimes_{\mathbb C[K]}V$ and decompose the $(H,K)$-bimodule

$$
\mathbb C[G]=\bigoplus_{x\in H\backslash G/K}\mathbb C[HxK].
$$

For $L_x=H\cap xKx^{-1}$, the map

$$
\mathbb C[H]\otimes_{\mathbb C[L_x]}{}^xV
\longrightarrow
\mathbb C[HxK]\otimes_{\mathbb C[K]}V,
\qquad h\otimes v\longmapsto hx\otimes v,
$$

is a well-defined $H$-equivariant isomorphism. Taking the direct sum over the double cosets proves the result.

##### Mackey irreducibility criterion

↑ **Parent:** [Mackey restriction formula](#mackey-restriction-formula)

For an irreducible $H$-representation $V$, the induced representation $\operatorname{Ind}_H^GV$ is irreducible exactly when, for every nonidentity double coset representative $x\in H\backslash G/H$, the restrictions of $V$ and its $x$-conjugate to $H\cap xHx^{-1}$ have inner product zero.

##### Bruhat decomposition of SL2 over a finite field

↑ **Parent:** [Mackey restriction formula](#mackey-restriction-formula)

This is the finite special-linear-group instance of the general [Bruhat decomposition](lie-theory.md#bruhat-decomposition).

For the upper-triangular subgroup $B$ of $SL_2(\mathbb F_p)$ and

$$
w=\begin{pmatrix}0&-1\\1&0\end{pmatrix},
$$

the two double cosets are $B$ and $BwB$, and $B\cap wBw^{-1}=T$, the diagonal subgroup.

###### Mackey inner product for the finite SL2 principal series

↑ **Parent:** [Bruhat decomposition of SL2 over a finite field](#bruhat-decomposition-of-sl2-over-a-finite-field)

For one-dimensional representations $\theta,\varphi$ of the upper-triangular subgroup $B\leq SL_2(\mathbb F_p)$,

$$
\left\langle\operatorname{Ind}_B^G\theta,
\operatorname{Ind}_B^G\varphi\right\rangle_G
=\mathbf1_{\theta=\varphi}
+\mathbf1_{\theta^w|_T=\varphi|_T},
$$

where $\theta^w(t)=\theta(w^{-1}tw)$.

###### Irreducible principal series of finite SL2

↑ **Parent:** [Mackey inner product for the finite SL2 principal series](#mackey-inner-product-for-the-finite-sl2-principal-series)

Every linear character of the upper-triangular subgroup $B\leq SL_2(\mathbb F_q)$ with $q\geq4$ is obtained from a multiplicative character $\theta$ of $\mathbb F_q^\times$. Its induction to $SL_2(\mathbb F_q)$ is irreducible exactly when $\theta^2\ne1$.

### Square orbits of additive characters of a finite field

↑ **Parent:** [Induced representation](#induced-representation)

The diagonal subgroup of $SL_2(\mathbb F_p)$ conjugates $u(x)$ to $u(a^2x)$. It therefore has two orbits, each of size $(p-1)/2$, on the nontrivial characters $\chi(v\mathbin\cdot)$ of the unipotent subgroup: one indexed by squares and one by nonsquares.

#### Induction from the diagonal subgroup of upper-triangular SL2

↑ **Parent:** [Square orbits of additive characters of a finite field](#square-orbits-of-additive-characters-of-a-finite-field)

If $B=U\rtimes T$ is the upper-triangular subgroup of $SL_2(\mathbb F_p)$ and $\theta$ is one-dimensional on $T$, then

$$
\operatorname{Ind}_T^B\theta
$$

is the direct sum of three pairwise nonisomorphic irreducibles. Their restrictions to $U$ have character supports given by the trivial character, the square orbit, and the nonsquare orbit, so their dimensions are $1,(p-1)/2,(p-1)/2$.

## Irreducible representation

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Irreducible_representation)

An irreducible [group representation](#group-representation) is nonzero and has no nonzero proper [invariant subspace](#invariant-subspace). These are the pieces that cannot be decomposed further by taking a smaller symmetry-preserved [vector space](vector-space.md).

The real two-dimensional rotation through $120$ degrees illustrates the role of the coefficient [field](algebra.md#field). A one-dimensional real [invariant subspace](#invariant-subspace) would supply a real [eigenvector](linear-operator-theory.md#eigenvector), but the characteristic polynomial $\lambda^2+\lambda+1$ has no real root. The [representation](#group-representation) is therefore irreducible over the [real numbers](arithmetic.md#real-number). Over the [complex numbers](complex-analysis.md#complex-number), that polynomial has distinct [roots of unity](algebra.md#root-of-unity) $e^{2\pi i/3}$ and $e^{-2\pi i/3}$, giving two invariant [eigenlines](linear-operator-theory.md#eigenline). Irreducibility over the [real numbers](arithmetic.md#real-number) does not imply [absolute irreducibility](#absolute-irreducibility-of-a-group-representation).

### Totally symmetric representation

↑ **Parent:** [Irreducible representation](#irreducible-representation)

The one-dimensional [trivial representation](#trivial-representation), in which every symmetry operation acts as $+1$. An integral over a symmetry-invariant domain can be nonzero only when its integrand contains such a component. Molecular [character tables](#character-table) often label it $A_1$ or $A_g$.

### Absolute irreducibility of a group representation

↑ **Parent:** [Irreducible representation](#irreducible-representation)

A [group representation](#group-representation) over a [field](algebra.md#field) is absolutely [irreducible](#irreducible-representation) if it remains [irreducible](#irreducible-representation) after every [field extension](algebra.md#field-extension). For a finite-dimensional [representation](#group-representation) it is enough to check an [algebraic closure](algebra.md#algebraic-closure). Irreducibility over the original [field](algebra.md#field) alone is weaker: the two-dimensional real rotation [representation](#group-representation) of the cyclic group of order three splits into two lines over the complex numbers.

### Absolutely irreducible real representation

↑ **Parent:** [Irreducible representation](#irreducible-representation)

A real [group representation](#group-representation) is absolutely irreducible if its complexification is irreducible. For a finite group this is equivalent to having only scalar real endomorphisms commuting with the representation. Independent coordinate sign changes force a commuting matrix to be diagonal; a transitive cyclic permutation of the coordinates then forces its entries equal. Alternatively, the coordinate projections and the cyclic permutation directly prove irreducibility over either field.

### Eigenvalue orbit under conjugation

↑ **Parent:** [Irreducible representation](#irreducible-representation)

If conjugation sends an operator to its inverse, the conjugating element sends its $\lambda$-eigenspace to the $\lambda^{-1}$-eigenspace.

### Irreducible complex representations of a finite dihedral group

↑ **Parent:** [Irreducible representation](#irreducible-representation)

For $D_{2n}=\langle r,s:r^n=s^2=1,\ srs=r^{-1}\rangle$, every irreducible complex representation has degree at most two. If $v$ is an eigenvector of $r$ with eigenvalue $\lambda$, then $sv$ has eigenvalue $\lambda^{-1}$, so irreducibility makes the representation equal to $\operatorname{span}\{v,sv\}$.

#### Two-dimensional representations of a finite dihedral group

↑ **Parent:** [Irreducible complex representations of a finite dihedral group](#irreducible-complex-representations-of-a-finite-dihedral-group)

For $\omega=e^{2\pi i/n}$ and $1\leq j<n/2$, define

$$
r\longmapsto
\begin{pmatrix}\omega^j&0\\0&\omega^{-j}\end{pmatrix},
\qquad
s\longmapsto
\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

These representations are irreducible and pairwise nonisomorphic. They give all two-dimensional irreducibles: $(n-1)/2$ of them for odd $n$, and $n/2-1$ for even $n$.

##### Faithful irreducible representation of D8

↑ **Parent:** [Two-dimensional representations of a finite dihedral group](#two-dimensional-representations-of-a-finite-dihedral-group)

For $D_8=\langle r,s:r^4=s^2=1,\ srs=r^{-1}\rangle$, the matrices

$$
r\longmapsto
\begin{pmatrix}i&0\\0&-i\end{pmatrix},
\qquad
s\longmapsto
\begin{pmatrix}0&1\\1&0\end{pmatrix}
$$

define a faithful irreducible two-dimensional complex representation.

## Infinite dihedral group

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Infinite_dihedral_group)

The infinite dihedral group is $\langle r,t\mid t^2=1,\ trt^{-1}=r^{-1}\rangle$.

### Representation of the infinite dihedral group

↑ **Parent:** [Infinite dihedral group](#infinite-dihedral-group)

Its irreducible complex representations have dimension at most two; the two-dimensional family pairs eigenvalues $\lambda$ and $\lambda^{-1}$ of the rotation generator.

#### Nonfaithful representations of the infinite dihedral group

↑ **Parent:** [Representation of the infinite dihedral group](#representation-of-the-infinite-dihedral-group)

Every nonfaithful finite-dimensional complex representation of the infinite dihedral group is a direct sum of subrepresentations of dimension at most two. Its kernel contains a nonzero power of the rotation, so the representation factors through a [finite dihedral group](finite-group-theory.md#dihedral-group). [Maschke's theorem](#maschke-s-theorem) makes that quotient representation semisimple, and all [irreducible complex representations of a finite dihedral group](#irreducible-complex-representations-of-a-finite-dihedral-group) have dimension at most two.

#### Quadratic-polynomial representation of the infinite dihedral group

↑ **Parent:** [Representation of the infinite dihedral group](#representation-of-the-infinite-dihedral-group)

Let the rotation and reflection generators act on polynomials of degree at most two by

$$
(Tp)(x)=p(x+1),
\qquad
(Sp)(x)=p(-x).
$$

Then $S^2=I$ and $STS=T^{-1}$. The operator $T$ has one size-three unipotent [Jordan block](linear-operator-theory.md#jordan-block), so this three-dimensional representation cannot split into invariant subspaces of dimension at most two.

#### Induced two-dimensional dihedral representation

↑ **Parent:** [Representation of the infinite dihedral group](#representation-of-the-infinite-dihedral-group)

For $\lambda\ne\pm1$, the rotation acts by $\operatorname{diag}(\lambda,\lambda^{-1})$ and the reflection interchanges the two eigenlines.

## One-dimensional character

↑ **Parent:** [Representation theory](representation-theory.md)

A one-dimensional character is a [character of a representation](#character-of-a-representation) arising from a one-dimensional representation, equivalently a homomorphism from a group to the multiplicative group of its scalar field.

### One-dimensional characters factor through the abelianization

↑ **Parent:** [One-dimensional character](#one-dimensional-character)

Every [one-dimensional character](#one-dimensional-character) kills the [commutator subgroup](group-theory.md#commutator-subgroup) and therefore factors through the [abelianization](group-theory.md#abelianization). Conversely, every character of the abelianization pulls back to a one-dimensional character of the group.

## Finite quotient representation

↑ **Parent:** [Representation theory](representation-theory.md)

A representation factors through a finite quotient exactly when its kernel contains the defining kernel of that quotient.

## Indecomposable representation

↑ **Parent:** [Representation theory](representation-theory.md)

An indecomposable representation is nonzero and cannot be expressed as a [direct sum](vector-space.md#direct-sum) of two nonzero invariant subspaces. It is an [indecomposable module](module-theory.md#indecomposable-module) over the associated [group algebra](associative-algebra.md#group-algebra) or representing algebra.

### Nonsplit extension of representations

↑ **Parent:** [Indecomposable representation](#indecomposable-representation)

A nonsplit extension contains an invariant subrepresentation with no invariant complementary subspace.

#### Split extension as a degeneration

↑ **Parent:** [Nonsplit extension of representations](#nonsplit-extension-of-representations)

An extension's vertexwise split arrow matrices are $\left(\begin{smallmatrix}f_X&\xi\\0&f_Z\end{smallmatrix}\right)$. Scaling the subobject by $t$ multiplies $\xi$ by $t$. Nonzero $t$ preserves the middle isomorphism class; $t=0$ gives $X\oplus Z$. For a nonsplit extension, the split orbit is distinct and lies in the smaller-dimensional boundary of the middle orbit closure.

### Unipotent representation

↑ **Parent:** [Indecomposable representation](#indecomposable-representation)

A unipotent operator has every eigenvalue equal to one and may create a nonsplit Jordan-block extension.

## ↑ Ancestors (4)

1. [Algebra](algebra.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Ferdinand Georg Frobenius](mathematics.md#ferdinand-georg-frobenius)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-302.md#1/solution)
