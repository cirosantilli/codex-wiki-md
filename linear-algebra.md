# Linear algebra

↑ **Parent:** [Algebra](algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_algebra)

**Table of contents**

- [Hyperbolic pair](#hyperbolic-pair)
- [Cartesian basis](#cartesian-basis)
- [Bilinear form](#bilinear-form)
  - [Orthogonal complement for a bilinear form](#orthogonal-complement-for-a-bilinear-form)
  - [Isometry of a space with a form](#isometry-of-a-space-with-a-form)
    - [Anisotropic vector for a form](#anisotropic-vector-for-a-form)
    - [Witt's theorem](#witt-s-theorem)
  - [Positive-definite bilinear form](#positive-definite-bilinear-form)
    - [Positive definiteness](#positive-definiteness)
  - [Alternating bilinear form](#alternating-bilinear-form)
  - [Symmetric bilinear form](#symmetric-bilinear-form)
    - [Modified trace form on real matrices](#modified-trace-form-on-real-matrices)
    - [Witt group of a field](#witt-group-of-a-field)
  - [Bounded bilinear form](#bounded-bilinear-form)
    - [Grothendieck inequality](#grothendieck-inequality)
      - [Grothendieck theorem for L1 to Hilbert operators](#grothendieck-theorem-for-l1-to-hilbert-operators)
        - [Rademacher span is not complemented in L1](#rademacher-span-is-not-complemented-in-l1)
    - [Boundedness criterion for a bilinear form](#boundedness-criterion-for-a-bilinear-form)
  - [Coercive bilinear form](#coercive-bilinear-form)
  - [Degenerate bilinear form](#degenerate-bilinear-form)
  - [Radical of a bilinear form](#radical-of-a-bilinear-form)
  - [Nondegenerate bilinear form](#nondegenerate-bilinear-form)
    - [Dual isomorphisms induced by a nondegenerate pairing](#dual-isomorphisms-induced-by-a-nondegenerate-pairing)
    - [Symplectic vector space](#symplectic-vector-space)
      - [Symplectic linear map](#symplectic-linear-map)
      - [Symplectic subspace](#symplectic-subspace)
        - [Orientation criterion for a graph of symplectic planes](#orientation-criterion-for-a-graph-of-symplectic-planes)
      - [Eigenspaces of a symplectic involution](#eigenspaces-of-a-symplectic-involution)
      - [Symplectic orthogonal complement](#symplectic-orthogonal-complement)
      - [Isotropic subspace of a symplectic vector space](#isotropic-subspace-of-a-symplectic-vector-space)
      - [Symplectic basis](#symplectic-basis)
    - [Representation of a bilinear form relative to a nondegenerate bilinear form](#representation-of-a-bilinear-form-relative-to-a-nondegenerate-bilinear-form)
  - [Inertia of a bilinear form](#inertia-of-a-bilinear-form)
    - [Signature pair of a real symmetric bilinear form](#signature-pair-of-a-real-symmetric-bilinear-form)
- [Sesquilinear form](#sesquilinear-form)
  - [Orthogonal complement for a sesquilinear form](#orthogonal-complement-for-a-sesquilinear-form)
  - [Hermitian form](#hermitian-form)
    - [Hermitian form over a quadratic finite field](#hermitian-form-over-a-quadratic-finite-field)
      - [Hermitian hyperbolic plane over a finite field](#hermitian-hyperbolic-plane-over-a-finite-field)
      - [Orthonormalization of a finite-field Hermitian form](#orthonormalization-of-a-finite-field-hermitian-form)
    - [Monomial orthonormal basis on the unit torus](#monomial-orthonormal-basis-on-the-unit-torus)
    - [Radical of a Hermitian form](#radical-of-a-hermitian-form)
    - [Positive semidefinite Hermitian form](#positive-semidefinite-hermitian-form)
    - [Indefinite Hermitian form](#indefinite-hermitian-form)
    - [Matrix of a Hermitian form](#matrix-of-a-hermitian-form)
- [Vector space](vector-space.md)
  - [Sequence space](vector-space.md#sequence-space)
  - [Zero vector](vector-space.md#zero-vector)
  - [Vector space over the rational numbers](vector-space.md#vector-space-over-the-rational-numbers)
  - [Antilinear map](vector-space.md#antilinear-map)
    - [Quaternionic structure on a complex vector space](vector-space.md#quaternionic-structure-on-a-complex-vector-space)
    - [Antiunitary operator](vector-space.md#antiunitary-operator)
  - [Complex vector space](vector-space.md#complex-vector-space)
  - [Real vector space](vector-space.md#real-vector-space)
    - [Majorization](vector-space.md#majorization)
      - [Majorization of summable sequences](vector-space.md#majorization-of-summable-sequences)
        - [Doubly stochastic realization of summable-sequence majorization](vector-space.md#doubly-stochastic-realization-of-summable-sequence-majorization)
  - [Vector space over a finite field](vector-space.md#vector-space-over-a-finite-field)
    - [Finite-field Kakeya set](vector-space.md#finite-field-kakeya-set)
      - [Tangent-line finite-field Kakeya construction](vector-space.md#tangent-line-finite-field-kakeya-construction)
      - [Finite-field Kakeya polynomial bound](vector-space.md#finite-field-kakeya-polynomial-bound)
  - [Linear span](vector-space.md#linear-span)
    - [Spanning set](vector-space.md#spanning-set)
  - [Quotient vector space](vector-space.md#quotient-vector-space)
    - [Parallel lines as a quotient vector space](vector-space.md#parallel-lines-as-a-quotient-vector-space)
  - [Vector subspace](vector-space.md#vector-subspace)
    - [Proper vector subspace](vector-space.md#proper-vector-subspace)
    - [Flag (linear algebra)](vector-space.md#flag-linear-algebra)
      - [Complete flag](vector-space.md#complete-flag)
    - [Fixed coordinate subspace](vector-space.md#fixed-coordinate-subspace)
    - [Intersection of vector subspaces](vector-space.md#intersection-of-vector-subspaces)
    - [Sum of vector subspaces](vector-space.md#sum-of-vector-subspaces)
    - [Hyperplane](vector-space.md#hyperplane)
    - [Closed vector subspace](vector-space.md#closed-vector-subspace)
      - [Positive distance between a unit sphere and a disjoint finite-dimensional subspace](vector-space.md#positive-distance-between-a-unit-sphere-and-a-disjoint-finite-dimensional-subspace)
  - [Affine subspace](vector-space.md#affine-subspace)
    - [Affine hull](vector-space.md#affine-hull)
    - [Affine hyperplane](vector-space.md#affine-hyperplane)
    - [Affine line in a vector space](vector-space.md#affine-line-in-a-vector-space)
  - [Linear combination](vector-space.md#linear-combination)
    - [Coefficient](vector-space.md#coefficient)
  - [Scalar multiplication](vector-space.md#scalar-multiplication)
    - [Scalar multiple](vector-space.md#scalar-multiple)
  - [Dimension (vector space)](vector-space.md#dimension-vector-space)
    - [Finite-dimensional vector space](vector-space.md#finite-dimensional-vector-space)
    - [Infinite-dimensional vector space](vector-space.md#infinite-dimensional-vector-space)
  - [Direct sum](vector-space.md#direct-sum)
    - [Common plane for three pairwise complementary subspaces](vector-space.md#common-plane-for-three-pairwise-complementary-subspaces)
    - [Orthogonal direct sum](vector-space.md#orthogonal-direct-sum)
    - [Direct summand](vector-space.md#direct-summand)
      - [Unimodular basis test for an integer direct summand](vector-space.md#unimodular-basis-test-for-an-integer-direct-summand)
    - [Dimension formula for a sum of subspaces](vector-space.md#dimension-formula-for-a-sum-of-subspaces)
    - [Direct-sum complement](vector-space.md#direct-sum-complement)
  - [Linear independence](vector-space.md#linear-independence)
    - [Minimally dependent vector family](vector-space.md#minimally-dependent-vector-family)
      - [Distinct diagonal weights break a first column dependence](vector-space.md#distinct-diagonal-weights-break-a-first-column-dependence)
    - [Linear dependence](vector-space.md#linear-dependence)
      - [Linear relation](vector-space.md#linear-relation)
  - [Basis](vector-space.md#basis)
    - [Basis vector](vector-space.md#basis-vector)
    - [Adjacent sums of a cyclic basis](vector-space.md#adjacent-sums-of-a-cyclic-basis)
    - [Basis extension](vector-space.md#basis-extension)
    - [Standard basis](vector-space.md#standard-basis)
    - [Steinitz exchange lemma](vector-space.md#steinitz-exchange-lemma)
    - [Monomial basis](vector-space.md#monomial-basis)
  - [Vector](vector-space.md#vector)
    - [Pseudovector](vector-space.md#pseudovector)
    - [Polar vector](vector-space.md#polar-vector)
    - [Euclidean vector](vector-space.md#euclidean-vector)
    - [Unit vector](vector-space.md#unit-vector)
    - [Cross product](vector-space.md#cross-product)
  - [Scalar](vector-space.md#scalar)
  - [Linear map](vector-space.md#linear-map)
    - [Zero-composition subspaces of a linear map](vector-space.md#zero-composition-subspaces-of-a-linear-map)
    - [One-sided inverses of finite-dimensional endomorphisms](vector-space.md#one-sided-inverses-of-finite-dimensional-endomorphisms)
    - [Rank of a linear map](vector-space.md#rank-of-a-linear-map)
      - [Rank bounds for a sum of linear maps](vector-space.md#rank-bounds-for-a-sum-of-linear-maps)
    - [Transvection](vector-space.md#transvection)
      - [Transvection conjugacy over a finite field](vector-space.md#transvection-conjugacy-over-a-finite-field)
      - [Elementary transvection matrix](vector-space.md#elementary-transvection-matrix)
        - [Transvections generate the special linear group](vector-space.md#transvections-generate-the-special-linear-group)
    - [Shear mapping](vector-space.md#shear-mapping)
    - [Uniform dilation](vector-space.md#uniform-dilation)
    - [Complex-linear map](vector-space.md#complex-linear-map)
    - [Image of a linear map](vector-space.md#image-of-a-linear-map)
      - [Image obstruction by an annihilating functional](vector-space.md#image-obstruction-by-an-annihilating-functional)
    - [Surjective linear map](vector-space.md#surjective-linear-map)
    - [First isomorphism theorem for vector spaces](vector-space.md#first-isomorphism-theorem-for-vector-spaces)
    - [Linear isomorphism](vector-space.md#linear-isomorphism)
    - [Linear function](vector-space.md#linear-function)
      - [Affine function](vector-space.md#affine-function)
    - [Linearity](vector-space.md#linearity)
    - [Superposition principle](vector-space.md#superposition-principle)
    - [Linear operator](vector-space.md#linear-operator)
      - [Semisimple linear operator](vector-space.md#semisimple-linear-operator)
      - [Locally nilpotent operator](vector-space.md#locally-nilpotent-operator)
        - [Algebraic exponential of a locally nilpotent operator](vector-space.md#algebraic-exponential-of-a-locally-nilpotent-operator)
      - [Operator commutator](vector-space.md#operator-commutator)
      - [Multiplication operator](vector-space.md#multiplication-operator)
        - [Spectrum of a real multiplication operator](vector-space.md#spectrum-of-a-real-multiplication-operator)
      - [Projection (linear algebra)](vector-space.md#projection-linear-algebra)
        - [Kadec-Snobar projection bound](vector-space.md#kadec-snobar-projection-bound)
        - [Inner product adapted to an idempotent linear map](vector-space.md#inner-product-adapted-to-an-idempotent-linear-map)
        - [Similarity classification of idempotent linear maps](vector-space.md#similarity-classification-of-idempotent-linear-maps)
        - [Oblique projection](vector-space.md#oblique-projection)
          - [Finite-dimensional Hilbert sampling reconstruction](vector-space.md#finite-dimensional-hilbert-sampling-reconstruction)
      - [Operator domain](vector-space.md#operator-domain)
        - [Densely defined operator](vector-space.md#densely-defined-operator)
      - [Identity operator](vector-space.md#identity-operator)
      - [Composition operator](vector-space.md#composition-operator)
        - [Invariant functional of a composition operator](vector-space.md#invariant-functional-of-a-composition-operator)
      - [Unitary operator](vector-space.md#unitary-operator)
        - [Unitary equivalence](vector-space.md#unitary-equivalence)
        - [Eigenphase](vector-space.md#eigenphase)
        - [Unitary conjugation](vector-space.md#unitary-conjugation)
        - [Von Neumann mean ergodic theorem](vector-space.md#von-neumann-mean-ergodic-theorem)
          - [Orthogonal decomposition for unitary ergodic averages](vector-space.md#orthogonal-decomposition-for-unitary-ergodic-averages)
      - [Commuting operators](vector-space.md#commuting-operators)
        - [Commuting maps preserve eigenspaces](vector-space.md#commuting-maps-preserve-eigenspaces)
      - [Anticommutator](vector-space.md#anticommutator)
        - [Two-by-two anticommutator characteristic polynomial](vector-space.md#two-by-two-anticommutator-characteristic-polynomial)
      - [Conjugate linear operators](vector-space.md#conjugate-linear-operators)
        - [Conjugation operator on an endomorphism space](vector-space.md#conjugation-operator-on-an-endomorphism-space)
    - [Matrix](vector-space.md#matrix)
      - [Cauchy matrix](vector-space.md#cauchy-matrix)
      - [Matrix norm](vector-space.md#matrix-norm)
      - [Matrix pencil](vector-space.md#matrix-pencil)
      - [Total nonnegativity of a matrix](vector-space.md#total-nonnegativity-of-a-matrix)
        - [Checkerboard inverse of a totally nonnegative matrix](vector-space.md#checkerboard-inverse-of-a-totally-nonnegative-matrix)
      - [Elementary column operation](vector-space.md#elementary-column-operation)
      - [Hadamard matrix](vector-space.md#hadamard-matrix)
      - [Square matrix](vector-space.md#square-matrix)
      - [Realification of a complex matrix](vector-space.md#realification-of-a-complex-matrix)
        - [Realification determinant identity](vector-space.md#realification-determinant-identity)
      - [Entrywise matrix L1 norm](vector-space.md#entrywise-matrix-l1-norm)
      - [Entrywise matrix function](vector-space.md#entrywise-matrix-function)
      - [Hadamard product](vector-space.md#hadamard-product)
        - [Hadamard power](vector-space.md#hadamard-power)
      - [Hermite normal form](vector-space.md#hermite-normal-form)
        - [Row lattice of an integer matrix](vector-space.md#row-lattice-of-an-integer-matrix)
        - [Row Hermite normal form in rank two](vector-space.md#row-hermite-normal-form-in-rank-two)
      - [Doubly stochastic matrix](vector-space.md#doubly-stochastic-matrix)
        - [Two-coordinate stochastic averaging](vector-space.md#two-coordinate-stochastic-averaging)
        - [Birkhoff-von Neumann theorem](vector-space.md#birkhoff-von-neumann-theorem)
          - [Birkhoff decomposition by support matchings](vector-space.md#birkhoff-decomposition-by-support-matchings)
          - [Alternating-cycle perturbation of a doubly stochastic matrix](vector-space.md#alternating-cycle-perturbation-of-a-doubly-stochastic-matrix)
      - [Rational matrix](vector-space.md#rational-matrix)
      - [Nonnegative matrix](vector-space.md#nonnegative-matrix)
        - [Irreducible nonnegative matrix](vector-space.md#irreducible-nonnegative-matrix)
          - [Primitive nonnegative matrix](vector-space.md#primitive-nonnegative-matrix)
        - [Perron–Frobenius theorem](vector-space.md#perron-frobenius-theorem)
      - [All-ones matrix](vector-space.md#all-ones-matrix)
      - [Row and column spaces](vector-space.md#row-and-column-spaces)
        - [Row space](vector-space.md#row-space)
        - [Column space](vector-space.md#column-space)
      - [Binary matrix](vector-space.md#binary-matrix)
      - [Submatrix](vector-space.md#submatrix)
        - [Minor (linear algebra)](vector-space.md#minor-linear-algebra)
          - [Principal minor](vector-space.md#principal-minor)
      - [Entrywise maximum norm](vector-space.md#entrywise-maximum-norm)
      - [Tridiagonal matrix](vector-space.md#tridiagonal-matrix)
      - [Block matrix](vector-space.md#block-matrix)
        - [Block diagonal matrix](vector-space.md#block-diagonal-matrix)
        - [Block tridiagonal matrix](vector-space.md#block-tridiagonal-matrix)
      - [Diagonally dominant matrix](vector-space.md#diagonally-dominant-matrix)
        - [Strictly diagonally dominant matrix](vector-space.md#strictly-diagonally-dominant-matrix)
          - [Inverse infinity-norm bound from diagonal dominance](vector-space.md#inverse-infinity-norm-bound-from-diagonal-dominance)
      - [Transpose](vector-space.md#transpose)
      - [Matrix logarithm](vector-space.md#matrix-logarithm)
        - [Analytic determinant square root for accretive symmetric matrices](vector-space.md#analytic-determinant-square-root-for-accretive-symmetric-matrices)
        - [Diagonal logarithm concavity bound](vector-space.md#diagonal-logarithm-concavity-bound)
        - [Existence of a logarithm for every invertible complex matrix](vector-space.md#existence-of-a-logarithm-for-every-invertible-complex-matrix)
        - [Klein's inequality](vector-space.md#klein-s-inequality)
      - [Matrix power](vector-space.md#matrix-power)
      - [Matrix element](vector-space.md#matrix-element)
      - [Sparse matrix](vector-space.md#sparse-matrix)
        - [Compressed sparse storage](vector-space.md#compressed-sparse-storage)
        - [Matrix bandwidth](vector-space.md#matrix-bandwidth)
      - [Matrix unit](vector-space.md#matrix-unit)
      - [Matrix rank](vector-space.md#matrix-rank)
        - [Rank bound for a matrix product](vector-space.md#rank-bound-for-a-matrix-product)
        - [Column rank](vector-space.md#column-rank)
        - [Row rank](vector-space.md#row-rank)
        - [Rank orbit of a matrix under left-right multiplication](vector-space.md#rank-orbit-of-a-matrix-under-left-right-multiplication)
        - [Subadditivity of matrix rank](vector-space.md#subadditivity-of-matrix-rank)
        - [Full column rank](vector-space.md#full-column-rank)
        - [Full row rank](vector-space.md#full-row-rank)
      - [Identity matrix](vector-space.md#identity-matrix)
      - [Rank-one matrix](vector-space.md#rank-one-matrix)
      - [Bidiagonal matrix](vector-space.md#bidiagonal-matrix)
        - [Upper bidiagonal matrix](vector-space.md#upper-bidiagonal-matrix)
      - [Matrix multiplication](vector-space.md#matrix-multiplication)
        - [Matrix product](vector-space.md#matrix-product)
        - [Outer product](vector-space.md#outer-product)
      - [Hessenberg matrix](vector-space.md#hessenberg-matrix)
        - [Upper Hessenberg matrix](vector-space.md#upper-hessenberg-matrix)
      - [Permutation matrix](vector-space.md#permutation-matrix)
        - [Signed permutation matrix](vector-space.md#signed-permutation-matrix)
      - [Matrix representation of a linear map](vector-space.md#matrix-representation-of-a-linear-map)
      - [Kronecker product](vector-space.md#kronecker-product)
        - [Kronecker sum](vector-space.md#kronecker-sum)
- [Singular value decomposition](#singular-value-decomposition)
  - [Autonne-Takagi factorization](#autonne-takagi-factorization)
  - [Singular value](#singular-value)
    - [Right singular vector](#right-singular-vector)
    - [Left singular vector](#left-singular-vector)
- [Unimodular matrix](#unimodular-matrix)
- [Householder transformation](#householder-transformation)
- [Change of basis](#change-of-basis)
  - [Change-of-basis matrix](#change-of-basis-matrix)
- [Circulant matrix](#circulant-matrix)
- [Invertible matrix](#invertible-matrix)
  - [Singular matrix](#singular-matrix)
- [Kernel of a linear map](#kernel-of-a-linear-map)
  - [Nullity of a linear map](#nullity-of-a-linear-map)
  - [Trivial kernel](#trivial-kernel)
  - [Rank-nullity theorem](#rank-nullity-theorem)
    - [Equality in the rank-sum and nullity-product inequalities](#equality-in-the-rank-sum-and-nullity-product-inequalities)
    - [Kernel jump in a parameter-dependent linear map](#kernel-jump-in-a-parameter-dependent-linear-map)
- [Cokernel](#cokernel)
- [Dual space](#dual-space)
  - [Algebraic dual of a direct sum](#algebraic-dual-of-a-direct-sum)
  - [Bidual of a normed space](#bidual-of-a-normed-space)
  - [Perfect pairing](#perfect-pairing)
  - [Separating subspace of an algebraic dual](#separating-subspace-of-an-algebraic-dual)
  - [Bidual evaluation map](#bidual-evaluation-map)
  - [Covector](#covector)
  - [Linear functional](#linear-functional)
    - [Minimizing a linear functional on a sphere](#minimizing-a-linear-functional-on-a-sphere)
    - [Discontinuous functional detected by vanishing sequence tails](#discontinuous-functional-detected-by-vanishing-sequence-tails)
  - [Dual basis](#dual-basis)
    - [Factorial monomial basis for polynomial differentiation](#factorial-monomial-basis-for-polynomial-differentiation)
  - [Annihilator of a vector subspace](#annihilator-of-a-vector-subspace)
  - [Transpose of a linear map](#transpose-of-a-linear-map)
    - [Dual image and kernel annihilator identity](#dual-image-and-kernel-annihilator-identity)
    - [Equality of row rank and column rank](#equality-of-row-rank-and-column-rank)
      - [Simultaneous basis exchange from a nonzero minor](#simultaneous-basis-exchange-from-a-nonzero-minor)
    - [Duals of a subspace and its quotient](#duals-of-a-subspace-and-its-quotient)
  - [Surjectivity of independent linear functionals](#surjectivity-of-independent-linear-functionals)
  - [Polynomial moment functional](#polynomial-moment-functional)
- [Rank of a matrix with affine columns](#rank-of-a-matrix-with-affine-columns)
- [Matrix determinant lemma](#matrix-determinant-lemma)
- [Permanent (mathematics)](#permanent-mathematics)
  - [Dense permanent approximation](#dense-permanent-approximation)
- [Matrix inverse](#matrix-inverse)
  - [Block matrix inverse](#block-matrix-inverse)
  - [Sherman–Morrison formula](#sherman-morrison-formula)
  - [Moore-Penrose inverse](#moore-penrose-inverse)
    - [Moore--Penrose inverse of a Hilbert-space operator](#moore-penrose-inverse-of-a-hilbert-space-operator)
    - [Penrose equations](#penrose-equations)
    - [Reverse-order law for the Moore--Penrose inverse](#reverse-order-law-for-the-moore-penrose-inverse)
  - [Push-through identity](#push-through-identity)
- [Matrix similarity](#matrix-similarity)
  - [Similarity transformation](#similarity-transformation)
    - [Positive diagonal symmetrization of a matrix](#positive-diagonal-symmetrization-of-a-matrix)
    - [Every automorphism of a full matrix algebra is inner](#every-automorphism-of-a-full-matrix-algebra-is-inner)
  - [Transpose similarity](#transpose-similarity)
  - [Real similarity from complex similarity](#real-similarity-from-complex-similarity)
- [Matrix trace](#matrix-trace)
  - [Scalar square of a traceless two-by-two matrix](#scalar-square-of-a-traceless-two-by-two-matrix)
  - [Nilpotence from vanishing traces of powers](#nilpotence-from-vanishing-traces-of-powers)
  - [Trace orthogonality nilpotence lemma](#trace-orthogonality-nilpotence-lemma)
  - [Trace is the unique normalized cyclic linear functional](#trace-is-the-unique-normalized-cyclic-linear-functional)
  - [Traceless matrix](#traceless-matrix)
    - [Traceless matrices are spanned by commutators](#traceless-matrices-are-spanned-by-commutators)
  - [Cyclic property of the trace](#cyclic-property-of-the-trace)
- [Operator theory](linear-operator-theory.md)
  - [Polar decomposition](linear-operator-theory.md#polar-decomposition)
  - [Shift operator](linear-operator-theory.md#shift-operator)
    - [Unilateral shift operator](linear-operator-theory.md#unilateral-shift-operator)
      - [Left shift operator](linear-operator-theory.md#left-shift-operator)
      - [Point spectrum](linear-operator-theory.md#point-spectrum)
      - [Wandering-vector characterization of a unilateral shift](linear-operator-theory.md#wandering-vector-characterization-of-a-unilateral-shift)
  - [Solvability condition](linear-operator-theory.md#solvability-condition)
  - [Spectrum (functional analysis)](linear-operator-theory.md#spectrum-functional-analysis)
    - [Approximate eigenvalue](linear-operator-theory.md#approximate-eigenvalue)
      - [Approximate eigenvector](linear-operator-theory.md#approximate-eigenvector)
    - [Residual spectrum](linear-operator-theory.md#residual-spectrum)
    - [Continuous spectrum](linear-operator-theory.md#continuous-spectrum)
    - [Spectrum of a bounded operator](linear-operator-theory.md#spectrum-of-a-bounded-operator)
  - [Compression of a linear operator](linear-operator-theory.md#compression-of-a-linear-operator)
  - [Self-adjoint operator](linear-operator-theory.md#self-adjoint-operator)
    - [Negative-energy direction gives exponential growth in a self-adjoint wave equation](linear-operator-theory.md#negative-energy-direction-gives-exponential-growth-in-a-self-adjoint-wave-equation)
    - [Friedrichs extension](linear-operator-theory.md#friedrichs-extension)
    - [Spectral Weyl sequence](linear-operator-theory.md#spectral-weyl-sequence)
      - [Singular Weyl sequence](linear-operator-theory.md#singular-weyl-sequence)
    - [Unbounded self-adjoint operator](linear-operator-theory.md#unbounded-self-adjoint-operator)
      - [Spectral positivity criterion for a self-adjoint operator](linear-operator-theory.md#spectral-positivity-criterion-for-a-self-adjoint-operator)
      - [Nonreal resolvent estimate for a self-adjoint operator](linear-operator-theory.md#nonreal-resolvent-estimate-for-a-self-adjoint-operator)
    - [Fredholm solvability condition for a self-adjoint operator](linear-operator-theory.md#fredholm-solvability-condition-for-a-self-adjoint-operator)
    - [Positive-definite operator](linear-operator-theory.md#positive-definite-operator)
      - [Strict operator positivity does not imply surjectivity](linear-operator-theory.md#strict-operator-positivity-does-not-imply-surjectivity)
    - [Finite-dimensional spectral theorem](linear-operator-theory.md#finite-dimensional-spectral-theorem)
      - [Multiplicity-free complete dyadic spectrum](linear-operator-theory.md#multiplicity-free-complete-dyadic-spectrum)
      - [Orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis)
    - [Laguerre differential operator on polynomials](linear-operator-theory.md#laguerre-differential-operator-on-polynomials)
      - [Laguerre polynomial](linear-operator-theory.md#laguerre-polynomial)
        - [Generalized Laguerre polynomial](linear-operator-theory.md#generalized-laguerre-polynomial)
          - [Rodrigues' formula](linear-operator-theory.md#rodrigues-formula)
  - [Real spectral theorem](linear-operator-theory.md#real-spectral-theorem)
  - [Power method](linear-operator-theory.md#power-method)
    - [Dominant eigenpair extraction from a two-step Krylov recurrence](linear-operator-theory.md#dominant-eigenpair-extraction-from-a-two-step-krylov-recurrence)
    - [Quadratic Rayleigh-quotient improvement for the power method](linear-operator-theory.md#quadratic-rayleigh-quotient-improvement-for-the-power-method)
    - [Active spectrum of the power method](linear-operator-theory.md#active-spectrum-of-the-power-method)
    - [Inverse iteration](linear-operator-theory.md#inverse-iteration)
      - [Convergence of fixed-shift inverse iteration](linear-operator-theory.md#convergence-of-fixed-shift-inverse-iteration)
        - [Sign behavior of fixed-shift inverse iteration](linear-operator-theory.md#sign-behavior-of-fixed-shift-inverse-iteration)
    - [Subspace iteration](linear-operator-theory.md#subspace-iteration)
      - [Dominant invariant subspace](linear-operator-theory.md#dominant-invariant-subspace)
      - [Power method with a dominant eigenvalue cluster](linear-operator-theory.md#power-method-with-a-dominant-eigenvalue-cluster)
  - [Characteristic polynomial](linear-operator-theory.md#characteristic-polynomial)
    - [Characteristic polynomials of AB and BA](linear-operator-theory.md#characteristic-polynomials-of-ab-and-ba)
    - [Faddeev–LeVerrier algorithm](linear-operator-theory.md#faddeev-leverrier-algorithm)
    - [Real parameter avoiding a singular matrix pencil](linear-operator-theory.md#real-parameter-avoiding-a-singular-matrix-pencil)
    - [Triangularization over an algebraically closed field](linear-operator-theory.md#triangularization-over-an-algebraically-closed-field)
  - [Eigenvalue interlacing](linear-operator-theory.md#eigenvalue-interlacing)
    - [Largest-eigenvalue interlacing for a principal submatrix](linear-operator-theory.md#largest-eigenvalue-interlacing-for-a-principal-submatrix)
  - [Jordan normal form](linear-operator-theory.md#jordan-normal-form)
    - [Unipotent involutions in characteristic two](linear-operator-theory.md#unipotent-involutions-in-characteristic-two)
    - [Density of diagonalizable complex matrices](linear-operator-theory.md#density-of-diagonalizable-complex-matrices)
    - [Repeated-eigenvalue classification in dimension two](linear-operator-theory.md#repeated-eigenvalue-classification-in-dimension-two)
    - [Jordan–Chevalley decomposition](linear-operator-theory.md#jordan-chevalley-decomposition)
      - [Adjoint compatibility of additive Jordan decomposition](linear-operator-theory.md#adjoint-compatibility-of-additive-jordan-decomposition)
        - [Semisimple matrix Lie algebras are closed under additive Jordan decomposition](linear-operator-theory.md#semisimple-matrix-lie-algebras-are-closed-under-additive-jordan-decomposition)
    - [Algebraic multiplicity](linear-operator-theory.md#algebraic-multiplicity)
    - [Geometric multiplicity](linear-operator-theory.md#geometric-multiplicity)
    - [Jordan block](linear-operator-theory.md#jordan-block)
      - [Square-root splitting of a defective double eigenvalue](linear-operator-theory.md#square-root-splitting-of-a-defective-double-eigenvalue)
      - [Nilpotent Jordan block](linear-operator-theory.md#nilpotent-jordan-block)
    - [Jordan normal form of conjugation on two-by-two matrices](linear-operator-theory.md#jordan-normal-form-of-conjugation-on-two-by-two-matrices)
    - [Characteristic and minimal polynomials determine similarity in dimension three](linear-operator-theory.md#characteristic-and-minimal-polynomials-determine-similarity-in-dimension-three)
    - [Generalized eigenvector](linear-operator-theory.md#generalized-eigenvector)
      - [Jordan chain](linear-operator-theory.md#jordan-chain)
        - [Length-two Jordan chain solution](linear-operator-theory.md#length-two-jordan-chain-solution)
      - [Generalized eigenspace](linear-operator-theory.md#generalized-eigenspace)
        - [Nilpotent commutator preserves generalized eigenspaces](linear-operator-theory.md#nilpotent-commutator-preserves-generalized-eigenspaces)
      - [Generalized eigenspaces for distinct eigenvalues form a direct sum](linear-operator-theory.md#generalized-eigenspaces-for-distinct-eigenvalues-form-a-direct-sum)
  - [Generalized eigenvalue problem](linear-operator-theory.md#generalized-eigenvalue-problem)
    - [Generalized characteristic polynomial](linear-operator-theory.md#generalized-characteristic-polynomial)
  - [Matrix exponential](linear-operator-theory.md#matrix-exponential)
    - [Skew-symmetric exponential as an axial rotation](linear-operator-theory.md#skew-symmetric-exponential-as-an-axial-rotation)
    - [Derivative of the matrix exponential](linear-operator-theory.md#derivative-of-the-matrix-exponential)
    - [Matrix exponential determinant identity](linear-operator-theory.md#matrix-exponential-determinant-identity)
    - [Matrix exponential when the square is minus the identity](linear-operator-theory.md#matrix-exponential-when-the-square-is-minus-the-identity)
    - [Baker--Campbell--Hausdorff formula](linear-operator-theory.md#baker-campbell-hausdorff-formula)
    - [Laplace transform of a matrix exponential](linear-operator-theory.md#laplace-transform-of-a-matrix-exponential)
  - [Minimal polynomial](linear-operator-theory.md#minimal-polynomial)
    - [Characteristic and minimal polynomials of right multiplication](linear-operator-theory.md#characteristic-and-minimal-polynomials-of-right-multiplication)
    - [Real matrices have real minimal polynomials](linear-operator-theory.md#real-matrices-have-real-minimal-polynomials)
    - [Integer powers for an annihilating polynomial with roots one and minus one](linear-operator-theory.md#integer-powers-for-an-annihilating-polynomial-with-roots-one-and-minus-one)
    - [Minimal polynomial of an invertible matrix](linear-operator-theory.md#minimal-polynomial-of-an-invertible-matrix)
    - [Minimal polynomials of AB and BA](linear-operator-theory.md#minimal-polynomials-of-ab-and-ba)
      - [Similarity of squared matrix products with one diagonalizable product](linear-operator-theory.md#similarity-of-squared-matrix-products-with-one-diagonalizable-product)
    - [Kernel decomposition for coprime polynomials](linear-operator-theory.md#kernel-decomposition-for-coprime-polynomials)
    - [Minimal polynomial bound from a triangular invariant flag](linear-operator-theory.md#minimal-polynomial-bound-from-a-triangular-invariant-flag)
  - [Jacobson lemma for a commuting commutator](linear-operator-theory.md#jacobson-lemma-for-a-commuting-commutator)
  - [Translation finite-difference operator](linear-operator-theory.md#translation-finite-difference-operator)
    - [Mixed finite difference of a polynomial](linear-operator-theory.md#mixed-finite-difference-of-a-polynomial)
  - [Nilpotent linear map](linear-operator-theory.md#nilpotent-linear-map)
    - [Nilpotent matrix](linear-operator-theory.md#nilpotent-matrix)
      - [Square-zero criterion for a two-by-two matrix](linear-operator-theory.md#square-zero-criterion-for-a-two-by-two-matrix)
      - [Counting nilpotent matrices by the Fitting decomposition](linear-operator-theory.md#counting-nilpotent-matrices-by-the-fitting-decomposition)
    - [Nilpotence of commutation by a nilpotent endomorphism](linear-operator-theory.md#nilpotence-of-commutation-by-a-nilpotent-endomorphism)
  - [Eigenvalue](linear-operator-theory.md#eigenvalue)
    - [Eigenvalue collision](linear-operator-theory.md#eigenvalue-collision)
    - [Spectral abscissa](linear-operator-theory.md#spectral-abscissa)
    - [Eigenvalue multiplicity](linear-operator-theory.md#eigenvalue-multiplicity)
    - [Zero eigenvalue](linear-operator-theory.md#zero-eigenvalue)
      - [Spectrum of a three-dimensional matrix with zero row sums](linear-operator-theory.md#spectrum-of-a-three-dimensional-matrix-with-zero-row-sums)
    - [Eigenvalue problem](linear-operator-theory.md#eigenvalue-problem)
    - [Eigenfunction](linear-operator-theory.md#eigenfunction)
      - [Nodeless eigenfunction](linear-operator-theory.md#nodeless-eigenfunction)
      - [Dirichlet eigenfunction](linear-operator-theory.md#dirichlet-eigenfunction)
      - [Adjoint eigenfunction](linear-operator-theory.md#adjoint-eigenfunction)
      - [Generalized eigenfunction](linear-operator-theory.md#generalized-eigenfunction)
    - [Eigenvector](linear-operator-theory.md#eigenvector)
      - [Zero mode](linear-operator-theory.md#zero-mode)
      - [Independence of eigenvectors for distinct eigenvalues](linear-operator-theory.md#independence-of-eigenvectors-for-distinct-eigenvalues)
      - [Eigenvalue equation](linear-operator-theory.md#eigenvalue-equation)
      - [Right eigenvector](linear-operator-theory.md#right-eigenvector)
      - [Left eigenvector](linear-operator-theory.md#left-eigenvector)
    - [Eigenspace](linear-operator-theory.md#eigenspace)
      - [Real square roots of operators with simple real spectrum](linear-operator-theory.md#real-square-roots-of-operators-with-simple-real-spectrum)
      - [Laplacian eigenspace](linear-operator-theory.md#laplacian-eigenspace)
      - [Eigenbasis](linear-operator-theory.md#eigenbasis)
    - [Simple eigenvalue](linear-operator-theory.md#simple-eigenvalue)
      - [Eigenvalue sensitivity](linear-operator-theory.md#eigenvalue-sensitivity)
        - [First-order perturbation of a simple eigenvalue](linear-operator-theory.md#first-order-perturbation-of-a-simple-eigenvalue)
    - [Diagonalizable matrix](linear-operator-theory.md#diagonalizable-matrix)
      - [Diagonalization of a matrix](linear-operator-theory.md#diagonalization-of-a-matrix)
      - [Diagonalizability inherited from an invertible power](linear-operator-theory.md#diagonalizability-inherited-from-an-invertible-power)
      - [Complex similarity of real matrices implies real similarity](linear-operator-theory.md#complex-similarity-of-real-matrices-implies-real-similarity)
      - [Distinct eigenvalues imply diagonalizability](linear-operator-theory.md#distinct-eigenvalues-imply-diagonalizability)
      - [Spectral decomposition](linear-operator-theory.md#spectral-decomposition)
        - [Dominant eigenvalue](linear-operator-theory.md#dominant-eigenvalue)
        - [Spectral gap](linear-operator-theory.md#spectral-gap)
          - [Ground-space perturbation bound](linear-operator-theory.md#ground-space-perturbation-bound)
          - [Davis-Kahan theorem](linear-operator-theory.md#davis-kahan-theorem)
            - [Davis-Kahan curvature lemma](linear-operator-theory.md#davis-kahan-curvature-lemma)
              - [Rank-one eigenprojector perturbation bound](linear-operator-theory.md#rank-one-eigenprojector-perturbation-bound)
  - [Conjugate transpose](linear-operator-theory.md#conjugate-transpose)
  - [Unitary matrix](linear-operator-theory.md#unitary-matrix)
    - [Hermitian parts of a unitary matrix](linear-operator-theory.md#hermitian-parts-of-a-unitary-matrix)
  - [Skew-Hermitian matrix](linear-operator-theory.md#skew-hermitian-matrix)
    - [Cross-product model of su(2)](linear-operator-theory.md#cross-product-model-of-su-2)
  - [Cayley transform of a Hermitian matrix](linear-operator-theory.md#cayley-transform-of-a-hermitian-matrix)
  - [Normal matrix](linear-operator-theory.md#normal-matrix)
    - [Normal matrices have equal adjoint norms](linear-operator-theory.md#normal-matrices-have-equal-adjoint-norms)
    - [Hoffman–Wielandt inequality](linear-operator-theory.md#hoffman-wielandt-inequality)
      - [Spectral Lipschitz bound from Frobenius distance](linear-operator-theory.md#spectral-lipschitz-bound-from-frobenius-distance)
    - [Adjoint eigenvector identity for a normal matrix](linear-operator-theory.md#adjoint-eigenvector-identity-for-a-normal-matrix)
    - [Normality criterion for a two-mode shear model](linear-operator-theory.md#normality-criterion-for-a-two-mode-shear-model)
    - [Matrix 2-norm of a normal matrix](linear-operator-theory.md#matrix-2-norm-of-a-normal-matrix)
    - [Non-normal matrix](linear-operator-theory.md#non-normal-matrix)
      - [Nonnormal eigenvalues do not bound a quadratic quotient](linear-operator-theory.md#nonnormal-eigenvalues-do-not-bound-a-quadratic-quotient)
      - [Transient growth](linear-operator-theory.md#transient-growth)
        - [Optimal initial state for triangular stable shear](linear-operator-theory.md#optimal-initial-state-for-triangular-stable-shear)
          - [Short-relative-time optimal state for triangular shear](linear-operator-theory.md#short-relative-time-optimal-state-for-triangular-shear)
        - [Instantaneous energy-growth criterion for a linear system](linear-operator-theory.md#instantaneous-energy-growth-criterion-for-a-linear-system)
        - [Optimal energy amplification of a linear system](linear-operator-theory.md#optimal-energy-amplification-of-a-linear-system)
        - [Two-dimensional triangular model of transient growth](linear-operator-theory.md#two-dimensional-triangular-model-of-transient-growth)
          - [Optimal time and gain of a Reynolds-scaled triangular model](linear-operator-theory.md#optimal-time-and-gain-of-a-reynolds-scaled-triangular-model)
          - [Orientation interval for transient energy growth](linear-operator-theory.md#orientation-interval-for-transient-energy-growth)
          - [Energy-neutral rotational nonlinearity](linear-operator-theory.md#energy-neutral-rotational-nonlinearity)
    - [Unitary diagonalization of a normal matrix](linear-operator-theory.md#unitary-diagonalization-of-a-normal-matrix)
  - [Schur decomposition](linear-operator-theory.md#schur-decomposition)
  - [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient)
    - [Rayleigh quotient with one Neumann endpoint](linear-operator-theory.md#rayleigh-quotient-with-one-neumann-endpoint)
    - [Hermitian Rayleigh quotient range](linear-operator-theory.md#hermitian-rayleigh-quotient-range)
    - [Odd variational trial gives an excited oscillator bound](linear-operator-theory.md#odd-variational-trial-gives-an-excited-oscillator-bound)
    - [Generalized Rayleigh quotient](linear-operator-theory.md#generalized-rayleigh-quotient)
    - [Rayleigh quotient iteration](linear-operator-theory.md#rayleigh-quotient-iteration)
      - [Local cubic convergence of Rayleigh quotient iteration](linear-operator-theory.md#local-cubic-convergence-of-rayleigh-quotient-iteration)
    - [Rayleigh-Ritz variational principle](linear-operator-theory.md#rayleigh-ritz-variational-principle)
      - [Odd-state variational principle for an even potential](linear-operator-theory.md#odd-state-variational-principle-for-an-even-potential)
      - [Gaussian variational bound for an attractive Gaussian well](linear-operator-theory.md#gaussian-variational-bound-for-an-attractive-gaussian-well)
      - [Finite-subspace variational method](linear-operator-theory.md#finite-subspace-variational-method)
        - [Two-mode variational bound for a linearly tilted square well](linear-operator-theory.md#two-mode-variational-bound-for-a-linearly-tilted-square-well)
  - [Cyclic vector](linear-operator-theory.md#cyclic-vector)
    - [Cyclic subspace](linear-operator-theory.md#cyclic-subspace)
  - [Companion matrix](linear-operator-theory.md#companion-matrix)
  - [Invariant direct-sum decomposition](linear-operator-theory.md#invariant-direct-sum-decomposition)
  - [Rational canonical form](linear-operator-theory.md#rational-canonical-form)
    - [Primary matrix centralizer formula](linear-operator-theory.md#primary-matrix-centralizer-formula)
      - [Counting matrices with a fixed primary polynomial](linear-operator-theory.md#counting-matrices-with-a-fixed-primary-polynomial)
    - [Invariant factors of a linear operator](linear-operator-theory.md#invariant-factors-of-a-linear-operator)
- [Multilinear algebra](#multilinear-algebra)
  - [Coalgebra](#coalgebra)
    - [Coideal](#coideal)
    - [Measuring coalgebra](#measuring-coalgebra)
      - [Universal measuring coalgebra](#universal-measuring-coalgebra)
    - [Group-like element](#group-like-element)
    - [Comodule](#comodule)
      - [Comodule tensor transformation formula](#comodule-tensor-transformation-formula)
        - [Multiplication compatibility for a comodule tensor transformation](#multiplication-compatibility-for-a-comodule-tensor-transformation)
      - [Corestriction functor for comodules](#corestriction-functor-for-comodules)
        - [Comodule natural transformation formula](#comodule-natural-transformation-formula)
      - [Coaction](#coaction)
    - [Convolution product for coalgebra maps](#convolution-product-for-coalgebra-maps)
    - [Sweedler notation](#sweedler-notation)
  - [Multilinear map](#multilinear-map)
    - [Bilinear map](#bilinear-map)
      - [Bilinearity](#bilinearity)
      - [Symmetric bilinear diagonal-parallel lemma](#symmetric-bilinear-diagonal-parallel-lemma)
      - [Derivative of a continuous bilinear map](#derivative-of-a-continuous-bilinear-map)
      - [Rank bound for a nonsingular complex bilinear map](#rank-bound-for-a-nonsingular-complex-bilinear-map)
      - [Complex bilinear dimension bound](#complex-bilinear-dimension-bound)
  - [Alternating multilinear map](#alternating-multilinear-map)
    - [Alternating trilinear form](#alternating-trilinear-form)
  - [Tensor product](#tensor-product)
    - [Universal property of a tensor product](#universal-property-of-a-tensor-product)
    - [Tensor-product basis](#tensor-product-basis)
    - [Tensor algebra](#tensor-algebra)
      - [Truncated tensor algebra](#truncated-tensor-algebra)
      - [Tensor power](#tensor-power)
        - [Tensor square](#tensor-square)
      - [Symmetric algebra](#symmetric-algebra)
        - [Symmetric power](#symmetric-power)
          - [Weight-transfer proof of irreducibility of symmetric powers](#weight-transfer-proof-of-irreducibility-of-symmetric-powers)
          - [Symmetric powers of the three-dimensional SU2 representation](#symmetric-powers-of-the-three-dimensional-su2-representation)
          - [Character generating series of symmetric powers](#character-generating-series-of-symmetric-powers)
          - [Symmetric square](#symmetric-square)
            - [Traceless symmetric square of the defining even orthogonal representation](#traceless-symmetric-square-of-the-defining-even-orthogonal-representation)
              - [Tensor-square decomposition of the defining even orthogonal representation](#tensor-square-decomposition-of-the-defining-even-orthogonal-representation)
            - [Symmetric square of a direct sum](#symmetric-square-of-a-direct-sum)
            - [Symmetric trace-free square of the defining orthogonal representation](#symmetric-trace-free-square-of-the-defining-orthogonal-representation)
  - [Exterior algebra](#exterior-algebra)
    - [Bivector](#bivector)
    - [Exterior product](#exterior-product)
    - [Polynomial polyvector field](#polynomial-polyvector-field)
      - [Schouten-Nijenhuis bracket](#schouten-nijenhuis-bracket)
    - [Grassmann algebra](#grassmann-algebra)
      - [Grassmann parity](#grassmann-parity)
      - [Grassmann derivative](#grassmann-derivative)
      - [Left Grassmann derivative](#left-grassmann-derivative)
      - [Grassmann variable](#grassmann-variable)
    - [Exterior power](#exterior-power)
      - [Exterior square](#exterior-square)
        - [Exterior square of a direct sum](#exterior-square-of-a-direct-sum)
        - [Symplectic contraction of an exterior square](#symplectic-contraction-of-an-exterior-square)
          - [Primitive exterior square](#primitive-exterior-square)
  - [Tensor](#tensor)
    - [Tensor index antisymmetrization](#tensor-index-antisymmetrization)
    - [Tensor index symmetrization](#tensor-index-symmetrization)
    - [Axially invariant second-rank tensor](#axially-invariant-second-rank-tensor)
      - [Smallest axial rotation group forcing second-rank transverse isotropy](#smallest-axial-rotation-group-forcing-second-rank-transverse-isotropy)
    - [Cartesian second-rank tensor](#cartesian-second-rank-tensor)
      - [Cubically invariant second-rank tensor](#cubically-invariant-second-rank-tensor)
      - [Scalar, symmetric-traceless and axial tensor decomposition](#scalar-symmetric-traceless-and-axial-tensor-decomposition)
      - [Divergence of a Cartesian second-rank tensor](#divergence-of-a-cartesian-second-rank-tensor)
      - [Oriented-axis invariant Cartesian tensor](#oriented-axis-invariant-cartesian-tensor)
      - [Coordinate half-turn invariance of a second-rank tensor](#coordinate-half-turn-invariance-of-a-second-rank-tensor)
    - [Composition of mixed tensors](#composition-of-mixed-tensors)
    - [Pseudotensor](#pseudotensor)
    - [Symmetric tensor](#symmetric-tensor)
      - [Axisymmetric symmetric rank-two tensor](#axisymmetric-symmetric-rank-two-tensor)
        - [Weighted chord tensor of a sphere](#weighted-chord-tensor-of-a-sphere)
      - [Polarization spanning of symmetric tensors](#polarization-spanning-of-symmetric-tensors)
      - [Symmetric second-rank tensor](#symmetric-second-rank-tensor)
    - [Quotient theorem for Cartesian tensors](#quotient-theorem-for-cartesian-tensors)
      - [Symmetric-test criterion for a third-rank Cartesian tensor](#symmetric-test-criterion-for-a-third-rank-cartesian-tensor)
      - [Scalar contraction test for a Cartesian tensor](#scalar-contraction-test-for-a-cartesian-tensor)
        - [Antisymmetric contraction test for an antisymmetric tensor](#antisymmetric-contraction-test-for-an-antisymmetric-tensor)
        - [Blindness of symmetric contraction tests to antisymmetric arrays](#blindness-of-symmetric-contraction-tests-to-antisymmetric-arrays)
    - [Traceless second-rank tensor](#traceless-second-rank-tensor)
    - [Slice rank](#slice-rank)
      - [Diagonal tensor](#diagonal-tensor)
        - [Slice rank of a diagonal tensor](#slice-rank-of-a-diagonal-tensor)
    - [Covariance and contravariance of vectors](#covariance-and-contravariance-of-vectors)
      - [Covariant tensor](#covariant-tensor)
    - [Kronecker delta](#kronecker-delta)
    - [Antisymmetric second-rank tensor](#antisymmetric-second-rank-tensor)
    - [Antisymmetric tensor](#antisymmetric-tensor)
      - [Totally antisymmetric tensor](#totally-antisymmetric-tensor)
    - [Isotropic tensor](#isotropic-tensor)
      - [Isotropic elasticity on tensor components](#isotropic-elasticity-on-tensor-components)
      - [Isotropic contractions of a fourth-rank tensor](#isotropic-contractions-of-a-fourth-rank-tensor)
      - [Isotropic third-rank tensor](#isotropic-third-rank-tensor)
      - [Isotropic second-rank tensor](#isotropic-second-rank-tensor)
    - [Einstein notation](#einstein-notation)
  - [Tensor contraction](#tensor-contraction)
    - [Metric trace](#metric-trace)
  - [Reciprocal basis](#reciprocal-basis)
    - [Reciprocal basis involution](#reciprocal-basis-involution)
    - [Orientation of an orthonormal reciprocal basis](#orientation-of-an-orthonormal-reciprocal-basis)
  - [Scalar triple product](#scalar-triple-product)
    - [Cross products with a common vector](#cross-products-with-a-common-vector)
    - [Squared scalar triple product from cyclic cross products](#squared-scalar-triple-product-from-cyclic-cross-products)
  - [Orientation of a vector space](#orientation-of-a-vector-space)
    - [Oriented volume](#oriented-volume)
  - [Determinant](#determinant)
    - [Nonintersecting lattice-path determinant](#nonintersecting-lattice-path-determinant)
    - [Determinant of the minimum-index matrix](#determinant-of-the-minimum-index-matrix)
    - [Cauchy–Binet formula](#cauchy-binet-formula)
    - [Cramer's rule](#cramer-s-rule)
    - [Hadamard determinant inequality](#hadamard-determinant-inequality)
    - [Pfaffian](#pfaffian)
    - [Determinant of a complex block representation](#determinant-of-a-complex-block-representation)
    - [Jacobi determinant derivative formula](#jacobi-determinant-derivative-formula)
    - [Derivative of the determinant](#derivative-of-the-determinant)
      - [Jacobi's formula](#jacobi-s-formula)
      - [Second derivative of the determinant](#second-derivative-of-the-determinant)
    - [Log-determinant](#log-determinant)
    - [Multilinearity of the determinant](#multilinearity-of-the-determinant)
    - [Multiplicativity of the determinant](#multiplicativity-of-the-determinant)
    - [Leibniz formula for determinants](#leibniz-formula-for-determinants)
    - [Tridiagonal determinant recurrence](#tridiagonal-determinant-recurrence)
- [System of linear equations](#system-of-linear-equations)
  - [Image criterion for a matrix factorization](#image-criterion-for-a-matrix-factorization)
  - [Augmented matrix](#augmented-matrix)
  - [Homogeneous linear system](#homogeneous-linear-system)
  - [Linear equation](#linear-equation)
    - [Affine solution space of a linear equation](#affine-solution-space-of-a-linear-equation)
  - [Fredholm alternative for a matrix](#fredholm-alternative-for-a-matrix)
- [Symmetric and antisymmetric parts of a matrix](#symmetric-and-antisymmetric-parts-of-a-matrix)
  - [Symmetric part of a matrix](#symmetric-part-of-a-matrix)
- [Symmetric matrix](#symmetric-matrix)
  - [Complex symmetric nilpotent matrix](#complex-symmetric-nilpotent-matrix)
  - [Axis decomposition of a symmetric matrix](#axis-decomposition-of-a-symmetric-matrix)
  - [Symmetric positive-definite matrix](#symmetric-positive-definite-matrix)
  - [Coaxial symmetric tensors](#coaxial-symmetric-tensors)
  - [Real symmetric spectral orthogonality](#real-symmetric-spectral-orthogonality)
  - [Orthogonal diagonalization of a real symmetric matrix](#orthogonal-diagonalization-of-a-real-symmetric-matrix)
  - [Copositive matrix](#copositive-matrix)
    - [Strictly copositive matrix](#strictly-copositive-matrix)
    - [Horn copositive matrix](#horn-copositive-matrix)
  - [Spectral theorem for real symmetric matrices](#spectral-theorem-for-real-symmetric-matrices)
- [Axis-angle decomposition](#axis-angle-decomposition)
  - [Inverse of an axis-angle linear map](#inverse-of-an-axis-angle-linear-map)
- [Reflection (mathematics)](#reflection-mathematics)
  - [Reflection matrix](#reflection-matrix)
    - [Composition of a plane rotation and a reflection](#composition-of-a-plane-rotation-and-a-reflection)
    - [Reflection in a hyperplane](#reflection-in-a-hyperplane)
    - [Composition of two plane reflections](#composition-of-two-plane-reflections)
- [Rotation matrix](#rotation-matrix)
  - [Trace of a three-dimensional rotation](#trace-of-a-three-dimensional-rotation)
  - [Planar rotation](#planar-rotation)
    - [Finite groups of planar rotations are cyclic](#finite-groups-of-planar-rotations-are-cyclic)
  - [Centralizer of a planar quarter-turn](#centralizer-of-a-planar-quarter-turn)
  - [Rotational symmetry](#rotational-symmetry)
    - [Rotational symmetry group of a regular icosahedron](#rotational-symmetry-group-of-a-regular-icosahedron)
    - [Rotational symmetry group of a regular dodecahedron](#rotational-symmetry-group-of-a-regular-dodecahedron)
- [Cartesian coordinate system](#cartesian-coordinate-system)
  - [Quadrant (plane geometry)](#quadrant-plane-geometry)
    - [Positive quadrant](#positive-quadrant)
- [Matrix geometric series](#matrix-geometric-series)
- [Adjugate matrix](#adjugate-matrix)
  - [Cofactor matrix](#cofactor-matrix)
    - [Cofactor](#cofactor)
  - [Adjugate identity](#adjugate-identity)
- [Matrix equivalence](#matrix-equivalence)
  - [Rank normal form](#rank-normal-form)
- [Block upper triangular matrix](#block-upper-triangular-matrix)
  - [Eigenvalue deflation by an invariant subspace](#eigenvalue-deflation-by-an-invariant-subspace)
- [Sylvester equation](#sylvester-equation)
- [Rank inequality for a composition](#rank-inequality-for-a-composition)
  - [Frobenius rank inequality](#frobenius-rank-inequality)
- [Schur complement](#schur-complement)
  - [Schur complement formula for a diagonal resolvent entry](#schur-complement-formula-for-a-diagonal-resolvent-entry)
- [Orthogonal similarity](#orthogonal-similarity)
- [Product of symmetric matrices](#product-of-symmetric-matrices)
- [Inner product](#inner-product)
  - [Inner product space](#inner-product-space)
  - [Generalized parallelogram identity](#generalized-parallelogram-identity)
  - [Fischer inner product](#fischer-inner-product)
  - [Frobenius inner product](#frobenius-inner-product)
  - [Discrete L2 inner product](#discrete-l2-inner-product)
  - [Weighted inner product](#weighted-inner-product)
  - [Dot product](#dot-product)
  - [Binary inner product](#binary-inner-product)
  - [Orthonormal set](#orthonormal-set)
    - [Orthonormal basis](#orthonormal-basis)
  - [Gram matrix](#gram-matrix)
    - [Unit vectors with a common inner product](#unit-vectors-with-a-common-inner-product)
    - [Gram determinant](#gram-determinant)
    - [Riesz dual basis in an inner product space](#riesz-dual-basis-in-an-inner-product-space)
    - [Gaussian empirical Gram matrix](#gaussian-empirical-gram-matrix)
      - [Gaussian Gram matrix concentration on a fixed subspace](#gaussian-gram-matrix-concentration-on-a-fixed-subspace)
    - [Sparse norm preservation from entrywise Gram control](#sparse-norm-preservation-from-entrywise-gram-control)
  - [Pythagorean theorem in an inner-product space](#pythagorean-theorem-in-an-inner-product-space)
  - [Orthogonal projection onto a finite-dimensional subspace](#orthogonal-projection-onto-a-finite-dimensional-subspace)
    - [Orthogonal projection matrix](#orthogonal-projection-matrix)
      - [Transverse projection operator](#transverse-projection-operator)
    - [Least-squares polynomial in an orthogonal-polynomial basis](#least-squares-polynomial-in-an-orthogonal-polynomial-basis)
  - [Orthogonal vectors](#orthogonal-vectors)
    - [Orthogonal basis](#orthogonal-basis)
  - [Nonorthogonal vectors](#nonorthogonal-vectors)
  - [Gram-Schmidt process](#gram-schmidt-process)
    - [QR decomposition](#qr-decomposition)
      - [Positive-diagonal QR decomposition preserves a complex structure](#positive-diagonal-qr-decomposition-preserves-a-complex-structure)
      - [Thin QR factorization from Cholesky decomposition](#thin-qr-factorization-from-cholesky-decomposition)
      - [Orthogonal coordinate reduction of a subspace](#orthogonal-coordinate-reduction-of-a-subspace)
      - [Linear least-squares problem](#linear-least-squares-problem)
    - [Gram-Schmidt orthogonalization for a symmetric bilinear form](#gram-schmidt-orthogonalization-for-a-symmetric-bilinear-form)
- [Quadratic form](#quadratic-form)
  - [Polar bilinear form of a quadratic form](#polar-bilinear-form-of-a-quadratic-form)
  - [Integral quadratic lattice](#integral-quadratic-lattice)
    - [Even lattice](#even-lattice)
    - [Unimodular lattice](#unimodular-lattice)
      - [Even unimodular lattice](#even-unimodular-lattice)
        - [E8 lattice](#e8-lattice)
  - [Off-diagonal all-ones quadratic form](#off-diagonal-all-ones-quadratic-form)
  - [Arf invariant of a quadratic form](#arf-invariant-of-a-quadratic-form)
    - [Binary quadratic refinement](#binary-quadratic-refinement)
      - [Two-transitive binary quadratic-form actions](#two-transitive-binary-quadratic-form-actions)
  - [Symmetric coefficients of a quadratic polynomial](#symmetric-coefficients-of-a-quadratic-polynomial)
  - [Principal-axis reduction of a quadric](#principal-axis-reduction-of-a-quadric)
  - [Matrix congruence](#matrix-congruence)
    - [Simultaneous congruence diagonalization with a positive form](#simultaneous-congruence-diagonalization-with-a-positive-form)
  - [Positive-definite quadratic form](#positive-definite-quadratic-form)
  - [Ternary quadratic form](#ternary-quadratic-form)
    - [Isotropy of nondegenerate ternary quadratic forms over finite fields](#isotropy-of-nondegenerate-ternary-quadratic-forms-over-finite-fields)
      - [Local isotropy of the five seven thirteen form](#local-isotropy-of-the-five-seven-thirteen-form)
  - [Hyperbolic plane (quadratic form)](#hyperbolic-plane-quadratic-form)
  - [Parallelogram law](#parallelogram-law)
  - [Rank of a quadratic form](#rank-of-a-quadratic-form)
    - [Rank-one quadratic form](#rank-one-quadratic-form)
  - [Signature of a quadratic form](#signature-of-a-quadratic-form)
  - [Polarization identity](#polarization-identity)
    - [Polarization argument for a vanishing quadratic form](#polarization-argument-for-a-vanishing-quadratic-form)
  - [Positive semidefinite bilinear form](#positive-semidefinite-bilinear-form)
  - [Definite matrix](#definite-matrix)
    - [Positive semidefinite matrix](#positive-semidefinite-matrix)
      - [Bipartite block-constant positive semidefinite matrix](#bipartite-block-constant-positive-semidefinite-matrix)
      - [Completely positive matrix](#completely-positive-matrix)
      - [Zero quadratic form of a positive semidefinite matrix](#zero-quadratic-form-of-a-positive-semidefinite-matrix)
      - [Positive semidefinite trace nonnegativity](#positive-semidefinite-trace-nonnegativity)
      - [Loewner order](#loewner-order)
      - [Square root of a matrix](#square-root-of-a-matrix)
        - [Principal square root of a positive semidefinite matrix](#principal-square-root-of-a-positive-semidefinite-matrix)
          - [Polar decomposition of an invertible real matrix](#polar-decomposition-of-an-invertible-real-matrix)
            - [Polar decomposition of an invertible complex matrix](#polar-decomposition-of-an-invertible-complex-matrix)
    - [Positive-definite matrix](#positive-definite-matrix)
      - [Cholesky decomposition](#cholesky-decomposition)
        - [Rank-one Cholesky update](#rank-one-cholesky-update)
      - [Sylvester's criterion](#sylvester-s-criterion)
      - [Condition number](#condition-number)
        - [Spectral condition number of a positive-definite matrix](#spectral-condition-number-of-a-positive-definite-matrix)
      - [Hermitian positive-definite matrix](#hermitian-positive-definite-matrix)
        - [Toeplitz matrix](#toeplitz-matrix)
          - [Symmetric tridiagonal Toeplitz matrix](#symmetric-tridiagonal-toeplitz-matrix)
          - [Toeplitz antisymmetric tridiagonal matrix](#toeplitz-antisymmetric-tridiagonal-matrix)
    - [Negative-definite matrix](#negative-definite-matrix)
  - [Sylvester's law of inertia](#sylvester-s-law-of-inertia)
    - [Criterion for membership in a diagonal basis](#criterion-for-membership-in-a-diagonal-basis)
  - [Isotropic quadratic form](#isotropic-quadratic-form)
    - [Hasse-Minkowski theorem](#hasse-minkowski-theorem)
      - [Hasse invariant of a quadratic form](#hasse-invariant-of-a-quadratic-form)
    - [Totally isotropic subspace](#totally-isotropic-subspace)
      - [Isotropic dimension bound from real inertia](#isotropic-dimension-bound-from-real-inertia)
      - [Complex quadratic forms have a large isotropic subspace](#complex-quadratic-forms-have-a-large-isotropic-subspace)
        - [Common zero of complex quadratic forms](#common-zero-of-complex-quadratic-forms)
      - [Maximum dimension of a totally isotropic subspace](#maximum-dimension-of-a-totally-isotropic-subspace)
    - [Isotropic vector](#isotropic-vector)
  - [Quadratic form gradient](#quadratic-form-gradient)
- [Schur product theorem](#schur-product-theorem)
  - [Coefficient-dominated entrywise positivity](#coefficient-dominated-entrywise-positivity)
- [Orthogonal group](#orthogonal-group)
  - [Orthogonal group as a regular level set](#orthogonal-group-as-a-regular-level-set)
  - [Cartan–Dieudonné theorem](#cartan-dieudonne-theorem)
  - [Determinant-twist projection in odd dimension](#determinant-twist-projection-in-odd-dimension)
  - [Odd-dimensional orthogonal determinant splitting](#odd-dimensional-orthogonal-determinant-splitting)
  - [Orthogonal matrix](#orthogonal-matrix)
    - [Orthogonal transformation](#orthogonal-transformation)
  - [Improper orthogonal transformation](#improper-orthogonal-transformation)
    - [Three-dimensional improper orthogonal transformation](#three-dimensional-improper-orthogonal-transformation)
  - [Special orthogonal group](#special-orthogonal-group)
    - [Trace height on the special orthogonal group](#trace-height-on-the-special-orthogonal-group)
    - [Low homotopy groups of special orthogonal groups](#low-homotopy-groups-of-special-orthogonal-groups)
    - [Special orthogonal sphere fibration](#special-orthogonal-sphere-fibration)
      - [Surjectivity of special orthogonal stabilization below the sphere dimension](#surjectivity-of-special-orthogonal-stabilization-below-the-sphere-dimension)
    - [SO(4) group](#so-4-group)
      - [Representations of SO(4) from two SU2 spins](#representations-of-so-4-from-two-su2-spins)
    - [Rotations preserving an axis](#rotations-preserving-an-axis)
    - [SO(3) group](#so-3-group)
      - [SO(3) as real projective three-space](#so-3-as-real-projective-three-space)
    - [Odd-dimensional special orthogonal transformation has a fixed vector](#odd-dimensional-special-orthogonal-transformation-has-a-fixed-vector)
    - [Special orthogonal group as a submanifold](#special-orthogonal-group-as-a-submanifold)
    - [Unit-vector stabilizer in a special orthogonal group](#unit-vector-stabilizer-in-a-special-orthogonal-group)
      - [Distinct unit-vector stabilizers are not transverse](#distinct-unit-vector-stabilizers-are-not-transverse)
    - [Rotation in three dimensions](#rotation-in-three-dimensions)
  - [Skew-symmetric matrix](#skew-symmetric-matrix)
    - [Unitary skew-diagonalization of an antisymmetric matrix](#unitary-skew-diagonalization-of-an-antisymmetric-matrix)
    - [Cross-product matrix](#cross-product-matrix)
      - [Cross-product matrix spectrum](#cross-product-matrix-spectrum)
- [Tensor product of linear maps](#tensor-product-of-linear-maps)
  - [Tensor-product operator](#tensor-product-operator)
- [Trace-duality bound](#trace-duality-bound)
- [Diagonal matrix](#diagonal-matrix)
  - [Scalar matrix](#scalar-matrix)
- [Triangular matrix](#triangular-matrix)
  - [Back substitution](#back-substitution)
  - [Upper triangular matrix](#upper-triangular-matrix)
    - [Strictly upper triangular matrix](#strictly-upper-triangular-matrix)
  - [Lower triangular matrix](#lower-triangular-matrix)
    - [Lower triangular matrix algebra](#lower-triangular-matrix-algebra)
  - [Triangular linear system](#triangular-linear-system)
    - [Forward substitution in a triangular system](#forward-substitution-in-a-triangular-system)
    - [Backward substitution in a triangular system](#backward-substitution-in-a-triangular-system)
- [Axis-angle representation](#axis-angle-representation)

## Hyperbolic pair

↑ **Parent:** [Linear algebra](linear-algebra.md)

Two vectors spanning a hyperbolic plane. For an [alternating bilinear form](#alternating-bilinear-form), choose $B(e,f)=1$; then their span is nondegenerate. For a [quadratic form](#quadratic-form) with polar form $B$, require also $Q(e)=Q(f)=0$. The analogous definition for a [Hermitian form](#hermitian-form) uses two isotropic vectors of pairing one. Extending such pairs to adapted [bases](vector-space.md#basis) is useful for constructing form-preserving maps.

## Cartesian basis

↑ **Parent:** [Linear algebra](linear-algebra.md)

A Cartesian basis is an orthonormal basis associated with the perpendicular axes of a [Cartesian coordinate system](#cartesian-coordinate-system).

## Bilinear form

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bilinear_form)

A bilinear form on a vector space $V$ over a field $F$ is a map $B:V\times V\to F$ that is linear in each argument separately.

### Orthogonal complement for a bilinear form

↑ **Parent:** [Bilinear form](#bilinear-form)

For a [bilinear form](#bilinear-form) on a finite-dimensional [vector space](vector-space.md), the displayed right [bilinear orthogonal complement](#orthogonal-complement-for-a-bilinear-form) is a subspace. Nondegeneracy identifies the ambient space with its dual and gives $\dim W^\perp=\dim V-\dim W$. If the form is symmetric or alternating, orthogonality is reciprocal and $(W^\perp)^\perp=W$. For a general nonsymmetric form, left and right complements must be distinguished. A restricted symmetric or alternating form has [radical of a bilinear form](#radical-of-a-bilinear-form) $W\cap W^\perp$; quotienting by that [radical of a bilinear form](#radical-of-a-bilinear-form) gives a [nondegenerate](#nondegenerate-bilinear-form) induced form.

### Isometry of a space with a form

↑ **Parent:** [Bilinear form](#bilinear-form)

A linear bijection between spaces carrying compatible [bilinear forms](#bilinear-form), [Hermitian forms](#hermitian-form) or [quadratic forms](#quadratic-form) is an [isometry of a space with a form](#isometry-of-a-space-with-a-form) when it preserves the specified form. Preserving the polar form alone need not preserve a [quadratic form](#quadratic-form) in characteristic two. Subspaces may have degenerate restricted forms even when the ambient form is nonsingular.

#### Anisotropic vector for a form

↑ **Parent:** [Isometry of a space with a form](#isometry-of-a-space-with-a-form)

A vector is anisotropic for a [quadratic form](#quadratic-form) if $Q(v)\ne0$, and for a [Hermitian form](#hermitian-form) if $h(v,v)\ne0$. The complementary zero-value condition is isotropy. For a [symmetric bilinear form](#symmetric-bilinear-form) in odd [characteristic of a field](algebra.md#characteristic-of-a-field), this agrees with the associated [quadratic form](#quadratic-form). A [nondegenerate](#nondegenerate-bilinear-form) [alternating bilinear form](#alternating-bilinear-form) has all self-pairings zero, so nondegeneracy must not be confused with the existence of anisotropic vectors.

<h4 id="witt-s-theorem">Witt's theorem</h4>

↑ **Parent:** [Isometry of a space with a form](#isometry-of-a-space-with-a-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Witt's_theorem)

An [isometry of a space with a form](#isometry-of-a-space-with-a-form) between subspaces of a finite-dimensional nonsingular classical space extends to an ambient isometry. This includes [alternating bilinear forms](#alternating-bilinear-form) in all characteristics, [symmetric bilinear forms](#symmetric-bilinear-form) in characteristic different from two, [Hermitian forms](#hermitian-form) with nontrivial involution, and [quadratic forms](#quadratic-form) with nonsingular polar form. No nonsingularity of the restricted subspace is required. Bare nonalternating symmetric bilinear forms in characteristic two require additional hypotheses and must not be confused with quadratic spaces.

### Positive-definite bilinear form

↑ **Parent:** [Bilinear form](#bilinear-form)

A symmetric real [bilinear form](#bilinear-form) is positive-definite when $B(v,v)>0$ for every nonzero vector. It defines an [inner product](#inner-product) and the associated [norm](functional-analysis.md#norm) $\sqrt{B(v,v)}$. The complex [Killing form](lie-algebra.md#killing-form) is not positive-definite on the entire complex [Cartan subalgebra](semisimple-lie-algebra.md#cartan-subalgebra); its restriction to the [Euclidean subspace of a Cartan subalgebra](semisimple-lie-algebra.md#euclidean-subspace-of-a-cartan-subalgebra) is a real positive-definite form.

#### Positive definiteness

↑ **Parent:** [Positive-definite bilinear form](#positive-definite-bilinear-form)

The strict positivity of a [quadratic form](#quadratic-form) on every nonzero [vector](vector-space.md#vector). A real symmetric [matrix](vector-space.md#matrix) has positive definiteness exactly when its associated [quadratic form](#quadratic-form) does, making it a [positive-definite matrix](#positive-definite-matrix). A [Hermitian form](#hermitian-form) is positive definite when its value on $(v,v)$ is real and strictly positive for every nonzero vector.

### Alternating bilinear form

↑ **Parent:** [Bilinear form](#bilinear-form)

A [bilinear form](#bilinear-form) is alternating if $B(v,v)=0$ for every [vector](vector-space.md#vector) $v$. Expanding $B(v+w,v+w)$ implies $B(v,w)=-B(w,v)$. The converse requires [characteristic](algebra.md#characteristic-of-a-field) different from two. In that characteristic a skew-symmetric [matrix](vector-space.md#matrix) of [odd integer](number-theory.md#odd-integer) size has zero [determinant](#determinant), since $\det A=\det(-A^T)=(-1)^n\det A$. Thus an alternating form on a finite odd-dimensional [vector space](vector-space.md) is degenerate. A [nondegenerate](#nondegenerate-bilinear-form) alternating form defines a [symplectic vector space](#symplectic-vector-space).

### Symmetric bilinear form

↑ **Parent:** [Bilinear form](#bilinear-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_bilinear_form)

A [bilinear form](#bilinear-form) $B$ is symmetric when $B(v,w)=B(w,v)$ for every pair of vectors $v,w$.

#### Modified trace form on real matrices

↑ **Parent:** [Symmetric bilinear form](#symmetric-bilinear-form)

On real $n$ by $n$ matrices with $n\geq2$, split into traceless symmetric matrices, skew-symmetric matrices and scalar matrices. These summands are orthogonal for the displayed [symmetric bilinear form](#symmetric-bilinear-form). The form is positive on the first summand, negative on the second and negative on the scalar identity direction. Its [inertia of a bilinear form](#inertia-of-a-bilinear-form) is $(n(n+1)/2-1,n(n-1)/2+1,0)$, its rank is $n^2$ and its [signature](#signature-of-a-quadratic-form) is $n-2$. Indeed $\operatorname{tr}(S^2)=\|S\|_F^2$, $\operatorname{tr}(K^2)=-\|K\|_F^2$ and $\phi(tI,tI)=-n(n-1)t^2$.

#### Witt group of a field

↑ **Parent:** [Symmetric bilinear form](#symmetric-bilinear-form)

For a field $K$ of characteristic different from two, $W(K)$ is the group of nonsingular symmetric bilinear forms modulo metabolic forms, with orthogonal sum as addition. A metabolic form has a half-dimensional totally isotropic subspace. Such a form is equivalent to a sum of hyperbolic planes, hence represents zero.

### Bounded bilinear form

↑ **Parent:** [Bilinear form](#bilinear-form)

A bilinear form $B:X\times X\to\mathbb R$ on a [normed vector space](functional-analysis.md#normed-vector-space) is bounded when some $C<\infty$ satisfies $|B(u,v)|\leq C\lVert u\rVert\lVert v\rVert$ for all $u,v\in X$.

#### Grothendieck inequality

↑ **Parent:** [Bounded bilinear form](#bounded-bilinear-form)

For a finite real scalar matrix $(a_{ij})$ and unit vectors $u_i,v_j$ in a real [Hilbert space](hilbert-space.md), $|\sum a_{ij}\langle u_i,v_j\rangle|\le K_G\max_{\varepsilon_i,\delta_j\in\{-1,1\}}|\sum a_{ij}\varepsilon_i\delta_j|$, with a universal constant. One valid bound is $K_G\le\pi/(2\log(1+\sqrt2))$. Expand $\sin(ct)$ using odd [tensor powers](#tensor-power) with coefficient magnitudes summing to $\sinh c=1$, then apply the Gaussian sign identity $\mathbb E[\operatorname{sgn}\langle G,u\rangle\operatorname{sgn}\langle G,v\rangle]=(2/\pi)\arcsin\langle u,v\rangle$. Taking $c=\log(1+\sqrt2)$ converts the expectation back to the original inner product. Complex scalars admit a universal bound twice this real bound by separating real and imaginary parts.

##### Grothendieck theorem for L1 to Hilbert operators

↑ **Parent:** [Grothendieck inequality](#grothendieck-inequality)

Every [bounded linear operator](topological-vector-space.md#continuous-linear-operator) $T:L^1(\mu)\to H$ into a [Hilbert space](hilbert-space.md) is an [absolutely summing operator](topological-vector-space.md#absolutely-summing-operator), with $\pi_1(T)\le K_G\|T\|$. For simple functions on a common disjoint partition, apply the [Grothendieck inequality](#grothendieck-inequality) to the vectors $T(1_A/\mu(A))$ and norming vectors of the images. The scalar sign or phase supremum is the weak 1-norm of the family. Approximation by simple functions proves the general result.

###### Rademacher span is not complemented in L1

↑ **Parent:** [Grothendieck theorem for L1 to Hilbert operators](#grothendieck-theorem-for-l1-to-hilbert-operators)

If the closed span of the [Rademacher functions](probability-theory.md#rademacher-function) were a [complemented subspace](banach-space.md#complemented-subspace) of $L^1(0,1)$, compose a projection with the inverse of its [l2 sequence space](banach-space.md#l2-sequence-space) parametrization. The [Grothendieck theorem for L1 to Hilbert operators](#grothendieck-theorem-for-l1-to-hilbert-operators) would make this map an [absolutely summing operator](topological-vector-space.md#absolutely-summing-operator). Its composition with the parametrization would make the identity on the infinite-dimensional [l2 sequence space](banach-space.md#l2-sequence-space) absolutely summing, contradicting its coordinate-vector test.

#### Boundedness criterion for a bilinear form

↑ **Parent:** [Bounded bilinear form](#bounded-bilinear-form)

A [bilinear form](#bilinear-form) on a [normed vector space](functional-analysis.md#normed-vector-space) is [continuous](calculus.md#continuous-function) exactly when it is bounded. For the nontrivial direction, continuity at $(0,0)$ gives $r,s>0$ such that $|B(x,y)|\leq1$ whenever $\lVert x\rVert<r$ and $\lVert y\rVert<s$; scaling nonzero $u,v$ into these balls gives $|B(u,v)|\leq4(rs)^{-1}\lVert u\rVert\lVert v\rVert$.

### Coercive bilinear form

↑ **Parent:** [Bilinear form](#bilinear-form)

A bilinear form $B$ on a [normed vector space](functional-analysis.md#normed-vector-space) is coercive when some $\alpha>0$ satisfies $B(v,v)\geq\alpha\lVert v\rVert^2$ for every $v$.

### Degenerate bilinear form

↑ **Parent:** [Bilinear form](#bilinear-form)

A bilinear form is degenerate when its [radical](#radical-of-a-bilinear-form) contains a nonzero vector.

### Radical of a bilinear form

↑ **Parent:** [Bilinear form](#bilinear-form)

The radical of a symmetric bilinear form $B$ is

$$
\operatorname{rad}B=\{v:B(v,w)=0\text{ for every }w\}.
$$

The form is nondegenerate exactly when its radical is zero.

### Nondegenerate bilinear form

↑ **Parent:** [Bilinear form](#bilinear-form)

A [bilinear form](#bilinear-form) $B$ on a finite-dimensional [vector space](vector-space.md) is nondegenerate when

$$
B(v,w)=0\text{ for every }v\quad\Longrightarrow\quad w=0,
$$

equivalently when $w\mapsto B(-,w)$ is an isomorphism from $V$ to its [dual space](#dual-space).

#### Dual isomorphisms induced by a nondegenerate pairing

↑ **Parent:** [Nondegenerate bilinear form](#nondegenerate-bilinear-form)

A [bilinear form](#bilinear-form) $b:U\times V\to K$ with zero left and right radicals induces injective [linear maps](vector-space.md#linear-map) $U\to V^*$ and $V\to U^*$. Finite dimensions force $\dim U=\dim V$, so both maps are isomorphisms. For any other bilinear form $c$, composing its maps to the [dual spaces](#dual-space) with these inverse isomorphisms gives unique endomorphisms $S,T$ with $c(x,y)=b(Sx,y)=b(x,Ty)$. In bases with invertible pairing matrix $B$ and coefficient matrix $C$, $S=B^{-T}C^T$ and $T=B^{-1}C$.

#### Symplectic vector space

↑ **Parent:** [Nondegenerate bilinear form](#nondegenerate-bilinear-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symplectic_vector_space)

A symplectic vector space is a vector space equipped with a nondegenerate antisymmetric bilinear form. Every finite-dimensional symplectic vector space has even dimension: splitting off one symplectic two-plane leaves a smaller nondegenerate antisymmetric space, and induction completes the decomposition.

##### Symplectic linear map

↑ **Parent:** [Symplectic vector space](#symplectic-vector-space)

A [linear map](vector-space.md#linear-map) $A:(V,\omega_V)\to(W,\omega_W)$ is symplectic when it pulls back the target [symplectic form](symplectic-geometry.md#symplectic-form) to the source form. [Nondegenerate bilinear form](#nondegenerate-bilinear-form) makes such a map [injective](algebra.md#injective-function). In equal finite dimensions it is an [isomorphism](algebra.md#isomorphism). The automorphisms form the [symplectic group](symplectic-geometry.md#symplectic-group) and preserve the [symplectic orientation](symplectic-geometry.md#symplectic-orientation) on the ambient space and on every [symplectic subspace](#symplectic-subspace).

##### Symplectic subspace

↑ **Parent:** [Symplectic vector space](#symplectic-vector-space)

A subspace of a [symplectic vector space](#symplectic-vector-space) is symplectic if the restricted [symplectic form](symplectic-geometry.md#symplectic-form) is [nondegenerate](#nondegenerate-bilinear-form). It has a [symplectic orthogonal complement](#symplectic-orthogonal-complement) and the ambient space is the direct sum of those two subspaces.

###### Orientation criterion for a graph of symplectic planes

↑ **Parent:** [Symplectic subspace](#symplectic-subspace)

Let $V=C\oplus D$ be a [symplectic orthogonal complement](#symplectic-orthogonal-complement) splitting into two [symplectic subspaces](#symplectic-subspace) of dimension two. In [symplectic bases](#symplectic-basis), the [graph of a function](function.md#graph-of-a-function) $A:D\to C$ pulls back the [symplectic form](symplectic-geometry.md#symplectic-form) to $\omega_D+A^*\omega_C=(1+\det A)\omega_D$. It is a [symplectic subspace](#symplectic-subspace) exactly when $\det A\ne-1$. Its [symplectic orientation](symplectic-geometry.md#symplectic-orientation) agrees with the orientation transported from $D$ exactly when $\det A>-1$. When $\det A<-1$, the transverse oriented pair $(C,\Gamma_A)$ has negative intersection sign, whereas two distinct complex lines in a compatible complex two-space have positive intersection sign.

##### Eigenspaces of a symplectic involution

↑ **Parent:** [Symplectic vector space](#symplectic-vector-space)

If $T$ preserves a [nondegenerate bilinear form](#nondegenerate-bilinear-form) $\omega$ that is alternating and satisfies $T^2=I$ on a finite-dimensional [vector space](vector-space.md) over a [field](algebra.md#field) of characteristic different from two, then

$$
V=\ker(T-I)\oplus\ker(T+I).
$$

The two [eigenspaces](linear-operator-theory.md#eigenspace) are orthogonal for $\omega$, since $\omega(v_+,v_-)=\omega(Tv_+,Tv_-)=-\omega(v_+,v_-)$. Each restricted form is nondegenerate: a vector annihilating its own eigenspace also annihilates the other and hence all of $V$. Both dimensions are even, say $2a$ and $2b$. Consequently $\operatorname{tr}T=2a-2b=\dim V-4b$ as an integer obtained from the eigenspace dimensions. Over the real numbers this gives the congruence $\operatorname{tr}T\equiv\dim V\pmod4$.

##### Symplectic orthogonal complement

↑ **Parent:** [Symplectic vector space](#symplectic-vector-space)

The symplectic orthogonal complement of a subspace $W$ is $W^\omega=\{v:\omega(v,w)=0\text{ for every }w\in W\}$. The [nondegenerate bilinear form](#nondegenerate-bilinear-form) gives $\dim W^\omega=\dim V-\dim W$. An [isotropic subspace of a symplectic vector space](#isotropic-subspace-of-a-symplectic-vector-space) satisfies $W\subset W^\omega$; a [Lagrangian subspace](symplectic-geometry.md#lagrangian-subspace) satisfies equality.

##### Isotropic subspace of a symplectic vector space

↑ **Parent:** [Symplectic vector space](#symplectic-vector-space)

A subspace $W$ of a [symplectic vector space](#symplectic-vector-space) $(V,\Omega)$ is isotropic when $\Omega|_{W\times W}=0$. It has at most half the dimension of $V$; equality makes it a [Lagrangian subspace](symplectic-geometry.md#lagrangian-subspace). This use of isotropic concerns an alternating [bilinear form](#bilinear-form), rather than an [isotropic quadratic form](#isotropic-quadratic-form).

##### Symplectic basis

↑ **Parent:** [Symplectic vector space](#symplectic-vector-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symplectic_basis)

A symplectic basis $(e_1,\ldots,e_n,f_1,\ldots,f_n)$ has pairings $\omega(e_i,f_j)=\delta_{ij}$ and all pairings between two $e_i$ or two $f_i$ equal to zero.

#### Representation of a bilinear form relative to a nondegenerate bilinear form

↑ **Parent:** [Nondegenerate bilinear form](#nondegenerate-bilinear-form)

If $B_1$ is a [nondegenerate bilinear form](#nondegenerate-bilinear-form) on a finite-dimensional vector space and $B_2$ is any bilinear form, there is a unique [linear map](vector-space.md#linear-map) $\alpha$ such that

$$
B_2(v,w)=B_1(v,\alpha w).
$$

The right radical of $B_2$ is $\ker\alpha$.

### Inertia of a bilinear form

↑ **Parent:** [Bilinear form](#bilinear-form)

The inertia of a real symmetric bilinear form is the triple giving the numbers of positive, negative, and zero squares in a diagonalization. [Sylvester's law of inertia](#sylvester-s-law-of-inertia) makes it independent of the chosen basis.

#### Signature pair of a real symmetric bilinear form

↑ **Parent:** [Inertia of a bilinear form](#inertia-of-a-bilinear-form)

For a real [symmetric bilinear form](#symmetric-bilinear-form), let $n_+$ and $n_-$ be the dimensions of its positive and negative diagonal subspaces. This pair gives the first two components of the [inertia of a bilinear form](#inertia-of-a-bilinear-form) and is independent of basis by the [Sylvester's law of inertia](#sylvester-s-law-of-inertia). For a nondegenerate form their sum is the full dimension; otherwise the nullity is an additional invariant. Another convention calls the difference $n_+-n_-$ the [signature of a quadratic form](#signature-of-a-quadratic-form). The pair convention describes the positive and negative harmonic spaces of the [real de Rham intersection form in dimension four](homology.md#real-de-rham-intersection-form-in-dimension-four).

## Sesquilinear form

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sesquilinear_form)

A complex sesquilinear form is linear in one argument and conjugate-linear in the other. Here the first argument is taken to be linear.

### Orthogonal complement for a sesquilinear form

↑ **Parent:** [Sesquilinear form](#sesquilinear-form)

For a [Hermitian form](#hermitian-form) or a [Hermitian form over a quadratic finite field](#hermitian-form-over-a-quadratic-finite-field), the displayed subspace is the orthogonal complement of $W$. If the form restricts nondegenerately to a finite-dimensional $W$, its invertible Gram matrix supplies, for each $v$, a unique $w_0\in W$ with $B(v-w_0,W)=0$. Consequently $V=W\oplus W^\perp$. When the form on $V$ is nondegenerate, its restriction to $W^\perp$ is too: a radical vector there is orthogonal to both summands and hence is zero.

### Hermitian form

↑ **Parent:** [Sesquilinear form](#sesquilinear-form)

A Hermitian form is a complex sesquilinear form $H$ satisfying $H(w,v)=\overline{H(v,w)}$.

#### Hermitian form over a quadratic finite field

↑ **Parent:** [Hermitian form](#hermitian-form)

Over the [finite field](algebra.md#finite-field) $K=\mathbb F_{q^2}$, a [sesquilinear form](#sesquilinear-form) relative to $a\mapsto a^q$ is linear in its first argument and conjugate-linear in its second. It is Hermitian when $B(w,v)=\overline{B(v,w)}$. Its diagonal values belong to $\mathbb F_q$; it is nondegenerate when $B(v,w)=0$ for every $w$ forces $v=0$. This definition applies in characteristic two as well.

##### Hermitian hyperbolic plane over a finite field

↑ **Parent:** [Hermitian form over a quadratic finite field](#hermitian-form-over-a-quadratic-finite-field)

In a two-dimensional nondegenerate [Hermitian form over a quadratic finite field](#hermitian-form-over-a-quadratic-finite-field), choose an [orthonormal basis](#orthonormal-basis) $v,w$ and $a$ with $a\bar a=-1$. Then $e=v+aw$ is an [isotropic vector](#isotropic-vector). Choose $g$ with $B(e,g)=1$, and choose $c$ with $c+\bar c=B(g,g)$. The vector $f=g-ce$ satisfies $B(e,f)=1$ and $B(f,f)=0$. Thus $e,f$ give the displayed matrix, including in characteristic two. Iterating on nondegenerate [orthogonal complement for a sesquilinear form](#orthogonal-complement-for-a-sesquilinear-form) leaves only a unit-norm line in odd dimension.

##### Orthonormalization of a finite-field Hermitian form

↑ **Parent:** [Hermitian form over a quadratic finite field](#hermitian-form-over-a-quadratic-finite-field)

A nondegenerate [Hermitian form over a quadratic finite field](#hermitian-form-over-a-quadratic-finite-field) has an [orthonormal basis](#orthonormal-basis). If all diagonal values vanished, evaluating $B(v+aw,v+aw)$ would give $\operatorname{Tr}(\bar a B(v,w))=0$ for every $a$, contradicting [quadratic finite-field norm and trace surjectivity](algebra.md#quadratic-finite-field-norm-and-trace-surjectivity) and nondegeneracy. Thus some $v$ has nonzero norm; rescaling using the [field norm](algebraic-number-theory.md#field-norm) makes it one. Its [orthogonal complement for a sesquilinear form](#orthogonal-complement-for-a-sesquilinear-form) is nondegenerate, so induction completes the [basis](vector-space.md#basis).

#### Monomial orthonormal basis on the unit torus

↑ **Parent:** [Hermitian form](#hermitian-form)

Integrate a [polynomial](polynomial.md) times the conjugate of another over the product of unit circles, with normalized product angular measure. [Fourier orthogonality](fourier-series.md#fourier-orthogonality) makes the [monomials](polynomial.md#monomial) $z_1^{\alpha_1}\cdots z_d^{\alpha_d}$ an [orthonormal basis](#orthonormal-basis) of the polynomial [vector space](vector-space.md). The [Hermitian form](#hermitian-form) is positive definite because the squared norm is the sum of squared absolute values of the finitely many coefficients. No completion or infinite series is needed to obtain this algebraic basis.

#### Radical of a Hermitian form

↑ **Parent:** [Hermitian form](#hermitian-form)

The radical of a [Hermitian form](#hermitian-form) is the [vector subspace](vector-space.md#vector-subspace) orthogonal to the entire space. The form descends to the [quotient vector space](vector-space.md#quotient-vector-space) by its radical: adding a radical [vector](vector-space.md#vector) to either argument does not change the value. For a [positive semidefinite Hermitian form](#positive-semidefinite-hermitian-form), the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) identifies this radical with its zero-norm [vectors](vector-space.md#vector), so the quotient form is positive definite. This conclusion does not hold for a general [indefinite Hermitian form](#indefinite-hermitian-form): a zero-norm [vector](vector-space.md#vector) need not belong to its radical.

#### Positive semidefinite Hermitian form

↑ **Parent:** [Hermitian form](#hermitian-form)

A [Hermitian form](#hermitian-form) is positive semidefinite when $h(v,v)\geq0$ for every [vector](vector-space.md#vector). It need not define an [inner product](#inner-product), because a nonzero [vector](vector-space.md#vector) may have zero squared [norm](functional-analysis.md#norm). The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) still holds: applying nonnegativity to $v+zw$ and minimizing the quadratic expression in $z$ gives $|h(v,w)|^2\leq h(v,v)h(w,w)$ when $h(w,w)>0$; when $h(w,w)=0$, varying $z$ forces $h(v,w)=0$. Thus its zero-norm [vectors](vector-space.md#vector) are exactly the [radical of a Hermitian form](#radical-of-a-hermitian-form). Quotienting this [radical of a Hermitian form](#radical-of-a-hermitian-form) gives a positive [inner product](#inner-product); taking its [Hilbert space completion](hilbert-space.md#hilbert-space-completion) then gives a [Hilbert space](hilbert-space.md). This is the final positivity step in the [Gupta-Bleuler null-state quotient](relativistic-quantum-field.md#gupta-bleuler-null-state-quotient).

#### Indefinite Hermitian form

↑ **Parent:** [Hermitian form](#hermitian-form)

An indefinite [Hermitian form](#hermitian-form) takes both positive and negative values on $\langle v,v\rangle$ for nonzero [vectors](vector-space.md#vector). For example, $-|v_0|^2+|v_1|^2+|v_2|^2+|v_3|^2$ is indefinite. It is not a positive [inner product](#inner-product) defining a [Hilbert space](hilbert-space.md), and a nonzero [vector](vector-space.md#vector) can have zero norm without being orthogonal to all [vectors](vector-space.md#vector). A positive semidefinite restricted form becomes a positive [inner product](#inner-product) only after quotienting its [radical of a Hermitian form](#radical-of-a-hermitian-form).

#### Matrix of a Hermitian form

↑ **Parent:** [Hermitian form](#hermitian-form)

For a basis $(v_i)$, the matrix $A$ of a [Hermitian form](#hermitian-form) has entries $A_{ij}=H(v_i,v_j)$. With the convention that $H$ is linear in its first argument, coordinate columns $x,y$ satisfy $H(x,y)=x^TA\overline y$.

## Vector space

↑ **Parent:** [Linear algebra](linear-algebra.md)

[This section is present in another page, follow this link to view it.](vector-space.md)

## Singular value decomposition

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singular_value_decomposition)

Every complex matrix has a factorization $A=V\Sigma U^\dagger$ with $U,V$ unitary and $\Sigma$ diagonal with nonnegative entries. The squared singular values are the eigenvalues of $A^\dagger A$.

### Autonne-Takagi factorization

↑ **Parent:** [Singular value decomposition](#singular-value-decomposition)

Every complex [symmetric matrix](#symmetric-matrix) admits a unitary congruence decomposition with a [unitary matrix](linear-operator-theory.md#unitary-matrix) $U$ and nonnegative diagonal entries $s_j$ equal to its [singular values](#singular-value). This differs from unitary similarity diagonalization. It reduces a [multimode squeezed vacuum](quantum-mechanics.md#multimode-squeezed-vacuum) to independent oscillator squeezing factors.

### Singular value

↑ **Parent:** [Singular value decomposition](#singular-value-decomposition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singular_value)

The singular values of a [matrix](vector-space.md#matrix) $A$ are the nonnegative [square roots](algebra.md#square-root) of the [eigenvalues](linear-operator-theory.md#eigenvalue) of $A^*A$.

#### Right singular vector

↑ **Parent:** [Singular value](#singular-value)

A unit right singular vector of a [matrix](vector-space.md#matrix) or [compact operator](compact-operator.md) $A$ is an [eigenvector](linear-operator-theory.md#eigenvector) of $A^*A$ with [eigenvalue](linear-operator-theory.md#eigenvalue) $\sigma_j^2$. For $\sigma_j>0$, $u_j=Av_j/\sigma_j$ is the corresponding [left singular vector](#left-singular-vector). The largest [singular value](#singular-value) is the [operator norm](continuous-dual-space.md#operator-norm) of $A$, attained on its corresponding [right singular vectors](#right-singular-vector).

#### Left singular vector

↑ **Parent:** [Singular value](#singular-value)

A unit left singular vector of a [matrix](vector-space.md#matrix) or [compact operator](compact-operator.md) $A$ is an [eigenvector](linear-operator-theory.md#eigenvector) of $AA^*$ with [eigenvalue](linear-operator-theory.md#eigenvalue) $\sigma_j^2$. For $\sigma_j>0$, it pairs with a [right singular vector](#right-singular-vector) $v_j$ through $Av_j=\sigma_j u_j$ and $A^*u_j=\sigma_j v_j$.

## Unimodular matrix

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unimodular_matrix)

An integral square matrix is unimodular when its determinant is $1$ or $-1$. Its inverse again has integral entries, so it defines an invertible change of integer coordinates.

## Householder transformation

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Householder_transformation)

For unit $v$, $I-2vv^T$ is an orthogonal reflection. Successive Householder similarities reduce a symmetric matrix while preserving symmetry.

## Change of basis

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Change_of_basis)

### Change-of-basis matrix

↑ **Parent:** [Change of basis](#change-of-basis)

If the columns of $P$ are the new basis vectors written in the old basis, coordinate columns satisfy $[v]_{\rm old}=P[v]_{\rm new}$. A linear operator's matrices are related by $A_{\rm new}=P^{-1}A_{\rm old}P$.

## Circulant matrix

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circulant_matrix)

## Invertible matrix

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Invertible_matrix)

### Singular matrix

↑ **Parent:** [Invertible matrix](#invertible-matrix)

A square matrix is singular when it is not [invertible](#invertible-matrix), equivalently when its [determinant](#determinant) is zero or its [kernel](#kernel-of-a-linear-map) is nontrivial.

## Kernel of a linear map

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kernel_of_a_linear_map)

### Nullity of a linear map

↑ **Parent:** [Kernel of a linear map](#kernel-of-a-linear-map)

The [nullity](#nullity-of-a-linear-map) is the [dimension](vector-space.md#dimension-vector-space) of the [kernel of a linear map](#kernel-of-a-linear-map). It counts independent directions annihilated by that map. For a finite-dimensional domain, the [rank-nullity theorem](#rank-nullity-theorem) gives $n(T)+r(T)=\dim V$.

### Trivial kernel

↑ **Parent:** [Kernel of a linear map](#kernel-of-a-linear-map)

A linear map has trivial kernel when its kernel is $\{0\}$. This is equivalent to the map being [injective](algebra.md#injective-function).

### Rank-nullity theorem

↑ **Parent:** [Kernel of a linear map](#kernel-of-a-linear-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rank-nullity_theorem)

For a linear map $T:V\to W$ with finite-dimensional domain,

$$
\dim V=\dim\ker T+\dim\operatorname{im}T.
$$

If a basis of $\ker T$ is extended to a basis of $V$, the images of the added basis vectors form a basis of $\operatorname{im}T$. Counting the two parts proves the formula.

#### Equality in the rank-sum and nullity-product inequalities

↑ **Parent:** [Rank-nullity theorem](#rank-nullity-theorem)

For [endomorphisms](algebra.md#endomorphism) $S,T$ of a finite-dimensional space of [dimension](vector-space.md#dimension-vector-space) $d$, $r(S+T)\le r(S)+r(T)$ and $n(ST)\le n(S)+n(T)$. If both equalities hold, the first gives $r(S)+r(T)\le d$, while the second gives $2d-r(S)-r(T)\le d$. Thus the [rank](#rank-one-quadratic-form) sum is $d$, $S+T$ is an [isomorphism](algebra.md#isomorphism), and $ST=0$. Conversely, $ST=0$ implies $\operatorname{im}T\subseteq\ker S$ and hence [rank](#rank-one-quadratic-form) sum at most $d$, whereas invertibility of $S+T$ gives [rank](#rank-one-quadratic-form) sum at least $d$. This proves both equalities.

#### Kernel jump in a parameter-dependent linear map

↑ **Parent:** [Rank-nullity theorem](#rank-nullity-theorem)

For a matrix whose entries depend on a parameter, a nonzero maximal minor certifies a fixed [matrix rank](vector-space.md#matrix-rank) away from its zeros. At a zero, other minors must still be checked: one vanishing minor does not itself imply a rank drop. Once the [matrix rank](vector-space.md#matrix-rank) is determined, the [rank-nullity theorem](#rank-nullity-theorem) gives the dimension of the [kernel of a linear map](#kernel-of-a-linear-map). Exceptional parameters can then be solved separately to exhibit the additional [kernel of a linear map](#kernel-of-a-linear-map) directions.

## Cokernel

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cokernel)

For a linear map $T:V\to W$, the cokernel is the quotient $\operatorname{coker}T=W/\operatorname{im}T$. The same definition applies to a homomorphism of [abelian groups](group.md#abelian-group).

## Dual space

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_space)

The dual space of a vector space $V$ over $F$ is $V^*=\operatorname{Hom}_F(V,F)$. If $V$ is finite-dimensional, then $\dim V^*=\dim V$.

### Algebraic dual of a direct sum

↑ **Parent:** [Dual space](#dual-space)

Restricting a [linear functional](#linear-functional) to each summand gives a family of functionals, with no finite-support restriction. Conversely an arbitrary such family acts on a vector by the finite sum of its nonzero coordinates. These constructions are inverse and prove the displayed algebraic [dual space](#dual-space) identity. A group action on the summands induces the product action by their algebraic contragredients.

### Bidual of a normed space

↑ **Parent:** [Dual space](#dual-space)

The bidual of a [normed vector space](functional-analysis.md#normed-vector-space) $X$ is the continuous dual $X^{**}=(X^*)^*$. Evaluation defines the [canonical embedding into the bidual](functional-analysis.md#canonical-embedding-into-the-bidual) $J_X(x)(f)=f(x)$. The [norm](functional-analysis.md#norm) inequality gives $\|J_Xx\|\le\|x\|$, and a norming functional from the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) gives equality. Thus $J_X$ is isometric, and its image is dense in its closure, a [completion of a normed space](functional-analysis.md#completion-of-a-normed-space).

### Perfect pairing

↑ **Parent:** [Dual space](#dual-space)

For finite-dimensional [vector spaces](vector-space.md) $V,W$ over a [field](algebra.md#field) $F$, a bilinear pairing $B:V\times W\to F$ is perfect when the induced [linear maps](vector-space.md#linear-map) $V\to W^*$ and $W\to V^*$ are [isomorphisms](algebra.md#isomorphism). Equivalently, both dimensions agree and the matrix of the pairing in any two bases is invertible. The evaluation pairing between a finite-dimensional [vector space](vector-space.md) and its [dual space](#dual-space) is perfect. This notion allows two different spaces; a [nondegenerate bilinear form](#nondegenerate-bilinear-form) is the case $V=W$.

### Separating subspace of an algebraic dual

↑ **Parent:** [Dual space](#dual-space)

A [linear subspace](vector-space.md#vector-subspace) $W\subseteq X^*$ is separating if every nonzero $x\in X$ has $T(x)\ne0$ for some $T\in W$. For finite-dimensional $X$, an evaluation map $X\to F^{\dim W}$ is [injective](algebra.md#injective-function), so the [rank-nullity theorem](#rank-nullity-theorem) forces $\dim W\geq\dim X=\dim X^*$ and $W=X^*$. For the infinite-dimensional [polynomial](polynomial.md) space, the span of its coefficient functionals is a proper separating [linear subspace](vector-space.md#vector-subspace) of the [dual space](#dual-space), which contains all sequences of coefficients, not just finitely supported ones.

### Bidual evaluation map

↑ **Parent:** [Dual space](#dual-space)

For an algebraic [dual space](#dual-space) $X^*=\operatorname{Hom}_F(X,F)$, the [linear map](vector-space.md#linear-map) $J:X\to X^{**}$ sends $x$ to evaluation at $x$. It is [injective](algebra.md#injective-function) because [linear functionals](#linear-functional) separate nonzero vectors: extend any nonzero vector to a [basis](vector-space.md#basis) and use its coordinate functional. If $X$ has a finite [basis](vector-space.md#basis) $e_i$ with [dual basis](#dual-basis) $e_i^*$, every $B\in X^{**}$ equals $J(\sum_iB(e_i^*)e_i)$, so $J$ is an [isomorphism](algebra.md#isomorphism). For infinite-dimensional spaces, [surjection](algebra.md#surjective-function) does not follow from this finite sum argument.

### Covector

↑ **Parent:** [Dual space](#dual-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Covector)

A covector is an element of the [dual space](#dual-space), hence a [linear functional](#linear-functional) on a vector space.

### Linear functional

↑ **Parent:** [Dual space](#dual-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_functional)

A linear functional is a linear map from a vector space to its scalar field.

#### Minimizing a linear functional on a sphere

↑ **Parent:** [Linear functional](#linear-functional)

For a nonzero Euclidean vector $w$, the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $z\cdot w\geq-\|w\|$ when $\|z\|=1$. Equality is attained uniquely at $z=-w/\|w\|$. On a sphere of radius $r>0$ the minimizer is $-rw/\|w\|$, and the minimum is $-r\|w\|$. This turns many constrained vector problems into a normalization of one fixed vector. If $w=0$, every point minimizes the functional.

#### Discontinuous functional detected by vanishing sequence tails

↑ **Parent:** [Linear functional](#linear-functional)

If a [linear functional](#linear-functional) on a [normed vector space](functional-analysis.md#normed-vector-space) has $f(v_N)=1$ for a sequence tending to zero in norm, it is discontinuous and unbounded. An explicit example is the algebraic span in $\ell^2$ of the coordinate vectors and $w=(2^{-n})_{n\geq1}$. Define $f(w)=1$ and $f(e_n)=0$. The tails $v_N=w-\sum_{n=1}^N2^{-n}e_n$ have norm $2^{-N}/\sqrt3$ but image one. Thus the functional vanishes on the dense finite-support subspace while being nonzero elsewhere.

### Dual basis

↑ **Parent:** [Dual space](#dual-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_basis)

For a basis $e_1,\ldots,e_n$ of $V$, its dual basis $e_1^*,\ldots,e_n^*$ is characterized by $e_i^*(e_j)=\delta_{ij}$.

#### Factorial monomial basis for polynomial differentiation

↑ **Parent:** [Dual basis](#dual-basis)

On polynomials of degree at most $n$, the derivative-evaluation functionals $e_j(\phi)=\phi^{(j)}(0)$ are dual to $p_j=x^j/j!$, since $e_i(p_j)=\delta_{ij}$. Differentiation maps $p_j$ to $p_{j-1}$, with $p_0$ mapped to zero. Its matrix is a single nilpotent Jordan block with ones above the diagonal, and its dual has the transpose matrix.

### Annihilator of a vector subspace

↑ **Parent:** [Dual space](#dual-space)

For $U\leq V$,

$$
U^\circ=\{f\in V^*:f|_U=0\}.
$$

In finite dimensions, $\dim U^\circ=\dim V-\dim U$.

### Transpose of a linear map

↑ **Parent:** [Dual space](#dual-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transpose_of_a_linear_map)

The dual of $\alpha:V\to W$ is $\alpha^*:W^*\to V^*$ defined by $\alpha^*(g)=g\circ\alpha$. In finite dimensions,

$$
\ker\alpha^*=(\operatorname{im}\alpha)^\circ,
\qquad
\operatorname{im}\alpha^*=(\ker\alpha)^\circ.
$$

#### Dual image and kernel annihilator identity

↑ **Parent:** [Transpose of a linear map](#transpose-of-a-linear-map)

For a [linear map](vector-space.md#linear-map) between finite-dimensional [vector spaces](vector-space.md), the image of its [dual map](#transpose-of-a-linear-map) is the [annihilator of a vector subspace](#annihilator-of-a-vector-subspace) given by its kernel. Inclusion follows by composition. Conversely a [linear functional](#linear-functional) vanishing on the kernel descends to the image and extends to the target by [basis extension](vector-space.md#basis-extension). The identity and the [rank-nullity theorem](#rank-nullity-theorem) show that a linear map and its dual have equal rank.

#### Equality of row rank and column rank

↑ **Parent:** [Transpose of a linear map](#transpose-of-a-linear-map)

For the map represented by a matrix $A$, column rank is the rank of the map and row rank is the rank of its dual. Since the dual map has kernel equal to the annihilator of the original image, rank-nullity gives equal ranks.

##### Simultaneous basis exchange from a nonzero minor

↑ **Parent:** [Equality of row rank and column rank](#equality-of-row-rank-and-column-rank)

If the columns $v_1,\ldots,v_m$ of an $n$ by $m$ matrix are independent, some $m$ by $m$ row minor is nonzero. A nonzero term of that minor's determinant selects distinct nonzero coordinates $f(i)$, and replacing the corresponding standard basis vectors $e_{f(i)}$ by the $v_i$ leaves a basis.

#### Duals of a subspace and its quotient

↑ **Parent:** [Transpose of a linear map](#transpose-of-a-linear-map)

For a finite-dimensional vector space and $U\leq V$, dualizing the quotient and inclusion maps gives

$$
(V/U)^*\cong U^\circ,
\qquad
U^*\cong V^*/U^\circ.
$$

### Surjectivity of independent linear functionals

↑ **Parent:** [Dual space](#dual-space)

If $q_1,\ldots,q_n\in V^*$ are linearly independent, then

$$
x\longmapsto(q_1(x),\ldots,q_n(x))
$$

maps $V$ onto $F^n$. Otherwise a nonzero functional annihilating its proper image would give a nontrivial linear relation among the $q_j$.

### Polynomial moment functional

↑ **Parent:** [Dual space](#dual-space)

A polynomial moment functional evaluates a polynomial through a weighted integral, such as $p\mapsto\int p(t)w(t)dt$; finitely many moments determine it on a bounded-degree polynomial space.

## Rank of a matrix with affine columns

↑ **Parent:** [Linear algebra](linear-algebra.md)

If the $j$th column of a matrix is $v+c_j\mathbf1$, then its image lies in $\operatorname{span}\{v,\mathbf1\}$. If $v$ is not constant and at least two $c_j$ differ, the rank is exactly two; for $m$ columns the nullity is $m-2$.

## Matrix determinant lemma

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_determinant_lemma)

## Permanent (mathematics)

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Permanent_(mathematics))

For an $n\times n$ matrix $A=(a_{ij})$, its permanent is

$$
\operatorname{perm}A=\sum_{\sigma\in S_n}\prod_{i=1}^n a_{i,\sigma(i)}.
$$

It resembles the [determinant](#determinant) without the signs of the permutations.

### Dense permanent approximation

↑ **Parent:** [Permanent (mathematics)](#permanent-mathematics)

If every row and column of an $n$-by-$n$ zero-one [matrix](vector-space.md#matrix) has more than $n/2$ ones, its [permanent of a matrix](#permanent-mathematics) has a [fully polynomial randomized approximation scheme](mathematical-optimization.md#fully-polynomial-randomized-approximation-scheme). The [short augmenting paths in a dense bipartite graph](graph-theory.md#short-augmenting-paths-in-a-dense-bipartite-graph) bound makes the leading coefficient dominate the [matching generating function](graph-theory.md#matching-generating-function) at polynomially large activity. The [weighted matching Markov chain](markov-process.md#weighted-matching-markov-chain) samples polynomially bounded activities in polynomial [mixing time](markov-process.md#mixing-time-of-a-markov-chain). Estimate successive [annealing ratios for a matching generating function](graph-theory.md#annealing-ratios-for-a-matching-generating-function) and divide by the final activity to the power $n$.

## Matrix inverse

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_inverse)

A matrix inverse satisfies $AA^{-1}=A^{-1}A=I$.

### Block matrix inverse

↑ **Parent:** [Matrix inverse](#matrix-inverse)

The inverse of a block matrix can be expressed through the inverse of one diagonal block and the inverse of its [Schur complement](#schur-complement). This reduces many deletion and conditioning identities to smaller matrix inversions.

<h3 id="sherman-morrison-formula">Sherman–Morrison formula</h3>

↑ **Parent:** [Matrix inverse](#matrix-inverse)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sherman–Morrison_formula)

If $A$ is invertible and $1+v^TA^{-1}u\ne0$, then

$$
(A+uv^T)^{-1}
=A^{-1}-\frac{A^{-1}uv^TA^{-1}}{1+v^TA^{-1}u}.
$$

### Moore-Penrose inverse

↑ **Parent:** [Matrix inverse](#matrix-inverse)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moore-Penrose_inverse)

The Moore-Penrose inverse is the unique matrix $A^+$ satisfying $AA^+A=A$, $A^+AA^+=A^+$, and symmetry of $AA^+$ and $A^+A$. If $A=UDV^T$ is a singular value decomposition, then $A^+=VD^+U^T$.

<h4 id="moore-penrose-inverse-of-a-hilbert-space-operator">Moore--Penrose inverse of a Hilbert-space operator</h4>

↑ **Parent:** [Moore-Penrose inverse](#moore-penrose-inverse)

For a bounded operator $A:X\to Y$ between [Hilbert spaces](hilbert-space.md), $A^\dagger$ has domain $\mathcal R(A)\oplus\mathcal R(A)^\perp$, maps into $\mathcal N(A)^\perp$, and inverts the restriction of $A$ to $\mathcal N(A)^\perp$. It is bounded exactly when $\mathcal R(A)$ is closed.

#### Penrose equations

↑ **Parent:** [Moore-Penrose inverse](#moore-penrose-inverse)

The Moore--Penrose inverse is characterized by

$$
AA^\dagger A=A,
\quad
A^\dagger AA^\dagger=A^\dagger,
\quad
(AA^\dagger)^*=AA^\dagger,
\quad
(A^\dagger A)^*=A^\dagger A.
$$

<h4 id="reverse-order-law-for-the-moore-penrose-inverse">Reverse-order law for the Moore--Penrose inverse</h4>

↑ **Parent:** [Moore-Penrose inverse](#moore-penrose-inverse)

The identity $(AB)^\dagger=B^\dagger A^\dagger$ does not hold for arbitrary matrices. A sufficient condition is that $A$ have [full column rank](vector-space.md#full-column-rank) and $B$ have [full row rank](vector-space.md#full-row-rank).

### Push-through identity

↑ **Parent:** [Matrix inverse](#matrix-inverse)

For a rectangular matrix $X$ and $\lambda>0$,

$$
X^T(XX^T+\lambda I)^{-1}=(X^TX+\lambda I)^{-1}X^T.
$$

Multiplying either side by $XX^T+\lambda I$ verifies the identity.

## Matrix similarity

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_similarity)

Square matrices $A$ and $B$ are similar when $B=P^{-1}AP$ for some invertible matrix $P$. They represent the same linear operator in different bases and therefore have the same [Jordan normal form](linear-operator-theory.md#jordan-normal-form).

### Similarity transformation

↑ **Parent:** [Matrix similarity](#matrix-similarity)

A similarity transformation sends a square matrix $A$ to $SAS^{-1}$ for an invertible matrix $S$. It changes the basis of a linear operator and preserves its characteristic polynomial and eigenvalues.

#### Positive diagonal symmetrization of a matrix

↑ **Parent:** [Similarity transformation](#similarity-transformation)

If a real [matrix](vector-space.md#matrix) $B$ has a positive [diagonal matrix](#diagonal-matrix) $W$ such that $WB$ is a [symmetric matrix](#symmetric-matrix), then $H=W^{1/2}BW^{-1/2}$ is a [symmetric matrix](#symmetric-matrix) related to $B$ by a [similarity transformation](#similarity-transformation): $B^TW=WB$ gives $H^T=H$. Thus $B$ is a [diagonalizable matrix](linear-operator-theory.md#diagonalizable-matrix) with real [eigenvalues](linear-operator-theory.md#eigenvalue). If $\mathbf z^TWB\mathbf z\le0$ for all real [vectors](vector-space.md#vector) $\mathbf z$, its [eigenvalues](linear-operator-theory.md#eigenvalue) are nonpositive. This converts symmetry in a weighted [inner product](#inner-product) into Euclidean symmetry.

#### Every automorphism of a full matrix algebra is inner

↑ **Parent:** [Similarity transformation](#similarity-transformation)

Every unital algebra automorphism $F:M_n(\mathbb C)\to M_n(\mathbb C)$ has the form $F(X)=SXS^{-1}$ for some invertible $S$. One proof transports the matrix units through $F$, chooses compatible bases for their rank-one images, and reconstructs the common similarity transformation.

### Transpose similarity

↑ **Parent:** [Matrix similarity](#matrix-similarity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transpose_similarity)

Every square matrix over a field is similar to its transpose.

### Real similarity from complex similarity

↑ **Parent:** [Matrix similarity](#matrix-similarity)

If real matrices satisfy $C=SDS^{-1}$ for an invertible complex $S=X+iY$, then $CS=SD$, so both real matrices $X,Y$ intertwine $C$ and $D$. Since $\det(X+tY)$ is a nonzero real polynomial, some real $t$ makes $X+tY$ invertible and supplies a real similarity.

## Matrix trace

↑ **Parent:** [Linear algebra](linear-algebra.md)

The trace is the sum of diagonal entries,

$$
\operatorname{tr}A=\sum_iA_{ii}.
$$

Index interchange proves $\operatorname{tr}(AB)=\operatorname{tr}(BA)$ and hence cyclic invariance under any cyclic permutation of a product.

### Scalar square of a traceless two-by-two matrix

↑ **Parent:** [Matrix trace](#matrix-trace)

A two-by-two [matrix](vector-space.md#matrix) $M$ with zero [trace](#matrix-trace) satisfies $M^2=-(\det M)I$ by the [Cayley-Hamilton theorem](mathematics.md#cayley-hamilton-theorem). Over the [complex numbers](complex-analysis.md#complex-number), either $\det M\ne0$ and its two distinct [eigenvalues](linear-operator-theory.md#eigenvalue) make it diagonalizable, or $M^2=0$. A matrix commutator has zero trace, so this alternative applies to it. Diagonalization over the real numbers need not follow when $-\det M<0$.

### Nilpotence from vanishing traces of powers

↑ **Parent:** [Matrix trace](#matrix-trace)

For a complex $n$ by $n$ [matrix](vector-space.md#matrix), triangularization gives $\operatorname{tr}(A^k)=\sum_j\lambda_j^k$. The [zero power sums force a finite complex multiset to vanish](galois-theory.md#zero-power-sums-force-a-finite-complex-multiset-to-vanish) criterion makes every diagonal eigenvalue zero. A strictly upper-triangular $n$ by $n$ matrix has zero $n$th power: every nonzero product entry would require $n$ strictly increasing index steps. [Similarity](#matrix-similarity) then gives $A^n=0$.

### Trace orthogonality nilpotence lemma

↑ **Parent:** [Matrix trace](#matrix-trace)

Let $U\subseteq W\subseteq\operatorname{End}_{\mathbb C}(V)$ be [vector subspaces](vector-space.md#vector-subspace) and $M=\{T:[T,W]\subseteq U\}$. If $\alpha\in M$ and $\operatorname{tr}(\alpha\beta)=0$ for all $\beta\in M$, then $\alpha$ is a [nilpotent endomorphism](linear-operator-theory.md#nilpotent-linear-map).

To prove it, let $\beta$ act by $\overline\lambda$ on the [generalized eigenspace](linear-operator-theory.md#generalized-eigenspace) of $\alpha$ of [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda$. [Polynomial interpolation](numerical-analysis.md#polynomial-interpolation) on eigenvalue differences, together with [adjoint compatibility of additive Jordan decomposition](linear-operator-theory.md#adjoint-compatibility-of-additive-jordan-decomposition), expresses $\operatorname{ad}\beta$ as a [polynomial](polynomial.md) in $\operatorname{ad}\alpha$ with zero constant term. Since $\operatorname{ad}\alpha$ maps $W$ into $U$ and preserves $U$, this gives $\beta\in M$. Taking the [matrix trace](#matrix-trace) on each [generalized eigenspace](linear-operator-theory.md#generalized-eigenspace) yields $0=\sum_\lambda\dim(V_\lambda)|\lambda|^2$, so every [eigenvalue](linear-operator-theory.md#eigenvalue) is zero. This is the linear-algebra step behind the [Cartan solvability criterion](lie-algebra.md#cartan-solvability-criterion); $U,W$ need not be Lie subalgebras.

### Trace is the unique normalized cyclic linear functional

↑ **Parent:** [Matrix trace](#matrix-trace)

Over $\mathbb R$ or $\mathbb C$, every [linear functional](#linear-functional) on all $n\times n$ [matrices](vector-space.md#matrix) satisfying $f(AB)=f(BA)$ is a scalar multiple of the [trace](#matrix-trace). The [matrix units](vector-space.md#matrix-unit) show that the functional vanishes off the diagonal and has equal values on every diagonal unit. The normalization $f(I)=n$ fixes the scalar to one.

### Traceless matrix

↑ **Parent:** [Matrix trace](#matrix-trace)

A traceless matrix is a square [matrix](vector-space.md#matrix) whose [trace](#matrix-trace) is zero. Such [matrices](vector-space.md#matrix) form the [kernel](#kernel-of-a-linear-map) of the trace [linear functional](#linear-functional).

#### Traceless matrices are spanned by commutators

↑ **Parent:** [Traceless matrix](#traceless-matrix)

Every [commutator](lie-algebra.md#commutator) of square [matrices](vector-space.md#matrix) is traceless by cyclicity of the [trace](#matrix-trace). Conversely, off-diagonal [matrix units](vector-space.md#matrix-unit) and differences of diagonal units are themselves [commutators](lie-algebra.md#commutator) and span all [traceless matrices](#traceless-matrix). This proves equality with the linear span of commutators, without needing a theorem about representation as one commutator.

### Cyclic property of the trace

↑ **Parent:** [Matrix trace](#matrix-trace)

For square matrices whose product is defined, $\operatorname{tr}(A_1A_2\cdots A_n)$ is unchanged by a cyclic permutation of the factors. In particular, every [commutator](lie-algebra.md#commutator) has trace zero.

<h2 id="linear-operator-theory">Operator theory</h2>

↑ **Parent:** [Linear algebra](linear-algebra.md)

[This section is present in another page, follow this link to view it.](linear-operator-theory.md)

## Multilinear algebra

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multilinear_algebra)

Multilinear algebra studies maps linear in each of several arguments, including determinants, tensors, and exterior products.

### Coalgebra

↑ **Parent:** [Multilinear algebra](#multilinear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coalgebra)

A [comonoid](category-theory.md#comonoid) in the [monoidal category](category-theory.md#monoidal-category) of [modules](module-theory.md#module-mathematics) over a [commutative ring](commutative-algebra.md#commutative-ring), with tensor $\otimes_k$ and unit $k$.

#### Coideal

↑ **Parent:** [Coalgebra](#coalgebra)

A [linear subspace](vector-space.md#vector-subspace) $I$ of a [coalgebra](#coalgebra) satisfying the displayed conditions. These are exactly the conditions for the [comultiplication](category-theory.md#comultiplication) and [counit](category-theory.md#counit) to descend to the quotient [vector space](vector-space.md) $C/I$. An ideal that is also a coideal in a [bialgebra](commutative-algebra.md#bialgebra) gives a quotient [bialgebra](commutative-algebra.md#bialgebra).

#### Measuring coalgebra

↑ **Parent:** [Coalgebra](#coalgebra)

For unital [algebras over a field](algebra.md#algebra-over-a-field) $A,B$, a [coalgebra](#coalgebra) $C$ measures $A$ into $B$ when a linear map $p:C\to\operatorname{Hom}_k(A,B)$ satisfies the displayed identity and $p(c)(1_A)=\varepsilon(c)1_B$. [Group-like elements](#group-like-element) therefore act by unital [algebra homomorphisms over a field](algebra.md#algebra-homomorphism-over-a-field).

##### Universal measuring coalgebra

↑ **Parent:** [Measuring coalgebra](#measuring-coalgebra)

A terminal [measuring coalgebra](#measuring-coalgebra): every measuring map from $C$ factors uniquely through its universal measuring map by a [coalgebra](#coalgebra) homomorphism $C\to P(A,B)$. Composition of universal measurings makes $P(A,A)$ a [bialgebra](commutative-algebra.md#bialgebra), with the identity map providing its unit.

#### Group-like element

↑ **Parent:** [Coalgebra](#coalgebra)

An element of a [coalgebra](#coalgebra) satisfying the displayed identities. A [group-like element](#group-like-element) in a [Hopf algebra](algebra.md#hopf-algebra) is invertible with inverse its [antipode](algebra.md#antipode) image.

#### Comodule

↑ **Parent:** [Coalgebra](#coalgebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Comodule)

A right comodule is an object $M$ with a [coaction](#coaction) $\rho:M\to M\otimes C$ satisfying the coassociativity and [counit](category-theory.md#counit) laws. This definition extends from [coalgebras](#coalgebra) to [comonoids](category-theory.md#comonoid) in a [monoidal category](category-theory.md#monoidal-category).

##### Comodule tensor transformation formula

↑ **Parent:** [Comodule](#comodule)

A natural underlying transformation of tensor bifunctors on right [comodules](#comodule) over a [field](algebra.md#field) has components $\varphi_{M,N}(u\otimes v)=\sum u_{(0)}\otimes v_{(0)}\gamma(u_{(1)},v_{(1)})$. Recover $\gamma=(\varepsilon\otimes\varepsilon)\varphi_{H,H}$; colinearity and monoidal axioms impose further equations.

###### Multiplication compatibility for a comodule tensor transformation

↑ **Parent:** [Comodule tensor transformation formula](#comodule-tensor-transformation-formula)

For a transformation from the tensor built using $n$ to the tensor built using $m$, colinearity is $m*\gamma=\gamma*n$: $\sum m(a_{(1)},b_{(1)})\gamma(a_{(2)},b_{(2)})=\sum\gamma(a_{(1)},b_{(1)})n(a_{(2)},b_{(2)})$. Scalar maps enter this [convolution product for coalgebra maps](#convolution-product-for-coalgebra-maps) via the common algebra unit.

##### Corestriction functor for comodules

↑ **Parent:** [Comodule](#comodule)

A [comonoid morphism](category-theory.md#comonoid-morphism) $f:H\to K$ induces a [functor](category.md#functor) $f_*$ on right [comodules](#comodule), replacing $\rho$ by $(1\otimes f)\rho$ and preserving underlying objects and arrows. For [bimonoids](category-theory.md#bimonoid), it is strict monoidal exactly when $f$ is also a [monoid morphism](category-theory.md#monoid-morphism).

###### Comodule natural transformation formula

↑ **Parent:** [Corestriction functor for comodules](#corestriction-functor-for-comodules)

A [natural transformation](category.md#natural-transformation) between corestriction functors over a [field](algebra.md#field) has components $\beta_M(u)=\sum u_{(0)}\alpha(u_{(1)})$, recovered by $\alpha=\varepsilon\beta_H$. Monoidality forces $\alpha$ to be a unital [algebra homomorphism over a field](algebra.md#algebra-homomorphism-over-a-field); for a [Hopf algebra](algebra.md#hopf-algebra), $\alpha S$ supplies the inverse.

##### Coaction

↑ **Parent:** [Comodule](#comodule)

The structure map of a [comodule](#comodule); a right coaction satisfies $(\rho\otimes1)\rho=(1\otimes\Delta)\rho$ with coherent parentheses, and $(1\otimes\varepsilon)\rho$ is the inverse right [unitor](category-theory.md#unitor).

#### Convolution product for coalgebra maps

↑ **Parent:** [Coalgebra](#coalgebra)

For a [coalgebra](#coalgebra) $C$ and a unital associative [algebra over a commutative ring](commutative-algebra.md#algebra-over-a-commutative-ring) $A$, maps $f,g:C\to A$ have convolution $f*g=m_A(f\otimes g)\Delta_C$, with unit $j_A\varepsilon_C$. The two-sided convolution inverse of $1_H$ is the [antipode](algebra.md#antipode).

#### Sweedler notation

↑ **Parent:** [Coalgebra](#coalgebra)

The notation $\Delta h=\sum h_{(1)}\otimes h_{(2)}$ suppresses the summation index of a [comultiplication](category-theory.md#comultiplication); iterated indices use coassociativity. For a [comodule](#comodule), write $\rho(u)=\sum u_{(0)}\otimes u_{(1)}$.

### Multilinear map

↑ **Parent:** [Multilinear algebra](#multilinear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multilinear_map)

A [multilinear map](#multilinear-map) $F:V_1\times\cdots\times V_r\to W$ is a map between [vector spaces](vector-space.md) that is linear in each argument when all other arguments are fixed. For example the evaluation $(\omega,v)\mapsto\omega(v)$ is bilinear, and the [determinant](#determinant) is multilinear in its columns. The [universal property of a tensor product](#universal-property-of-a-tensor-product) replaces this separate linearity by a single [linear map](vector-space.md#linear-map) from $V_1\otimes\cdots\otimes V_r$.

#### Bilinear map

↑ **Parent:** [Multilinear map](#multilinear-map)

A bilinear map is a map $B:V\times W\to U$ between [vector spaces](vector-space.md) that is [linear](vector-space.md#linearity) in each argument when the other is fixed. The nonlinear [temperature](thermodynamics.md#temperature) [advection](fluid-mechanics.md#advection) can be written as the diagonal of a bilinear map, $\mathcal N(\phi,\chi)=-\mathbf u[\phi]\cdot\nabla\chi$, when [velocity](classical-mechanics.md#velocity) depends linearly on [temperature](thermodynamics.md#temperature). Unlike a [bilinear form](#bilinear-form), its output need not be a scalar.

##### Bilinearity

↑ **Parent:** [Bilinear map](#bilinear-map)

A map $B:V\times W\to Z$ between [vector spaces](vector-space.md) is bilinear when it is [linear](vector-space.md#linearity) in either argument with the other held fixed. A scalar-valued [bilinear form](#bilinear-form) is the case $V=W$ and $Z$ is the scalar field. Checking [bilinearity](#bilinearity) is one of the algebraic steps in verifying a real [inner product](#inner-product); being a [symmetric bilinear form](#symmetric-bilinear-form) and having positive squared [norm](functional-analysis.md#norm) impose further conditions.

##### Symmetric bilinear diagonal-parallel lemma

↑ **Parent:** [Bilinear map](#bilinear-map)

Let $S:W\times W\to W$ be a symmetric [bilinear map](#bilinear-map) on a finite-dimensional real [vector space](vector-space.md). If $S(v,v)$ is parallel to $v$ for every $v$, then it has the displayed form for one [covector](#covector) $V$. Write $S(e_i,e_i)=\alpha_i e_i$ in a [basis](vector-space.md#basis). Applying the condition to $e_i+e_j$ and $e_i-e_j$ excludes every component outside their span and gives $S(e_i,e_j)=(\alpha_j e_i+\alpha_i e_j)/2$. Set $V(e_i)=\alpha_i/2$ and extend by [bilinearity](#bilinearity). Dimension one follows by the same definition. The [trace](#matrix-trace) identity $S^a{}_{ac}=(n+1)V_c$ proves uniqueness without depending on the chosen [basis](vector-space.md#basis).

##### Derivative of a continuous bilinear map

↑ **Parent:** [Bilinear map](#bilinear-map)

A continuous bilinear map obeys $\|f(h,k)\|\le C\|h\|\|k\|$. Expanding $f(a+h,b+k)$ leaves the displayed linear term and remainder $f(h,k)$. For product [norm](functional-analysis.md#norm) $\rho=(\|h\|^2+\|k\|^2)^{1/2}$, the remainder has [norm](functional-analysis.md#norm) at most $C\rho^2/2$, hence is $o(\rho)$. This proves the [Fréchet derivative](calculus.md#frechet-derivative) formula.

##### Rank bound for a nonsingular complex bilinear map

↑ **Parent:** [Bilinear map](#bilinear-map)

Let $U,V$ be nonzero finite-dimensional complex [vector spaces](vector-space.md), and let $\phi:U\otimes V\to W$ have injective restrictions when either nonzero factor is fixed. It induces a map from $\mathbb{CP}^{a-1}\times\mathbb{CP}^{b-1}$ to $\mathbb{CP}^{r-1}$, where $a=\dim U$, $b=\dim V$, and $r=\operatorname{rank}\phi$. Pullback of the degree-two generator is $x+y$, since both factor restrictions are projective linear embeddings. Its $(a+b-2)$th power is $\binom{a+b-2}{a-1}x^{a-1}y^{b-1}\ne0$ in integral [cohomology](cohomology.md). The target must therefore have complex dimension at least $a+b-2$. Positivity of both factor dimensions is necessary; a zero factor can make the claimed inequality false.

##### Complex bilinear dimension bound

↑ **Parent:** [Bilinear map](#bilinear-map)

For nonzero finite-dimensional complex [vector spaces](vector-space.md) $U,V$, suppose a [bilinear map](#bilinear-map) never vanishes on a pair of nonzero vectors. Equivalently, each map obtained by fixing one nonzero argument is injective. If its associated map on $U\otimes V$ has image dimension $r$, projectivization gives a map to $\mathbb{CP}^{r-1}$ whose positive degree-two class pulls back to $x+y$. The nonzero top power $(x+y)^{\dim U+\dim V-2}$ in the product [cohomology ring of complex projective space](algebraic-topology.md#cohomology-ring-of-complex-projective-space) proves the bound. Multiplication of polynomials of bounded degree attains equality. Nonzero hypotheses matter: with a zero factor, slice conditions can be vacuous.

### Alternating multilinear map

↑ **Parent:** [Multilinear algebra](#multilinear-algebra)

An alternating multilinear map vanishes whenever two arguments are equal. Swapping two arguments reverses its sign.

#### Alternating trilinear form

↑ **Parent:** [Alternating multilinear map](#alternating-multilinear-map)

An alternating trilinear form is a scalar-valued map, linear in three arguments, which vanishes whenever two arguments agree. In characteristic zero, interchanging two arguments negates its value, while cyclic permutation preserves it. For a [symmetric bilinear form](#symmetric-bilinear-form) $B$ on a [Lie algebra](lie-algebra.md), the tensor $B([x,y],z)$ is alternating exactly when $B$ is an [invariant bilinear form on a Lie algebra](lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra).

### Tensor product

↑ **Parent:** [Multilinear algebra](#multilinear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tensor_product)

The tensor product $V\otimes W$ of [vector spaces](vector-space.md) is generated by symbols $v\otimes w$ subject to bilinearity. It is characterized by the property that every bilinear map from $V\times W$ factors uniquely through a [linear map](vector-space.md#linear-map) from $V\otimes W$.

#### Universal property of a tensor product

↑ **Parent:** [Tensor product](#tensor-product)

For [vector spaces](vector-space.md) $V_1,\ldots,V_r$, every [multilinear map](#multilinear-map) $F:V_1\times\cdots\times V_r\to W$ factors uniquely through a [linear map](vector-space.md#linear-map) $\widetilde F:V_1\otimes\cdots\otimes V_r\to W$ sending a decomposable tensor to $F$ of its factors. Thus multilinear formulas define [linear maps](vector-space.md#linear-map) on [tensor products](#tensor-product) without choosing a basis. [Tensor contraction](#tensor-contraction) is an example, using the evaluation pairing between a vector and a [covector](#covector).

#### Tensor-product basis

↑ **Parent:** [Tensor product](#tensor-product)

If $\{e_i\}$ and $\{f_j\}$ are [bases](vector-space.md#basis) of finite-dimensional [vector spaces](vector-space.md) $V,W$, then $\{e_i\otimes f_j\}$ is a basis of $V\otimes W$. Bilinearity gives spanning, and applying products of dual coordinate functionals gives independence. Thus $\dim(V\otimes W)=\dim V\dim W$.

#### Tensor algebra

↑ **Parent:** [Tensor product](#tensor-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tensor_algebra)

The tensor algebra of a [vector space](vector-space.md) $V$ is the [graded algebra](commutative-algebra.md#graded-algebra)

$$
T(V)=\bigoplus_{n\geq0}V^{\otimes n},
$$

with multiplication given by concatenation of tensors.

##### Truncated tensor algebra

↑ **Parent:** [Tensor algebra](#tensor-algebra)

The truncated [tensor algebra](#tensor-algebra) discards products of degree greater than $N$. Its multiplication is $(a\otimes b)^{(k)}=\sum_{j=0}^k a^{(j)}\otimes b^{(k-j)}$. Every element with scalar part $1$ is invertible by a finite geometric series in its positive-degree part. Truncated exponential and logarithm are finite polynomials.

##### Tensor power

↑ **Parent:** [Tensor algebra](#tensor-algebra)

The nth tensor power is the iterated [tensor product of modules](module-theory.md#tensor-product-of-modules) $V^{\otimes n}=V\otimes\cdots\otimes V$.

###### Tensor square

↑ **Parent:** [Tensor power](#tensor-power)

The tensor square is the second [tensor power](#tensor-power) $V^{\otimes2}=V\otimes V$. Over a field of characteristic different from two it decomposes as the [direct sum](vector-space.md#direct-sum) of the [symmetric square](#symmetric-square) and [exterior square](#exterior-square).

##### Symmetric algebra

↑ **Parent:** [Tensor algebra](#tensor-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_algebra)

The symmetric algebra is the quotient of $T(V)$ by the ideal generated by $v\otimes w-w\otimes v$. It is graded by [symmetric powers](#symmetric-power):

$$
S(V)=\bigoplus_{n\geq0}S^nV.
$$

###### Symmetric power

↑ **Parent:** [Symmetric algebra](#symmetric-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_power)

The nth symmetric power $S^nV$ is the quotient of $V^{\otimes n}$ that identifies tensors differing by a permutation of their factors. Equivalently, over characteristic zero it is the subspace of symmetric tensors.

###### Weight-transfer proof of irreducibility of symmetric powers

↑ **Parent:** [Symmetric power](#symmetric-power)

In the [symmetric power](#symmetric-power) $\operatorname{Sym}^m\mathbb C^n$ of the defining [unitary group](topological-group.md#unitary-group) representation, diagonal [torus](topology.md#torus) weights are indexed by nonnegative integer tuples summing to $m$, with one monomial per [weight space](semisimple-lie-algebra.md#weight-space). Torus averaging extracts a monomial from any nonzero invariant complex subspace. The complexified [Lie algebra](lie-algebra.md) acts by $E_{ij}=x_i\partial_{x_j}$ on the symmetric algebra. Whenever $a_j>0$, the displayed action moves one unit of degree from $j$ to $i$ with nonzero coefficient. Finite transfers connect every degree-$m$ monomial, so the subspace is the entire representation. The case $m=0$ is the one-dimensional trivial representation. This proof needs neither the [Weyl character formula](semisimple-lie-algebra.md#weyl-character-formula) nor the [Weyl dimension formula](semisimple-lie-algebra.md#weyl-dimension-formula).

###### Symmetric powers of the three-dimensional SU2 representation

↑ **Parent:** [Symmetric power](#symmetric-power)

The three-dimensional irreducible [representation](representation-theory.md#group-representation) $V_2$ of [SU(2)](topological-group.md#su-2-group) has weights $2,0,-2$. Thus the [character](representation-theory.md#character-of-a-representation) of its $n$th [symmetric power](#symmetric-power) is $\sum_{a+b+c=n}t^{2(a-c)}$. Its weight $2\ell$ has multiplicity $\lfloor(n-|\ell|)/2\rfloor+1$ for $|\ell|\leq n$. Subtracting adjacent weight multiplicities gives one copy of each $V_{2n},V_{2n-4},\ldots$. The invariant subspace is one-dimensional for even $n$ and zero for odd $n$.

###### Character generating series of symmetric powers

↑ **Parent:** [Symmetric power](#symmetric-power)

For [eigenvalues](linear-operator-theory.md#eigenvalue) $\lambda_1,\ldots,\lambda_d$ of a finite-order linear action, its [symmetric power](#symmetric-power) characters satisfy $\sum_{n\geq0}\chi_{S^nV}t^n=\prod_j(1-\lambda_jt)^{-1}$. The denominator is the alternating generating [polynomial](polynomial.md) of its [exterior power](#exterior-power) characters.

###### Symmetric square

↑ **Parent:** [Symmetric power](#symmetric-power)

The symmetric square is the quotient of $V\otimes V$ by $v\otimes w-w\otimes v$, and records symmetric tensors of rank two.

###### Traceless symmetric square of the defining even orthogonal representation

↑ **Parent:** [Symmetric square](#symmetric-square)

For $n\geq2$, contraction with the invariant [symmetric bilinear form](#symmetric-bilinear-form) splits off the trivial line in the [symmetric square](#symmetric-square) of the defining [special orthogonal group](#special-orthogonal-group) [representation](representation-theory.md#group-representation). Its [null space](#kernel-of-a-linear-map) is the traceless [symmetric square](#symmetric-square). It contains a [highest-weight vector](semisimple-lie-algebra.md#highest-weight-vector) of [weight](semisimple-lie-algebra.md#weight-representation-theory) $2e_1$, and the [Weyl dimension formula](semisimple-lie-algebra.md#weyl-dimension-formula) gives $(n+1)(2n-1)$, exactly its [dimension](vector-space.md#dimension-vector-space). [Complete reducibility of compact-group representations](representation-theory.md#complete-reducibility-of-compact-group-representations) therefore makes that [null space](#kernel-of-a-linear-map) [irreducible](representation-theory.md#irreducible-representation). The entire [symmetric square](#symmetric-square) is reducible because of the invariant line.

###### Tensor-square decomposition of the defining even orthogonal representation

↑ **Parent:** [Traceless symmetric square of the defining even orthogonal representation](#traceless-symmetric-square-of-the-defining-even-orthogonal-representation)

For $V=\mathbb C^{2n}$, $n\geq3$, the [symmetric square](#symmetric-square) splits into an invariant line and its irreducible traceless part of highest weight $2\varepsilon_1$. The [exterior square of the defining orthogonal representation](semisimple-lie-algebra.md#exterior-square-of-the-defining-orthogonal-representation) is the adjoint module of highest weight $\varepsilon_1+\varepsilon_2$. For $n=2$, the exterior square splits instead into highest weights $\varepsilon_1-\varepsilon_2$ and $\varepsilon_1+\varepsilon_2$. This exception reflects that [so4 Lie algebra](semisimple-lie-algebra.md#so4-lie-algebra) is semisimple but not simple.

###### Symmetric square of a direct sum

↑ **Parent:** [Symmetric square](#symmetric-square)

Over every [field](algebra.md#field), including [characteristic two](algebra.md#characteristic-two), there is a natural isomorphism

$$
S^2(V\oplus W)\cong S^2V\oplus(V\otimes W)\oplus S^2W.
$$

The middle summand maps $v\otimes w$ to the mixed product $vw$. Monomial [bases](vector-space.md#basis) prove bijectivity, and the [Leibniz rule](calculus.md#leibniz-rule) makes the map equivariant for [Lie algebra representations](lie-algebra.md#lie-algebra-representation).

###### Symmetric trace-free square of the defining orthogonal representation

↑ **Parent:** [Symmetric square](#symmetric-square)

For the defining real representation of $SO(d)$, the [symmetric square](#symmetric-square) splits as a scalar trace plus symmetric trace-free tensors: $\operatorname{Sym}^2(\mathbb R^d)=\mathbb R\oplus\operatorname{Sym}_0^2(\mathbb R^d)$. The trace projection is $S\mapsto S-(\operatorname{tr}S)I/d$, so the second summand has dimension $d(d+1)/2-1$.

For $d\geq3$ the trace-free summand is an irreducible real [group representation](representation-theory.md#group-representation). To see this, diagonalize a nonzero symmetric trace-free matrix in a nonzero invariant subspace. Two diagonal entries differ. Infinitesimal rotation in their plane yields a nonzero symmetric off-diagonal matrix; rotations carry it to every coordinate pair, and a rotation through $\pi/4$ produces a difference of two diagonal entries. These off-diagonal matrices and diagonal differences span all symmetric trace-free matrices, so the invariant subspace is the whole summand. For $d=24$, its dimension is 299, the third-level nontrivial multiplet of the [lowest levels of a fully transverse ND bosonic string](string-theory.md#lowest-levels-of-a-fully-transverse-nd-bosonic-string).

### Exterior algebra

↑ **Parent:** [Multilinear algebra](#multilinear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exterior_algebra)

The exterior algebra is the graded algebra

$$
\Lambda^\bullet V=\bigoplus_{k=0}^{\dim V}\Lambda^kV
$$

with multiplication given by the antisymmetric wedge product.

#### Bivector

↑ **Parent:** [Exterior algebra](#exterior-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bivector)

A bivector is an antisymmetric contravariant tensor of degree two. A simple bivector is a single [exterior product](#exterior-product) $u\wedge v$. A general bivector is a sum of such products; in four dimensions simplicity is equivalent to $w\wedge w=0$ for a nonzero bivector. Covariant counterparts are [differential two-forms](differential-form.md#2-form).

#### Exterior product

↑ **Parent:** [Exterior algebra](#exterior-algebra)

The exterior product is the multiplication $\bigwedge^pV\otimes\bigwedge^qV\to\bigwedge^{p+q}V$ of the [exterior algebra](#exterior-algebra). For [homogeneous elements of a graded algebra](commutative-algebra.md#homogeneous-element-of-a-graded-algebra), $u\wedge v=(-1)^{pq}v\wedge u$.

#### Polynomial polyvector field

↑ **Parent:** [Exterior algebra](#exterior-algebra)

For a [polynomial ring](commutative-algebra.md#polynomial-ring) $A$, a degree-$p$ polynomial polyvector field is an element of $\bigwedge_A^p\operatorname{Der}_k(A)$. Its product is the [exterior product](#exterior-product). Together with the [Schouten-Nijenhuis bracket](#schouten-nijenhuis-bracket) these spaces form a [Gerstenhaber algebra](commutative-algebra.md#gerstenhaber-algebra).

##### Schouten-Nijenhuis bracket

↑ **Parent:** [Polynomial polyvector field](#polynomial-polyvector-field)

The left Schouten-Nijenhuis bracket on [polynomial polyvector fields](#polynomial-polyvector-field) is the degree-minus-one [Gerstenhaber bracket](associative-algebra.md#gerstenhaber-bracket) extending the [commutator](lie-algebra.md#commutator) of [derivations](associative-algebra.md#derivation-of-an-algebra) and $[D,f]=D(f)$ by graded antisymmetry and the left [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule). For $\Pi=\partial_X\wedge\partial_Y$, this convention gives $[h\Pi,f]=h(f_Y\partial_X-f_X\partial_Y)$ and $[F\partial_X+G\partial_Y,h\Pi]=(D(h)-h(F_X+G_Y))\Pi$. A right insertion convention reverses the degree-two-with-function formula.

#### Grassmann algebra

↑ **Parent:** [Exterior algebra](#exterior-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Grassmann_algebra)

A Grassmann algebra is an exterior algebra regarded as an algebra of anticommuting generators. Its odd elements satisfy $\theta_i\theta_j=-\theta_j\theta_i$.

##### Grassmann parity

↑ **Parent:** [Grassmann algebra](#grassmann-algebra)

The parity grading records whether a homogeneous element has even or odd Grassmann degree. Homogeneous elements obey $XY=(-1)^{|X||Y|}YX$. An odd differential uses the [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule); this is the sign bookkeeping behind [left-acting BRST differential](relativistic-quantum-field.md#left-acting-brst-differential) calculations.

##### Grassmann derivative

↑ **Parent:** [Grassmann algebra](#grassmann-algebra)

A [Grassmann derivative](#grassmann-derivative) is an odd differentiation operation on a [Grassmann algebra](#grassmann-algebra). A [left Grassmann derivative](#left-grassmann-derivative) obeys $\partial_\theta^L(ab)=(\partial_\theta^La)b+(-1)^{|a|}a(\partial_\theta^Lb)$ for homogeneous $a$. Right derivatives use the corresponding right-sided product rule. Their placement must be fixed when differentiating fermionic sources in a [generating functional](perturbative-quantum-field-theory.md#generating-functional), since commuting ordinary derivatives would lose [fermionic signs](perturbative-quantum-field-theory.md#fermionic-sign).

##### Left Grassmann derivative

↑ **Parent:** [Grassmann algebra](#grassmann-algebra)

Left differentiation with respect to an odd [Grassmann variable](#grassmann-variable) is the odd linear operation $\partial_\theta^L\theta=1$, with zero derivative on every other generator. For a homogeneous element $a$ of parity $|a|$, it obeys the graded product rule

$$
\partial_\theta^L(ab)=(\partial_\theta^La)b+(-1)^{|a|}a(\partial_\theta^Lb).
$$

For independent odd generators, $\partial_{\bar\theta}^L(\theta\bar\theta)=-\theta$. This sign comes from moving the derivative through the first odd factor in the [Grassmann algebra](#grassmann-algebra). It fixes chirality in the [chiral-superfield component expansion](supersymmetry.md#chiral-superfield-component-expansion); an ordinary commuting-variable product rule would give the wrong sign.

##### Grassmann variable

↑ **Parent:** [Grassmann algebra](#grassmann-algebra)

A Grassmann variable is an odd generator $\theta$ of a [Grassmann algebra](#grassmann-algebra). In characteristic zero it obeys $\theta^2=0$, so functions of finitely many Grassmann variables have finite Taylor expansions.

#### Exterior power

↑ **Parent:** [Exterior algebra](#exterior-algebra)

The $k$th exterior power $\Lambda^kV$ is the quotient of $V^{\otimes k}$ that makes every tensor with two equal factors zero. It represents alternating $k$-linear maps and has dimension $\binom{\dim V}{k}$ in finite dimensions.

##### Exterior square

↑ **Parent:** [Exterior power](#exterior-power)

The exterior square is the quotient of $V\otimes V$ by tensors $v\otimes v$, and records antisymmetric tensors of rank two.

###### Exterior square of a direct sum

↑ **Parent:** [Exterior square](#exterior-square)

The [exterior square](#exterior-square) of a [direct sum](vector-space.md#direct-sum) splits into wedges of two vectors from $V$, two from $W$, or one from each. The mixed map sends $v\otimes w$ to $(v,0)\wedge(0,w)$. A combined [basis](vector-space.md#basis) proves it is an isomorphism, and the [exterior-power Lie algebra representation](lie-algebra.md#exterior-power-lie-algebra-representation) proves equivariance for modules. No division by $2$ is used.

###### Symplectic contraction of an exterior square

↑ **Parent:** [Exterior square](#exterior-square)

For a [symplectic vector space](#symplectic-vector-space) $(V,\omega)$, contraction is the map $c:\Lambda^2V\to\mathbb C$ defined by $c(v\wedge w)=\omega(v,w)$. It is equivariant for the [symplectic Lie algebra](semisimple-lie-algebra.md#symplectic-lie-algebra). In dimension four its five-dimensional [kernel](#kernel-of-a-linear-map) is irreducible of [highest weight](semisimple-lie-algebra.md#highest-weight-of-a-representation) $\omega_2$, while the invariant inverse-form bivector spans a complementary [trivial Lie algebra representation](lie-algebra.md#trivial-lie-algebra-representation).

###### Primitive exterior square

↑ **Parent:** [Symplectic contraction of an exterior square](#symplectic-contraction-of-an-exterior-square)

The primitive exterior square of a [symplectic vector space](#symplectic-vector-space) is the [kernel](#kernel-of-a-linear-map) of its [symplectic contraction of an exterior square](#symplectic-contraction-of-an-exterior-square). In [dimension](vector-space.md#dimension-vector-space) four, the invariant inverse-form bivector $\Omega$ has nonzero wedge square. Choose $\operatorname{vol}=\Omega\wedge\Omega/2$; the [symmetric bilinear form](#symmetric-bilinear-form) $\xi\wedge\eta=B(\xi,\eta)\operatorname{vol}$ is [nondegenerate](#nondegenerate-bilinear-form) on $\Lambda^2V$. The primitive subspace is $\Omega^\perp$, and therefore inherits a nondegenerate form of dimension five. The [symplectic Lie algebra](semisimple-lie-algebra.md#symplectic-lie-algebra) acts on it by infinitesimal [orthogonal transformations](#orthogonal-transformation).

### Tensor

↑ **Parent:** [Multilinear algebra](#multilinear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tensor)

A rank-$n$ tensor on a vector space $V$ is a multilinear map of $n$ vector or covector arguments, equivalently an element of an $n$-fold tensor product. Its components transform by one copy of the change-of-basis matrix for each index.

#### Tensor index antisymmetrization

↑ **Parent:** [Tensor](#tensor)

Antisymmetrization over selected [tensor](#tensor) indices averages their permutations with the [sign of a permutation](finite-group-theory.md#sign-of-a-permutation). Square brackets denote it, for example $T_{[ab]}=(T_{ab}-T_{ba})/2$. It projects onto the alternating part. Antisymmetrized second derivatives of a scalar vanish for a [torsion-free connection](fiber-bundle.md#torsion-free-connection), but antisymmetrized later derivatives act on a tensor and can produce [curvature](differential-geometry.md#curvature).

#### Tensor index symmetrization

↑ **Parent:** [Tensor](#tensor)

Symmetrization over $r$ selected [tensor](#tensor) indices is the average over all $r!$ permutations, with every sign positive. Parentheses denote this operation, for example $T_{(ab)}=(T_{ab}+T_{ba})/2$. It is a [projection](vector-space.md#projection-linear-algebra) onto the symmetric part and commutes with a [covariant derivative](general-relativity.md#covariant-derivative) acting on indices outside the parentheses.

#### Axially invariant second-rank tensor

↑ **Parent:** [Tensor](#tensor)

A [Cartesian second-rank tensor](#cartesian-second-rank-tensor) invariant under every proper rotation preserving an unoriented axis $n$ has this form. Rotations about the axis give a planar block $aI+bJ$ and eliminate mixed axial-planar entries. A half-turn about a transverse axis reverses $J$, forcing $b=0$. If only rotations about the oriented axis are imposed, this planar antisymmetric term may survive.

##### Smallest axial rotation group forcing second-rank transverse isotropy

↑ **Parent:** [Axially invariant second-rank tensor](#axially-invariant-second-rank-tensor)

The six-element [dihedral group](finite-group-theory.md#dihedral-group) generated by the displayed rotations already forces every invariant second-rank [tensor](#tensor) to have the same form as an [axially invariant second-rank tensor](#axially-invariant-second-rank-tensor). The axial threefold rotation eliminates mixed entries and leaves only a planar scalar plus a planar antisymmetric part; the transverse half-turn eliminates the latter. No smaller finite [subgroup](group.md#subgroup) suffices: cyclic rotation [groups](group.md) retain an axial antisymmetric [tensor](#tensor), while a four-element noncyclic rotation [group](group.md) retains arbitrary diagonal [tensors](#tensor) along its three mutually perpendicular half-turn axes.

#### Cartesian second-rank tensor

↑ **Parent:** [Tensor](#tensor)

A Cartesian second-rank tensor has component matrix $T$ in each [orthonormal basis](#orthonormal-basis), with transformation $T\prime=RTR^T$ under an orthogonal component change $R$. Both indices transform; this is why assigning arbitrary matrices independently in different bases does not define a [tensor](#tensor). The [determinant](#determinant), [trace](#matrix-trace), and [Frobenius inner product](#frobenius-inner-product) with another such tensor are unchanged by these basis transformations.

##### Cubically invariant second-rank tensor

↑ **Parent:** [Cartesian second-rank tensor](#cartesian-second-rank-tensor)

A [Cartesian second-rank tensor](#cartesian-second-rank-tensor) in three dimensions invariant under quarter-turn [rotations](riemannian-geometry.md#rotation-mathematics) about all three coordinate axes is a scalar multiple of the [identity matrix](vector-space.md#identity-matrix). Squaring the quarter-turns gives coordinate half-turns; invariance under these forces every off-diagonal component to vanish. The quarter-turns then equate the three diagonal components. This conclusion does not require the original [tensor](#tensor) to be symmetric.

##### Scalar, symmetric-traceless and axial tensor decomposition

↑ **Parent:** [Cartesian second-rank tensor](#cartesian-second-rank-tensor)

Every three-dimensional [Cartesian second-rank tensor](#cartesian-second-rank-tensor) splits into scalar, symmetric-traceless, and antisymmetric parts. Their coefficients are $P=P_{kk}/3$, $S_{ij}=(P_{ij}+P_{ji})/2-P\delta_{ij}$, and $A_k=\epsilon_{kij}P_{ij}/2$. The epsilon contraction identity reconstructs the antisymmetric part and proves uniqueness. Under proper rotations $A$ behaves as a vector, but under reflections it is an [axial vector](vector-space.md#pseudovector).

##### Divergence of a Cartesian second-rank tensor

↑ **Parent:** [Cartesian second-rank tensor](#cartesian-second-rank-tensor)

For a constant orthogonal Cartesian coordinate change $x'=Rx$, a [Cartesian second-rank tensor](#cartesian-second-rank-tensor) obeys $T'_{ij}=R_{ik}R_{jl}T_{kl}$. The [chain rule](calculus.md#chain-rule) gives $\partial'_j=R_{jm}\partial_m$. Consequently $\partial'_jT'_{ij}=R_{ik}R_{jl}R_{jm}\partial_mT_{kl}=R_{ik}\partial_lT_{kl}$, the transformation rule for a [vector](vector-space.md#vector). Under non-Cartesian position-dependent coordinate changes, partial derivatives must be replaced by the appropriate [covariant derivative](general-relativity.md#covariant-derivative).

##### Oriented-axis invariant Cartesian tensor

↑ **Parent:** [Cartesian second-rank tensor](#cartesian-second-rank-tensor)

A [Cartesian second-rank tensor](#cartesian-second-rank-tensor) invariant under all rotations about an oriented unit axis $n$ has the displayed form. A half-turn about the axis eliminates the mixed axial-transverse entries, and a quarter-turn makes the transverse block a scalar matrix plus an antisymmetric planar rotation generator. Conversely both transverse terms commute with every rotation about the axis. The antisymmetric term is allowed unless symmetry or an additional axis-reversing rotation is imposed. This differs from an [axially invariant second-rank tensor](#axially-invariant-second-rank-tensor) for an unoriented axis.

##### Coordinate half-turn invariance of a second-rank tensor

↑ **Parent:** [Cartesian second-rank tensor](#cartesian-second-rank-tensor)

A [Cartesian second-rank tensor](#cartesian-second-rank-tensor) invariant under half-turns about all three coordinate axes is diagonal. Each half-turn has diagonal signs, and each off-diagonal entry changes sign under at least one of them. Invariance therefore kills all off-diagonal entries. It does not make the diagonal entries equal: that requires additional rotational invariance, as for an [isotropic second-rank tensor](#isotropic-second-rank-tensor).

#### Composition of mixed tensors

↑ **Parent:** [Tensor](#tensor)

A type-$(1,1)$ [tensor](#tensor) identifies with an [endomorphism](algebra.md#endomorphism) of a finite-dimensional [vector space](vector-space.md). Composing two such maps produces another type-$(1,1)$ [tensor](#tensor), because $(X,\eta)\mapsto\eta(B(A(X)))$ is a [multilinear map](#multilinear-map). In output-first components the result is $C^a{}_b=B^a{}_cA^c{}_b$; the contracted index implements composition, and a basis change conjugates the corresponding matrices.

#### Pseudotensor

↑ **Parent:** [Tensor](#tensor)

Under an orthogonal coordinate transformation $R$, a Cartesian pseudotensor has the usual [tensor](#tensor) transformation law multiplied by $\det R$. Thus proper [rotation matrices](#rotation-matrix) act as on ordinary tensors, while an orientation-reversing change contributes an extra minus sign. Interpreted as a rank-three pseudotensor, the [Levi-Civita symbol](calculus.md#levi-civita-symbol) has the same numerical components in every orthonormal frame, because its ordinary three-index transformation already contributes a factor $\det R$.

#### Symmetric tensor

↑ **Parent:** [Tensor](#tensor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_tensor)

A symmetric [tensor](#tensor) is unchanged by every [permutation](combinatorics.md#permutation) of its slots. A [symmetric second-rank tensor](#symmetric-second-rank-tensor) is the rank-two case; symmetry for higher rank requires invariance under every such slot exchange.

##### Axisymmetric symmetric rank-two tensor

↑ **Parent:** [Symmetric tensor](#symmetric-tensor)

A [symmetric tensor](#symmetric-tensor) invariant under rotations about a fixed nonzero vector $y$ has the form $\alpha I+\beta yy^T$. Choose the third coordinate axis parallel to $y$: rotation by a half-turn makes the mixed axial-transverse entries vanish, and all transverse rotations make the transverse block a scalar multiple of the identity. Its two transverse eigenvalues are $\alpha$ and its axial eigenvalue is $\alpha+\beta|y|^2$. The [trace](#matrix-trace) and the quadratic contraction $y^TTy$ determine these two coefficients. Full isotropy holds exactly when $\beta=0$.

###### Weighted chord tensor of a sphere

↑ **Parent:** [Axisymmetric symmetric rank-two tensor](#axisymmetric-symmetric-rank-two-tensor)

For $|y|=a$ and $n>-1$, this surface integral is finite: near $x=y$ its integrand has size $O(|x-y|^{2n})$ and the two-dimensional area element supplies one further power of distance. Rotational covariance and symmetry make it an [axisymmetric symmetric rank-two tensor](#axisymmetric-symmetric-rank-two-tensor). Put $K=\pi(2a)^{2n+2}$. Polar integration about the $y$ axis gives $\operatorname{tr}T=K/(n+1)$ and $y^TTy=a^2K/(n+2)$. Solving $3\alpha+\beta a^2=\operatorname{tr}T$ and $\alpha+\beta a^2=y^TTy/a^2$ gives $\alpha=K/[2(n+1)(n+2)]$ and $\beta=\alpha(2n+1)/a^2$. Thus the weighted chord tensor becomes an [isotropic tensor](#isotropic-tensor) exactly at $n=-1/2$.

##### Polarization spanning of symmetric tensors

↑ **Parent:** [Symmetric tensor](#symmetric-tensor)

Over a field of [characteristic zero](algebra.md#characteristic-zero), degree-$n$ [symmetric tensors](#symmetric-tensor) are spanned by pure powers $a^{\otimes n}$. Inclusion-exclusion expands $\sum_{J\subseteq[n]}(-1)^{n-|J|}(\sum_{j\in J}a_j)^{\otimes n}$ into the sum of all [permutation](combinatorics.md#permutation) orderings of $a_1\otimes\cdots\otimes a_n$. Every surviving term uses each of the $n$ labels once. This converts an invariant-tensor spanning problem into pure [tensor powers](#tensor-power).

##### Symmetric second-rank tensor

↑ **Parent:** [Symmetric tensor](#symmetric-tensor)

A second-rank tensor is symmetric when $T_{ij}=T_{ji}$. Every second-rank tensor has the unique decomposition

$$
T_{ij}=\frac{T_{ij}+T_{ji}}2+\frac{T_{ij}-T_{ji}}2
$$

into symmetric and antisymmetric parts.

#### Quotient theorem for Cartesian tensors

↑ **Parent:** [Tensor](#tensor)

Suppose an array $T_{ij}$ is specified in each right-handed [orthonormal basis](#orthonormal-basis). If $w_i=T_{ij}v_j$ transforms as a [vector](vector-space.md#vector) for every [vector](vector-space.md#vector) $v$, then $T$ is a second-order Cartesian [tensor](#tensor) under those [basis](vector-space.md#basis) changes. Indeed $v'=Rv$, $w'=Rw$ imply $T'Rv=RTv$ for every $v$, hence $T'=RTR^T$. The condition on every test [vector](vector-space.md#vector) is essential; one contraction is insufficient.

##### Symmetric-test criterion for a third-rank Cartesian tensor

↑ **Parent:** [Quotient theorem for Cartesian tensors](#quotient-theorem-for-cartesian-tensors)

If contraction of an array with every [symmetric second-rank tensor](#symmetric-second-rank-tensor) is a [vector](vector-space.md#vector) in every orthonormal frame, its part symmetric in the contracted slots obeys the rank-three [tensor](#tensor) transformation law. The difference between its proposed transformation and actual components is symmetric and contracts to zero against every symmetric [matrix](vector-space.md#matrix), so it vanishes. The antisymmetric part is invisible, by the [blindness of symmetric contraction tests to antisymmetric arrays](#blindness-of-symmetric-contraction-tests-to-antisymmetric-arrays), and need not be tensorial.

##### Scalar contraction test for a Cartesian tensor

↑ **Parent:** [Quotient theorem for Cartesian tensors](#quotient-theorem-for-cartesian-tensors)

If an array specified in each [orthonormal basis](#orthonormal-basis) has invariant [Frobenius inner product](#frobenius-inner-product) with every [Cartesian second-rank tensor](#cartesian-second-rank-tensor), it transforms as such a tensor. For a component change $R$, invariance says $(R^TA\prime R-A):B=0$ for every matrix $B$. Nondegeneracy of the [Frobenius inner product](#frobenius-inner-product) forces the difference to vanish. Testing every tensor, rather than a single selected tensor, is essential.

###### Antisymmetric contraction test for an antisymmetric tensor

↑ **Parent:** [Scalar contraction test for a Cartesian tensor](#scalar-contraction-test-for-a-cartesian-tensor)

If an array is antisymmetric in every [orthonormal basis](#orthonormal-basis) and its contractions with every [antisymmetric second-rank tensor](#antisymmetric-second-rank-tensor) are invariant scalars, it obeys the [Cartesian second-rank tensor](#cartesian-second-rank-tensor) transformation law. The difference $D=R^TA\prime R-A$ is antisymmetric and orthogonal to every antisymmetric test matrix. Choosing the test matrix equal to $D$ gives $D:D=0$, hence $D=0$. The [Frobenius inner product](#frobenius-inner-product) is nondegenerate on the antisymmetric subspace.

###### Blindness of symmetric contraction tests to antisymmetric arrays

↑ **Parent:** [Scalar contraction test for a Cartesian tensor](#scalar-contraction-test-for-a-cartesian-tensor)

The [Frobenius inner product](#frobenius-inner-product) of a symmetric matrix and an antisymmetric matrix is zero. Thus invariant contractions of an array with all [symmetric second-rank tensors](#symmetric-second-rank-tensor) test only its symmetric part; an arbitrary basis-dependent antisymmetric part is invisible. A nonzero antisymmetric matrix in one basis and the zero matrix in another passes all such tests with scalar zero but is not a [Cartesian second-rank tensor](#cartesian-second-rank-tensor).

#### Traceless second-rank tensor

↑ **Parent:** [Tensor](#tensor)

A second-rank Cartesian [tensor](#tensor) is traceless when the contraction $T_{ii}$ vanishes. For a [symmetric second-rank tensor](#symmetric-second-rank-tensor), this is equivalent to its [eigenvalues](linear-operator-theory.md#eigenvalue) summing to zero. The orientational [nematic order parameter](critical-phenomenon.md#nematic-order-parameter) is both symmetric and traceless, excluding an isotropic scalar contribution.

#### Slice rank

↑ **Parent:** [Tensor](#tensor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Slice_rank)

For finite sets $X,Y,Z$ and a field $F$, a three-variable tensor $T:X\times Y\times Z\to F$ has slice rank at most $r$ when it is a sum of $r$ terms, each of which separates one variable from the other two. Such terms have one of the forms

$$
a(x)b(y,z),\qquad c(y)d(x,z),\qquad e(z)h(x,y).
$$

The slice rank is the least possible $r$.

##### Diagonal tensor

↑ **Parent:** [Slice rank](#slice-rank)

A three-variable tensor is diagonal when it vanishes unless its three arguments are equal.

###### Slice rank of a diagonal tensor

↑ **Parent:** [Diagonal tensor](#diagonal-tensor)

If

$$
T(x,y,z)=\begin{cases}c_x&x=y=z,\\0&\text{otherwise},\end{cases}
$$

on a finite set $X$, and every $c_x$ is nonzero, then the [slice rank](#slice-rank) of $T$ is $|X|$. The upper bound uses one $x$-slice for each diagonal entry. For the lower bound, restrict any shorter slice decomposition to a common kernel of the coefficient functions in two slice directions; the remaining diagonal matrix has rank larger than the number of slices available in the third direction, a contradiction.

#### Covariance and contravariance of vectors

↑ **Parent:** [Tensor](#tensor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Covariance_and_contravariance_of_vectors)

Covariance and contravariance describe how vector and covector components transform when a basis changes.

##### Covariant tensor

↑ **Parent:** [Covariance and contravariance of vectors](#covariance-and-contravariance-of-vectors)

A covariant tensor is multilinear in vector arguments and transforms with one covariant index for each argument.

#### Kronecker delta

↑ **Parent:** [Tensor](#tensor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kronecker_delta)

The Kronecker delta is $\delta_{ij}=1$ when $i=j$ and zero otherwise. It is the component matrix of the identity map in a basis.

#### Antisymmetric second-rank tensor

↑ **Parent:** [Tensor](#tensor)

A second-rank Cartesian tensor is antisymmetric when its components form a [skew-symmetric matrix](#skew-symmetric-matrix), $T_{ij}=-T_{ji}$. Orthogonal coordinate changes preserve this property because $T'=RTR^T$ implies $(T')^T=RT^TR^T=-T'$.

#### Antisymmetric tensor

↑ **Parent:** [Tensor](#tensor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antisymmetric_tensor)

An [antisymmetric tensor](#antisymmetric-tensor) changes sign under exchange of two indices in a specified subset of its indices. A [totally antisymmetric tensor](#totally-antisymmetric-tensor) has this property for every pair of indices.

##### Totally antisymmetric tensor

↑ **Parent:** [Antisymmetric tensor](#antisymmetric-tensor)

A tensor changes sign whenever two indices are interchanged. In three dimensions, a rank-two antisymmetric tensor is $A_{ij}=a_k\epsilon_{kij}$, a rank-three one is $A_{ijk}=a\epsilon_{ijk}$, and every totally antisymmetric tensor of rank greater than three vanishes.

#### Isotropic tensor

↑ **Parent:** [Tensor](#tensor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isotropic_tensor)

An isotropic tensor is invariant under every proper orthogonal change of basis. A rank-four isotropic tensor has the form

$$
T_{ijkl}=a\delta_{ij}\delta_{kl}
+b\delta_{ik}\delta_{jl}
+c\delta_{il}\delta_{jk}.
$$

Rank-five isotropic pseudotensors are formed by multiplying one Kronecker delta by one Levi-Civita symbol and permuting the five indices.

##### Isotropic elasticity on tensor components

↑ **Parent:** [Isotropic tensor](#isotropic-tensor)

The rank-four law $c_{ijkl}=\alpha\delta_{ij}\delta_{kl}+\beta\delta_{ik}\delta_{jl}+\gamma\delta_{il}\delta_{jk}$ sends a strain array to $P_{ij}=\alpha\delta_{ij}T_{kk}+\beta T_{ij}+\gamma T_{ji}$. Applying the [scalar, symmetric-traceless and axial tensor decomposition](#scalar-symmetric-traceless-and-axial-tensor-decomposition) gives the displayed independent actions on the three components. The inverse requires all relevant coefficients nonzero. Restricting to a [symmetric second-rank tensor](#symmetric-second-rank-tensor) eliminates the axial part and gives $P_{ij}=\alpha\delta_{ij}T_{kk}+(\beta+\gamma)T_{ij}$. Without that symmetry restriction the two-parameter form is not generally valid.

##### Isotropic contractions of a fourth-rank tensor

↑ **Parent:** [Isotropic tensor](#isotropic-tensor)

Contract an [isotropic tensor](#isotropic-tensor) with the [Kronecker delta](#kronecker-delta) or the [Levi-Civita symbol](calculus.md#levi-civita-symbol), using invariance under proper rotations. The three displayed contractions have ranks one, two and three. The only isotropic vector is zero; an [isotropic second-rank tensor](#isotropic-second-rank-tensor) is a scalar delta, and an [isotropic third-rank tensor](#isotropic-third-rank-tensor) is a scalar epsilon. For $T_{ijkl}=\alpha\delta_{ij}\delta_{kl}+\beta\delta_{ik}\delta_{jl}+\gamma\delta_{il}\delta_{jk}$, direct contraction gives $\mu=3\alpha+\beta+\gamma$ and $\nu=\beta-\gamma$.

##### Isotropic third-rank tensor

↑ **Parent:** [Isotropic tensor](#isotropic-tensor)

A rank-three Cartesian [tensor](#tensor) invariant under every proper [rotation matrix](#rotation-matrix) in three dimensions is a multiple of the [Levi-Civita symbol](calculus.md#levi-civita-symbol). Half-turns about coordinate axes force every nonzero component to contain each coordinate label once, and quarter-turns make these components alternating. Conversely, the [determinant](#determinant) formula $R_{ia}R_{jb}R_{kc}\epsilon_{abc}=(\det R)\epsilon_{ijk}$ proves invariance when $\det R=1$. Requiring invariance under reflections as an ordinary tensor forces $b=0$; invariance under proper rotations alone permits nonzero $b$.

##### Isotropic second-rank tensor

↑ **Parent:** [Isotropic tensor](#isotropic-tensor)

A second-rank Cartesian [tensor](#tensor) invariant under every proper [rotation matrix](#rotation-matrix) is a scalar multiple of the [Kronecker delta](#kronecker-delta). Half-turns about the coordinate axes kill its off-diagonal entries, and quarter-turns make its diagonal entries equal. A tensor of the form $v_iw_j$ is an [outer product](vector-space.md#outer-product) with matrix rank at most one, so it is isotropic in three dimensions only when it vanishes, equivalently when $v=0$ or $w=0$.

#### Einstein notation

↑ **Parent:** [Tensor](#tensor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Einstein_notation)

Einstein notation sums automatically over an index repeated once up and once down, or twice in Euclidean coordinates.

### Tensor contraction

↑ **Parent:** [Multilinear algebra](#multilinear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tensor_contraction)

#### Metric trace

↑ **Parent:** [Tensor contraction](#tensor-contraction)

The metric trace contracts two indices of a covariant rank-two tensor: $T=g^{\mu\nu}T_{\mu\nu}$. For the metric itself in $D$ dimensions, $g^{\mu\nu}g_{\mu\nu}=D$.

### Reciprocal basis

↑ **Parent:** [Multilinear algebra](#multilinear-algebra)

For a basis $e_1,e_2,e_3$ with [scalar triple product](#scalar-triple-product) $\Delta$, the reciprocal vectors are cyclic cross products divided by $\Delta$ and satisfy $f_i\cdot e_j=\delta_{ij}$. This construction is used for the basis of a [reciprocal lattice](quantum-mechanics.md#reciprocal-lattice).

#### Reciprocal basis involution

↑ **Parent:** [Reciprocal basis](#reciprocal-basis)

For a three-dimensional [basis](vector-space.md#basis) with nonzero [scalar triple product](#scalar-triple-product) $\Delta$, its [reciprocal basis](#reciprocal-basis) satisfies $\widehat e_2\times\widehat e_3=e_1/\Delta$ and the cyclic analogues. Consequently its [scalar triple product](#scalar-triple-product) is $1/\Delta$, and taking the [reciprocal basis](#reciprocal-basis) again recovers the original [basis](vector-space.md#basis). The coordinates of $V$ in the original [basis](vector-space.md#basis) are $V\cdot\widehat e_i$; in the [reciprocal basis](#reciprocal-basis) they are $V\cdot e_i$.

#### Orientation of an orthonormal reciprocal basis

↑ **Parent:** [Reciprocal basis](#reciprocal-basis)

For a real basis matrix $E$ with basis vectors as rows, the [reciprocal basis](#reciprocal-basis) has row matrix $E^{-T}$. If either basis is [orthonormal](#orthonormal-set), both are, and $E^{-T}=E$. Thus $E$ is an [orthogonal matrix](#orthogonal-matrix), with determinant either $1$ or $-1$. It is a [rotation matrix](#rotation-matrix) precisely when the original ordered basis is positively oriented relative to the reference coordinates. For example, $\operatorname{diag}(1,1,-1)$ is its own orthonormal reciprocal basis matrix but is an [improper orthogonal transformation](#improper-orthogonal-transformation).

### Scalar triple product

↑ **Parent:** [Multilinear algebra](#multilinear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scalar_triple_product)

The scalar triple product $a\cdot(b\times c)$ is the signed volume of the parallelepiped spanned by three vectors.

#### Cross products with a common vector

↑ **Parent:** [Scalar triple product](#scalar-triple-product)

The [cross product](vector-space.md#cross-product) of two [cross products](vector-space.md#cross-product) sharing their first vector is parallel to that vector, with scalar factor equal to the [scalar triple product](#scalar-triple-product). In [suffix notation](#einstein-notation), use $\epsilon_{ijk}\epsilon_{kpq}=\delta_{ip}\delta_{jq}-\delta_{iq}\delta_{jp}$. The component of the double [cross product](vector-space.md#cross-product) becomes $A_i\epsilon_{q\ell m}C_qA_\ell B_m-C_i\epsilon_{p\ell m}A_pA_\ell B_m$. The second term vanishes by antisymmetry of the [Levi-Civita symbol](calculus.md#levi-civita-symbol); the first equals $A_i(A\cdot(B\times C))$, proving the identity even when the vectors are dependent.

#### Squared scalar triple product from cyclic cross products

↑ **Parent:** [Scalar triple product](#scalar-triple-product)

Apply the [vector triple product identity](calculus.md#vector-triple-product) with first vector $b\times c$. Its contraction with $c$ vanishes, so $(b\times c)\times(c\times a)=[a\cdot(b\times c)]c$. Dotting with $a\times b$ gives the square of the [scalar triple product](#scalar-triple-product). This is also the [Gram determinant](#gram-determinant) of $a,b,c$, hence is nonnegative even when the vectors are linearly dependent.

### Orientation of a vector space

↑ **Parent:** [Multilinear algebra](#multilinear-algebra)

An orientation of a finite-dimensional real vector space distinguishes its ordered bases into two classes according to the sign of their change-of-basis determinant.

#### Oriented volume

↑ **Parent:** [Orientation of a vector space](#orientation-of-a-vector-space)

An oriented volume retains the sign of a determinant; reversing the orientation changes that sign.

### Determinant

↑ **Parent:** [Multilinear algebra](#multilinear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Determinant)

The determinant is the alternating multilinear volume scale of a square matrix; it is nonzero exactly for invertible matrices.

#### Nonintersecting lattice-path determinant

↑ **Parent:** [Determinant](#determinant)

For a weighted acyclic directed graph, let $M_{ij}$ be the sum of path weights from $A_j$ to $B_i$. Expanding $\det M$ gives a signed sum of path families. At the first intersection in a fixed topological order, swap the two path tails. The operation preserves weight and reverses the endpoint [permutation](combinatorics.md#permutation)'s sign, so intersecting families cancel. Only vertex-disjoint families remain. If planarity forces these families to join identically indexed endpoints, their sum has positive sign. Applied to northeast paths with horizontal weight $x_r$ at height $r$, this gives the skew [Jacobi–Trudi identity](combinatorics.md#jacobi-trudi-identity).

#### Determinant of the minimum-index matrix

↑ **Parent:** [Determinant](#determinant)

Let $L$ be the [triangular matrix](#triangular-matrix) with $L_{ij}=1$ for $j\leq i$ and zero otherwise. Then $(LL^T)_{ij}=\min(i,j)$ and $\det L=1$, so the [determinant](#determinant) of $LL^T$ is one. More generally, for $0=t_0<t_1<\cdots<t_n$, the [matrix](vector-space.md#matrix) with entries $\min(t_i,t_j)$ factors as $L\operatorname{diag}(t_k-t_{k-1})L^T$ and has [determinant](#determinant) $\prod_k(t_k-t_{k-1})$. This is the finite-dimensional structure behind the [Brownian covariance kernel](random-variable.md#brownian-covariance-kernel).

<h4 id="cauchy-binet-formula">Cauchy–Binet formula</h4>

↑ **Parent:** [Determinant](#determinant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy–Binet_formula)

For [matrices](vector-space.md#matrix) $A\in\mathbb R^{r\times m}$ and $B\in\mathbb R^{m\times r}$ with $r\leq m$,

$$
\det(AB)=\sum_{\substack{S\subseteq\{1,\ldots,m\}\\|S|=r}}\det A_{:,S}\det B_{S,:},
$$

where the indices of $S$ are taken in increasing order. To prove it, write the $j$th column of $AB$ as $\sum_q B_{qj}A_{:,q}$ and expand its [determinant](#determinant) by multilinearity. Terms with a repeated $q$ vanish by alternation. For each remaining index set $S=\{s_1<\cdots<s_r\}$, collect all permutations $q_j=s_{\sigma(j)}$. The factor from $A$ is $\operatorname{sgn}(\sigma)\det A_{:,S}$; the sum of the products $\operatorname{sgn}(\sigma)\prod_j B_{s_{\sigma(j)},j}$ is $\det B_{S,:}$. This proves the formula. Applying it to selected rows and columns proves that a product of compatible [totally nonnegative matrices](vector-space.md#total-nonnegativity-of-a-matrix) is totally nonnegative.

<h4 id="cramer-s-rule">Cramer's rule</h4>

↑ **Parent:** [Determinant](#determinant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cramer's_rule)

For an invertible square [matrix](vector-space.md#matrix) $A$ and $Ax=b$, replace column $i$ by $b$ to form $A_i$. Multilinearity of the [determinant](#determinant) and $b=\sum_jx_j A_{\cdot j}$ give $\det A_i=x_i\det A$: all other summands have repeated columns and vanish. Division gives the formula. With integer coefficients this supplies explicit rational solutions and, together with the [Hadamard determinant inequality](#hadamard-determinant-inequality), bounds their numerators and denominators.

#### Hadamard determinant inequality

↑ **Parent:** [Determinant](#determinant)

For a square [matrix](vector-space.md#matrix) with row vectors $r_i$, the absolute [determinant](#determinant) is at most the product of the [Euclidean norms](functional-analysis.md#euclidean-norm) of its rows. If the rows are dependent the [determinant](#determinant) is zero. Otherwise [Gram-Schmidt process](#gram-schmidt-process) leaves the [determinant](#determinant) unchanged and replaces each row by its component orthogonal to its predecessors. The resulting orthogonal rows have lengths no greater than the original rows, and their volume is their product. This proves the inequality; equality holds for mutually orthogonal rows.

#### Pfaffian

↑ **Parent:** [Determinant](#determinant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pfaffian)

For an antisymmetric $2n\times2n$ matrix, the Pfaffian is $\operatorname{Pf}(A)=(2^nn!)^{-1}\sum_{\sigma\in S_{2n}}\operatorname{sgn}(\sigma)\prod_{j=1}^n A_{\sigma(2j-1),\sigma(2j)}$. Equivalently, it is the coefficient of the top exterior power of the associated alternating form, with the usual factorial normalization. Its square is the [determinant](#determinant). In size four it is $a_{12}a_{34}-a_{13}a_{24}+a_{14}a_{23}$, so its vanishing characterizes the simple nonzero [bivectors](#bivector) of the [Klein quadric](differential-geometry.md#klein-quadric).

#### Determinant of a complex block representation

↑ **Parent:** [Determinant](#determinant)

The block matrix $M=\begin{pmatrix}A&-B\\B&A\end{pmatrix}$ is similar over $\mathbb C$ to $\operatorname{diag}(A+iB,A-iB)$ via $T=\begin{pmatrix}I&I\\-iI&iI\end{pmatrix}$. Therefore its [determinant](#determinant) is $\det(A+iB)\det(A-iB)$ for arbitrary square matrices $A,B$. The argument uses a constant [change-of-basis matrix](#change-of-basis-matrix) and [multiplicativity of the determinant](#multiplicativity-of-the-determinant).

#### Jacobi determinant derivative formula

↑ **Parent:** [Determinant](#determinant)

For a differentiable invertible [matrix](vector-space.md#matrix) $A(t)$, $\frac d{dt}\log\det A=\operatorname{tr}(A^{-1}\dot A)$ wherever a consistent logarithm is defined. In particular a positive spatial [metric tensor](general-relativity.md#metric-tensor) satisfies $h^{ij}\dot h_{ij}=\dot h/h$. This separates its local volume change from shape change.

#### Derivative of the determinant

↑ **Parent:** [Determinant](#determinant)

For an invertible [matrix](vector-space.md#matrix) $A$ and any [matrix](vector-space.md#matrix) $H$,

$$
D(\det)_A(H)=\det(A)\operatorname{tr}(A^{-1}H).
$$

Indeed $\det(A+tH)=\det(A)\det(I+tA^{-1}H)$, and multilinearity shows that the linear coefficient of $\det(I+tB)$ is $\operatorname{tr}B$. At a singular [matrix](vector-space.md#matrix) the [derivative](calculus.md#derivative) is instead written $\operatorname{tr}(\operatorname{adj}(A)H)$; this [polynomial](polynomial.md) formula holds for all $A$.

<h5 id="jacobi-s-formula">Jacobi's formula</h5>

↑ **Parent:** [Derivative of the determinant](#derivative-of-the-determinant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobi's_formula)

For an arbitrary square [matrix](vector-space.md#matrix) $A$, the [derivative of the determinant](#derivative-of-the-determinant) in direction $H$ is the displayed expression. Differentiating the [determinant](#determinant)'s [multilinear](#multilinear-map) expansion gives the sum of entries of $H$ weighted by their cofactors, equal to the displayed [trace](#matrix-trace). If $A$ is invertible, $\operatorname{adj}(A)=(\det A)A^{-1}$ gives $(\det A)\operatorname{tr}(A^{-1}H)$, and division by $\det A$ gives the [Jacobi determinant derivative formula](#jacobi-determinant-derivative-formula) for the logarithmic [derivative](calculus.md#derivative). The adjugate expression remains valid at singular [matrices](vector-space.md#matrix).

##### Second derivative of the determinant

↑ **Parent:** [Derivative of the determinant](#derivative-of-the-determinant)

The [derivative of the determinant](#derivative-of-the-determinant) at an invertible [matrix](vector-space.md#matrix) is $D\det_A(K)=\det A\operatorname{tr}(A^{-1}K)$. At $A=I+H$, use $\det(I+H)=1+\operatorname{tr}H+O(\|H\|^2)$ and $(I+H)^{-1}=I-H+O(\|H\|^2)$. Differentiating the first derivative gives the displayed symmetric [bilinear map](#bilinear-map). More generally $D^2\det_A(H,K)=\det A[\operatorname{tr}(A^{-1}H)\operatorname{tr}(A^{-1}K)-\operatorname{tr}(A^{-1}HA^{-1}K)]$.

#### Log-determinant

↑ **Parent:** [Determinant](#determinant)

On [positive-definite matrices](#positive-definite-matrix), the log-determinant has differential $d\log\det A=\operatorname{Tr}(A^{-1}dA)$ and is a [strictly concave function](real-analysis.md#strictly-concave-function).

#### Multilinearity of the determinant

↑ **Parent:** [Determinant](#determinant)

The determinant is linear in each row and in each column when all the others are held fixed.

#### Multiplicativity of the determinant

↑ **Parent:** [Determinant](#determinant)

The determinant is multiplicative: for square matrices of the same size, $\det(AB)=\det(A)\det(B)$.

#### Leibniz formula for determinants

↑ **Parent:** [Determinant](#determinant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Leibniz_formula_for_determinants)

For an $n$ by $n$ matrix,

$$
\det A=\sum_{\sigma\in S_n}\operatorname{sgn}(\sigma)
\prod_{i=1}^na_{i,\sigma(i)}.
$$

#### Tridiagonal determinant recurrence

↑ **Parent:** [Determinant](#determinant)

For diagonal entries $a_i$, superdiagonal entries $b_i$, and subdiagonal entries $c_i$, the leading principal determinants satisfy

$$
d_n=a_nd_{n-1}-b_{n-1}c_{n-1}d_{n-2},
\qquad d_0=1,\quad d_1=a_1.
$$

## System of linear equations

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/System_of_linear_equations)

A linear system $Ax=b$ is consistent when $b$ lies in the column space of $A$; its solutions form a translate of $\ker A$.

### Image criterion for a matrix factorization

↑ **Parent:** [System of linear equations](#system-of-linear-equations)

For [matrices](vector-space.md#matrix) representing [linear maps](vector-space.md#linear-map) on finite-dimensional [vector spaces](vector-space.md), $AX=B$ has a solution precisely when the [image of a linear map](vector-space.md#image-of-a-linear-map) represented by $B$ is contained in that represented by $A$. Necessity follows by applying the equation to vectors. For sufficiency choose an $A$-preimage of each column of $B$ and assemble those vectors as the columns of $X$. All solutions are $X_0+N$ with $AN=0$, equivalently every column of $N$ lies in the [kernel of a linear map](#kernel-of-a-linear-map) represented by $A$. When $B$ has at least one column, a solution is unique precisely when $A$ has trivial [kernel](#kernel-of-a-linear-map).

### Augmented matrix

↑ **Parent:** [System of linear equations](#system-of-linear-equations)

The augmented [matrix](vector-space.md#matrix) of a [linear system](#system-of-linear-equations) $Ax=b$ appends the right-hand side as one extra column. Elementary row operations preserve its solution set. The [linear system](#system-of-linear-equations) is consistent exactly when the coefficient [matrix rank](vector-space.md#matrix-rank) equals the augmented [matrix rank](vector-space.md#matrix-rank), because this is equivalent to $b$ lying in the span of the columns of $A$. A larger augmented [matrix rank](vector-space.md#matrix-rank) produces a zero coefficient row with a nonzero right-hand side during [Gaussian elimination](numerical-analysis.md#gaussian-elimination).

### Homogeneous linear system

↑ **Parent:** [System of linear equations](#system-of-linear-equations)

A [linear system](#system-of-linear-equations) is homogeneous when its forcing is zero. Its solution set is the [kernel of a linear map](#kernel-of-a-linear-map), a [vector subspace](vector-space.md#vector-subspace). If $Ax=b$ has a particular solution $x_0$, all its solutions are $x_0+\ker A$: subtracting the particular solution leaves a [homogeneous linear system](#homogeneous-linear-system). The [rank-nullity theorem](#rank-nullity-theorem) gives the dimension of this freedom.

### Linear equation

↑ **Parent:** [System of linear equations](#system-of-linear-equations)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_equation)

A linear equation is an equation in which the unknowns occur only to the first power and are combined linearly.

#### Affine solution space of a linear equation

↑ **Parent:** [Linear equation](#linear-equation)

For a [linear map](vector-space.md#linear-map) $L:V\to W$ and one solution $Lu_0=f$, all solutions are $u_0+\ker L$. This follows because $L(u-u_0)=0$, and conversely adding any kernel element preserves the equation. If $U\subseteq V$ is a [vector subspace](vector-space.md#vector-subspace) representing a desired regularity class and $u_0\in U$, then every solution to this one inhomogeneous equation lies in $U$ exactly when $\ker L\subseteq U$. For distributional differential equations, take $U$ to be the distributions represented by [smooth functions](analysis.md#smooth-function).

### Fredholm alternative for a matrix

↑ **Parent:** [System of linear equations](#system-of-linear-equations)

The system $Ax=b$ is solvable exactly when $b$ is orthogonal to every vector in $\ker A^T$.

## Symmetric and antisymmetric parts of a matrix

↑ **Parent:** [Linear algebra](linear-algebra.md)

Every square matrix decomposes uniquely as $A=(A+A^T)/2+(A-A^T)/2$, a symmetric part plus an antisymmetric part.

### Symmetric part of a matrix

↑ **Parent:** [Symmetric and antisymmetric parts of a matrix](#symmetric-and-antisymmetric-parts-of-a-matrix)

The symmetric part of a real square [matrix](vector-space.md#matrix) is $H=(A+A^T)/2$. It controls the quadratic form because $x^TAx=x^THx$; the antisymmetric part contributes zero. In a [linear differential equation](differential-equation.md#linear-differential-equation) $x'=Ax$, it determines the instantaneous derivative of the squared [Euclidean norm](functional-analysis.md#euclidean-norm).

## Symmetric matrix

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_matrix)

A real matrix is symmetric when $A^T=A$. It represents a [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) in the standard Euclidean [inner product](#inner-product).

### Complex symmetric nilpotent matrix

↑ **Parent:** [Symmetric matrix](#symmetric-matrix)

The displayed nonzero [matrix](vector-space.md#matrix) is symmetric under transpose but not [Hermitian](hilbert-space.md#hermitian-operator). It is [nilpotent](commutative-algebra.md#nilpotent), so all its [eigenvalues](linear-operator-theory.md#eigenvalue) are zero and it cannot be [diagonalizable](linear-operator-theory.md#diagonalizable-matrix). Thus real-symmetric spectral conclusions require reality or a Hermitian hypothesis; complex transpose symmetry alone is insufficient.

### Axis decomposition of a symmetric matrix

↑ **Parent:** [Symmetric matrix](#symmetric-matrix)

Fix $v\ne0$, put $s=v^Tv$, $t=v^TTv$, and $P=I-vv^T/s$. Any real [symmetric matrix](#symmetric-matrix) on three-dimensional [Euclidean space](functional-analysis.md#euclidean-norm) has a unique decomposition with $C^Tv=0$, $Dv=0$ and $\operatorname{tr}D=0$:

$$
A=\frac12\left(\operatorname{tr}T-\frac ts\right),\qquad B=\frac{t/s-A}{s},\qquad C=\frac{PTv}{s},\qquad D=PTP-AP.
$$

The transverse restriction is a symmetric two-dimensional matrix, whose [traceless matrix](#traceless-matrix) part has dimension two. Together the two scalars, two components of $C$ and two components of $D$ give the six parameters of $T$.

### Symmetric positive-definite matrix

↑ **Parent:** [Symmetric matrix](#symmetric-matrix)

A real [symmetric matrix](#symmetric-matrix) is positive definite when its [quadratic form](#quadratic-form) is positive on every nonzero vector. By the [spectral theorem](hilbert-space.md#spectral-theorem), this is equivalent to all its [eigenvalues](linear-operator-theory.md#eigenvalue) being positive. It has a unique symmetric positive-definite square root.

### Coaxial symmetric tensors

↑ **Parent:** [Symmetric matrix](#symmetric-matrix)

Two real [symmetric matrices](#symmetric-matrix) are coaxial when they share an [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis). Equivalently they commute. Degenerate [eigenspaces](linear-operator-theory.md#eigenspace) can have several choices of shared axes.

### Real symmetric spectral orthogonality

↑ **Parent:** [Symmetric matrix](#symmetric-matrix)

A real [symmetric matrix](#symmetric-matrix) is a [Hermitian matrix](hilbert-space.md#hermitian-operator), so $u^*Au$ is real for every complex vector $u$. If $u$ is an [eigenvector](linear-operator-theory.md#eigenvector), its [eigenvalue](linear-operator-theory.md#eigenvalue) is $(u^*Au)/(u^*u)$ and is real. Then $u^*Av=(Au)^*v$ gives $(\mu-\lambda)u^*v=0$. Reality is used in changing conjugate transpose to transpose; complex symmetry alone does not imply real eigenvalues.

### Orthogonal diagonalization of a real symmetric matrix

↑ **Parent:** [Symmetric matrix](#symmetric-matrix)

A real [symmetric matrix](#symmetric-matrix) has real [eigenvalues](linear-operator-theory.md#eigenvalue), orthogonal [eigenspaces](linear-operator-theory.md#eigenspace) for distinct eigenvalues, and an [orthonormal basis](#orthonormal-basis) of eigenvectors. From diagonalizability, apply the [Gram-Schmidt process](#gram-schmidt-process) within each eigenspace; all its linear combinations stay in that eigenspace. This gives $A=Q\Lambda Q^T$ with an orthogonal matrix $Q$ and real diagonal $\Lambda$.

### Copositive matrix

↑ **Parent:** [Symmetric matrix](#symmetric-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Copositive_matrix)

A real [symmetric matrix](#symmetric-matrix) $A$ is copositive if its [quadratic form](#quadratic-form) satisfies $x^TAx\geq0$ for every $x$ in the [nonnegative orthant](mathematical-optimization.md#nonnegative-orthant). Every [positive semidefinite matrix](#positive-semidefinite-matrix) and every symmetric [nonnegative matrix](vector-space.md#nonnegative-matrix) is copositive, as is their sum. The converse fails for the [Horn copositive matrix](#horn-copositive-matrix).

#### Strictly copositive matrix

↑ **Parent:** [Copositive matrix](#copositive-matrix)

A real [symmetric matrix](#symmetric-matrix) whose [quadratic form](#quadratic-form) is positive at every nonzero [vector](vector-space.md#vector) in the [nonnegative orthant](mathematical-optimization.md#nonnegative-orthant). By [compactness](topology.md#compact-space) of the nonnegative [unit sphere](topology.md#unit-sphere), this is equivalent to a positive uniform lower bound $x^TAx\geq\delta\|x\|_2^2$ on that orthant. It need not be a [positive-definite matrix](#positive-definite-matrix).

#### Horn copositive matrix

↑ **Parent:** [Copositive matrix](#copositive-matrix)

The five-dimensional Horn copositive matrix has diagonal entries $1$, entries $-1$ on the edges of the five-cycle, and entries $1$ on the remaining pairs:

$$
H=\begin{pmatrix}
1&-1&1&1&-1\\
-1&1&-1&1&1\\
1&-1&1&-1&1\\
1&1&-1&1&-1\\
-1&1&1&-1&1
\end{pmatrix}.
$$

For $x\geq0$, a cyclic relabelling puts a smallest coordinate at $x_5$. The identity

$$
x^THx=(x_1-x_2+x_3-x_4+x_5)^2+4x_2x_5+4x_1(x_4-x_5)
$$

then proves that $H$ is a [copositive matrix](#copositive-matrix).

However, $H$ is outside the [positive-semidefinite-plus-nonnegative cone](mathematical-optimization.md#positive-semidefinite-plus-nonnegative-cone). Set $w=(1,2,1,0,0)^T$. Its [quadratic form](#quadratic-form) is zero. If $H=P+N$ with $P$ a [positive semidefinite matrix](#positive-semidefinite-matrix) and $N$ a symmetric [nonnegative matrix](vector-space.md#nonnegative-matrix), both $w^TPw$ and $w^TNw$ must vanish. Positivity of the first three coordinates of $w$ forces every entry of the leading $3\times3$ block of $N$ to vanish. Applying the argument to all cyclic shifts of $w$ forces every entry of $N$ to vanish, since each pair of indices lies in a cyclic interval of length three. This would make $H$ a [positive semidefinite matrix](#positive-semidefinite-matrix), but [zero quadratic form of a positive semidefinite matrix](#zero-quadratic-form-of-a-positive-semidefinite-matrix) would then give $Hw=0$, whereas $Hw=(0,0,0,2,2)^T$.

### Spectral theorem for real symmetric matrices

↑ **Parent:** [Symmetric matrix](#symmetric-matrix)

Every real symmetric matrix has an [orthonormal basis](#orthonormal-basis) of real eigenvectors. Equivalently, it admits an orthogonal diagonalization $A=O^TDO$ with $D$ real diagonal and $O$ an [orthogonal matrix](#orthogonal-matrix).

This is the finite-dimensional real-symmetric case of the [spectral theorem](hilbert-space.md#spectral-theorem).

## Axis-angle decomposition

↑ **Parent:** [Linear algebra](linear-algebra.md)

An axis-angle map fixes or scales one axis and acts on its perpendicular plane by a rotation, possibly combined with a dilation.

When the axis is fixed pointwise and the plane has no dilation, this reduces to an [axis-angle representation](#axis-angle-representation) of a three-dimensional [rotation](riemannian-geometry.md#rotation-mathematics).

### Inverse of an axis-angle linear map

↑ **Parent:** [Axis-angle decomposition](#axis-angle-decomposition)

Invert the axial scalar and invert the perpendicular complex scalar $\alpha+i\gamma$ as $(\alpha-i\gamma)/(\alpha^2+\gamma^2)$.

## Reflection (mathematics)

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reflection_(mathematics))

A reflection fixes a hyperplane pointwise and reverses its normal direction.

### Reflection matrix

↑ **Parent:** [Reflection (mathematics)](#reflection-mathematics)

A plane reflection with unit normal $n$ is $I-2nn^T$; it fixes the plane $n^\perp$ and negates $n$.

#### Composition of a plane rotation and a reflection

↑ **Parent:** [Reflection matrix](#reflection-matrix)

A [planar rotation](#planar-rotation) about a point on the axis of a [Euclidean reflection](#reflection-mathematics), composed after that [Euclidean reflection](#reflection-mathematics), is a [Euclidean reflection](#reflection-mathematics) whose axis has been rotated by half the rotation angle. In coordinates centred at the fixed point, with the original axis horizontal, write $S=\operatorname{diag}(1,-1)$. Then

$$
R_\alpha S=\begin{pmatrix}\cos\alpha&\sin\alpha\\\sin\alpha&-\cos\alpha\end{pmatrix}=R_{\alpha/2}SR_{-\alpha/2}.
$$

This [matrix](vector-space.md#matrix) fixes the direction $(\cos(\alpha/2),\sin(\alpha/2))$ and reverses its perpendicular direction. The axis is an unoriented line, so its angle is defined modulo $\pi$.

#### Reflection in a hyperplane

↑ **Parent:** [Reflection matrix](#reflection-matrix)

For a nonzero normal vector $a$, reflection in $a\cdot x=0$ has matrix

$$
I-\frac{2aa^T}{a^Ta}.
$$

Its eigenvalues are $-1$ along $a$ and $1$ on $a^\perp$, so its determinant is $-1$.

#### Composition of two plane reflections

↑ **Parent:** [Reflection matrix](#reflection-matrix)

The composition of reflections in two planes through the origin is a rotation about their line of intersection through twice the oriented angle between the planes.

## Rotation matrix

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rotation_matrix)

A rotation matrix is an orthogonal matrix with determinant $1$.

### Trace of a three-dimensional rotation

↑ **Parent:** [Rotation matrix](#rotation-matrix)

A proper three-dimensional [rotation matrix](#rotation-matrix) has an axis eigenvalue one and perpendicular-plane eigenvalues $e^{i\theta},e^{-i\theta}$. Their sum gives the displayed [trace](#matrix-trace) identity. It determines the angle cosine but does not by itself choose the oriented axis or angle sign.

### Planar rotation

↑ **Parent:** [Rotation matrix](#rotation-matrix)

A planar rotation about the origin is the [linear map](vector-space.md#linear-map) represented by the [rotation matrix](#rotation-matrix) $R_\theta=\left(\begin{smallmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{smallmatrix}\right)$. It preserves [inner products](#inner-product), lengths, oriented angles and area, with positive angles measured anticlockwise. Its inverse is $R_{-\theta}$ and its [determinant](#determinant) is one.

#### Finite groups of planar rotations are cyclic

↑ **Parent:** [Planar rotation](#planar-rotation)

A finite [group](group.md) of [planar rotations](#planar-rotation) about one point is a [cyclic group](group.md#cyclic-group). For a nontrivial group, choose its smallest positive rotation angle $\alpha$. Subtracting multiples of $\alpha$ from any other group angle leaves a group angle in $[0,\alpha)$, hence zero. Applying the same argument to $2\pi$ shows that $\alpha=2\pi/m$ for a positive integer $m$. The identity-only group is cyclic as well.

### Centralizer of a planar quarter-turn

↑ **Parent:** [Rotation matrix](#rotation-matrix)

For $J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$, the real [matrix](vector-space.md#matrix) solutions of $AJ=JA$ are precisely

$$
A=uI+vJ=\begin{pmatrix}u&-v\\v&u\end{pmatrix},\qquad u,v\in\mathbb R.
$$

A nonzero such matrix equals $\sqrt{u^2+v^2}\,R_\theta$, where $R_\theta$ is a planar [rotation matrix](#rotation-matrix) with $\cos\theta=u/\sqrt{u^2+v^2}$ and $\sin\theta=v/\sqrt{u^2+v^2}$. It acts like multiplication by the [complex number](complex-analysis.md#complex-number) $u+iv$. The zero matrix is the zero scalar multiple of any rotation.

### Rotational symmetry

↑ **Parent:** [Rotation matrix](#rotation-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rotational_symmetry)

An object has rotational symmetry when a nontrivial [rotation matrix](#rotation-matrix) leaves it unchanged.

#### Rotational symmetry group of a regular icosahedron

↑ **Parent:** [Rotational symmetry](#rotational-symmetry)

The orientation-preserving [rotational symmetry](#rotational-symmetry) group of a [regular icosahedron](geometry-and-topology.md#regular-icosahedron) has order sixty. Its [conjugacy classes](group-theory.md#conjugacy-class) have sizes $1,15,20,12,12$: identity; half-turns about opposite-edge axes; [rotations](riemannian-geometry.md#rotation-mathematics) through $\pm2\pi/3$ about opposite-face axes; and [rotations](riemannian-geometry.md#rotation-mathematics) through $\pm2\pi/5$ and $\pm4\pi/5$ about opposite-vertex axes, respectively. Conjugation carries an axis to its rotated axis and preserves the [rotation](riemannian-geometry.md#rotation-mathematics) angle. The [transitive group action](group-theory.md#transitive-group-action) on edges, faces and vertices gives the indicated classes, with reversal of the axis identifying the two signs. A [normal subgroup](group-theory.md#normal-subgroup) must contain whole [conjugacy classes](group-theory.md#conjugacy-class); none of the proper nonidentity sums of these class sizes is a divisor of sixty. Thus this group is a [simple group](finite-group-theory.md#simple-group).

#### Rotational symmetry group of a regular dodecahedron

↑ **Parent:** [Rotational symmetry](#rotational-symmetry)

The [rotations in three dimensions](#rotation-in-three-dimensions) preserving a [dodecahedron](geometry-and-topology.md#dodecahedron) form a group of order $60$. There are $24$ nonidentity rotations about the six axes through opposite face centres, $20$ about the ten axes through opposite vertices, and $15$ half-turns about the fifteen axes through opposite edge midpoints. Its nonidentity [conjugacy classes](group-theory.md#conjugacy-class) have sizes $12,12,20,15$: the [centralizer](group-theory.md#centralizer) of a rotation of order five or three consists of rotations about its oriented axis and has order five or three, respectively, while all edge half-turns are conjugate. A [normal subgroup](group-theory.md#normal-subgroup) is a union of whole [conjugacy classes](group-theory.md#conjugacy-class) containing the identity. No proper nontrivial sum of these class sizes plus one divides $60$, proving that it is a [simple group](finite-group-theory.md#simple-group). The [centralizers](group-theory.md#centralizer) of the fifteen [involutions](group-theory.md#involution) are five distinct [Klein four-groups](finite-group-theory.md#klein-four-group), each containing three [involutions](group-theory.md#involution). Conjugation permutes these five subgroups nontrivially. The kernel is a [normal subgroup](group-theory.md#normal-subgroup), so simplicity makes this nontrivial action injective. Its sign map to a group of order two must be trivial, since simplicity would otherwise force an impossible injection of sixty elements into two. Thus its image lies in the [alternating group](finite-group-theory.md#alternating-group) $A_5$, and equality of orders makes the image all of $A_5$.

## Cartesian coordinate system

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cartesian_coordinate_system)

A Cartesian coordinate system specifies a point by its signed components along mutually perpendicular coordinate axes.

### Quadrant (plane geometry)

↑ **Parent:** [Cartesian coordinate system](#cartesian-coordinate-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quadrant_(plane_geometry))

The two coordinate axes divide a [Cartesian coordinate system](#cartesian-coordinate-system) in the plane into four open quadrants, distinguished by the signs of their coordinates. The [positive quadrant](#positive-quadrant) is the first quadrant.

#### Positive quadrant

↑ **Parent:** [Quadrant (plane geometry)](#quadrant-plane-geometry)

The positive quadrant of the Cartesian plane is the set of points $(x,y)$ with $x>0$ and $y>0$.

## Matrix geometric series

↑ **Parent:** [Linear algebra](linear-algebra.md)

For invertible $I-A$, $\sum_{j=0}^{n-1}A^j=(I-A^n)(I-A)^{-1}$.

## Adjugate matrix

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Adjugate_matrix)

The adjugate is the transpose of the cofactor matrix and satisfies $A\operatorname{adj}(A)=(\det A)I$.

### Cofactor matrix

↑ **Parent:** [Adjugate matrix](#adjugate-matrix)

The [cofactor matrix](#cofactor-matrix) consists of the signed minors of a [matrix](vector-space.md#matrix). It is the transpose of the [adjugate matrix](#adjugate-matrix). The inverse expression applies to invertible matrices; the definition by minors also applies to singular matrices. Cofactors transform oriented hypersurface area vectors in a [change of variables formula](calculus.md#change-of-variables-formula).

#### Cofactor

↑ **Parent:** [Cofactor matrix](#cofactor-matrix)

The [cofactor](#cofactor) of a [matrix](vector-space.md#matrix) entry is the signed [determinant](#determinant) of the minor obtained by deleting its row and column. These scalars form the [cofactor matrix](#cofactor-matrix), and their transpose forms the [adjugate matrix](#adjugate-matrix). They give row and column expansions of the [determinant](#determinant), including for singular [matrices](vector-space.md#matrix).

### Adjugate identity

↑ **Parent:** [Adjugate matrix](#adjugate-matrix)

Every square matrix $M$ over a commutative ring satisfies

$$
M\operatorname{adj}(M)=\operatorname{adj}(M)M=\det(M)I.
$$

## Matrix equivalence

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_equivalence)

Equivalent matrices represent the same linear map after independent changes of domain and codomain bases.

### Rank normal form

↑ **Parent:** [Matrix equivalence](#matrix-equivalence)

Every matrix of rank $r$ is equivalent to a block matrix with $I_r$ in its upper-left corner and zeros elsewhere. This follows by choosing bases adapted to the kernel and image of the represented [linear map](vector-space.md#linear-map).

## Block upper triangular matrix

↑ **Parent:** [Linear algebra](linear-algebra.md)

A block upper triangular matrix is a [block matrix](vector-space.md#block-matrix) with square diagonal blocks and zero blocks below them. Its determinant is the product of the determinants of its diagonal blocks.

### Eigenvalue deflation by an invariant subspace

↑ **Parent:** [Block upper triangular matrix](#block-upper-triangular-matrix)

If a $k$-dimensional [invariant subspace](representation-theory.md#invariant-subspace) is mapped to the span of the first $k$ coordinate vectors by a [similarity transformation](#similarity-transformation), the transformed matrix has block form

$$
\begin{pmatrix}B&C\\0&D\end{pmatrix}.
$$

Its [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) factors as $\det(\lambda I-B)\det(\lambda I-D)$, so its eigenvalues are the eigenvalues of the two diagonal blocks, counted with [algebraic multiplicity](linear-operator-theory.md#algebraic-multiplicity).

## Sylvester equation

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sylvester_equation)

The Sylvester equation $AX-XB=C$ has a unique solution $X$ for every $C$ exactly when $A$ and $B$ have disjoint spectra.

## Rank inequality for a composition

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rank_inequality_for_a_composition)

For maps through a finite-dimensional intermediate space V, rank(alpha beta) is at least rank(alpha)+rank(beta)-dim(V).

### Frobenius rank inequality

↑ **Parent:** [Rank inequality for a composition](#rank-inequality-for-a-composition)

For compatible [matrices](vector-space.md#matrix) $P,Q,R$, the inequality is $\operatorname{rank}(PQ)+\operatorname{rank}(QR)\leq\operatorname{rank}(Q)+\operatorname{rank}(PQR)$. One proof uses the block [matrix](vector-space.md#matrix) $M=\begin{pmatrix}PQ&0\\Q&QR\end{pmatrix}$. Subtract $P$ times its lower block row from its upper block row and then subtract its first block column times $R$ from its second. The result is $\begin{pmatrix}0&-PQR\\Q&0\end{pmatrix}$, with rank $\operatorname{rank}(Q)+\operatorname{rank}(PQR)$. On the other hand, choose independent columns of $PQ$ from the first block column and independent columns of $QR$ from the second. The corresponding columns of $M$ are independent: project a relation onto the upper block first, and then onto the lower block. Thus $\operatorname{rank}(M)\geq\operatorname{rank}(PQ)+\operatorname{rank}(QR)$.

## Schur complement

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur_complement)

For an invertible block P, the Schur complement of P in a block matrix is $S-RP^{-1}Q$.

### Schur complement formula for a diagonal resolvent entry

↑ **Parent:** [Schur complement](#schur-complement)

For a [Hermitian matrix](hilbert-space.md#hermitian-operator), let $x_i$ be its $i$th column without the diagonal entry and let $G^{(i)}=(X^{(i)}-zI)^{-1}$. Solve the two block equations of the inverse against the $i$th coordinate vector to obtain this formula. Both full and minor inverses must exist; nonreal $z$ guarantees that. In the real symmetric case $x_i^*$ may be replaced by $x_i^T$.

## Orthogonal similarity

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orthogonal_similarity)

Orthogonal similarity maps A to QAQ^T and preserves eigenvalues and symmetry.

## Product of symmetric matrices

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Product_of_symmetric_matrices)

Every complex square matrix is a product of two symmetric matrices, one invertible.

## Inner product

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inner_product)

### Inner product space

↑ **Parent:** [Inner product](#inner-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inner_product_space)

An inner product space is a real or complex [vector space](vector-space.md) equipped with a positive-definite [inner product](#inner-product). Over the real numbers the form is symmetric and bilinear; over the complex numbers it is conjugate symmetric and sesquilinear. It defines the [norm](functional-analysis.md#norm) $\|v\|=\sqrt{\langle v,v\rangle}$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) proves the triangle inequality for this norm. A complete inner product space is a [Hilbert space](hilbert-space.md); every finite-dimensional inner product space is complete.

### Generalized parallelogram identity

↑ **Parent:** [Inner product](#inner-product)

Averaging squared norms of all signed sums of finitely many vectors in an inner-product space cancels every mixed term. This equates the average to the sum of the individual squared norms, distinguishing Hilbert-space geometry from other sequence-space norms.

### Fischer inner product

↑ **Parent:** [Inner product](#inner-product)

The Fischer inner product on [polynomials](polynomial.md) is $\langle x^\alpha,x^\beta\rangle_F=\alpha!\,\delta_{\alpha\beta}$. Multiplication by $x_i$ is adjoint to differentiation by $x_i$. Therefore multiplication by $|x|^2$ is adjoint to the ordinary [Laplacian](calculus.md#laplacian), yielding the [harmonic decomposition of homogeneous polynomials](partial-differential-equation.md#harmonic-decomposition-of-homogeneous-polynomials) by finite-dimensional orthogonality.

### Frobenius inner product

↑ **Parent:** [Inner product](#inner-product)

For complex [matrices](vector-space.md#matrix), the [inner product](#inner-product) $\langle A,B\rangle_F=\operatorname{tr}(A^*B)$ is conjugate-linear in its first argument. On real [symmetric matrices](#symmetric-matrix) it becomes $\operatorname{tr}(AB)$. In particular $\langle A,xx^T\rangle_F=x^TAx$, identifying [quadratic forms](#quadratic-form) with linear tests on [matrices](vector-space.md#matrix).

### Discrete L2 inner product

↑ **Parent:** [Inner product](#inner-product)

The discrete L2 inner product is the cell-volume-weighted [Hermitian inner product](#hermitian-form) on a uniform grid. Its associated [norm](functional-analysis.md#norm) is the [discrete L2 norm](functional-analysis.md#discrete-l2-norm). It provides the finite-dimensional analogue of spatial [integration by parts](calculus.md#integration-by-parts) and continuous [energy method](numerical-analysis.md#energy-method) identities.

### Weighted inner product

↑ **Parent:** [Inner product](#inner-product)

For a positive weight $w$, the weighted inner product of [functions](function.md) is $\langle f,g\rangle_w=\int\overline f g w$. It is the usual [inner product](#inner-product) in the [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) for the measure $w(x)dx$. A [Sturm-Liouville eigenfunction expansion](analysis.md#sturm-liouville-eigenfunction-expansion) uses this weight to make its [eigenfunctions](linear-operator-theory.md#eigenfunction) [orthogonal](#orthogonal-vectors).

### Dot product

↑ **Parent:** [Inner product](#inner-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dot_product)

The dot product of Euclidean vectors is $\mathbf a\cdot\mathbf b=\sum_i a_i b_i$. It equals $|\mathbf a||\mathbf b|\cos\theta$, where $\theta$ is the angle between them.

### Binary inner product

↑ **Parent:** [Inner product](#inner-product)

For $x,y\in\mathbb F_2^n$, the binary inner product is $x\cdot y=\sum_i x_iy_i$ in $\mathbb F_2$. Its value is the parity of the coordinates at which both vectors are one.

### Orthonormal set

↑ **Parent:** [Inner product](#inner-product)

An [orthonormal set](#orthonormal-set) consists of [vectors](vector-space.md#vector) that have [norm](functional-analysis.md#norm) one and are pairwise [orthogonal](#orthogonal-vectors). Its [Gram matrix](#gram-matrix) is the [identity matrix](vector-space.md#identity-matrix).

#### Orthonormal basis

↑ **Parent:** [Orthonormal set](#orthonormal-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orthonormal_basis)

An orthonormal basis is a [basis](vector-space.md#basis) whose vectors are pairwise [orthogonal](#orthogonal-vectors) and each have [norm](functional-analysis.md#normed-vector-space) one.

### Gram matrix

↑ **Parent:** [Inner product](#inner-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gram_matrix)

For vectors $v_1,\ldots,v_n$, the Gram matrix is

$$
G_{ij}=\langle v_i,v_j\rangle.
$$

Two finite vector families with the same Gram matrix are related by an isometry between their spans; in finite dimensions that isometry can be extended to a unitary map after completing orthonormal bases.

#### Unit vectors with a common inner product

↑ **Parent:** [Gram matrix](#gram-matrix)

For $n\geq2$, the [Gram matrix](#gram-matrix) of $n$ unit [vectors](vector-space.md#vector) with common distinct-pair [inner product](#inner-product) $t$ is $G=(1-t)I+t\mathbf1\mathbf1^T$. Its [eigenvalues](linear-operator-theory.md#eigenvalue) are $1+(n-1)t$ on the all-ones direction and $1-t$ on its orthogonal complement. It is a [positive-definite symmetric matrix](#symmetric-positive-definite-matrix) exactly when $-1/(n-1)<t<1$, permitting a linearly independent realization in $\mathbb R^n$. An explicit construction takes the columns of

$$
B=\sqrt{1-t}(I-uu^T)+\sqrt{1+(n-1)t}\,uu^T,
\qquad u=\mathbf1/\sqrt n.
$$

The two orthogonal projections have product zero, so $B^TB=G$; positive [eigenvalues](linear-operator-theory.md#eigenvalue) also make $B$ invertible. At either endpoint the corresponding eigenspace becomes a linear dependence.

#### Gram determinant

↑ **Parent:** [Gram matrix](#gram-matrix)

The determinant of a [Gram matrix](#gram-matrix) is nonnegative and vanishes precisely when its vectors are [linearly dependent](vector-space.md#linear-dependence). In Euclidean three-dimensional space, three column vectors form a square [matrix](vector-space.md#matrix) $V$, whose [Gram matrix](#gram-matrix) is $V^TV$. Its determinant is $(\det V)^2=[v_1\cdot(v_2\times v_3)]^2$, the square of the [scalar triple product](#scalar-triple-product) and of the parallelepiped volume.

#### Riesz dual basis in an inner product space

↑ **Parent:** [Gram matrix](#gram-matrix)

For a basis $(u_i)$ of a finite-dimensional [inner product space](#inner-product-space) with conjugate-linear first argument, define $G_{ij}=(u_i,u_j)$ and $\widehat u_k=\sum_l(G^{-1})_{lk}u_l$. Then $(u_i,\widehat u_k)=\delta_{ik}$ and $(\widehat u_j,\widehat u_k)=(G^{-1})_{jk}$. This is the inner-product representation of the [dual basis](#dual-basis); requiring the dual vectors to lie in the given span is essential.

#### Gaussian empirical Gram matrix

↑ **Parent:** [Gram matrix](#gram-matrix)

For a matrix $G$ with [independent](random-variable.md#independent-random-variables) standard normal entries, $G^TG/n$ is a [Gaussian empirical Gram matrix](#gaussian-empirical-gram-matrix) and has [expectation](probability-theory.md#expected-value) equal to the identity. With mean known to be zero it is the raw empirical second moment. Subtracting a sample mean would give a different estimator. On any fixed unit vector its [quadratic form](#quadratic-form) is a chi-squared variable divided by $n$.

##### Gaussian Gram matrix concentration on a fixed subspace

↑ **Parent:** [Gaussian empirical Gram matrix](#gaussian-empirical-gram-matrix)

For $G$ with $n$ [independent](random-variable.md#independent-random-variables) standard Gaussian rows in dimension $k$, combine a constant-radius sphere [metric net](topological-analysis.md#metric-net), the [quadratic form net bound](topological-analysis.md#quadratic-form-net-bound), the [chi-squared concentration inequality](probability-theory.md#chi-squared-concentration-inequality), and a [union bound](probability-inequality.md#boole-s-inequality). This gives $P(\|G^TG/n-I_k\|_{\mathrm{op}}>1/2)\leq2\exp(k\log B-n/1024)$ for a numerical $B$. Taking $n$ larger than a constant times $k\log p$ gives exponential decay in $k\log p$. The subspace is fixed, so no union over supports is needed.

#### Sparse norm preservation from entrywise Gram control

↑ **Parent:** [Gram matrix](#gram-matrix)

If $E=A^TA/d-I$ has [entrywise maximum norm](vector-space.md#entrywise-maximum-norm) at most $t$, every vector $z$ supported on at most $s$ coordinates satisfies $|z^TEz|\leq t\|z\|_1^2\leq st\|z\|_2^2$. Thus the squared norm distortion is at most $st$ on all such sparse vectors. Use the quadratic inequality at $z=0$, where a ratio would be undefined.

### Pythagorean theorem in an inner-product space

↑ **Parent:** [Inner product](#inner-product)

If $u$ and $v$ are orthogonal, then

$$
\lVert u+v\rVert^2=\lVert u\rVert^2+\lVert v\rVert^2.
$$

### Orthogonal projection onto a finite-dimensional subspace

↑ **Parent:** [Inner product](#inner-product)

If $e_0,\ldots,e_n$ is an orthogonal basis of a finite-dimensional subspace $W$, the unique closest point in $W$ to $f$ is

$$
P_Wf=\sum_{k=0}^n\frac{\langle f,e_k\rangle}{\langle e_k,e_k\rangle}e_k.
$$

The residual $f-P_Wf$ is orthogonal to $W$.

#### Orthogonal projection matrix

↑ **Parent:** [Orthogonal projection onto a finite-dimensional subspace](#orthogonal-projection-onto-a-finite-dimensional-subspace)

A complex matrix $P$ represents an [orthogonal projection](hilbert-space.md#orthogonal-projection) exactly when

$$
P^2=P=P^\dagger.
$$

Its image and kernel are orthogonal complements.

##### Transverse projection operator

↑ **Parent:** [Orthogonal projection matrix](#orthogonal-projection-matrix)

For a nonnull vector $k$ in a space with a nondegenerate bilinear form, $P_{\mu\nu}=\eta_{\mu\nu}-k_\mu k_\nu/k^2$ projects onto the subspace transverse to $k$. It obeys $P_{\mu\nu}k^\nu=0$ and $P^2=P$.

#### Least-squares polynomial in an orthogonal-polynomial basis

↑ **Parent:** [Orthogonal projection onto a finite-dimensional subspace](#orthogonal-projection-onto-a-finite-dimensional-subspace)

For orthogonal polynomials $Q_0,\ldots,Q_n$ under a positive weighted integral inner product, the least-squares approximation to $f$ of degree at most $n$ is

$$
p_n^*=\sum_{k=0}^n\frac{\langle f,Q_k\rangle}{\langle Q_k,Q_k\rangle}Q_k.
$$

Its residual is orthogonal to every polynomial of degree at most $n$.

### Orthogonal vectors

↑ **Parent:** [Inner product](#inner-product)

Two [vectors](vector-space.md#vector) are orthogonal when their [inner product](#inner-product) is zero.

#### Orthogonal basis

↑ **Parent:** [Orthogonal vectors](#orthogonal-vectors)

An [orthogonal basis](#orthogonal-basis) of an inner-product [vector space](vector-space.md) consists of nonzero mutually [orthogonal vectors](#orthogonal-vectors) that span the space. The [orthogonal projection](hilbert-space.md#orthogonal-projection) of $v$ onto a finite-dimensional span is $\sum_i\langle v,u_i\rangle u_i/\langle u_i,u_i\rangle$. Dividing each vector by its norm produces an [orthonormal basis](#orthonormal-basis). For centered random variables, the inner product is [covariance](variance.md#covariance); an orthogonal basis therefore consists of uncorrelated variables, without requiring unit variance.

### Nonorthogonal vectors

↑ **Parent:** [Inner product](#inner-product)

Two [vectors](vector-space.md#vector) are nonorthogonal when their [inner product](#inner-product) is nonzero. In the [power method](linear-operator-theory.md#power-method), the starting vector must be nonorthogonal to a dominant [eigenvector](linear-operator-theory.md#eigenvector).

### Gram-Schmidt process

↑ **Parent:** [Inner product](#inner-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gram-Schmidt_process)

The Gram-Schmidt process replaces linearly independent vectors $v_1,\ldots,v_n$ by orthogonal vectors with the same successive spans, subtracting from each $v_k$ its projections onto the preceding vectors.

#### QR decomposition

↑ **Parent:** [Gram-Schmidt process](#gram-schmidt-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/QR_decomposition)

A reduced QR decomposition of a full-column-rank matrix writes $A=QR$, where $Q$ has orthonormal columns and $R$ is upper triangular with positive diagonal.

##### Positive-diagonal QR decomposition preserves a complex structure

↑ **Parent:** [QR decomposition](#qr-decomposition)

Let $K$ be block diagonal with $2\times2$ blocks $J=\begin{pmatrix}0&1\\-1&0\end{pmatrix}$. If a real invertible [matrix](vector-space.md#matrix) $A$ commutes with $K$, its [QR decomposition](#qr-decomposition) $A=BC$, with $B$ orthogonal and $C$ upper triangular with positive diagonal, has both $BK=KB$ and $CK=KC$. Indeed $CKC^{-1}=B^{-1}KB$, so $E=K^{-1}CKC^{-1}$ is orthogonal and upper triangular in $2\times2$ blocks. Orthogonality forces its off-diagonal blocks to vanish. Its diagonal blocks are $J^{-1}C_iJC_i^{-1}$. For $C_i=\begin{pmatrix}a&b\\0&d\end{pmatrix}$ with $a,d>0$, this block is $\begin{pmatrix}d/a&-b/a\\-b/a&(a^2+b^2)/(ad)\end{pmatrix}$. Orthogonality of its columns forces $b=0,d=a$, and hence each block is the identity. Thus $E=I$, proving the claim.

##### Thin QR factorization from Cholesky decomposition

↑ **Parent:** [QR decomposition](#qr-decomposition)

If a real $m$-by-$n$ matrix $A$ has full column rank, with $m\ge n$, then $A^TA$ is [positive-definite](#positive-definite-bilinear-form). Its upper-triangular [Cholesky decomposition](#cholesky-decomposition) $A^TA=R^TR$, with positive diagonal, is unique. Defining $Q=AR^{-1}$ gives $Q^TQ=I$ and $A=QR$. Any other such factorization yields another Cholesky factor of $A^TA$, so its $R$ and then its $Q$ must agree. This proves existence and uniqueness; it does not assert that forming $A^TA$ is the most numerically stable algorithm.

##### Orthogonal coordinate reduction of a subspace

↑ **Parent:** [QR decomposition](#qr-decomposition)

For a full-column-rank $n\times k$ matrix $V$, extend the thin [QR decomposition](#qr-decomposition) $V=Q_1R_1$ to an [orthogonal matrix](#orthogonal-matrix) $Q=(Q_1\ Q_2)$. Then

$$
Q^TV=\begin{pmatrix}R_1\\0\end{pmatrix},
$$

so $Q^T$ maps the column space of $V$ onto the first $k$ coordinate directions. Successive [Householder transformations](#householder-transformation) construct the same reduction without first forming a full orthogonal basis.

##### Linear least-squares problem

↑ **Parent:** [QR decomposition](#qr-decomposition)

A linear least-squares problem minimizes $\|Ax-b\|_2$ over $x$. If $A=QR$ has full column rank, orthogonality reduces it to the upper-triangular system formed from the leading block of $R$ and the leading entries of $Q^Tb$.

#### Gram-Schmidt orthogonalization for a symmetric bilinear form

↑ **Parent:** [Gram-Schmidt process](#gram-schmidt-process)

For a symmetric bilinear form $B$, the same projection formula

$$
u_k=v_k-\sum_{j<k}\frac{B(v_k,u_j)}{B(u_j,u_j)}u_j
$$

produces a $B$-orthogonal basis whenever the chosen pivots $B(u_j,u_j)$ are nonzero. Reordering the input vectors can avoid a zero pivot when a suitable anisotropic vector remains.

## Quadratic form

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quadratic_form)

A quadratic form is a homogeneous degree-two function $Q(v)$ represented in coordinates by $v^TAv$ with $A$ symmetric.

### Polar bilinear form of a quadratic form

↑ **Parent:** [Quadratic form](#quadratic-form)

The displayed [bilinear form](#bilinear-form) is the polar form of a [quadratic form](#quadratic-form). In odd [characteristic of a field](algebra.md#characteristic-of-a-field), $Q(x)=B_Q(x,x)/2$ recovers the [quadratic form](#quadratic-form); in [characteristic of a field](algebra.md#characteristic-of-a-field) two, different forms can have the same [alternating bilinear form](#alternating-bilinear-form). Over $\mathbb F_2$, two such forms differ by a [linear map](vector-space.md#linear-map) to the [field](algebra.md#field), giving the affine parametrization of [binary quadratic refinements](#binary-quadratic-refinement).

### Integral quadratic lattice

↑ **Parent:** [Quadratic form](#quadratic-form)

An integral quadratic lattice is a finite-rank [free abelian group](group-theory.md#free-abelian-group) with a nondegenerate integral symmetric [bilinear form](#bilinear-form). Its norm convention here is $q(x)=B(x,x)$. A basis gives an integral [Gram matrix](#gram-matrix); basis changes preserve its determinant up to multiplication by the square of a unit.

#### Even lattice

↑ **Parent:** [Integral quadratic lattice](#integral-quadratic-lattice)

Every vector in an even lattice has even integral norm. The [E8 lattice](#e8-lattice) and the hyperbolic plane appearing in the [K3 intersection lattice](complex-geometry.md#k3-intersection-lattice) are examples.

#### Unimodular lattice

↑ **Parent:** [Integral quadratic lattice](#integral-quadratic-lattice)

The integral Gram determinant has absolute value one, equivalently the lattice equals its bilinear-form dual. The [K3 intersection lattice](complex-geometry.md#k3-intersection-lattice) is an indefinite example.

##### Even unimodular lattice

↑ **Parent:** [Unimodular lattice](#unimodular-lattice)

An [integral quadratic lattice](#integral-quadratic-lattice) that is both an [even lattice](#even-lattice) and a [unimodular lattice](#unimodular-lattice). The [K3 intersection lattice](complex-geometry.md#k3-intersection-lattice) has signature $(3,19)$, while the positive-definite [E8 lattice](#e8-lattice) has rank eight.

###### E8 lattice

↑ **Parent:** [Even unimodular lattice](#even-unimodular-lattice)

The positive-definite rank-eight [even unimodular lattice](#even-unimodular-lattice) can be realized as vectors in $\mathbb Z^8$ or $(\mathbb Z+1/2)^8$ whose coordinate sum is even, with the ordinary Euclidean inner product. Negating this form gives $E_8(-1)$ in the [K3 intersection lattice](complex-geometry.md#k3-intersection-lattice).

### Off-diagonal all-ones quadratic form

↑ **Parent:** [Quadratic form](#quadratic-form)

Its symmetric matrix is $\mathbf1\mathbf1^T-I$. The line spanned by $\mathbf1$ has eigenvalue $n-1$ and its orthogonal complement has eigenvalue $-1$. Thus for $n>1$ it is nondegenerate with inertia $(1,n-1,0)$; for $n=1$ it vanishes. This gives a useful explicit example for [Sylvester's law of inertia](#sylvester-s-law-of-inertia).

### Arf invariant of a quadratic form

↑ **Parent:** [Quadratic form](#quadratic-form)

For a nonsingular quadratic form over $\mathbb F_2$ with symplectic basis $(e_i,f_i)$, the invariant is $\sum_iQ(e_i)Q(f_i)$. For fixed polar form in dimension $2m$, the two types have $2^{m-1}(2^m+1)$ and $2^{m-1}(2^m-1)$ forms.

#### Binary quadratic refinement

↑ **Parent:** [Arf invariant of a quadratic form](#arf-invariant-of-a-quadratic-form)

A [binary quadratic refinement](#binary-quadratic-refinement) of a fixed nonsingular [alternating bilinear form](#alternating-bilinear-form) $B$ has polar form $B$. The difference of two refinements is linear, so nondegeneracy gives the displayed unique parametrization by $v$. For $\dim V=2m$, refinements of plus and minus [Arf invariant of a quadratic form](#arf-invariant-of-a-quadratic-form) have respectively $2^{m-1}(2^m+1)$ and $2^{m-1}(2^m-1)$ elements. Completing the square in the binary character sum gives $\epsilon(Q_v)=\epsilon(Q_0)(-1)^{Q_0(v)}$.

##### Two-transitive binary quadratic-form actions

↑ **Parent:** [Binary quadratic refinement](#binary-quadratic-refinement)

The [symplectic group over a finite field](finite-group-theory.md#symplectic-group-over-a-finite-field) is transitive on each of the two quadratic types. The stabilizer of a refinement is its [orthogonal group over a finite field](group-theory.md#orthogonal-group-over-a-finite-field). In the displayed parametrization, other refinements of the same type correspond to nonzero singular vectors, and refinements of opposite type to nonsingular vectors. [Witt's lemma](#witt-s-theorem) makes the orthogonal stabilizer transitive on each of these vector sets. Thus both type actions are [two-transitive](group-theory.md#two-transitive-group-action) for $m\ge2$, and a minus stabilizer is transitive on the plus orbit. For $m=1$ the minus orbit is a singleton.

### Symmetric coefficients of a quadratic polynomial

↑ **Parent:** [Quadratic form](#quadratic-form)

A quadratic [homogeneous polynomial](algebra.md#homogeneous-polynomial) determines a unique symmetric bilinear coefficient tensor. An antisymmetric addition to its coefficient array gives zero contribution, so tensorial conditions on its coefficients must refer to this symmetric representative. In particular, the correspondence between [quadratic geodesic first integrals](riemannian-geometry.md#quadratic-geodesic-first-integral) and [rank-two Killing tensors](riemannian-geometry.md#rank-two-killing-tensor) uses symmetric coefficients.

### Principal-axis reduction of a quadric

↑ **Parent:** [Quadratic form](#quadratic-form)

Write a real quadratic polynomial as $x^THx+2q^Tx+c$, with $H$ symmetric. If $H$ is invertible, translation by $x_0=-H^{-1}q$ removes the linear term. An orthonormal eigenbasis then makes the remaining [quadratic form](#quadratic-form) diagonal. Eigenvalue signs and the translated constant determine the real geometry, such as an ellipsoid or a [one-sheet hyperboloid](differential-geometry.md#one-sheet-hyperboloid). A singular $H$ requires separate treatment of linear terms in its null directions; a center need not exist.

### Matrix congruence

↑ **Parent:** [Quadratic form](#quadratic-form)

Two [symmetric matrices](#symmetric-matrix) are congruent when $C=P^TAP$ for an [invertible matrix](#invertible-matrix) $P$. This is the transformation of a [quadratic form](#quadratic-form) under an invertible linear change of coordinates. It differs from [matrix similarity](#matrix-similarity), which uses $P^{-1}AP$. [Completing the square](polynomial.md#completing-the-square) diagonalizes a real [quadratic form](#quadratic-form) by [matrix congruence](#matrix-congruence).

#### Simultaneous congruence diagonalization with a positive form

↑ **Parent:** [Matrix congruence](#matrix-congruence)

If $A$ is real symmetric positive definite and $B$ is real symmetric, let $S=A^{-1/2}$. The matrix $SBS$ is symmetric and has an orthonormal eigenbasis, represented by $Q$. Taking $P=SQ$ gives the two displayed congruences. The diagonal entries are determined by the [generalized eigenvalue problem](linear-operator-theory.md#generalized-eigenvalue-problem) $\det(B-\lambda A)=0$, since $P^T(B-\lambda A)P$ is diagonal with entries $\lambda_j-\lambda$. Positive definiteness of the first form is essential to this construction.

### Positive-definite quadratic form

↑ **Parent:** [Quadratic form](#quadratic-form)

A real quadratic form $q$ is positive definite when $q(v)>0$ for every nonzero vector $v$. In a basis that diagonalizes it, this is equivalent to every diagonal coefficient being positive.

### Ternary quadratic form

↑ **Parent:** [Quadratic form](#quadratic-form)

A ternary quadratic form is a [quadratic form](#quadratic-form) in three variables. A diagonal integral example is $aX^2+bY^2+cZ^2$ with integer coefficients $a,b,c$.

#### Isotropy of nondegenerate ternary quadratic forms over finite fields

↑ **Parent:** [Ternary quadratic form](#ternary-quadratic-form)

Over a [finite field](algebra.md#finite-field) of odd cardinality $q$, a diagonal nondegenerate [ternary quadratic form](#ternary-quadratic-form) $A x^2+B y^2+C z^2$ has a zero with $z=1$: the sets $\{A x^2\}$ and $\{-C-B y^2\}$ both have $(q+1)/2$ elements and must intersect. This gives a nonzero nonsingular zero. Over a local integer ring with these coefficients units, the [Hensel lemma](arithmetic.md#hensel-s-lemma) lifts it to an isotropic vector in the fraction field.

##### Local isotropy of the five seven thirteen form

↑ **Parent:** [Isotropy of nondegenerate ternary quadratic forms over finite fields](#isotropy-of-nondegenerate-ternary-quadratic-forms-over-finite-fields)

This [ternary quadratic form](#ternary-quadratic-form) has a nonzero zero over $\mathbb Q_p$ exactly when $p\ne7$. Away from $2,5,7,13$, the finite-field square-set intersection proof supplies a nonsingular residue zero, and [Hensel lemma](arithmetic.md#hensel-s-lemma) lifts it. At 5 use $(0,1,1)$ modulo 5; at 13 use $(3,1,0)$. At 2 hold $x=2,z=1$ and apply the [strong form of Hensel lemma](arithmetic.md#strong-form-of-hensel-lemma) to $7Y^2+33$ at $Y=1$: the function and derivative have [valuations](algebra.md#valuation) 3 and 1. At 7, the equation modulo 7 forces $x=z=0$ because 5 is not a square; reduction after dividing by 7 then forces $y=0$. Any normalized integral nonzero solution would therefore have all coordinates divisible by 7, a contradiction.

### Hyperbolic plane (quadratic form)

↑ **Parent:** [Quadratic form](#quadratic-form)

A hyperbolic plane is a two-dimensional [vector space](vector-space.md) with a [quadratic form](#quadratic-form) and a [basis](vector-space.md#basis) $e,f$ satisfying $q(e)=q(f)=0$ and $B(e,f)=1$, where $B$ is the [polar bilinear form of a quadratic form](#polar-bilinear-form-of-a-quadratic-form). Equivalently, $q(xe+yf)=xy$. This definition also applies in characteristic two. Over the [real numbers](arithmetic.md#real-number), the identity $xy=((x+y)/2)^2-((x-y)/2)^2$ gives one positive and one negative square, hence signature zero. The signature statement is specific to real quadratic forms.

### Parallelogram law

↑ **Parent:** [Quadratic form](#quadratic-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parallelogram_law)

The parallelogram law for a quadratic form $Q$ is

$$
Q(x+y)+Q(x-y)=2Q(x)+2Q(y).
$$

Conversely, under the usual divisibility assumptions, a function satisfying this identity and the appropriate homogeneity comes from a symmetric bilinear form by polarization.

### Rank of a quadratic form

↑ **Parent:** [Quadratic form](#quadratic-form)

The rank of a quadratic form is the rank of its associated symmetric bilinear form.

#### Rank-one quadratic form

↑ **Parent:** [Rank of a quadratic form](#rank-of-a-quadratic-form)

A rank-one quadratic form is the square of a [linear form](#linear-functional) up to a scalar. More generally, a bilinear expression $(u^Tx)(v^Ty)$ is rank one because its coefficient matrix is the [outer product](vector-space.md#outer-product) $uv^T$.

### Signature of a quadratic form

↑ **Parent:** [Quadratic form](#quadratic-form)

The signature of a real quadratic form is the number of positive squares minus the number of negative squares in its diagonal normal form.

### Polarization identity

↑ **Parent:** [Quadratic form](#quadratic-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polarization_identity)

Over a field of characteristic other than two, a quadratic form recovers its symmetric bilinear form by

$$
B(u,v)=\frac12\bigl(Q(u+v)-Q(u)-Q(v)\bigr).
$$

#### Polarization argument for a vanishing quadratic form

↑ **Parent:** [Polarization identity](#polarization-identity)

For a complex sesquilinear form $B$, the values $B(x,x)$ determine $B(x,y)$. In particular, expanding at $x+y$ and $x+iy$ shows that $B(x,x)=0$ for every $x$ implies $B=0$. Over the reals this conclusion can fail for nonsymmetric bilinear forms, as a nonzero skew-symmetric form has zero diagonal.

### Positive semidefinite bilinear form

↑ **Parent:** [Quadratic form](#quadratic-form)

A symmetric bilinear form is positive semidefinite when $B(v,v)\geq0$ for every $v$, and positive definite when equality is possible only for $v=0$.

### Definite matrix

↑ **Parent:** [Quadratic form](#quadratic-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Definite_matrix)

A definite matrix is a Hermitian matrix whose associated quadratic form has a fixed sign. Positive and negative semidefinite matrices allow zero as well.

#### Positive semidefinite matrix

↑ **Parent:** [Definite matrix](#definite-matrix)

A real symmetric or complex Hermitian matrix $A$ is positive semidefinite when $x^\dagger Ax\geq0$ for every [vector](vector-space.md#vector) $x$, equivalently when all its [eigenvalues](linear-operator-theory.md#eigenvalue) are nonnegative.

##### Bipartite block-constant positive semidefinite matrix

↑ **Parent:** [Positive semidefinite matrix](#positive-semidefinite-matrix)

For positive block sizes, the real [matrix](vector-space.md#matrix) $\begin{pmatrix}aJ&bJ\\bJ&aJ\end{pmatrix}$ is a [positive semidefinite matrix](#positive-semidefinite-matrix) exactly when $a\geq|b|$. For test-vector block sums $s,t$, its [quadratic form](#quadratic-form) is $(a+b)(s+t)^2/2+(a-b)(s-t)^2/2$. This proves sufficiency; testing $s=\pm t$ proves necessity. Zero sums in both blocks describe part of its [kernel](#kernel-of-a-linear-map).

##### Completely positive matrix

↑ **Parent:** [Positive semidefinite matrix](#positive-semidefinite-matrix)

A real [symmetric matrix](#symmetric-matrix) admitting a finite sum of nonnegative [rank-one matrices](vector-space.md#rank-one-matrix) $x_jx_j^T$. It is both a [positive semidefinite matrix](#positive-semidefinite-matrix) and a [nonnegative matrix](vector-space.md#nonnegative-matrix), but these two properties alone need not imply membership in the [completely positive cone](mathematical-optimization.md#completely-positive-cone) in arbitrary [dimension](vector-space.md#dimension-vector-space). This [matrix](vector-space.md#matrix) notion is distinct from a [completely positive map](quantum-information-theory.md#completely-positive-map).

##### Zero quadratic form of a positive semidefinite matrix

↑ **Parent:** [Positive semidefinite matrix](#positive-semidefinite-matrix)

If $P$ is a real [positive semidefinite matrix](#positive-semidefinite-matrix), then $x^TPx=0$ if and only if $Px=0$. Indeed $x^TPx=\|\sqrt P\,x\|^2$ by the [principal square root of a positive semidefinite matrix](#principal-square-root-of-a-positive-semidefinite-matrix), so a zero [quadratic form](#quadratic-form) puts $x$ in the [kernel](#kernel-of-a-linear-map) of $\sqrt P$ and hence of $P$.

##### Positive semidefinite trace nonnegativity

↑ **Parent:** [Positive semidefinite matrix](#positive-semidefinite-matrix)

For real [positive semidefinite matrices](#positive-semidefinite-matrix) $A,B$, their product need not be symmetric, but its [matrix trace](#matrix-trace) is nonnegative:

$$
\operatorname{tr}(AB)=\operatorname{tr}(\sqrt A\,B\sqrt A)\geq0.
$$

The equality uses the cyclic property of the [matrix trace](#matrix-trace), and the last [matrix](vector-space.md#matrix) is a [positive semidefinite matrix](#positive-semidefinite-matrix). Consequently the [Loewner order](#loewner-order) inequality $A\preceq C$ implies $\operatorname{tr}(AB)\leq\operatorname{tr}(CB)$ whenever $B\succeq0$.

##### Loewner order

↑ **Parent:** [Positive semidefinite matrix](#positive-semidefinite-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loewner_order)

The Loewner order on [Hermitian matrices](hilbert-space.md#hermitian-operator) is defined by $A\preceq B$ when $B-A$ is a [positive semidefinite matrix](#positive-semidefinite-matrix).

##### Square root of a matrix

↑ **Parent:** [Positive semidefinite matrix](#positive-semidefinite-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Square_root_of_a_matrix)

A square root of a square matrix $A$ is a matrix $B$ satisfying $B^2=A$.

###### Principal square root of a positive semidefinite matrix

↑ **Parent:** [Square root of a matrix](#square-root-of-a-matrix)

If $A=Q\operatorname{diag}(\lambda_1,\ldots,\lambda_n)Q^T$ is real symmetric and positive semidefinite, its principal square root is

$$
\sqrt A=Q\operatorname{diag}(\sqrt{\lambda_1},\ldots,\sqrt{\lambda_n})Q^T.
$$

It is symmetric and positive semidefinite, and is positive definite exactly when $A$ is.

###### Polar decomposition of an invertible real matrix

↑ **Parent:** [Principal square root of a positive semidefinite matrix](#principal-square-root-of-a-positive-semidefinite-matrix)

Every invertible real matrix has the polar decomposition

$$
M=RP,
\qquad
P=\sqrt{M^TM},
\qquad
R=MP^{-1},
$$

where $P$ is symmetric positive definite and $R$ is orthogonal.

This is the invertible real-matrix case of [polar decomposition](linear-operator-theory.md#polar-decomposition).

###### Polar decomposition of an invertible complex matrix

↑ **Parent:** [Polar decomposition of an invertible real matrix](#polar-decomposition-of-an-invertible-real-matrix)

Every invertible complex matrix has the unique polar decomposition

$$
M=PU,
\qquad
P=\sqrt{MM^*},
\qquad
U=P^{-1}M,
$$

where $P$ is a positive-definite [Hermitian matrix](hilbert-space.md#hermitian-operator) and $U$ is a [unitary matrix](linear-operator-theory.md#unitary-matrix). Writing $P=e^B$ gives $B=\frac12\log(MM^*)$, which is Hermitian.

#### Positive-definite matrix

↑ **Parent:** [Definite matrix](#definite-matrix)

A real symmetric matrix $A$ is positive definite when

$$
x^TAx>0
$$

for every nonzero real [vector](vector-space.md#vector) $x$. It therefore defines the [inner product](#inner-product) $\langle x,y\rangle_A=x^TAy$ and is invertible.

##### Cholesky decomposition

↑ **Parent:** [Positive-definite matrix](#positive-definite-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cholesky_decomposition)

Every real symmetric [positive-definite matrix](#positive-definite-matrix) has a unique factorization $A=LL^T$ in which $L$ is a lower [triangular matrix](#triangular-matrix) with positive diagonal entries.

###### Rank-one Cholesky update

↑ **Parent:** [Cholesky decomposition](#cholesky-decomposition)

Given a [Cholesky decomposition](#cholesky-decomposition) $A=LL^T$, a rank-one Cholesky update computes a triangular factor of $A+xx^T$ in $O(n^2)$ operations without refactorizing the matrix from scratch.

<h5 id="sylvester-s-criterion">Sylvester's criterion</h5>

↑ **Parent:** [Positive-definite matrix](#positive-definite-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sylvester's_criterion)

A Hermitian matrix is positive definite exactly when all its leading principal minors are positive.

##### Condition number

↑ **Parent:** [Positive-definite matrix](#positive-definite-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Condition_number)

The condition number of a problem measures how strongly relative perturbations of its input can amplify relative changes in its output. For an invertible matrix and a chosen operator norm, $\kappa(A)=\lVert A\rVert\lVert A^{-1}\rVert$.

###### Spectral condition number of a positive-definite matrix

↑ **Parent:** [Condition number](#condition-number)

For a real symmetric positive-definite matrix,

$$
\kappa_2(A)=\frac{\lambda_{\max}(A)}{\lambda_{\min}(A)}.
$$

It measures the sensitivity of the linear system and controls convergence bounds for iterative solvers.

##### Hermitian positive-definite matrix

↑ **Parent:** [Positive-definite matrix](#positive-definite-matrix)

A complex matrix $A$ is Hermitian positive definite when $A^*=A$ and $z^*Az>0$ for every nonzero complex vector $z$.

###### Toeplitz matrix

↑ **Parent:** [Hermitian positive-definite matrix](#hermitian-positive-definite-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Toeplitz_matrix)

A Toeplitz matrix is constant along each diagonal, so its entries have the form $T_{nm}=t_{n-m}$.

###### Symmetric tridiagonal Toeplitz matrix

↑ **Parent:** [Toeplitz matrix](#toeplitz-matrix)

An $m\times m$ symmetric tridiagonal Toeplitz matrix has one constant diagonal $\alpha$ and equal constant subdiagonal and superdiagonal $\beta$. Its eigenvectors are the [discrete sine transform](numerical-analysis.md#discrete-sine-transform) vectors $q^{(k)}_j=\sin(jk\pi/(m+1))$, with eigenvalues $\alpha+2\beta\cos(k\pi/(m+1))$.

###### Toeplitz antisymmetric tridiagonal matrix

↑ **Parent:** [Toeplitz matrix](#toeplitz-matrix)

An $M\times M$ Toeplitz antisymmetric tridiagonal matrix with diagonal $a$, superdiagonal $b$, and subdiagonal $-b$ has eigenvalues

$$
\lambda_j=a+2ib\cos\frac{j\pi}{M+1},
\qquad 1\leq j\leq M.
$$

All such matrices share an orthonormal eigenbasis after the same diagonal unitary change from the discrete sine basis.

#### Negative-definite matrix

↑ **Parent:** [Definite matrix](#definite-matrix)

A real symmetric matrix $A$ is negative definite when $x^TAx<0$ for every nonzero real [vector](vector-space.md#vector) $x$. Equivalently, $-A$ is a [positive-definite matrix](#positive-definite-matrix) and every [eigenvalue](linear-operator-theory.md#eigenvalue) of $A$ is negative.

<h3 id="sylvester-s-law-of-inertia">Sylvester's law of inertia</h3>

↑ **Parent:** [Quadratic form](#quadratic-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sylvester's_law_of_inertia)

Every real quadratic form is congruent to a diagonal form with entries $+1,-1,0$, and the numbers of entries of each kind are invariant.

#### Criterion for membership in a diagonal basis

↑ **Parent:** [Sylvester's law of inertia](#sylvester-s-law-of-inertia)

A vector $v$ can be included in a diagonal [basis](vector-space.md#basis) for a real [quadratic form](#quadratic-form) precisely when $v\ne0$ and either its quadratic value is nonzero or it lies in the [radical of a bilinear form](#radical-of-a-bilinear-form). A nonzero quadratic value gives the direct splitting $\mathbb Rv\oplus v^\perp$ and induction. A nonzero radical vector can be included in a radical basis. Conversely, an [isotropic vector](#isotropic-vector) in a diagonal basis is orthogonal to every basis vector, and must lie in the radical.

### Isotropic quadratic form

↑ **Parent:** [Quadratic form](#quadratic-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isotropic_quadratic_form)

An isotropic quadratic form has a nonzero vector on which it vanishes.

#### Hasse-Minkowski theorem

↑ **Parent:** [Isotropic quadratic form](#isotropic-quadratic-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hasse–Minkowski_theorem)

A nondegenerate [quadratic form](#quadratic-form) over a [number field](algebraic-number-theory.md#number-field) is isotropic if and only if it is isotropic over every completion. Over $\mathbb Q$, these are the real field and all [P-adic numbers](arithmetic.md#p-adic-number). It turns a rational existence problem into local tests; denominators can then be cleared for an integral homogeneous equation.

##### Hasse invariant of a quadratic form

↑ **Parent:** [Hasse-Minkowski theorem](#hasse-minkowski-theorem)

For a nondegenerate diagonal [quadratic form](#quadratic-form) $q=\langle a_1,\ldots,a_m\rangle$, this product of [quadratic Hilbert symbols](arithmetic.md#quadratic-hilbert-symbol) is independent of diagonalization. Over a [p-adic field](arithmetic.md#p-adic-field), dimension, determinant square class and this invariant classify the form up to isometry. The product of the local invariants of a globally diagonalized form is one by the [Hilbert reciprocity law](arithmetic.md#hilbert-reciprocity-law); real places additionally record signature.

#### Totally isotropic subspace

↑ **Parent:** [Isotropic quadratic form](#isotropic-quadratic-form)

A subspace $E$ is totally isotropic for $B$ when $B(u,v)=0$ for all $u,v\in E$. For a real [nondegenerate bilinear form](#nondegenerate-bilinear-form) of inertia $(p,q)$, its dimension is at most $\min(p,q)$.

##### Isotropic dimension bound from real inertia

↑ **Parent:** [Totally isotropic subspace](#totally-isotropic-subspace)

For a nondegenerate real [quadratic form](#quadratic-form) of inertia $(p,q)$, projection of a totally isotropic subspace onto either its positive or negative coordinate subspace is injective: a vector with one projection zero would have strictly one-signed quadratic value unless it vanished. Thus its dimension is at most both $p$ and $q$. This bound is attained by pairing one positive and one negative coordinate for each of $\min(p,q)$ independent null vectors.

##### Complex quadratic forms have a large isotropic subspace

↑ **Parent:** [Totally isotropic subspace](#totally-isotropic-subspace)

A [quadratic form](#quadratic-form) of rank $r$ on $\mathbb C^n$ is congruent to $x_1^2+\cdots+x_r^2$. Pair its nonzero coordinates into vectors $e_{2j-1}+ie_{2j}$, and include the [radical of a bilinear form](#radical-of-a-bilinear-form). Their span is a [totally isotropic subspace](#totally-isotropic-subspace) and has dimension $\lfloor r/2\rfloor+n-r=n-\lceil r/2\rceil\ge\lfloor n/2\rfloor$. The form vanishes on every vector of this subspace, not merely on its basis vectors.

###### Common zero of complex quadratic forms

↑ **Parent:** [Complex quadratic forms have a large isotropic subspace](#complex-quadratic-forms-have-a-large-isotropic-subspace)

Any $d$ [quadratic forms](#quadratic-form) on $\mathbb C^n$ have a common nonzero zero when $n\ge2^d$. Choose a [totally isotropic subspace](#totally-isotropic-subspace) for the first form, of dimension at least $\lfloor n/2\rfloor$. Restrict the remaining forms to it and repeat by induction. After $d$ stages at least one dimension remains. This elementary sufficient bound does not assert that $2^d$ is the best possible threshold.

##### Maximum dimension of a totally isotropic subspace

↑ **Parent:** [Totally isotropic subspace](#totally-isotropic-subspace)

For a real [quadratic form](#quadratic-form) on an $n$-dimensional [vector space](vector-space.md), with rank $r$ and signature $s$ defined as positive minus negative index, the maximum dimension of a [totally isotropic subspace](#totally-isotropic-subspace) is $n-(r+|s|)/2$. Quotienting by the [radical of a bilinear form](#radical-of-a-bilinear-form) leaves a nondegenerate form of indices $p,q$. Projection of an isotropic subspace to each sign-coordinate space is injective, bounding its dimension by $\min(p,q)$. The radical and vectors pairing one positive with one negative unit coordinate attain the bound $n-r+\min(p,q)$.

#### Isotropic vector

↑ **Parent:** [Isotropic quadratic form](#isotropic-quadratic-form)

A vector $v$ is isotropic for a quadratic form $q$ when $q(v)=0$.

### Quadratic form gradient

↑ **Parent:** [Quadratic form](#quadratic-form)

For symmetric $A$, the quadratic form $x^TAx$ has gradient $2Ax$.

## Schur product theorem

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur_product_theorem)

The entrywise product of two positive semidefinite matrices is positive semidefinite. Writing each matrix as a sum of rank-one Gram matrices reduces the claim to $(uu^T)\circ(vv^T)=(u\circ v)(u\circ v)^T$.

### Coefficient-dominated entrywise positivity

↑ **Parent:** [Schur product theorem](#schur-product-theorem)

Let real [power series](real-analysis.md#power-series) $f(t)=\sum_{k\geq0}f_kt^k$ and $g(t)=\sum_{k\geq0}g_kt^k$ converge on $[-1,1]$, with $f_k\geq|g_k|$ for every index including zero. If $X\succeq0$ has entries there, applying $f$ within two diagonal blocks and $g$ across them preserves [positive semidefiniteness](#positive-semidefinite-matrix). Indeed the [coefficient](vector-space.md#coefficient) [matrix](vector-space.md#matrix) $H_k$ is a [bipartite block-constant positive semidefinite matrix](#bipartite-block-constant-positive-semidefinite-matrix). Each $H_k\circ X^{\circ k}$ is [positive semidefinite](#positive-semidefinite-matrix) by the [Schur product theorem](#schur-product-theorem), and their sum converges to the transformed [matrix](vector-space.md#matrix). Closedness of the [positive semidefinite cone](mathematical-optimization.md#positive-semidefinite-cone) completes the proof. Convergence at one gives $\sum f_k<\infty$, so [coefficient](vector-space.md#coefficient) domination ensures [absolute convergence](real-analysis.md#absolute-convergence) of both series throughout the interval. Without the zero-index condition, $f=-1$, $g=0$ and $X=0$ give a counterexample.

## Orthogonal group

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orthogonal_group)

The real orthogonal group is $O(n)=\{R:R^TR=I\}$. Its tangent space at the identity is the vector space of skew-symmetric matrices.

### Orthogonal group as a regular level set

↑ **Parent:** [Orthogonal group](#orthogonal-group)

The smooth Gram map $F(A)=A^TA$ takes real matrices to symmetric matrices. At an orthogonal $A$, its derivative sends $AH/2$ to any prescribed symmetric matrix $H$. The regular level set $F^{-1}(I)$ is therefore a [smooth manifold](differential-geometry.md#smooth-manifold) of the displayed dimension.

// Target: geometry-and-topology.bigb

<h3 id="cartan-dieudonne-theorem">Cartan–Dieudonné theorem</h3>

↑ **Parent:** [Orthogonal group](#orthogonal-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cartan–Dieudonné_theorem)

Every [orthogonal transformation](#orthogonal-transformation) of a finite-dimensional nondegenerate quadratic space over a field of characteristic different from two is a product of at most its [dimension](vector-space.md#dimension-vector-space) many hyperplane reflections. In the real positive-definite case, a reflection normal to $gv-v$ sends $gv$ to $v$ whenever $gv\ne v$. Composing with that reflection fixes $v$ and leaves an [orthogonal transformation](#orthogonal-transformation) of $v^\perp$, so induction proves the bound. Each reflection has [determinant](#determinant) minus one, hence orientation-preserving transformations use an [even number](number-theory.md#even-number) of reflections.

### Determinant-twist projection in odd dimension

↑ **Parent:** [Orthogonal group](#orthogonal-group)

For real [orthogonal matrices](#orthogonal-matrix) in odd dimension $d$, multiplying by their [determinant](#determinant) defines a [group homomorphism](group-theory.md#group-homomorphism) from $O(d)$ onto $SO(d)$. Scalar factors commute, so $\pi(AB)=\pi(A)\pi(B)$, while $\det\pi(A)=(\det A)^{d+1}=1$. The map fixes $SO(d)$ and has [kernel](#kernel-of-a-linear-map) $\{I,-I\}$. Since $-I$ is central and has determinant $-1$ in odd dimension, $O(d)\cong SO(d)\times C_2$. In even dimension the same expression does not map every orthogonal matrix into the [special orthogonal group](#special-orthogonal-group).

### Odd-dimensional orthogonal determinant splitting

↑ **Parent:** [Orthogonal group](#orthogonal-group)

In odd dimension, the map $A\mapsto(\det A)A$ is a surjective [group homomorphism](group-theory.md#group-homomorphism) from the [orthogonal group](#orthogonal-group) to the [special orthogonal group](#special-orthogonal-group), with [kernel of a group homomorphism](group-theory.md#kernel-of-a-group-homomorphism) $\{I,-I\}$. Scalar matrices commute, and $\det[(\det A)A]=(\det A)^{2m+2}=1$. Together with the [determinant](#determinant) sign, it identifies $O(2m+1)$ with the [direct product of groups](group-theory.md#direct-product-of-groups) $SO(2m+1)\times C_2$. In even dimension, scalar multiplication by $\det A$ does not repair the determinant, so this construction does not give the same splitting.

### Orthogonal matrix

↑ **Parent:** [Orthogonal group](#orthogonal-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orthogonal_matrix)

A real square matrix is orthogonal when $R^TR=I$, equivalently when its columns form an orthonormal basis.

#### Orthogonal transformation

↑ **Parent:** [Orthogonal matrix](#orthogonal-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orthogonal_transformation)

An orthogonal transformation of a real inner-product space is a linear map $Q$ satisfying $Q^TQ=I$. It preserves inner products, lengths, angles, and therefore [Gaussian curvature](second-fundamental-form.md#gaussian-curvature) when applied to an embedded surface in Euclidean space.

### Improper orthogonal transformation

↑ **Parent:** [Orthogonal group](#orthogonal-group)

An improper orthogonal transformation has determinant $-1$. In three dimensions it may be a plane reflection or a rotation composed with a reflection perpendicular to the rotation axis.

#### Three-dimensional improper orthogonal transformation

↑ **Parent:** [Improper orthogonal transformation](#improper-orthogonal-transformation)

A real [orthogonal matrix](#orthogonal-matrix) $T$ of size three with $\det T=-1$ has an [eigenvector](linear-operator-theory.md#eigenvector) $n$ of [eigenvalue](linear-operator-theory.md#eigenvalue) $-1$. Its [orthogonal complement](hilbert-space.md#orthogonal-complement) is invariant, and the restriction there is an orientation-preserving plane rotation. Thus $T$ is a rotation about the axis $\mathbb Rn$ composed with a [reflection](#reflection-mathematics) across the plane perpendicular to $n$. Writing the plane angle as $\phi$, $\operatorname{tr}T=-1+2\cos\phi$. A pure plane [reflection](#reflection-mathematics) is the case $\phi=0$; if $\det(T-I)\ne0$, it cannot be a pure plane [reflection](#reflection-mathematics).

### Special orthogonal group

↑ **Parent:** [Orthogonal group](#orthogonal-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Special_orthogonal_group)

The special orthogonal group is

$$
SO(n)=\{A\in M_n(\mathbb R):A^TA=I,\ \det A=1\}.
$$

Every element of $SO(2)$ is a rotation in the plane. Every element of $SO(3)$ fixes an axis and restricts to a planar rotation on its perpendicular plane.

#### Trace height on the special orthogonal group

↑ **Parent:** [Special orthogonal group](#special-orthogonal-group)

For positive distinct diagonal entries $c_1<\cdots<c_n$, the [critical points](analysis.md#critical-point) of this function are diagonal sign [matrices](vector-space.md#matrix) $D=\operatorname{diag}(\varepsilon_1,\ldots,\varepsilon_n)$ with $\prod\varepsilon_i=1$. Criticality forces $CX$ symmetric; its square is $C^2$, so it commutes with the distinct-spectrum diagonal [matrix](vector-space.md#matrix) $C^2$ and is diagonal. In the skew coordinates $a_{ij}$ its [Hessian](calculus.md#hessian-matrix) is $-\sum_{i<j}(c_i\varepsilon_i+c_j\varepsilon_j)a_{ij}^2$. The sign of each parenthesis is that of $\varepsilon_j$, giving [Morse index](differential-geometry.md#morse-index) $\sum_{j:\varepsilon_j=1}(j-1)$.

#### Low homotopy groups of special orthogonal groups

↑ **Parent:** [Special orthogonal group](#special-orthogonal-group)

All the [special orthogonal groups](#special-orthogonal-group) are connected, and their second [homotopy groups](algebraic-topology.md#homotopy-group) vanish. The rotation circle gives $SO(2)\cong S^1$. Conjugation by [unit quaternions](algebra.md#unit-quaternion) gives the twofold [universal cover](algebraic-topology.md#universal-cover) $S^3\to SO(3)$, so $\pi_1SO(3)=\mathbb Z/2$ and $\pi_3SO(3)=\mathbb Z$. The [special orthogonal sphere fibration](#special-orthogonal-sphere-fibration) $SO(n-1)\to SO(n)\to S^{n-1}$ propagates the first two [homotopy groups](algebraic-topology.md#homotopy-group) for $n\geq4$. In dimension four its [exact sequence](homology.md#exact-sequence) has a zero map from the [torsion group](group-theory.md#torsion-group) $\pi_4S^3=\mathbb Z/2$ to $\pi_3SO(3)=\mathbb Z$, giving $\pi_3SO(4)=\mathbb Z^2$. For $SO(1)$ all positive groups vanish, and $\pi_3SO(2)=0$.

#### Special orthogonal sphere fibration

↑ **Parent:** [Special orthogonal group](#special-orthogonal-group)

The last-column map $p(A)=Ae_{s+1}$ has fiber $SO(s)$, included as $\operatorname{diag}(B,1)$. Local completion of a unit vector by the [Gram-Schmidt process](#gram-schmidt-process) gives local [fiber bundle](fiber-bundle.md) charts. Consequently it has the [homotopy lifting property](algebraic-topology.md#homotopy-lifting-property) and the [long exact sequence of homotopy groups of a fibration](algebraic-topology.md#long-exact-sequence-of-homotopy-groups-of-a-fibration).

##### Surjectivity of special orthogonal stabilization below the sphere dimension

↑ **Parent:** [Special orthogonal sphere fibration](#special-orthogonal-sphere-fibration)

Project a based map $\alpha:S^r\to SO(s+1)$ to $S^s$. Since $r<s$, the resulting [homotopy class](algebraic-topology.md#homotopy-class) vanishes. Lift a based null-homotopy by the [special orthogonal sphere fibration](#special-orthogonal-sphere-fibration). Its endpoint lies in the fiber $SO(s)$. If the lift moves its base point, right-multiply at time $t$ by the inverse of its base-point value, which lies in the fiber. This keeps the projected homotopy unchanged and makes the lift based. Thus $\alpha$ is based-homotopic to a map into $SO(s)$, proving the asserted surjectivity.

<h4 id="so-4-group">SO(4) group</h4>

↑ **Parent:** [Special orthogonal group](#special-orthogonal-group)

The [SO(4) group](#so-4-group) consists of real orthogonal four-by-four matrices of determinant one. It preserves orientation and the Euclidean metric. Its [Spin(4) double cover](semisimple-lie-algebra.md#spin-4-double-cover) identifies it with the quotient of two copies of [SU(2)](topological-group.md#su-2-group) by their simultaneous central sign.

<h5 id="representations-of-so-4-from-two-su2-spins">Representations of SO(4) from two SU2 spins</h5>

↑ **Parent:** [SO(4) group](#so-4-group)

Tensor products $V_{j_L}\otimes V_{j_R}$ give the [irreducible representations](representation-theory.md#irreducible-representation) of the [Spin(4) double cover](semisimple-lie-algebra.md#spin-4-double-cover). The simultaneous central sign acts by $(-1)^{2j_L+2j_R}$, so exactly the integer-sum pairs descend to [SO(4)](#so-4-group). Their dimensions are $(2j_L+1)(2j_R+1)$. Under the diagonal spatial rotation subgroup, the [Clebsch-Gordan decomposition for SU2](representation-theory.md#clebsch-gordan-decomposition-for-su2) gives spins from $|j_L-j_R|$ through $j_L+j_R$ in steps of one.

#### Rotations preserving an axis

↑ **Parent:** [Special orthogonal group](#special-orthogonal-group)

The subgroup of three-dimensional proper rotations preserving a chosen unoriented axis consists of all rotations about it and all half-turns about perpendicular axes. It is isomorphic to $O(2)$; the continuous molecular point-group notation is $D_\infty$. This uncountable group is different from the abstract countable infinite dihedral group $\mathbb Z\rtimes C_2$.

<h4 id="so-3-group">SO(3) group</h4>

↑ **Parent:** [Special orthogonal group](#special-orthogonal-group)

The SO(3) group consists of real three-by-three [orthogonal matrices](#orthogonal-matrix) with [determinant](#determinant) one. It acts by [rotation in three dimensions](#rotation-in-three-dimensions). Its [group manifold](lie-theory.md#group-manifold) is $\mathbb{RP}^3$, since the [Adjoint double cover from SU(2) to SO(3)](lie-theory.md#adjoint-double-cover-from-su-2-to-so-3) identifies antipodal points of the [three-sphere](geometry-and-topology.md#three-sphere).

<h5 id="so-3-as-real-projective-three-space">SO(3) as real projective three-space</h5>

↑ **Parent:** [SO(3) group](#so-3-group)

The [Adjoint double cover from SU(2) to SO(3)](lie-theory.md#adjoint-double-cover-from-su-2-to-so-3) has kernel $\{I,-I\}$. Under [SU(2) as the three-sphere](topological-group.md#su-2-as-the-three-sphere), multiplication by $-I$ is the antipodal map, so the quotient is [Real projective space](algebraic-topology.md#real-projective-space) $\mathbb{RP}^3$. Equivalently, an axis-angle ball of radius $\pi$ has opposite boundary points identified. The [fundamental group](algebraic-topology.md#fundamental-group) is $\mathbb Z_2$.

#### Odd-dimensional special orthogonal transformation has a fixed vector

↑ **Parent:** [Special orthogonal group](#special-orthogonal-group)

Every real orthogonal transformation of odd dimension with determinant one has eigenvalue $+1$. Nonreal eigenvalues come in conjugate pairs with product one, while real eigenvalues are $+1$ or $-1$. There are an odd number of real eigenvalues and an even number of negative ones, leaving at least one positive eigenvalue. The corresponding eigenvector is fixed.

#### Special orthogonal group as a submanifold

↑ **Parent:** [Special orthogonal group](#special-orthogonal-group)

The map $A\mapsto A^TA$ from real matrices to symmetric matrices has derivative $H\mapsto R^TH+H^TR$ at $R\in O(n)$, which is surjective. Thus $SO(n)$ is a submanifold of dimension $n(n-1)/2$, and

$$
T_RSO(n)=\{H:R^TH+H^TR=0\}
=\{RA:A^T=-A\}.
$$

#### Unit-vector stabilizer in a special orthogonal group

↑ **Parent:** [Special orthogonal group](#special-orthogonal-group)

For $v\in S^n$, the stabilizer $S_v=\{R\in SO(n+1):Rv=v\}$ is conjugate to the block subgroup $SO(n)$ acting on $v^\perp$. Hence it is a submanifold of dimension $n(n-1)/2$, with

$$
T_RS_v=\{RA:A^T=-A,\ Av=0\}.
$$

##### Distinct unit-vector stabilizers are not transverse

↑ **Parent:** [Unit-vector stabilizer in a special orthogonal group](#unit-vector-stabilizer-in-a-special-orthogonal-group)

For distinct $v,w\in S^n$, the submanifolds $S_v,S_w\subseteq SO(n+1)$ are not transverse. They both contain the identity. If $v,w$ are independent, the bivector $v\wedge w$ is a nonzero normal direction common to both tangent spaces there; if $w=-v$, the two stabilizers coincide.

#### Rotation in three dimensions

↑ **Parent:** [Special orthogonal group](#special-orthogonal-group)

A rotation in three dimensions is an element of $SO(3)$. It fixes an axis and acts as a two-dimensional rotation on the plane perpendicular to that axis.

### Skew-symmetric matrix

↑ **Parent:** [Orthogonal group](#orthogonal-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Skew-symmetric_matrix)

A matrix is skew-symmetric when $A^T=-A$.

#### Unitary skew-diagonalization of an antisymmetric matrix

↑ **Parent:** [Skew-symmetric matrix](#skew-symmetric-matrix)

A complex [matrix](vector-space.md#matrix) $Z=-Z^T$ can be put by unitary congruence into two-by-two skew blocks and zero blocks; the magnitudes $|z_r|$ are its [singular values](#singular-value), each repeated twice. One proof uses the [antilinear map](vector-space.md#antilinear-map) $A(v)=Z\bar v$. Because $Z^\dagger=-\bar Z$, $A^2=-ZZ^\dagger$. On a nonzero eigenspace of $ZZ^\dagger$ with [eigenvalue](linear-operator-theory.md#eigenvalue) $s^2$, any unit vector $v$ has orthogonal partner $A(v)/s$, and $A(A(v)/s)=-sv$. These orthonormal pairs give the blocks; the orthogonal complement is invariant, so the procedure repeats. Phases of the paired vectors set the block phases.

#### Cross-product matrix

↑ **Parent:** [Skew-symmetric matrix](#skew-symmetric-matrix)

For $a=(a_1,a_2,a_3)^T$, the map $b\mapsto a\times b$ has matrix

$$
[a]_\times=
\begin{pmatrix}
0&-a_3&a_2\\
a_3&0&-a_1\\
-a_2&a_1&0
\end{pmatrix}.
$$

It has trace zero and annihilates $a$, so its determinant is zero.

##### Cross-product matrix spectrum

↑ **Parent:** [Cross-product matrix](#cross-product-matrix)

The [cross-product matrix](#cross-product-matrix) $A\mathbf x=\mathbf n\times\mathbf x$ obeys $A\mathbf n=0$ and $A^2=\mathbf n\mathbf n^T-|\mathbf n|^2I$, by the [vector triple product](calculus.md#vector-triple-product). On the [orthogonal complement](hilbert-space.md#orthogonal-complement) of a nonzero $\mathbf n$, this is $-|\mathbf n|^2I$; hence the two remaining complex [eigenvalues](linear-operator-theory.md#eigenvalue) are $\pm i|\mathbf n|$. In an orthonormal basis adapted to $\mathbf n$, $A$ is a planar quarter-turn multiplied by $|\mathbf n|$, with zero action along its axis.

## Tensor product of linear maps

↑ **Parent:** [Linear algebra](linear-algebra.md)

The [tensor product](#tensor-product) of linear maps is determined by $(A\otimes B)(x\otimes y)=Ax\otimes By$ and linear extension.

### Tensor-product operator

↑ **Parent:** [Tensor product of linear maps](#tensor-product-of-linear-maps)

A tensor-product operator factors as $A\otimes B$ on a [tensor product](#tensor-product) of two spaces. If both factors are [positive semidefinite operators](hilbert-space.md#positive-operator), their tensor-product operator is positive: a [tensor-product basis](#tensor-product-basis) of eigenvectors has eigenvalues $a_ib_j\geq0$. This positivity underlies the necessary direction of the [positive partial transpose criterion](quantum-information-theory.md#positive-partial-transpose-criterion).

## Trace-duality bound

↑ **Parent:** [Linear algebra](linear-algebra.md)

For $M\succeq0$ with $\operatorname{tr}M\leq s$, $\operatorname{tr}(MA)\leq s\max(\lambda_{\max}(A),0)\leq s\lVert A\rVert_{\rm op}$.

## Diagonal matrix

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diagonal_matrix)

A diagonal matrix has zero entries away from its main diagonal. Its eigenvalues are its diagonal entries.

### Scalar matrix

↑ **Parent:** [Diagonal matrix](#diagonal-matrix)

A [scalar matrix](#scalar-matrix) is a scalar multiple of the identity [matrix](vector-space.md#matrix), equivalently a [diagonal matrix](#diagonal-matrix) with all diagonal entries equal. It commutes with every square [matrix](vector-space.md#matrix) of the same size. In $GL_n(F)$, the nonzero [scalar matrices](#scalar-matrix) form the central [subgroup](group.md#subgroup) removed to define the [projective linear group](group-theory.md#projective-linear-group).

## Triangular matrix

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Triangular_matrix)

An upper or lower triangular matrix has all entries on one side of the main diagonal equal to zero. Its eigenvalues, with algebraic multiplicity, are its diagonal entries.

### Back substitution

↑ **Parent:** [Triangular matrix](#triangular-matrix)

An upper [triangular matrix](#triangular-matrix) system with nonzero diagonal is solved from the last row upward. Once $x_{i+1},\ldots,x_n$ are known, use $x_i=(b_i-\sum_{j>i}a_{ij}x_j)/a_{ii}$. The nonzero diagonal guarantees a unique solution; this is the final solve after a [QR factorization](#qr-decomposition).

### Upper triangular matrix

↑ **Parent:** [Triangular matrix](#triangular-matrix)

An upper triangular matrix has zero entries below its main diagonal. Its [determinant](#determinant) is the product of its diagonal entries, and an invertible upper triangular linear system is solved by backward substitution.

#### Strictly upper triangular matrix

↑ **Parent:** [Upper triangular matrix](#upper-triangular-matrix)

A [square matrix](vector-space.md#square-matrix) is strictly upper triangular if every entry on or below its diagonal is zero. A product of $n$ such $n$-by-$n$ matrices vanishes, so they form a [nilpotent Lie algebra](lie-algebra.md#nilpotent-lie-algebra) under the [commutator](lie-algebra.md#commutator). Multiplication by an [upper triangular matrix](#upper-triangular-matrix) preserves strict upper triangularity and zero [trace](#matrix-trace).

### Lower triangular matrix

↑ **Parent:** [Triangular matrix](#triangular-matrix)

A lower triangular matrix has zero entries above its main diagonal. Its [determinant](#determinant) is the product of its diagonal entries, and an invertible lower triangular linear system is solved by forward substitution.

#### Lower triangular matrix algebra

↑ **Parent:** [Lower triangular matrix](#lower-triangular-matrix)

The algebra $T_n(k)$ consists of the lower triangular $n$ by $n$ matrices over $k$. Its [Jacobson radical](noncommutative-algebra.md#jacobson-radical) $N$ consists of the strictly lower triangular matrices, and

$$
N^i=\operatorname{span}\{e_{rs}:r-s\geq i\}.
$$

The $n$ simple left modules $S_r$ are one-dimensional, with a matrix acting through its $r$th diagonal entry. For the left regular module,

$$
N^i/N^{i+1}\cong S_{i+1}\oplus\cdots\oplus S_n.
$$

### Triangular linear system

↑ **Parent:** [Triangular matrix](#triangular-matrix)

A triangular linear system is solved by forward substitution for a lower triangular coefficient matrix or backward substitution for an upper triangular coefficient matrix, using $O(n^2)$ operations for a dense $n$ by $n$ matrix.

#### Forward substitution in a triangular system

↑ **Parent:** [Triangular linear system](#triangular-linear-system)

Forward substitution solves a lower-triangular system from its first row downward, substituting each newly determined variable into the rows below.

#### Backward substitution in a triangular system

↑ **Parent:** [Triangular linear system](#triangular-linear-system)

Backward substitution solves an upper-triangular system from its last row upward.

## Axis-angle representation

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axis–angle_representation)

An [axis-angle representation](#axis-angle-representation) specifies a rotation of three-dimensional Euclidean space by an oriented unit axis and an angle. The axis is fixed, and the perpendicular plane undergoes a pure [rotation](riemannian-geometry.md#rotation-mathematics), with no dilation.

## ↑ Ancestors (4)

1. [Algebra](algebra.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-12.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-9.md#2/solution)
- [Self-orthogonal binary subspace](coding-theory.md#self-orthogonal-binary-subspace)
