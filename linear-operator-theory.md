# Operator theory

↑ **Parent:** [Linear algebra](linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Operator_theory)

Linear operator theory studies [linear maps](vector-space.md#linear-map), their [spectra](#spectrum-functional-analysis), invariant subspaces, and normal forms.

**Table of contents**

- [Polar decomposition](#polar-decomposition)
- [Shift operator](#shift-operator)
  - [Unilateral shift operator](#unilateral-shift-operator)
    - [Left shift operator](#left-shift-operator)
    - [Point spectrum](#point-spectrum)
    - [Wandering-vector characterization of a unilateral shift](#wandering-vector-characterization-of-a-unilateral-shift)
- [Solvability condition](#solvability-condition)
- [Spectrum (functional analysis)](#spectrum-functional-analysis)
  - [Approximate eigenvalue](#approximate-eigenvalue)
    - [Approximate eigenvector](#approximate-eigenvector)
  - [Residual spectrum](#residual-spectrum)
  - [Continuous spectrum](#continuous-spectrum)
  - [Spectrum of a bounded operator](#spectrum-of-a-bounded-operator)
- [Compression of a linear operator](#compression-of-a-linear-operator)
- [Self-adjoint operator](#self-adjoint-operator)
  - [Negative-energy direction gives exponential growth in a self-adjoint wave equation](#negative-energy-direction-gives-exponential-growth-in-a-self-adjoint-wave-equation)
  - [Friedrichs extension](#friedrichs-extension)
  - [Spectral Weyl sequence](#spectral-weyl-sequence)
    - [Singular Weyl sequence](#singular-weyl-sequence)
  - [Unbounded self-adjoint operator](#unbounded-self-adjoint-operator)
    - [Spectral positivity criterion for a self-adjoint operator](#spectral-positivity-criterion-for-a-self-adjoint-operator)
    - [Nonreal resolvent estimate for a self-adjoint operator](#nonreal-resolvent-estimate-for-a-self-adjoint-operator)
  - [Fredholm solvability condition for a self-adjoint operator](#fredholm-solvability-condition-for-a-self-adjoint-operator)
  - [Positive-definite operator](#positive-definite-operator)
    - [Strict operator positivity does not imply surjectivity](#strict-operator-positivity-does-not-imply-surjectivity)
  - [Finite-dimensional spectral theorem](#finite-dimensional-spectral-theorem)
    - [Multiplicity-free complete dyadic spectrum](#multiplicity-free-complete-dyadic-spectrum)
    - [Orthonormal eigenbasis](#orthonormal-eigenbasis)
  - [Laguerre differential operator on polynomials](#laguerre-differential-operator-on-polynomials)
    - [Laguerre polynomial](#laguerre-polynomial)
      - [Generalized Laguerre polynomial](#generalized-laguerre-polynomial)
        - [Rodrigues' formula](#rodrigues-formula)
- [Real spectral theorem](#real-spectral-theorem)
- [Power method](#power-method)
  - [Dominant eigenpair extraction from a two-step Krylov recurrence](#dominant-eigenpair-extraction-from-a-two-step-krylov-recurrence)
  - [Quadratic Rayleigh-quotient improvement for the power method](#quadratic-rayleigh-quotient-improvement-for-the-power-method)
  - [Active spectrum of the power method](#active-spectrum-of-the-power-method)
  - [Inverse iteration](#inverse-iteration)
    - [Convergence of fixed-shift inverse iteration](#convergence-of-fixed-shift-inverse-iteration)
      - [Sign behavior of fixed-shift inverse iteration](#sign-behavior-of-fixed-shift-inverse-iteration)
  - [Subspace iteration](#subspace-iteration)
    - [Dominant invariant subspace](#dominant-invariant-subspace)
    - [Power method with a dominant eigenvalue cluster](#power-method-with-a-dominant-eigenvalue-cluster)
- [Characteristic polynomial](#characteristic-polynomial)
  - [Characteristic polynomials of AB and BA](#characteristic-polynomials-of-ab-and-ba)
  - [Faddeev–LeVerrier algorithm](#faddeev-leverrier-algorithm)
  - [Real parameter avoiding a singular matrix pencil](#real-parameter-avoiding-a-singular-matrix-pencil)
  - [Triangularization over an algebraically closed field](#triangularization-over-an-algebraically-closed-field)
- [Eigenvalue interlacing](#eigenvalue-interlacing)
  - [Largest-eigenvalue interlacing for a principal submatrix](#largest-eigenvalue-interlacing-for-a-principal-submatrix)
- [Jordan normal form](#jordan-normal-form)
  - [Unipotent involutions in characteristic two](#unipotent-involutions-in-characteristic-two)
  - [Density of diagonalizable complex matrices](#density-of-diagonalizable-complex-matrices)
  - [Repeated-eigenvalue classification in dimension two](#repeated-eigenvalue-classification-in-dimension-two)
  - [Jordan–Chevalley decomposition](#jordan-chevalley-decomposition)
    - [Adjoint compatibility of additive Jordan decomposition](#adjoint-compatibility-of-additive-jordan-decomposition)
      - [Semisimple matrix Lie algebras are closed under additive Jordan decomposition](#semisimple-matrix-lie-algebras-are-closed-under-additive-jordan-decomposition)
  - [Algebraic multiplicity](#algebraic-multiplicity)
  - [Geometric multiplicity](#geometric-multiplicity)
  - [Jordan block](#jordan-block)
    - [Square-root splitting of a defective double eigenvalue](#square-root-splitting-of-a-defective-double-eigenvalue)
    - [Nilpotent Jordan block](#nilpotent-jordan-block)
  - [Jordan normal form of conjugation on two-by-two matrices](#jordan-normal-form-of-conjugation-on-two-by-two-matrices)
  - [Characteristic and minimal polynomials determine similarity in dimension three](#characteristic-and-minimal-polynomials-determine-similarity-in-dimension-three)
  - [Generalized eigenvector](#generalized-eigenvector)
    - [Jordan chain](#jordan-chain)
      - [Length-two Jordan chain solution](#length-two-jordan-chain-solution)
    - [Generalized eigenspace](#generalized-eigenspace)
      - [Nilpotent commutator preserves generalized eigenspaces](#nilpotent-commutator-preserves-generalized-eigenspaces)
    - [Generalized eigenspaces for distinct eigenvalues form a direct sum](#generalized-eigenspaces-for-distinct-eigenvalues-form-a-direct-sum)
- [Generalized eigenvalue problem](#generalized-eigenvalue-problem)
  - [Generalized characteristic polynomial](#generalized-characteristic-polynomial)
- [Matrix exponential](#matrix-exponential)
  - [Skew-symmetric exponential as an axial rotation](#skew-symmetric-exponential-as-an-axial-rotation)
  - [Derivative of the matrix exponential](#derivative-of-the-matrix-exponential)
  - [Matrix exponential determinant identity](#matrix-exponential-determinant-identity)
  - [Matrix exponential when the square is minus the identity](#matrix-exponential-when-the-square-is-minus-the-identity)
  - [Baker--Campbell--Hausdorff formula](#baker-campbell-hausdorff-formula)
  - [Laplace transform of a matrix exponential](#laplace-transform-of-a-matrix-exponential)
- [Minimal polynomial](#minimal-polynomial)
  - [Characteristic and minimal polynomials of right multiplication](#characteristic-and-minimal-polynomials-of-right-multiplication)
  - [Real matrices have real minimal polynomials](#real-matrices-have-real-minimal-polynomials)
  - [Integer powers for an annihilating polynomial with roots one and minus one](#integer-powers-for-an-annihilating-polynomial-with-roots-one-and-minus-one)
  - [Minimal polynomial of an invertible matrix](#minimal-polynomial-of-an-invertible-matrix)
  - [Minimal polynomials of AB and BA](#minimal-polynomials-of-ab-and-ba)
    - [Similarity of squared matrix products with one diagonalizable product](#similarity-of-squared-matrix-products-with-one-diagonalizable-product)
  - [Kernel decomposition for coprime polynomials](#kernel-decomposition-for-coprime-polynomials)
  - [Minimal polynomial bound from a triangular invariant flag](#minimal-polynomial-bound-from-a-triangular-invariant-flag)
- [Jacobson lemma for a commuting commutator](#jacobson-lemma-for-a-commuting-commutator)
- [Translation finite-difference operator](#translation-finite-difference-operator)
  - [Mixed finite difference of a polynomial](#mixed-finite-difference-of-a-polynomial)
- [Nilpotent linear map](#nilpotent-linear-map)
  - [Nilpotent matrix](#nilpotent-matrix)
    - [Square-zero criterion for a two-by-two matrix](#square-zero-criterion-for-a-two-by-two-matrix)
    - [Counting nilpotent matrices by the Fitting decomposition](#counting-nilpotent-matrices-by-the-fitting-decomposition)
  - [Nilpotence of commutation by a nilpotent endomorphism](#nilpotence-of-commutation-by-a-nilpotent-endomorphism)
- [Eigenvalue](#eigenvalue)
  - [Eigenvalue collision](#eigenvalue-collision)
  - [Spectral abscissa](#spectral-abscissa)
  - [Eigenvalue multiplicity](#eigenvalue-multiplicity)
  - [Zero eigenvalue](#zero-eigenvalue)
    - [Spectrum of a three-dimensional matrix with zero row sums](#spectrum-of-a-three-dimensional-matrix-with-zero-row-sums)
  - [Eigenvalue problem](#eigenvalue-problem)
  - [Eigenfunction](#eigenfunction)
    - [Nodeless eigenfunction](#nodeless-eigenfunction)
    - [Dirichlet eigenfunction](#dirichlet-eigenfunction)
    - [Adjoint eigenfunction](#adjoint-eigenfunction)
    - [Generalized eigenfunction](#generalized-eigenfunction)
  - [Eigenvector](#eigenvector)
    - [Zero mode](#zero-mode)
    - [Independence of eigenvectors for distinct eigenvalues](#independence-of-eigenvectors-for-distinct-eigenvalues)
    - [Eigenvalue equation](#eigenvalue-equation)
    - [Right eigenvector](#right-eigenvector)
    - [Left eigenvector](#left-eigenvector)
  - [Eigenspace](#eigenspace)
    - [Real square roots of operators with simple real spectrum](#real-square-roots-of-operators-with-simple-real-spectrum)
    - [Laplacian eigenspace](#laplacian-eigenspace)
    - [Eigenbasis](#eigenbasis)
  - [Simple eigenvalue](#simple-eigenvalue)
    - [Eigenvalue sensitivity](#eigenvalue-sensitivity)
      - [First-order perturbation of a simple eigenvalue](#first-order-perturbation-of-a-simple-eigenvalue)
  - [Diagonalizable matrix](#diagonalizable-matrix)
    - [Diagonalization of a matrix](#diagonalization-of-a-matrix)
    - [Diagonalizability inherited from an invertible power](#diagonalizability-inherited-from-an-invertible-power)
    - [Complex similarity of real matrices implies real similarity](#complex-similarity-of-real-matrices-implies-real-similarity)
    - [Distinct eigenvalues imply diagonalizability](#distinct-eigenvalues-imply-diagonalizability)
    - [Spectral decomposition](#spectral-decomposition)
      - [Dominant eigenvalue](#dominant-eigenvalue)
      - [Spectral gap](#spectral-gap)
        - [Ground-space perturbation bound](#ground-space-perturbation-bound)
        - [Davis-Kahan theorem](#davis-kahan-theorem)
          - [Davis-Kahan curvature lemma](#davis-kahan-curvature-lemma)
            - [Rank-one eigenprojector perturbation bound](#rank-one-eigenprojector-perturbation-bound)
- [Conjugate transpose](#conjugate-transpose)
- [Unitary matrix](#unitary-matrix)
  - [Hermitian parts of a unitary matrix](#hermitian-parts-of-a-unitary-matrix)
- [Skew-Hermitian matrix](#skew-hermitian-matrix)
  - [Cross-product model of su(2)](#cross-product-model-of-su-2)
- [Cayley transform of a Hermitian matrix](#cayley-transform-of-a-hermitian-matrix)
- [Normal matrix](#normal-matrix)
  - [Normal matrices have equal adjoint norms](#normal-matrices-have-equal-adjoint-norms)
  - [Hoffman–Wielandt inequality](#hoffman-wielandt-inequality)
    - [Spectral Lipschitz bound from Frobenius distance](#spectral-lipschitz-bound-from-frobenius-distance)
  - [Adjoint eigenvector identity for a normal matrix](#adjoint-eigenvector-identity-for-a-normal-matrix)
  - [Normality criterion for a two-mode shear model](#normality-criterion-for-a-two-mode-shear-model)
  - [Matrix 2-norm of a normal matrix](#matrix-2-norm-of-a-normal-matrix)
  - [Non-normal matrix](#non-normal-matrix)
    - [Nonnormal eigenvalues do not bound a quadratic quotient](#nonnormal-eigenvalues-do-not-bound-a-quadratic-quotient)
    - [Transient growth](#transient-growth)
      - [Optimal initial state for triangular stable shear](#optimal-initial-state-for-triangular-stable-shear)
        - [Short-relative-time optimal state for triangular shear](#short-relative-time-optimal-state-for-triangular-shear)
      - [Instantaneous energy-growth criterion for a linear system](#instantaneous-energy-growth-criterion-for-a-linear-system)
      - [Optimal energy amplification of a linear system](#optimal-energy-amplification-of-a-linear-system)
      - [Two-dimensional triangular model of transient growth](#two-dimensional-triangular-model-of-transient-growth)
        - [Optimal time and gain of a Reynolds-scaled triangular model](#optimal-time-and-gain-of-a-reynolds-scaled-triangular-model)
        - [Orientation interval for transient energy growth](#orientation-interval-for-transient-energy-growth)
        - [Energy-neutral rotational nonlinearity](#energy-neutral-rotational-nonlinearity)
  - [Unitary diagonalization of a normal matrix](#unitary-diagonalization-of-a-normal-matrix)
- [Schur decomposition](#schur-decomposition)
- [Rayleigh quotient](#rayleigh-quotient)
  - [Rayleigh quotient with one Neumann endpoint](#rayleigh-quotient-with-one-neumann-endpoint)
  - [Hermitian Rayleigh quotient range](#hermitian-rayleigh-quotient-range)
  - [Odd variational trial gives an excited oscillator bound](#odd-variational-trial-gives-an-excited-oscillator-bound)
  - [Generalized Rayleigh quotient](#generalized-rayleigh-quotient)
  - [Rayleigh quotient iteration](#rayleigh-quotient-iteration)
    - [Local cubic convergence of Rayleigh quotient iteration](#local-cubic-convergence-of-rayleigh-quotient-iteration)
  - [Rayleigh-Ritz variational principle](#rayleigh-ritz-variational-principle)
    - [Odd-state variational principle for an even potential](#odd-state-variational-principle-for-an-even-potential)
    - [Gaussian variational bound for an attractive Gaussian well](#gaussian-variational-bound-for-an-attractive-gaussian-well)
    - [Finite-subspace variational method](#finite-subspace-variational-method)
      - [Two-mode variational bound for a linearly tilted square well](#two-mode-variational-bound-for-a-linearly-tilted-square-well)
- [Cyclic vector](#cyclic-vector)
  - [Cyclic subspace](#cyclic-subspace)
- [Companion matrix](#companion-matrix)
- [Invariant direct-sum decomposition](#invariant-direct-sum-decomposition)
- [Rational canonical form](#rational-canonical-form)
  - [Primary matrix centralizer formula](#primary-matrix-centralizer-formula)
    - [Counting matrices with a fixed primary polynomial](#counting-matrices-with-a-fixed-primary-polynomial)
  - [Invariant factors of a linear operator](#invariant-factors-of-a-linear-operator)

## Polar decomposition

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polar_decomposition)

For a bounded operator $A$ on a Hilbert space, set $|A|=(A^*A)^{1/2}$. There is a unique partial isometry $U$, zero on $\ker A$, satisfying $A=U|A|$; on the range of $|A|$, define $U(|A|x)=Ax$ and extend by continuity. This is well-defined and isometric because $\|Ax\|^2=\langle A^*Ax,x\rangle=\||A|x\|^2$. For an invertible square matrix, $U$ is unitary.

## Shift operator

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shift_operator)

A shift operator translates the components of a function or sequence by a fixed displacement. Bilateral shifts act on doubly infinite sequences; the [unilateral shift operator](#unilateral-shift-operator) acts on a one-sided sequence space and has distinct forward and backward versions.

### Unilateral shift operator

↑ **Parent:** [Shift operator](#shift-operator)

The unilateral shifts on sequences move every component one place left or right. Their spectra illustrate behavior absent in finite dimensions.

#### Left shift operator

↑ **Parent:** [Unilateral shift operator](#unilateral-shift-operator)

On the [Hilbert space](hilbert-space.md) $\ell^2(\mathbb N)$, the left shift deletes the first coordinate. It is the [adjoint operator](hilbert-space.md#adjoint-operator) of the [unilateral shift operator](#unilateral-shift-operator) $S$. The identities $LS=I$ and $SLf=f-f_1e_1$ show that it is also the [Moore–Penrose inverse of an operator](inverse-problem.md#moore-penrose-inverse-of-an-operator) for $S$; both maps have [operator norm](continuous-dual-space.md#operator-norm) one.

#### Point spectrum

↑ **Parent:** [Unilateral shift operator](#unilateral-shift-operator)

The point spectrum of an operator is its set of eigenvalues.

#### Wandering-vector characterization of a unilateral shift

↑ **Parent:** [Unilateral shift operator](#unilateral-shift-operator)

An operator $T$ is a unilateral shift exactly when it is an isometry, $(\operatorname{Im}T)^\perp$ is one-dimensional, and $\bigcap_{n\geq1}\operatorname{Im}(T^n)=\{0\}$. A unit vector $e_1$ in the first orthogonal complement is wandering, and $e_n=T^{n-1}e_1$ is a complete orthonormal basis.

## Solvability condition

↑ **Parent:** [Operator theory](linear-operator-theory.md)

A solvability condition is a compatibility requirement on data for an equation to admit a solution in a specified function space or with specified boundary behavior. For a bounded [linear operator](vector-space.md#linear-operator) between [Hilbert spaces](hilbert-space.md), the equation $Lu=f$ requires $f$ to be orthogonal to the kernel of the adjoint. A closed range makes that requirement sufficient; the [Fredholm alternative for a compact operator](compact-operator.md#fredholm-alternative) applies this principle to $I-K$ with compact $K$. in an asymptotic inner problem, exclusion of a growing homogeneous mode can impose an analogous weighted-integral condition.

## Spectrum (functional analysis)

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spectrum_(functional_analysis))

The spectrum of a [linear operator](vector-space.md#linear-operator) consists of the [scalars](vector-space.md#scalar) $\lambda$ for which $A-\lambda I$ is not invertible. In finite dimensions it is the set of [eigenvalues](#eigenvalue).

### Approximate eigenvalue

↑ **Parent:** [Spectrum (functional analysis)](#spectrum-functional-analysis)

An approximate eigenvalue of a bounded operator $T$ is a scalar $\lambda$ admitting unit vectors $x_n$ with $\|(T-\lambda I)x_n\|\to0$. Every approximate eigenvalue belongs to the [spectrum](#spectrum-functional-analysis); for a [normal operator](hilbert-space.md#normal-operator), all spectral points are approximate eigenvalues.

#### Approximate eigenvector

↑ **Parent:** [Approximate eigenvalue](#approximate-eigenvalue)

The [unit vectors](vector-space.md#unit-vector) realizing an [approximate eigenvalue](#approximate-eigenvalue) are approximate [eigenvectors](#eigenvector): their residual tends to zero, although they need not converge to any genuine [eigenvector](#eigenvector).

### Residual spectrum

↑ **Parent:** [Spectrum (functional analysis)](#spectrum-functional-analysis)

In the disjoint convention for a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) $T$, the [residual spectrum](#residual-spectrum) consists of $\lambda$ for which $T-\lambda I$ is injective but has nondense range. Together with the [point spectrum](#point-spectrum) and [continuous spectrum](#continuous-spectrum) it partitions the [spectrum of a bounded operator](#spectrum-of-a-bounded-operator). Some conventions also include noninjective operators with nondense range, so the convention must be stated.

### Continuous spectrum

↑ **Parent:** [Spectrum (functional analysis)](#spectrum-functional-analysis)

For a [self-adjoint operator](#self-adjoint-operator) $T$, a real number $\lambda$ lies in the continuous [spectrum](#spectrum-functional-analysis) when $T-\lambda I$ is [injective](algebra.md#injective-function) with dense range but is not surjective. Such spectral values need not be [eigenvalues](#eigenvalue) of normalizable states. The free-particle [Hamiltonian](classical-mechanics.md#hamiltonian) on the real line has a continuous energy [spectrum](#spectrum-functional-analysis).

### Spectrum of a bounded operator

↑ **Parent:** [Spectrum (functional analysis)](#spectrum-functional-analysis)

For a bounded operator on a complex Banach space, the spectrum is a nonempty compact subset of the complex plane contained in the closed disk of radius equal to the operator norm.

## Compression of a linear operator

↑ **Parent:** [Operator theory](linear-operator-theory.md)

If $V$ is a subspace of a space with an [inner product](linear-algebra.md#inner-product) and $P_V$ is its [orthogonal projection](linear-algebra.md#orthogonal-projection-onto-a-finite-dimensional-subspace), the compression of an operator $A$ to $V$ is

$$
P_VA|_V:V\longrightarrow V.
$$

If the columns of $Z$ are an [orthonormal basis](linear-algebra.md#orthonormal-basis) of $V$, its matrix in that basis is $Z^*AZ$.

## Self-adjoint operator

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Self-adjoint_operator)

A [densely defined operator](vector-space.md#densely-defined-operator) $T$ on a [Hilbert space](hilbert-space.md) is self-adjoint when it equals its [adjoint operator](hilbert-space.md#adjoint-operator), including equality of their [operator domains](vector-space.md#operator-domain):

$$
D(T)=D(T^*),\qquad Tv=T^*v\quad(v\in D(T)).
$$

For a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) defined on the whole [Hilbert space](hilbert-space.md), this is equivalent to

$$
\langle Tv,w\rangle=\langle v,Tw\rangle
$$

for all vectors $v,w$. For an [unbounded self-adjoint operator](#unbounded-self-adjoint-operator), the domain condition is essential: the inner-product identity on $D(T)$ alone gives only a [symmetric operator](hilbert-space.md#symmetric-operator).

### Negative-energy direction gives exponential growth in a self-adjoint wave equation

↑ **Parent:** [Self-adjoint operator](#self-adjoint-operator)

Let $\ddot q=Fq$ on a [Hilbert space](hilbert-space.md), with time-independent [self-adjoint operator](#self-adjoint-operator) $F$, and conserved quadratic energy $E=\|\dot q\|^2/2-\langle q,Fq\rangle/2$. If $\langle q_0,Fq_0\rangle>0$, set $\dot q(0)=\alpha q_0$ with $\alpha^2=\langle q_0,Fq_0\rangle/\|q_0\|^2$ and $\alpha>0$. This gives $E=0$. For $N=\|q\|^2$, $N'=2\operatorname{Re}\langle q,\dot q\rangle$ and $N''=4\|\dot q\|^2$, so

$$
(\ln N)''=\frac{4[N\|\dot q\|^2-(\operatorname{Re}\langle q,\dot q\rangle)^2]}{N^2}\geq0
$$

by the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). Since $(\ln N)'(0)=2\alpha$, $N(t)\geq N(0)e^{2\alpha t}$. Positivity of $N$ follows from $N'(0)>0$ and $N''\geq0$. Thus a negative direction of the restoring energy $W=-\langle q,Fq\rangle/2$ yields an exponentially growing solution without a normal-mode expansion or a variational spectral theorem. If $W$ is positive definite, conserved $E$ instead controls the energy norm; a bound in the original [Hilbert space](hilbert-space.md) norm additionally follows from a coercive lower bound on $W$.

### Friedrichs extension

↑ **Parent:** [Self-adjoint operator](#self-adjoint-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Friedrichs_extension)

A densely defined semibounded [symmetric operator](hilbert-space.md#symmetric-operator) on a [Hilbert space](hilbert-space.md) has a canonical semibounded extension that is a [self-adjoint operator](#self-adjoint-operator) obtained by closing its [quadratic form](linear-algebra.md#quadratic-form). After shifting the lower bound to zero, complete the initial form domain in the norm $(\|u\|^2+q[u])^{1/2}$; the associated closed form determines the Friedrichs extension. For the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) on a polygonal surface, this specifies the finite-energy realization at corners. Different choices of the initial form domain impose [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition), or mixed [boundary conditions](differential-equation.md#boundary-condition); the extension does not choose the boundary condition independently of that domain.

### Spectral Weyl sequence

↑ **Parent:** [Self-adjoint operator](#self-adjoint-operator)

For a bounded [self-adjoint operator](#self-adjoint-operator) $L$, a spectral Weyl sequence at $\lambda$ consists of unit vectors $f_n$ with $\|(L-\lambda I)f_n\|\to0$. Such a sequence exists exactly at points of the [spectrum of a bounded operator](#spectrum-of-a-bounded-operator). If no sequence exists, the shifted operator is bounded below, with closed range and zero kernel. Self-adjointness then makes its range dense, so it is invertible. This spectral criterion is different from the equidistribution [Weyl criterion](measure-theory.md#weyl-criterion).

#### Singular Weyl sequence

↑ **Parent:** [Spectral Weyl sequence](#spectral-weyl-sequence)

A singular Weyl sequence for a bounded [self-adjoint operator](#self-adjoint-operator) $L$ at $\lambda$ is a [spectral Weyl sequence](#spectral-weyl-sequence) that also converges weakly to zero. Such a sequence exists exactly when $\lambda$ is in the [essential spectrum of a bounded self-adjoint operator](functional-analysis.md#essential-spectrum-of-a-bounded-self-adjoint-operator). An infinite-dimensional shifted kernel gives a weakly null [orthonormal sequence](hilbert-space.md#orthonormal-sequence). If that kernel is finite-dimensional but the shifted range is not closed, choose approximate null vectors in the kernel complement and extract a weakly convergent subsequence; its limit belongs to both kernel and complement, so is zero.

### Unbounded self-adjoint operator

↑ **Parent:** [Self-adjoint operator](#self-adjoint-operator)

A densely defined [linear operator](vector-space.md#linear-operator) on a complex [Hilbert space](hilbert-space.md) is self-adjoint when its [adjoint operator](hilbert-space.md#adjoint-operator) has exactly the same domain and agrees there. Symmetry only requires $A\subseteq A^*$ and does not guarantee self-adjointness. A self-adjoint operator is a [closed operator](functional-analysis.md#closed-linear-operator) with real [spectrum](#spectrum-functional-analysis). Domains matter for differential operators and unbounded [multiplication operators](vector-space.md#multiplication-operator).

#### Spectral positivity criterion for a self-adjoint operator

↑ **Parent:** [Unbounded self-adjoint operator](#unbounded-self-adjoint-operator)

[Positivity](quantum-information-theory.md#positivity-linear-maps) makes $A-z$ bounded below with dense closed range for every $z<0$, excluding negative spectral values. Conversely if the [spectrum](#spectrum-functional-analysis) is nonnegative, $R=(I+A)^{-1}$ has [spectrum](#spectrum-functional-analysis) in $[0,1]$ by the [resolvent spectral mapping identity](mathematics.md#resolvent-spectral-mapping-identity). The [numerical-range endpoint approximate-eigenvalue theorem](functional-analysis.md#numerical-range-endpoint-approximate-eigenvalue-theorem) gives $0\leq R\leq I$, and positive-form [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\|Rf\|^2\leq\langle Rf,f\rangle$. For $u=Rf$, $\langle Au,u\rangle=\langle Rf,f\rangle-\|Rf\|^2\geq0$.

#### Nonreal resolvent estimate for a self-adjoint operator

↑ **Parent:** [Unbounded self-adjoint operator](#unbounded-self-adjoint-operator)

Symmetry gives $\|(A-z)u\|\geq|\operatorname{Im}z|\|u\|$ when $z$ is nonreal. Closedness makes the range closed; its orthogonal complement is $\ker(A-\overline z)=0$, so it is also dense and hence surjective. This proves the resolvent estimate and reality of the [spectrum](#spectrum-functional-analysis). Equality of the adjoint domains is needed in the range argument.

### Fredholm solvability condition for a self-adjoint operator

↑ **Parent:** [Self-adjoint operator](#self-adjoint-operator)

For a [self-adjoint operator](#self-adjoint-operator) $L$, solving $Lu=f$ requires $f$ to be [orthogonal](linear-algebra.md#orthogonal-vectors) to every $v\in\ker L$, because $\langle v,Lu\rangle=\langle Lv,u\rangle=0$. When the range is closed, this condition is also sufficient: $(\operatorname{ran}L)^\perp=\ker L$ and closedness gives $\operatorname{ran}L=(\ker L)^\perp$. In finite dimensions the range is automatically closed. This [Fredholm solvability condition](analysis.md#fredholm-solvability-condition) determines [amplitude equations](dynamical-systems.md#amplitude-equation) by projecting perturbative forcing onto critical [eigenfunctions](#eigenfunction).

### Positive-definite operator

↑ **Parent:** [Self-adjoint operator](#self-adjoint-operator)

A [self-adjoint operator](#self-adjoint-operator) $A$ is positive definite when $\langle Av,v\rangle>0$ for every nonzero vector $v$ in its domain. In finite dimension it is invertible and has positive [eigenvalues](#eigenvalue). In infinite dimension, strict positivity of individual quadratic-form values need not give a bounded inverse; the stronger uniform bound $\langle Av,v\rangle\geq c\|v\|^2$ with $c>0$ supplies coercivity.

For maps $\beta:U\to V$ and $\gamma:V\to W$ between finite-dimensional [inner product spaces](linear-algebra.md#inner-product-space), with $\operatorname{im}\beta=\ker\gamma$, the operator $\beta\beta^*+\gamma^*\gamma$ is positive definite. Its [quadratic form](linear-algebra.md#quadratic-form) is $\|\beta^*v\|^2+\|\gamma v\|^2$, whose zero set is $\operatorname{im}\beta\cap(\operatorname{im}\beta)^\perp=\{0\}$. This uses the [adjoint operator](hilbert-space.md#adjoint-operator) relation $\ker\beta^*=(\operatorname{im}\beta)^\perp$.

#### Strict operator positivity does not imply surjectivity

↑ **Parent:** [Positive-definite operator](#positive-definite-operator)

On $\ell^2$, the bounded [self-adjoint operator](#self-adjoint-operator) $(Lv)_j=v_j/j$ is strictly positive. Yet $f_j=1/j$ lies in $\ell^2$ and $Lu=f$ would require the non-square-summable vector $u_j=1$. A positive uniform lower bound, rather than strict positivity alone, guarantees a bounded inverse for a bounded [self-adjoint operator](#self-adjoint-operator).

### Finite-dimensional spectral theorem

↑ **Parent:** [Self-adjoint operator](#self-adjoint-operator)

Every self-adjoint operator on a finite-dimensional real inner-product space has an orthonormal basis of eigenvectors and only real eigenvalues.

#### Multiplicity-free complete dyadic spectrum

↑ **Parent:** [Finite-dimensional spectral theorem](#finite-dimensional-spectral-theorem)

A [Hermitian operator](hilbert-space.md#hermitian-operator) on a $2^n$-dimensional [Hilbert space](hilbert-space.md), with $2^n$ distinct [eigenvalues](#eigenvalue) all belonging to $\{c/2^n:0\leq c<2^n\}$, must occupy this entire grid. This follows from the [pigeonhole principle](algebra.md#pigeonhole-principle): the set of possible values and the set of distinct [eigenvalues](#eigenvalue) have the same [cardinality](set-theory.md#cardinality). Its minimum [eigenvalue](#eigenvalue) is zero, so the operator is necessarily singular. Distinctness therefore does not imply invertibility; it forces a one-dimensional [kernel](linear-algebra.md#kernel-of-a-linear-map) in this specific complete-grid setting.

#### Orthonormal eigenbasis

↑ **Parent:** [Finite-dimensional spectral theorem](#finite-dimensional-spectral-theorem)

An orthonormal eigenbasis of a [linear operator](vector-space.md#linear-operator) is an [orthonormal basis](linear-algebra.md#orthonormal-basis) consisting of [eigenvectors](#eigenvector).

### Laguerre differential operator on polynomials

↑ **Parent:** [Self-adjoint operator](#self-adjoint-operator)

On polynomials with weighted inner product

$$
\langle f,g\rangle=\int_0^\infty f(x)g(x)e^{-x}\,dx,
$$

the operator

$$
Lf=xf''+(1-x)f'
$$

is self-adjoint because $e^{-x}Lf=(xe^{-x}f')'$. Its eigenvalues on polynomials of degree at most $n$ are $0,-1,\ldots,-n$; its eigenvectors are scalar multiples of the [Laguerre polynomials](#laguerre-polynomial).

#### Laguerre polynomial

↑ **Parent:** [Laguerre differential operator on polynomials](#laguerre-differential-operator-on-polynomials)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laguerre_polynomial)

##### Generalized Laguerre polynomial

↑ **Parent:** [Laguerre polynomial](#laguerre-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_Laguerre_polynomial)

The generalized Laguerre polynomial $L_n^{(\alpha)}$ is orthogonal on $[0,\infty)$ for the weight $x^\alpha e^{-x}$ when $\alpha>-1$.

###### Rodrigues' formula

↑ **Parent:** [Generalized Laguerre polynomial](#generalized-laguerre-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rodrigues'_formula)

A Rodrigues formula constructs an orthogonal polynomial by differentiating a weight multiplied by a power. For generalized Laguerre polynomials,

$$
L_n^{(\alpha)}(x)
=\frac{x^{-\alpha}e^x}{n!}\frac{d^n}{dx^n}
\left(e^{-x}x^{n+\alpha}\right).
$$

## Real spectral theorem

↑ **Parent:** [Operator theory](linear-operator-theory.md)

Every real symmetric matrix is orthogonally diagonalizable. Distinct eigenspaces are orthogonal because symmetry gives $\lambda\langle u,v\rangle=\mu\langle u,v\rangle$.

## Power method

↑ **Parent:** [Operator theory](linear-operator-theory.md)

Iterate $q^{(k+1)}=Aq^{(k)}/\|Aq^{(k)}\|$. With a unique [dominant eigenvalue](#dominant-eigenvalue) separated by a [spectral gap](#spectral-gap) and a starting [vector](vector-space.md#vector) that is [nonorthogonal](linear-algebra.md#nonorthogonal-vectors) to its [eigenvector](#eigenvector), the directions converge at the spectral-ratio rate.

The power method is [power iteration](numerical-analysis.md#power-iteration); its convergence depends on the dominant spectral component of the starting vector.

### Dominant eigenpair extraction from a two-step Krylov recurrence

↑ **Parent:** [Power method](#power-method)

When two independent iterates span an invariant two-dimensional subspace, their recurrence gives the characteristic polynomial $\lambda^2-s\lambda+p$. For distinct roots $\lambda_1,\lambda_2$, corresponding eigenvectors are $y_{k+1}-\lambda_2y_k$ and $y_{k+1}-\lambda_1y_k$. For a merely approximately dominant subspace, the same computation gives approximate eigenpairs. A single orbit cannot separate a repeated eigenvalue's entire eigenspace when its projection is only one direction.

### Quadratic Rayleigh-quotient improvement for the power method

↑ **Parent:** [Power method](#power-method)

For a real symmetric matrix with $|\lambda_1|>|\lambda_2|$ and a starting vector having nonzero component in the leading eigendirection, power-method direction errors are

$$
O\!\left(\left|\frac{\lambda_2}{\lambda_1}\right|^k\right),
$$

whereas the [Rayleigh quotient](#rayleigh-quotient) error is

$$
O\!\left(\left|\frac{\lambda_2}{\lambda_1}\right|^{2k}\right).
$$

The improvement occurs because orthogonality cancels terms linear in the direction error.

### Active spectrum of the power method

↑ **Parent:** [Power method](#power-method)

The active spectrum consists of eigenvalues whose eigenspaces have nonzero projection of the starting vector. The power method converges toward the eigenvalue of largest modulus in this active spectrum; an exactly absent dominant component is never created in exact arithmetic.

### Inverse iteration

↑ **Parent:** [Power method](#power-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_iteration)

Inverse iteration repeatedly solves $(A-sI)y_{k+1}=q_k$ and normalizes. It is the power method for $(A-sI)^{-1}$ and converges toward an eigenvector whose eigenvalue is closest to the shift $s$.

#### Convergence of fixed-shift inverse iteration

↑ **Parent:** [Inverse iteration](#inverse-iteration)

If $A$ is real symmetric, $s$ is not an eigenvalue, one eigenvalue $\lambda_*$ is uniquely closest to $s$, and the initial vector has a nonzero component in its eigenspace, fixed-shift inverse iteration converges to that eigenspace. Its asymptotic direction-error ratio is

$$
\frac{|\lambda_*-s|}{|\lambda_{\rm next}-s|},
$$

where $\lambda_{\rm next}$ is second closest to $s$.

##### Sign behavior of fixed-shift inverse iteration

↑ **Parent:** [Convergence of fixed-shift inverse iteration](#convergence-of-fixed-shift-inverse-iteration)

If the closest eigenvalue $\lambda_*$ lies above the shift, the dominant eigenvalue $(\lambda_*-s)^{-1}$ of the inverse is positive and normalized iterates approach one fixed sign of its eigenvector. If $\lambda_*<s$, that inverse eigenvalue is negative, so the direction converges but consecutive normalized vectors alternate signs. At a shift exactly midway between two simple eigenvalues, the two inverse eigenvalues have equal modulus and opposite signs, so generic iterates alternate between two mixtures instead of selecting one eigenvector.

### Subspace iteration

↑ **Parent:** [Power method](#power-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subspace_iteration)

Subspace iteration repeatedly applies a matrix to several independent vectors and orthonormalizes them, converging to a dominant invariant subspace when a spectral gap separates the selected eigenvalue cluster.

#### Dominant invariant subspace

↑ **Parent:** [Subspace iteration](#subspace-iteration)

A dominant invariant subspace is spanned by eigenvectors whose eigenvalue moduli exceed those outside the subspace.

#### Power method with a dominant eigenvalue cluster

↑ **Parent:** [Subspace iteration](#subspace-iteration)

When several eigenvalues share the largest modulus, normalized power iterates need not converge individually, but every limit lies in their joint invariant subspace.

## Characteristic polynomial

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Characteristic_polynomial)

The characteristic polynomial is

$$
\chi_A(t)=\det(tI-A).
$$

Its roots are precisely the eigenvalues of $A$.

### Characteristic polynomials of AB and BA

↑ **Parent:** [Characteristic polynomial](#characteristic-polynomial)

For square matrices $A,B$ over a field,

$$
\det(tI-AB)=\det(tI-BA).
$$

If $A$ is invertible, the products are [similar matrices](linear-algebra.md#matrix-similarity). In general, apply that case to $(A-sI)B$ and $B(A-sI)$ for all but finitely many $s$, then use polynomial identity in $s$.

<h3 id="faddeev-leverrier-algorithm">Faddeev–LeVerrier algorithm</h3>

↑ **Parent:** [Characteristic polynomial](#characteristic-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Faddeev–LeVerrier_algorithm)

If

$$
\det(tI-A)=t^n+c_1t^{n-1}+\cdots+c_n,
$$

the Faddeev–LeVerrier algorithm computes the coefficients recursively from traces of powers:

$$
c_k=-\frac1k\left(\operatorname{tr}(A^k)+c_1\operatorname{tr}(A^{k-1})+\cdots+c_{k-1}\operatorname{tr}(A)\right).
$$

### Real parameter avoiding a singular matrix pencil

↑ **Parent:** [Characteristic polynomial](#characteristic-polynomial)

For real matrices $A,B$, $p(t)=\det(A+tB)$ is a real polynomial. If $p(i)\ne0$, it is not the zero polynomial, so some real $\lambda$ satisfies $p(\lambda)\ne0$.

### Triangularization over an algebraically closed field

↑ **Parent:** [Characteristic polynomial](#characteristic-polynomial)

Every square matrix over an algebraically closed field is similar to an upper-triangular matrix. Choose an eigenvector, extend it to a basis, and apply induction to the induced lower-right block.

## Eigenvalue interlacing

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eigenvalue_interlacing)

Eigenvalue interlacing bounds the ordered eigenvalues of a compressed or rank-modified operator between those of the original operator.

### Largest-eigenvalue interlacing for a principal submatrix

↑ **Parent:** [Eigenvalue interlacing](#eigenvalue-interlacing)

Let a real [symmetric matrix](linear-algebra.md#symmetric-matrix) $M$ have ordered [eigenvalues](#eigenvalue) $\lambda_1\ge\lambda_2\ge\cdots\ge\lambda_n$, with $n\ge2$. If $A$ is obtained by deleting one matching row and column, its largest eigenvalue $\mu_1$ satisfies

$$
\lambda_1\ge\mu_1\ge\lambda_2.
$$

The [Rayleigh quotient](#rayleigh-quotient) of $A$ is that of $M$ restricted to vectors whose deleted coordinate is zero. This gives the upper bound. Some nonzero linear combination of the top two orthonormal [eigenvectors](#eigenvector) has that coordinate zero; normalizing it gives a quotient at least $\lambda_2$. The argument does not require distinct eigenvalues.

## Jordan normal form

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jordan_normal_form)

### Unipotent involutions in characteristic two

↑ **Parent:** [Jordan normal form](#jordan-normal-form)

An involution in characteristic two has Jordan blocks of sizes at most two. Its conjugacy type is determined by the rank of $N$, subject to $2\operatorname{rank}N\le\dim V$. GL-conjugacy can split in SL if the centralizer determinant map is not onto; that issue must be checked separately. In $SL_3(4)$ a one-dimensional untouched block makes that determinant map onto, yielding one involution class. In $SL_4(2)=GL_4(2)$ the two possible nonzero ranks give two classes. Their projective quotients have equal order but different involution class counts.

### Density of diagonalizable complex matrices

↑ **Parent:** [Jordan normal form](#jordan-normal-form)

Perturb each diagonal position of a [Jordan normal form](#jordan-normal-form) matrix by a different arbitrarily small scalar, avoiding the finitely many collisions between diagonal entries. The resulting upper triangular matrix has distinct [eigenvalues](#eigenvalue), hence is [diagonalizable](#diagonalizable-matrix). Conjugate back to approximate any complex matrix. Continuous identities proved for [diagonalizable matrices](#diagonalizable-matrix) can therefore extend to all matrices.

### Repeated-eigenvalue classification in dimension two

↑ **Parent:** [Jordan normal form](#jordan-normal-form)

A complex two-dimensional linear operator whose two eigenvalues both equal $a$ is similar either to $aI$ or to $\begin{pmatrix}a&1\\0&a\end{pmatrix}$. Choose an eigenvector and complete it to a basis. The matrix becomes $\begin{pmatrix}a&c\\0&a\end{pmatrix}$ because its characteristic polynomial is $(t-a)^2$. A nonzero $c$ can be normalized to one by rescaling the first basis vector. The two types are distinguished by eigenspace dimension.

<h3 id="jordan-chevalley-decomposition">Jordan–Chevalley decomposition</h3>

↑ **Parent:** [Jordan normal form](#jordan-normal-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jordan–Chevalley_decomposition)

Over an [algebraically closed field](algebra.md#algebraically-closed-field), a [linear operator](vector-space.md#linear-operator) $X$ has a unique decomposition into a commuting [diagonalisable endomorphism](#diagonalizable-matrix) $X_s$ and [nilpotent endomorphism](#nilpotent-linear-map) $X_n$. On its [generalized eigenspace](#generalized-eigenspace) for $\lambda$, set $X_s=\lambda I$ and $X_n=X-\lambda I$. The [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) makes both parts polynomials in $X$, so they preserve every $X$-invariant subspace. Uniqueness follows by restricting any other commuting decomposition to those generalized eigenspaces. Over a perfect field the semisimple part need only become diagonalizable after scalar extension.

#### Adjoint compatibility of additive Jordan decomposition

↑ **Parent:** [Jordan–Chevalley decomposition](#jordan-chevalley-decomposition)

The [commutator](lie-algebra.md#commutator) action of $X_s$ is diagonalizable on [endomorphisms](algebra.md#endomorphism): on $\operatorname{Hom}(V_\lambda,V_\mu)$ it acts by $\mu-\lambda$. The action of $X_n$ is nilpotent by [nilpotence of commutation by a nilpotent endomorphism](#nilpotence-of-commutation-by-a-nilpotent-endomorphism). The two actions commute, so uniqueness of the [Additive Jordan decomposition](#jordan-chevalley-decomposition) identifies them as the parts of $\operatorname{ad}X$.

##### Semisimple matrix Lie algebras are closed under additive Jordan decomposition

↑ **Parent:** [Adjoint compatibility of additive Jordan decomposition](#adjoint-compatibility-of-additive-jordan-decomposition)

For a complex [semisimple Lie algebra](semisimple-lie-algebra.md) $\mathfrak g\subseteq\operatorname{End}(V)$ and $X\in\mathfrak g$, both parts of its [Additive Jordan decomposition](#jordan-chevalley-decomposition) lie in $\mathfrak g$. The polynomial semisimple part of $\operatorname{ad}X$ shows $X_s$ normalizes $\mathfrak g$. Split $\operatorname{End}(V)=\mathfrak g\oplus M$ by the [Weyl complete reducibility theorem](semisimple-lie-algebra.md#weyl-complete-reducibility-theorem); the $M$-component of $X_s$ centralizes $\mathfrak g$. On each irreducible summand of $V$ it is scalar by the [Schur lemma](representation-theory.md#schur-s-lemma). Its trace is zero because $\mathfrak g$ is a [perfect Lie algebra](semisimple-lie-algebra.md#perfect-lie-algebra) and the nilpotent part has zero trace, so those scalars vanish. Nonsemisimple subalgebras may fail this property: $\mathbb C(I+N)$ with $N\ne0$ nilpotent contains neither Jordan part of $I+N$.

### Algebraic multiplicity

↑ **Parent:** [Jordan normal form](#jordan-normal-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_multiplicity)

The algebraic multiplicity of an eigenvalue is its multiplicity as a root of the characteristic polynomial. In Jordan form it is the sum of the sizes of all blocks carrying that eigenvalue.

### Geometric multiplicity

↑ **Parent:** [Jordan normal form](#jordan-normal-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometric_multiplicity)

The geometric multiplicity of an eigenvalue is the dimension of its eigenspace. In Jordan form it equals the number of blocks carrying that eigenvalue.

### Jordan block

↑ **Parent:** [Jordan normal form](#jordan-normal-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jordan_block)

A Jordan block has one eigenvalue on its diagonal and ones on its superdiagonal.

#### Square-root splitting of a defective double eigenvalue

↑ **Parent:** [Jordan block](#jordan-block)

The model [matrix](vector-space.md#matrix) $B=\begin{pmatrix}0&1\\\epsilon&d\end{pmatrix}$ has a defective double [eigenvalue](#eigenvalue) when $d=\epsilon=0$. Its [characteristic polynomial](#characteristic-polynomial) is $\lambda^2-d\lambda-\epsilon$, giving the displayed roots. For fixed nonzero $d$ the small root is $-\epsilon/d+O(\epsilon^2)$ and the other is $d+\epsilon/d+O(\epsilon^2)$. These expansions cease to be ordered at $d=O(\sqrt\epsilon)$, the [distinguished limit](differential-equation.md#distinguished-limit) in which both roots split on a square-root scale. This is the generic leading behavior when a perturbation closes a two-dimensional [Jordan block](#jordan-block) through a nonzero lower-left entry; it need not occur for a perturbation that leaves that entry zero.

#### Nilpotent Jordan block

↑ **Parent:** [Jordan block](#jordan-block)

A nilpotent Jordan block has zeros on its diagonal and ones on its superdiagonal. Its $k$th power has ones on the $k$th superdiagonal, and a block of size $d$ satisfies $J_d(0)^d=0$.

### Jordan normal form of conjugation on two-by-two matrices

↑ **Parent:** [Jordan normal form](#jordan-normal-form)

If $\beta$ has eigenvalues $\lambda,\mu\ne0$ and is diagonalizable on a two-dimensional complex vector space, then

$$
\operatorname{JNF}(\phi_\beta)
=\operatorname{diag}\left(1,1,\frac\mu\lambda,\frac\lambda\mu\right).
$$

If $\beta$ has one size-two Jordan block, then

$$
\operatorname{JNF}(\phi_\beta)=J_3(1)\oplus J_1(1).
$$

### Characteristic and minimal polynomials determine similarity in dimension three

↑ **Parent:** [Jordan normal form](#jordan-normal-form)

Over an algebraically closed field, the characteristic polynomial gives the total size of the Jordan blocks for each eigenvalue, while the minimal polynomial gives the largest block size. For total dimension at most three, these two numbers determine the partition into block sizes: a multiplicity-three eigenvalue has partition $3$, $2+1$, or $1+1+1$ according as its largest block has size $3$, $2$, or $1$. Hence two matrices of size at most three with the same characteristic and minimal polynomials are similar.

### Generalized eigenvector

↑ **Parent:** [Jordan normal form](#jordan-normal-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_eigenvector)

A generalized eigenvector lies in the kernel of a positive power of A minus lambda I.

#### Jordan chain

↑ **Parent:** [Generalized eigenvector](#generalized-eigenvector)

A Jordan chain of a [linear operator](vector-space.md#linear-operator) $T$ for an [eigenvalue](#eigenvalue) $\lambda$ is a list of nonzero vectors satisfying $(T-\lambda I)v_1=0$ and $(T-\lambda I)v_j=v_{j-1}$ for $2\leq j\leq r$. These vectors are [linearly independent](vector-space.md#linear-independence): in a vanishing [linear combination](vector-space.md#linear-combination), applying the largest relevant power of $T-\lambda I$ isolates the last coefficient times $v_1$, then descending induction removes all coefficients. On their span the operator has one [Jordan block](#jordan-block). This is different from a [generalized eigenfunction](#generalized-eigenfunction) that solves $(T-\lambda I)u=0$ outside the original function space.

##### Length-two Jordan chain solution

↑ **Parent:** [Jordan chain](#jordan-chain)

If $(M-\lambda I)e=0$ and $(M-\lambda I)v=e$, the vector $v$ is a [generalized eigenvector](#generalized-eigenvector) and $e^{\lambda t}(v+te)$ solves $\dot x=Mx$. The polynomial factor distinguishes a nontrivial [Jordan block](#jordan-block) from an ordinary repeated eigenvalue with a full eigenvector [basis](vector-space.md#basis).

#### Generalized eigenspace

↑ **Parent:** [Generalized eigenvector](#generalized-eigenvector)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_eigenspace)

The generalized eigenspace of a [linear operator](vector-space.md#linear-operator) $A$ for an [eigenvalue](#eigenvalue) $\lambda$ is the union of the kernels $\ker(A-\lambda I)^N$. In finite dimension this union stabilizes for sufficiently large $N$.

##### Nilpotent commutator preserves generalized eigenspaces

↑ **Parent:** [Generalized eigenspace](#generalized-eigenspace)

For [endomorphisms](algebra.md#endomorphism) of a finite-dimensional complex [vector space](vector-space.md), suppose repeated commutation with $T$ annihilates $S$. Write the blocks of $S$ using the [generalized eigenspaces](#generalized-eigenspace) of $T$. On $\operatorname{Hom}(V_\lambda,V_\mu)$, the operator $\operatorname{ad}T$ is $(\mu-\lambda)I$ plus a [nilpotent endomorphism](#nilpotent-linear-map). If $\lambda\ne\mu$, it is invertible, so $(\operatorname{ad}T)^N S=0$ forces that off-diagonal block of $S$ to vanish. Thus $S$ preserves each [generalized eigenspace](#generalized-eigenspace). This allows a [nilpotent Lie algebra](lie-algebra.md#nilpotent-lie-algebra) representation to be split by generalized eigenvalues even when its acting operators do not commute.

#### Generalized eigenspaces for distinct eigenvalues form a direct sum

↑ **Parent:** [Generalized eigenvector](#generalized-eigenvector)

For a linear operator $f$, the generalized eigenspaces

$$
\ker(f-\alpha I)^n
$$

belonging to distinct eigenvalues are linearly independent. On the generalized $\alpha$-eigenspace, $f-\beta I=(\alpha-\beta)I+N$ is invertible for $\beta\ne\alpha$ because the nilpotent part $N$ has a finite geometric-series inverse.

## Generalized eigenvalue problem

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_eigenvalue_problem)

A generalized eigenvalue problem asks for a nonzero vector $v$ and scalar $\lambda$ satisfying $Av=\lambda Bv$. When $B$ is invertible, it is equivalent to the ordinary [eigenvalue](#eigenvalue) problem $B^{-1}Av=\lambda v$.

### Generalized characteristic polynomial

↑ **Parent:** [Generalized eigenvalue problem](#generalized-eigenvalue-problem)

The generalized characteristic polynomial of a matrix pair $(A,B)$ is $\det(A-\lambda B)$. Every finite generalized eigenvalue is one of its roots.

## Matrix exponential

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_exponential)

For a square matrix $A$, its exponential is the convergent power series

$$
e^{tA}=\sum_{k=0}^{\infty}\frac{t^kA^k}{k!}.
$$

It is the fundamental matrix for $y'=Ay$ and satisfies $e^{(s+t)A}=e^{sA}e^{tA}$.

### Skew-symmetric exponential as an axial rotation

↑ **Parent:** [Matrix exponential](#matrix-exponential)

For a nonzero real three-dimensional [skew-symmetric matrix](linear-algebra.md#skew-symmetric-matrix), choose real orthogonal vectors $u,v$ of equal length with $Au=\theta v$, $Av=-\theta u$ and $\theta>0$, and a real unit vector $e_3$ in its kernel. The [matrix exponential](#matrix-exponential) acts by $e^Au=u\cos\theta+v\sin\theta$, $e^Av=v\cos\theta-u\sin\theta$ and $e^Ae_3=e_3$. Its matrix in this [orthonormal basis](linear-algebra.md#orthonormal-basis) is a planar [rotation matrix](linear-algebra.md#rotation-matrix) with an unchanged axis. A purely imaginary nonzero [eigenvalue](#eigenvalue) and its complex [eigenvector](#eigenvector) give $u,v$ by taking real and imaginary parts; antisymmetry proves their equal norms and orthogonality.

### Derivative of the matrix exponential

↑ **Parent:** [Matrix exponential](#matrix-exponential)

This formula allows a [matrix](vector-space.md#matrix) and its derivative to fail to commute. Differentiate the absolutely convergent [power series](real-analysis.md#power-series) of the [matrix exponential](#matrix-exponential) to obtain $\sum_{k\geq1}k!^{-1}\sum_{j=0}^{k-1}f^jf'f^{k-1-j}$. Expanding the integral gives the same coefficients, since $\int_0^1(1-u)^au^b\,du=a!b!/(a+b+1)!$. The formula reduces to $e^ff'$ when $[f,f']=0$.

### Matrix exponential determinant identity

↑ **Parent:** [Matrix exponential](#matrix-exponential)

The [determinant](linear-algebra.md#determinant) is a smooth [Lie group homomorphism](lie-theory.md#lie-group-homomorphism) from the real [general linear group](group-theory.md#general-linear-group) to $\mathbb R^\times$. Its derivative at the identity is the [trace](linear-algebra.md#matrix-trace), and the flow-defined exponential on $\mathbb R^\times$ is the ordinary scalar exponential. [Naturality of the Lie group exponential](lie-theory.md#naturality-of-the-lie-group-exponential) therefore proves the identity without diagonalizability assumptions. The series $\sum_{k\geq0}t^kA^k/k!$ is the flow-defined [matrix exponential](#matrix-exponential) because it solves $E'=EA$, $E(0)=I$, and has inverse $E(-t)$.

### Matrix exponential when the square is minus the identity

↑ **Parent:** [Matrix exponential](#matrix-exponential)

If a real square matrix satisfies $M^2=-I$, split the absolutely convergent [matrix exponential](#matrix-exponential) into even and odd powers to obtain $e^{tM}=I\cos t+M\sin t$. It is the fundamental matrix for $\mathbf x'=M\mathbf x$. Consequently every solution has period $2\pi$, and the [eigenvalues](#eigenvalue) over the complex numbers belong to $\{i,-i\}$.

<h3 id="baker-campbell-hausdorff-formula">Baker--Campbell--Hausdorff formula</h3>

↑ **Parent:** [Matrix exponential](#matrix-exponential)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Baker–Campbell–Hausdorff_formula)

The Baker--Campbell--Hausdorff formula expresses the local [matrix logarithm](vector-space.md#matrix-logarithm) of a product of exponentials as

$$
\log(e^Xe^Y)=X+Y+\frac12[X,Y]+\frac1{12}[X,[X,Y]]+\frac1{12}[Y,[Y,X]]+\cdots.
$$

### Laplace transform of a matrix exponential

↑ **Parent:** [Matrix exponential](#matrix-exponential)

On its half-plane of convergence,

$$
\mathcal L\{e^{tA}\}(s)=(sI-A)^{-1}.
$$

Indeed, applying the transform to $y'=Ay$, $y(0)=y_0$, gives $(sI-A)Y=y_0$ for every $y_0$.

## Minimal polynomial

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Minimal_polynomial)

The minimal polynomial $m_A$ is the unique monic polynomial of least degree satisfying $m_A(A)=0$. It divides every polynomial that annihilates $A$.

### Characteristic and minimal polynomials of right multiplication

↑ **Parent:** [Minimal polynomial](#minimal-polynomial)

On two-by-two complex matrices let $\rho_A(X)=XA$. In row-entry coordinates, its matrix is $\operatorname{diag}(A^T,A^T)$, so its [characteristic polynomial](#characteristic-polynomial) is the square of that of $A$. For every polynomial $p$, $p(\rho_A)(X)=Xp(A)$. Thus $p(A)=0$ implies $p(\rho_A)=0$, and the reverse implication follows by taking $X=I$. The operators have exactly the same annihilating polynomials and hence the same [minimal polynomial](#minimal-polynomial). In general, right multiplication on $r$-by-$n$ matrices has characteristic polynomial $\chi_A^r$ and the same minimal polynomial.

### Real matrices have real minimal polynomials

↑ **Parent:** [Minimal polynomial](#minimal-polynomial)

The [minimal polynomial](#minimal-polynomial) of a real [matrix](vector-space.md#matrix), initially computed over the [complex numbers](complex-analysis.md#complex-number), has real coefficients. Its coefficientwise [complex conjugate](complex-analysis.md#complex-conjugate) is also a [monic polynomial](polynomial.md#monic-polynomial) of the same degree annihilating the [matrix](vector-space.md#matrix). Uniqueness of the [minimal polynomial](#minimal-polynomial) forces the two [polynomials](polynomial.md) to agree.

### Integer powers for an annihilating polynomial with roots one and minus one

↑ **Parent:** [Minimal polynomial](#minimal-polynomial)

If a square [matrix](vector-space.md#matrix) satisfies $(A-I)(A+I)^2=0$, then $A^{-1}=A^2+A-I$, and every integer [matrix power](vector-space.md#matrix-power) lies in the span of $I,A,A^2$. Writing $s=(-1)^n$, the universal formula is $A^n=\alpha_nA^2+\beta_nA+\gamma_nI$, where $\alpha_n=(1-s)/4+ns/2$, $\beta_n=(1-s)/2$ and $\gamma_n=(1+3s)/4-ns/2$. The polynomial $p_n(t)$ on the right satisfies $p_n(1)=1$, $p_n(-1)=(-1)^n$ and $p_n'(-1)=n(-1)^{n-1}$. These value and derivative conditions implement interpolation at a repeated root. For negative integers the inverse formula first puts $A^n$ in the same polynomial algebra; the nilpotent block identity $(I-N)^n=I-nN$ for $N^2=0$ proves the derivative rule for every integer.

### Minimal polynomial of an invertible matrix

↑ **Parent:** [Minimal polynomial](#minimal-polynomial)

A square matrix $A$ is [invertible](linear-algebra.md#invertible-matrix) exactly when its [minimal polynomial](#minimal-polynomial) has nonzero constant term. If $m_A(t)=tq(t)$, then $Aq(A)=0$, and invertibility would contradict the minimality of $m_A$. Conversely, if $m_A(t)=tq(t)+c$ with $c\ne0$, then $A[-q(A)/c]=I$.

### Minimal polynomials of AB and BA

↑ **Parent:** [Minimal polynomial](#minimal-polynomial)

For square matrices $A,B$,

$$
m_{BA}(t)\mid t,m_{AB}(t),
\qquad
m_{AB}(t)\mid t,m_{BA}(t).
$$

Indeed, $(BA)^{k+1}=B(AB)^kA$. Thus the two minimal polynomials have the same nonzero factors with the same multiplicities, while their powers of $t$ differ by at most one.

#### Similarity of squared matrix products with one diagonalizable product

↑ **Parent:** [Minimal polynomials of AB and BA](#minimal-polynomials-of-ab-and-ba)

The identity $(BA)^{j+1}=B(AB)^jA$ gives $m_{BA}(t)\mid t\,m_{AB}(t)$. If $AB$ is [diagonalizable](#diagonalizable-matrix), its [minimal polynomial](#minimal-polynomial) has simple roots. Hence all nonzero Jordan blocks of $BA$ have size one and its zero blocks have size at most two. Squaring kills these nilpotent blocks, making both squared products diagonalizable. Their eigenvalue multisets agree by [Characteristic polynomials of AB and BA](#characteristic-polynomials-of-ab-and-ba), so the squared products are [similar matrices](linear-algebra.md#matrix-similarity).

### Kernel decomposition for coprime polynomials

↑ **Parent:** [Minimal polynomial](#minimal-polynomial)

If $p_1,\ldots,p_r$ are pairwise coprime, then

$$
\ker\!\left(\prod_i p_i(A)\right)
=\bigoplus_i\ker p_i(A).
$$

Bezout identities between the factors construct the corresponding projections.

### Minimal polynomial bound from a triangular invariant flag

↑ **Parent:** [Minimal polynomial](#minimal-polynomial)

If an upper-triangular $n$ by $n$ matrix has diagonal entries $\lambda_1,\ldots,\lambda_n$, its standard invariant flag satisfies

$$
(A-\lambda_kI)V_k\subseteq V_{k-1}.
$$

The commuting product $\prod_k(A-\lambda_kI)$ therefore vanishes, proving $\deg m_A\leq n$ without invoking the full Cayley-Hamilton theorem.

## Jacobson lemma for a commuting commutator

↑ **Parent:** [Operator theory](linear-operator-theory.md)

Let $C=[B,A]$ and suppose $AC=CA$. Then $C$ is nilpotent. For the derivation $D(X)=[B,X]$, one has $D(p(A))=p'(A)C$. If $f(A)=0$, induction gives

$$
f^{(k)}(A)C^{2^k-1}=0.
$$

Indeed, if $uC^m=C^mu=0$, differentiating $uC^m=0$ and multiplying on the left by $C^m$ gives $C^mD(u)C^m=0$; for $u=f^{(k)}(A)$ this replaces $m$ by $2m+1$. Taking $k=\deg f$ makes $f^{(k)}$ a nonzero constant and proves nilpotence.

## Translation finite-difference operator

↑ **Parent:** [Operator theory](linear-operator-theory.md)

On all real-valued functions on $\mathbb R$, define $D_rf(x)=f(x+r)-f(x)$. The operators commute, and every real number except $-1$ is an eigenvalue. For eigenvalue $\lambda\ne-1$, values may be chosen independently on the cosets of $r\mathbb Z$ and extended by $f(x+r)=(1+\lambda)f(x)$, so every eigenspace is infinite-dimensional.

### Mixed finite difference of a polynomial

↑ **Parent:** [Translation finite-difference operator](#translation-finite-difference-operator)

If $p$ has degree $n$ and leading coefficient $a_n$, then for nonzero steps $r_1,\ldots,r_n$,

$$
D_{r_1}\cdots D_{r_n}p=n!a_n\prod_{i=1}^nr_i.
$$

Consequently a degree-$n$ polynomial cannot be the sum of $n$ functions each periodic with some nonzero period.

## Nilpotent linear map

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nilpotent_linear_map)

A [linear map](vector-space.md#linear-map) $T:V\to V$ is nilpotent if $T^k=0$ for some [positive integer](number-theory.md#positive-integer) $k$.

### Nilpotent matrix

↑ **Parent:** [Nilpotent linear map](#nilpotent-linear-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nilpotent_matrix)

A square [matrix](vector-space.md#matrix) is nilpotent when one of its positive powers is zero. It represents a [nilpotent linear map](#nilpotent-linear-map) in a chosen basis; changing basis preserves nilpotence. Over an algebraically closed field, its [Jordan normal form](#jordan-normal-form) has only zero-eigenvalue blocks.

#### Square-zero criterion for a two-by-two matrix

↑ **Parent:** [Nilpotent matrix](#nilpotent-matrix)

For a real or complex two-by-two [matrix](vector-space.md#matrix) $A$, the [Cayley-Hamilton theorem](mathematics.md#cayley-hamilton-theorem) reads $A^2-(\operatorname{tr}A)A+(\det A)I=0$. Hence $A^2=0$ exactly when $\operatorname{tr}A=\det A=0$. Conversely, if $A^m=0$ for any positive integer $m$, every [eigenvalue](#eigenvalue) is zero and the same identity gives $A^2=0$. Thus a nonzero [nilpotent matrix](#nilpotent-matrix) of this size has nilpotency index two.

#### Counting nilpotent matrices by the Fitting decomposition

↑ **Parent:** [Nilpotent matrix](#nilpotent-matrix)

There are $q^{n^2-n}$ [nilpotent matrices](#nilpotent-matrix) of size n over $F_q$. Every matrix has a unique invariant direct sum on which it is nilpotent and invertible. Counting those ordered decompositions gives $q^{n^2}/|GL_n(q)|=\sum_{k=0}^n a_k/|GL_k(q)|$. Subtraction at n and n−1 yields $a_n=q^{n^2-n}$. Translation by the identity counts [unipotent matrices](lie-theory.md#unipotent-matrix).

### Nilpotence of commutation by a nilpotent endomorphism

↑ **Parent:** [Nilpotent linear map](#nilpotent-linear-map)

For a [nilpotent endomorphism](#nilpotent-linear-map) $N$ of a [vector space](vector-space.md), the [commutator](lie-algebra.md#commutator) action $\operatorname{ad}N:T\mapsto NT-TN$ on its [endomorphisms](algebra.md#endomorphism) is nilpotent. The commuting left and right multiplication maps give $(\operatorname{ad}N)^r(T)=\sum_{j=0}^r(-1)^j\binom rjN^{r-j}TN^j$. If $N^q=0$ and $r\geq2q-1$, every summand vanishes. This works in every [characteristic of a field](algebra.md#characteristic-of-a-field) and is useful when applying [Engel theorem](lie-algebra.md#engel-s-theorem) to an [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra).

## Eigenvalue

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eigenvalue)

A [scalar](vector-space.md#scalar) $\lambda$ is an eigenvalue of a [linear operator](vector-space.md#linear-operator) $A$ when $Av=\lambda v$ for some nonzero [vector](vector-space.md#vector) $v$.

### Eigenvalue collision

↑ **Parent:** [Eigenvalue](#eigenvalue)

An eigenvalue collision occurs when distinct branches of [eigenvalues](#eigenvalue) coincide in a parameter-dependent family of [matrices](vector-space.md#matrix) or [linear operators](vector-space.md#linear-operator). The resulting repeated eigenvalue need not retain a full [eigenbasis](#eigenbasis); its geometric and algebraic multiplicities must be compared to decide [diagonalizability](#diagonalizable-matrix).

### Spectral abscissa

↑ **Parent:** [Eigenvalue](#eigenvalue)

The [spectral abscissa](#spectral-abscissa) is the largest real part of a [matrix](vector-space.md#matrix)'s [eigenvalues](#eigenvalue). It describes asymptotic exponential rates of its [matrix exponential](#matrix-exponential), but a [non-normal matrix](#non-normal-matrix) can also have transient amplification. It is generally distinct from the [Euclidean logarithmic norm](continuous-dual-space.md#euclidean-logarithmic-norm), which gives an immediate Euclidean energy-growth bound.

### Eigenvalue multiplicity

↑ **Parent:** [Eigenvalue](#eigenvalue)

Geometric multiplicity is the dimension of an [eigenspace](#eigenspace); algebraic multiplicity is its multiplicity as a root of the [characteristic polynomial](#characteristic-polynomial). For a real symmetric [matrix](vector-space.md#matrix) they coincide because it has an orthonormal eigenbasis.

### Zero eigenvalue

↑ **Parent:** [Eigenvalue](#eigenvalue)

Zero is an eigenvalue of a linear operator exactly when the operator has a nontrivial [kernel](linear-algebra.md#kernel-of-a-linear-map). Its eigenvectors are precisely the nonzero vectors in that kernel.

#### Spectrum of a three-dimensional matrix with zero row sums

↑ **Parent:** [Zero eigenvalue](#zero-eigenvalue)

Consider

$$
B=\begin{pmatrix}-(a+b)&a&b\\c&-(c+d)&d\\e&f&-(e+f)\end{pmatrix}.
$$

Its row sums vanish, so $(1,1,1)^T$ is an [eigenvector](#eigenvector) for the [zero eigenvalue](#zero-eigenvalue). Its [characteristic polynomial](#characteristic-polynomial) is

$$
\det(\lambda I-B)=\lambda(\lambda^2+S\lambda+T),\qquad S=a+b+c+d+e+f,
$$

with sum of [principal minors](vector-space.md#principal-minor) of order two

$$
T=ad+bc+bd+ae+af+bf+ce+cf+de.
$$

The other [eigenvalues](#eigenvalue) are $(-S\pm\sqrt{S^2-4T})/2$. No symmetry is required for this formula; [positive diagonal symmetrization of a matrix](linear-algebra.md#positive-diagonal-symmetrization-of-a-matrix) is a sufficient condition for real roots.

### Eigenvalue problem

↑ **Parent:** [Eigenvalue](#eigenvalue)

An eigenvalue problem asks for the [eigenvalues](#eigenvalue) and corresponding [eigenvectors](#eigenvector) or [eigenfunctions](#eigenfunction) of a [linear operator](vector-space.md#linear-operator). It is commonly written as the [eigenvalue equation](#eigenvalue-equation) $Av=\lambda v$.

### Eigenfunction

↑ **Parent:** [Eigenvalue](#eigenvalue)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eigenfunction)

An eigenfunction is a nonzero function $f$ satisfying $Lf=\lambda f$ for a linear operator $L$ and scalar [eigenvalue](#eigenvalue) $\lambda$.

#### Nodeless eigenfunction

↑ **Parent:** [Eigenfunction](#eigenfunction)

A nodeless real [eigenfunction](#eigenfunction) has no zero in the interior of the domain. For a one-dimensional confining [Schrödinger operator](physics.md#schrodinger-operator), the [nodeless theorem for a one-dimensional ground state](quantum-theory.md#nodeless-theorem-for-a-one-dimensional-ground-state) identifies the [ground state](quantum-mechanics.md#ground-state) as the eigenfunction that can be chosen strictly positive. Normalizable excited states have nodes.

#### Dirichlet eigenfunction

↑ **Parent:** [Eigenfunction](#eigenfunction)

A [Dirichlet eigenfunction](#dirichlet-eigenfunction) is an [eigenfunction](#eigenfunction) of a differential operator satisfying a homogeneous [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition). The term applies to more general boundary-value operators as well as the [Dirichlet Laplacian](partial-differential-equation.md#dirichlet-laplacian).

#### Adjoint eigenfunction

↑ **Parent:** [Eigenfunction](#eigenfunction)

An adjoint [eigenfunction](#eigenfunction) is a nonzero [eigenfunction](#eigenfunction) of the [adjoint operator](hilbert-space.md#adjoint-operator) on its adjoint domain. For an [inner product](linear-algebra.md#inner-product) conjugate-linear in its first argument, $L^*g=\overline\lambda g$ implies $\langle g,(L-\lambda)f\rangle=0$ for every $f$ in the domain of $L$. Consequently a necessary [solvability condition](#solvability-condition) for $(L-\lambda)f=h$ is $\langle g,h\rangle=0$. If $L-\lambda I$ is a [Fredholm operator](functional-analysis.md#fredholm-operator), orthogonality to every element of its adjoint kernel is also sufficient. [Boundary conditions](differential-equation.md#boundary-condition) and weights in a coupled system enter the adjoint domain and must be derived by [integration by parts](calculus.md#integration-by-parts); copying the original [eigenfunction](#eigenfunction) without checking them can give a wrong projection.

#### Generalized eigenfunction

↑ **Parent:** [Eigenfunction](#eigenfunction)

A generalized eigenfunction solves the [eigenvalue equation](#eigenvalue-equation) for a [linear operator](vector-space.md#linear-operator) in an enlarged space, often a space of [distributions](distribution-theory.md#distribution-mathematical-analysis), although it may fail to belong to the underlying [Hilbert space](hilbert-space.md). A [plane wave](quantum-mechanics.md#plane-wave) $e^{ikx}$ on the whole [real line](real-analysis.md#real-line) is a generalized [momentum eigenstate](quantum-mechanics.md#momentum-eigenstate), with [momentum](classical-mechanics.md#momentum) $\hbar k$, and is not [square-integrable](measure-theory.md#square-integrable-function). This usage differs from a [generalized eigenvector](#generalized-eigenvector) in a [Jordan chain](#jordan-chain), where a higher power of $L-\lambda$ vanishes rather than $L-\lambda$ itself.

### Eigenvector

↑ **Parent:** [Eigenvalue](#eigenvalue)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eigenvector)

A nonzero [vector](vector-space.md#vector) $v$ is an eigenvector of a [linear operator](vector-space.md#linear-operator) $A$ when $Av=\lambda v$ for some [eigenvalue](#eigenvalue) $\lambda$.

#### Zero mode

↑ **Parent:** [Eigenvector](#eigenvector)

A [zero mode](#zero-mode) is a nonzero eigenvector of an operator with eigenvalue zero. For a differential fluctuation operator it must also satisfy the specified [boundary conditions](differential-equation.md#boundary-condition). A zero mode prevents ordinary inversion of the operator and makes its unmodified [functional determinant](quantum-field-theory.md#functional-determinant) vanish. Gauge directions can produce zero modes of a kinetic operator, while stationary-path focusing can produce them in a semiclassical boundary-value problem. Removing, separately integrating or otherwise treating these directions is necessary before using a Gaussian determinant formula.

#### Independence of eigenvectors for distinct eigenvalues

↑ **Parent:** [Eigenvector](#eigenvector)

Applying the product of the other eigenvalue factors to a linear relation isolates each coefficient. Distinct [eigenvalues](#eigenvalue) therefore give [linearly independent](vector-space.md#linear-independence) [eigenvectors](#eigenvector). A complete eigenvector [basis](vector-space.md#basis) diagonalizes the associated [linear system of ordinary differential equations](differential-equation.md#linear-system-of-differential-equations).

#### Eigenvalue equation

↑ **Parent:** [Eigenvector](#eigenvector)

The eigenvalue equation $Av=\lambda v$ asks for a nonzero [eigenvector](#eigenvector) $v$ and its [eigenvalue](#eigenvalue) $\lambda$.

#### Right eigenvector

↑ **Parent:** [Eigenvector](#eigenvector)

A right eigenvector satisfies $Av=\lambda v$.

#### Left eigenvector

↑ **Parent:** [Eigenvector](#eigenvector)

A left eigenvector satisfies $u^TA=\lambda u^T$, equivalently $A^Tu=\lambda u$ over the real numbers.

### Eigenspace

↑ **Parent:** [Eigenvalue](#eigenvalue)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eigenspace)

The eigenspace for $\lambda$ is $\ker(A-\lambda I)$.

#### Real square roots of operators with simple real spectrum

↑ **Parent:** [Eigenspace](#eigenspace)

If a real [linear operator](vector-space.md#linear-operator) $A$ on an $n$-dimensional [vector space](vector-space.md) has $n$ distinct real [eigenvalues](#eigenvalue), any real square root $B$ commutes with $A$ and preserves each one-dimensional [eigenspace](#eigenspace). There $B$ is multiplication by a real $b_i$, hence $\lambda_i=b_i^2\geq0$. Conversely, if all the eigenvalues are nonnegative, choosing $b_i=\sqrt{\lambda_i}$ on an [eigenbasis](#eigenbasis) supplies a real square root. Without simple spectrum the necessity fails: a real quarter-turn squares to $-I$.

#### Laplacian eigenspace

↑ **Parent:** [Eigenspace](#eigenspace)

The [vector space](vector-space.md) of functions satisfying $\Delta f=\lambda f$ for a specified [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator). On a [closed manifold](differential-geometry.md#closed-manifold) its dimension is finite and is the spectral multiplicity of $\lambda$. A finite isometric [group action](group-theory.md#group-action) preserves this space; invariant elements are the [Laplacian eigenfunctions](partial-differential-equation.md#laplacian-eigenfunction) on the corresponding smooth quotient.

#### Eigenbasis

↑ **Parent:** [Eigenspace](#eigenspace)

An eigenbasis is a [basis](vector-space.md#basis) consisting of [eigenvectors](#eigenvector) of one operator.

### Simple eigenvalue

↑ **Parent:** [Eigenvalue](#eigenvalue)

An eigenvalue is simple when it has [algebraic multiplicity](#algebraic-multiplicity) one.

#### Eigenvalue sensitivity

↑ **Parent:** [Simple eigenvalue](#simple-eigenvalue)

For unit [left eigenvector](#left-eigenvector) $u$ and [right eigenvector](#right-eigenvector) $v$ of a real matrix at a [simple eigenvalue](#simple-eigenvalue) $\lambda$, its normwise sensitivity is

$$
s(\lambda)=\frac1{|u^Tv|}.
$$

It measures the first-order amplification of a matrix perturbation into an eigenvalue perturbation.

##### First-order perturbation of a simple eigenvalue

↑ **Parent:** [Eigenvalue sensitivity](#eigenvalue-sensitivity)

If $A(t)=A+tE$ and $\lambda(t)$ is a [differentiable function](analysis.md#differentiable-function) defining a simple eigenvalue, then

$$
\lambda'(0)=\frac{u^TEv}{u^Tv}.
$$

The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and the [operator norm](continuous-dual-space.md#operator-norm) give

$$
|\lambda'(0)|\leq\|E\|_2s(\lambda).
$$

### Diagonalizable matrix

↑ **Parent:** [Eigenvalue](#eigenvalue)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diagonalizable_matrix)

A matrix is diagonalizable exactly when its eigenvectors span the whole vector space.

#### Diagonalization of a matrix

↑ **Parent:** [Diagonalizable matrix](#diagonalizable-matrix)

A diagonalization is a factorization $A=PDP^{-1}$ in which $D$ is diagonal and the columns of $P$ form an eigenvector basis.

#### Diagonalizability inherited from an invertible power

↑ **Parent:** [Diagonalizable matrix](#diagonalizable-matrix)

Let $A$ be invertible over an algebraically closed field. If $A^m$ is diagonalizable for some $m>0$, then $A$ is diagonalizable. Indeed, a nontrivial Jordan block $A|_E=\lambda I+N$ has $\lambda\ne0$ and

$$
(\lambda I+N)^m=\lambda^mI+m\lambda^{m-1}N+\cdots.
$$

The first nonzero nilpotent term prevents this power from being diagonalizable.

#### Complex similarity of real matrices implies real similarity

↑ **Parent:** [Diagonalizable matrix](#diagonalizable-matrix)

Suppose real matrices $A,B$ satisfy $AP=PB$ for an invertible complex matrix $P=X+iY$. Then $AX=XB$ and $AY=YB$. The real polynomial $\det(X+tY)$ is not identically zero because its value at $t=i$ is nonzero, so some real $t$ makes $X+tY$ invertible. This real matrix intertwines $A$ and $B$.

#### Distinct eigenvalues imply diagonalizability

↑ **Parent:** [Diagonalizable matrix](#diagonalizable-matrix)

Eigenvectors belonging to distinct eigenvalues are linearly independent. Consequently, an $n$-dimensional operator with $n$ distinct eigenvalues is diagonalizable.

#### Spectral decomposition

↑ **Parent:** [Diagonalizable matrix](#diagonalizable-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spectral_decomposition)

A spectral decomposition expresses a [linear operator](vector-space.md#linear-operator) through its [eigenvalues](#eigenvalue) and projections onto its [eigenspaces](#eigenspace).

##### Dominant eigenvalue

↑ **Parent:** [Spectral decomposition](#spectral-decomposition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dominant_eigenvalue)

An [eigenvalue](#eigenvalue) is dominant when its [modulus](complex-analysis.md#modulus) is greater than or equal to that of every other eigenvalue. It is uniquely dominant when the inequality is strict.

##### Spectral gap

↑ **Parent:** [Spectral decomposition](#spectral-decomposition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spectral_gap)

A spectral gap is a positive separation between designated parts of the [spectrum](#spectrum-functional-analysis) of a [linear operator](vector-space.md#linear-operator). For the [power method](#power-method), the relevant gap separates the modulus of the [dominant eigenvalue](#dominant-eigenvalue) from the other eigenvalue moduli.

###### Ground-space perturbation bound

↑ **Parent:** [Spectral gap](#spectral-gap)

Suppose $H\geq0$ has ground energy zero and positive [spectral gap](#spectral-gap) at least $g$, and $0\leq V\leq I$. Let $\nu$ be the minimum of $V$ restricted to the [ground space](quantum-mechanics.md#ground-state-subspace). Splitting a normalized vector into ground and excited components bounds its energy below by $\delta\nu+(g-\delta)y^2-2\delta y$, with $y$ the excited norm. Completing the square yields the displayed bound for $0<\delta<g$. The error is controlled by the gap and cannot be treated as a uniform $O(\delta^2)$ when $g$ closes.

###### Davis-Kahan theorem

↑ **Parent:** [Spectral gap](#spectral-gap)

The Davis-Kahan theorem bounds the change of an invariant [eigenspace](#eigenspace) of a [symmetric matrix](linear-algebra.md#symmetric-matrix) in terms of a matrix perturbation and an appropriate [spectral gap](#spectral-gap). The [rank-one eigenprojector perturbation bound](#rank-one-eigenprojector-perturbation-bound) below depends only on the unperturbed gap. [Yu, Wang and Samworth's formulation](https://arxiv.org/abs/1405.0680) gives population-gap bounds in greater generality.

###### Davis-Kahan curvature lemma

↑ **Parent:** [Davis-Kahan theorem](#davis-kahan-theorem)

If a [symmetric matrix](linear-algebra.md#symmetric-matrix) $H$ has largest [eigenvalue](#eigenvalue) $\lambda_1$ separated from $\lambda_2$ by $\gamma>0$, and $P=vv^\top$ is its leading rank-one [orthogonal projection matrix](linear-algebra.md#orthogonal-projection-matrix), then every unit vector $u$, with $Q=uu^\top$, satisfies the displayed inequality. Expanding $u$ in an [orthonormal eigenbasis](#orthonormal-eigenbasis) gives $\lambda_1-u^\top Hu\geq\gamma(1-|u^\top v|^2)$, while $\|P-Q\|_F^2=2(1-|u^\top v|^2)$. The analogous statement for a smallest [eigenvalue](#eigenvalue) follows by replacing $H$ by $-H$.

###### Rank-one eigenprojector perturbation bound

↑ **Parent:** [Davis-Kahan curvature lemma](#davis-kahan-curvature-lemma)

Let $\widehat P$ project onto a leading unit [eigenvector](#eigenvector) of $H+W$, with $H$ as in the [Davis-Kahan curvature lemma](#davis-kahan-curvature-lemma). Its maximizing [Rayleigh quotient](#rayleigh-quotient) gives $\operatorname{tr}(H(P-\widehat P))\leq\operatorname{tr}(W(\widehat P-P))$. Duality of the [operator norm](continuous-dual-space.md#operator-norm) and [trace norm](functional-analysis.md#trace-norm), together with the rank-two bound $\|\widehat P-P\|_*\leq\sqrt2\|\widehat P-P\|_F$, proves the estimate. No gap condition on the perturbed matrix is needed.

## Conjugate transpose

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugate_transpose)

The adjoint of a complex matrix is its conjugate transpose,

$$
A^\dagger=\overline A^T.
$$

## Unitary matrix

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unitary_matrix)

A complex matrix is unitary when $U^\dagger U=UU^\dagger=I$. Its columns form an orthonormal basis, and it preserves inner products and norms.

### Hermitian parts of a unitary matrix

↑ **Parent:** [Unitary matrix](#unitary-matrix)

Every [unitary matrix](#unitary-matrix) has a unique decomposition $U=A+iB$ into [Hermitian matrices](hilbert-space.md#hermitian-operator). The formulas follow by adding and subtracting $U$ and its [conjugate transpose](#conjugate-transpose). Expanding $U^\dagger U=UU^\dagger=I$ gives $A^2+B^2+i(AB-BA)=I$ and $A^2+B^2-i(AB-BA)=I$. Therefore the parts commute and $A^2+B^2=I$.

## Skew-Hermitian matrix

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Skew-Hermitian_matrix)

A complex matrix $A$ is skew-Hermitian when $A^\dagger=-A$. Its [matrix exponential](#matrix-exponential) $e^{tA}$ is [unitary](#unitary-matrix) for every real $t$.

<h3 id="cross-product-model-of-su-2">Cross-product model of su(2)</h3>

↑ **Parent:** [Skew-Hermitian matrix](#skew-hermitian-matrix)

The real vector space of traceless [skew-Hermitian matrices](#skew-hermitian-matrix) of size two is the [Lie algebra](lie-algebra.md) $\mathfrak{su}(2)$. For the basis $M_1=\frac12\operatorname{diag}(i,-i)$, $M_2=\frac12\begin{pmatrix}0&1\\-1&0\end{pmatrix}$, $M_3=\frac12\begin{pmatrix}0&i\\i&0\end{pmatrix}$, cyclic [commutators](lie-algebra.md#commutator) satisfy $[M_1,M_2]=M_3$. The map $a\mapsto\sum a_jM_j$ carries the [cross product](vector-space.md#cross-product) to the [commutator](lie-algebra.md#commutator). Every target is a single commutator: choose a unit vector perpendicular to its associated vector $c$ and use $u\times(c\times u)=c$.

## Cayley transform of a Hermitian matrix

↑ **Parent:** [Operator theory](linear-operator-theory.md)

If $A$ is a [Hermitian matrix](hilbert-space.md#hermitian-operator), then $(I+iA)^{-1}(I-iA)$ is [unitary](#unitary-matrix). This Cayley transform maps each real eigenvalue $\lambda$ to the unit-modulus number $(1-i\lambda)/(1+i\lambda)$.

## Normal matrix

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_matrix)

A matrix is normal when $AA^\dagger=A^\dagger A$.

### Normal matrices have equal adjoint norms

↑ **Parent:** [Normal matrix](#normal-matrix)

For a [normal matrix](#normal-matrix), $N^\dagger N=NN^\dagger$. Consequently $\|Nx\|^2=x^\dagger N^\dagger Nx=x^\dagger NN^\dagger x=\|N^\dagger x\|^2$. In particular, $N$ and its [Hermitian conjugate](hilbert-space.md#hermitian-conjugation) have the same [kernel of a linear map](linear-algebra.md#kernel-of-a-linear-map).

<h3 id="hoffman-wielandt-inequality">Hoffman–Wielandt inequality</h3>

↑ **Parent:** [Normal matrix](#normal-matrix)

For two [normal matrices](#normal-matrix) of the same size, a pairing of their [eigenvalues](#eigenvalue) has squared Euclidean discrepancy at most the squared [Frobenius norm](compact-operator.md#frobenius-norm) of their difference. For [Hermitian matrices](hilbert-space.md#hermitian-operator), the increasing real [eigenvalue](#eigenvalue) order gives such a pairing, because it minimizes squared discrepancy. For real [symmetric matrices](linear-algebra.md#symmetric-matrix), the norm square is $\operatorname{Tr}(A-B)^2$.

#### Spectral Lipschitz bound from Frobenius distance

↑ **Parent:** [Hoffman–Wielandt inequality](#hoffman-wielandt-inequality)

For equally sized [Hermitian matrices](hilbert-space.md#hermitian-operator) and a real test [function](function.md) with [Lipschitz bound](real-analysis.md#lipschitz-bound) one, the difference of its averages under their [empirical spectral measures](probability-theory.md#empirical-spectral-measure) is at most $N^{-1/2}$ times the [Frobenius norm](compact-operator.md#frobenius-norm) of their difference. Pair the increasing [eigenvalues](#eigenvalue), apply the [triangle inequality](topological-analysis.md#triangle-inequality) and [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality), then use the [Hoffman–Wielandt inequality](#hoffman-wielandt-inequality).

### Adjoint eigenvector identity for a normal matrix

↑ **Parent:** [Normal matrix](#normal-matrix)

If a [normal matrix](#normal-matrix) satisfies $Ax=\lambda x$, then $A^\dagger x=\overline\lambda x$. Indeed, $M=A-\lambda I$ is normal and $\|Mx\|^2=x^\dagger M^\dagger Mx=x^\dagger MM^\dagger x=\|M^\dagger x\|^2$. Since $Mx=0$, also $M^\dagger x=0$. This identity proves orthogonality of distinct [eigenspaces](#eigenspace) and gives spectral restrictions for [Hermitian matrices](hilbert-space.md#hermitian-operator), [skew-Hermitian matrices](#skew-hermitian-matrix) and [unitary matrices](#unitary-matrix).

### Normality criterion for a two-mode shear model

↑ **Parent:** [Normal matrix](#normal-matrix)

For $A=\begin{pmatrix}-i\omega_1&a\\c&-i(\omega_1-b)\end{pmatrix}$ with real parameters,

$$
AA^\dagger-A^\dagger A=\begin{pmatrix}a^2-c^2&-ib(a+c)\\ib(a+c)&c^2-a^2\end{pmatrix}.
$$

Thus the displayed conditions are necessary and sufficient for a [normal matrix](#normal-matrix). In the family $a=1$, $b=c=q$, normality requires $q=-1$, not $q=1$. If $q=10/Re$, this is the formal value $Re=-10$ and no positive [Reynolds number](fluid-mechanics.md#reynolds-number) qualifies. At that value $A$ is a [skew-Hermitian matrix](#skew-hermitian-matrix) and its exponential is unitary, so every initial direction has [optimal energy amplification of a linear system](#optimal-energy-amplification-of-a-linear-system) equal to one.

### Matrix 2-norm of a normal matrix

↑ **Parent:** [Normal matrix](#normal-matrix)

For every finite-dimensional normal matrix $A$, the [matrix 2-norm](continuous-dual-space.md#matrix-2-norm) equals the [spectral radius](analysis.md#spectral-radius):

$$
\lVert A\rVert_2=\max_{\lambda\in\sigma(A)}|\lambda|=\rho(A).
$$

This follows by [unitary diagonalization of a normal matrix](#unitary-diagonalization-of-a-normal-matrix) and unitary invariance of the matrix 2-norm.

### Non-normal matrix

↑ **Parent:** [Normal matrix](#normal-matrix)

A matrix is non-normal when it does not commute with its adjoint. Its eigenvectors need not be orthogonal, so combinations of individually decaying modes may grow temporarily.

#### Nonnormal eigenvalues do not bound a quadratic quotient

↑ **Parent:** [Non-normal matrix](#non-normal-matrix)

The real [matrix](vector-space.md#matrix) $B_M=\begin{pmatrix}1&M\\0&1\end{pmatrix}$ has both [eigenvalues](#eigenvalue) equal to one, whereas $x^TB_Mx/(x^Tx)=1+M/2$ for $x=(1,1)^T$. Hence no universal constant bounds this quotient by the maximum [eigenvalue](#eigenvalue) of every real [matrix](vector-space.md#matrix) with real [eigenvalues](#eigenvalue).

#### Transient growth

↑ **Parent:** [Non-normal matrix](#non-normal-matrix)

Transient growth is finite-time amplification in a stable linear system. For a non-normal generator it can occur even when every eigenvalue has negative real part, because nonorthogonal eigenmodes can interfere constructively.

##### Optimal initial state for triangular stable shear

↑ **Parent:** [Transient growth](#transient-growth)

For $M=\begin{pmatrix}-1/R&0\\1&-2/R\end{pmatrix}$ with $R>0$, write $s=t/R$. Its [matrix exponential](#matrix-exponential) is $B=\begin{pmatrix}a&0\\R(a-a^2)&a^2\end{pmatrix}$, $a=e^{-s}$. The maximizing unit initial state is the largest-[eigenvalue](#eigenvalue) eigenvector of $B^*B$. Its component ratio is the displayed expression, with $d=(e^s+1)/(2R)+(R/2)(e^s-1)$. This follows by solving the quadratic eigenvector equation for the symmetric two-by-two Gram matrix. The state tends to $(1,0)^T$ for $t\gg R$.

###### Short-relative-time optimal state for triangular shear

↑ **Parent:** [Optimal initial state for triangular stable shear](#optimal-initial-state-for-triangular-stable-shear)

In the [optimal initial state for triangular stable shear](#optimal-initial-state-for-triangular-stable-shear), expansion of $e^{t/R}$ gives the displayed leading parameter with relative error $O(t/R)$. Keeping both terms distinguishes a large-$R$ shear regime from the limit $t\to0$ at fixed $R$. The latter direction is the largest-[eigenvalue](#eigenvalue) direction of the Hermitian part of $M$; the former can instead have large absolute time and substantial shear amplification even though $t/R$ is small.

##### Instantaneous energy-growth criterion for a linear system

↑ **Parent:** [Transient growth](#transient-growth)

For $x'=Lx$ and $E=\|x\|_2^2$, the [Hermitian matrix](hilbert-space.md#hermitian-operator) $H=(L+L^*)/2$ gives $\dot E=2x^*Hx$. Thus some initial condition grows immediately iff the largest [eigenvalue](#eigenvalue) of $H$ is positive. All trajectories have nonincreasing energy iff $H$ is a [negative semidefinite matrix](calculus.md#negative-semidefinite-matrix). This differs from requiring negative real parts for the [eigenvalues](#eigenvalue) of $L$: a [non-normal matrix](#non-normal-matrix) can satisfy modal decay while allowing [transient growth](#transient-growth).

##### Optimal energy amplification of a linear system

↑ **Parent:** [Transient growth](#transient-growth)

For the [matrix exponential](#matrix-exponential) $A(t)=e^{Lt}$, maximizing the energy ratio over nonzero initial conditions gives

$$
G(t)=\max_{x_0\ne0}\frac{x_0^*A(t)^*A(t)x_0}{x_0^*x_0}=\|A(t)\|_2^2=\sigma_{\max}(A(t))^2.
$$

The [Rayleigh quotient](#rayleigh-quotient) achieves its maximum at an [eigenvector](#eigenvector) of $A^*A$ with largest [eigenvalue](#eigenvalue), equivalently a [right singular vector](linear-algebra.md#right-singular-vector) of $A$. Such an optimal disturbance is generally not an [eigenvector](#eigenvector) of $L$.

##### Two-dimensional triangular model of transient growth

↑ **Parent:** [Transient growth](#transient-growth)

For $L=\begin{pmatrix}\lambda_1&0\\1&\lambda_2\end{pmatrix}$ with distinct real negative [eigenvalues](#eigenvalue), the [matrix exponential](#matrix-exponential) is $A=\begin{pmatrix}a&0\\b&d\end{pmatrix}$, where $a=e^{\lambda_1t}$, $d=e^{\lambda_2t}$ and $b=(a-d)/(\lambda_1-\lambda_2)$. The [optimal energy amplification of a linear system](#optimal-energy-amplification-of-a-linear-system) is

$$
G(t)=\frac{a^2+b^2+d^2+\sqrt{(a^2+b^2+d^2)^2-4a^2d^2}}2.
$$

Its [eigenvectors](#eigenvector) are [nonorthogonal](linear-algebra.md#nonorthogonal-vectors), and immediate energy growth occurs exactly when $\lambda_1\lambda_2<1/4$. If $\lambda_2>\lambda_1$, putting $\alpha=(\lambda_2-\lambda_1)^{-1}$ gives $G(t)\sim(1+\alpha^2)e^{2\lambda_2t}$. The optimal asymptotic initial direction $(\alpha,1)$ is an [adjoint eigenvector](#left-eigenvector), while the eventual state aligns with the right [eigenvector](#eigenvector) $(0,1)$.

###### Optimal time and gain of a Reynolds-scaled triangular model

↑ **Parent:** [Two-dimensional triangular model of transient growth](#two-dimensional-triangular-model-of-transient-growth)

For $L=\begin{pmatrix}-1/R&1\\0&-1/(4R)\end{pmatrix}$ with $R>1$, put $s=\sqrt{1-R^{-2}}$ and $q=(5-3s)/(5+3s)$. The [optimal energy amplification of a linear system](#optimal-energy-amplification-of-a-linear-system) reaches its maximum at

$$
T^*=-\frac{4R}{3}\log q,\qquad G_{\max}=\frac{1+s}{1-s}q^{5/3}.
$$

The maximizing initial orientation is $\rho^+$ and the final orientation is $\rho^-$ from the [orientation interval for transient energy growth](#orientation-interval-for-transient-energy-growth). Taking $R\to\infty$ gives the displayed viscous-time and Reynolds-squared asymptotics. These constants belong to this specified triangular model, not to every [non-normal matrix](#non-normal-matrix).

###### Orientation interval for transient energy growth

↑ **Parent:** [Two-dimensional triangular model of transient growth](#two-dimensional-triangular-model-of-transient-growth)

For $L=\begin{pmatrix}-1/R&1\\0&-1/(4R)\end{pmatrix}$ and $R>1$, write $\rho=x_2/x_1$. The energy derivative is $x_1^2[-1/R+\rho-\rho^2/(4R)]$, positive exactly between the displayed orientations. Linear trajectories cross the sector from $\rho^+$ to $\rho^-$ because $\dot\rho=\rho[3/(4R)-\rho]$. An [energy-neutral rotational nonlinearity](#energy-neutral-rotational-nonlinearity) can reverse the crossing direction; the growth sector itself remains the same.

###### Energy-neutral rotational nonlinearity

↑ **Parent:** [Two-dimensional triangular model of transient growth](#two-dimensional-triangular-model-of-transient-growth)

A nonlinear term $f(|x|)Nx$ with real skew-symmetric [matrix](vector-space.md#matrix) $N$ contributes zero to the derivative of the quadratic energy $|x|^2/2$. It changes orientation rather than magnitude directly. If a separate linear generator is a [non-normal matrix](#non-normal-matrix), that reorientation can still alter later [transient growth](#transient-growth), so energy cancellation alone does not make the nonlinear evolution equivalent to the linear one.

### Unitary diagonalization of a normal matrix

↑ **Parent:** [Normal matrix](#normal-matrix)

Every finite-dimensional complex normal matrix has an orthonormal eigenbasis, equivalently

$$
U^\dagger AU=D
$$

for some unitary $U$ and diagonal $D$.

## Schur decomposition

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur_decomposition)

Every complex square matrix is unitarily similar to an upper triangular matrix. The proof selects an eigenvector, extends it to an orthonormal basis, and applies induction to the compression on its orthogonal complement.

## Rayleigh quotient

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rayleigh_quotient)

For a self-adjoint operator $H$, the Rayleigh quotient is

$$
R[\psi]=\frac{\langle\psi|H|\psi\rangle}{\langle\psi|\psi\rangle}.
$$

For a symmetric matrix this reduces to $x^TAx/(x^Tx)$.

### Rayleigh quotient with one Neumann endpoint

↑ **Parent:** [Rayleigh quotient](#rayleigh-quotient)

For a nonzero real solution of $\phi''+(C-k^2)\phi=0$ on a finite interval, [integration by parts](calculus.md#integration-by-parts) gives $\mathcal R=\int(C\phi^2-\phi'^2)dz/\int\phi^2dz$ in the displayed form. A [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) only at the lower endpoint does not remove the upper boundary term. Equality with $k^2$ additionally requires $\phi(z_2)\phi'(z_2)=0$. With the lower condition, nonconstant oscillatory solutions satisfy this when their phase advance is an integer multiple of $\pi/2$; affine solutions must be constant, while nonzero hyperbolic-cosine solutions fail the condition. Infinite intervals additionally require convergence of both integrals.

### Hermitian Rayleigh quotient range

↑ **Parent:** [Rayleigh quotient](#rayleigh-quotient)

The [Rayleigh quotient](#rayleigh-quotient) of a finite-dimensional [Hermitian matrix](hilbert-space.md#hermitian-operator) ranges over its smallest-to-largest [eigenvalue](#eigenvalue) interval. In an [orthonormal basis](linear-algebra.md#orthonormal-basis) of [eigenvectors](#eigenvector) it is a weighted average of the [eigenvalues](#eigenvalue), with nonnegative weights summing to one. Combining the extreme [eigenvectors](#eigenvector) with coefficients $\sqrt{1-t},\sqrt t$ realizes every value of the interval.

### Odd variational trial gives an excited oscillator bound

↑ **Parent:** [Rayleigh quotient](#rayleigh-quotient)

An odd trial state is orthogonal to the even oscillator ground state. Its [Rayleigh quotient](#rayleigh-quotient) therefore bounds the first excited energy from above, unlike an arbitrary trial state. The kinetic [quadratic form](linear-algebra.md#quadratic-form) permits continuous compactly supported trials with [derivative](calculus.md#derivative) jumps.

### Generalized Rayleigh quotient

↑ **Parent:** [Rayleigh quotient](#rayleigh-quotient)

For symmetric $A$ and positive-definite $B$, the generalized Rayleigh quotient is $x^TAx/(x^TBx)$. Its stationary values are the [generalized eigenvalues](#generalized-eigenvalue-problem) of $Av=\lambda Bv$, and its maximum is the largest such eigenvalue.

### Rayleigh quotient iteration

↑ **Parent:** [Rayleigh quotient](#rayleigh-quotient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rayleigh_quotient_iteration)

Starting from a unit vector $v_k$, Rayleigh quotient iteration sets $\mu_k=R[v_k]$, solves

$$
(A-\mu_kI)w_k=v_k,
$$

and normalizes $v_{k+1}=w_k/\|w_k\|_2$. The shift $\mu_k$ is updated from the new vector.

#### Local cubic convergence of Rayleigh quotient iteration

↑ **Parent:** [Rayleigh quotient iteration](#rayleigh-quotient-iteration)

Let a real symmetric matrix have simple eigenpairs $(\lambda_i,w_i)$ and let

$$
x=c^{-1}\left(w_1+\epsilon\sum_{i\geq2}a_iw_i\right).
$$

Then its [Rayleigh quotient](#rayleigh-quotient) is

$$
R_A(x)=\lambda_1+\epsilon^2D+O(\epsilon^4),
\qquad
D=\sum_{i\geq2}a_i^2(\lambda_i-\lambda_1).
$$

After one shifted inverse solve and normalization, the relative coefficients are

$$
-\epsilon^3\frac{Da_i}{\lambda_i-\lambda_1}+O(\epsilon^5).
$$

Thus the eigenvector direction error is cubed at each sufficiently close iterate.

### Rayleigh-Ritz variational principle

↑ **Parent:** [Rayleigh quotient](#rayleigh-quotient)

The extremal Rayleigh quotients of a self-adjoint operator are the extremal spectral values. In particular, a Hamiltonian with a discrete spectrum satisfies $R[\psi]\geq E_0$, with equality precisely on its ground-state eigenspace. More generally, minimizing over states orthogonal to the first $j$ eigenspaces gives an upper bound on $E_j$.

#### Odd-state variational principle for an even potential

↑ **Parent:** [Rayleigh-Ritz variational principle](#rayleigh-ritz-variational-principle)

For a one-dimensional even potential, the ground state is even and the first excited state is odd. Every normalized odd trial wavefunction is therefore orthogonal to the ground state and gives

$$
E_1\leq\langle\psi_{\rm odd},H\psi_{\rm odd}\rangle.
$$

#### Gaussian variational bound for an attractive Gaussian well

↑ **Parent:** [Rayleigh-Ritz variational principle](#rayleigh-ritz-variational-principle)

For

$$
H=-\frac{d^2}{dx^2}-V_0e^{-x^2}
$$

and the trial state $\psi_a(x)=e^{-ax^2/2}$,

$$
E_0\leq E(a)
=\frac a2-V_0\sqrt{\frac a{1+a}}.
$$

This is negative for some $a>0$ for every $V_0>0$, proving that the attractive well has a bound state. For small $V_0$, taking $a=V_0^2$ gives

$$
-V_0<E_0\leq-\frac12V_0^2+O(V_0^4).
$$

#### Finite-subspace variational method

↑ **Parent:** [Rayleigh-Ritz variational principle](#rayleigh-ritz-variational-principle)

For an orthonormal trial set $\phi_1,\ldots,\phi_N$, the Rayleigh quotient on their span is

$$
\frac{\alpha^\dagger\mathcal H\alpha}{\alpha^\dagger\alpha},
\qquad
\mathcal H_{nm}=\langle\phi_n|H|\phi_m\rangle.
$$

Its minimum is the smallest eigenvalue of $\mathcal H$, which is therefore the optimal variational upper bound available in that trial subspace.

##### Two-mode variational bound for a linearly tilted square well

↑ **Parent:** [Finite-subspace variational method](#finite-subspace-variational-method)

For the first two sine modes in a width-$a$ infinite well with  
$V(x)=9\hbar^2x/(ma^3)$, the Hamiltonian in units $\hbar^2/(ma^2)$ is

$$
\begin{pmatrix}
(\pi^2+9)/2&-16/\pi^2\\
-16/\pi^2&(4\pi^2+9)/2
\end{pmatrix}.
$$

Its lower eigenvalue gives the upper bound

$$
E_0\leq\frac{\hbar^2}{ma^2}
\left[
\frac{5\pi^2+18}{4}
-\sqrt{\frac{9\pi^4}{16}+\frac{256}{\pi^4}}
\right].
$$

## Cyclic vector

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cyclic_vector)

A cyclic vector has iterates under an operator that span the whole vector space.

### Cyclic subspace

↑ **Parent:** [Cyclic vector](#cyclic-vector)

A [cyclic subspace](#cyclic-subspace) generated by $x$ under a [linear operator](vector-space.md#linear-operator) $T$ is the [span](vector-space.md#linear-span) of its successive iterates $x,Tx,T^2x,\ldots$. In finite dimension it is already generated by the first $n$ iterates. The first linear dependence expresses the next iterate in previous ones and proves invariance without using the [Cayley-Hamilton theorem](mathematics.md#cayley-hamilton-theorem).

## Companion matrix

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Companion_matrix)

A companion matrix represents multiplication by x in the power basis modulo a monic polynomial.

## Invariant direct-sum decomposition

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Invariant_direct-sum_decomposition)

An invariant direct-sum decomposition splits a space into nonzero subspaces preserved by the operator.

## Rational canonical form

↑ **Parent:** [Operator theory](linear-operator-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rational_canonical_form)

Rational canonical form expresses a linear map as a direct sum of companion matrices of invariant factors, and works over any field.

### Primary matrix centralizer formula

↑ **Parent:** [Rational canonical form](#rational-canonical-form)

For $M=\bigoplus_j(F_q[t]/(f^j))^{m_j}$ with $f$ irreducible of degree d and partition $\lambda=(j^{m_j})$, its automorphism group has order $q^{d\sum_i(\lambda'_i)^2}\prod_j\prod_{r=1}^{m_j}(1-q^{-dr})$. The [endomorphism](algebra.md#endomorphism) algebra has dimension $d\sum_{a,b}\min(a,b)m_am_b=d\sum_i(\lambda'_i)^2$; its semisimple quotient is $\prod_jM_{m_j}(F_{q^d})$, and units are precisely lifts of units in that quotient.

#### Counting matrices with a fixed primary polynomial

↑ **Parent:** [Primary matrix centralizer formula](#primary-matrix-centralizer-formula)

Fix an irreducible polynomial f of degree d with nonzero constant term. In $GL_{dm}(q)$, the number of matrices whose minimal polynomial is a power of f is $|GL_{dm}(q)|q^{d(m^2-m)}/|GL_m(q^d)|$. The [primary matrix centralizer formula](#primary-matrix-centralizer-formula) is identical to the unipotent centralizer formula over $F_{q^d}$, and summing reciprocal centralizer orders reduces to [counting nilpotent matrices by the Fitting decomposition](#counting-nilpotent-matrices-by-the-fitting-decomposition).

### Invariant factors of a linear operator

↑ **Parent:** [Rational canonical form](#rational-canonical-form)

For a finite-dimensional vector space regarded as an $F[X]$-module through a linear operator, the monic invariant factors $a_1\mid\cdots\mid a_k$ give the decomposition $\bigoplus_iF[X]/(a_i)$. Their product is the characteristic polynomial and the largest is the minimal polynomial.

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra.md)
2. [Algebra](algebra.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)
