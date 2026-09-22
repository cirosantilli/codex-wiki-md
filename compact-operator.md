# Compact operator

↑ **Parent:** [Functional analysis](functional-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compact_operator)

A bounded operator is compact when it maps the unit ball to a relatively compact set.

**Table of contents**

- [Compact L2 potential perturbation of the Dirichlet Laplacian](#compact-l2-potential-perturbation-of-the-dirichlet-laplacian)
- [Nondegenerate representations by compact operators](#nondegenerate-representations-by-compact-operators)
- [Compact operators send weak convergence to norm convergence](#compact-operators-send-weak-convergence-to-norm-convergence)
- [Norm-closedness of compact operators](#norm-closedness-of-compact-operators)
- [Schauder theorem for compact operators](#schauder-theorem-for-compact-operators)
- [Orthogonal eigenvectors of a compact operator](#orthogonal-eigenvectors-of-a-compact-operator)
- [Finite-rank approximation theorem for compact operators on a Hilbert space](#finite-rank-approximation-theorem-for-compact-operators-on-a-hilbert-space)
- [Fredholm alternative](#fredholm-alternative)
- [Hilbert-Schmidt operator](#hilbert-schmidt-operator)
  - [Compact averaging of a rank-one operator](#compact-averaging-of-a-rank-one-operator)
  - [Hilbert-Schmidt kernel bound](#hilbert-schmidt-kernel-bound)
  - [Hilbert-Schmidt norm](#hilbert-schmidt-norm)
    - [Frobenius norm](#frobenius-norm)
  - [Hilbert-Schmidt inner product](#hilbert-schmidt-inner-product)
    - [Rank bound for a weighted operator trace](#rank-bound-for-a-weighted-operator-trace)
    - [Hilbert-Schmidt distance](#hilbert-schmidt-distance)
  - [Trace-class operator](#trace-class-operator)
    - [Trace-class duality](#trace-class-duality)
    - [Fredholm determinant](#fredholm-determinant)
      - [Fredholm determinant of an exponential commutator](#fredholm-determinant-of-an-exponential-commutator)
    - [Hilbert-Schmidt factorization of a trace-class operator](#hilbert-schmidt-factorization-of-a-trace-class-operator)
    - [Schatten norm Hölder inequality](#schatten-norm-holder-inequality)
    - [Operator trace](#operator-trace)
      - [Trace duality](#trace-duality)
    - [Rank-one operator](#rank-one-operator)
- [Finite-rank operator](#finite-rank-operator)
  - [Finite-rank Fredholm alternative](#finite-rank-fredholm-alternative)
- [Spectral theorem for compact Hermitian operators](#spectral-theorem-for-compact-hermitian-operators)
  - [Courant–Fischer min-max principle](#courant-fischer-min-max-principle)
  - [Finite-rank truncation of a compact Hermitian operator](#finite-rank-truncation-of-a-compact-hermitian-operator)
- [Coordinate-projection approximation of a compact operator](#coordinate-projection-approximation-of-a-compact-operator)
- [Riesz–Schauder theorem](#riesz-schauder-theorem)
- [Finite-section approximation of a compact operator](#finite-section-approximation-of-a-compact-operator)
- [Compact resolvent](#compact-resolvent)
  - [Compact elliptic spectral theorem](#compact-elliptic-spectral-theorem)
    - [Eigenvalue counting function](#eigenvalue-counting-function)
  - [Imaginary Airy operator](#imaginary-airy-operator)

## Compact L2 potential perturbation of the Dirichlet Laplacian

↑ **Parent:** [Compact operator](compact-operator.md)

On a bounded open set, let $Tv\in W_0^{1,2}$ be the [weak solution](partial-differential-equation.md#weak-solution) of $\Delta Tv=v$. The energy estimate bounds $T:L^2\to W_0^{1,2}$. For $p>n$, put $q=2p/(p-2)<2n/(n-2)$. The zero-boundary [Rellich-Kondrachov compactness theorem](sobolev-space.md#rellich-kondrachov-theorem) gives compact embedding into $L^q$, and [Hölder's inequality](real-analysis.md#holder-s-inequality) gives $\|wz\|_2\leq\|w\|_p\|z\|_q$. Hence $Kv=wTv$ is compact on $L^2$, without a regularity assumption on the boundary. Writing $v=\Delta u$ makes $\Delta u-wu=f$ equivalent to $(I-K)v=f$. The [Fredholm alternative for a compact operator](#fredholm-alternative) then identifies unique solvability with triviality of the homogeneous kernel.

## Nondegenerate representations by compact operators

↑ **Parent:** [Compact operator](compact-operator.md)

A nondegenerate star-algebra of [compact operators](compact-operator.md) decomposes its [Hilbert space](hilbert-space.md) into irreducible closed reducing subspaces, each equivalence class occurring finitely many times. Pass to its norm closure. A nonzero compact positive element supplies a finite-rank spectral projection; a minimal projection in its finite-dimensional corner has scalar corner algebra. A cyclic vector in its range generates an irreducible reducing subspace. A maximal orthogonal family exhausts the space by nondegeneracy. Infinitely many equivalent copies would give orthogonal unit vectors whose images under some compact algebra element have equal nonzero norms, contradicting compactness.

## Compact operators send weak convergence to norm convergence

↑ **Parent:** [Compact operator](compact-operator.md)

For a bounded operator $K$ between [Hilbert spaces](hilbert-space.md), compactness is equivalent to $f_n\rightharpoonup f$ implying $Kf_n\to Kf$ in norm. The [Uniform boundedness principle](banach-space.md#uniform-boundedness-principle) bounds a weakly convergent sequence. Relative compactness of its images and the unique possible weak limit then give norm convergence. Conversely, every bounded domain sequence has a weakly convergent subsequence, so the image of the [unit ball](functional-analysis.md#unit-ball) is relatively compact.

## Norm-closedness of compact operators

↑ **Parent:** [Compact operator](compact-operator.md)

An [operator norm](continuous-dual-space.md#operator-norm) limit of compact operators between [Banach spaces](banach-space.md) is compact. Approximate the image of the unit ball by the image under one compact operator and transfer a finite epsilon-net across the small operator-norm error.

## Schauder theorem for compact operators

↑ **Parent:** [Compact operator](compact-operator.md)

A bounded operator $T:X\to Y$ between [Banach spaces](banach-space.md) is compact if and only if its [dual map of bounded linear operator](continuous-dual-space.md#transpose-of-a-bounded-linear-operator) $T^*:Y^*\to X^*$ is compact.

## Orthogonal eigenvectors of a compact operator

↑ **Parent:** [Compact operator](compact-operator.md)

If $Tx_j=\lambda_jx_j$ for an infinite orthonormal sequence $(x_j)$ and a compact operator $T$ on a [Hilbert space](hilbert-space.md), then $\lambda_j\to0$. Otherwise a subsequence of the vectors $Tx_j$ stays pairwise separated, contradicting compactness.

## Finite-rank approximation theorem for compact operators on a Hilbert space

↑ **Parent:** [Compact operator](compact-operator.md)

Every compact operator on a Hilbert space is an operator-norm limit of finite-rank operators. Cover the compact closure of the image of the unit ball by finitely many small balls, span their centres by a finite-dimensional space $E$, and approximate $T$ by $P_ET$.

## Fredholm alternative

↑ **Parent:** [Compact operator](compact-operator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fredholm_alternative)

If $T$ is compact and $\lambda\ne0$, then $T-\lambda I$ is injective exactly when it is surjective. Equivalently, every nonzero point of the spectrum of $T$ is an eigenvalue. Compactness turns an approximate eigenvector sequence into a convergent eigenvector sequence.

## Hilbert-Schmidt operator

↑ **Parent:** [Compact operator](compact-operator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert–Schmidt_operator)

A bounded [linear operator](vector-space.md#linear-operator) on a [Hilbert space](hilbert-space.md) is Hilbert-Schmidt when $\sum_n\|Te_n\|^2<\infty$ for one, equivalently every, [orthonormal basis](linear-algebra.md#orthonormal-basis). Every Hilbert-Schmidt operator is a [compact operator](compact-operator.md).

### Compact averaging of a rank-one operator

↑ **Parent:** [Hilbert-Schmidt operator](#hilbert-schmidt-operator)

For a strongly continuous [unitary representation](representation-theory.md#unitary-representation) of a [compact group](topological-group.md#compact-group), this [Bochner integral](measure-theory.md#bochner-integral) exists in the [Hilbert-Schmidt norm](#hilbert-schmidt-norm) and is a positive [compact operator](compact-operator.md) commuting with the representation. It is nonzero if $\xi\ne0$, because $\langle K_\xi\xi,\xi\rangle=\int_G|\langle U_g\xi,\xi\rangle|^2\,dg>0$. A nonzero [eigenspace](linear-operator-theory.md#eigenspace) is finite-dimensional and invariant. Applying this on [orthogonal complements](hilbert-space.md#orthogonal-complement) yields an [orthogonal direct sum](vector-space.md#orthogonal-direct-sum) of finite-dimensional [irreducible representations](representation-theory.md#irreducible-representation), with no separability assumption on the represented [Hilbert space](hilbert-space.md).

### Hilbert-Schmidt kernel bound

↑ **Parent:** [Hilbert-Schmidt operator](#hilbert-schmidt-operator)

For $(Tg)(v)=\int k(v,w)g(w)\,dw$, the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\|Tg\|_2\leq\|k\|_{L^2(v,w)}\|g\|_2$. The kernel norm is the [Hilbert-Schmidt norm](#hilbert-schmidt-norm), which bounds the [operator norm](continuous-dual-space.md#operator-norm). Uniform kernel bounds apply also to spatially parametrized operators after integrating over position.

### Hilbert-Schmidt norm

↑ **Parent:** [Hilbert-Schmidt operator](#hilbert-schmidt-operator)

The Hilbert-Schmidt norm of a [Hilbert-Schmidt operator](#hilbert-schmidt-operator) is the square root of the displayed sum. The value is independent of the [orthonormal basis](linear-algebra.md#orthonormal-basis), by the [Parseval identity](fourier-analysis.md#parseval-identity). For a finite [matrix](vector-space.md#matrix), it is the [Frobenius norm](#frobenius-norm).

#### Frobenius norm

↑ **Parent:** [Hilbert-Schmidt norm](#hilbert-schmidt-norm)

The Frobenius norm is the finite-matrix [Hilbert-Schmidt norm](#hilbert-schmidt-norm). It equals $\sqrt{\operatorname{tr}(A^*A)}$, is unchanged by unitary multiplication on either side, and is the square root of the sum of squared singular values. For unit vectors $u,v$, $\|uu^*-vv^*\|_F^2=2(1-|u^*v|^2)$, a useful sign-invariant measure of distance between rank-one [orthogonal projection matrices](linear-algebra.md#orthogonal-projection-matrix).

### Hilbert-Schmidt inner product

↑ **Parent:** [Hilbert-Schmidt operator](#hilbert-schmidt-operator)

For [Hilbert-Schmidt operators](#hilbert-schmidt-operator) $A$ and $B$, the Hilbert-Schmidt inner product is $\langle A,B\rangle_{\mathrm{HS}}=\operatorname{tr}(A^*B)$. Its induced norm is the [Hilbert-Schmidt norm](#hilbert-schmidt-norm).

#### Rank bound for a weighted operator trace

↑ **Parent:** [Hilbert-Schmidt inner product](#hilbert-schmidt-inner-product)

If $\rho$ is a [density operator](quantum-theory.md#density-matrix) with decreasing [eigenvalues](linear-operator-theory.md#eigenvalue) $\lambda_j$ and $T$ has [matrix rank](vector-space.md#matrix-rank) at most $k$, let $\Pi$ project onto the image of $T$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) for the [Hilbert-Schmidt inner product](#hilbert-schmidt-inner-product) gives

$$
|\operatorname{Tr}(\rho T)|^2\leq\operatorname{Tr}(\rho\Pi)\operatorname{Tr}(\rho T^\dagger T).
$$

The [Hermitian effect variational principle](mathematical-optimization.md#hermitian-effect-variational-principle) bounds $\operatorname{Tr}(\rho\Pi)$ by $\sum_{j<k}\lambda_j$, proving the claimed estimate without assuming $\rho$ is invertible.

#### Hilbert-Schmidt distance

↑ **Parent:** [Hilbert-Schmidt inner product](#hilbert-schmidt-inner-product)

The Hilbert-Schmidt distance is $d_{\mathrm{HS}}(A,B)=\lVert A-B\rVert_{\mathrm{HS}}$.

### Trace-class operator

↑ **Parent:** [Hilbert-Schmidt operator](#hilbert-schmidt-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trace-class_operator)

A bounded operator $T$ on a separable Hilbert space is trace class when $|T|^{1/2}$ is Hilbert--Schmidt. Its trace norm is

$$
\|T\|_1=\bigl\||T|^{1/2}\bigr\|_{\mathrm{HS}}^2
=\sum_n\langle|T|e_n,e_n\rangle.
$$

#### Trace-class duality

↑ **Parent:** [Trace-class operator](#trace-class-operator)

The dual of the [trace-class operators](#trace-class-operator), and also of the normed space of [finite-rank operators](#finite-rank-operator) with the [trace norm](functional-analysis.md#trace-norm), is isometrically the space of [bounded operators](topological-vector-space.md#continuous-linear-operator). The pairing is $F_B(T)=\operatorname{Tr}(BT)$. For $R_{x,y}z=\langle z,y\rangle x$, one has $\|R_{x,y}\|_1=\|x\|\|y\|$ and $F_B(R_{x,y})=\langle Bx,y\rangle$, using an [inner product](linear-algebra.md#inner-product) linear in its first argument. A bounded functional on these [rank-one operators](#rank-one-operator) gives a bounded [sesquilinear form](linear-algebra.md#sesquilinear-form) and hence a unique $B$ by the [Riesz representation theorem](hilbert-space.md#riesz-representation-theorem). The [singular value decomposition](linear-algebra.md#singular-value-decomposition) proves $\|F_B\|=\|B\|$ and the [triangle inequality](topological-analysis.md#triangle-inequality) for the [trace norm](functional-analysis.md#trace-norm).

#### Fredholm determinant

↑ **Parent:** [Trace-class operator](#trace-class-operator)

For a trace-class operator $K$ on a [Hilbert space](hilbert-space.md), the Fredholm determinant is the convergent product over its eigenvalues, counted with algebraic multiplicity. For self-adjoint $K$, [spectral theorem for compact self-adjoint operators](#spectral-theorem-for-compact-hermitian-operators) reduces the product to a diagonal calculation. For $\|K\|<1$, $\log\det(I+K)=\sum_{n\geq1}(-1)^{n+1}\operatorname{tr}(K^n)/n$. This identity exposes the successive [cumulants](probability-theory.md#cumulant) in a [Gaussian quadratic exponential moment](stochastic-process.md#gaussian-quadratic-exponential-moment).

##### Fredholm determinant of an exponential commutator

↑ **Parent:** [Fredholm determinant](#fredholm-determinant)

For bounded operators with trace-class commutator, the multiplicative commutator differs from identity by a [trace-class operator](#trace-class-operator). Along $F(t)=e^{tA}e^Be^{-tA}e^{-B}$, the trace of its logarithmic derivative is the constant $\operatorname{Tr}[A,B]$. This follows by writing $e^BAe^{-B}-A$ as the integral of conjugates of $[B,A]$ and using trace invariance under bounded similarities. Integrating the [Fredholm determinant](#fredholm-determinant) derivative from $F(0)=I$ proves the formula. Individual traces of $A$ and $B$ need not exist.

#### Hilbert-Schmidt factorization of a trace-class operator

↑ **Parent:** [Trace-class operator](#trace-class-operator)

An operator is trace class exactly when it factors as $T=AB$ with $A$ and $B$ Hilbert--Schmidt. The factors can be chosen so that $\|T\|_1=\|A\|_{\mathrm{HS}}\|B\|_{\mathrm{HS}}$ by using the [polar decomposition of a bounded operator](banach-algebra.md#polar-decomposition-of-a-bounded-operator).

<h4 id="schatten-norm-holder-inequality">Schatten norm Hölder inequality</h4>

↑ **Parent:** [Trace-class operator](#trace-class-operator)

The Schatten norm Hölder inequality gives $\lVert AB\rVert_r\leq\lVert A\rVert_p\lVert B\rVert_q$ when $1/r=1/p+1/q$. In particular, the product of two [Hilbert-Schmidt operators](#hilbert-schmidt-operator) is trace class and

$$
\lVert AB\rVert_1\leq\lVert A\rVert_{\mathrm{HS}}\lVert B\rVert_{\mathrm{HS}}.
$$

#### Operator trace

↑ **Parent:** [Trace-class operator](#trace-class-operator)

For a trace-class operator, the series $\operatorname{tr}T=\sum_n\langle Te_n,e_n\rangle$ converges absolutely and is independent of the orthonormal basis. It satisfies $|\operatorname{tr}T|\leq\|T\|_1$.

The [trace-class operator](#trace-class-operator) condition makes this [operator trace](#operator-trace) well-defined; the class of eligible operators and the trace functional are distinct concepts.

##### Trace duality

↑ **Parent:** [Operator trace](#operator-trace)

Every bounded operator $S$ defines a functional $T\mapsto\operatorname{tr}(ST)$ on the trace-class operators, and

$$
\|S\|=\sup_{\|T\|_1\leq1}|\operatorname{tr}(ST)|.
$$

Finite-rank density in $\mathcal S_1$ makes every continuous functional arise uniquely this way.

#### Rank-one operator

↑ **Parent:** [Trace-class operator](#trace-class-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rank-one_operator)

For vectors $x,y$ in a Hilbert space, the rank-one operator $(x\otimes y)z=\langle z,y\rangle x$ has $\|x\otimes y\|_1=\|x\|\|y\|$ and $\operatorname{tr}(x\otimes y)=\langle x,y\rangle$.

## Finite-rank operator

↑ **Parent:** [Compact operator](compact-operator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite-rank_operator)

A finite-rank operator has finite-dimensional image and is compact.

### Finite-rank Fredholm alternative

↑ **Parent:** [Finite-rank operator](#finite-rank-operator)

For a finite-rank operator $S$ and $\lambda\ne0$, if $\lambda$ is not an eigenvalue then $S-\lambda I$ is surjective. Decompose the Hilbert space into $\operatorname{im}S$ and its orthogonal complement, then use injectivity and surjectivity equivalence on the finite-dimensional image.

## Spectral theorem for compact Hermitian operators

↑ **Parent:** [Compact operator](compact-operator.md)

A compact Hermitian operator has real nonzero eigenvalues of finite multiplicity, with zero as their only possible accumulation point, and an orthonormal eigenbasis after a basis of its kernel is included.

This is the discrete-eigenbasis case of the [spectral theorem](hilbert-space.md#spectral-theorem) for a [compact operator](compact-operator.md) that is self-adjoint.

<h3 id="courant-fischer-min-max-principle">Courant–Fischer min-max principle</h3>

↑ **Parent:** [Spectral theorem for compact Hermitian operators](#spectral-theorem-for-compact-hermitian-operators)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Courant–Fischer_min-max_principle)

For a compact positive self-adjoint operator $T$ with decreasing eigenvalues $\lambda_1\geq\lambda_2\geq\cdots$, the Courant–Fischer principle gives

$$
\lambda_k
=\min_{\dim V=k-1}\max_{\substack{x\perp V\\\lVert x\rVert=1}}
\langle Tx,x\rangle.
$$

In particular, $S\geq T$ in quadratic-form order implies $\lambda_k(S)\geq\lambda_k(T)$ for every $k$.

### Finite-rank truncation of a compact Hermitian operator

↑ **Parent:** [Spectral theorem for compact Hermitian operators](#spectral-theorem-for-compact-hermitian-operators)

If

$$
Tx=\sum_n\lambda_n\langle x,e_n\rangle e_n,
\qquad \lambda_n\to0,
$$

then truncating the sum after $N$ terms gives finite-rank Hermitian $T_N$ with

$$
\lVert T-T_N\rVert=\sup_{n>N}|\lambda_n|\to0.
$$

## Coordinate-projection approximation of a compact operator

↑ **Parent:** [Compact operator](compact-operator.md)

Let $P_N$ project $\ell^2$ onto its first $N$ coordinates. Although $P_N\to I$ only strongly on the whole unit ball, convergence is uniform on every compact subset. Hence compact $T$ satisfies

$$
\lVert P_NT-T\rVert\to0,
$$

and each $P_NT$ has finite rank.

<h2 id="riesz-schauder-theorem">Riesz–Schauder theorem</h2>

↑ **Parent:** [Compact operator](compact-operator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riesz–Schauder_theorem)

Every nonzero spectral point of a compact operator is an isolated eigenvalue of finite algebraic multiplicity, and zero is the only possible accumulation point of the spectrum.

## Finite-section approximation of a compact operator

↑ **Parent:** [Compact operator](compact-operator.md)

If finite-rank orthogonal projections $P_n$ converge strongly to the identity and $A$ is compact, then $\lVert A-P_nAP_n\rVert\to0$. The finite-section spectra converge to $\operatorname{Sp}(A)$ in Hausdorff distance, including for nonnormal $A$.

## Compact resolvent

↑ **Parent:** [Compact operator](compact-operator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compact_resolvent)

A closed densely defined operator has compact resolvent when $(A-zI)^{-1}$ is compact at one, equivalently every, resolvent point. Its spectrum consists only of isolated eigenvalues of finite multiplicity, with possible accumulation only at infinity.

### Compact elliptic spectral theorem

↑ **Parent:** [Compact resolvent](#compact-resolvent)

On a [closed manifold](differential-geometry.md#closed-manifold) with a [Riemannian metric](differential-geometry.md#riemannian-metric) the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) is [self-adjoint](linear-operator-theory.md#self-adjoint-operator) with [compact resolvent](#compact-resolvent). It has a complete smooth [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis), finite-dimensional [eigenspaces](linear-operator-theory.md#eigenspace), nonnegative [eigenvalues](linear-operator-theory.md#eigenvalue) tending to infinity, and polynomial eigenvalue-counting bounds. [Elliptic regularity](distribution-theory.md#elliptic-regularity) bounds derivatives of its [eigenfunctions](linear-operator-theory.md#eigenfunction) polynomially in their [eigenvalues](linear-operator-theory.md#eigenvalue).

#### Eigenvalue counting function

↑ **Parent:** [Compact elliptic spectral theorem](#compact-elliptic-spectral-theorem)

For a nonnegative [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) with [compact resolvent](#compact-resolvent), this function counts [eigenvalues](linear-operator-theory.md#eigenvalue) up to a given level with their multiplicities. For the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) on a closed $n$-dimensional [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), $N(\Lambda)\leq C(1+\Lambda)^{n/2}$. To prove this bound, multiply each vector in the low-eigenvalue subspace by a finite set of chart cutoffs and record its local [Fourier coefficients](fourier-series.md#fourier-coefficient) of frequency at most $R$. The total number of retained coefficients is $O(R^n)$, while the sum of discarded squared norms is at most $CR^{-2}(1+\Lambda)\|u\|_2^2$ by [Parseval identity](fourier-analysis.md#parseval-identity) and the energy bound. For $R$ a sufficiently large multiple of $\sqrt{1+\Lambda}$, vanishing of all recorded coefficients forces $u=0$. The recording map is injective and proves the dimension bound. Inverting this estimate gives $\lambda_j\geq c(j+1)^{2/n}-1$.

### Imaginary Airy operator

↑ **Parent:** [Compact resolvent](#compact-resolvent)

The imaginary Airy operator $-d^2/dx^2+ix$ on $L^2(\mathbb R)$ has compact resolvent but empty spectrum. Real translations shift it by a purely imaginary scalar, forcing vertical translation invariance of its spectrum.

## ↑ Ancestors (5)

1. [Functional analysis](functional-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (67)

- [Atkinson theorem](functional-analysis.md#atkinson-theorem)
- [Calkin algebra](banach-algebra.md#calkin-algebra)
- [Classification of separable self-adjoint operators modulo compacts](hilbert-space.md#classification-of-separable-self-adjoint-operators-modulo-compacts)
- [Compact averaging of a rank-one operator](#compact-averaging-of-a-rank-one-operator)
- [Compact perturbation invariance of Fredholm operators](functional-analysis.md#compact-perturbation-invariance-of-fredholm-operators)
- [Completely continuous operator](topological-vector-space.md#completely-continuous-operator)
- [Global variational form of the Michael criterion](astrophysical-fluid-dynamics.md#global-variational-form-of-the-michael-criterion)
- [Hilbert-Schmidt operator](#hilbert-schmidt-operator)
- [Left singular vector](linear-algebra.md#left-singular-vector)
- [Mixed-boundary singular system of the Volterra operator](functional-analysis.md#mixed-boundary-singular-system-of-the-volterra-operator)
- [Moore–Penrose inverse of an operator](inverse-problem.md#moore-penrose-inverse-of-an-operator)
- [Nondegenerate representations by compact operators](#nondegenerate-representations-by-compact-operators)
- [Norm-compact unit ball criterion](hilbert-space.md#norm-compact-unit-ball-criterion)
- [Odd topological K-theory](algebraic-topology.md#odd-topological-k-theory)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-42.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-6.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-10.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#22f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3.md#21g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#22h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#22h/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#22h/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#7/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#22h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1.md#22g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7.md#3/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-78.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-78.md#4/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-72.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-72.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#19g/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5.md#2/11/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#21f/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#21f/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-107.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#1/3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2.md#22f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105.md#3/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-106.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#21i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#22g/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-154.md#1/1/4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#23f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-225.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-106.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-358.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-358.md#1/a/solution)
- [Right singular vector](linear-algebra.md#right-singular-vector)
- [Spectral theorem for compact Hermitian operators](#spectral-theorem-for-compact-hermitian-operators)
- [Strong convergence of relaxed Landweber iteration](inverse-problem.md#strong-convergence-of-relaxed-landweber-iteration)
- [Weyl-von Neumann theorem](hilbert-space.md#weyl-von-neumann-theorem)
