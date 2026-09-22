# Vector space

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vector_space)

A vector space consists of [vectors](#vector) that may be added and multiplied by [scalars](#scalar), subject to the vector-space axioms.

**Table of contents**

- [Sequence space](#sequence-space)
- [Zero vector](#zero-vector)
- [Vector space over the rational numbers](#vector-space-over-the-rational-numbers)
- [Antilinear map](#antilinear-map)
  - [Quaternionic structure on a complex vector space](#quaternionic-structure-on-a-complex-vector-space)
  - [Antiunitary operator](#antiunitary-operator)
- [Complex vector space](#complex-vector-space)
- [Real vector space](#real-vector-space)
  - [Majorization](#majorization)
    - [Majorization of summable sequences](#majorization-of-summable-sequences)
      - [Doubly stochastic realization of summable-sequence majorization](#doubly-stochastic-realization-of-summable-sequence-majorization)
- [Vector space over a finite field](#vector-space-over-a-finite-field)
  - [Finite-field Kakeya set](#finite-field-kakeya-set)
    - [Tangent-line finite-field Kakeya construction](#tangent-line-finite-field-kakeya-construction)
    - [Finite-field Kakeya polynomial bound](#finite-field-kakeya-polynomial-bound)
- [Linear span](#linear-span)
  - [Spanning set](#spanning-set)
- [Quotient vector space](#quotient-vector-space)
  - [Parallel lines as a quotient vector space](#parallel-lines-as-a-quotient-vector-space)
- [Vector subspace](#vector-subspace)
  - [Proper vector subspace](#proper-vector-subspace)
  - [Flag (linear algebra)](#flag-linear-algebra)
    - [Complete flag](#complete-flag)
  - [Fixed coordinate subspace](#fixed-coordinate-subspace)
  - [Intersection of vector subspaces](#intersection-of-vector-subspaces)
  - [Sum of vector subspaces](#sum-of-vector-subspaces)
  - [Hyperplane](#hyperplane)
  - [Closed vector subspace](#closed-vector-subspace)
    - [Positive distance between a unit sphere and a disjoint finite-dimensional subspace](#positive-distance-between-a-unit-sphere-and-a-disjoint-finite-dimensional-subspace)
- [Affine subspace](#affine-subspace)
  - [Affine hull](#affine-hull)
  - [Affine hyperplane](#affine-hyperplane)
  - [Affine line in a vector space](#affine-line-in-a-vector-space)
- [Linear combination](#linear-combination)
  - [Coefficient](#coefficient)
- [Scalar multiplication](#scalar-multiplication)
  - [Scalar multiple](#scalar-multiple)
- [Dimension (vector space)](#dimension-vector-space)
  - [Finite-dimensional vector space](#finite-dimensional-vector-space)
  - [Infinite-dimensional vector space](#infinite-dimensional-vector-space)
- [Direct sum](#direct-sum)
  - [Common plane for three pairwise complementary subspaces](#common-plane-for-three-pairwise-complementary-subspaces)
  - [Orthogonal direct sum](#orthogonal-direct-sum)
  - [Direct summand](#direct-summand)
    - [Unimodular basis test for an integer direct summand](#unimodular-basis-test-for-an-integer-direct-summand)
  - [Dimension formula for a sum of subspaces](#dimension-formula-for-a-sum-of-subspaces)
  - [Direct-sum complement](#direct-sum-complement)
- [Linear independence](#linear-independence)
  - [Minimally dependent vector family](#minimally-dependent-vector-family)
    - [Distinct diagonal weights break a first column dependence](#distinct-diagonal-weights-break-a-first-column-dependence)
  - [Linear dependence](#linear-dependence)
    - [Linear relation](#linear-relation)
- [Basis](#basis)
  - [Basis vector](#basis-vector)
  - [Adjacent sums of a cyclic basis](#adjacent-sums-of-a-cyclic-basis)
  - [Basis extension](#basis-extension)
  - [Standard basis](#standard-basis)
  - [Steinitz exchange lemma](#steinitz-exchange-lemma)
  - [Monomial basis](#monomial-basis)
- [Vector](#vector)
  - [Pseudovector](#pseudovector)
  - [Polar vector](#polar-vector)
  - [Euclidean vector](#euclidean-vector)
  - [Unit vector](#unit-vector)
  - [Cross product](#cross-product)
- [Scalar](#scalar)
- [Linear map](#linear-map)
  - [Zero-composition subspaces of a linear map](#zero-composition-subspaces-of-a-linear-map)
  - [One-sided inverses of finite-dimensional endomorphisms](#one-sided-inverses-of-finite-dimensional-endomorphisms)
  - [Rank of a linear map](#rank-of-a-linear-map)
    - [Rank bounds for a sum of linear maps](#rank-bounds-for-a-sum-of-linear-maps)
  - [Transvection](#transvection)
    - [Transvection conjugacy over a finite field](#transvection-conjugacy-over-a-finite-field)
    - [Elementary transvection matrix](#elementary-transvection-matrix)
      - [Transvections generate the special linear group](#transvections-generate-the-special-linear-group)
  - [Shear mapping](#shear-mapping)
  - [Uniform dilation](#uniform-dilation)
  - [Complex-linear map](#complex-linear-map)
  - [Image of a linear map](#image-of-a-linear-map)
    - [Image obstruction by an annihilating functional](#image-obstruction-by-an-annihilating-functional)
  - [Surjective linear map](#surjective-linear-map)
  - [First isomorphism theorem for vector spaces](#first-isomorphism-theorem-for-vector-spaces)
  - [Linear isomorphism](#linear-isomorphism)
  - [Linear function](#linear-function)
    - [Affine function](#affine-function)
  - [Linearity](#linearity)
  - [Superposition principle](#superposition-principle)
  - [Linear operator](#linear-operator)
    - [Semisimple linear operator](#semisimple-linear-operator)
    - [Locally nilpotent operator](#locally-nilpotent-operator)
      - [Algebraic exponential of a locally nilpotent operator](#algebraic-exponential-of-a-locally-nilpotent-operator)
    - [Operator commutator](#operator-commutator)
    - [Multiplication operator](#multiplication-operator)
      - [Spectrum of a real multiplication operator](#spectrum-of-a-real-multiplication-operator)
    - [Projection (linear algebra)](#projection-linear-algebra)
      - [Kadec-Snobar projection bound](#kadec-snobar-projection-bound)
      - [Inner product adapted to an idempotent linear map](#inner-product-adapted-to-an-idempotent-linear-map)
      - [Similarity classification of idempotent linear maps](#similarity-classification-of-idempotent-linear-maps)
      - [Oblique projection](#oblique-projection)
        - [Finite-dimensional Hilbert sampling reconstruction](#finite-dimensional-hilbert-sampling-reconstruction)
    - [Operator domain](#operator-domain)
      - [Densely defined operator](#densely-defined-operator)
    - [Identity operator](#identity-operator)
    - [Composition operator](#composition-operator)
      - [Invariant functional of a composition operator](#invariant-functional-of-a-composition-operator)
    - [Unitary operator](#unitary-operator)
      - [Unitary equivalence](#unitary-equivalence)
      - [Eigenphase](#eigenphase)
      - [Unitary conjugation](#unitary-conjugation)
      - [Von Neumann mean ergodic theorem](#von-neumann-mean-ergodic-theorem)
        - [Orthogonal decomposition for unitary ergodic averages](#orthogonal-decomposition-for-unitary-ergodic-averages)
    - [Commuting operators](#commuting-operators)
      - [Commuting maps preserve eigenspaces](#commuting-maps-preserve-eigenspaces)
    - [Anticommutator](#anticommutator)
      - [Two-by-two anticommutator characteristic polynomial](#two-by-two-anticommutator-characteristic-polynomial)
    - [Conjugate linear operators](#conjugate-linear-operators)
      - [Conjugation operator on an endomorphism space](#conjugation-operator-on-an-endomorphism-space)
  - [Matrix](#matrix)
    - [Cauchy matrix](#cauchy-matrix)
    - [Matrix norm](#matrix-norm)
    - [Matrix pencil](#matrix-pencil)
    - [Total nonnegativity of a matrix](#total-nonnegativity-of-a-matrix)
      - [Checkerboard inverse of a totally nonnegative matrix](#checkerboard-inverse-of-a-totally-nonnegative-matrix)
    - [Elementary column operation](#elementary-column-operation)
    - [Hadamard matrix](#hadamard-matrix)
    - [Square matrix](#square-matrix)
    - [Realification of a complex matrix](#realification-of-a-complex-matrix)
      - [Realification determinant identity](#realification-determinant-identity)
    - [Entrywise matrix L1 norm](#entrywise-matrix-l1-norm)
    - [Entrywise matrix function](#entrywise-matrix-function)
    - [Hadamard product](#hadamard-product)
      - [Hadamard power](#hadamard-power)
    - [Hermite normal form](#hermite-normal-form)
      - [Row lattice of an integer matrix](#row-lattice-of-an-integer-matrix)
      - [Row Hermite normal form in rank two](#row-hermite-normal-form-in-rank-two)
    - [Doubly stochastic matrix](#doubly-stochastic-matrix)
      - [Two-coordinate stochastic averaging](#two-coordinate-stochastic-averaging)
      - [Birkhoff-von Neumann theorem](#birkhoff-von-neumann-theorem)
        - [Birkhoff decomposition by support matchings](#birkhoff-decomposition-by-support-matchings)
        - [Alternating-cycle perturbation of a doubly stochastic matrix](#alternating-cycle-perturbation-of-a-doubly-stochastic-matrix)
    - [Rational matrix](#rational-matrix)
    - [Nonnegative matrix](#nonnegative-matrix)
      - [Irreducible nonnegative matrix](#irreducible-nonnegative-matrix)
        - [Primitive nonnegative matrix](#primitive-nonnegative-matrix)
      - [Perron–Frobenius theorem](#perron-frobenius-theorem)
    - [All-ones matrix](#all-ones-matrix)
    - [Row and column spaces](#row-and-column-spaces)
      - [Row space](#row-space)
      - [Column space](#column-space)
    - [Binary matrix](#binary-matrix)
    - [Submatrix](#submatrix)
      - [Minor (linear algebra)](#minor-linear-algebra)
        - [Principal minor](#principal-minor)
    - [Entrywise maximum norm](#entrywise-maximum-norm)
    - [Tridiagonal matrix](#tridiagonal-matrix)
    - [Block matrix](#block-matrix)
      - [Block diagonal matrix](#block-diagonal-matrix)
      - [Block tridiagonal matrix](#block-tridiagonal-matrix)
    - [Diagonally dominant matrix](#diagonally-dominant-matrix)
      - [Strictly diagonally dominant matrix](#strictly-diagonally-dominant-matrix)
        - [Inverse infinity-norm bound from diagonal dominance](#inverse-infinity-norm-bound-from-diagonal-dominance)
    - [Transpose](#transpose)
    - [Matrix logarithm](#matrix-logarithm)
      - [Analytic determinant square root for accretive symmetric matrices](#analytic-determinant-square-root-for-accretive-symmetric-matrices)
      - [Diagonal logarithm concavity bound](#diagonal-logarithm-concavity-bound)
      - [Existence of a logarithm for every invertible complex matrix](#existence-of-a-logarithm-for-every-invertible-complex-matrix)
      - [Klein's inequality](#klein-s-inequality)
    - [Matrix power](#matrix-power)
    - [Matrix element](#matrix-element)
    - [Sparse matrix](#sparse-matrix)
      - [Compressed sparse storage](#compressed-sparse-storage)
      - [Matrix bandwidth](#matrix-bandwidth)
    - [Matrix unit](#matrix-unit)
    - [Matrix rank](#matrix-rank)
      - [Rank bound for a matrix product](#rank-bound-for-a-matrix-product)
      - [Column rank](#column-rank)
      - [Row rank](#row-rank)
      - [Rank orbit of a matrix under left-right multiplication](#rank-orbit-of-a-matrix-under-left-right-multiplication)
      - [Subadditivity of matrix rank](#subadditivity-of-matrix-rank)
      - [Full column rank](#full-column-rank)
      - [Full row rank](#full-row-rank)
    - [Identity matrix](#identity-matrix)
    - [Rank-one matrix](#rank-one-matrix)
    - [Bidiagonal matrix](#bidiagonal-matrix)
      - [Upper bidiagonal matrix](#upper-bidiagonal-matrix)
    - [Matrix multiplication](#matrix-multiplication)
      - [Matrix product](#matrix-product)
      - [Outer product](#outer-product)
    - [Hessenberg matrix](#hessenberg-matrix)
      - [Upper Hessenberg matrix](#upper-hessenberg-matrix)
    - [Permutation matrix](#permutation-matrix)
      - [Signed permutation matrix](#signed-permutation-matrix)
    - [Matrix representation of a linear map](#matrix-representation-of-a-linear-map)
    - [Kronecker product](#kronecker-product)
      - [Kronecker sum](#kronecker-sum)

## Sequence space

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sequence_space)

A sequence space is a [vector space](vector-space.md) of scalar [sequences](real-analysis.md#sequence), closed under coordinatewise addition and scalar multiplication. Examples include the [l-p sequence space](banach-space.md#l-p-sequence-space), the [l-infinity sequence space](banach-space.md#l-infinity-sequence-space) and spaces of convergent sequences.

## Zero vector

↑ **Parent:** [Vector space](vector-space.md)

The [zero vector](#zero-vector) of a [vector space](vector-space.md) is its additive identity: $v+0=0+v=v$ for every [vector](#vector) $v$. It is unique, because if $0'$ is another such identity then $0=0+0'=0'$. Distributivity gives $\alpha0=\alpha(0+0)=\alpha0+\alpha0$, so $\alpha0=0$ after cancellation. In a coordinate [vector](#vector) space it has every coordinate zero.

## Vector space over the rational numbers

↑ **Parent:** [Vector space](vector-space.md)

A [vector space](vector-space.md) with scalar [field](algebra.md#field) $\mathbb Q$ is equivalently a [torsion-free divisible Abelian group](group.md#torsion-free-divisible-abelian-group). An embedding of such groups automatically respects rational scalar multiplication because solutions to $nb=ma$ are unique.

## Antilinear map

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antilinear_map)

For complex [vector spaces](vector-space.md), an antilinear map satisfies $A(\alpha u+\beta v)=\overline\alpha Au+\overline\beta Av$. It is linear over the [real numbers](arithmetic.md#real-number) and conjugates complex [scalar multiplication](#scalar-multiplication). This differs from two [conjugate linear operators](#conjugate-linear-operators), which are related by similarity rather than conjugate-linearity.

### Quaternionic structure on a complex vector space

↑ **Parent:** [Antilinear map](#antilinear-map)

An antilinear endomorphism $J$ with square $-1$ equips a [complex vector space](#complex-vector-space) with a quaternionic structure: complex multiplication supplies the quaternionic generator $i$ and $J$ supplies $j$, satisfying $Ji=-iJ$. Such a space has even complex dimension. There is no invariant complex line, because $Jv=cv$ would imply $-v=|c|^2v$. In dimension four the invariant complex two-planes are quaternionic lines, forming $\mathbb{HP}^1\cong S^4$. This is the [Euclidean reality structure on twistor space](general-relativity.md#euclidean-reality-structure-on-twistor-space) used in [twistor theory](general-relativity.md#twistor-theory).

### Antiunitary operator

↑ **Parent:** [Antilinear map](#antilinear-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antiunitary_operator)

An antiunitary operator between complex [Hilbert spaces](hilbert-space.md) is a surjective [antilinear map](#antilinear-map) satisfying the displayed [inner product](linear-algebra.md#inner-product) identity. It preserves [norms](functional-analysis.md#norm) but conjugates scalars. In a chosen [orthonormal basis](linear-algebra.md#orthonormal-basis) it is $UK$, with $U$ a [unitary operator](#unitary-operator) and $K$ coefficientwise [complex conjugation](complex-analysis.md#complex-conjugation). Conversely any such $UK$ is antiunitary. Antilinearity by itself does not preserve norms.

## Complex vector space

↑ **Parent:** [Vector space](vector-space.md)

A [vector space](vector-space.md) over the [field](algebra.md#field) of [complex numbers](complex-analysis.md#complex-number). A [complex-linear map](#complex-linear-map) preserves addition and multiplication by complex scalars.

## Real vector space

↑ **Parent:** [Vector space](vector-space.md)

A real vector space is a [vector space](vector-space.md) over the [field](algebra.md#field) $\mathbb R$ of [real numbers](arithmetic.md#real-number).

### Majorization

↑ **Parent:** [Real vector space](#real-vector-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Majorization)

For real vectors of equal length and equal sum, write $x\prec y$ when $\sum_{j=1}^k x_j^\downarrow\leq\sum_{j=1}^k y_j^\downarrow$ for every proper initial segment; the downward arrow means decreasing rearrangement. Majorization compares how unevenly a fixed total is distributed. The uniform probability vector is majorized by every probability vector, while $(1,0,\ldots,0)$ majorizes every probability vector. The order controls exact pure-state entanglement conversion in [Nielsen's pure-state conversion theorem](bell-state.md#nielsen-s-pure-state-conversion-theorem).

#### Majorization of summable sequences

↑ **Parent:** [Majorization](#majorization)

For decreasing positive sequences in $\ell^1$, write $x\prec y$ if every initial [partial sum](real-analysis.md#partial-sum) of $x$ is at most the corresponding [partial sum](real-analysis.md#partial-sum) of $y$ and the finite total sums agree. The finiteness requirement matters: equality of two divergent totals interpreted as infinity is too weak to guarantee a [doubly stochastic realization of summable-sequence majorization](#doubly-stochastic-realization-of-summable-sequence-majorization).

##### Doubly stochastic realization of summable-sequence majorization

↑ **Parent:** [Majorization of summable sequences](#majorization-of-summable-sequences)

Decreasing strictly positive [summable sequences](real-analysis.md#summable-sequence) with equal totals and $x\prec y$ admit an infinite [doubly stochastic matrix](#doubly-stochastic-matrix) realizing the displayed relation. Choose $k$ with $y_k\geq x_1>y_{k+1}$ and average the pair to obtain $x_1$ and $y_k+y_{k+1}-x_1$. The remaining decreasing sequence majorizes the remaining target sequence: short initial sums contain values at least $x_1$, and longer sums are the old sums minus $x_1$. Repeat on the tail, freezing one normalized finite-support row at each stage. Limit column sums are at most one; [Tonelli's theorem](measure-theory.md#tonelli-theorem), equal finite totals and strict positivity of every $y_j$ force every column sum to equal one.

## Vector space over a finite field

↑ **Parent:** [Vector space](vector-space.md)

If $\mathbb F_q$ is a finite field, a vector space of finite dimension $d$ over $\mathbb F_q$ has $q^d$ elements. Every infinite-dimensional vector space over $\mathbb F_p$ is an infinite elementary abelian $p$-group under addition.

### Finite-field Kakeya set

↑ **Parent:** [Vector space over a finite field](#vector-space-over-a-finite-field)

A subset of $\mathbb F_q^n$ is a finite-field Kakeya set when it contains an [affine line in a vector space](#affine-line-in-a-vector-space) in every one-dimensional direction. The line position may depend on the direction. The [polynomial method in combinatorics](combinatorics.md#polynomial-method-in-combinatorics) yields the [finite-field Kakeya polynomial bound](#finite-field-kakeya-polynomial-bound) on its [cardinality](set-theory.md#cardinality).

#### Tangent-line finite-field Kakeya construction

↑ **Parent:** [Finite-field Kakeya set](#finite-field-kakeya-set)

For odd characteristic, the union of the lines $y=mx-m^2/4$ contains a line of every finite slope. For fixed $x$, completing the square shows that it comprises the $(p+1)/2$ values of $y$ for which $x^2-y$ is a square, including zero. Adding the vertical line $x=0$ completes the directions and gives cardinality $(p^2+2p-1)/2=(1/2+o(1))p^2$. This is a [finite-field Kakeya set](#finite-field-kakeya-set) whose density tends to one half.

#### Finite-field Kakeya polynomial bound

↑ **Parent:** [Finite-field Kakeya set](#finite-field-kakeya-set)

For a [finite-field Kakeya set](#finite-field-kakeya-set) $A\subseteq\mathbb F_q^n$, a smaller [cardinality](set-theory.md#cardinality) would give a nonzero [polynomial](polynomial.md) of [total degree of a polynomial](polynomial.md#total-degree-of-a-polynomial) at most $q-1$ vanishing on $A$, by the [dimension of a bounded-total-degree polynomial space](polynomial.md#dimension-of-a-bounded-total-degree-polynomial-space). Its restriction to each complete [affine line in a vector space](#affine-line-in-a-vector-space) has $q$ [roots of a polynomial](polynomial.md#root-of-a-polynomial) and degree less than $q$, hence vanishes identically. The top [homogeneous polynomial](algebra.md#homogeneous-polynomial) part then vanishes in every direction. A [polynomial](polynomial.md) of degree less than $q$ in each variable cannot vanish everywhere on $\mathbb F_q^n$ unless it is zero, giving a contradiction. For the [prime field](algebra.md#prime-field), this is the [polynomial nonvanishing below the field size](combinatorics.md#polynomial-nonvanishing-below-the-field-size).

## Linear span

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_span)

The linear span of a subset $S$ of a [vector space](vector-space.md) is the set of all finite [linear combinations](#linear-combination) of elements of $S$.

### Spanning set

↑ **Parent:** [Linear span](#linear-span)

A subset $S$ of a [vector space](vector-space.md) is a spanning set when its [linear span](#linear-span) is the whole vector space.

## Quotient vector space

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quotient_vector_space)

For a [vector subspace](#vector-subspace) $W\leq V$, the quotient vector space $V/W$ consists of cosets $v+W$, with vector operations induced from $V$.

### Parallel lines as a quotient vector space

↑ **Parent:** [Quotient vector space](#quotient-vector-space)

For fixed $u\ne0$, the parallel [affine lines](ringed-space.md#affine-line) $l_x=x+\operatorname{span}(u)$ are precisely the cosets of the indicated [quotient vector space](#quotient-vector-space). Changing representatives adds a multiple of $u$, so $l_x+l_y=l_{x+y}$ and $a l_x=l_{ax}$ are well-defined. The zero is the whole line $l_0$, not a single point. If $(u,b_1,b_2)$ is a [basis](#basis), the two line classes $l_{b_1},l_{b_2}$ form a [basis](#basis) of the quotient by spanning and independence modulo $\operatorname{span}(u)$.

## Vector subspace

↑ **Parent:** [Vector space](vector-space.md)

A vector subspace is a subset closed under vector addition and scalar multiplication, and is therefore itself a [vector space](vector-space.md).

### Proper vector subspace

↑ **Parent:** [Vector subspace](#vector-subspace)

A proper [vector subspace](#vector-subspace) of a [vector space](vector-space.md) is one strictly smaller than the ambient space. In a finite-dimensional [vector space](vector-space.md), this is equivalent to having smaller [dimension](#dimension-vector-space): a [basis](#basis) of the subspace can be extended to a [basis](#basis) of the ambient space, and strict inclusion requires at least one additional [vector](#vector).

### Flag (linear algebra)

↑ **Parent:** [Vector subspace](#vector-subspace)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flag_(linear_algebra))

A flag is a strictly nested chain of [vector subspaces](#vector-subspace) of a fixed [vector space](vector-space.md). A [complete flag](#complete-flag) contains a subspace of every possible dimension. For an action by [linear maps](#linear-map), an invariant flag means that each of its [vector subspaces](#vector-subspace) is an [invariant subspace](representation-theory.md#invariant-subspace). A [basis](#basis) adapted to an invariant complete flag makes all these maps upper triangular, connecting [complete flags](#complete-flag) to [simultaneous triangularization of a Lie algebra representation](lie-algebra.md#simultaneous-triangularization-of-a-lie-algebra-representation).

#### Complete flag

↑ **Parent:** [Flag (linear algebra)](#flag-linear-algebra)

A complete flag in an $n$-dimensional [vector space](vector-space.md) is a nested sequence of [vector subspaces](#vector-subspace) with $\dim V_i=i$. An action preserves such a flag exactly when its [matrices](#matrix) are upper triangular in a [basis](#basis) adapted to the flag. The [Lie theorem](lie-algebra.md#lie-s-theorem) supplies an invariant complete flag for every complex finite-dimensional [Lie algebra representation](lie-algebra.md#lie-algebra-representation) of a [solvable Lie algebra](lie-algebra.md#solvable-lie-algebra).

### Fixed coordinate subspace

↑ **Parent:** [Vector subspace](#vector-subspace)

The [fixed coordinate subspace](#fixed-coordinate-subspace) of dimension $k$ in $\mathbb R^p$ consists of vectors whose coordinates after the first $k$ vanish. Restricting a [quadratic form](linear-algebra.md#quadratic-form) to it uses only the leading $k$ by $k$ matrix block. It specifies one fixed support; allowing every support of size $k$ would introduce another combinatorial counting step.

### Intersection of vector subspaces

↑ **Parent:** [Vector subspace](#vector-subspace)

The intersection of any family of [vector subspaces](#vector-subspace) of a common [vector space](vector-space.md) is the set of vectors belonging to every member of the family. It is again a vector subspace.

### Sum of vector subspaces

↑ **Parent:** [Vector subspace](#vector-subspace)

The sum of vector subspaces $U,W\leq V$ is

$$
U+W=\{u+w:u\in U,\ w\in W\}.
$$

It is the smallest [vector subspace](#vector-subspace) containing both $U$ and $W$.

### Hyperplane

↑ **Parent:** [Vector subspace](#vector-subspace)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperplane)

A hyperplane is a [vector subspace](#vector-subspace) of codimension one. A projective hyperplane in $\mathbb P^n$ is the zero set of one nonzero homogeneous linear form.

### Closed vector subspace

↑ **Parent:** [Vector subspace](#vector-subspace)

A closed vector subspace of a [topological vector space](topological-vector-space.md) is both a [vector subspace](#vector-subspace) and a [closed set](topology.md#closed-set). The kernel of a [continuous linear map](topological-vector-space.md#continuous-linear-operator) is a closed vector subspace.

#### Positive distance between a unit sphere and a disjoint finite-dimensional subspace

↑ **Parent:** [Closed vector subspace](#closed-vector-subspace)

If $E$ is a nonzero [closed linear subspace](#closed-vector-subspace) of a normed ambient space and $F$ is finite-dimensional with $E\cap F=\{0\}$, the unit sphere of $E$ has positive distance from $F$. Otherwise a sequence of nearly coincident points yields a bounded sequence in $F$, hence a convergent subsequence; closedness of $E$ puts its norm-one limit in both [vector subspaces](#vector-subspace). In applications to a [bidual space](linear-algebra.md#bidual-of-a-normed-space), completeness of the [Banach space](banach-space.md) makes its canonical image closed.

## Affine subspace

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affine_subspace)

An affine subspace of a [vector space](vector-space.md) is a translate $v+W$ of a [vector subspace](#vector-subspace) $W$. Its dimension is the [dimension](#dimension-vector-space) of $W$.

### Affine hull

↑ **Parent:** [Affine subspace](#affine-subspace)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affine_hull)

The smallest [affine subspace](#affine-subspace) containing a nonempty set $S$. For any chosen $a\in S$, the displayed formula proves existence and minimality: every containing affine subspace must contain all the indicated differences in its direction space. Equivalently it consists of finite affine combinations $\sum_i\lambda_i s_i$ with $\sum_i\lambda_i=1$. Its dimension can be smaller than the dimension of an affine hyperplane in which the set has been embedded.

### Affine hyperplane

↑ **Parent:** [Affine subspace](#affine-subspace)

In a finite-dimensional real vector space, a level set of a nonzero [linear functional](linear-algebra.md#linear-functional) is an affine hyperplane. Choosing $v_0$ in that level set gives $H=v_0+\ker\ell$, so its dimension is one less than that of the ambient space. With a Euclidean inner product, translation followed by an orthonormal basis of $\ker\ell$ identifies it isometrically with the lower-dimensional Euclidean space. The coordinate-sum constraint on balanced cut vectors is an example.

### Affine line in a vector space

↑ **Parent:** [Affine subspace](#affine-subspace)

In a [vector space](vector-space.md) over a [field](algebra.md#field) $k$, an affine line is a translate of a one-dimensional [vector subspace](#vector-subspace). Its direction is that [vector subspace](#vector-subspace), so multiplying $v$ by a nonzero scalar preserves the direction. Over a [finite field](algebra.md#finite-field) of size $q$ it contains exactly $q$ distinct points. This usage concerns affine subsets of vector spaces, rather than the [affine line](ringed-space.md#affine-line) as an [affine scheme](ringed-space.md#affine-scheme).

## Linear combination

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_combination)

A linear combination of vectors $v_1,\ldots,v_n$ is a sum $a_1v_1+\cdots+a_nv_n$ with scalar coefficients $a_i$.

### Coefficient

↑ **Parent:** [Linear combination](#linear-combination)

A [scalar](#scalar) multiplying a specified term in a [linear combination](#linear-combination), [polynomial](polynomial.md) or [power series](real-analysis.md#power-series). When the term family has [linear independence](#linear-independence), the [coefficients](#coefficient) are unique; uniqueness of finite [Laurent polynomial](polynomial.md#laurent-polynomial) [coefficients](#coefficient) follows after multiplying by a sufficiently large power to obtain an ordinary [polynomial](polynomial.md).

## Scalar multiplication

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scalar_multiplication)

Scalar multiplication is the [vector space](vector-space.md) operation $(a,v)\mapsto av$ taking a scalar and a vector to a vector.

### Scalar multiple

↑ **Parent:** [Scalar multiplication](#scalar-multiplication)

A scalar multiple of a vector $v$ is a vector of the form $av$ for a scalar $a$.

## Dimension (vector space)

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dimension_(vector_space))

The dimension of a vector space is the cardinality of any of its [bases](#basis).

### Finite-dimensional vector space

↑ **Parent:** [Dimension (vector space)](#dimension-vector-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite-dimensional_vector_space)

A vector space is finite-dimensional when it has a [finite set](set.md#finite-set) as a [basis](#basis).

### Infinite-dimensional vector space

↑ **Parent:** [Dimension (vector space)](#dimension-vector-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Infinite-dimensional_vector_space)

An infinite-dimensional vector space has no finite [basis](#basis), so its [dimension](#dimension-vector-space) is an infinite cardinal.

## Direct sum

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Direct_sum)

The direct sum $U\oplus W$ of two [vector spaces](vector-space.md) consists of pairs $(u,w)$ with componentwise operations. A vector space is an internal direct sum of subspaces $U$ and $W$ exactly when every vector has a unique expression $u+w$ with $u\in U$ and $w\in W$.

### Common plane for three pairwise complementary subspaces

↑ **Parent:** [Direct sum](#direct-sum)

If $V=A_1\oplus A_2=A_2\oplus A_3=A_1\oplus A_3$ with nonzero subspaces, choose $0\ne v\in A_3$ and write $v=a_1+a_2$ using the first [direct sum of vector spaces](#direct-sum). Both components are nonzero. The plane spanned by them meets $A_1$ and $A_2$ in their component lines and meets $A_3$ in the line through $v$. Its intersection with $A_3$ cannot be the whole plane, since $a_1\notin A_3$.

### Orthogonal direct sum

↑ **Parent:** [Direct sum](#direct-sum)

An orthogonal direct sum is a [direct sum](#direct-sum) whose distinct summands are mutually [orthogonal](linear-algebra.md#orthogonal-vectors). For $v\in V$ and $w\in W$, the [Pythagorean identity](linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) gives $\|v+w\|^2=\|v\|^2+\|w\|^2$. In a [Hilbert space](hilbert-space.md), a [closed subspace of a Hilbert space](hilbert-space.md#closed-subspace-of-a-hilbert-space) and its [orthogonal complement](hilbert-space.md#orthogonal-complement) give an orthogonal direct sum of the entire space. The component maps are [orthogonal projections](hilbert-space.md#orthogonal-projection) and have [operator norm](continuous-dual-space.md#operator-norm) one when their ranges are nonzero.

### Direct summand

↑ **Parent:** [Direct sum](#direct-sum)

A [submodule](module-theory.md#submodule) $N$ of a [module](module-theory.md#module-mathematics) $M$ is a direct summand if some [submodule](module-theory.md#submodule) $L$ gives $M=N\oplus L$. Equivalently, the inclusion has a left inverse [R-module homomorphism](module-theory.md#module-homomorphism), or $N$ is the image of an [idempotent](commutative-algebra.md#idempotent) [endomorphism](algebra.md#endomorphism) of $M$.

#### Unimodular basis test for an integer direct summand

↑ **Parent:** [Direct summand](#direct-summand)

Integer row vectors forming a square [unimodular matrix](linear-algebra.md#unimodular-matrix) are a basis of the corresponding [free abelian group](group-theory.md#free-abelian-group): the adjugate formula makes the inverse integral. The subgroup spanned by any subset of that basis is therefore a [direct summand](#direct-summand), complemented by the remaining basis vectors. In contrast, a proper finite-index subgroup of a free abelian group cannot be a direct summand: its nonzero finite quotient would have to embed as a subgroup of a torsion-free group.

### Dimension formula for a sum of subspaces

↑ **Parent:** [Direct sum](#direct-sum)

For finite-dimensional subspaces $U,W$ of a common vector space,

$$
\dim(U+W)+\dim(U\cap W)=\dim U+\dim W.
$$

### Direct-sum complement

↑ **Parent:** [Direct sum](#direct-sum)

For every subspace $U$ of a finite-dimensional vector space $V$, extending a basis of $U$ to a basis of $V$ produces a subspace $W$ such that $V=U\oplus W$.

## Linear independence

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_independence)

Vectors $v_1,\ldots,v_n$ are linearly independent when

$$
a_1v_1+\cdots+a_nv_n=0
$$

implies $a_1=\cdots=a_n=0$.

### Minimally dependent vector family

↑ **Parent:** [Linear independence](#linear-independence)

A finite [vector](#vector) family is minimally dependent if it is [linearly dependent](#linear-dependence) and every proper subfamily is [linearly independent](#linear-independence). For $n\geq2$, the family $e_1,\ldots,e_{n-1},\sum_{j=1}^{n-1}e_j$ in $\mathbb R^n$ is an example. The sum supplies a nonzero dependence. If the sum [vector](#vector) is omitted, the remaining [vectors](#vector) are a coordinate basis; if $e_j$ is omitted, its coordinate in any proposed relation forces the coefficient of the sum [vector](#vector) to vanish, then all other coefficients vanish. Every smaller proper subfamily lies in one of these independent $(n-1)$-element subfamilies.

#### Distinct diagonal weights break a first column dependence

↑ **Parent:** [Minimally dependent vector family](#minimally-dependent-vector-family)

Let the first $k$ columns of a [matrix](#matrix) be the first dependent prefix, with no zero column. Their relation space has dimension one, and every nonzero relation $b$ has at least two nonzero coordinates. If both $Ab=0$ and $A\operatorname{diag}(\lambda_j)b=0$, one-dimensionality gives $\lambda_jb_j=cb_j$ for all $j$. Two nonzero coordinates would force two of the distinct weights $\lambda_j$ to agree, a contradiction.

### Linear dependence

↑ **Parent:** [Linear independence](#linear-independence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_dependence)

Vectors are linearly dependent when some nonzero choice of coefficients gives a vanishing linear combination.

#### Linear relation

↑ **Parent:** [Linear dependence](#linear-dependence)

A linear relation among [vectors](#vector) $v_1,\ldots,v_n$ is a coefficient tuple $(a_1,\ldots,a_n)$ satisfying $\sum_i a_iv_i=0$. It is nontrivial if at least one coefficient is nonzero. For the [matrix](#matrix) with these vectors as columns, the space of relations is its [kernel](linear-algebra.md#kernel-of-a-linear-map). The vectors are [linearly independent](#linear-independence) exactly when this kernel is zero. An invertible change of coordinates preserves every relation, since $S\sum_i a_iv_i=0$ if and only if $\sum_i a_iv_i=0$.

## Basis

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Basis_(linear_algebra))

A basis is a [linearly independent](#linear-independence) spanning family of [vectors](#vector) in a [vector space](vector-space.md).

### Basis vector

↑ **Parent:** [Basis](#basis)

A [basis vector](#basis-vector) is one of the [vectors](#vector) in a specified [basis](#basis) of a [vector space](vector-space.md). Its coordinate column in that [basis](#basis) has one entry equal to one and all other entries zero. Columns of a [matrix of a linear map](#matrix-representation-of-a-linear-map) are the images of domain [basis vectors](#basis-vector), expressed in the chosen codomain [basis](#basis).

### Adjacent sums of a cyclic basis

↑ **Parent:** [Basis](#basis)

For a [basis](#basis) $e_1,\ldots,e_n$ with cyclic indexing, the vectors $e_j+e_{j+1}$ have coefficient matrix $I+S$, where $S$ cyclically shifts coordinates. Its [determinant](linear-algebra.md#determinant) is $1-(-1)^n$. They therefore form a [basis](#basis) exactly when $n$ is odd over a field of characteristic different from two. For even $n$, alternating coefficients produce a nontrivial [linear dependence](#linear-dependence).

### Basis extension

↑ **Parent:** [Basis](#basis)

Every [linearly independent](#linear-independence) subset of a finite-dimensional [vector space](vector-space.md) extends to a [basis](#basis). Starting with its vectors, add a vector outside their current [span](#linear-span) until the span is the whole space. Each addition preserves [linear independence](#linear-independence), and the process stops because the dimension is finite. This also lets a [linear functional](linear-algebra.md#linear-functional) on a [vector subspace](#vector-subspace) extend to the ambient space by assigning arbitrary values on the additional basis vectors.

### Standard basis

↑ **Parent:** [Basis](#basis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Standard_basis)

The standard basis of the [vector space](vector-space.md) $\mathbb R^n$ consists of the [vectors](#vector) $e_i$ whose $i$th coordinate is one and whose other coordinates are zero. Every [vector](#vector) $x$ has the unique expression $x=\sum_i x_ie_i$ in this [basis](#basis).

### Steinitz exchange lemma

↑ **Parent:** [Basis](#basis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Steinitz_exchange_lemma)

If a [vector space](vector-space.md) is spanned by $n$ vectors, every [linearly independent](#linear-independence) family in it has at most $n$ members. Consequently, any two finite [bases](#basis) have the same number of vectors.

### Monomial basis

↑ **Parent:** [Basis](#basis)

For polynomials in fixed variables and of a fixed degree, the monomials of that degree form a basis of the corresponding homogeneous component.

## Vector

↑ **Parent:** [Vector space](vector-space.md)

A vector is an element of a [vector space](vector-space.md).

### Pseudovector

↑ **Parent:** [Vector](#vector)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pseudovector)

An axial vector transforms as $\mathbf a'=(\det Q)Q\mathbf a$ under an [orthogonal matrix](linear-algebra.md#orthogonal-matrix) $Q$. It agrees with a [polar vector](#polar-vector) under a proper [rotation matrix](linear-algebra.md#rotation-matrix) and has the additional determinant sign under an orientation-reversing transformation. [Angular momentum](classical-mechanics.md#angular-momentum) and [angular velocity](classical-mechanics.md#angular-velocity) are axial [vectors](#vector).

### Polar vector

↑ **Parent:** [Vector](#vector)

A polar [vector](#vector) transforms as $\mathbf v'=Q\mathbf v$ under an [orthogonal matrix](linear-algebra.md#orthogonal-matrix) $Q$, including an orientation-reversing transformation. Displacement, [velocity](classical-mechanics.md#velocity) and [force](classical-mechanics.md#force) are polar [vectors](#vector). An [axial vector](#pseudovector) instead transforms as $\mathbf a'=(\det Q)Q\mathbf a$.

### Euclidean vector

↑ **Parent:** [Vector](#vector)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclidean_vector)

A Euclidean vector is a vector in a finite-dimensional real inner-product space, represented in Cartesian coordinates by an ordered tuple of real components.

### Unit vector

↑ **Parent:** [Vector](#vector)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unit_vector)

A unit vector is a [vector](#vector) whose [norm](functional-analysis.md#norm) is one.

### Cross product

↑ **Parent:** [Vector](#vector)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cross_product)

The cross product $a\times b$ of two three-dimensional [vectors](#vector) is perpendicular to both, has magnitude $|a||b|\sin\theta$, and is oriented by the right-hand rule.

## Scalar

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scalar_(mathematics))

A scalar is an element of the field over which a [vector space](vector-space.md) is defined.

## Linear map

↑ **Parent:** [Vector space](vector-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_map)

A linear map preserves vector addition and scalar multiplication.

### Zero-composition subspaces of a linear map

↑ **Parent:** [Linear map](#linear-map)

For $\alpha:U\to V$, maps in $M^l(\alpha)$ factor uniquely through $V/\operatorname{im}\alpha$; maps in $M^r(\alpha)$ have [image](set-theory.md#image-of-a-function) in $\ker\alpha$. Thus these [vector subspaces](#vector-subspace) are naturally $L(V/\operatorname{im}\alpha,U)$ and $L(V,\ker\alpha)$, of dimensions $(\dim V-\operatorname{rank}\alpha)\dim U$ and $(\dim U-\operatorname{rank}\alpha)\dim V$. Passing to a [dual map](linear-algebra.md#transpose-of-a-linear-map) reverses composition and interchanges these two spaces. This gives a basis-free route to equality of the ranks of a map and its dual.

### One-sided inverses of finite-dimensional endomorphisms

↑ **Parent:** [Linear map](#linear-map)

For endomorphisms $S,T$ of the same finite-dimensional [vector space](vector-space.md), $ST=I$ makes $S$ surjective and $T$ injective. The [rank-nullity theorem](linear-algebra.md#rank-nullity-theorem) makes both invertible, hence $TS=I$. The finite-dimensional and equal-domain assumptions matter; unilateral shift operators on an infinite-dimensional sequence space give one-sided inverses that are not two-sided.

### Rank of a linear map

↑ **Parent:** [Linear map](#linear-map)

The rank of a [linear map](#linear-map) is the dimension of its [image of a linear map](#image-of-a-linear-map). In finite-dimensional spaces it equals the [rank of a matrix](#matrix-rank) representing the map in any bases.

#### Rank bounds for a sum of linear maps

↑ **Parent:** [Rank of a linear map](#rank-of-a-linear-map)

The image of $A+B$ lies in $\operatorname{im}A+\operatorname{im}B$. The [dimension formula for a sum of subspaces](#dimension-formula-for-a-sum-of-subspaces) gives the upper bound. Applying it to $A=(A+B)-B$ and then interchanging $A,B$ gives the lower bound. Both extremes are sharp: cancelling diagonal blocks gives the difference of ranks; diagonal maps with supports covering the whole space and positive coefficients give full rank when the sum of prescribed ranks is at least the dimension.

### Transvection

↑ **Parent:** [Linear map](#linear-map)

For a nonzero [vector](#vector) $v$ and nonzero [linear functional](linear-algebra.md#linear-functional) $f$ vanishing on $v$, this invertible map fixes the [hyperplane](#hyperplane) $\ker f$ pointwise and has determinant one. Its inverse is $I-vf$, since $(vf)^2=0$. A [symplectic transvection](finite-group-theory.md#symplectic-transvection) is obtained by taking $f=cB(-,v)$ for a nondegenerate [alternating bilinear form](linear-algebra.md#alternating-bilinear-form).

#### Transvection conjugacy over a finite field

↑ **Parent:** [Transvection](#transvection)

Every nonidentity [transvection](#transvection) has an adapted basis in which it is $I+E_{12}$. Thus all such maps are conjugate in the [general linear group](group-theory.md#general-linear-group). In dimension at least three, a scaling of a third basis vector centralizes this matrix and has arbitrary nonzero determinant; adjusting a conjugator by this scaling proves conjugacy in the [special linear group](group-theory.md#special-linear-group) as well.

// Target: algebra.bigb

#### Elementary transvection matrix

↑ **Parent:** [Transvection](#transvection)

This [matrix](#matrix) adds $t$ times coordinate $j$ to coordinate $i$. Left multiplication performs the corresponding row addition. Such matrices generate the [special linear group over a finite field](finite-group-theory.md#special-linear-group-over-a-finite-field): row elimination also realizes signed interchanges and compensating diagonal scalings using products of these matrices.

##### Transvections generate the special linear group

↑ **Parent:** [Elementary transvection matrix](#elementary-transvection-matrix)

Row additions reduce an invertible matrix to diagonal form without changing determinant. A determinant-one diagonal matrix is a product of diagonal two-coordinate blocks $\operatorname{diag}(a,a^{-1})$, each expressible as a product of six [elementary transvection matrices](#elementary-transvection-matrix). Therefore these matrices generate the [special linear group](group-theory.md#special-linear-group) over a field.

// Target: algebra.bigb

### Shear mapping

↑ **Parent:** [Linear map](#linear-map)

A horizontal shear fixes the horizontal axis pointwise and sends $(x,y)$ to $(x+ky,y)$. Its [determinant](linear-algebra.md#determinant) is one and both [eigenvalues](linear-operator-theory.md#eigenvalue) are one. A nonzero shear preserves area but generally changes lengths and angles. Composing a shear with a [planar rotation](linear-algebra.md#planar-rotation) can produce a symmetric stretch; having [determinant](linear-algebra.md#determinant) one alone does not make a [linear map](#linear-map) a shear.

### Uniform dilation

↑ **Parent:** [Linear map](#linear-map)

A uniform dilation about the origin multiplies every vector by one positive real scale $s$. The [linear map](#linear-map) $\mathbf x\mapsto s\mathbf x$ multiplies lengths by $s$ and $d$-dimensional volumes by $s^d$. This differs from stretching different axes by different factors. The case $s=1$ is the [identity map](function.md#identity-function).

### Complex-linear map

↑ **Parent:** [Linear map](#linear-map)

A real-linear map between [complex vector spaces](#complex-vector-space) that commutes with multiplication by $i$. On $\mathbb C$, its real matrix is $\begin{pmatrix}a&-b\\b&a\end{pmatrix}$, representing multiplication by $a+ib$. On $\mathbb C$, such a map with real [determinant](linear-algebra.md#determinant) one is a rotation. In higher complex dimension, determinant one does not force the map to be a [unitary operator](#unitary-operator).

### Image of a linear map

↑ **Parent:** [Linear map](#linear-map)

The [image](set-theory.md#image-and-preimage-of-a-function) of a linear map $T:V\to W$ is the [vector subspace](#vector-subspace) $\operatorname{im}T=\{T(v):v\in V\}$ of its codomain.

#### Image obstruction by an annihilating functional

↑ **Parent:** [Image of a linear map](#image-of-a-linear-map)

If a [linear functional](linear-algebra.md#linear-functional) $\ell$ vanishes on the [image of a linear map](#image-of-a-linear-map) $T$ but $\ell(b)\ne0$, the equation $Tx=b$ has no solution. In Euclidean coordinates, a vector $n$ with $n^TA=0$ provides such an obstruction whenever $n^Tb\ne0$. In finite dimensions these annihilating functionals exactly characterize membership in the image: $b\in\operatorname{im}A$ precisely when it is orthogonal to every vector in $\ker A^T$.

### Surjective linear map

↑ **Parent:** [Linear map](#linear-map)

A linear map $T:V\to W$ is surjective when its [image](set-theory.md#image-and-preimage-of-a-function) is all of $W$. For finite-dimensional spaces this is equivalent to $\operatorname{rank}T=\dim W$.

### First isomorphism theorem for vector spaces

↑ **Parent:** [Linear map](#linear-map)

For a linear map $T:V\to W$, the induced map

$$
V/\ker T\longrightarrow\operatorname{im}T,
\qquad
v+\ker T\longmapsto T(v),
$$

is a vector-space isomorphism.

### Linear isomorphism

↑ **Parent:** [Linear map](#linear-map)

A linear isomorphism is a [bijective](function.md#bijection) [linear map](#linear-map). Its inverse is also linear.

### Linear function

↑ **Parent:** [Linear map](#linear-map)

This is a scalar-valued [linear functional](linear-algebra.md#linear-functional), so it vanishes at the origin; an affine function with a nonzero constant term is a different notion.

A real linear function on $\mathbb R^n$ has the form $x\mapsto c^Tx$.

#### Affine function

↑ **Parent:** [Linear function](#linear-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affine_function)

An affine function on a real or complex [vector space](vector-space.md) has the form $x\mapsto Lx+b$, where $L$ is a [linear map](#linear-map) and $b$ is constant. Its derivative is the constant map $L$. It is linear exactly when $b=0$.

### Linearity

↑ **Parent:** [Linear map](#linear-map)

Linearity is the property $T(ax+by)=aT(x)+bT(y)$.

### Superposition principle

↑ **Parent:** [Linear map](#linear-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Superposition_principle)

For a homogeneous [linear](#linearity) equation, every linear combination of solutions is again a solution.

### Linear operator

↑ **Parent:** [Linear map](#linear-map)

A linear operator is a [linear map](#linear-map) from a [vector space](vector-space.md) to itself.

#### Semisimple linear operator

↑ **Parent:** [Linear operator](#linear-operator)

A [linear operator](#linear-operator) is semisimple if it becomes [diagonalizable](linear-operator-theory.md#diagonalizable-matrix) over an algebraic closure; equivalently, its [minimal polynomial](linear-operator-theory.md#minimal-polynomial) has no repeated root over that closure. If an invertible operator $A$ has finite order $r$ prime to the [characteristic of a field](algebra.md#characteristic-of-a-field), its [minimal polynomial](linear-operator-theory.md#minimal-polynomial) divides $X^r-1$. The derivative $rX^{r-1}$ is coprime to this polynomial, so $A$ is semisimple. Its invariant irreducible summands over a [finite field](algebra.md#finite-field) become multiplication by scalars in suitable [finite field extensions](algebra.md#finite-field-extension).

#### Locally nilpotent operator

↑ **Parent:** [Linear operator](#linear-operator)

A linear operator $T$ is locally nilpotent if for each vector $v$ there is an integer $m(v)$ such that $T^{m(v)}v=0$. In finite dimension this is equivalent to being a [nilpotent operator](linear-operator-theory.md#nilpotent-linear-map). Differentiation on the [polynomial ring](commutative-algebra.md#polynomial-ring) is locally nilpotent in characteristic zero but has no uniform nilpotence exponent.

##### Algebraic exponential of a locally nilpotent operator

↑ **Parent:** [Locally nilpotent operator](#locally-nilpotent-operator)

Over a field of characteristic zero, a [locally nilpotent operator](#locally-nilpotent-operator) has an algebraically defined exponential, because the sum is finite for each vector. Its inverse is $\exp(-T)$. The nilpotence bound may depend on the vector. In an [sl2 Lie algebra](semisimple-lie-algebra.md#sl2-lie-algebra) [Verma module](semisimple-lie-algebra.md#verma-module), the raising operator is locally nilpotent but the lowering operator is not, so the latter's exponential does not define an endomorphism of the ordinary algebraic module.

// Target: lie-algebra.bigb

#### Operator commutator

↑ **Parent:** [Linear operator](#linear-operator)

The commutator measures failure of two operators to commute, on a common domain where the products are defined. Direct expansion gives $[AB,C]=A[B,C]+[A,C]B$. A common [eigenvector](linear-operator-theory.md#eigenvector) of $A,B$ lies in the kernel of $[A,B]$, so an injective commutator excludes all nonzero common [eigenvectors](linear-operator-theory.md#eigenvector). A nonzero commutator need not itself be injective, and therefore does not alone exclude an individual common [eigenvector](linear-operator-theory.md#eigenvector).

#### Multiplication operator

↑ **Parent:** [Linear operator](#linear-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiplication_operator)

For a finite almost-everywhere measurable function $f$, the multiplication operator on [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) has maximal [operator domain](#operator-domain) $D(M_f)=\{u\in L^2:fu\in L^2\}$. It is a [closed operator](functional-analysis.md#closed-linear-operator): if $u_n\to u$ and $fu_n\to v$ in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space), subsequences converge almost everywhere, giving $v=fu$. Its domain is dense, since truncating a function to the sets $|f|\leq n$ approximates it in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space). If $f$ is bounded, this is a bounded [linear operator](#linear-operator) of norm equal to the essential supremum of $|f|$.

##### Spectrum of a real multiplication operator

↑ **Parent:** [Multiplication operator](#multiplication-operator)

For a real [measurable function](measure-theory.md#measurable-function) $m$ on a [sigma-finite measure](measure-theory.md#sigma-finite-measure) space, multiplication on $D(M_m)=\{f\in L^2:mf\in L^2\}$ is an [unbounded self-adjoint operator](linear-operator-theory.md#unbounded-self-adjoint-operator). Testing its adjoint relation on $\{|m|\leq n\}$ identifies the same maximal domain. Outside the [essential range](measure-theory.md#essential-range), multiplication by $(m-z)^{-1}$ is a bounded resolvent. Inside it, normalized indicators of finite-positive-measure sets where $m$ is close to $z$ are [approximate eigenvectors](linear-operator-theory.md#approximate-eigenvector), so the inverse cannot be bounded.

#### Projection (linear algebra)

↑ **Parent:** [Linear operator](#linear-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projection_(linear_algebra))

A [linear projection](#projection-linear-algebra) is an [idempotent](commutative-algebra.md#idempotent) [linear operator](#linear-operator): $P^2=P$. Every vector decomposes as $x=Px+(I-P)x$, into the [image of a linear map](#image-of-a-linear-map) and the [kernel of a linear map](linear-algebra.md#kernel-of-a-linear-map). Those two [vector subspaces](#vector-subspace) form a [direct sum](#direct-sum). An [orthogonal projection](hilbert-space.md#orthogonal-projection) additionally uses the [orthogonal complement](hilbert-space.md#orthogonal-complement) in an [inner product space](linear-algebra.md#inner-product-space).

##### Kadec-Snobar projection bound

↑ **Parent:** [Projection (linear algebra)](#projection-linear-algebra)

Every finite-dimensional [vector subspace](#vector-subspace) $E$ of a [Banach space](banach-space.md) $X$ is the range of a bounded [linear projection](#projection-linear-algebra) with the displayed norm bound. In maximal inscribed Euclidean or Hermitian [ellipsoid](geometry-and-topology.md#ellipsoid) coordinates, write the [John contact decomposition](geometry-and-topology.md#john-contact-decomposition) as $\sum_rc_ru_ru_r^*=I_E$. Its contact functionals $\phi_r(x)=u_r^*x$ have norm one on $E$. Extend them to $X$ by the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) and set $Px=\sum_rc_r\widetilde\phi_r(x)u_r$. This restricts to the identity on $E$. The contact synthesis operator has Euclidean norm one, the weights sum to $\dim E$, and the Euclidean unit ball is contained in the norm unit ball; these facts give $\|Px\|_E\le\sqrt{\dim E}\|x\|_X$.

##### Inner product adapted to an idempotent linear map

↑ **Parent:** [Projection (linear algebra)](#projection-linear-algebra)

For an [idempotent linear map](#projection-linear-algebra) $P$ on a finite-dimensional real [vector space](vector-space.md), take any positive definite [inner product](linear-algebra.md#inner-product) on that space. The displayed new [inner product](linear-algebra.md#inner-product) is positive definite since its squared norm vanishes only if both $Pu$ and $(I-P)u$ vanish. It makes the [kernel of a linear map](linear-algebra.md#kernel-of-a-linear-map) and [image of a linear map](#image-of-a-linear-map) orthogonal. Since $P^2=P$, one has $\langle Pu,v\rangle_P=\langle u,Pv\rangle_P$; thus $P$ becomes an [orthogonal projection](hilbert-space.md#orthogonal-projection).

##### Similarity classification of idempotent linear maps

↑ **Parent:** [Projection (linear algebra)](#projection-linear-algebra)

If $T^2=T$, every [vector](#vector) splits as $v=(v-Tv)+Tv$ in $\ker T\oplus\operatorname{im}T$. On these summands $T$ is respectively zero and the identity. Its [matrix](#matrix) in an adapted [basis](#basis) is therefore $\operatorname{diag}(0,I_r)$, where $r$ is its [rank of a linear map](#rank-of-a-linear-map). Two [idempotent linear maps](#projection-linear-algebra) on the same finite-dimensional [vector space](vector-space.md) are [similar matrices](linear-algebra.md#matrix-similarity) exactly when their ranks agree.

##### Oblique projection

↑ **Parent:** [Projection (linear algebra)](#projection-linear-algebra)

If two [closed subspaces of a Hilbert space](hilbert-space.md#closed-subspace-of-a-hilbert-space) give $H=V\oplus W$, the projection onto $V$ along $W$ fixes $V$ and vanishes on $W$. It need not be an [orthogonal projection](hilbert-space.md#orthogonal-projection). The [bounded inverse theorem](functional-analysis.md#bounded-inverse-theorem) applied to the addition map $(v,w)\mapsto v+w$ on the complete component spaces proves boundedness of the component maps. With both complementary subspaces nonzero, its [operator norm](continuous-dual-space.md#operator-norm) and that of $I-Q$ equal $\sec\theta_{V,W^\perp}$, with the [directed subspace angle](hilbert-space.md#directed-subspace-angle) convention. Indeed, for fixed $v\in V$, the smallest possible [norm](functional-analysis.md#norm) of $v+w$ over $w\in W$ is $\|P_{W^\perp}v\|$, which proves the formula for $\|Q\|$. Equality with $\|I-Q\|$ follows from the block representation $Q=\begin{pmatrix}I&B\\0&0\end{pmatrix}$ on $V\oplus V^\perp$: both squared [operator norms](continuous-dual-space.md#operator-norm) are $1+\|B\|^2$. If a summand is zero, $Q$ is zero or the [identity operator](#identity-operator), and one complementary [operator norm](continuous-dual-space.md#operator-norm) is zero; those cases must be treated directly.

###### Finite-dimensional Hilbert sampling reconstruction

↑ **Parent:** [Oblique projection](#oblique-projection)

For equal finite-dimensional [closed subspaces of a Hilbert space](hilbert-space.md#closed-subspace-of-a-hilbert-space) $T,S$, positivity of $\cos\theta_{T,S}$ makes $P_S|_T$ invertible. The displayed reconstruction is the unique element of $T$ whose [orthogonal projection](hilbert-space.md#orthogonal-projection) onto $S$ matches that of $f$. It is the [oblique projection](#oblique-projection) onto $T$ along $S^\perp$. Its [operator norm](continuous-dual-space.md#operator-norm) is the value of the [secant function](geometry-and-topology.md#secant-trigonometry) at the [directed subspace angle](hilbert-space.md#directed-subspace-angle), and its error is at most that [secant function](geometry-and-topology.md#secant-trigonometry) value times the best [orthogonal projection](hilbert-space.md#orthogonal-projection) error. The lower error bound follows from the [Pythagorean identity](linear-algebra.md#pythagorean-theorem-in-an-inner-product-space). Zero-dimensional cases are handled directly.

#### Operator domain

↑ **Parent:** [Linear operator](#linear-operator)

The domain $\mathcal D(A)$ of an operator $A$ is the set of vectors on which $A$ is defined. For an unbounded differential operator, the domain includes regularity and boundary conditions and is part of the operator's definition.

##### Densely defined operator

↑ **Parent:** [Operator domain](#operator-domain)

A [linear operator](#linear-operator) $T$ on a [Hilbert space](hilbert-space.md) $H$ is densely defined when its [operator domain](#operator-domain) is a [dense subset](topology.md#dense-set) of $H$. Density makes the [adjoint operator](hilbert-space.md#adjoint-operator) unique wherever its defining inner-product identity has a solution.

#### Identity operator

↑ **Parent:** [Linear operator](#linear-operator)

The identity operator maps every vector to itself. Every nonzero vector is an [eigenvector](linear-operator-theory.md#eigenvector) with [eigenvalue](linear-operator-theory.md#eigenvalue) one.

#### Composition operator

↑ **Parent:** [Linear operator](#linear-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Composition_operator)

Given a map $\tau:X\to X$, the associated composition operator on a function space sends $f$ to $f\circ\tau$.

##### Invariant functional of a composition operator

↑ **Parent:** [Composition operator](#composition-operator)

A functional $\mu$ is invariant under the composition operator $T$ when $\mu(Tf)=\mu(f)$ for every $f$. On a compact metric space, a point-evaluation functional can be averaged along an orbit, and a weak-star convergent subsequence of those averages produces an invariant functional.

#### Unitary operator

↑ **Parent:** [Linear operator](#linear-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unitary_operator)

A unitary operator $U$ on a complex vector space with an [inner product](linear-algebra.md#inner-product) satisfies $U^*U=UU^*=I$ and therefore preserves inner products.

##### Unitary equivalence

↑ **Parent:** [Unitary operator](#unitary-operator)

Two operators on [Hilbert spaces](hilbert-space.md) are unitarily equivalent if a [unitary operator](#unitary-operator) maps their operator domains onto one another and intertwines their actions. Their [spectra](linear-operator-theory.md#spectrum-functional-analysis) and [eigenvalue](linear-operator-theory.md#eigenvalue) multiplicities then agree. For nonnegative [self-adjoint operators](linear-operator-theory.md#self-adjoint-operator) it suffices that the unitary maps their closed [quadratic form](linear-algebra.md#quadratic-form) domains onto one another and preserves the forms, since the associated operator is determined by the form.

##### Eigenphase

↑ **Parent:** [Unitary operator](#unitary-operator)

An eigenphase of a [unitary operator](#unitary-operator) is a real number $\theta$ modulo one specifying an [eigenvalue](linear-operator-theory.md#eigenvalue) $e^{2\pi i\theta}$. Every unitary eigenvalue has [modulus](complex-analysis.md#modulus) one. [Quantum phase estimation](quantum-theory.md#quantum-phase-estimation) records the eigenphase corresponding to an input [eigenvector](linear-operator-theory.md#eigenvector); a superposition retains the corresponding labels coherently before measurement.

##### Unitary conjugation

↑ **Parent:** [Unitary operator](#unitary-operator)

Unitary conjugation maps an operator $A$ to $UAU^\dagger$ for a [unitary operator](#unitary-operator) $U$. It preserves [eigenvalues](linear-operator-theory.md#eigenvalue), [operator norms](continuous-dual-space.md#operator-norm), and algebraic relations such as products and adjoints.

##### Von Neumann mean ergodic theorem

↑ **Parent:** [Unitary operator](#unitary-operator)

For a [unitary operator](#unitary-operator) $U$ on a [Hilbert space](hilbert-space.md), the [Cesaro averages](real-analysis.md#cesaro-mean)

$$
A_n=\frac1n\sum_{j=0}^{n-1}U^j
$$

converge strongly to the [orthogonal projection](hilbert-space.md#orthogonal-projection) onto the fixed-point subspace $\ker(U-I)$.

###### Orthogonal decomposition for unitary ergodic averages

↑ **Parent:** [Von Neumann mean ergodic theorem](#von-neumann-mean-ergodic-theorem)

For a [unitary operator](#unitary-operator) $U$, the orthogonal complement of $\operatorname{Ran}(I-U)$ is $\ker(I-U^*)=\ker(I-U)$. On the fixed space, [Cesaro averages](real-analysis.md#cesaro-mean) act as the identity. On $(I-U)g$ they telescope to $(g-U^Ng)/N$. Their uniform norm bound extends convergence to the closure of the range, proving the [Von Neumann mean ergodic theorem](#von-neumann-mean-ergodic-theorem).

#### Commuting operators

↑ **Parent:** [Linear operator](#linear-operator)

Two [linear operators](#linear-operator) $A$ and $B$ commute when $AB=BA$. Their [matrix exponentials](linear-operator-theory.md#matrix-exponential) then satisfy $e^{A+B}=e^Ae^B=e^Be^A$.

##### Commuting maps preserve eigenspaces

↑ **Parent:** [Commuting operators](#commuting-operators)

If $CD=DC$ and $Dx=\lambda x$, then $D(Cx)=C(Dx)=\lambda Cx$. Therefore each [eigenspace](linear-operator-theory.md#eigenspace) of $D$ is invariant under $C$. The vector $Cx$ may be zero; invariance does not require it to be a nonzero [eigenvector](linear-operator-theory.md#eigenvector). This observation is the starting point for [simultaneous diagonalization](mathematics.md#simultaneous-diagonalization).

#### Anticommutator

↑ **Parent:** [Linear operator](#linear-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Anticommutator)

The anticommutator of two operators is $\{A,B\}=AB+BA$. They anticommute when this operator vanishes, equivalently when $AB=-BA$.

##### Two-by-two anticommutator characteristic polynomial

↑ **Parent:** [Anticommutator](#anticommutator)

If $A$ is diagonalizable, the [anticommutator](#anticommutator) map $B\mapsto AB+BA$ has [eigenvalues](linear-operator-theory.md#eigenvalue) $2\lambda_1$, $\lambda_1+\lambda_2$ twice, and $2\lambda_2$. Their product gives the displayed [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial). The [density of diagonalizable complex matrices](linear-operator-theory.md#density-of-diagonalizable-complex-matrices) and continuity of polynomial coefficients prove the formula also for defective matrices.

#### Conjugate linear operators

↑ **Parent:** [Linear operator](#linear-operator)

Linear operators $\alpha$ and $\beta$ on the same finite-dimensional vector space are conjugate when $\beta=s^{-1}\alpha s$ for some linear isomorphism $s$. Their matrices in any fixed basis are similar.

##### Conjugation operator on an endomorphism space

↑ **Parent:** [Conjugate linear operators](#conjugate-linear-operators)

For an invertible operator $\beta$ on $V$, the map

$$
\phi_\beta:\operatorname{End}(V)\to\operatorname{End}(V),
\qquad A\mapsto\beta^{-1}A\beta
$$

is a linear isomorphism. Conjugate choices of $\beta$ induce conjugate operators $\phi_\beta$.

### Matrix

↑ **Parent:** [Linear map](#linear-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_(mathematics))

A matrix represents a [linear map](#linear-map) after bases have been chosen for its domain and codomain.

#### Cauchy matrix

↑ **Parent:** [Matrix](#matrix)

A [Cauchy matrix](#cauchy-matrix) has entries $1/(x_i+y_j)$ with nonzero denominators. If $x_i=y_i>0$ are distinct, it is positive definite: $C_{ij}=\int_0^\infty e^{-x_is}e^{-x_js}ds$ is the Gram matrix of linearly independent exponential functions. This form occurs in finite-rank [inverse scattering transform](integrable-systems.md#inverse-scattering-transform) reconstructions.

#### Matrix norm

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_norm)

A matrix norm is a [norm](functional-analysis.md#norm) on a [vector space](vector-space.md) of [matrices](#matrix); common choices include induced [operator norms](continuous-dual-space.md#operator-norm) and the [Frobenius norm](compact-operator.md#frobenius-norm). A submultiplicative matrix norm additionally satisfies $\|AB\|\leq\|A\|\|B\|$. The [matrix 2-norm](continuous-dual-space.md#matrix-2-norm) is the norm induced by [Euclidean norms](functional-analysis.md#euclidean-norm) and equals the largest [singular value](linear-algebra.md#singular-value).

#### Matrix pencil

↑ **Parent:** [Matrix](#matrix)

A matrix pencil is an affine one-parameter family of [matrices](#matrix). For square matrices of size $m$, its determinant is a [polynomial](polynomial.md) of degree at most $m$. If $B$ is invertible, its leading coefficient is $\det B\ne0$, so at most $m$ distinct parameters give a singular matrix. This translates linear dependence in a family of bases into polynomial root counting.

#### Total nonnegativity of a matrix

↑ **Parent:** [Matrix](#matrix)

A real rectangular [matrix](#matrix) is totally nonnegative if every square minor, with row and column indices in increasing order, is nonnegative. A nonnegative bidiagonal [matrix](#matrix) is totally nonnegative, and products of compatible [totally nonnegative matrices](#total-nonnegativity-of-a-matrix) have the same property by the [Cauchy–Binet formula](linear-algebra.md#cauchy-binet-formula). This controls signs of inverse entries and underlies stability and shape-preserving properties of [B-spline](uniform-approximation.md#b-spline) collocation. Total nonnegativity permits zero minors; strict total positivity requires every such minor to be positive.

##### Checkerboard inverse of a totally nonnegative matrix

↑ **Parent:** [Total nonnegativity of a matrix](#total-nonnegativity-of-a-matrix)

If an invertible square [totally nonnegative matrix](#total-nonnegativity-of-a-matrix) $A$ has size $n$, then $\det A>0$ and

$$
(-1)^{i+j}(A^{-1})_{ij}\geq0.
$$

Indeed the [adjugate identity](linear-algebra.md#adjugate-identity) gives $(A^{-1})_{ij}=(-1)^{i+j}\det A_{\widehat j,\widehat i}/\det A$, and the deleted-row/deleted-column minor is nonnegative. Consequently an alternating vector $v_j=(-1)^j$ gives $(A^{-1}v)_i=(-1)^i\sum_j|(A^{-1})_{ij}|$.

#### Elementary column operation

↑ **Parent:** [Matrix](#matrix)

An [elementary column operation](#elementary-column-operation) interchanges two columns of a [matrix](#matrix), scales one by a nonzero scalar, or adds a multiple of another column. It is an [elementary row operation](numerical-analysis.md#elementary-row-operation) on the transpose. Hence it has the same three effects on the [determinant](linear-algebra.md#determinant): changing sign, multiplying by the scale factor, or leaving the [determinant](linear-algebra.md#determinant) unchanged.

#### Hadamard matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hadamard_matrix)

A [Hadamard matrix](#hadamard-matrix) is a real square [matrix](#matrix) with entries $+1$ and $-1$ whose rows are pairwise [orthogonal](linear-algebra.md#orthogonal-vectors). Each row has squared [norm](functional-analysis.md#norm) $n$, so $HH^T=nI$ and $H/\sqrt n$ is an [orthogonal matrix](linear-algebra.md#orthogonal-matrix). In particular $H$ is invertible, with $H^{-1}=H^T/n$. The four-by-four example

$$
H=\begin{pmatrix}1&1&1&1\\1&-1&1&-1\\1&1&-1&-1\\1&-1&-1&1\end{pmatrix}
$$

is symmetric and satisfies $H^2=4I$. It supplies an exact intertwiner in [four-tile mixed-boundary transplantation between a disk and a nonorientable surface](riemannian-geometry.md#four-tile-mixed-boundary-transplantation-between-a-disk-and-a-nonorientable-surface).

#### Square matrix

↑ **Parent:** [Matrix](#matrix)

A [matrix](#matrix) with the same number of rows and columns represents an [endomorphism](algebra.md#endomorphism) of a finite-dimensional [vector space](vector-space.md) after choosing a [basis](#basis). Square matrices support [trace](linear-algebra.md#matrix-trace), [determinant](linear-algebra.md#determinant), powers and the [matrix exponential](linear-operator-theory.md#matrix-exponential).

#### Realification of a complex matrix

↑ **Parent:** [Matrix](#matrix)

For $A=P+iQ$ with real matrices $P,Q$, the same [linear map](#linear-map) viewed over the reals has block matrix $\begin{pmatrix}P&-Q\\Q&P\end{pmatrix}$ in grouped real/imaginary coordinates. Interleaved coordinates merely permute the basis. Its complexification splits into the matrices $A$ and $\overline A$, giving the [realification determinant identity](#realification-determinant-identity).

##### Realification determinant identity

↑ **Parent:** [Realification of a complex matrix](#realification-of-a-complex-matrix)

The [realification of a complex matrix](#realification-of-a-complex-matrix) has real determinant $|\det_{\mathbb C}A|^2$. Indeed the invertible complex coordinate change $(x,y)\mapsto(x+iy,x-iy)$ conjugates its complexified block matrix to $\operatorname{diag}(A,\overline A)$. Taking determinants gives the identity, including singular matrices.

#### Entrywise matrix L1 norm

↑ **Parent:** [Matrix](#matrix)

For a real [matrix](#matrix) $M$, the entrywise L1 norm is $\sum_{r,s}|M_{rs}|$, the [L1 norm](functional-analysis.md#l1-norm) of its vector of entries. It is the usual penalty in the all-entry convention for the [Graphical Lasso](variance.md#graphical-lasso).

#### Entrywise matrix function

↑ **Parent:** [Matrix](#matrix)

Applying a [scalar](#scalar) function separately to each [matrix](#matrix) entry: $(f[X])_{ij}=f(X_{ij})$. This differs from [spectral matrix functional calculus](hilbert-space.md#spectral-matrix-functional-calculus). In particular, $\arcsin[Y]$ in [Gaussian hyperplane rounding](mathematical-optimization.md#gaussian-hyperplane-rounding) is entrywise, and its contribution to a [matrix trace](linear-algebra.md#matrix-trace) can be restricted to selected blocks by the support of the other [matrix](#matrix).

#### Hadamard product

↑ **Parent:** [Matrix](#matrix)

The [matrix](#matrix) with entries $(P\circ Q)_{ij}=P_{ij}Q_{ij}$. It differs from ordinary [matrix multiplication](#matrix-multiplication). The [Schur product theorem](linear-algebra.md#schur-product-theorem) states that it preserves [positive semidefiniteness](linear-algebra.md#positive-semidefinite-matrix) when both factors are [positive semidefinite matrices](linear-algebra.md#positive-semidefinite-matrix).

##### Hadamard power

↑ **Parent:** [Hadamard product](#hadamard-product)

For integer $k\geq1$, the entrywise power has entries $X_{ij}^k$ and equals the repeated [Hadamard product](#hadamard-product). The zero power is the all-ones [matrix](#matrix), even at zero entries, because it represents the constant function one. Every nonnegative integer [Hadamard power](#hadamard-power) of a [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix) is [positive semidefinite](linear-algebra.md#positive-semidefinite-matrix) by the [Schur product theorem](linear-algebra.md#schur-product-theorem). It is not an ordinary [matrix](#matrix) power.

#### Hermite normal form

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hermite_normal_form)

The Hermite normal form is a canonical triangular form for an integer [matrix](#matrix) under integer elementary row operations or, in the column convention, column operations. In the row convention for a nonsingular rank-two [matrix](#matrix), positive diagonal entries and reduction of the upper-right entry modulo the lower diagonal entry give the [row Hermite normal form in rank two](#row-hermite-normal-form-in-rank-two).

##### Row lattice of an integer matrix

↑ **Parent:** [Hermite normal form](#hermite-normal-form)

The row lattice of an integer [matrix](#matrix) with $m$ rows is the set of their integer linear combinations. It is an [Euclidean lattice](fourier-analysis.md#euclidean-lattice) in its real span, since it is contained in the discrete set $\mathbb Z^n$ and spans that real vector space. For a nonsingular two-by-two integer [matrix](#matrix), the [row Hermite normal form in rank two](#row-hermite-normal-form-in-rank-two) gives a canonical [basis](#basis) and proves that its index in $\mathbb Z^2$ is the absolute value of its [determinant](linear-algebra.md#determinant).

##### Row Hermite normal form in rank two

↑ **Parent:** [Hermite normal form](#hermite-normal-form)

For a [finite-index subgroup](group.md#finite-index-subgroup) $L\leq\mathbb Z^2$, its projection to the first coordinate is $a\mathbb Z$ and its intersection with the second axis is $\{0\}\times d\mathbb Z$, with $a,d>0$. Choose $(a,b)\in L$, reducing $b$ modulo $d$. Together with $(0,d)$ it is a [basis](#basis) of this [row lattice](#row-lattice-of-an-integer-matrix): subtracting a multiple of $(a,b)$ from any vector leaves a vector on the second axis. These parameters are unique, and reduction of the two coordinates shows $[\mathbb Z^2:L]=ad$. Consequently an integral [matrix](#matrix) of positive [determinant](linear-algebra.md#determinant) $n$ has a unique representative of this form under left multiplication by $SL_2(\mathbb Z)$, with $ad=n$. This proves the lattice facts underlying [determinant-n matrix representatives for Hecke operators](modular-function.md#determinant-n-matrix-representatives-for-hecke-operators).

#### Doubly stochastic matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Doubly_stochastic_matrix)

A square real [matrix](#matrix) is doubly stochastic if its entries are nonnegative and every row and column sums to $1$. Its positive-entry support satisfies the condition of the [Hall marriage theorem](graph-theory.md#hall-s-marriage-theorem): for a row subset $S$, $|S|\leq|N(S)|$ by summing column capacities. Consequently its support contains a [permutation matrix](#permutation-matrix).

##### Two-coordinate stochastic averaging

↑ **Parent:** [Doubly stochastic matrix](#doubly-stochastic-matrix)

This [doubly stochastic matrix](#doubly-stochastic-matrix) replaces two values $a,b$ by $ta+(1-t)b$ and $(1-t)a+tb$, preserving their sum. It fixes all other coordinates when embedded in a larger [matrix](#matrix). A finite product of such averaging [matrices](#matrix) and [permutation matrices](#permutation-matrix) is again doubly stochastic.

##### Birkhoff-von Neumann theorem

↑ **Parent:** [Doubly stochastic matrix](#doubly-stochastic-matrix)

Every [doubly stochastic matrix](#doubly-stochastic-matrix) is a [convex combination](mathematical-optimization.md#convex-combination) of [permutation matrices](#permutation-matrix). Equivalently, the [extreme points](mathematical-optimization.md#extreme-point) of the doubly stochastic [convex polytope](mathematical-optimization.md#convex-polytope) are exactly the permutation matrices. The extreme-point assertion follows from an [alternating-cycle perturbation of a doubly stochastic matrix](#alternating-cycle-perturbation-of-a-doubly-stochastic-matrix); the convex-hull assertion follows because a bounded finite-dimensional polytope is the convex hull of its vertices. Permutation matrices are extreme since their zero entries force the same zeros in every convex decomposition.

###### Birkhoff decomposition by support matchings

↑ **Parent:** [Birkhoff-von Neumann theorem](#birkhoff-von-neumann-theorem)

For a [doubly stochastic matrix](#doubly-stochastic-matrix), the [Hall marriage theorem](graph-theory.md#hall-s-marriage-theorem) supplies a [perfect matching](graph-theory.md#perfect-matching) in its positive-entry support. Subtract the smallest matched entry times the corresponding [permutation matrix](#permutation-matrix). The residual has equal row and column sums and smaller support unless it vanishes. Repeating gives a [convex combination](mathematical-optimization.md#convex-combination) of [permutation matrices](#permutation-matrix). With $r$ initially positive entries, there are at most $r-n+1$ terms, since a positive-mass residual has at least $n$ positive entries. Elementary augmenting-path matching gives $O(n^5)$ arithmetic operations.

###### Alternating-cycle perturbation of a doubly stochastic matrix

↑ **Parent:** [Birkhoff-von Neumann theorem](#birkhoff-von-neumann-theorem)

For a [doubly stochastic matrix](#doubly-stochastic-matrix) with a fractional entry, form the row-column [bipartite graph](graph-theory.md#bipartite-graph) of entries strictly between zero and one. Every incident vertex has degree at least two, so there is an even cycle. A matrix supported on that cycle with alternating entries $+1,-1$ has zero row and column sums. A sufficiently small positive multiple can be both added and subtracted while preserving entry bounds. The original matrix is then the midpoint of two distinct doubly stochastic matrices, so it is not an [extreme point](mathematical-optimization.md#extreme-point).

#### Rational matrix

↑ **Parent:** [Matrix](#matrix)

A rational matrix is a [matrix](#matrix) whose entries are [rational numbers](number-theory.md#rational-number). Multiplying by a common denominator produces an [integer](number-theory.md#integer) matrix and preserves its homogeneous solution set.

#### Nonnegative matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nonnegative_matrix)

A real [matrix](#matrix) is nonnegative when every entry is nonnegative. This entrywise condition differs from being a [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix): the [symmetric matrix](linear-algebra.md#symmetric-matrix) $\begin{pmatrix}0&1\\1&0\end{pmatrix}$ is nonnegative but has [eigenvalues](linear-operator-theory.md#eigenvalue) $1$ and $-1$.

##### Irreducible nonnegative matrix

↑ **Parent:** [Nonnegative matrix](#nonnegative-matrix)

A square [nonnegative matrix](#nonnegative-matrix) $A$ is irreducible if for each pair $(i,j)$ there is an integer $k\geq0$ with $(A^k)_{ij}>0$. This says that every index can reach every other through positive entries. The [Perron–Frobenius theorem](#perron-frobenius-theorem) then gives a positive leading [eigenvector](linear-operator-theory.md#eigenvector) and an algebraically [simple eigenvalue](linear-operator-theory.md#simple-eigenvalue). Irreducibility alone permits other [eigenvalues](linear-operator-theory.md#eigenvalue) of the same [modulus](complex-analysis.md#modulus): the cyclic permutation [matrix](#matrix) $\begin{pmatrix}0&1\\1&0\end{pmatrix}$ has [eigenvalues](linear-operator-theory.md#eigenvalue) $1,-1$.

###### Primitive nonnegative matrix

↑ **Parent:** [Irreducible nonnegative matrix](#irreducible-nonnegative-matrix)

A square [nonnegative matrix](#nonnegative-matrix) $A$ is primitive if some positive integer power $A^k$ has strictly positive entries. It is therefore an [irreducible nonnegative matrix](#irreducible-nonnegative-matrix). The [Perron–Frobenius theorem](#perron-frobenius-theorem) gives a leading [eigenvalue](linear-operator-theory.md#eigenvalue) whose [modulus](complex-analysis.md#modulus) is strictly larger than that of every other [eigenvalue](linear-operator-theory.md#eigenvalue). Every strictly positive [matrix](#matrix) is primitive; the two-cycle permutation [matrix](#matrix) is irreducible but not primitive.

<h5 id="perron-frobenius-theorem">Perron–Frobenius theorem</h5>

↑ **Parent:** [Nonnegative matrix](#nonnegative-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perron–Frobenius_theorem)

The strictly positive case states that a real square [matrix](#matrix) $W$ with $W_{ij}>0$ has a positive [simple eigenvalue](linear-operator-theory.md#simple-eigenvalue) $\lambda$ and positive left and right [eigenvectors](linear-operator-theory.md#eigenvector), with all other [eigenvalues](linear-operator-theory.md#eigenvalue) strictly smaller in [modulus](complex-analysis.md#modulus). The [Brouwer fixed-point theorem](topological-analysis.md#brouwer-fixed-point-theorem) applied to $v\mapsto Wv/(\mathbf1^TWv)$ on the nonnegative unit [simplex](algebraic-topology.md#simplex) gives $v>0$ and $Wv=\lambda v$. For another [eigenvector](linear-operator-theory.md#eigenvector) $z$, maximize $|z_i|/v_i$; the [triangle inequality](topological-analysis.md#triangle-inequality) gives $|\mu|\leq\lambda$. Equality forces every [modulus](complex-analysis.md#modulus) ratio and [complex argument](complex-analysis.md#argument-complex-analysis) to agree because every entry is positive, so $z$ is proportional to $v$ and $\mu=\lambda$. Apply the same argument to $W^T$ for a positive left [eigenvector](linear-operator-theory.md#eigenvector); its positive pairing with $v$ rules out a [generalized eigenvector](linear-operator-theory.md#generalized-eigenvector) at $\lambda$, establishing algebraic simplicity. For merely nonnegative matrices a nonnegative leading [eigenvector](linear-operator-theory.md#eigenvector) exists. An [irreducible nonnegative matrix](#irreducible-nonnegative-matrix) has a positive leading [eigenvector](linear-operator-theory.md#eigenvector) and simple Perron [eigenvalue](linear-operator-theory.md#eigenvalue); a [primitive nonnegative matrix](#primitive-nonnegative-matrix) has the strict [modulus](complex-analysis.md#modulus) gap.

#### All-ones matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/All-ones_matrix)

The all-ones matrix $J=\mathbf e\mathbf e^T$ has every entry equal to one, where $\mathbf e=(1,\ldots,1)^T$. On $\mathbb R^n$, the matrix $J/n$ is the [orthogonal projection matrix](linear-algebra.md#orthogonal-projection-matrix) onto $\operatorname{span}\{\mathbf e\}$.

#### Row and column spaces

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Row_and_column_spaces)

The [row space](#row-space) of a [matrix](#matrix) is the span of its rows, and its [column space](#column-space) is the span of its columns. Both have dimension equal to the [matrix rank](#matrix-rank), though they lie in different ambient coordinate spaces for a rectangular matrix.

##### Row space

↑ **Parent:** [Row and column spaces](#row-and-column-spaces)

The row space of a [matrix](#matrix) is the [linear span](#linear-span) of its rows. It is the [column space](#column-space) of the [matrix transpose](#transpose).

##### Column space

↑ **Parent:** [Row and column spaces](#row-and-column-spaces)

The column space of a [matrix](#matrix) $A$ is the [linear span](#linear-span) of its columns. It is the [image of a linear map](#image-of-a-linear-map) represented by $A$.

#### Binary matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_matrix)

A binary matrix is a [matrix](#matrix) all of whose entries belong to $\{0,1\}$.

#### Submatrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Submatrix)

A submatrix is obtained from a [matrix](#matrix) by retaining selected rows and selected columns. A principal submatrix of a square matrix retains the same index set for its rows and columns.

##### Minor (linear algebra)

↑ **Parent:** [Submatrix](#submatrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Minor_(linear_algebra))

A matrix minor is the [determinant](linear-algebra.md#determinant) of a square [submatrix](#submatrix) obtained by selecting rows and columns of a [matrix](#matrix). Over a [field](algebra.md#field), the [matrix rank](#matrix-rank) is less than $r$ exactly when every $r$-by-$r$ [matrix minor](#minor-linear-algebra) vanishes. In a [matrix](#matrix) of [regular functions](ringed-space.md#regular-function), these equations define a closed rank-defect locus, explaining the [determinantal variety](algebraic-geometry.md#determinantal-variety) construction.

###### Principal minor

↑ **Parent:** [Minor (linear algebra)](#minor-linear-algebra)

A principal minor is the [determinant](linear-algebra.md#determinant) of a square [submatrix](#submatrix) selected using the same index set for rows and columns. For a three-by-three [matrix](#matrix), the coefficient of $\lambda$ in its monic [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) is the sum of its three principal minors of order two.

#### Entrywise maximum norm

↑ **Parent:** [Matrix](#matrix)

The entrywise maximum norm is the largest absolute value of a matrix entry. For compatible vectors $x$ and $y$,

$$
|x^TAy|\leq\|A\|_{\max}\|x\|_1\|y\|_1.
$$

#### Tridiagonal matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tridiagonal_matrix)

A tridiagonal matrix has zero entries outside its main diagonal and the two adjacent diagonals. Linear systems with a nonsingular tridiagonal coefficient matrix can be solved in linear time by the [Thomas algorithm](numerical-analysis.md#tridiagonal-matrix-algorithm).

#### Block matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Block_matrix)

A block matrix partitions its rows and columns into rectangular submatrices called blocks, allowing a matrix calculation to be expressed in terms of those blocks.

##### Block diagonal matrix

↑ **Parent:** [Block matrix](#block-matrix)

A [block matrix](#block-matrix) is block diagonal if all off-diagonal blocks vanish. It represents independent actions on a [direct sum](#direct-sum) of [vector spaces](vector-space.md). Its [determinant](linear-algebra.md#determinant) is the product of the diagonal-block [determinants](linear-algebra.md#determinant).

##### Block tridiagonal matrix

↑ **Parent:** [Block matrix](#block-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Block_tridiagonal_matrix)

A block tridiagonal matrix has nonzero blocks only on its main block diagonal and the two adjacent block diagonals. It is the block analogue of a [tridiagonal matrix](#tridiagonal-matrix).

#### Diagonally dominant matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diagonally_dominant_matrix)

A square matrix is diagonally dominant when the absolute value of every diagonal entry is at least the sum of the absolute values of the other entries in its row.

##### Strictly diagonally dominant matrix

↑ **Parent:** [Diagonally dominant matrix](#diagonally-dominant-matrix)

A matrix is strictly diagonally dominant when every diagonal-dominance inequality is strict. A real symmetric strictly diagonally dominant matrix with positive diagonal is [positive definite](linear-algebra.md#positive-definite-matrix) by the [Gershgorin circle theorem](numerical-analysis.md#gershgorin-circle-theorem).

###### Inverse infinity-norm bound from diagonal dominance

↑ **Parent:** [Strictly diagonally dominant matrix](#strictly-diagonally-dominant-matrix)

If $\delta=\min_i(|a_{ii}|-\sum_{j\ne i}|a_{ij}|)>0$, then $A$ is invertible and its [operator norm](continuous-dual-space.md#operator-norm) on $\ell^\infty$ satisfies the displayed bound. For $Ax=b$, choose $i$ maximizing $|x_i|$. The [reverse triangle inequality](topological-analysis.md#reverse-triangle-inequality) gives $|b_i|\ge\delta\|x\|_{\ell^\infty}$. Taking $b=0$ proves injectivity and hence invertibility in finite dimensions; taking arbitrary $b$ proves the bound. The estimate is useful for converting [strict diagonal dominance](#strictly-diagonally-dominant-matrix) into quantitative [matrix inverse](linear-algebra.md#matrix-inverse) stability.

#### Transpose

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transpose)

The matrix transpose interchanges rows and columns: $(A^T)_{ij}=A_{ji}$. On a fixed matrix space, $A\mapsto A^T$ is the [transposition map](#transpose), a [linear map](#linear-map) that preserves the [trace norm](functional-analysis.md#trace-norm) but is not completely positive in dimensions greater than one.

#### Matrix logarithm

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_logarithm)

For a positive-definite [Hermitian matrix](hilbert-space.md#hermitian-operator) with [spectral decomposition](linear-operator-theory.md#spectral-decomposition) $A=U\operatorname{diag}(\lambda_j)U^*$, the matrix logarithm is $\log A=U\operatorname{diag}(\log\lambda_j)U^*$. More generally it is a branch of the inverse of the [matrix exponential](linear-operator-theory.md#matrix-exponential) when such a branch exists.

##### Analytic determinant square root for accretive symmetric matrices

↑ **Parent:** [Matrix logarithm](#matrix-logarithm)

On complex symmetric [matrices](#matrix) with positive-definite real part, the [determinant](linear-algebra.md#determinant) has a nonzero analytic square root normalized positively on real positive [matrices](#matrix). It is continued within this accretive domain. For $A=G+iB$, put $C=G^{-1/2}BG^{-1/2}$ with real [eigenvalues](linear-operator-theory.md#eigenvalue) $b_j$; then $d(A)=\sqrt{\det G}\prod_j\sqrt{1+ib_j}$, using positive-real-part roots for each factor. The principal scalar square root of the product [determinant](linear-algebra.md#determinant) need not equal this continued root: accumulated [determinant](linear-algebra.md#determinant) arguments can cross the scalar branch cut. The principal [matrix](#matrix) logarithm instead tracks all factors consistently.

##### Diagonal logarithm concavity bound

↑ **Parent:** [Matrix logarithm](#matrix-logarithm)

For a positive-definite [Hermitian operator](hilbert-space.md#hermitian-operator) $A=\sum_jt_j|u_j\rangle\langle u_j|$ and a unit vector $v$, the weights $|\langle v|u_j\rangle|^2$ form a probability distribution. Scalar logarithmic concavity bounds their average of $\log t_j$ by the logarithm of their average of $t_j$. Positive semidefinite operators follow by a limiting convention. Using the eigenbasis of a [density operator](quantum-theory.md#density-matrix) $\rho$ gives $S(\rho\|\sigma)\geq D(r\|q)$, where $r$ is the spectrum of $\rho$ and $q$ the diagonal of $\sigma$ in that basis. This yields [nonnegativity of quantum relative entropy](von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy) without commutativity.

##### Existence of a logarithm for every invertible complex matrix

↑ **Parent:** [Matrix logarithm](#matrix-logarithm)

An invertible complex [Jordan block](linear-operator-theory.md#jordan-block) $\lambda I+N$, with $N^s=0$, has logarithm $\ell I+\sum_{k=1}^{s-1}(-1)^{k+1}(N/\lambda)^k/k$, where $e^\ell=\lambda$. Applying this construction blockwise and conjugating back proves surjectivity of the [matrix exponential](linear-operator-theory.md#matrix-exponential) on the complex [general linear group](group-theory.md#general-linear-group). There is no globally single-valued continuous choice of logarithm.

<h5 id="klein-s-inequality">Klein's inequality</h5>

↑ **Parent:** [Matrix logarithm](#matrix-logarithm)

For positive-definite [Hermitian matrices](hilbert-space.md#hermitian-operator) $A,B$, Klein's inequality gives

$$
\operatorname{Tr}[A(\ln A-\ln B)]\geq\operatorname{Tr}(A-B),
$$

with equality exactly when $A=B$. To prove it, let $a_i,b_j$ be their [eigenvalues](linear-operator-theory.md#eigenvalue) and $u_i,v_j$ their orthonormal eigenvectors. The weights $w_{ij}=|\langle u_i,v_j\rangle|^2$ have row and column sums one. The difference between the two sides is

$$
\sum_{i,j}w_{ij}\left[a_i\ln\frac{a_i}{b_j}-a_i+b_j\right]\geq0
$$

by the scalar [logarithm inequality](calculus.md#logarithm-inequality) $\ln t\leq t-1$. Equality requires $a_i=b_j$ whenever $w_{ij}>0$, implying $A=B$. Limits extend the result to positive semidefinite matrices with the appropriate support condition. Applying it to trace-one matrices proves [nonnegativity of quantum relative entropy](von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy).

#### Matrix power

↑ **Parent:** [Matrix](#matrix)

For a square [matrix](#matrix) $A$ and a [nonnegative integer](number-theory.md#integer) $k$, the matrix power is the repeated product

$$
A^k=\underbrace{AA\cdots A}_{k\text{ factors}},
$$

with $A^0=I$.

#### Matrix element

↑ **Parent:** [Matrix](#matrix)

A matrix element $A_{ij}$ is the entry in row $i$ and column $j$ of a [matrix](#matrix) $A$.

#### Sparse matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sparse_matrix)

A sparse matrix has few nonzero [matrix elements](#matrix-element) in each row or column compared with its dimension. Algorithms normally require an efficient oracle that lists the positions and values of those entries.

##### Compressed sparse storage

↑ **Parent:** [Sparse matrix](#sparse-matrix)

[Compressed sparse storage](#compressed-sparse-storage) keeps a [sparse matrix](#sparse-matrix) as numerical nonzero values, their row or column indices, and pointers to the start of each compressed column or row. It avoids allocating all $N^2$ entries. A sparse direct solver must additionally allocate possible [fill-in](numerical-analysis.md#fill-in) predicted by [symbolic factorization](numerical-analysis.md#symbolic-factorization), because elimination can create entries absent from the input.

##### Matrix bandwidth

↑ **Parent:** [Sparse matrix](#sparse-matrix)

The bandwidth in this convention is the largest distance from the main diagonal of a nonzero [matrix](#matrix) entry. A symmetric positive-definite [matrix](#matrix) of bandwidth $b$ can be factored using $O(Nb^2)$ operations and $O(Nb)$ storage; its [Cholesky decomposition](linear-algebra.md#cholesky-decomposition) does not introduce entries outside that band. A variable permutation changes bandwidth, so it is a property of both the sparsity pattern and its ordering.

#### Matrix unit

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_unit)

The matrix unit $E_{ij}$ has entry one in row $i$, column $j$, and zero in every other position. The matrix units form the standard [basis](#basis) of the [vector space](vector-space.md) of matrices of a fixed size.

#### Matrix rank

↑ **Parent:** [Matrix](#matrix)

The rank of a matrix is the [dimension](#dimension-vector-space) of its column space, equivalently the dimension of its row space.

##### Rank bound for a matrix product

↑ **Parent:** [Matrix rank](#matrix-rank)

For composable [linear maps](#linear-map), $\operatorname{im}(AB)=A(\operatorname{im}B)$ lies in $\operatorname{im}A$ and has [dimension](#dimension-vector-space) at most that of $\operatorname{im}B$. This proves the bound on the [rank of a matrix](#matrix-rank) product. When $A$ is $m\times p$, $B$ is $p\times n$, and $m,n\geq p$, the bound $p$ is attained by $A=\binom{I_p}{0}$ and $B=(I_p\ 0)$.

##### Column rank

↑ **Parent:** [Matrix rank](#matrix-rank)

The [column rank](#column-rank) of a [matrix](#matrix) is the dimension of its image as a [linear map](#linear-map), equivalently the dimension of the span of its columns. Multiplication on the left by an [invertible matrix](linear-algebra.md#invertible-matrix) preserves all column relations, and [elementary column operations](#elementary-column-operation) preserve their span. In [row echelon form](numerical-analysis.md#row-echelon-form) the pivot columns form a basis of the [column space](#column-space). Its dimension equals the number of nonzero rows, and hence the [row rank](#row-rank).

##### Row rank

↑ **Parent:** [Matrix rank](#matrix-rank)

The [row rank](#row-rank) of a [matrix](#matrix) is the dimension of the [vector space](vector-space.md) spanned by its rows. [Elementary row operations](numerical-analysis.md#elementary-row-operation) preserve this space; multiplication on the right by an [invertible matrix](linear-algebra.md#invertible-matrix) preserves all [linear relations](#linear-relation) among the rows. In [row echelon form](numerical-analysis.md#row-echelon-form) the nonzero rows are [linearly independent](#linear-independence), so the row rank is the number of pivots. The pivot columns are also [linearly independent](#linear-independence) and span the [column space](#column-space), proving equality with the [column rank](#column-rank).

##### Rank orbit of a matrix under left-right multiplication

↑ **Parent:** [Matrix rank](#matrix-rank)

Two rectangular matrices are related by invertible left and right multiplication exactly when their ranks agree. The rank-$r$ orbit in $\operatorname{Mat}_{b\times a}(k)$ has dimension $r(a+b-r)$: choose its image in a [Grassmannian](differential-geometry.md#grassmannian), then a surjective map to that image. These are the representation orbits of the [one-arrow quiver](algebra.md#kronecker-quiver-with-one-arrow).

##### Subadditivity of matrix rank

↑ **Parent:** [Matrix rank](#matrix-rank)

The image of the [linear map](#linear-map) $A+B$ is contained in the sum of the images of $A$ and $B$. Since the [dimension of a vector space](#dimension-vector-space) of this sum is at most the sum of their dimensions, [matrix rank](#matrix-rank) is subadditive. Iteration shows that a sum of $r$ [matrices](#matrix) of [matrix rank](#matrix-rank) at most one has [matrix rank](#matrix-rank) at most $r$, over any [field](algebra.md#field).

##### Full column rank

↑ **Parent:** [Matrix rank](#matrix-rank)

An $m\times n$ matrix has full column rank when its rank is $n$, equivalently when its columns are [linearly independent vectors](#linear-independence).

##### Full row rank

↑ **Parent:** [Matrix rank](#matrix-rank)

An $m\times n$ matrix has full row rank when its rank is $m$, equivalently when its rows are [linearly independent vectors](#linear-independence).

#### Identity matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Identity_matrix)

The identity matrix has ones on its main diagonal and zeros elsewhere, and satisfies $IA=AI=A$ whenever the products are defined.

#### Rank-one matrix

↑ **Parent:** [Matrix](#matrix)

A nonzero matrix has rank one exactly when it can be written as an outer product $uv^T$.

#### Bidiagonal matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bidiagonal_matrix)

A bidiagonal matrix has nonzero entries only on its main diagonal and one adjacent diagonal. The [upper bidiagonal matrix](#upper-bidiagonal-matrix) uses the superdiagonal; the lower version uses the subdiagonal.

##### Upper bidiagonal matrix

↑ **Parent:** [Bidiagonal matrix](#bidiagonal-matrix)

An upper bidiagonal matrix can have nonzero entries only on its main diagonal and first superdiagonal.

#### Matrix multiplication

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_multiplication)

Matrix multiplication represents composition of linear maps. Its entries are $(AB)_{ij}=\sum_kA_{ik}B_{kj}$.

##### Matrix product

↑ **Parent:** [Matrix multiplication](#matrix-multiplication)

For [matrices](#matrix) $A\in\mathbb F^{m\times n}$ and $B\in\mathbb F^{n\times p}$, their matrix product is the [matrix](#matrix) $AB\in\mathbb F^{m\times p}$ with entries $(AB)_{ij}=\sum_{k=1}^nA_{ik}B_{kj}$. The operation producing it is [matrix multiplication](#matrix-multiplication), representing composition of the corresponding [linear maps](#linear-map).

##### Outer product

↑ **Parent:** [Matrix multiplication](#matrix-multiplication)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Outer_product)

The outer product of column vectors $u$ and $v$ is the rank-at-most-one matrix $uv^T$, whose $(i,j)$ entry is $u_iv_j$.

#### Hessenberg matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hessenberg_matrix)

An upper Hessenberg matrix has zero entries below the first subdiagonal; the lower version has zero entries above the first superdiagonal. The [upper Hessenberg matrix](#upper-hessenberg-matrix) is one of these two forms.

##### Upper Hessenberg matrix

↑ **Parent:** [Hessenberg matrix](#hessenberg-matrix)

An upper Hessenberg matrix has zero entries below its first subdiagonal: $a_{ij}=0$ whenever $i>j+1$.

#### Permutation matrix

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Permutation_matrix)

A permutation matrix has exactly one entry equal to one in each row and column and zeros elsewhere. Left or right multiplication permutes coordinates, and $P^{-1}=P^T$.

##### Signed permutation matrix

↑ **Parent:** [Permutation matrix](#permutation-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Signed_permutation_matrix)

A signed permutation matrix has exactly one nonzero entry in each row and column, and every nonzero entry is $1$ or $-1$. It is a product of a diagonal sign matrix and a [permutation matrix](#permutation-matrix).

#### Matrix representation of a linear map

↑ **Parent:** [Matrix](#matrix)

Given ordered bases $\mathcal B=(v_j)$ and $\mathcal C=(w_i)$, the matrix $[T]_{\mathcal C\leftarrow\mathcal B}$ has column $j$ equal to the $\mathcal C$-coordinate vector of $T(v_j)$.

#### Kronecker product

↑ **Parent:** [Matrix](#matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kronecker_product)

For matrices $A$ and $B$, the Kronecker product $A\otimes B$ replaces each entry $a_{ij}$ by the block $a_{ij}B$. It satisfies

$$
(A\otimes B)(C\otimes D)=AC\otimes BD
$$

whenever the products are defined.

##### Kronecker sum

↑ **Parent:** [Kronecker product](#kronecker-product)

The [Kronecker sum](#kronecker-sum) of square [matrices](#matrix) combines their [Kronecker products](#kronecker-product) with [identity matrices](#identity-matrix). If $Ax=\lambda x$ and $By=\mu y$, then $x\otimes y$ is an [eigenvector](linear-operator-theory.md#eigenvector) with [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda+\mu$. Tensor-product spatial grids therefore turn separated coordinate Laplacians into a [Kronecker sum](#kronecker-sum). Two [Hermitian matrices](hilbert-space.md#hermitian-operator) give a Hermitian [Kronecker sum](#kronecker-sum), allowing an [energy method](numerical-analysis.md#energy-method) without computing every eigenvector.

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra.md)
2. [Algebra](algebra.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (323)

- [Affine function](#affine-function)
- [Affine group](lie-theory.md#affine-group)
- [Affine line in a vector space](#affine-line-in-a-vector-space)
- [Affine space](geometry-and-topology.md#affine-space)
- [Affine space of solutions of the Hodge Poisson equation](differential-form.md#affine-space-of-solutions-of-the-hodge-poisson-equation)
- [Affine subspace](#affine-subspace)
- [Algebra over a field](algebra.md#algebra-over-a-field)
- [Algebraic structure](algebra.md#algebraic-structure)
- [Alternating bilinear form](linear-algebra.md#alternating-bilinear-form)
- [Antilinear map](#antilinear-map)
- [Antipodal-free closed cover from simplex Voronoi cells](algebraic-topology.md#antipodal-free-closed-cover-from-simplex-voronoi-cells)
- [Basis](#basis)
- [Basis extension](#basis-extension)
- [Basis vector](#basis-vector)
- [Bilinear map](linear-algebra.md#bilinear-map)
- [Bilinearity](linear-algebra.md#bilinearity)
- [Block diagonal matrix](#block-diagonal-matrix)
- [Boolean multilinearization](polynomial.md#boolean-multilinearization)
- [Burnside matrix-algebra theorem](associative-algebra.md#burnside-matrix-algebra-theorem)
- [Čech cohomology of the punctured affine plane](ringed-space.md#cech-cohomology-of-the-punctured-affine-plane)
- [Coideal](linear-algebra.md#coideal)
- [Complete flag](#complete-flag)
- [Complex bilinear dimension bound](linear-algebra.md#complex-bilinear-dimension-bound)
- [Complex vector space](#complex-vector-space)
- [Composition of mixed tensors](linear-algebra.md#composition-of-mixed-tensors)
- [Conic Carathéodory theorem](mathematical-optimization.md#conic-caratheodory-theorem)
- [Convex cone](mathematical-optimization.md#convex-cone)
- [Convex domination form of the Hahn-Banach theorem](functional-analysis.md#convex-domination-form-of-the-hahn-banach-theorem)
- [Cotangent space of a formal power series ring](commutative-algebra.md#cotangent-space-of-a-formal-power-series-ring)
- [Cotangent space of a local ring](commutative-algebra.md#cotangent-space-of-a-local-ring)
- [Cross-product Lie algebra](lie-algebra.md#cross-product-lie-algebra)
- [Cyclic trace identity between adjacent weight spaces](semisimple-lie-algebra.md#cyclic-trace-identity-between-adjacent-weight-spaces)
- [Defining representation of a matrix Lie algebra](lie-algebra.md#defining-representation-of-a-matrix-lie-algebra)
- [Determinant of Hermitian congruence](hilbert-space.md#determinant-of-hermitian-congruence)
- [Dimension of a bounded-total-degree polynomial space](polynomial.md#dimension-of-a-bounded-total-degree-polynomial-space)
- [Direct sum](#direct-sum)
- [Dual image and kernel annihilator identity](linear-algebra.md#dual-image-and-kernel-annihilator-identity)
- [Eigenspace decomposition of a linear involution](group-theory.md#eigenspace-decomposition-of-a-linear-involution)
- [Eigenspaces of a symplectic involution](linear-algebra.md#eigenspaces-of-a-symplectic-involution)
- [Elementary abelian group](group.md#elementary-abelian-group)
- [Exterior square of the defining orthogonal representation](semisimple-lie-algebra.md#exterior-square-of-the-defining-orthogonal-representation)
- [Fan in toric geometry](toric-geometry.md#fan-in-toric-geometry)
- [Fekete interpolation sites for a continuous function space](uniform-approximation.md#fekete-interpolation-sites-for-a-continuous-function-space)
- [Finite convex function as supremum of affine minorants](real-analysis.md#finite-convex-function-as-supremum-of-affine-minorants)
- [Finite-dimensional non-Archimedean norm equivalence over a complete field](arithmetic.md#finite-dimensional-non-archimedean-norm-equivalence-over-a-complete-field)
- [Flag (linear algebra)](#flag-linear-algebra)
- [Formal power series module](commutative-algebra.md#formal-power-series-module)
- [Free graded Lie algebra](lie-algebra.md#free-graded-lie-algebra)
- [Frobenius monoid](category-theory.md#frobenius-monoid)
- [Function space](functional-analysis.md#function-space)
- [General affine group](group-theory.md#general-affine-group)
- [General linear group](group-theory.md#general-linear-group)
- [General linear group modulo the unitary group](fiber-bundle.md#general-linear-group-modulo-the-unitary-group)
- [General linear Lie algebra](lie-algebra.md#general-linear-lie-algebra)
- [Global dimension](module-theory.md#global-dimension)
- [Group algebra](associative-algebra.md#group-algebra)
- [Group representation](representation-theory.md#group-representation)
- [Homogeneous function](real-analysis.md#homogeneous-function)
- [Hyperbolic plane (quadratic form)](linear-algebra.md#hyperbolic-plane-quadratic-form)
- [Hyperplane separation theorem](mathematical-optimization.md#hyperplane-separation-theorem)
- [Image criterion for a matrix factorization](linear-algebra.md#image-criterion-for-a-matrix-factorization)
- [Initial-form lower bound for ideal generators](algebra.md#initial-form-lower-bound-for-ideal-generators)
- [Inner product adapted to an idempotent linear map](#inner-product-adapted-to-an-idempotent-linear-map)
- [Inner product space](linear-algebra.md#inner-product-space)
- [Intersection of vector subspaces](#intersection-of-vector-subspaces)
- [Joint spectrum](mathematics.md#joint-spectrum)
- [Laplacian eigenspace](linear-operator-theory.md#laplacian-eigenspace)
- [Lie algebra](lie-algebra.md)
- [Lie algebra representation](lie-algebra.md#lie-algebra-representation)
- [Linear endomorphism](algebra.md#linear-endomorphism)
- [Linear operator](#linear-operator)
- [Linear space (geometry)](combinatorics.md#linear-space-geometry)
- [Linear span](#linear-span)
- [Matrix norm](#matrix-norm)
- [Matrix unit](#matrix-unit)
- [Maximum dimension of a totally isotropic subspace](linear-algebra.md#maximum-dimension-of-a-totally-isotropic-subspace)
- [Minkowski addition](geometry-and-topology.md#minkowski-addition)
- [Module isomorphism](module-theory.md#module-isomorphism)
- [Monomial orthonormal basis on the unit torus](linear-algebra.md#monomial-orthonormal-basis-on-the-unit-torus)
- [Multilinear map](linear-algebra.md#multilinear-map)
- [Nilpotence of commutation by a nilpotent endomorphism](linear-operator-theory.md#nilpotence-of-commutation-by-a-nilpotent-endomorphism)
- [Nilpotent commutator preserves generalized eigenspaces](linear-operator-theory.md#nilpotent-commutator-preserves-generalized-eigenspaces)
- [Nondegenerate bilinear form](linear-algebra.md#nondegenerate-bilinear-form)
- [One-sided inverses of finite-dimensional endomorphisms](#one-sided-inverses-of-finite-dimensional-endomorphisms)
- [Order of a finite group of exponent two](group.md#order-of-a-finite-group-of-exponent-two)
- [Orthogonal basis](linear-algebra.md#orthogonal-basis)
- [Orthogonal complement for a bilinear form](linear-algebra.md#orthogonal-complement-for-a-bilinear-form)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3.md#17c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3.md#1a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-3.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-6.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1.md#8d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-1.md#14g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3.md#7f/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-11.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-14.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-15.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-3.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-3.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-4.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-6.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3.md#1f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3.md#7g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-10.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-15.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-23.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-24.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-36.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-1.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-22.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-3.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-4.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2.md#5b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1.md#1c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1.md#9c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1.md#16f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-1.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-15.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-24.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-24.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-33.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4.md#1h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1.md#22g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-15.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-4.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-56.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-2.md#10g/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1.md#18f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-15.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-15.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-2.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-2.md#6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-27.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-52.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-60.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-60.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-89.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-89.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-1.md#7c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-2.md#1e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-20.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-8.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1.md#9g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2.md#1g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3.md#10g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-4.md#13e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#19f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#20h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-17.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-17.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-2.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-21.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-21.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-21.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-6.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-1.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-16.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-19.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-2.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-24.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-3.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4.md#4/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-19.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-21.md#1/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-21.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-4.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2.md#10e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4.md#1e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-1.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-13.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-15.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-36.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-5.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-7.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-8.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1.md#1g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4.md#10g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4.md#1g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-1.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-1.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-15.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-24.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-3.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-4.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-41.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#19g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4.md#26k/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-1.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-1.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-1.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-11.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-12.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-17.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-18.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-40.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1.md#9f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-2.md#10f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-2.md#12g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-101.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-101.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-101.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-102.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-109.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-115.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-122.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-122.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-302.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-302.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-313.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1.md#1f/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1.md#9f/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4.md#11e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#16i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-109.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-128.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-128.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-134.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-339.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-339.md#1/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-2.md#1e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-4.md#1e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-1.md#1f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-2.md#12e/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-115.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-302.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1.md#8f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-115.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#30k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#19h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-101.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-1.md#8g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-4.md#9e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#19h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2.md#18h/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-1.md#8a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-4.md#1f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1.md#22i/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-101.md#1/iv/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1.md#31k/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-102.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-111.md#2/a/solution)
- [Perfect pairing](linear-algebra.md#perfect-pairing)
- [Positivity (linear maps)](quantum-information-theory.md#positivity-linear-maps)
- [Projective representation](representation-theory.md#projective-representation)
- [Proper vector subspace](#proper-vector-subspace)
- [Quadratic constant extension of a q-squared linearized splitting field](polynomial.md#quadratic-constant-extension-of-a-q-squared-linearized-splitting-field)
- [Quasi-norm](functional-analysis.md#quasi-norm)
- [Quotient Lie algebra](lie-algebra.md#quotient-lie-algebra)
- [Radially open convex set](mathematical-optimization.md#radially-open-convex-set)
- [Rank bound for a nonsingular complex bilinear map](linear-algebra.md#rank-bound-for-a-nonsingular-complex-bilinear-map)
- [Rank of a vector bundle](fiber-bundle.md#rank-of-a-vector-bundle)
- [Rational space](algebraic-topology.md#rational-space)
- [Real square roots of operators with simple real spectrum](linear-operator-theory.md#real-square-roots-of-operators-with-simple-real-spectrum)
- [Real vector space](#real-vector-space)
- [Representation of a Banach algebra](module-theory.md#representation-of-a-banach-algebra)
- [Representation of an associative algebra](module-theory.md#representation-of-an-associative-algebra)
- [Representation over the rational numbers](representation-theory.md#representation-over-the-rational-numbers)
- [Right inverse](function.md#right-inverse)
- [Row rank](#row-rank)
- [Scalar](#scalar)
- [Scalar multiplication](#scalar-multiplication)
- [Schur functor](lie-theory.md#schur-functor)
- [Schur module](lie-theory.md#schur-module)
- [Section of a vector bundle](fiber-bundle.md#section-of-a-vector-bundle)
- [Seminorm](topological-vector-space.md#seminorm)
- [Sequence space](#sequence-space)
- [Similarity classification of idempotent linear maps](#similarity-classification-of-idempotent-linear-maps)
- [Singular endomorphism has a nonzero two-sided annihilator](algebra.md#singular-endomorphism-has-a-nonzero-two-sided-annihilator)
- [Solution space of a homogeneous linear differential equation](differential-equation.md#solution-space-of-a-homogeneous-linear-differential-equation)
- [Spanning set](#spanning-set)
- [Splitting criterion for a cyclic algebra](associative-algebra.md#splitting-criterion-for-a-cyclic-algebra)
- [Square-class group of a field](galois-theory.md#square-class-group-of-a-field)
- [Square matrix](#square-matrix)
- [Standard basis](#standard-basis)
- [Steinitz exchange lemma](#steinitz-exchange-lemma)
- [Super vector space](commutative-algebra.md#super-vector-space)
- [Symmetric bilinear diagonal-parallel lemma](linear-algebra.md#symmetric-bilinear-diagonal-parallel-lemma)
- [Symplectic group over a field](symplectic-geometry.md#symplectic-group-over-a-field)
- [Tangent space](differential-geometry.md#tangent-space)
- [Tensor algebra](linear-algebra.md#tensor-algebra)
- [Tensor product](linear-algebra.md#tensor-product)
- [Tensor-product basis](linear-algebra.md#tensor-product-basis)
- [Topological vector space](topological-vector-space.md)
- [Topology determines norm equivalence](functional-analysis.md#topology-determines-norm-equivalence)
- [Total weight of a full-support binary linear code](coding-theory.md#total-weight-of-a-full-support-binary-linear-code)
- [Translation (geometry)](geometry-and-topology.md#translation-geometry)
- [Triangular decomposition of a Lie algebra](semisimple-lie-algebra.md#triangular-decomposition-of-a-lie-algebra)
- [Union of three incomparable nonprime ideals](commutative-algebra.md#union-of-three-incomparable-nonprime-ideals)
- [Universal property of a tensor product](linear-algebra.md#universal-property-of-a-tensor-product)
- [VC dimension of a vector space](foundations-of-mathematics.md#vc-dimension-of-a-vector-space)
- [Vector](#vector)
- [Vector-space freeness from maximal independence](module-theory.md#vector-space-freeness-from-maximal-independence)
- [Vector space of univariate polynomials](polynomial.md#vector-space-of-univariate-polynomials)
- [Vector space over the rational numbers](#vector-space-over-the-rational-numbers)
- [Vector subspace](#vector-subspace)
- [Vector-valued function](function.md#vector-valued-function)
- [Vertex operator algebra](algebra.md#vertex-operator-algebra)
- [Zero vector](#zero-vector)
