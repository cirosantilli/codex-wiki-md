# Hilbert space

↑ **Parent:** [Functional analysis](functional-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert_space)

A Hilbert space is a real or complex [inner product space](linear-algebra.md#inner-product-space) that is [complete](topological-analysis.md#completeness) in the [norm](functional-analysis.md#norm) $\|v\|=\sqrt{\langle v,v\rangle}$. Completeness means that every [Cauchy sequence](real-analysis.md#cauchy-sequence) has a [limit](calculus.md#limit-of-a-function) in the space: if its terms become arbitrarily close in this [norm](functional-analysis.md#norm), they converge to an allowed [vector](vector-space.md#vector). The [inner product](linear-algebra.md#inner-product) supplies lengths and [orthogonality](linear-algebra.md#orthogonal-vectors); completeness ensures that limiting approximation procedures do not leave the space.

Finite-dimensional Euclidean spaces are examples, but the same geometry also works for [sequences](real-analysis.md#sequence) and [functions](function.md). In the [l2 sequence space](banach-space.md#l2-sequence-space),

$$
\langle u,v\rangle=\sum_{n=1}^{\infty}u_n\overline{v_n},\qquad
\|u\|^2=\sum_{n=1}^{\infty}|u_n|^2.
$$

In the [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) on $[-1,1]$ with Lebesgue measure,

$$
\langle f,g\rangle=\int_{-1}^{1}f(x)\overline{g(x)}\,dx,\qquad
\|f\|^2=\int_{-1}^{1}|f(x)|^2\,dx.
$$

These formulas use the convention linear in the first argument. Elements of the [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) are equivalence classes of [square-integrable functions](measure-theory.md#square-integrable-function) agreeing [almost everywhere](measure-theory.md#almost-everywhere), so zero distance really identifies the same element. A [vector](vector-space.md#vector) can therefore be a whole [function](function.md), and its squared length can measure an integrated squared error.

For example, approximating $f(x)=x^2$ by $a+bx$ is a nearest-point problem in this [Hilbert space](hilbert-space.md). The allowed approximations form the [linear span](vector-space.md#linear-span) of $1,x$, and the [orthogonal projection](#orthogonal-projection) is the constant $1/3$. Its residual $x^2-1/3$ is [orthogonal](linear-algebra.md#orthogonal-vectors) to both allowed directions because its [integral](calculus.md#integral) and its [inner product](linear-algebra.md#inner-product) with $x$ vanish. The geometry therefore identifies the best approximation without searching through every pair of [coefficients](vector-space.md#coefficient).

This is useful whenever a complicated [vector](vector-space.md#vector) must be represented by a tractable collection of directions. [Fourier series](fourier-series.md) approximate [functions](function.md) with [orthogonal](linear-algebra.md#orthogonal-vectors) oscillations; the [Parseval identity](fourier-analysis.md#parseval-identity) relates the sum of squared [coefficients](vector-space.md#coefficient) to the squared [norm](functional-analysis.md#norm). [Least-squares solutions](inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem) approximate attainable data using a [linear operator](vector-space.md#linear-operator). The [Hilbert projection theorem](#hilbert-projection-theorem) explains why a nearest element exists and is unique for a nonempty [closed convex set](mathematical-optimization.md#closed-convex-set). Distinct application settings share the same geometry of useful components and [orthogonal](linear-algebra.md#orthogonal-vectors) residuals. Casey Rodriguez's MIT lectures develop these connections between [Hilbert spaces](hilbert-space.md), [Fourier series](fourier-series.md), and nearest-point problems.[Rodriguez, MIT 18.102, lectures 14–17, 2021](https://ocw.mit.edu/courses/18-102-introduction-to-functional-analysis-spring-2021/pages/lecture-notes-and-readings/)

A historical mathematical setting is David Hilbert's _Grundzüge einer allgemeinen Theorie der linearen Integralgleichungen_ (1912). Its preface states that it reprints six communications published during 1904–1910 on [linear integral equations](analysis.md#linear-integral-equation). This provides a concrete source for the integral-equation setting associated with the name, while the abstract definition above incorporates later developments.[Hilbert, Grundzüge einer allgemeinen Theorie der linearen Integralgleichungen, 1912, preface](https://archive.org/details/grundzugeallg00hilbrich)

**Table of contents**

- [Reducing subspace of a Hilbert-space operator](#reducing-subspace-of-a-hilbert-space-operator)
- [Hilbert tensor product](#hilbert-tensor-product)
- [Hardy space of the circle](#hardy-space-of-the-circle)
- [Bargmann-Fock space](#bargmann-fock-space)
- [Norm-compact unit ball criterion](#norm-compact-unit-ball-criterion)
- [Closed subspace of a Hilbert space](#closed-subspace-of-a-hilbert-space)
- [Linear isometry of Hilbert spaces](#linear-isometry-of-hilbert-spaces)
  - [Unitary extension of a finite-dimensional isometry](#unitary-extension-of-a-finite-dimensional-isometry)
- [N-term approximation](#n-term-approximation)
  - [Best N-term approximation](#best-n-term-approximation)
    - [Best N-term wavelet approximation of piecewise Hölder functions](#best-n-term-wavelet-approximation-of-piecewise-holder-functions)
  - [Linear N-term approximation](#linear-n-term-approximation)
- [Hilbert space completion](#hilbert-space-completion)
  - [Mean-square completion of trigonometric polynomials](#mean-square-completion-of-trigonometric-polynomials)
- [Separable Hilbert space](#separable-hilbert-space)
- [Hilbert projection theorem](#hilbert-projection-theorem)
  - [Orthogonal decomposition by a closed subspace](#orthogonal-decomposition-by-a-closed-subspace)
    - [Orthogonal complement](#orthogonal-complement)
      - [Double orthogonal complement](#double-orthogonal-complement)
    - [Orthogonal projection](#orthogonal-projection)
      - [Directed subspace angle](#directed-subspace-angle)
        - [Complementarity from two directed subspace angles](#complementarity-from-two-directed-subspace-angles)
      - [Smallest angle between two subspaces](#smallest-angle-between-two-subspaces)
        - [Kitaev geometrical lemma](#kitaev-geometrical-lemma)
      - [Powers of a product of two orthogonal projections](#powers-of-a-product-of-two-orthogonal-projections)
- [Riesz representation theorem](#riesz-representation-theorem)
  - [Kernel-orthogonal proof of the Riesz representation theorem](#kernel-orthogonal-proof-of-the-riesz-representation-theorem)
  - [Adjoint operator](#adjoint-operator)
    - [Adjoint in weighted coordinates](#adjoint-in-weighted-coordinates)
    - [Adjoint of a densely defined operator](#adjoint-of-a-densely-defined-operator)
    - [Adjoint of a commutator](#adjoint-of-a-commutator)
    - [Symmetric operator](#symmetric-operator)
      - [Two-endpoint symmetric derivative has whole complex spectrum](#two-endpoint-symmetric-derivative-has-whole-complex-spectrum)
    - [Image-kernel orthogonality for an adjoint](#image-kernel-orthogonality-for-an-adjoint)
    - [Invertibility from lower bounds on an operator and its adjoint](#invertibility-from-lower-bounds-on-an-operator-and-its-adjoint)
    - [Hermitian conjugation](#hermitian-conjugation)
    - [Formal adjoint](#formal-adjoint)
      - [Boundary terms exclude formal adjoint eigenvectors](#boundary-terms-exclude-formal-adjoint-eigenvectors)
      - [Adjoint reciprocity for a weighted Helmholtz operator](#adjoint-reciprocity-for-a-weighted-helmholtz-operator)
      - [Complete boundary-jet condition for formal adjoints](#complete-boundary-jet-condition-for-formal-adjoints)
    - [Hermitian operator](#hermitian-operator)
      - [Hermitian quadratic form](#hermitian-quadratic-form)
      - [Hermitian part of a matrix](#hermitian-part-of-a-matrix)
      - [Determinant of Hermitian congruence](#determinant-of-hermitian-congruence)
      - [Positive operator](#positive-operator)
        - [Positive definite symmetric operator](#positive-definite-symmetric-operator)
          - [Quadratic variational principle for a symmetric positive operator](#quadratic-variational-principle-for-a-symmetric-positive-operator)
            - [Symmetric part determines a real quadratic functional](#symmetric-part-determines-a-real-quadratic-functional)
          - [Uniformly positive definite symmetric operator](#uniformly-positive-definite-symmetric-operator)
        - [Positive contraction](#positive-contraction)
        - [Support of a positive operator](#support-of-a-positive-operator)
        - [Positive square root of an operator](#positive-square-root-of-an-operator)
      - [Positive-negative decomposition of a Hermitian operator](#positive-negative-decomposition-of-a-hermitian-operator)
        - [Negative part of a Hermitian operator](#negative-part-of-a-hermitian-operator)
        - [Positive part of a Hermitian operator](#positive-part-of-a-hermitian-operator)
      - [Löwner order](#lowner-order)
        - [Operator monotonicity of the square root](#operator-monotonicity-of-the-square-root)
    - [Adjoint criterion for an invariant orthogonal complement](#adjoint-criterion-for-an-invariant-orthogonal-complement)
    - [Normal operator](#normal-operator)
      - [Normal spectrum equals approximate point spectrum](#normal-spectrum-equals-approximate-point-spectrum)
      - [Spectral theorem](#spectral-theorem)
        - [Spectral theorem for normal operators](#spectral-theorem-for-normal-operators)
          - [Finite commuting normal operators have joint spectral projections](#finite-commuting-normal-operators-have-joint-spectral-projections)
          - [Spectral matrix functional calculus](#spectral-matrix-functional-calculus)
          - [Spectral theorem for normal operators on a separable Hilbert space](#spectral-theorem-for-normal-operators-on-a-separable-hilbert-space)
            - [Weyl-von Neumann theorem](#weyl-von-neumann-theorem)
              - [Classification of separable self-adjoint operators modulo compacts](#classification-of-separable-self-adjoint-operators-modulo-compacts)
            - [Projection-valued measure](#projection-valued-measure)
              - [Cyclic multiplication model for a normal operator](#cyclic-multiplication-model-for-a-normal-operator)
              - [Scalar-measure construction of a projection-valued measure](#scalar-measure-construction-of-a-projection-valued-measure)
              - [Spectral theorem for a commutative operator algebra](#spectral-theorem-for-a-commutative-operator-algebra)
                - [Full support of a faithful spectral measure](#full-support-of-a-faithful-spectral-measure)
              - [Spectral projector](#spectral-projector)
            - [Spectral measure of a normal operator](#spectral-measure-of-a-normal-operator)
              - [Spectral projection gives a reducing subspace](#spectral-projection-gives-a-reducing-subspace)
              - [Scalar spectral measure](#scalar-spectral-measure)
                - [Weak convergence of scalar spectral measures](#weak-convergence-of-scalar-spectral-measures)
              - [Stone formula](#stone-formula)
- [Weak convergence in a Hilbert space](#weak-convergence-in-a-hilbert-space)
  - [Weak Banach–Saks theorem in a Hilbert space](#weak-banach-saks-theorem-in-a-hilbert-space)
  - [Coordinate criterion for weak convergence in a separable Hilbert space](#coordinate-criterion-for-weak-convergence-in-a-separable-hilbert-space)
  - [Weak subsequence of a bounded Hilbert-space sequence](#weak-subsequence-of-a-bounded-hilbert-space-sequence)
  - [Weak lower semicontinuity of the Hilbert norm](#weak-lower-semicontinuity-of-the-hilbert-norm)
  - [Radon-Riesz theorem](#radon-riesz-theorem)
    - [Uniform basis-tail criterion for strong convergence](#uniform-basis-tail-criterion-for-strong-convergence)
  - [Weakly null orthonormal sequence](#weakly-null-orthonormal-sequence)
  - [Mazur's lemma](#mazur-s-lemma)
    - [Mazur theorem](#mazur-theorem)
  - [Norm-closed convex set is weakly closed](#norm-closed-convex-set-is-weakly-closed)
- [Orthonormal sequence](#orthonormal-sequence)
  - [Hilbertian basis](#hilbertian-basis)
    - [Parseval identity for a Hilbertian basis](#parseval-identity-for-a-hilbertian-basis)
  - [Bessel's inequality](#bessel-s-inequality)

## Reducing subspace of a Hilbert-space operator

↑ **Parent:** [Hilbert space](hilbert-space.md)

A [closed](topology.md#closed-set) subspace of a [Hilbert space](hilbert-space.md) reduces a [bounded operator](topological-vector-space.md#continuous-linear-operator) when both the operator and its adjoint leave the subspace invariant. Equivalently, the [orthogonal](linear-algebra.md#orthogonal-vectors) projection onto it commutes with the operator: the adjoint invariance makes its [orthogonal complement](#orthogonal-complement) invariant too. For a star-closed algebra of operators, the [closed](topology.md#closed-set) span of the orbit of any [vector](vector-space.md#vector) is reducing for the whole algebra. This enables an [orthogonal](linear-algebra.md#orthogonal-vectors) direct-sum decomposition into cyclic actions when constructing [Borel functional calculus for a normal operator](banach-algebra.md#borel-functional-calculus-for-a-normal-operator).

## Hilbert tensor product

↑ **Parent:** [Hilbert space](hilbert-space.md)

The Hilbert tensor product is the completion of the algebraic [tensor product](linear-algebra.md#tensor-product) of [Hilbert spaces](hilbert-space.md) with $\langle u\otimes v,u'\otimes v'\rangle=\langle u,u'\rangle\langle v,v'\rangle$, extended sesquilinearly. Orthonormal bases identify this inner product with the Euclidean inner product on coefficient arrays, proving positivity. In particular, $\langle u^{\otimes m},v^{\otimes m}\rangle=\langle u,v\rangle^m$ and $\|u^{\otimes m}\|=\|u\|^m$. These identities turn scalar [power series](real-analysis.md#power-series) into vector embeddings, as in the proof of the [Grothendieck inequality](linear-algebra.md#grothendieck-inequality).

## Hardy space of the circle

↑ **Parent:** [Hilbert space](hilbert-space.md)

The Hardy space of the circle is the closed subspace of [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) whose negative [Fourier coefficients](fourier-series.md#fourier-coefficient) vanish. The [orthogonal projection](#orthogonal-projection) onto it is denoted $P_+$. A continuous symbol $f$ defines a [Toeplitz operator](finite-difference.md#toeplitz-operator) $T_f=P_+M_f|_{H^2}$. For continuous $f,g$, $T_fT_g-T_{fg}$ is compact: it is finite rank for Laurent polynomials, and uniform approximation extends the result.

## Bargmann-Fock space

↑ **Parent:** [Hilbert space](hilbert-space.md)

The Bargmann-Fock space is a [Hilbert space](hilbert-space.md) of entire [holomorphic functions](complex-analysis.md#holomorphic-function) with Gaussian-weighted area inner product. If $f(z)=\sum a_nz^n$, angular integration and the [Gaussian integral](calculus.md#gaussian-integral) give $\|f\|^2=\sum n!|a_n|^2$. Conversely any such square-summable coefficient sequence defines an entire function, since $\sum|a_nz^n|\leq(\sum n!|a_n|^2)^{1/2}e^{|z|^2/2}$. This proves completeness and shows that $z^n/\sqrt{n!}$ is an [orthonormal basis](linear-algebra.md#orthonormal-basis). The same bound shows boundedness of evaluation and gives reproducing kernel $e^{z\bar w}$.

## Norm-compact unit ball criterion

↑ **Parent:** [Hilbert space](hilbert-space.md)

The closed [unit ball](functional-analysis.md#unit-ball) of a [Hilbert space](hilbert-space.md) is compact in norm exactly when the space is finite-dimensional. Finite-dimensional compactness follows from the [Heine-Borel theorem](topology.md#heine-borel-theorem). In infinite dimension, an [orthonormal sequence](#orthonormal-sequence) has pairwise distance $\sqrt2$ and no convergent subsequence. Restricting a [compact operator](compact-operator.md) that equals a nonzero multiple of the identity on a subspace therefore forces that subspace to be finite-dimensional.

## Closed subspace of a Hilbert space

↑ **Parent:** [Hilbert space](hilbert-space.md)

A [vector subspace](vector-space.md#vector-subspace) closed in the [norm topology](functional-analysis.md#norm-topology) of a [Hilbert space](hilbert-space.md) is complete in the inherited [norm](functional-analysis.md#norm) and [inner product](linear-algebra.md#inner-product). Its [orthogonal complement](#orthogonal-complement) gives a decomposition of the ambient [Hilbert space](hilbert-space.md) into an [orthogonal direct sum](vector-space.md#orthogonal-direct-sum). This closedness permits [orthogonal projection](#orthogonal-projection) and ensures limits used in range arguments remain in the subspace. Every finite-dimensional [vector subspace](vector-space.md#vector-subspace) is closed.

## Linear isometry of Hilbert spaces

↑ **Parent:** [Hilbert space](hilbert-space.md)

A linear map $V:\mathcal H\to\mathcal K$ is an isometry when it preserves inner products, equivalently $V^\dagger V=I$. It need not be surjective. It maps an [orthonormal basis](linear-algebra.md#orthonormal-basis) to an orthonormal family, and $\rho\mapsto V\rho V^\dagger$ preserves the nonzero [eigenvalues](linear-operator-theory.md#eigenvalue) and the [Von Neumann entropy](von-neumann-entropy.md) of a [density operator](quantum-theory.md#density-matrix).

### Unitary extension of a finite-dimensional isometry

↑ **Parent:** [Linear isometry of Hilbert spaces](#linear-isometry-of-hilbert-spaces)

A [linear isometry](#linear-isometry-of-hilbert-spaces) from a subspace of a finite-dimensional [Hilbert space](hilbert-space.md) into the same ambient space extends to a [unitary operator](vector-space.md#unitary-operator). Complete an [orthonormal basis](linear-algebra.md#orthonormal-basis) of the input subspace and its isometric image to full [orthonormal bases](linear-algebra.md#orthonormal-basis), then map the first to the second. The equal complement dimensions make this possible. Orthogonality of the specified image columns, not normalization alone, is essential. In an infinite-dimensional space arbitrary isometries need not be surjective; the finite-dimensional same-space hypothesis cannot be dropped.

## N-term approximation

↑ **Parent:** [Hilbert space](hilbert-space.md)

An N-term approximation in an [orthonormal basis](linear-algebra.md#orthonormal-basis) uses at most $N$ basis functions. For a chosen index set $\Lambda$, its optimal coefficients are the [inner products](linear-algebra.md#inner-product) with those functions, and its squared error is the sum of the omitted squared coefficients by the [Parseval identity](fourier-analysis.md#parseval-identity).

### Best N-term approximation

↑ **Parent:** [N-term approximation](#n-term-approximation)

The best N-term approximation in an [orthonormal basis](linear-algebra.md#orthonormal-basis) retains $N$ coefficients of greatest absolute value. It minimizes the squared [Hilbert space](hilbert-space.md) error over all index sets of size at most $N$. The selection makes the approximation nonlinear in the data, even though coefficient extraction is linear.

<h4 id="best-n-term-wavelet-approximation-of-piecewise-holder-functions">Best N-term wavelet approximation of piecewise Hölder functions</h4>

↑ **Parent:** [Best N-term approximation](#best-n-term-approximation)

For a bounded [function](function.md) on an interval with finitely many jumps and piecewise $C^\alpha$ bounds, localized [orthonormal wavelets](fourier-analysis.md#orthonormal-wavelet) with sufficient [vanishing moments](fourier-analysis.md#vanishing-moment) give squared [best N-term approximation](#best-n-term-approximation) error $O(N^{-2\alpha})$. There are $O(2^j)$ smooth-region coefficients of size $O(2^{-j(\alpha+1/2)})$, and only $O(K)$ jump-crossing coefficients of size $O(2^{-j/2})$ per level. Retain all coefficients through level $J$ and the jump-crossing coefficients through $L=\lceil2\alpha J\rceil$ when $\alpha>1/2$. This costs $O(2^J+KJ)$ and leaves squared tails $O(2^{-2\alpha J}+2^{-L})$. Choosing $2^J$ comparable to $N$ proves the rate by the [Parseval identity](fourier-analysis.md#parseval-identity).

### Linear N-term approximation

↑ **Parent:** [N-term approximation](#n-term-approximation)

A linear N-term approximation fixes its index set independently of the approximated function. Wavelet approximation normally orders by increasing resolution, whereas [Fourier series](fourier-series.md) approximation normally keeps the lowest frequencies. An arbitrary reordering can change or destroy a claimed convergence rate.

## Hilbert space completion

↑ **Parent:** [Hilbert space](hilbert-space.md)

The Hilbert space completion of an [inner product space](linear-algebra.md#inner-product-space) $V$ is a [Hilbert space](hilbert-space.md) containing an isometric dense copy of $V$. It can be constructed from [Cauchy sequences](real-analysis.md#cauchy-sequence) in $V$, identifying two sequences when the norm of their difference tends to zero.

The space of [finitely supported sequences](banach-space.md#finitely-supported-sequence) with the [l2 sequence space](banach-space.md#l2-sequence-space) [norm](functional-analysis.md#norm) illustrates the need for completion. Let $u^{(n)}=(1,1/2,\ldots,1/n,0,\ldots)$. For $m>n$,

$$
\|u^{(m)}-u^{(n)}\|_2^2=\sum_{k=n+1}^{m}\frac1{k^2}\leq\int_n^{\infty}\frac{dx}{x^2}=\frac1n.
$$

This is a [Cauchy sequence](real-analysis.md#cauchy-sequence), but its coordinatewise [limit](calculus.md#limit-of-a-function) $(1/k)_{k\geq1}$ is not finitely supported. It belongs to the [l2 sequence space](banach-space.md#l2-sequence-space), which is the completion. The same construction permits infinitely many small components while controlling their total squared size. An infinite [orthonormal basis](linear-algebra.md#orthonormal-basis) of a [Hilbert space](hilbert-space.md) consequently permits norm-convergent series; a [Hamel basis](vector-space.md#basis) represents each [vector](vector-space.md#vector) by a finite sum, so these two uses of "basis" must be distinguished.

### Mean-square completion of trigonometric polynomials

↑ **Parent:** [Hilbert space completion](#hilbert-space-completion)

Start with finite real linear combinations of $1$, $\cos(\lambda x)$ and $\sin(\lambda x)$ with arbitrary positive real frequencies, and use the [inner product](linear-algebra.md#inner-product) $\langle f,g\rangle_M=\lim_{R\to\infty}R^{-1}\int_{-R}^Rfg$. Product-to-sum identities give existence of these averages and mutual [orthogonality](linear-algebra.md#orthogonal-vectors) of distinct frequencies. The squared [norm](functional-analysis.md#norm) is $2a_0^2+\sum_\lambda(a_\lambda^2+b_\lambda^2)$. Its [Hilbert space completion](#hilbert-space-completion) contains an uncountable [orthonormal set](linear-algebra.md#orthonormal-set), so is not a [separable Hilbert space](#separable-hilbert-space). This construction does not equip all [locally square-integrable functions](measure-theory.md#locally-square-integrable-function) with an [inner product](linear-algebra.md#inner-product): compactly supported nonzero functions have zero mean square, and other functions have divergent or nonexistent averages.

## Separable Hilbert space

↑ **Parent:** [Hilbert space](hilbert-space.md)

A Hilbert space is separable when it has a countable dense subset, equivalently a countable [Hilbertian basis](#hilbertian-basis).

## Hilbert projection theorem

↑ **Parent:** [Hilbert space](hilbert-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert_projection_theorem)

For every nonempty [closed convex set](mathematical-optimization.md#closed-convex-set) $C$ in a [Hilbert space](hilbert-space.md) and every $x$ in that space, there is a unique $p\in C$ satisfying

$$
\|x-p\|=\inf_{z\in C}\|x-z\|.
$$

Closedness and completeness let a limiting approximation attain the infimum; [convexity](real-analysis.md#convex-function) prevents two different minimizers. The proof idea is to choose a sequence approaching the infimum. The [parallelogram identity](linear-algebra.md#parallelogram-law) and the admissible midpoint make it a [Cauchy sequence](real-analysis.md#cauchy-sequence); applying the same identity to two putative minimizers proves uniqueness.

For a [closed subspace of a Hilbert space](#closed-subspace-of-a-hilbert-space), this nearest-point map is an [orthogonal projection](#orthogonal-projection) and is [linear](vector-space.md#linearity). For a general [closed convex set](mathematical-optimization.md#closed-convex-set) it need not be [linear](vector-space.md#linearity): projecting the real line onto $[0,1]$ clips values below zero to zero and values above one to one. The theorem is therefore useful for both linear approximation and constrained nearest-point problems.[Rodriguez, MIT 18.102, lecture 17: minimizers and orthogonal complements](https://ocw.mit.edu/courses/18-102-introduction-to-functional-analysis-spring-2021/resources/18102-sp21-lecture-17/)

Closedness is essential even in familiar examples. For the open [interval](real-analysis.md#interval-mathematics) $(0,1)\subseteq\mathbb R$ and $x=0$, the distance infimum is zero but no nearest point exists. The same obstruction appears when approximating $(1/k)_{k\geq1}$ by [finitely supported sequences](banach-space.md#finitely-supported-sequence): the infimum is zero, but the limit lies outside that subspace until we take its [Hilbert space completion](#hilbert-space-completion).

### Orthogonal decomposition by a closed subspace

↑ **Parent:** [Hilbert projection theorem](#hilbert-projection-theorem)

For a closed subspace $F$ of a Hilbert space,

$$
H=F\oplus F^\perp.
$$

The closest point $P_Fx$ gives the first component, and differentiating $\|x-P_Fx-tu\|^2$ at zero shows that the remainder is orthogonal to every $u\in F$.

#### Orthogonal complement

↑ **Parent:** [Orthogonal decomposition by a closed subspace](#orthogonal-decomposition-by-a-closed-subspace)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orthogonal_complement)

The orthogonal complement of a subset $F$ of an inner-product space is

$$
F^\perp=\{x:\langle x,y\rangle=0\text{ for every }y\in F\}.
$$

##### Double orthogonal complement

↑ **Parent:** [Orthogonal complement](#orthogonal-complement)

For a linear subspace $F$ of a [Hilbert space](hilbert-space.md),

$$
F^{\perp\perp}=\overline F.
$$

Thus $F=F^{\perp\perp}$ exactly when $F$ is closed.

#### Orthogonal projection

↑ **Parent:** [Orthogonal decomposition by a closed subspace](#orthogonal-decomposition-by-a-closed-subspace)

The orthogonal projection $P_F$ onto a [closed subspace of a Hilbert space](#closed-subspace-of-a-hilbert-space) $F$ sends $x$ to its component in the [orthogonal decomposition](#orthogonal-decomposition-by-a-closed-subspace)

$$
x=P_Fx+r,\qquad P_Fx\in F,\quad r\in F^\perp.
$$

The residual $r$ is [orthogonal](linear-algebra.md#orthogonal-vectors) to every permitted direction. For any $z\in F$, the [Pythagorean theorem](geometry-and-topology.md#pythagorean-theorem) gives

$$
\|x-z\|^2=\|r\|^2+\|P_Fx-z\|^2.
$$

Thus $P_Fx$ uniquely minimizes the distance to $F$. It is a [linear map](vector-space.md#linear-map), is idempotent, and is [nonexpansive](convex-optimization.md#nonexpansive-mapping): $\|P_Fx-P_Fy\|\leq\|x-y\|$; taking $y=0$ gives $\|P_Fx\|\leq\|x\|$.

In $\mathbb R^2$, project $v=(1,3)$ onto the line spanned by $u=(2,1)$. The [inner product](linear-algebra.md#inner-product) gives

$$
P_Fv=\frac{\langle v,u\rangle}{\langle u,u\rangle}u
=\frac55u=(2,1),\qquad r=(-1,2).
$$

The check $\langle r,u\rangle=-2+2=0$ confirms orthogonality, and $\|v\|^2=10=5+5=\|P_Fv\|^2+\|r\|^2$. Projecting again changes nothing, since the result already lies on the line.

<a id="image-orthogonal-projection-gives-the-unique-nearest-point-on-a-line-and-a-perpendicular-residual"></a>
![](orthogonal-projection-geometry.png)

**[Figure 1](#image-orthogonal-projection-gives-the-unique-nearest-point-on-a-line-and-a-perpendicular-residual). Orthogonal projection gives the unique nearest point on a line and a perpendicular residual**.

For a finite [orthonormal basis](linear-algebra.md#orthonormal-basis) $e_1,\ldots,e_m$ of $F$, the same operation is $P_Fx=\sum_j\langle x,e_j\rangle e_j$, using the convention linear in the first argument. Replacing coordinate [vectors](vector-space.md#vector) by [functions](function.md) gives exactly the same approximation principle. For $f(x)=x^2$ in the real [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) on $[-1,1]$ and $F=\operatorname{span}\{1,x\}$, the directions are [orthogonal](linear-algebra.md#orthogonal-vectors), with squared [norms](functional-analysis.md#norm) $2$ and $2/3$. Their [inner products](linear-algebra.md#inner-product) with $f$ are $2/3$ and zero, so

$$
P_Ff=\frac{2/3}{2}\cdot1+\frac0{2/3}\cdot x=\frac13.
$$

Direct integration gives the squared error $\|x^2-1/3\|^2=8/45$. For any competing affine [polynomial](polynomial.md), the [orthogonal](linear-algebra.md#orthogonal-vectors) residual yields

$$
\int_{-1}^{1}\bigl(x^2-a-bx\bigr)^2\,dx
=\frac8{45}+2\left(a-\frac13\right)^2+\frac23b^2.
$$

Every deviation from $a=1/3$, $b=0$ adds a nonnegative error. The best [function](function.md) need not pass through any selected data point: it minimizes an integrated error across the whole [interval](real-analysis.md#interval-mathematics).

<a id="image-projecting-x-squared-onto-affine-functions-gives-the-constant-one-third-and-minimum-integrated-squared-error-8-45"></a>
![](hilbert-function-approximation.png)

**[Figure 2](#image-projecting-x-squared-onto-affine-functions-gives-the-constant-one-third-and-minimum-integrated-squared-error-8-45). Projecting x squared onto affine functions gives the constant one third and minimum integrated squared error 8/45**.

##### Directed subspace angle

↑ **Parent:** [Orthogonal projection](#orthogonal-projection)

For a nonzero [closed subspace of a Hilbert space](#closed-subspace-of-a-hilbert-space) $V$ and a [closed subspace of a Hilbert space](#closed-subspace-of-a-hilbert-space) $W$, this angle measures the worst loss under projection from $V$ to $W$. Its positive cosine is a uniform lower bound for $P_W|_V$. The order of the subspaces matters in general. This is distinct from the [smallest angle between two subspaces](#smallest-angle-between-two-subspaces), whose cosine is a supremum. For equal finite dimensions the cosine is the smallest [singular value](linear-algebra.md#singular-value) of the cross [Gram matrix](linear-algebra.md#gram-matrix) of [orthonormal bases](linear-algebra.md#orthonormal-basis). When $V$ is zero, the infimum is over an empty unit sphere and does not define an angle in $[0,\pi/2]$; use a lower-bound formulation instead.

###### Complementarity from two directed subspace angles

↑ **Parent:** [Directed subspace angle](#directed-subspace-angle)

For [closed subspaces of a Hilbert space](#closed-subspace-of-a-hilbert-space), set $T=P_{V^\perp}|_W$. The two positive cosines bound $T$ and its [adjoint operator](#adjoint-operator) $P_W|_{V^\perp}$ below. The first bound gives a closed range and [injectivity](algebra.md#injective-function); the second makes the range dense by [image-kernel orthogonality for an adjoint](#image-kernel-orthogonality-for-an-adjoint). Thus $T$ is a bounded bijection, and $w=T^{-1}P_{V^\perp}f$ yields the unique [direct sum](vector-space.md#direct-sum) decomposition $f=w+v$. In equal finite dimensions, a lower bound on $T$ alone suffices by the [rank-nullity theorem](linear-algebra.md#rank-nullity-theorem).

##### Smallest angle between two subspaces

↑ **Parent:** [Orthogonal projection](#orthogonal-projection)

For two finite-dimensional subspaces with projections $P,Q$, define $\cos\vartheta=\sup_{\|u\|=\|v\|=1}|\langle u,v\rangle|=\|PQ\|$, with vectors drawn from the respective subspaces. The angle is zero when they intersect nontrivially. To measure separation after removing a common intersection, restrict both subspaces to its orthogonal complement. The resulting angle controls sums of [positive operators](#positive-operator) in the [Kitaev geometrical lemma](#kitaev-geometrical-lemma).

###### Kitaev geometrical lemma

↑ **Parent:** [Smallest angle between two subspaces](#smallest-angle-between-two-subspaces)

Suppose [positive operators](#positive-operator) $A,B$ have positive [eigenvalues](linear-operator-theory.md#eigenvalue) at least $\gamma$ and their nullspaces meet only at zero. If $\vartheta$ is their [smallest angle between two subspaces](#smallest-angle-between-two-subspaces), then $A+B\geq2\gamma\sin^2(\vartheta/2)I$. Indeed $A+B\geq\gamma(2I-P-Q)$, while $(P+Q)^2\leq(1+\cos\vartheta)(P+Q)$ gives $P+Q\leq(1+\cos\vartheta)I$. With a common nullspace, apply the same proof on its orthogonal complement to bound the positive [spectral gap](linear-operator-theory.md#spectral-gap).

##### Powers of a product of two orthogonal projections

↑ **Parent:** [Orthogonal projection](#orthogonal-projection)

For [orthogonal projections](#orthogonal-projection) $P,Q$ with $\|PQ\|\leq q<1$, the identity $(PQ)^r=PQ(QPQ)^{r-1}$ and $\|QPQ\|=\|PQ\|^2$ imply $\|(PQ)^r\|\leq q^{2r-1}$ for $r\geq1$. When the projections have a common fixed subspace, first remove its [orthogonal projection](#orthogonal-projection). This estimate is stronger than generic submultiplicativity and is useful for alternating local projection layers.

## Riesz representation theorem

↑ **Parent:** [Hilbert space](hilbert-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riesz_representation_theorem)

Every bounded linear functional on a Hilbert space is inner product with one unique vector, with equal norms.

### Kernel-orthogonal proof of the Riesz representation theorem

↑ **Parent:** [Riesz representation theorem](#riesz-representation-theorem)

For a nonzero bounded functional $f$ on a Hilbert space, choose nonzero $z\in(\ker f)^\perp$. Then

$$
x-\frac{f(x)}{f(z)}z\in\ker f
$$

implies $f(x)=\langle x,f(z)z/\lVert z\rVert^2\rangle$ in the real case. Cauchy-Schwarz and evaluation on the representing vector give equality of the two norms.

### Adjoint operator

↑ **Parent:** [Riesz representation theorem](#riesz-representation-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Adjoint_operator)

For a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) $T:H\to K$ between real or complex [Hilbert spaces](hilbert-space.md), its adjoint is the unique [bounded linear operator](topological-vector-space.md#continuous-linear-operator) $T^*:K\to H$ satisfying

$$
\langle Tx,y\rangle_K=\langle x,T^*y\rangle_H\qquad(x\in H,\ y\in K).
$$

The [inner product](linear-algebra.md#inner-product) here is linear in its first argument. The [adjoint operator](#adjoint-operator) transfers an output measurement back to the input: measuring $Tx$ against the [vector](vector-space.md#vector) $y$ gives exactly the same scalar as measuring $x$ against $T^*y$. It depends on both [inner products](linear-algebra.md#inner-product).

<a id="image-the-adjoint-transfers-a-measurement-direction-while-preserving-its-measured-value"></a>
![](adjoint-operator-pairing.png)

**[Figure 3](#image-the-adjoint-transfers-a-measurement-direction-while-preserving-its-measured-value). The adjoint transfers a measurement direction while preserving its measured value**.

In this real example,

$$
A=\begin{pmatrix}2&1\\0&1\end{pmatrix},\quad x=\begin{pmatrix}1\\1\end{pmatrix},\quad y=\begin{pmatrix}1\\0\end{pmatrix},\quad Ax=\begin{pmatrix}3\\1\end{pmatrix},\quad A^*y=\begin{pmatrix}2\\1\end{pmatrix}.
$$

Both [inner products](linear-algebra.md#inner-product) equal $3$. The dashed lines collect all [vectors](vector-space.md#vector) giving that same measurement: the output line $u_1=3$ becomes the input line $2x_1+x_2=3$. The [adjoint operator](#adjoint-operator) therefore moves the direction that describes the measurement. It generally differs from the [inverse matrix](linear-algebra.md#matrix-inverse): here $A^{-1}y=(1/2,0)^{\mathrm T}$.

For an explicitly complex example, use the standard [inner product](linear-algebra.md#inner-product) $\langle u,v\rangle=\sum_j u_j\overline{v_j}$ on $\mathbb C^2$. In the standard [orthonormal basis](linear-algebra.md#orthonormal-basis), the [adjoint operator](#adjoint-operator) is represented by the [conjugate transpose](linear-operator-theory.md#conjugate-transpose):

$$
T=\begin{pmatrix}1&i\\2&1-i\end{pmatrix},\qquad T^*=\begin{pmatrix}1&2\\-i&1+i\end{pmatrix}.
$$

For $x=(1+i,2)^{\mathrm T}$ and $y=(1,i)^{\mathrm T}$, direct [matrix multiplication](vector-space.md#matrix-multiplication) gives

$$
Tx=\begin{pmatrix}1+3i\\4\end{pmatrix},\qquad T^*y=\begin{pmatrix}1+2i\\-1\end{pmatrix},
$$

and hence

$$
\langle Tx,y\rangle=(1+3i)+4(-i)=1-i,\qquad \langle x,T^*y\rangle=(1+i)(1-2i)-2=1-i.
$$

The [complex conjugate](complex-analysis.md#complex-conjugate) is essential to this agreement.

Existence follows from the [Riesz representation theorem](#riesz-representation-theorem): for fixed $y$, the bounded [linear functional](linear-algebra.md#linear-functional) $x\mapsto\langle Tx,y\rangle$ has a unique representing [vector](vector-space.md#vector) $T^*y$. The resulting [adjoint operator](#adjoint-operator) has the same [operator norm](continuous-dual-space.md#operator-norm) as $T$, and

$$
\|T^*\|=\|T\|,\qquad \|T^*T\|=\|T\|^2.
$$

MIT's lecture 18 develops the representation argument and the [conjugate transpose](linear-operator-theory.md#conjugate-transpose) example.[Rodriguez, notes by Andrew Lin, MIT 18.102, lecture 18, Theorem 185 and Example 186, 2021](https://ocw.mit.edu/courses/18-102-introduction-to-functional-analysis-spring-2021/7f23bfc43ee2e1efd238a5384e5b9d51_MIT18_102s21_lec18.pdf)

This transfer explains the [normal equation for a linear inverse problem](inverse-problem.md#normal-equation-for-a-linear-inverse-problem): a [least-squares solution](inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem) has residual $Tx-b$ [orthogonal](linear-algebra.md#orthogonal-vectors) to every attainable direction $Th$, so $\langle h,T^*(Tx-b)\rangle=0$ for every $h$, equivalently $T^*Tx=T^*b$. An output residual becomes an input condition through the same [adjoint operator](#adjoint-operator). All identities in this section concern [bounded operators](topological-vector-space.md#continuous-linear-operator) defined on the whole source [Hilbert space](hilbert-space.md); for a [densely defined operator](vector-space.md#densely-defined-operator) that is not bounded, use the [adjoint of a densely defined operator](#adjoint-of-a-densely-defined-operator) and check its [operator domain](vector-space.md#operator-domain).

#### Adjoint in weighted coordinates

↑ **Parent:** [Adjoint operator](#adjoint-operator)

Suppose a [linear map](vector-space.md#linear-map) between finite-dimensional [Hilbert spaces](hilbert-space.md) has [matrix](vector-space.md#matrix) $A$, and their [inner products](linear-algebra.md#inner-product) in the chosen [bases](vector-space.md#basis) are $\langle x,z\rangle_H=z^*G_Hx$ and $\langle u,v\rangle_K=v^*G_Ku$. The [Gram matrices](linear-algebra.md#gram-matrix) $G_H,G_K$ are [positive-definite matrices](linear-algebra.md#positive-definite-matrix). Writing $A^*=\overline A^{\mathrm T}$ for the ordinary [conjugate transpose](linear-operator-theory.md#conjugate-transpose), the coordinate [matrix](vector-space.md#matrix) of the [adjoint operator](#adjoint-operator) is

$$
[T^*]=G_H^{-1}A^*G_K.
$$

Indeed, the defining [inner product](linear-algebra.md#inner-product) identity says $y^*G_KAx=y^*[T^*]^*G_Hx$ for all $x,y$. Thus simply transposing and conjugating is valid in [orthonormal bases](linear-algebra.md#orthonormal-basis), where both [Gram matrices](linear-algebra.md#gram-matrix) are the [identity matrix](vector-space.md#identity-matrix).

For the [weighted inner product](linear-algebra.md#weighted-inner-product) $\langle x,y\rangle_G=\overline{y_1}x_1+4\overline{y_2}x_2$ and the coordinate swap $A=\begin{pmatrix}0&1\\1&0\end{pmatrix}$, the [adjoint operator](#adjoint-operator) has [matrix](vector-space.md#matrix) $\begin{pmatrix}0&4\\1/4&0\end{pmatrix}$. With $x=(1,0)^{\mathrm T}$ and $y=(0,1)^{\mathrm T}$, both [inner products](linear-algebra.md#inner-product) equal $4$. The coordinate swap is its own ordinary [transpose](vector-space.md#transpose), but is not [self-adjoint](linear-operator-theory.md#self-adjoint-operator) in this [weighted inner product](linear-algebra.md#weighted-inner-product).

#### Adjoint of a densely defined operator

↑ **Parent:** [Adjoint operator](#adjoint-operator)

For a densely defined operator on a [Hilbert space](hilbert-space.md), $h$ belongs to $D(T^*)$ exactly when the functional $f\mapsto\langle Tf,h\rangle$ is bounded in the ambient Hilbert norm on $D(T)$. Density makes its representing vector $T^*h$ unique. Differential expressions alone do not determine this domain.

// Target: analysis.bigb

#### Adjoint of a commutator

↑ **Parent:** [Adjoint operator](#adjoint-operator)

When compositions and adjoints are defined on the common test domain, reversing products gives $[A,B]^*=[B^*,A^*]$. In particular a self-adjoint [Dolbeault Laplacian](complex-geometry.md#dolbeault-laplacian) and the mutually adjoint Lefschetz operators satisfy $[\Delta_{\bar\partial},L]^*=[\Lambda,\Delta_{\bar\partial}]$.

#### Symmetric operator

↑ **Parent:** [Adjoint operator](#adjoint-operator)

A [densely defined operator](vector-space.md#densely-defined-operator) $T$ on a [Hilbert space](hilbert-space.md) is symmetric when

$$
\langle Tv,w\rangle=\langle v,Tw\rangle\qquad(v,w\in D(T)).
$$

Equivalently, $T$ agrees with its [adjoint operator](#adjoint-operator) on $D(T)$, while $D(T^*)$ may be larger. A [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) additionally requires equality of these [operator domains](vector-space.md#operator-domain).

##### Two-endpoint symmetric derivative has whole complex spectrum

↑ **Parent:** [Symmetric operator](#symmetric-operator)

Its adjoint is $if'$ on all of $H^1(0,1)$, with no endpoint conditions. Every complex $\lambda$ is an adjoint eigenvalue, with eigenfunction $e^{-i\lambda x}$. Thus every complex $\lambda$ obstructs surjectivity of $\lambda I-A_0$. The original operator has no eigenvalues because its zero initial value kills any solution of $if'=\lambda f$.

// Target: analysis.bigb

#### Image-kernel orthogonality for an adjoint

↑ **Parent:** [Adjoint operator](#adjoint-operator)

For a [linear map](vector-space.md#linear-map) $T:V\to W$ between finite-dimensional [inner product spaces](linear-algebra.md#inner-product-space),

$$
(\operatorname{im}T)^\perp=\ker T^*,
\qquad
\operatorname{im}T=(\ker T^*)^\perp.
$$

The first equality follows directly from the defining identity for the [adjoint operator](#adjoint-operator); the second follows by taking [orthogonal complements](#orthogonal-complement). In an infinite-dimensional [Hilbert space](hilbert-space.md), the second equality generally requires closure of the image.

#### Invertibility from lower bounds on an operator and its adjoint

↑ **Parent:** [Adjoint operator](#adjoint-operator)

A bounded operator $T$ on a Hilbert space is invertible exactly when both $T$ and $T^*$ are bounded below. A lower bound on $T$ makes it injective with closed range, while a lower bound on $T^*$ gives $\ker T^*=0$ and hence dense range through

$$
(\operatorname{ran}T)^\perp=\ker T^*.
$$

Closed dense range is the whole space, and the lower bound controls the inverse.

#### Hermitian conjugation

↑ **Parent:** [Adjoint operator](#adjoint-operator)

Hermitian conjugation is the operation of taking the [adjoint operator](#adjoint-operator), written $T^\dagger=T^*$. For a [matrix](vector-space.md#matrix) in [orthonormal bases](linear-algebra.md#orthonormal-basis), it takes the [complex conjugate](complex-analysis.md#complex-conjugate) of each entry and exchanges rows with columns:

$$
(A^\dagger)_{jk}=\overline{A_{kj}},\qquad A^\dagger=\overline A^{\mathrm T}.
$$

For a real [matrix](vector-space.md#matrix) it is the ordinary [transpose](vector-space.md#transpose). For the complex [matrix](vector-space.md#matrix) $T$ in the [adjoint operator](#adjoint-operator) example, its second row $(2,1-i)$ becomes the second column $(2,1+i)^{\mathrm T}$ of $T^\dagger$. This is the same [conjugate transpose](linear-operator-theory.md#conjugate-transpose) used in MIT's treatment of complex [inner products](linear-algebra.md#inner-product) and [Hermitian matrices](#hermitian-operator).[Strang, MIT 18.06SC, lecture 26 summary, Complex matrices, pp. 1–2, 2011](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/53f17d47bf99d26fdc472b3177c256a8_MIT18_06SCF11_Ses3.2sum.pdf)

For [bounded operators](topological-vector-space.md#continuous-linear-operator) with matching source and target [Hilbert spaces](hilbert-space.md), [Hermitian conjugation](#hermitian-conjugation) satisfies

$$
(A+B)^\dagger=A^\dagger+B^\dagger,\quad (\alpha A)^\dagger=\overline\alpha A^\dagger,\quad (BA)^\dagger=A^\dagger B^\dagger,\quad (A^\dagger)^\dagger=A.
$$

The reversal of [function composition](function.md#function-composition) is forced by moving both [linear operators](vector-space.md#linear-operator) across an [inner product](linear-algebra.md#inner-product):

$$
\langle BAx,y\rangle=\langle Ax,B^\dagger y\rangle=\langle x,A^\dagger B^\dagger y\rangle.
$$

The calculation identifies the [adjoint operator](#adjoint-operator) by the uniqueness theorem in Melrose's MIT notes.[Melrose, MIT 18.102, Functional Analysis, Chapter 3, §11, 2020](https://ocw.mit.edu/courses/18-102-introduction-to-functional-analysis-spring-2021/3d4cc88026d44a01f936cd6a0aa995cb_MIT18_102s20_lec_FA.pdf)

For a computed order check, let $S=\begin{pmatrix}0&1\\1&0\end{pmatrix}$ and reuse $T=\begin{pmatrix}1&i\\2&1-i\end{pmatrix}$. Then

$$
(ST)^\dagger=T^\dagger S=\begin{pmatrix}2&1\\1+i&-i\end{pmatrix},\qquad ST^\dagger=\begin{pmatrix}-i&1+i\\1&2\end{pmatrix}.
$$

Keeping the original order gives a different [matrix](vector-space.md#matrix). Likewise $(iT)^\dagger=-iT^\dagger$: taking the [adjoint operator](#adjoint-operator) is conjugate-linear as an operation on [linear operators](vector-space.md#linear-operator), although each individual $T^\dagger$ is a [linear map](vector-space.md#linear-map) on [vectors](vector-space.md#vector).

#### Formal adjoint

↑ **Parent:** [Adjoint operator](#adjoint-operator)

The formal adjoint of a differential operator $L$ is characterized by moving $L$ between factors under an integral by [integration by parts](calculus.md#integration-by-parts), while discarding boundary terms for compactly supported functions.

##### Boundary terms exclude formal adjoint eigenvectors

↑ **Parent:** [Formal adjoint](#formal-adjoint)

The [formal adjoint](#formal-adjoint) of an infinite matrix does not specify the domain of the true adjoint. For the weighted difference generator $(Qf)_n=4^n(f_{n-1}/2-f_n)$, its formal positive-eigenvalue solution is $h_n=2^{-n}h_0\prod_{k<n}(1+\alpha4^{-k})$. This is square summable but does not belong to the true adjoint domain of the maximal operator: testing against $f_n=2^{-n}$ contradicts the adjoint identity. The nonzero limiting boundary term is the obstruction.

// Target: analysis.bigb

##### Adjoint reciprocity for a weighted Helmholtz operator

↑ **Parent:** [Formal adjoint](#formal-adjoint)

For smooth positive $f$, let $L=f^{-1}\nabla\cdot(f\nabla)+k^2$. Its unweighted bilinear transpose is the displayed operator. If $v$ satisfies $\alpha v+\beta\partial_nv=0$, its transpose boundary condition is $\alpha u+\beta(\partial_nu-u\partial_n\log f)=0$. The resulting Green kernels satisfy $G_L(\mathbf r_2,\mathbf r_1)=G_{L^{\mathrm T}}(\mathbf r_1,\mathbf r_2)$. Equivalently $G_{L^{\mathrm T}}(\mathbf r,\mathbf r_2)=f(\mathbf r)G_L(\mathbf r,\mathbf r_2)/f(\mathbf r_2)$, exhibiting [weighted acoustic Green-function reciprocity](physics.md#weighted-acoustic-green-function-reciprocity).

##### Complete boundary-jet condition for formal adjoints

↑ **Parent:** [Formal adjoint](#formal-adjoint)

For an order-$m$ operator with smooth coefficients on a bounded piecewise smooth domain, [integration by parts](calculus.md#integration-by-parts) has no boundary remainder when at each boundary point either the entire [boundary jet](partial-differential-equation.md#boundary-jet) of $u$ through order $m-1$ vanishes or the entire such jet of $v$ vanishes. Every boundary summand pairs [derivatives](calculus.md#derivative) of the two functions of order at most $m-1$. It is insufficient to require only that, for each same multi-index $\beta$, one of $\partial^\beta u$ and $\partial^\beta v$ vanish: for $P=\partial_x^2$, $u=x(a-x)\chi(y)$ and $v=1$ on a rectangle, all those same-index products vanish on the boundary but $\int(Pu)v=-2a\int\chi\ne0$.

#### Hermitian operator

↑ **Parent:** [Adjoint operator](#adjoint-operator)

A [bounded operator](topological-vector-space.md#continuous-linear-operator) $T:H\to H$ on a real or complex [Hilbert space](hilbert-space.md) is Hermitian, or [self-adjoint](linear-operator-theory.md#self-adjoint-operator), when $T=T^*$. Equivalently,

$$
\langle Tx,y\rangle=\langle x,Ty\rangle\qquad(x,y\in H).
$$

Its directional values $q_T(x)=\langle Tx,x\rangle$ are real, since this identity makes $q_T(x)$ equal its [complex conjugate](complex-analysis.md#complex-conjugate). Reality allows either sign; a [positive operator](#positive-operator) additionally requires nonnegative values in every direction.

<a id="image-self-adjoint-directional-values-may-change-sign-touch-zero-or-stay-strictly-positive"></a>
![](hermitian-quadratic-values.png)

**[Figure 4](#image-self-adjoint-directional-values-may-change-sign-touch-zero-or-stay-strictly-positive). Self-adjoint directional values may change sign, touch zero, or stay strictly positive**.

The diagram compares [Hermitian quadratic forms](#hermitian-quadratic-form) along paths of [unit vectors](vector-space.md#unit-vector). The [Hermitian matrix](#hermitian-operator) $D=\operatorname{diag}(1,-1)$ takes the values $1$ and $-1$ on the standard [basis vectors](vector-space.md#basis-vector); $P=\operatorname{diag}(1,0)$ takes the values $1$ and $0$; and

$$
H=\begin{pmatrix}2&i\\-i&2\end{pmatrix},\qquad e_1=\frac1{\sqrt2}\begin{pmatrix}1\\i\end{pmatrix},\qquad e_3=\frac1{\sqrt2}\begin{pmatrix}1\\-i\end{pmatrix}
$$

satisfies $He_1=e_1$ and $He_3=3e_3$. These [eigenvectors](linear-operator-theory.md#eigenvector) form an [orthonormal basis](linear-algebra.md#orthonormal-basis), and every $x=ae_1+be_3$ has $q_H(x)=|a|^2+3|b|^2$. Thus $H$ is a [positive operator](#positive-operator), with [eigenvalues](linear-operator-theory.md#eigenvalue) $1,3$ and [operator norm](continuous-dual-space.md#operator-norm) $3$.

Three conditions describe different geometry. A [Hermitian operator](#hermitian-operator) satisfies $T=T^*$; a [normal operator](#normal-operator) satisfies $T^*T=TT^*$; a [unitary operator](vector-space.md#unitary-operator) satisfies $T^*T=TT^*=I$, where $I$ is the [identity operator](vector-space.md#identity-operator). Every [Hermitian operator](#hermitian-operator) and every [unitary operator](vector-space.md#unitary-operator) is a [normal operator](#normal-operator). Concrete [matrices](vector-space.md#matrix) separate the conditions:

- The [Hermitian matrix](#hermitian-operator) $H$ above is a [normal operator](#normal-operator) and a [positive operator](#positive-operator), but not a [unitary matrix](linear-operator-theory.md#unitary-matrix), because $\|He_3\|=3$.
- $U=\operatorname{diag}(i,1)$ is a [unitary matrix](linear-operator-theory.md#unitary-matrix) and [normal matrix](linear-operator-theory.md#normal-matrix), but not a [Hermitian matrix](#hermitian-operator), since $U^*=\operatorname{diag}(-i,1)$.
- $N=\operatorname{diag}(2,i)$ is a [normal matrix](linear-operator-theory.md#normal-matrix), but neither a [Hermitian matrix](#hermitian-operator) nor a [unitary matrix](linear-operator-theory.md#unitary-matrix): its first standard [basis vector](vector-space.md#basis-vector) doubles in [norm](functional-analysis.md#norm).
- $J=\begin{pmatrix}0&1\\0&0\end{pmatrix}$ is not a [normal matrix](linear-operator-theory.md#normal-matrix), since $J^*J=\operatorname{diag}(0,1)$ and $JJ^*=\operatorname{diag}(1,0)$.

The [spectrum](linear-operator-theory.md#spectrum-functional-analysis) of a bounded [Hermitian operator](#hermitian-operator) is real. In finite [dimension](vector-space.md#dimension-vector-space), the [spectral theorem](#spectral-theorem) supplies an [orthonormal basis](linear-algebra.md#orthonormal-basis) of [eigenvectors](linear-operator-theory.md#eigenvector), turning its action into independent real scalings. This makes the geometry easy to interpret: each [eigenvalue](linear-operator-theory.md#eigenvalue) records a signed response along an [orthogonal](linear-algebra.md#orthogonal-vectors) direction. An arbitrary bounded [Hermitian operator](#hermitian-operator) in infinite [dimension](vector-space.md#dimension-vector-space) need not have any [eigenvectors](linear-operator-theory.md#eigenvector); the general [spectral theorem](#spectral-theorem) uses a [projection-valued measure](#projection-valued-measure). MIT's lecture 21 develops the real [spectrum](linear-operator-theory.md#spectrum-functional-analysis) and the [orthogonality](linear-algebra.md#orthogonal-vectors) of [eigenspaces](linear-operator-theory.md#eigenspace).[Rodriguez, notes by Andrew Lin, MIT 18.102, lecture 21, Theorems 223 and 227, 2021](https://ocw.mit.edu/courses/18-102-introduction-to-functional-analysis-spring-2021/345c4a5141559a4069aeb3105acd8ef3_MIT18_102s21_lec21.pdf)

A historical connection is the study of forms with conjugate variables. In his 1901 account of Charles Hermite's work, Camille Jordan describes these forms and emphasizes their role in reducing forms with real or complex [coefficients](vector-space.md#coefficient). In today's notation, $x^*Hx$ is the diagonal value of a [Hermitian form](linear-algebra.md#hermitian-form); the conjugate variables make a real-valued expression possible even with complex [coefficients](vector-space.md#coefficient).[Jordan, Notice sur M. Ch. Hermite, Journal de mathématiques pures et appliquées 7, pp. 92 and 95, 1901](https://www.numdam.org/item/JMPA_1901_5_7__91_0.pdf)

For a [densely defined operator](vector-space.md#densely-defined-operator) outside this bounded setting, the displayed pairing identity alone defines a [symmetric operator](#symmetric-operator). A [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) must also have the same [operator domain](vector-space.md#operator-domain) as its [adjoint operator](#adjoint-operator).

##### Hermitian quadratic form

↑ **Parent:** [Hermitian operator](#hermitian-operator)

A bounded [Hermitian operator](#hermitian-operator) determines a [Hermitian form](linear-algebra.md#hermitian-form) $b_T(x,y)=\langle Tx,y\rangle$ and its real-valued diagonal expression $q_T(x)=b_T(x,x)$. On a complex [Hilbert space](hilbert-space.md),

$$
q_T(\alpha x)=|\alpha|^2q_T(x).
$$

Thus it is a [quadratic form](linear-algebra.md#quadratic-form) on the underlying real [vector space](vector-space.md); it is generally not a [quadratic form](linear-algebra.md#quadratic-form) over the complex [field](algebra.md#field), whose scaling rule would involve $\alpha^2$. This distinction explains why replacing $x^*$ by $x^{\mathrm T}$ loses the geometry of a complex [inner product](linear-algebra.md#inner-product).

For a finite-dimensional [Hermitian operator](#hermitian-operator) with an [orthonormal basis](linear-algebra.md#orthonormal-basis) of [eigenvectors](linear-operator-theory.md#eigenvector) $e_j$ and corresponding [eigenvalues](linear-operator-theory.md#eigenvalue) $\lambda_j$, the [spectral theorem](#spectral-theorem) gives

$$
x=\sum_j c_je_j\quad\Longrightarrow\quad q_T(x)=\sum_j\lambda_j|c_j|^2.
$$

For a [unit vector](vector-space.md#unit-vector), this is an average of the [eigenvalues](linear-operator-theory.md#eigenvalue) with nonnegative weights summing to one. It is also the [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient), so its minimum and maximum are the smallest and largest [eigenvalues](linear-operator-theory.md#eigenvalue).

In the [Hermitian operator](#hermitian-operator) diagram, take $x(\theta)=(\cos\theta,\sin\theta)^{\mathrm T}$ for $D,P$, and $x_H(\theta)=\cos\theta\,e_1+\sin\theta\,e_3$ for $H$. The computed curves are

$$
q_D(x(\theta))=\cos(2\theta),\quad q_P(x(\theta))=\cos^2\theta,\quad q_H(x_H(\theta))=\cos^2\theta+3\sin^2\theta.
$$

These paths illustrate the extremal values; the [spectral theorem](#spectral-theorem) supplies the bounds for every complex [unit vector](vector-space.md#unit-vector), including those outside the plotted paths.

##### Hermitian part of a matrix

↑ **Parent:** [Hermitian operator](#hermitian-operator)

The Hermitian part of a square [matrix](vector-space.md#matrix) is half its sum with its [conjugate transpose](linear-operator-theory.md#conjugate-transpose). It is a [Hermitian matrix](#hermitian-operator) and satisfies $\operatorname{Re}(x^*Ax)=x^*Hx$. Its largest [eigenvalue](linear-operator-theory.md#eigenvalue) is the [numerical abscissa](continuous-dual-space.md#euclidean-logarithmic-norm), controlling instantaneous growth of the [Euclidean norm](functional-analysis.md#euclidean-norm) under $x'=Ax$.

##### Determinant of Hermitian congruence

↑ **Parent:** [Hermitian operator](#hermitian-operator)

For a complex $n\times n$ matrix $B$, the real [linear map](vector-space.md#linear-map) $A\mapsto BAB^*$ on the $n^2$-dimensional real [vector space](vector-space.md) of [Hermitian matrices](#hermitian-operator) has [determinant](linear-algebra.md#determinant) $|\det B|^{2n}$. A real [basis](vector-space.md#basis) of [Hermitian matrices](#hermitian-operator) is also a complex [basis](vector-space.md#basis) of all matrices, so the matrix of this restriction equals the matrix of the complex-linear congruence map. Left and right multiplication separately have [determinants](linear-algebra.md#determinant) $(\det B)^n$ and $(\overline{\det B})^n$.

##### Positive operator

↑ **Parent:** [Hermitian operator](#hermitian-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Positive_operator)

A bounded [Hermitian operator](#hermitian-operator) $T$ on a [Hilbert space](hilbert-space.md) is positive, also called a [positive semidefinite operator](#positive-operator), when

$$
q_T(x)=\langle Tx,x\rangle\geq0\qquad\text{for every }x\in H.
$$

The value must be real as well as nonnegative. This permits zero values on nonzero [vectors](vector-space.md#vector): the zero [linear operator](vector-space.md#linear-operator) is positive. For a bounded [Hermitian operator](#hermitian-operator), positivity is equivalent to its [spectrum](linear-operator-theory.md#spectrum-functional-analysis) being contained in $[0,\infty)$; in finite [dimension](vector-space.md#dimension-vector-space), this is the condition that all [eigenvalues](linear-operator-theory.md#eigenvalue) are nonnegative.[Rodriguez, notes by Andrew Lin, MIT 18.102, lecture 21, Corollary 225, 2021](https://ocw.mit.edu/courses/18-102-introduction-to-functional-analysis-spring-2021/345c4a5141559a4069aeb3105acd8ef3_MIT18_102s21_lec21.pdf)

The [Hermitian operator](#hermitian-operator) diagram separates three cases. $D=\operatorname{diag}(1,-1)$ is [self-adjoint](linear-operator-theory.md#self-adjoint-operator) but not positive, because $q_D((0,1)^{\mathrm T})=-1$. The [orthogonal projection](#orthogonal-projection) $P=\operatorname{diag}(1,0)$ is positive semidefinite, with $q_P(x)=|x_1|^2$, but is not strictly positive on every nonzero [vector](vector-space.md#vector). The complex [Hermitian matrix](#hermitian-operator) $H=\begin{pmatrix}2&i\\-i&2\end{pmatrix}$ is positive definite because $q_H(ae_1+be_3)=|a|^2+3|b|^2>0$ whenever $(a,b)\ne(0,0)$. For real [symmetric matrices](linear-algebra.md#symmetric-matrix), MIT's lecture 27 relates these tests to the geometry of [quadratic forms](linear-algebra.md#quadratic-form) and their minima.[Strang, MIT 18.06SC, lecture 27 summary, Positive definite matrices and minima, pp. 1–2, 2011](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/d163e012754258d3b374548504d8a18a_MIT18_06SCF11_Ses3.3sum.pdf)

A fundamental source of [positive operators](#positive-operator) is $T^*T$ for a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) $T:H\to K$:

$$
(T^*T)^*=T^*T,\qquad \langle T^*Tx,x\rangle=\langle Tx,Tx\rangle=\|Tx\|^2\geq0.
$$

For the complex [matrix](vector-space.md#matrix) $T=\begin{pmatrix}1&i\\2&1-i\end{pmatrix}$ used above,

$$
T^*T=\begin{pmatrix}5&2-i\\2+i&3\end{pmatrix},\qquad q_{T^*T}(x)=|x_1+ix_2|^2+|2x_1+(1-i)x_2|^2.
$$

Its [eigenvalues](linear-operator-theory.md#eigenvalue) are $4-\sqrt6$ and $4+\sqrt6$, both positive. Positivity organizes the squared error minimized by a [least-squares solution](inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem): the same $T^*T$ occurs in the [normal equation for a linear inverse problem](inverse-problem.md#normal-equation-for-a-linear-inverse-problem). The [positive square root of an operator](#positive-square-root-of-an-operator) gives the converse squared-length description, $q_T(x)=\|T^{1/2}x\|^2$ for every bounded [positive operator](#positive-operator) $T$.

On a real [Hilbert space](hilbert-space.md), nonnegativity of $\langle Tx,x\rangle$ alone does not imply [self-adjointness](linear-operator-theory.md#self-adjoint-operator), so the [Hermitian operator](#hermitian-operator) hypothesis is part of the definition. On a complex [Hilbert space](hilbert-space.md), real-valuedness of all these expressions already forces [self-adjointness](linear-operator-theory.md#self-adjoint-operator) by the [polarization identity](linear-algebra.md#polarization-identity).

Strict positivity and a uniform positive lower bound also differ in infinite [dimension](vector-space.md#dimension-vector-space). On the [l2 sequence space](banach-space.md#l2-sequence-space), the bounded [Hermitian operator](#hermitian-operator) $(Tx)_n=x_n/n$ satisfies

$$
q_T(x)=\sum_{n=1}^{\infty}\frac{|x_n|^2}{n}>0\quad(x\ne0),\qquad q_T(e_n)=\frac1n\longrightarrow0.
$$

Consequently no $\gamma>0$ satisfies $q_T(x)\geq\gamma\|x\|^2$ for every $x$. Compare the [positive definite symmetric operator](#positive-definite-symmetric-operator) and [uniformly positive definite symmetric operator](#uniformly-positive-definite-symmetric-operator) conditions.

###### Positive definite symmetric operator

↑ **Parent:** [Positive operator](#positive-operator)

A [symmetric operator](#symmetric-operator) $L$ on a real [Hilbert space](hilbert-space.md) is strictly positive definite when $\langle Lv,v\rangle>0$ for every nonzero $v$ in its [operator domain](vector-space.md#operator-domain). Strict positivity proves uniqueness of a solution of $Lu=f$, but in infinite dimension it need not prove existence for every $f$. A [uniformly positive definite symmetric operator](#uniformly-positive-definite-symmetric-operator) additionally has a positive lower bound independent of $v$. Symmetry must be stated separately when positivity is defined only by a real quadratic expression: adding a [skew-symmetric matrix](linear-algebra.md#skew-symmetric-matrix) changes the operator without changing that expression.

###### Quadratic variational principle for a symmetric positive operator

↑ **Parent:** [Positive definite symmetric operator](#positive-definite-symmetric-operator)

For a symmetric [bounded bilinear form](linear-algebra.md#bounded-bilinear-form) $B$ that is strictly positive on nonzero vectors, and a bounded [linear functional](linear-algebra.md#linear-functional) $\ell$, set $I(v)=B(v,v)-2\ell(v)$. The [first variation](calculus-of-variations.md#first-variation) is $DI(v)[w]=2(B(v,w)-\ell(w))$. A [weak solution](partial-differential-equation.md#weak-solution) $u$ of $B(u,w)=\ell(w)$ satisfies $I(u+w)-I(u)=B(w,w)$, so it is the unique minimizer. Conversely, any minimizer solves the weak equation. A [coercive bilinear form](linear-algebra.md#coercive-bilinear-form) gives existence by the [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem); strict positivity alone does not.

###### Symmetric part determines a real quadratic functional

↑ **Parent:** [Quadratic variational principle for a symmetric positive operator](#quadratic-variational-principle-for-a-symmetric-positive-operator)

For a bounded operator on a real [Hilbert space](hilbert-space.md), $\langle Lv,v\rangle=\langle Sv,v\rangle$ with $S=(L+L^*)/2$. Consequently the [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) of $\langle Lv,v\rangle-2\langle f,v\rangle$ is $Sv=f$. It is $Lv=f$ only when $L$ is [self-adjoint](linear-operator-theory.md#self-adjoint-operator) or when the relevant solution also annihilates the skew part. For example $L=\begin{pmatrix}1&-1\\1&1\end{pmatrix}$ has positive quadratic form $\|v\|^2$, but that form contains no information about its skew part.

###### Uniformly positive definite symmetric operator

↑ **Parent:** [Positive definite symmetric operator](#positive-definite-symmetric-operator)

A [positive definite symmetric operator](#positive-definite-symmetric-operator) is uniformly positive definite if $\langle Lv,v\rangle\geq\gamma\|v\|^2$ for some $\gamma>0$. For a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) defined on a whole [Hilbert space](hilbert-space.md), this is a symmetric [coercive operator](functional-analysis.md#coercive-operator), and the [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) supplies a unique solution to $Lu=f$ for every $f$. For a differential operator, the corresponding bounded coercive form is used on its form space.

###### Positive contraction

↑ **Parent:** [Positive operator](#positive-operator)

A positive contraction is a [positive operator](#positive-operator) whose [operator norm](continuous-dual-space.md#operator-norm) is at most one. Its [spectrum](linear-operator-theory.md#spectrum-functional-analysis) lies in $[0,1]$, so the [spectral theorem for normal operators](#spectral-theorem-for-normal-operators) gives $M^2\leq M$. Positive contractions are the effects in a [POVM](quantum-measurement.md#positive-operator-valued-measure) and occur in the [pure-state gentle measurement bound](quantum-information-theory.md#pure-state-gentle-measurement-bound).

###### Support of a positive operator

↑ **Parent:** [Positive operator](#positive-operator)

The support of a [positive operator](#positive-operator) is the [orthogonal complement](#orthogonal-complement) of its [kernel](linear-algebra.md#kernel-of-a-linear-map). In finite dimension it is the span of [eigenvectors](linear-operator-theory.md#eigenvector) with positive [eigenvalues](linear-operator-theory.md#eigenvalue), equivalently the operator's image. [Quantum relative entropy](von-neumann-entropy.md#quantum-relative-entropy) is finite only when the first state's support lies in the reference state's support.

###### Positive square root of an operator

↑ **Parent:** [Positive operator](#positive-operator)

Every bounded [positive operator](#positive-operator) $T$ has a unique positive operator $T^{1/2}$ satisfying $(T^{1/2})^2=T$. The [spectral theorem for normal operators on a separable Hilbert space](#spectral-theorem-for-normal-operators-on-a-separable-hilbert-space) constructs it by applying the scalar square-root function to the spectrum.

##### Positive-negative decomposition of a Hermitian operator

↑ **Parent:** [Hermitian operator](#hermitian-operator)

The [spectral theorem for normal operators](#spectral-theorem-for-normal-operators) gives a unique decomposition

$$
A=A_+-A_-,
$$

where $A_+,A_-\geq0$ and their supports are orthogonal. They are called the positive and negative parts of $A$. If $\operatorname{Tr}A=0$, then $\operatorname{Tr}A_+=\operatorname{Tr}A_-=\lVert A\rVert_1/2$.

###### Negative part of a Hermitian operator

↑ **Parent:** [Positive-negative decomposition of a Hermitian operator](#positive-negative-decomposition-of-a-hermitian-operator)

The negative part of a [Hermitian operator](#hermitian-operator) is $X_-=\sum_i\max(-\lambda_i,0)P_i=(|X|-X)/2$. In this convention $X_-$ is itself a [positive operator](#positive-operator), and $X=X_+-X_-$. Its support is orthogonal to that of the [positive part of a Hermitian operator](#positive-part-of-a-hermitian-operator).

###### Positive part of a Hermitian operator

↑ **Parent:** [Positive-negative decomposition of a Hermitian operator](#positive-negative-decomposition-of-a-hermitian-operator)

For a [Hermitian operator](#hermitian-operator) with [spectral decomposition](linear-operator-theory.md#spectral-decomposition) $X=\sum_i\lambda_iP_i$, its positive part is $X_+=\sum_i\max(\lambda_i,0)P_i=(|X|+X)/2$. It is a [positive operator](#positive-operator) supported on the positive spectral subspace. Together with the [negative part of a Hermitian operator](#negative-part-of-a-hermitian-operator) it satisfies $X=X_+-X_-$ and $|X|=X_++X_-$.

<h5 id="lowner-order">Löwner order</h5>

↑ **Parent:** [Hermitian operator](#hermitian-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Löwner_order)

For [Hermitian operators](#hermitian-operator) $A$ and $B$, one writes $A\leq B$ when $B-A$ is positive semidefinite. This partial order is also called the semidefinite order.

###### Operator monotonicity of the square root

↑ **Parent:** [Löwner order](#lowner-order)

For bounded positive [self-adjoint operators](linear-operator-theory.md#self-adjoint-operator), $0\leq A\leq B$ implies $A^{1/2}\leq B^{1/2}$. Thus the nonnegative square-root function is operator monotone.

#### Adjoint criterion for an invariant orthogonal complement

↑ **Parent:** [Adjoint operator](#adjoint-operator)

For a subspace $U$ of a finite-dimensional inner-product space,

$$
T(U)\subseteq U
\quad\Longleftrightarrow\quad
T^*(U^\perp)\subseteq U^\perp.
$$

This follows directly by moving $T$ across the inner product and using $(U^\perp)^\perp=U$.

#### Normal operator

↑ **Parent:** [Adjoint operator](#adjoint-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_operator)

An operator is normal when $TT^*=T^*T$. Equivalently,

$$
\lVert Tx\rVert=\lVert T^*x\rVert
$$

for every $x$; the converse follows by polarizing the quadratic form of the self-adjoint commutator $T^*T-TT^*$.

##### Normal spectrum equals approximate point spectrum

↑ **Parent:** [Normal operator](#normal-operator)

For a normal bounded operator, $\sigma(T)=\sigma_{\mathrm{ap}}(T)$. If $T-\lambda I$ is bounded below, its range is closed; normality makes its adjoint injective, so the range is also dense and the operator is invertible.

##### Spectral theorem

↑ **Parent:** [Normal operator](#normal-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spectral_theorem)

The spectral theorem represents a [normal operator](#normal-operator) by multiplication by its spectral parameter. In a finite-dimensional [inner product space](linear-algebra.md#inner-product-space), this is diagonalization in an [orthonormal basis](linear-algebra.md#orthonormal-basis); for a [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) on a [Hilbert space](hilbert-space.md), it uses a [projection-valued measure](#projection-valued-measure). Unbounded operators additionally require their natural square-integrability domain.

###### Spectral theorem for normal operators

↑ **Parent:** [Spectral theorem](#spectral-theorem)

Every normal operator on a finite-dimensional complex inner-product space has an orthonormal basis of eigenvectors. An eigenvector is also an eigenvector of the adjoint with conjugate eigenvalue, so its orthogonal complement reduces the operator and induction applies.

###### Finite commuting normal operators have joint spectral projections

↑ **Parent:** [Spectral theorem for normal operators](#spectral-theorem-for-normal-operators)

A finite family of pairwise commuting [normal operators](#normal-operator) on a finite-dimensional complex [inner product space](linear-algebra.md#inner-product-space), commuting also with each other's adjoints, generates a commutative unital [C-star algebra](banach-algebra.md#c-star-algebra). Its finite [maximal ideal space](banach-algebra.md#maximal-ideal-space-of-a-commutative-banach-algebra) identifies the algebra with functions on finitely many points. The characteristic functions of those points pull back under the [Gelfand transform](banach-algebra.md#gelfand-representation) to mutually orthogonal self-adjoint [linear projections](vector-space.md#projection-linear-algebra) summing to the identity. Their ranges are the simultaneous eigenspaces, giving simultaneous diagonalization without choosing separate incompatible eigenbases.

###### Spectral matrix functional calculus

↑ **Parent:** [Spectral theorem for normal operators](#spectral-theorem-for-normal-operators)

For a [Hermitian matrix](#hermitian-operator) with unitary diagonalization $A=U\operatorname{diag}(\lambda_i)U^*$, define $f(A)=U\operatorname{diag}(f(\lambda_i))U^*$ for a function on its finite spectrum. This acts on [eigenvalues](linear-operator-theory.md#eigenvalue), unlike an [entrywise matrix function](vector-space.md#entrywise-matrix-function) $f[A]$. For example, the spectral square of a [matrix](vector-space.md#matrix) is its ordinary [matrix](vector-space.md#matrix) product with itself, whereas its entrywise square is a [Hadamard power](vector-space.md#hadamard-power).

###### Spectral theorem for normal operators on a separable Hilbert space

↑ **Parent:** [Spectral theorem for normal operators](#spectral-theorem-for-normal-operators)

A normal operator on a separable Hilbert space has a unique projection-valued spectral measure $E$ such that $A=\int z\,dE(z)$, with the natural square-integrability domain in the unbounded case.

###### Weyl-von Neumann theorem

↑ **Parent:** [Spectral theorem for normal operators on a separable Hilbert space](#spectral-theorem-for-normal-operators-on-a-separable-hilbert-space)

Every [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) on a separable complex [Hilbert space](hilbert-space.md) is diagonal modulo a [compact operator](compact-operator.md). For a bounded operator the compact self-adjoint error can have arbitrarily small [Hilbert-Schmidt norm](compact-operator.md#hilbert-schmidt-norm). In a cyclic spectral representation, partition a bounded real interval into $N$ intervals of width at most $\delta$ and successively bisect. Orthogonal step-function differences give basis vectors supported in the parent intervals. A diagonal value chosen in each support interval gives total squared column error at most $3N\delta^2$. Since $N=O(\delta^{-1})$, this tends to zero. Apply the construction to countably many cyclic summands with summable squared error bounds. For an unbounded operator first split into bounded spectral intervals, obtaining a bounded compact error on the same domain.

###### Classification of separable self-adjoint operators modulo compacts

↑ **Parent:** [Weyl-von Neumann theorem](#weyl-von-neumann-theorem)

Bounded [self-adjoint operators](linear-operator-theory.md#self-adjoint-operator) on separable infinite-dimensional complex [Hilbert spaces](hilbert-space.md) are unitarily equivalent modulo [compact operators](compact-operator.md) exactly when they have the same [essential spectrum in the Calkin algebra](functional-analysis.md#essential-spectrum-in-the-calkin-algebra). The [Weyl-von Neumann theorem](#weyl-von-neumann-theorem) diagonalizes each modulo a compact error. Their diagonal cluster sets are the essential spectra; [cluster-set matching of bounded sequences](real-analysis.md#cluster-set-matching-of-bounded-sequences) pairs the two diagonal lists with differences tending to zero, giving a compact diagonal difference. The separability assumption is essential: projections with countable and uncountable range dimensions can have the same essential spectrum but cannot differ by a [compact operator](compact-operator.md) after unitary conjugation.

###### Projection-valued measure

↑ **Parent:** [Spectral theorem for normal operators on a separable Hilbert space](#spectral-theorem-for-normal-operators-on-a-separable-hilbert-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projection-valued_measure)

A projection-valued measure $E$ assigns an [orthogonal projection](#orthogonal-projection) $E(B)$ to each measurable set, with $E(\varnothing)=0$, $E(X)=I$, $E(B\cap C)=E(B)E(C)$, and countable additivity in the [strong operator topology](functional-analysis.md#strong-operator-topology) on pairwise disjoint sets.

###### Cyclic multiplication model for a normal operator

↑ **Parent:** [Projection-valued measure](#projection-valued-measure)

The [continuous functional calculus](banach-algebra.md#continuous-functional-calculus) of a bounded [normal operator](#normal-operator) $T$ is a representation of $C(K)$, with $K=\sigma(T)$. The [Riesz-Markov-Kakutani representation theorem](functional-analysis.md#riesz-markov-kakutani-representation-theorem) represents $f\mapsto\langle f(T)v,v\rangle$ by a positive regular measure $\mu_v$. The assignment $f\mapsto f(T)v$ is isometric for the $L^2(\mu_v)$ [norm](functional-analysis.md#norm), and extends to a unitary map onto the [closed](topology.md#closed-set) cyclic subspace it generates. Multiplication by $z$ and $\overline z$ represent $T$ and $T^*$. Orthogonal decomposition into cyclic [reducing subspaces](#reducing-subspace-of-a-hilbert-space-operator), allowing an uncountable family, constructs the [Borel functional calculus for a normal operator](banach-algebra.md#borel-functional-calculus-for-a-normal-operator) without requiring separability.

###### Scalar-measure construction of a projection-valued measure

↑ **Parent:** [Projection-valued measure](#projection-valued-measure)

For a unital star-representation $\pi:C(K)\to\mathcal B(H)$, the [Riesz-Markov-Kakutani representation theorem](functional-analysis.md#riesz-markov-kakutani-representation-theorem) gives regular measures $\mu_{x,y}$ representing $f\mapsto\langle\pi(f)x,y\rangle$. Define $P(E)$ by $\langle P(E)x,y\rangle=\mu_{x,y}(E)$. Positivity and $\mu_{x,x}(K)=\|x\|^2$ make these positive contractions. The identities $\mu_{\pi(f)x,y}=f\mu_{x,y}$ imply commutation with $\pi(f)$ and $\mu_{P(E)x,y}=1_E\mu_{x,y}$; hence $P(F)P(E)=P(F\cap E)$. Thus each $P(E)$ is an [orthogonal projection](#orthogonal-projection). Scalar countable additivity and orthogonality give countable additivity in the [strong operator topology](functional-analysis.md#strong-operator-topology), constructing the normalized regular [projection-valued measure](#projection-valued-measure).

###### Spectral theorem for a commutative operator algebra

↑ **Parent:** [Projection-valued measure](#projection-valued-measure)

If $A$ is a commutative [C-star algebra](banach-algebra.md#c-star-algebra) of bounded operators on a [Hilbert space](hilbert-space.md) containing its identity, there is a unique regular [projection-valued measure](#projection-valued-measure) $E$ on the [character space](banach-algebra.md#character-space-of-an-algebra) $\Phi_A$ such that $E(\Phi_A)=I$ and $a=\int_{\Phi_A}\widehat a\,dE$ for every $a\in A$, where $\widehat a$ is the [Gelfand transform](banach-algebra.md#gelfand-representation).

###### Full support of a faithful spectral measure

↑ **Parent:** [Spectral theorem for a commutative operator algebra](#spectral-theorem-for-a-commutative-operator-algebra)

For a faithful representation of $C(K)$ by integration against a regular [projection-valued measure](#projection-valued-measure) $P$, every nonempty open subset $U$ satisfies $P(U)\ne0$. Choose a nonzero continuous function supported inside $U$, using compact Hausdorff normality. If $P(U)=0$, its spectral integral vanishes, contradicting faithfulness. Regularity is understood through the [scalar spectral measures](#scalar-spectral-measure).

###### Spectral projector

↑ **Parent:** [Projection-valued measure](#projection-valued-measure)

A spectral projector is the value $E(B)$ of the [projection-valued measure](#projection-valued-measure) of a normal operator on a measurable part $B$ of its spectrum. In finite dimension, the spectral projector onto an eigenspace extracts the corresponding eigenvector component.

###### Spectral measure of a normal operator

↑ **Parent:** [Spectral theorem for normal operators on a separable Hilbert space](#spectral-theorem-for-normal-operators-on-a-separable-hilbert-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spectral_measure_of_a_normal_operator)

For vectors $f,g$, the scalar spectral measure is $\mu_{f,g}(S)=\langle E(S)f,g\rangle$. Functional calculus satisfies $\langle h(A)f,g\rangle=\int h\,d\mu_{f,g}$.

###### Spectral projection gives a reducing subspace

↑ **Parent:** [Spectral measure of a normal operator](#spectral-measure-of-a-normal-operator)

For a bounded [normal operator](#normal-operator) $T$ with [spectral measure of a normal operator](#spectral-measure-of-a-normal-operator) $P$, any projection $P(E)$ commutes with $T$ and $T^*$ by the [Borel functional calculus for a normal operator](banach-algebra.md#borel-functional-calculus-for-a-normal-operator). Its range is a closed reducing subspace. If the spectrum has two points, choose disjoint nonempty relative open sets around them. [Full support of a faithful spectral measure](#full-support-of-a-faithful-spectral-measure) makes both projections nonzero and their product zero, so either range is nonzero and proper, in particular an [invariant subspace](representation-theory.md#invariant-subspace).

###### Scalar spectral measure

↑ **Parent:** [Spectral measure of a normal operator](#spectral-measure-of-a-normal-operator)

For a [projection-valued measure](#projection-valued-measure) $E$ and vectors $v,w$, the scalar spectral measure is the complex measure $\mu_{v,w}(B)=\langle E(B)v,w\rangle$. The positive measure $\mu_v=\mu_{v,v}$ has total mass $\|v\|^2$.

###### Weak convergence of scalar spectral measures

↑ **Parent:** [Scalar spectral measure](#scalar-spectral-measure)

Scalar spectral measures $\mu^{(n)}_{v,w}$ converge weakly to $\mu_{v,w}$ when $\int f\,d\mu^{(n)}_{v,w}\to\int f\,d\mu_{v,w}$ for every bounded continuous function $f$. Uniform second-moment bounds supply the tightness needed to pass from polynomial tests to all such $f$.

###### Stone formula

↑ **Parent:** [Spectral measure of a normal operator](#spectral-measure-of-a-normal-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stone_formula)

Stone's formula recovers spectral projections of a self-adjoint operator from the jump of its resolvent across the real axis, with half weight at interval endpoints.

## Weak convergence in a Hilbert space

↑ **Parent:** [Hilbert space](hilbert-space.md)

A sequence $x_n$ converges weakly to $x$ when $\langle x_n,y\rangle\to\langle x,y\rangle$ for every $y$ in the Hilbert space.

<h3 id="weak-banach-saks-theorem-in-a-hilbert-space">Weak Banach–Saks theorem in a Hilbert space</h3>

↑ **Parent:** [Weak convergence in a Hilbert space](#weak-convergence-in-a-hilbert-space)

If $x_n\rightharpoonup x$ in a [Hilbert space](hilbert-space.md), some subsequence $(x_{n_k})$ has [Cesàro means](real-analysis.md#cesaro-mean) converging in norm to $x$. For $x=0$, choose the subsequence so successive vectors have summably small inner products; expansion of the squared norm of its averages then proves convergence.

Thus [Hilbert spaces](hilbert-space.md) have the weak form of the [Banach-Saks property](banach-space.md#banach-saks-property).

### Coordinate criterion for weak convergence in a separable Hilbert space

↑ **Parent:** [Weak convergence in a Hilbert space](#weak-convergence-in-a-hilbert-space)

For a Hilbertian basis $(e_i)$, a sequence $x_n$ converges weakly if and only if $(x_n)$ is norm bounded and every coordinate sequence $\langle x_n,e_i\rangle$ converges.

### Weak subsequence of a bounded Hilbert-space sequence

↑ **Parent:** [Weak convergence in a Hilbert space](#weak-convergence-in-a-hilbert-space)

Every bounded sequence in a separable Hilbert space has a weakly convergent subsequence. Successive subsequences make each basis coordinate converge, and a diagonal subsequence converges in every coordinate; the [coordinate criterion for weak convergence in a separable Hilbert space](#coordinate-criterion-for-weak-convergence-in-a-separable-hilbert-space) finishes the proof.

### Weak lower semicontinuity of the Hilbert norm

↑ **Parent:** [Weak convergence in a Hilbert space](#weak-convergence-in-a-hilbert-space)

If $x_n\rightharpoonup x$ in a Hilbert space, then

$$
\lVert x\rVert\leq\liminf_n\lVert x_n\rVert.
$$

For $x\ne0$, take the inner product with $x$ and apply Cauchy-Schwarz before passing to the lower limit.

### Radon-Riesz theorem

↑ **Parent:** [Weak convergence in a Hilbert space](#weak-convergence-in-a-hilbert-space)

In a Hilbert space, weak convergence $x_n\rightharpoonup x$ together with $\lVert x_n\rVert\to\lVert x\rVert$ implies strong convergence $x_n\to x$.

#### Uniform basis-tail criterion for strong convergence

↑ **Parent:** [Radon-Riesz theorem](#radon-riesz-theorem)

Suppose $x_n\rightharpoonup x$ in a separable Hilbert space with Hilbertian basis $(e_i)$. Then $x_n\to x$ in norm exactly when

$$
\forall\epsilon>0\ \exists I\ 
\forall n,\qquad
\sum_{i\geq I}|\langle x_n,e_i\rangle|^2<\epsilon.
$$

The condition prevents norm from escaping to successively higher basis coordinates.

### Weakly null orthonormal sequence

↑ **Parent:** [Weak convergence in a Hilbert space](#weak-convergence-in-a-hilbert-space)

Every [orthonormal sequence](#orthonormal-sequence) in a Hilbert space converges weakly to zero, by [Bessel inequality](#bessel-s-inequality), but no subsequence converges strongly because distinct terms remain distance $\sqrt2$ apart.

<h3 id="mazur-s-lemma">Mazur's lemma</h3>

↑ **Parent:** [Weak convergence in a Hilbert space](#weak-convergence-in-a-hilbert-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mazur's_lemma)

If $x_n$ converges weakly to $x$ in a Banach space, there are convex combinations of each tail $\{x_n,x_{n+1},\ldots\}$ that converge in norm to $x$.

#### Mazur theorem

↑ **Parent:** [Mazur's lemma](#mazur-s-lemma)

The weak closure and norm closure of a convex subset of a real or complex normed space coincide. If a point lies outside the norm closure, the [Hahn-Banach separation theorem](functional-analysis.md#hahn-banach-separation-theorem) supplies a weakly continuous linear functional that separates it from the convex set.

### Norm-closed convex set is weakly closed

↑ **Parent:** [Weak convergence in a Hilbert space](#weak-convergence-in-a-hilbert-space)

A norm-closed convex subset of a Banach space contains every weak limit of its sequences. Apply [Mazur lemma](#mazur-s-lemma) to obtain norm-convergent convex combinations that remain in the set.

## Orthonormal sequence

↑ **Parent:** [Hilbert space](hilbert-space.md)

An orthonormal sequence $(e_n)$ satisfies $\langle e_n,e_m\rangle=0$ for $n\ne m$ and $\lVert e_n\rVert=1$.

This is the sequential form of [orthonormality](linear-algebra.md#orthonormal-set).

### Hilbertian basis

↑ **Parent:** [Orthonormal sequence](#orthonormal-sequence)

A Hilbertian basis is a complete orthonormal family: its closed linear span is the whole Hilbert space, equivalently every vector is the norm-convergent sum of its Fourier coefficients against the basis.

#### Parseval identity for a Hilbertian basis

↑ **Parent:** [Hilbertian basis](#hilbertian-basis)

For a Hilbertian basis $(e_i)$,

$$
\langle x,y\rangle
=\sum_i\langle x,e_i\rangle\overline{\langle y,e_i\rangle},
\qquad
\lVert x\rVert^2=\sum_i|\langle x,e_i\rangle|^2.
$$

<h3 id="bessel-s-inequality">Bessel's inequality</h3>

↑ **Parent:** [Orthonormal sequence](#orthonormal-sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bessel's_inequality)

For an orthonormal sequence $(e_n)$ in a Hilbert space,

$$
\sum_n|\langle x,e_n\rangle|^2\leq\lVert x\rVert^2.
$$

## ↑ Ancestors (5)

1. [Functional analysis](functional-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (384)

- [2-summing operator](topological-vector-space.md#2-summing-operator)
- [Adjoint in weighted coordinates](#adjoint-in-weighted-coordinates)
- [Adjoint of a densely defined operator](#adjoint-of-a-densely-defined-operator)
- [Adjoint operator](#adjoint-operator)
- [Antiunitary operator](vector-space.md#antiunitary-operator)
- [Banach-Saks property](banach-space.md#banach-saks-property)
- [Bargmann-Fock space](#bargmann-fock-space)
- [Best linear prediction from an infinite past](time-series.md#best-linear-prediction-from-an-infinite-past)
- [Best N-term approximation](#best-n-term-approximation)
- [Born rule](quantum-mechanics.md#born-rule)
- [Bounded bilinear form](linear-algebra.md#bounded-bilinear-form)
- [C-star unitization by left multiplication](banach-algebra.md#c-star-unitization-by-left-multiplication)
- [Calkin algebra](banach-algebra.md#calkin-algebra)
- [Cameron-Martin space of a Gaussian measure](stochastic-process.md#cameron-martin-space-of-a-gaussian-measure)
- [Cameron-Martin space of a Gaussian random variable in a Banach space](stochastic-process.md#cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space)
- [Classification of separable self-adjoint operators modulo compacts](#classification-of-separable-self-adjoint-operators-modulo-compacts)
- [Closed convex set](mathematical-optimization.md#closed-convex-set)
- [Closed linear span](vector-space.md#closed-linear-span)
- [Closed-range bound on the kernel complement](functional-analysis.md#closed-range-bound-on-the-kernel-complement)
- [Closed subspace of a Hilbert space](#closed-subspace-of-a-hilbert-space)
- [Coercive bilinear form](linear-algebra.md#coercive-bilinear-form)
- [Compact averaging of a rank-one operator](compact-operator.md#compact-averaging-of-a-rank-one-operator)
- [Compact operators send weak convergence to norm convergence](compact-operator.md#compact-operators-send-weak-convergence-to-norm-convergence)
- [Compact perturbation invariance of Fredholm operators](functional-analysis.md#compact-perturbation-invariance-of-fredholm-operators)
- [Complex structure on the Klein-Gordon solution space](quantum-field-theory.md#complex-structure-on-the-klein-gordon-solution-space)
- [Confining-potential energy space](nonlinear-analysis.md#confining-potential-energy-space)
- [Conjugate index vector](quantum-theory.md#conjugate-index-vector)
- [Conjugate of the squared distance to a convex set](convex-optimization.md#conjugate-of-the-squared-distance-to-a-convex-set)
- [Convergence of primal-dual hybrid gradient](convex-optimization.md#convergence-of-primal-dual-hybrid-gradient)
- [Covariant photon Fock space](relativistic-quantum-field.md#covariant-photon-fock-space)
- [Cyclic unitary representation of a positive-definite function](analysis.md#cyclic-unitary-representation-of-a-positive-definite-function)
- [Cylindrical Brownian motion](brownian-motion.md#cylindrical-brownian-motion)
- [Densely defined operator](vector-space.md#densely-defined-operator)
- [Density matrix](quantum-theory.md#density-matrix)
- [Dirichlet form of the Kac collision operator](statistical-physics.md#dirichlet-form-of-the-kac-collision-operator)
- [Double orthogonal complement](#double-orthogonal-complement)
- [Duality mapping](banach-space.md#duality-mapping)
- [Ellipsoid level sets of a positive-definite quadratic form](linear-algebra.md#ellipsoid-level-sets-of-a-positive-definite-quadratic-form)
- [Ellipticity of a bounded Hilbert-space operator](functional-analysis.md#ellipticity-of-a-bounded-hilbert-space-operator)
- [Energy eigenvalue](quantum-mechanics.md#energy-eigenvalue)
- [Entropy bound from overlap with a pure state](von-neumann-entropy.md#entropy-bound-from-overlap-with-a-pure-state)
- [Essential spectrum in the Calkin algebra](functional-analysis.md#essential-spectrum-in-the-calkin-algebra)
- [Essential spectrum of a bounded self-adjoint operator](functional-analysis.md#essential-spectrum-of-a-bounded-self-adjoint-operator)
- [Exact spectral gap of normalized velocity relaxation](statistical-physics.md#exact-spectral-gap-of-normalized-velocity-relaxation)
- [Exact variational solution in a two-level system](quantum-theory.md#exact-variational-solution-in-a-two-level-system)
- [Expectation value](quantum-mechanics.md#expectation-value)
- [Exponential tilting of an isonormal Gaussian process](stochastic-process.md#exponential-tilting-of-an-isonormal-gaussian-process)
- [Exponentially weighted L2 space](measure-theory.md#exponentially-weighted-l2-space)
- [Extreme points of the density-operator state space](quantum-theory.md#extreme-points-of-the-density-operator-state-space)
- [Fermion-number sectors in supersymmetric quantum mechanics](quantum-mechanics.md#fermion-number-sectors-in-supersymmetric-quantum-mechanics)
- [Fidelity of quantum states](quantum-information-theory.md#fidelity-of-quantum-states)
- [Finite element method](numerical-analysis.md#finite-element-method)
- [Five-qubit error correcting code](quantum-error-correction.md#five-qubit-error-correcting-code)
- [Fixed-energy initial-condition optimality](control-theory.md#fixed-energy-initial-condition-optimality)
- [Fock space](quantum-field-theory.md#fock-space)
- [Fourier transform on a finite group](additive-combinatorics.md#fourier-transform-on-a-finite-group)
- [Fractional Dirichlet domain scale](partial-differential-equation.md#fractional-dirichlet-domain-scale)
- [Fredholm determinant](compact-operator.md#fredholm-determinant)
- [Fredholm index](functional-analysis.md#fredholm-index)
- [Friedrichs extension](linear-operator-theory.md#friedrichs-extension)
- [Gaussian random element](random-variable.md#gaussian-random-element)
- [Generalized eigenfunction](linear-operator-theory.md#generalized-eigenfunction)
- [Generalized singular vector](convex-optimization.md#generalized-singular-vector)
- [Grothendieck inequality](linear-algebra.md#grothendieck-inequality)
- [Grothendieck theorem for L1 to Hilbert operators](linear-algebra.md#grothendieck-theorem-for-l1-to-hilbert-operators)
- [Ground state](quantum-mechanics.md#ground-state)
- [Gupta-Bleuler null-state quotient](relativistic-quantum-field.md#gupta-bleuler-null-state-quotient)
- [H1 space](sobolev-space.md#h1-space)
- [Haar twirling conditional expectation](quantum-theory.md#haar-twirling-conditional-expectation)
- [Half-density](ringed-space.md#half-density)
- [Heine-Borel theorem](topology.md#heine-borel-theorem)
- [Heisenberg-Weyl operator](quantum-information-theory.md#heisenberg-weyl-operator)
- [Hermitian conjugation](#hermitian-conjugation)
- [Hermitian operator](#hermitian-operator)
- [Hermitian quadratic form](#hermitian-quadratic-form)
- [Hilbert projection theorem](#hilbert-projection-theorem)
- [Hilbert-Schmidt operator](compact-operator.md#hilbert-schmidt-operator)
- [Hilbert space](hilbert-space.md)
- [Hilbert-space central limit theorem](convergence-of-random-variables.md#hilbert-space-central-limit-theorem)
- [Hilbert space completion](#hilbert-space-completion)
- [Hilbert space module over a von Neumann algebra](functional-analysis.md#hilbert-space-module-over-a-von-neumann-algebra)
- [Hilbert-space-valued random variable](random-variable.md#hilbert-space-valued-random-variable)
- [Hilbert tensor product](#hilbert-tensor-product)
- [Holstein–Primakoff occupation constraint](quantum-mechanics.md#holstein-primakoff-occupation-constraint)
- [Image-kernel orthogonality for an adjoint](#image-kernel-orthogonality-for-an-adjoint)
- [Indefinite Hermitian form](linear-algebra.md#indefinite-hermitian-form)
- [Inner product space](linear-algebra.md#inner-product-space)
- [Isonormal Gaussian process](stochastic-process.md#isonormal-gaussian-process)
- [Johnson–Lindenstrauss lemma](functional-analysis.md#johnson-lindenstrauss-lemma)
- [Källén–Lehmann spectral representation](scalar-field-theory.md#kallen-lehmann-spectral-representation)
- [L2 sequence space](banach-space.md#l2-sequence-space)
- [L2 space is a Hilbert space](measure-theory.md#l2-space-is-a-hilbert-space)
- [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem)
- [Least-squares existence criterion](inverse-problem.md#least-squares-existence-criterion)
- [Least-squares solution of a linear inverse problem](inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem)
- [Left shift operator](linear-operator-theory.md#left-shift-operator)
- [Linear regression](linear-regression.md)
- [Locally square-integrable function](measure-theory.md#locally-square-integrable-function)
- [Maximally mixed state](quantum-theory.md#maximally-mixed-state)
- [Maximum entropy of a quantum state](von-neumann-entropy.md#maximum-entropy-of-a-quantum-state)
- [Moore--Penrose inverse of a Hilbert-space operator](linear-algebra.md#moore-penrose-inverse-of-a-hilbert-space-operator)
- [Multiplicity-free complete dyadic spectrum](linear-operator-theory.md#multiplicity-free-complete-dyadic-spectrum)
- [Negative-energy direction gives exponential growth in a self-adjoint wave equation](linear-operator-theory.md#negative-energy-direction-gives-exponential-growth-in-a-self-adjoint-wave-equation)
- [No-ghost theorem for the critical bosonic string](string-theory.md#no-ghost-theorem-for-the-critical-bosonic-string)
- [Nondegenerate representations by compact operators](compact-operator.md#nondegenerate-representations-by-compact-operators)
- [Norm-compact unit ball criterion](#norm-compact-unit-ball-criterion)
- [Normal equation for coercive Tikhonov regularization](inverse-problem.md#normal-equation-for-coercive-tikhonov-regularization)
- [Numerical radius](functional-analysis.md#numerical-radius)
- [Odd topological K-theory](algebraic-topology.md#odd-topological-k-theory)
- [One-dimensional harmonic oscillator form domain](quantum-mechanics.md#one-dimensional-harmonic-oscillator-form-domain)
- [Operator formalism](quantum-mechanics.md#operator-formalism)
- [Operator norm duality](continuous-dual-space.md#operator-norm-duality)
- [Operator predual from matrix coefficients](functional-analysis.md#operator-predual-from-matrix-coefficients)
- [Order preservation for the linear Boltzmann equation](statistical-physics.md#order-preservation-for-the-linear-boltzmann-equation)
- [Original and weak continuity of linear maps between Fréchet spaces](weak-topology.md#original-and-weak-continuity-of-linear-maps-between-frechet-spaces)
- [Orthogonal direct sum](vector-space.md#orthogonal-direct-sum)
- [Orthogonal eigenvectors of a compact operator](compact-operator.md#orthogonal-eigenvectors-of-a-compact-operator)
- [Orthogonal projection onto a finite-dimensional subspace](linear-algebra.md#orthogonal-projection-onto-a-finite-dimensional-subspace)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3.md#20f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-6.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-7.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2.md#17f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-7.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-7.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-10.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-11.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-57.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-47.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-50.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-58.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#22f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-52.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-63.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4.md#22g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-60.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-64.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-8.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10.md#8/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-11.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-34.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-34.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-34.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-59.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4.md#22f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1.md#8/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-11.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-13.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-13.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-48.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-58.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-80.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-9.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3.md#7b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#30b/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-12.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-12.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-12.md#6/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-50.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-50.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-56.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#5/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#7/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#31e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#31e/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50.md#3/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-62.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63.md#2/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63.md#2/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-64.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-64.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-70.md#4/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-70.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3.md#21g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-5.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69.md#1/1/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-78.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-78.md#4/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-25.md#1/c/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-36.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-36.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63.md#2/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63.md#3/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63.md#3/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-75.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-5.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-5.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-5.md#1/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-5.md#1/g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-52.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-62.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-7.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-72.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-72.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-72.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-14.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5.md#2/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5.md#2/10/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5.md#2/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-7.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-81.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1.md#14a/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-105.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-105.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-311.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-325.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#32c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#21f/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#21f/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-106.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-301.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-307.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#1/1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#1/2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#3/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#3/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#3/4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#3/5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#3/7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3.md#16b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2.md#26j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105.md#2/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-106.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-108.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-203.md#3/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#1/1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#3/1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#3/2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#23h/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-105.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-105.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-105.md#2/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-326.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#33a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#22h/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-105.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-154.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-326.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-326.md#2/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#33b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#22f/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-105.md#2/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-205.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-225.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-324.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-105.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-105.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-105.md#2/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-323.md#4/a/solution)
- [Perfect quantum error-correcting code](quantum-error-correction.md#perfect-quantum-error-correcting-code)
- [Polarized fermionic Fock space](quantum-mechanics.md#polarized-fermionic-fock-space)
- [Positive definite symmetric operator](#positive-definite-symmetric-operator)
- [Positive operator](#positive-operator)
- [Positive operator-valued measure](quantum-measurement.md#positive-operator-valued-measure)
- [Positive semidefinite Hermitian form](linear-algebra.md#positive-semidefinite-hermitian-form)
- [Positivity-preserving linear operator on L1](topological-vector-space.md#positivity-preserving-linear-operator-on-l1)
- [Proximal operator under affine rescaling](convex-optimization.md#proximal-operator-under-affine-rescaling)
- [Quadratic norm penalty](inverse-problem.md#quadratic-norm-penalty)
- [Quantum error-correcting code](quantum-error-correction.md#quantum-error-correcting-code)
- [Quantum error correction](quantum-error-correction.md)
- [Quantum Hamming bound](quantum-error-correction.md#quantum-hamming-bound)
- [Quantum register](quantum-circuit.md#quantum-register)
- [Quantum state continuity at a finite Hamiltonian step](quantum-mechanics.md#quantum-state-continuity-at-a-finite-hamiltonian-step)
- [Quantum superposition](quantum-mechanics.md#quantum-superposition)
- [Quantum system](quantum-mechanics.md#quantum-system)
- [Quartic-norm variational regularization](inverse-problem.md#quartic-norm-variational-regularization)
- [Qubit](quantum-mechanics.md#qubit)
- [Qudit](quantum-mechanics.md#qudit)
- [Range of a bounded linear operator](topological-vector-space.md#range-of-a-bounded-linear-operator)
- [Range of the Volterra integration operator](functional-analysis.md#range-of-the-volterra-integration-operator)
- [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient)
- [Reducing subspace of a Hilbert-space operator](#reducing-subspace-of-a-hilbert-space-operator)
- [Regularization of an inverse problem](inverse-problem.md#regularization-of-an-inverse-problem)
- [Restricted unitary group](topological-group.md#restricted-unitary-group)
- [Self-adjoint operator](linear-operator-theory.md#self-adjoint-operator)
- [Solvability condition](linear-operator-theory.md#solvability-condition)
- [Source-condition estimate for symmetric Bregman distance](inverse-problem.md#source-condition-estimate-for-symmetric-bregman-distance)
- [Spectral theorem](#spectral-theorem)
- [Spectral theorem for a commutative operator algebra](#spectral-theorem-for-a-commutative-operator-algebra)
- [Sphere in a normed vector space](functional-analysis.md#sphere-in-a-normed-vector-space)
- [Stone theorem for the circle group](representation-theory.md#stone-theorem-for-the-circle-group)
- [Strict positivity without coercivity can fail variational solvability](functional-analysis.md#strict-positivity-without-coercivity-can-fail-variational-solvability)
- [Strong convergence of relaxed Landweber iteration](inverse-problem.md#strong-convergence-of-relaxed-landweber-iteration)
- [Subgradient inversion under convex conjugacy](convex-optimization.md#subgradient-inversion-under-convex-conjugacy)
- [Sum of reproducing-kernel Hilbert spaces](probability-and-statistics.md#sum-of-reproducing-kernel-hilbert-spaces)
- [Supersymmetric factorization and zero-mode normalizability](quantum-mechanics.md#supersymmetric-factorization-and-zero-mode-normalizability)
- [Symmetric operator](#symmetric-operator)
- [Symmetric part determines a real quadratic functional](#symmetric-part-determines-a-real-quadratic-functional)
- [Symmetry and coercivity in quadratic energy minimization](numerical-analysis.md#symmetry-and-coercivity-in-quadratic-energy-minimization)
- [Tikhonov filter norm bound](inverse-problem.md#tikhonov-filter-norm-bound)
- [Tikhonov regularization](inverse-problem.md#tikhonov-regularization)
- [Tikhonov regularization with a coercive penalty operator](inverse-problem.md#tikhonov-regularization-with-a-coercive-penalty-operator)
- [Total variation calibration](inverse-problem.md#total-variation-calibration)
- [Unbounded self-adjoint operator](linear-operator-theory.md#unbounded-self-adjoint-operator)
- [Uniformly positive definite symmetric operator](#uniformly-positive-definite-symmetric-operator)
- [Unital algebra](associative-algebra.md#unital-algebra)
- [Unitary equivalence](vector-space.md#unitary-equivalence)
- [Unitary extension of a finite-dimensional isometry](#unitary-extension-of-a-finite-dimensional-isometry)
- [Van der Corput lemma (Hilbert space sequences)](measure-theory.md#van-der-corput-lemma-hilbert-space-sequences)
- [Variational problem](calculus-of-variations.md#variational-problem)
- [Von Neumann algebra](functional-analysis.md#von-neumann-algebra)
- [Von Neumann double commutant theorem](associative-algebra.md#von-neumann-double-commutant-theorem)
- [Von Neumann mean ergodic theorem](vector-space.md#von-neumann-mean-ergodic-theorem)
- [Weak Banach–Saks theorem in a Hilbert space](#weak-banach-saks-theorem-in-a-hilbert-space)
- [Weak sequential compactness in a Hilbert space](functional-analysis.md#weak-sequential-compactness-in-a-hilbert-space)
- [Weighted Hilbert structure of velocity-reset relaxation](statistical-physics.md#weighted-hilbert-structure-of-velocity-reset-relaxation)
- [Weyl theorem for compact self-adjoint perturbations](functional-analysis.md#weyl-theorem-for-compact-self-adjoint-perturbations)
- [Weyl-von Neumann theorem](#weyl-von-neumann-theorem)
- [White-noise likelihood for a square-integrable shift](stochastic-process.md#white-noise-likelihood-for-a-square-integrable-shift)
- [Zero mode in the fermion-vacuum sector](quantum-mechanics.md#zero-mode-in-the-fermion-vacuum-sector)
