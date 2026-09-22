# Numerical linear algebra

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Numerical_linear_algebra)

Numerical linear algebra develops stable finite algorithms for matrix computations.

**Table of contents**

- [Matrix preconditioning](#matrix-preconditioning)
  - [Matrix preconditioner](#matrix-preconditioner)
    - [Jacobi preconditioner](#jacobi-preconditioner)
  - [Left preconditioning](#left-preconditioning)
  - [Right preconditioning](#right-preconditioning)
  - [Symmetric positive-definite preconditioning](#symmetric-positive-definite-preconditioning)
    - [Symmetric preconditioning as energy geometry](#symmetric-preconditioning-as-energy-geometry)
  - [Diagonal scaling for a two-dimensional linear system](#diagonal-scaling-for-a-two-dimensional-linear-system)
  - [Preconditioned steepest descent](#preconditioned-steepest-descent)
    - [Condition-number bound for preconditioned steepest descent](#condition-number-bound-for-preconditioned-steepest-descent)
- [Power iteration](#power-iteration)
  - [Exact two-dimensional power iteration](#exact-two-dimensional-power-iteration)
  - [Power iteration convergence for a diagonalizable matrix](#power-iteration-convergence-for-a-diagonalizable-matrix)
    - [Power iteration direction error](#power-iteration-direction-error)
  - [Sign and phase in power iteration](#sign-and-phase-in-power-iteration)
  - [Power iteration eigenpair diagnostics](#power-iteration-eigenpair-diagnostics)
  - [Power iteration failure cases](#power-iteration-failure-cases)
- [Gaussian elimination](#gaussian-elimination)
  - [Bareiss algorithm](#bareiss-algorithm)
  - [Gaussian elimination with a row swap](#gaussian-elimination-with-a-row-swap)
  - [Pivot element](#pivot-element)
  - [Elimination multiplier](#elimination-multiplier)
  - [Sparse Gaussian elimination](#sparse-gaussian-elimination)
    - [Sparse elimination of a four-leaf star](#sparse-elimination-of-a-four-leaf-star)
    - [Leaf elimination of a tree-pattern positive-definite matrix](#leaf-elimination-of-a-tree-pattern-positive-definite-matrix)
    - [Symbolic factorization](#symbolic-factorization)
    - [Elimination tree](#elimination-tree)
    - [Nested dissection](#nested-dissection)
    - [Minimum degree algorithm](#minimum-degree-algorithm)
    - [Fill-in](#fill-in)
    - [Matrix graph](#matrix-graph)
      - [Elimination graph](#elimination-graph)
        - [Fill-path criterion for symmetric elimination](#fill-path-criterion-for-symmetric-elimination)
  - [Columnwise partial pivoting](#columnwise-partial-pivoting)
    - [Tiny-pivot roundoff in Gaussian elimination](#tiny-pivot-roundoff-in-gaussian-elimination)
  - [Row echelon form](#row-echelon-form)
    - [Row-equivalent matrices](#row-equivalent-matrices)
    - [Row reduction with a parameterized right-hand side](#row-reduction-with-a-parameterized-right-hand-side)
    - [Reduced row echelon form](#reduced-row-echelon-form)
      - [Reading solutions from reduced row echelon form](#reading-solutions-from-reduced-row-echelon-form)
      - [Uniqueness of reduced row echelon form](#uniqueness-of-reduced-row-echelon-form)
  - [Elementary row operation](#elementary-row-operation)
    - [Elementary matrix](#elementary-matrix)
- [LU decomposition](#lu-decomposition)
  - [Computed three-by-three LU decomposition](#computed-three-by-three-lu-decomposition)
  - [Unit triangular matrix](#unit-triangular-matrix)
  - [Triangular solves for LU decomposition](#triangular-solves-for-lu-decomposition)
    - [Forward substitution](#forward-substitution)
  - [Pivoted LU decomposition](#pivoted-lu-decomposition)
  - [Reusing LU factors for multiple right-hand sides](#reusing-lu-factors-for-multiple-right-hand-sides)
  - [LU factorization and solve costs](#lu-factorization-and-solve-costs)
- [LDL decomposition](#ldl-decomposition)
- [Eigenpair residual](#eigenpair-residual)
  - [Backward error of an approximate eigenpair](#backward-error-of-an-approximate-eigenpair)
- [Householder QR decomposition](#householder-qr-decomposition)
  - [Householder reduction of an overdetermined consistent system](#householder-reduction-of-an-overdetermined-consistent-system)
- [Householder tridiagonalization](#householder-tridiagonalization)
  - [Skew-symmetric Householder tridiagonalization](#skew-symmetric-householder-tridiagonalization)
- [Unshifted QR algorithm](#unshifted-qr-algorithm)
  - [Accumulated QR factorization identity](#accumulated-qr-factorization-identity)
  - [Symmetric bandwidth preservation under QR iteration](#symmetric-bandwidth-preservation-under-qr-iteration)
  - [Simultaneous iteration interpretation of the QR algorithm](#simultaneous-iteration-interpretation-of-the-qr-algorithm)
    - [Two-column dominant-subspace condition](#two-column-dominant-subspace-condition)
  - [Block deflation in the QR algorithm](#block-deflation-in-the-qr-algorithm)
- [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)
  - [Semiconvergence of cyclic Poisson iterations](#semiconvergence-of-cyclic-poisson-iterations)
  - [Richardson iteration](#richardson-iteration)
  - [Gauss-Seidel method](#gauss-seidel-method)
    - [Gauss-Seidel iteration for a two-variable positive-definite system](#gauss-seidel-iteration-for-a-two-variable-positive-definite-system)
      - [Exact error contraction of a two-variable Gauss-Seidel iteration](#exact-error-contraction-of-a-two-variable-gauss-seidel-iteration)
    - [Gauss-Seidel convergence from diagonal dominance and positive definiteness](#gauss-seidel-convergence-from-diagonal-dominance-and-positive-definiteness)
      - [Gauss-Seidel iteration can diverge for an invertible matrix](#gauss-seidel-iteration-can-diverge-for-an-invertible-matrix)
  - [Successive over-relaxation](#successive-over-relaxation)
  - [Iteration matrix](#iteration-matrix)
    - [Convergence criterion for a stationary iteration](#convergence-criterion-for-a-stationary-iteration)
    - [Residual and forward error in a stationary iteration](#residual-and-forward-error-in-a-stationary-iteration)
  - [Matrix splitting](#matrix-splitting)
    - [Householder-John theorem](#householder-john-theorem)
  - [Jacobi method](#jacobi-method)
    - [Jacobi iteration for a three-variable tridiagonal system](#jacobi-iteration-for-a-three-variable-tridiagonal-system)
      - [Error modes of a three-variable Jacobi iteration](#error-modes-of-a-three-variable-jacobi-iteration)
    - [Jacobi convergence from strict diagonal dominance](#jacobi-convergence-from-strict-diagonal-dominance)
    - [Skew-tridiagonal Jacobi and Gauss-Seidel iterations](#skew-tridiagonal-jacobi-and-gauss-seidel-iterations)
    - [Weighted Jacobi method](#weighted-jacobi-method)
      - [Weighted Jacobi eigenvalues for a square Dirichlet grid](#weighted-jacobi-eigenvalues-for-a-square-dirichlet-grid)
      - [Weighted Jacobi method for the one-dimensional Poisson equation](#weighted-jacobi-method-for-the-one-dimensional-poisson-equation)
        - [High-frequency smoothing factor of weighted Jacobi](#high-frequency-smoothing-factor-of-weighted-jacobi)
          - [Exact finite-grid high-frequency Jacobi smoothing optimum](#exact-finite-grid-high-frequency-jacobi-smoothing-optimum)
    - [Jacobi convergence for a three-by-three equicorrelation matrix](#jacobi-convergence-for-a-three-by-three-equicorrelation-matrix)
    - [Jacobi convergence for a symmetric positive-definite tridiagonal matrix](#jacobi-convergence-for-a-symmetric-positive-definite-tridiagonal-matrix)

## Matrix preconditioning

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra.md)

[Matrix preconditioning](#matrix-preconditioning) transforms a [linear system](linear-algebra.md#system-of-linear-equations) using an inexpensive auxiliary solve to improve its [eigenvalues](linear-operator-theory.md#eigenvalue). For [symmetric positive-definite matrices](linear-algebra.md#symmetric-positive-definite-matrix), a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) $M$ produces $M^{-1/2}AM^{-1/2}$, preserving the symmetric structure needed by the [Conjugate gradient method](gradient-descent.md#conjugate-gradient-method).

A useful [matrix preconditioner](#matrix-preconditioner) combines a cheap solve with favorable transformed [eigenvalues](linear-operator-theory.md#eigenvalue); neither property alone is enough.[Math 221, Matrix Computations, Fall 2023; Notes for Ma221 Lecture 15, Dec 1, 2023; PDF p. 1, opening transformation, goals (1) and (2), and example (1)](mathematics-bibliography.md#math-221-matrix-computations-fall-2023/notes-for-ma221-lecture-15-dec-1-2023)

The aim is to make each correction more effective without making it expensive. The example under [diagonal scaling for a two-dimensional linear system](#diagonal-scaling-for-a-two-dimensional-linear-system) turns thin [ellipses](euclidean-geometry.md#ellipse) into nearly circular ones and makes [preconditioned steepest descent](#preconditioned-steepest-descent) effective.

### Matrix preconditioner

↑ **Parent:** [Matrix preconditioning](#matrix-preconditioning)

A [matrix preconditioner](#matrix-preconditioner) is an auxiliary [invertible matrix](linear-algebra.md#invertible-matrix) whose [matrix inverse](matrix-inverse.md) is cheap to apply and whose use improves the [eigenvalues](linear-operator-theory.md#eigenvalue) of a [linear system](linear-algebra.md#system-of-linear-equations). In [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) problems, a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) $M$ preserves that structure under the symmetric transformation $M^{-1/2}AM^{-1/2}$.

Applying $M^{-1}$ means solving $Mz=r$ for a supplied [vector](vector-space.md#vector) $r$. This notation does not require forming a general [matrix inverse](matrix-inverse.md). A [diagonal matrix](linear-algebra.md#diagonal-matrix) gives componentwise divisions; a factored [matrix](vector-space.md#matrix) gives auxiliary solves such as [forward substitution](#forward-substitution) and [back substitution](linear-algebra.md#back-substitution).[Math 221, Matrix Computations, Fall 2009; Basic iterative methods, web lines 297–308, recurrence (\*) and cheap auxiliary-solve requirement](mathematics-bibliography.md#math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009)

Choosing $M=I$ makes the solve trivial but changes nothing; choosing $M=A$ gives the exact correction but asks us to solve the original [linear system](linear-algebra.md#system-of-linear-equations).[Math 221, Matrix Computations, Fall 2023; Notes for Ma221 Lecture 15, Dec 1, 2023; PDF p. 1, contrasting M = I and M = A; p. 2, example (3), two triangular solves](mathematics-bibliography.md#math-221-matrix-computations-fall-2023/notes-for-ma221-lecture-15-dec-1-2023)

#### Jacobi preconditioner

↑ **Parent:** [Matrix preconditioner](#matrix-preconditioner)

The [Jacobi preconditioner](#jacobi-preconditioner) keeps only the diagonal entries of the [matrix](vector-space.md#matrix) $A$. For a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix), these entries are positive, so its auxiliary solve is $z_i=r_i/a_{ii}$. It rescales coordinates with very different diagonal sizes, but cannot remove arbitrary off-diagonal coupling.[Math 221, Matrix Computations, Fall 2023; Notes for Ma221 Lecture 15, Dec 1, 2023; PDF p. 1, example (1), diagonal or Jacobi preconditioning](mathematics-bibliography.md#math-221-matrix-computations-fall-2023/notes-for-ma221-lecture-15-dec-1-2023)

This shares a [diagonal matrix](linear-algebra.md#diagonal-matrix) with the [Jacobi method](#jacobi-method), but the roles differ. The [Jacobi method](#jacobi-method) specifies a whole [stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system); a [Jacobi preconditioner](#jacobi-preconditioner) supplies an auxiliary solve to another [iterative method](numerical-analysis.md#iterative-method), including the [Preconditioned conjugate gradient method](gradient-descent.md#preconditioned-conjugate-gradient-method).

### Left preconditioning

↑ **Parent:** [Matrix preconditioning](#matrix-preconditioning)

[Left preconditioning](#left-preconditioning) multiplies both sides of the [linear system](linear-algebra.md#system-of-linear-equations) $Ax=b$ by the same [invertible matrix](linear-algebra.md#invertible-matrix) $M^{-1}$. It leaves the unknown [vector](vector-space.md#vector) $x$ unchanged. The original [linear-system residual](gradient-descent.md#linear-system-residual) is $r=b-Ax$; the transformed [linear-system residual](gradient-descent.md#linear-system-residual) is $M^{-1}r$. Applying the transformed [linear map](vector-space.md#linear-map) to $v$ first computes $Av$, then solves $Mz=Av$.

For [symmetric positive-definite matrices](linear-algebra.md#symmetric-positive-definite-matrix) $A$ and $M$, $M^{-1}A$ is generally not a [symmetric matrix](linear-algebra.md#symmetric-matrix) in the [Euclidean inner product](inner-product.md#dot-product). Its positive [eigenvalues](linear-operator-theory.md#eigenvalue) alone do not justify ordinary Euclidean [Conjugate gradient method](gradient-descent.md#conjugate-gradient-method) recurrences. The remedy is [symmetric positive-definite preconditioning](#symmetric-positive-definite-preconditioning), implemented through the [Preconditioned conjugate gradient method](gradient-descent.md#preconditioned-conjugate-gradient-method).

### Right preconditioning

↑ **Parent:** [Matrix preconditioning](#matrix-preconditioning)

[Right preconditioning](#right-preconditioning) substitutes $x=M^{-1}u$ into the [linear system](linear-algebra.md#system-of-linear-equations) $Ax=b$. Applying its transformed [linear map](vector-space.md#linear-map) first solves $Mz=v$, then computes $Az$. Recover the solution by solving $Mx=u$. Its [linear-system residual](gradient-descent.md#linear-system-residual) $b-AM^{-1}u$ is exactly the original [linear-system residual](gradient-descent.md#linear-system-residual) $b-Ax$, which is useful when monitoring the imbalance in the original equations.

The [left preconditioning](#left-preconditioning) and [right preconditioning](#right-preconditioning) transformed [matrices](vector-space.md#matrix) are [similar matrices](linear-algebra.md#matrix-similarity):

$$
AM^{-1}=M(M^{-1}A)M^{-1}.
$$

They therefore have the same [eigenvalues](linear-operator-theory.md#eigenvalue), although their [Euclidean norm](normed-vector-space.md#euclidean-norm) [condition numbers](quadratic-form.md#condition-number) and residual histories need not agree. A [similarity transformation](linear-algebra.md#similarity-transformation) preserves [eigenvalues](linear-operator-theory.md#eigenvalue); a nonorthogonal change of coordinates need not preserve lengths.

### Symmetric positive-definite preconditioning

↑ **Parent:** [Matrix preconditioning](#matrix-preconditioning)

Let $A$ and $M$ be real [symmetric positive-definite matrices](linear-algebra.md#symmetric-positive-definite-matrix). The [principal square root of a positive semidefinite matrix](quadratic-form.md#principal-square-root-of-a-positive-semidefinite-matrix) construction gives an [invertible matrix](linear-algebra.md#invertible-matrix) for each. Set

$$
S=M^{1/2},\qquad B=S^{-1}AS^{-1},\qquad y=Sx,\qquad c=S^{-1}b.
$$

Then $Ax=b$ is equivalent to $By=c$. This is a [matrix congruence](quadratic-form.md#matrix-congruence), and $B$ is a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix): $B^T=B$, and for every nonzero [vector](vector-space.md#vector) $v$,

$$
v^TBv=(S^{-1}v)^TA(S^{-1}v)>0,
$$

since $S^{-1}v\ne0$. This short proof establishes both requirements for applying the [Conjugate gradient method](gradient-descent.md#conjugate-gradient-method) to the transformed [linear system](linear-algebra.md#system-of-linear-equations).

The left transformed [matrix](vector-space.md#matrix) has the same [eigenvalues](linear-operator-theory.md#eigenvalue) because

$$
M^{-1}A=S^{-1}BS.
$$

Its correct geometry uses the [weighted inner product](inner-product.md#weighted-inner-product) $\langle u,v\rangle_M=u^TMv$: $\langle u,M^{-1}Av\rangle_M=u^TAv=\langle M^{-1}Au,v\rangle_M$. Thus it is symmetric in this [inner product](inner-product.md), even when it is not a [symmetric matrix](linear-algebra.md#symmetric-matrix) in ordinary coordinates. The spectral [condition number](quadratic-form.md#condition-number) governing the transformed symmetric problem is $\kappa_2(B)$, not generally $\kappa_2(M^{-1}A)$.

The [Preconditioned conjugate gradient method](gradient-descent.md#preconditioned-conjugate-gradient-method) realizes this transformation using auxiliary solves $Mz_k=r_k$, without constructing $S$ or its [matrix inverse](matrix-inverse.md). With fixed $M$, initialize $r_0=b-Ax_0$ and $p_0=z_0$; while $r_k\ne0$, use

$$
\alpha_k=\frac{r_k^Tz_k}{p_k^TAp_k},\quad x_{k+1}=x_k+\alpha_kp_k,\quad r_{k+1}=r_k-\alpha_kAp_k,
$$

then solve $Mz_{k+1}=r_{k+1}$ and set

$$
\beta_k=\frac{r_{k+1}^Tz_{k+1}}{r_k^Tz_k},\qquad p_{k+1}=z_{k+1}+\beta_kp_k.
$$

Stop at a zero [linear-system residual](gradient-descent.md#linear-system-residual) before forming another ratio. Positive definiteness makes the denominators positive before termination.[Math 221, Matrix Computations, Fall 2023; Notes for Ma221 Lecture 15, Dec 1, 2023; PDF p. 1, equivalent symmetric system and Preconditioned CG algorithm](mathematics-bibliography.md#math-221-matrix-computations-fall-2023/notes-for-ma221-lecture-15-dec-1-2023)

An [invertible matrix](linear-algebra.md#invertible-matrix) alone is insufficient: with $A=I$ and $M=\operatorname{diag}(-1,1)$, the left transformed [matrix](vector-space.md#matrix) has [eigenvalues](linear-operator-theory.md#eigenvalue) $-1,1$, and $M$ has no real [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) square root. Even a valid [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) can worsen conditioning if its scaling is unsuitable, as the next worked example shows.

#### Symmetric preconditioning as energy geometry

↑ **Parent:** [Symmetric positive-definite preconditioning](#symmetric-positive-definite-preconditioning)

For a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) $A$, solving $Ax_*=b$ is equivalent to minimizing the [quadratic form](quadratic-form.md) with linear term

$$
F(x)=\frac12x^TAx-b^Tx.
$$

Writing the error [vector](vector-space.md#vector) $e=x-x_*$ and expanding gives the exact [energy norm](finite-element-method.md#energy-norm) identity

$$
F(x)-F(x_*)=\frac12e^TAe=\frac12\|e\|_A^2.
$$

The cross term vanishes because $Ax_*=b$. With $\eta=Se$ and $B=S^{-1}AS^{-1}$, the same quantity is $\eta^TB\eta/2$. [Symmetric positive-definite preconditioning](#symmetric-positive-definite-preconditioning) changes coordinates without changing the energy assigned to a corresponding error [vector](vector-space.md#vector).

In an [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) of $A$, the [level set](topology.md#level-set) $e^TAe=t>0$ has semiaxis lengths $\sqrt{t/\lambda_i}$. Its longest-to-shortest axis ratio is $\sqrt{\kappa_2(A)}$. A large [spectral condition number of a positive-definite matrix](quadratic-form.md#spectral-condition-number-of-a-positive-definite-matrix) therefore appears geometrically as a thin [ellipsoid](euclidean-geometry.md#ellipsoid). Good scaling makes the transformed [ellipsoid](euclidean-geometry.md#ellipsoid) rounder, allowing a simple search direction to improve all coordinates together.

The negative [gradient](multivariable-calculus.md#gradient) of $F$ is the [linear-system residual](gradient-descent.md#linear-system-residual) $r$. Relative to the [norm](normed-vector-space.md#norm) $\|v\|_M=\sqrt{v^TMv}$, a steepest direction is $z=M^{-1}r$: the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) applied to $r^Tv=(S^{-1}r)^T(Sv)$ shows that the greatest decrease per unit $M$-length occurs along this direction. Equivalently, ordinary [gradient descent](gradient-descent.md) in $y=Sx$ becomes [preconditioned steepest descent](#preconditioned-steepest-descent) in $x$.[§9.4.1, printed pp. 476–477, equation (9.25), quadratic-norm steepest direction and change of coordinates](mathematics-bibliography.md#convex-optimization-by-stephen-boyd-and-lieven-vandenberghe)

### Diagonal scaling for a two-dimensional linear system

↑ **Parent:** [Matrix preconditioning](#matrix-preconditioning)

Consider the original [linear system](linear-algebra.md#system-of-linear-equations)

$$
A=\begin{pmatrix}1&1/5\\1/5&100\end{pmatrix},\qquad b=\begin{pmatrix}1\\1\end{pmatrix},\qquad M=\begin{pmatrix}1&0\\0&100\end{pmatrix}.
$$

Completing the square proves that $A$ is a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix):

$$
e^TAe=(e_1+e_2/5)^2+\frac{2499}{25}e_2^2>0\qquad(e\ne0).
$$

The [Jacobi preconditioner](#jacobi-preconditioner) $M$ has $S=\operatorname{diag}(1,10)$. [Symmetric positive-definite preconditioning](#symmetric-positive-definite-preconditioning) gives

$$
B=\begin{pmatrix}1&1/50\\1/50&1\end{pmatrix},\qquad c=\begin{pmatrix}1\\1/10\end{pmatrix}.
$$

Its [eigenvectors](linear-operator-theory.md#eigenvector) $(1,1)^T$ and $(1,-1)^T$ have [eigenvalues](linear-operator-theory.md#eigenvalue) $51/50$ and $49/50$. Hence

$$
\kappa_2(B)=\frac{51}{49}\approx1.040816.
$$

The [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) of $A$ is $\lambda^2-101\lambda+2499/25$. Its [eigenvalues](linear-operator-theory.md#eigenvalue) and [spectral condition number of a positive-definite matrix](quadratic-form.md#spectral-condition-number-of-a-positive-definite-matrix) are

$$
\lambda_\pm=\frac{505\pm\sqrt{245029}}{10},\qquad \kappa_2(A)=\frac{\lambda_+}{\lambda_-}\approx100.040824.
$$

The [ellipse](euclidean-geometry.md#ellipse) axis ratio drops from about $10.0020$ to $1.0202$. The transformation multiplies the second coordinate by ten, bringing the two energy scales together.

<a id="image-diagonal-scaling-changes-thin-energy-ellipses-into-nearly-circular-energy-ellipses"></a>
![](matrix-preconditioning-energy-ellipses.png)

**[Figure 1](#image-diagonal-scaling-changes-thin-energy-ellipses-into-nearly-circular-energy-ellipses). Diagonal scaling changes thin energy ellipses into nearly circular energy ellipses**.

Both panels show the same energy [level sets](topology.md#level-set), expressed in error coordinates $e=x-x_*$ and $\eta=M^{1/2}e$. Their coordinate axes have equal scales. The marked displacement $(1,0.1)^T$ becomes $(1,1)^T$; its energy remains $e^TAe/2=1.02$. These are exact contours of the specified [quadratic form](quadratic-form.md).

Solving the original equations gives

$$
x_*=\frac1{2499}\begin{pmatrix}2495\\20\end{pmatrix},\qquad y_*=\frac1{2499}\begin{pmatrix}2495\\200\end{pmatrix}.
$$

Direct [matrix multiplication](vector-space.md#matrix-multiplication) checks both [linear-system residuals](gradient-descent.md#linear-system-residual):

$$
Ax_* = \frac1{2499}\begin{pmatrix}2495+4\\499+2000\end{pmatrix}=b,\qquad By_* = \frac1{2499}\begin{pmatrix}2495+4\\499/10+200\end{pmatrix}=c.
$$

By contrast, [left preconditioning](#left-preconditioning) gives $M^{-1}A=\begin{pmatrix}1&1/5\\1/500&1\end{pmatrix}$, which is visibly not a [symmetric matrix](linear-algebra.md#symmetric-matrix), despite having the same positive [eigenvalues](linear-operator-theory.md#eigenvalue) as $B$.

A bad scaling can reverse the benefit: the still valid [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) $M_{\rm bad}=\operatorname{diag}(100,1)$ gives $B_{\rm bad}=\begin{pmatrix}1/100&1/50\\1/50&100\end{pmatrix}$. Its [Rayleigh quotients](linear-operator-theory.md#rayleigh-quotient) on the coordinate [unit vectors](vector-space.md#unit-vector) are $0.01$ and $100$, so $\kappa_2(B_{\rm bad})\ge10000$. Cheapness and positive definiteness do not guarantee improved conditioning.

### Preconditioned steepest descent

↑ **Parent:** [Matrix preconditioning](#matrix-preconditioning)

For fixed [symmetric positive-definite matrices](linear-algebra.md#symmetric-positive-definite-matrix) $A$ and $M$, [preconditioned steepest descent](#preconditioned-steepest-descent) minimizes $F(x)=x^TAx/2-b^Tx$ along the direction supplied by the auxiliary solve. Given $x_k$, form the [linear-system residual](gradient-descent.md#linear-system-residual) $r_k=b-Ax_k$. If $r_k=0$, stop: $x_k=x_*$. Otherwise solve $Mz_k=r_k$ and use

$$
\alpha_k=\frac{r_k^Tz_k}{z_k^TAz_k},\qquad x_{k+1}=x_k+\alpha_kz_k,\qquad r_{k+1}=r_k-\alpha_kAz_k.
$$

This is [exact line search for a positive-definite quadratic](gradient-descent.md#exact-line-search-for-a-positive-definite-quadratic) along $z_k$. Indeed,

$$
F(x_k+\alpha z_k)=F(x_k)-\alpha r_k^Tz_k+\frac12\alpha^2z_k^TAz_k,
$$

whose [derivative](calculus.md#derivative) vanishes at the displayed positive [step size](convex-optimization.md#step-size). Unlike the [Preconditioned conjugate gradient method](gradient-descent.md#preconditioned-conjugate-gradient-method), it uses the fresh $z_k$ directly rather than combining it with a previous conjugate direction.

For [diagonal scaling for a two-dimensional linear system](#diagonal-scaling-for-a-two-dimensional-linear-system), start at $x_0=0$. Without [matrix preconditioning](#matrix-preconditioning), take $M=I$: $z_0=(1,1)^T$, $\alpha_0=10/507$, and

$$
x_1=\frac1{507}\begin{pmatrix}10\\10\end{pmatrix},\qquad r_1=\frac{165}{169}\begin{pmatrix}1\\-1\end{pmatrix}.
$$

With the [Jacobi preconditioner](#jacobi-preconditioner) $M=\operatorname{diag}(1,100)$, $z_0=(1,1/100)^T$, $\alpha_0=505/507$, and

$$
x_1=\begin{pmatrix}505/507\\101/10140\end{pmatrix},\qquad r_1=\begin{pmatrix}33/16900\\-33/169\end{pmatrix}.
$$

The original [linear-system residual](gradient-descent.md#linear-system-residual) becomes much smaller after this correction. Quantify progress in the same [energy norm](finite-element-method.md#energy-norm) in both cases: $E_k=F(x_k)-F(x_*)$ and $E_0=2515/4998$. Exact substitution gives

$$
\frac{E_1}{E_0}=q_I=\frac{81675}{85007}\approx0.960803228,\qquad \frac{E_1^{(M)}}{E_0}=q_M=\frac{3267}{8500700}\approx0.000384321291.
$$

In this particular example the entire histories are $E_k/E_0=q_I^k$ and $E_k^{(M)}/E_0=q_M^k$. To check that this is exact, the next [step sizes](convex-optimization.md#step-size) are $10/503$ and $505/503$, respectively, and their residual updates give $r_2=q_Ir_0$ and $r_2^{(M)}=q_Mr_0$. Multiplying a [linear-system residual](gradient-descent.md#linear-system-residual) by a nonzero [scalar](vector-space.md#scalar) leaves the next [step size](convex-optimization.md#step-size) unchanged; every pair of steps repeats the same directions at a smaller scale. The two first-step energy ratios then establish these formulas for all $k$.

<a id="image-computed-steepest-descent-method-energy-errors-before-and-after-jacobi-preconditioning"></a>
![](matrix-preconditioning-steepest-descent-energy-errors.png)

**[Figure 2](#image-computed-steepest-descent-method-energy-errors-before-and-after-jacobi-preconditioning). Computed steepest descent method energy errors before and after Jacobi preconditioning**.

The curves come from exact rational updates of the specified [linear system](linear-algebra.md#system-of-linear-equations), converted to decimal values for plotting. The left panel counts iterations. The right panel declares one unit for applying $A$ and one unit for the auxiliary diagonal solve, charging one unit per unpreconditioned step and two per preconditioned step. It excludes setup and [vector](vector-space.md#vector) operations, so it compares a declared cost model rather than measured runtime. Scaling is advantageous even with that extra charge.

These curves compare [steepest descent method](gradient-descent.md) iterations. On this two-dimensional [linear system](linear-algebra.md#system-of-linear-equations), both the [Conjugate gradient method](gradient-descent.md#conjugate-gradient-method) and the [Preconditioned conjugate gradient method](gradient-descent.md#preconditioned-conjugate-gradient-method) terminate within two steps in exact arithmetic. The plot therefore establishes no CG iteration-count advantage for this example; the benefit of scaling for larger problems depends on their [eigenvalues](linear-operator-theory.md#eigenvalue) and auxiliary-solve costs.

#### Condition-number bound for preconditioned steepest descent

↑ **Parent:** [Preconditioned steepest descent](#preconditioned-steepest-descent)

Let $m=\lambda_{\min}(B)>0$, $L=\lambda_{\max}(B)$ and $\kappa=L/m=\kappa_2(B)$ for the transformed [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix). Then [preconditioned steepest descent](#preconditioned-steepest-descent) satisfies

$$
E_{k+1}\le\left(\frac{\kappa-1}{\kappa+1}\right)^2E_k.
$$

This is a worst-case bound, not necessarily the actual rate. For our scaled example the bound is $(1/50)^2=0.0004$, slightly above its computed factor $q_M\approx0.000384321291$. If the initial transformed error is an [eigenvector](linear-operator-theory.md#eigenvector), [exact line search for a positive-definite quadratic](gradient-descent.md#exact-line-search-for-a-positive-definite-quadratic) removes it in one step, regardless of the full [condition number](quadratic-form.md#condition-number).

A short proof compares [exact line search for a positive-definite quadratic](gradient-descent.md#exact-line-search-for-a-positive-definite-quadratic) with the trial [step size](convex-optimization.md#step-size) $\alpha=2/(m+L)$ in the transformed coordinates. In an [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) of $B$, each error coefficient is multiplied by $1-\alpha\lambda_i$, whose [absolute value](real-analysis.md#absolute-value) is at most $(L-m)/(L+m)$. Summing $\lambda_i$ times the squared coefficients bounds the trial energy by the square of this factor. The exact minimizing [step size](convex-optimization.md#step-size) does at least as well. This also explains the terminating case $m=L$: the trial step removes the entire error in one iteration.

## Power iteration

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Power_iteration)

[Power iteration](#power-iteration) finds a [dominant eigenvalue](linear-operator-theory.md#dominant-eigenvalue) and its [eigenvector](linear-operator-theory.md#eigenvector) by repeatedly applying a [matrix](vector-space.md#matrix) and rescaling the resulting [vector](vector-space.md#vector). The essential idea is selective amplification: components along different [eigenvectors](linear-operator-theory.md#eigenvector) grow at different rates, so one direction can eventually dominate. It is the computational form of the [power method](linear-operator-theory.md#power-method) and is useful when applying a large [sparse matrix](vector-space.md#sparse-matrix) to a [vector](vector-space.md#vector) is cheap but computing its whole [spectral decomposition](linear-operator-theory.md#spectral-decomposition) is expensive.

For a square [matrix](vector-space.md#matrix) over the [real numbers](arithmetic.md#real-number) or [complex numbers](complex-analysis.md#complex-number) $A$, choose a [unit vector](vector-space.md#unit-vector) $x_0$ and repeat

$$
y_{k+1}=Ax_k,\qquad x_{k+1}=\frac{y_{k+1}}{\|y_{k+1}\|_2}.
$$

Here $\|\cdot\|_2$ is the [Euclidean norm](normed-vector-space.md#euclidean-norm). If $y_{k+1}=0$, stop before division: the current [vector](vector-space.md#vector) is an [eigenvector](linear-operator-theory.md#eigenvector) for the [zero eigenvalue](linear-operator-theory.md#zero-eigenvalue), and this iteration cannot continue. Otherwise, in exact arithmetic,

$$
x_k=\frac{A^kx_0}{\|A^kx_0\|_2}.
$$

Repeated normalization keeps the stored [vectors](vector-space.md#vector) at manageable size without changing their directions; it does not guarantee that an individual multiplication cannot exceed the range of [floating-point arithmetic](floating-point-arithmetic.md). The [dominant eigenvalue](linear-operator-theory.md#dominant-eigenvalue) means largest [modulus](complex-analysis.md#modulus), which need not mean largest signed real value.[Power Method](mathematics-bibliography.md#templates-for-the-solution-of-algebraic-eigenvalue-problems-a-practical-guide/power-method)

### Exact two-dimensional power iteration

↑ **Parent:** [Power iteration](#power-iteration)

Consider the [symmetric matrix](linear-algebra.md#symmetric-matrix) and initial [unit vector](vector-space.md#unit-vector)

$$
A=\begin{pmatrix}2&1\\1&2\end{pmatrix},\qquad x_0=\begin{pmatrix}1\\0\end{pmatrix}.
$$

Its [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) consists of $u_1=(1,1)^T/\sqrt2$ and $u_2=(1,-1)^T/\sqrt2$, with [eigenvalues](linear-operator-theory.md#eigenvalue) $3$ and $1$. Since $x_0=(u_1+u_2)/\sqrt2$, direct multiplication gives

$$
A^kx_0=\frac12\begin{pmatrix}3^k+1\\3^k-1\end{pmatrix},\qquad x_k=\frac{u_1+3^{-k}u_2}{\sqrt{1+3^{-2k}}}.
$$

The first unnormalized [vectors](vector-space.md#vector) are $(1,0)^T$, $(2,1)^T$, $(5,4)^T$, and $(14,13)^T$. If $\theta_k$ is the acute [angle](geometry-and-topology.md#angle) from the line spanned by the dominant [eigenvector](linear-operator-theory.md#eigenvector), then $\tan\theta_k=3^{-k}$. Every application divides the unwanted-to-wanted component ratio by three: normalization changes lengths, while the [spectral gap](linear-operator-theory.md#spectral-gap) selects the direction.

<a id="image-exact-power-iteration-directions-and-errors-for-a-symmetric-matrix-with-eigenvalues-3-and-1"></a>
![](power-iteration-symmetric-direction-error.png)

**[Figure 3](#image-exact-power-iteration-directions-and-errors-for-a-symmetric-matrix-with-eigenvalues-3-and-1). Exact power iteration directions and errors for a symmetric matrix with eigenvalues 3 and 1**.

The right panel compares the [power iteration direction error](#power-iteration-direction-error), [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) error, and [eigenpair residual](#eigenpair-residual). With $t_k=3^{-k}$, their exact values are

$$
\varepsilon_k=\frac{t_k}{\sqrt{1+t_k^2}},\qquad 3-\rho_k=\frac{2t_k^2}{1+t_k^2},\qquad \|r_k\|_2=\frac{2t_k}{1+t_k^2}.
$$

Thus a very accurate [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) can appear well before the [eigenvector](linear-operator-theory.md#eigenvector) is comparably accurate. This is an example of [quadratic Rayleigh-quotient improvement for the power method](linear-operator-theory.md#quadratic-rayleigh-quotient-improvement-for-the-power-method).

### Power iteration convergence for a diagonalizable matrix

↑ **Parent:** [Power iteration](#power-iteration)

Suppose $A\in\mathbb C^{n\times n}$ is a [diagonalizable matrix](linear-operator-theory.md#diagonalizable-matrix), $n\ge2$, with an [eigenbasis](linear-operator-theory.md#eigenbasis) $v_1,\ldots,v_n$ and [spectral decomposition](linear-operator-theory.md#spectral-decomposition)

$$
A=V\Lambda V^{-1},\qquad V=(v_1\ \cdots\ v_n),\qquad \Lambda=\operatorname{diag}(\lambda_1,\ldots,\lambda_n).
$$

Assume the [dominant eigenvalue](linear-operator-theory.md#dominant-eigenvalue) $\lambda_1$ is a [simple eigenvalue](linear-operator-theory.md#simple-eigenvalue) and

$$
|\lambda_1|>|\lambda_2|\ge\cdots\ge|\lambda_n|,\qquad x_0=\sum_{j=1}^n c_jv_j,\qquad c_1\ne0.
$$

Then the normalized [power iteration](#power-iteration) approaches the one-dimensional [eigenspace](linear-operator-theory.md#eigenspace) of $\lambda_1$. Its asymptotic direction-error bound has factor $\gamma=|\lambda_2/\lambda_1|<1$. This [spectral gap](linear-operator-theory.md#spectral-gap) is a gap in [modulus](complex-analysis.md#modulus): if $g=|\lambda_1|-|\lambda_2|$, then $\gamma=1-g/|\lambda_1|$. A small relative gap gives slow convergence.[Power Method](mathematics-bibliography.md#templates-for-the-solution-of-algebraic-eigenvalue-problems-a-practical-guide/power-method)

The short proof is the exact [eigenbasis](linear-operator-theory.md#eigenbasis) identity

$$
\frac{A^kx_0}{c_1\lambda_1^k}=v_1+\sum_{j=2}^n\frac{c_j}{c_1}\left(\frac{\lambda_j}{\lambda_1}\right)^kv_j.
$$

The remaining sum has [norm](normed-vector-space.md#norm) bounded by a constant times $\gamma^k$. This proves convergence of direction, allowing a changing sign or complex factor. A tiny $c_1$ or a poorly conditioned, [nonorthogonal](inner-product.md#nonorthogonal-vectors) [eigenbasis](linear-operator-theory.md#eigenbasis) can delay visible convergence: the [condition number](quadratic-form.md#condition-number) of $V$ affects constants, while $\gamma$ controls the eventual rate. The bound need not be an equality; if the initial coefficient of the second-largest [eigenvalue](linear-operator-theory.md#eigenvalue) vanishes, the [active spectrum of the power method](linear-operator-theory.md#active-spectrum-of-the-power-method) gives a faster rate. When $\gamma=0$, all unwanted components disappear after one multiplication.[§1, PDF pp. 1–2: diagonalizable expansion and nonzero first coordinate of the starting vector](mathematics-bibliography.md#numerical-analysis-spring-2022/power-iteration-2022-03-07-lecture-notes)

The hypothesis is $c_1=(V^{-1}x_0)_1\ne0$, not an ordinary nonzero [inner product](inner-product.md) with the right [eigenvector](linear-operator-theory.md#eigenvector). Let $w_1^*$ be the first row of $V^{-1}$, a [left eigenvector](linear-operator-theory.md#left-eigenvector) normalized so $w_1^*v_j$ is $1$ for $j=1$ and $0$ otherwise; $*$ denotes [conjugate transpose](linear-operator-theory.md#conjugate-transpose). Then $c_1=w_1^*x_0$. For a [Hermitian matrix](hilbert-space.md#hermitian-operator), choose an [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) and the criterion becomes $v_1^*x_0\ne0$: the starting [vector](vector-space.md#vector) must be [nonorthogonal](inner-product.md#nonorthogonal-vectors) to the dominant [eigenvector](linear-operator-theory.md#eigenvector). For a general [diagonalizable matrix](linear-operator-theory.md#diagonalizable-matrix), the [nonorthogonal](inner-product.md#nonorthogonal-vectors) [eigenbasis](linear-operator-theory.md#eigenbasis) makes these two tests different, as illustrated under [power iteration failure cases](#power-iteration-failure-cases).

#### Power iteration direction error

↑ **Parent:** [Power iteration convergence for a diagonalizable matrix](#power-iteration-convergence-for-a-diagonalizable-matrix)

For a [unit vector](vector-space.md#unit-vector) $u$ spanning the target [eigenspace](linear-operator-theory.md#eigenspace) and a normalized iterate $x_k$, define

$$
\varepsilon_k=\|(I-uu^*)x_k\|_2=\sqrt{1-|u^*x_k|^2}.
$$

This is the [norm](normed-vector-space.md#norm) of the component in the [orthogonal complement](hilbert-space.md#orthogonal-complement) of $u$, equivalently the sine of the acute [angle](geometry-and-topology.md#angle) to its line. It ignores the arbitrary sign or complex unit factor of an [eigenvector](linear-operator-theory.md#eigenvector). Under [power iteration convergence for a diagonalizable matrix](#power-iteration-convergence-for-a-diagonalizable-matrix), $\varepsilon_k=O(\gamma^k)$ in [Big O notation](real-analysis.md#big-o-notation). The [orthogonal projection](hilbert-space.md#orthogonal-projection) defines how we measure direction; it does not assume that the [eigenbasis](linear-operator-theory.md#eigenbasis) of $A$ is [orthogonal](inner-product.md#orthogonal-vectors). In computation, the projection form avoids subtracting nearly equal numbers inside the square root.

### Sign and phase in power iteration

↑ **Parent:** [Power iteration](#power-iteration)

Under [power iteration convergence for a diagonalizable matrix](#power-iteration-convergence-for-a-diagonalizable-matrix), take $v_1=u_1$ to be a [unit vector](vector-space.md#unit-vector). The displayed formula describes both the dominant [eigenvector](linear-operator-theory.md#eigenvector) direction and its rotating complex unit factor. With real data and a positive [dominant eigenvalue](linear-operator-theory.md#dominant-eigenvalue), $x_k$ converges to $u_1$ or $-u_1$ according to the sign of $c_1$. With a negative [dominant eigenvalue](linear-operator-theory.md#dominant-eigenvalue), consecutive [vectors](vector-space.md#vector) approach opposite signs even though their [power iteration direction error](#power-iteration-direction-error) tends to zero.

For complex data write $\lambda_1=|\lambda_1|e^{i\phi}$, where $\phi$ is its [complex argument](complex-analysis.md#argument-complex-analysis). The leading factor turns by $e^{i\phi}$ per step, so the [vectors](vector-space.md#vector) generally do not converge. For example, $A=\operatorname{diag}(2i,1)$ and $x_0=(1,1)^T/\sqrt2$ give $A^kx_0=((2i)^k,1)^T/\sqrt2$: the first component cycles through four phases while the ratio of component [moduli](complex-analysis.md#modulus) tends to zero. Its [power iteration direction error](#power-iteration-direction-error) is $2^{-k}/\sqrt{1+2^{-2k}}$. Multiplying $x_k$ by $e^{-i(\arg c_1+k\phi)}$ gives a sequence converging to $u_1$.

A stopping rule based only on $\|x_{k+1}-x_k\|_2$ therefore rejects successful sign-alternating iterations. A comparison invariant under complex unit factors is

$$
\min_{|\omega|=1}\|x_{k+1}-\omega x_k\|_2=\sqrt{2-2|x_k^*x_{k+1}|}.
$$

Even this comparison can be small for a slowly changing wrong mixture; the [eigenpair residual](#eigenpair-residual) supplies a separate diagnostic.

### Power iteration eigenpair diagnostics

↑ **Parent:** [Power iteration](#power-iteration)

For each [unit vector](vector-space.md#unit-vector) iterate compute the [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) $\rho_k=x_k^*Ax_k$ and the [eigenpair residual](#eigenpair-residual) $r_k=Ax_k-\rho_kx_k$. Use the same multiplication $Ax_k$ for both diagnostics and the next normalized iterate. For any complex [matrix](vector-space.md#matrix), this [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) minimizes $\|Ax_k-\mu x_k\|_2$ over complex [scalars](vector-space.md#scalar) $\mu$, because $x_k^*r_k=0$. Under [power iteration convergence for a diagonalizable matrix](#power-iteration-convergence-for-a-diagonalizable-matrix), $\rho_k\to\lambda_1$ and $\|r_k\|_2\to0$, even when the [vectors](vector-space.md#vector) alternate signs or phases.[§3, PDF p. 3: approximate eigenvector equation and Rayleigh quotient](mathematics-bibliography.md#numerical-analysis-spring-2022/power-iteration-2022-03-07-lecture-notes)

A dimensionless stopping quantity is

$$
\eta_k=\frac{\|r_k\|_2}{\|A\|_2+|\rho_k|},
$$

when the denominator is positive; $\|A\|_2$ is the [operator norm](continuous-dual-space.md#operator-norm), and a known upper bound may replace it if computing it is costly. A small [eigenpair residual](#eigenpair-residual) certifies a small [backward error of an approximate eigenpair](#backward-error-of-an-approximate-eigenpair), but does not establish that the [eigenvalue](linear-operator-theory.md#eigenvalue) found is dominant.

For a [Hermitian matrix](hilbert-space.md#hermitian-operator) with [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) $u_j$, write $x_k=\sum_j a_ju_j$. Then the independently useful identity

$$
\|r_k\|_2^2=\sum_j|a_j|^2|\lambda_j-\rho_k|^2
$$

shows that some [eigenvalue](linear-operator-theory.md#eigenvalue) lies within $\|r_k\|_2$ of $\rho_k$. If a specific target [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda_1$ is separated from all the others by $\delta_k=\min_{j>1}|\lambda_j-\rho_k|>0$, it also gives $\varepsilon_k\le\|r_k\|_2/\delta_k$. This separation is measured from the computed [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient); it differs from the dominant-[modulus](complex-analysis.md#modulus) [spectral gap](linear-operator-theory.md#spectral-gap). For a [nonnormal matrix](linear-operator-theory.md#non-normal-matrix), the same [orthogonal](inner-product.md#orthogonal-vectors) expansion is unavailable and a small [eigenpair residual](#eigenpair-residual) alone need not imply a comparably small distance to the [spectrum](linear-operator-theory.md#spectrum-functional-analysis).

### Power iteration failure cases

↑ **Parent:** [Power iteration](#power-iteration)

A tied largest [modulus](complex-analysis.md#modulus) can prevent even direction convergence. With $D=\operatorname{diag}(2,-2)$ and $x_0=(1,1)^T/\sqrt2$,

$$
x_k=\frac1{\sqrt2}\begin{pmatrix}1\\(-1)^k\end{pmatrix},\qquad \rho_k=0,\qquad \|r_k\|_2=2.
$$

The two directions form a cycle; neither is an [eigenvector](linear-operator-theory.md#eigenvector). There is no dominant-[modulus](complex-analysis.md#modulus) [spectral gap](linear-operator-theory.md#spectral-gap). A tied [modulus](complex-analysis.md#modulus) is not a universal failure: an initial [eigenvector](linear-operator-theory.md#eigenvector) remains on its line, and $A=2I$ preserves every direction. [Subspace iteration](linear-operator-theory.md#subspace-iteration) addresses a separated cluster by targeting a [dominant invariant subspace](linear-operator-theory.md#dominant-invariant-subspace) instead of one [eigenvector](linear-operator-theory.md#eigenvector).

An [orthogonal](inner-product.md#orthogonal-vectors) start can fail despite a strict [spectral gap](linear-operator-theory.md#spectral-gap). For $A=\begin{pmatrix}2&1\\1&2\end{pmatrix}$ and $x_0=(1,-1)^T/\sqrt2$, the dominant component is zero, so $Ax_0=x_0$ and every iterate equals $x_0$. The [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) is exactly $1$ and the [eigenpair residual](#eigenpair-residual) is zero, although the [dominant eigenvalue](linear-operator-theory.md#dominant-eigenvalue) is $3$. Exact arithmetic never creates a missing component.[Power Method](mathematics-bibliography.md#templates-for-the-solution-of-algebraic-eigenvalue-problems-a-practical-guide/power-method)

<a id="image-tied-eigenvalue-moduli-an-orthogonal-start-and-sign-alternation-in-power-iteration"></a>
![](power-iteration-tied-modulus-orthogonal-start.png)

**[Figure 4](#image-tied-eigenvalue-moduli-an-orthogonal-start-and-sign-alternation-in-power-iteration). Tied eigenvalue moduli, an orthogonal start, and sign alternation in power iteration**.

The third panel contrasts these failures with $N=\operatorname{diag}(-3,1)$, $x_0=(1,1)^T/\sqrt2$, for which

$$
x_k=\frac1{\sqrt{1+3^{-2k}}}\begin{pmatrix}(-1)^k\\3^{-k}\end{pmatrix}.
$$

Here the horizontal [eigenvector](linear-operator-theory.md#eigenvector) direction converges with a strict [spectral gap](linear-operator-theory.md#spectral-gap), while the normalized [vectors](vector-space.md#vector) alternate signs. This is the successful direction convergence described under [sign and phase in power iteration](#sign-and-phase-in-power-iteration).

For a [nonorthogonal](inner-product.md#nonorthogonal-vectors) [eigenbasis](linear-operator-theory.md#eigenbasis), even the word “orthogonal” must be used carefully. The [diagonalizable matrix](linear-operator-theory.md#diagonalizable-matrix) $C=\begin{pmatrix}3&2\\0&1\end{pmatrix}$ has right [eigenvectors](linear-operator-theory.md#eigenvector) $v_1=(1,0)^T$, $v_2=(-1,1)^T$, and dominant [left eigenvector](linear-operator-theory.md#left-eigenvector) $w_1=(1,1)^T$. For $x_0=(a,b)^T$, the dominant coefficient is $c_1=w_1^Tx_0=a+b$. The starting [vector](vector-space.md#vector) $v_2$ is [nonorthogonal](inner-product.md#nonorthogonal-vectors) to $v_1$ but stays at the smaller [eigenvalue](linear-operator-theory.md#eigenvalue) $1$; $(0,1)^T$ is [orthogonal](inner-product.md#orthogonal-vectors) to $v_1$ but has $c_1=1$ and converges to the dominant direction. The [left eigenvector](linear-operator-theory.md#left-eigenvector) test, not the right-[eigenvector](linear-operator-theory.md#eigenvector) [inner product](inner-product.md), controls the outcome.

A [random vector](random-variable.md#random-vector) drawn from a [continuous probability distribution](continuous-probability-distribution.md) with a [probability density function](continuous-probability-distribution.md#probability-density-function) on the full real or complex [vector space](vector-space.md) has $c_1\ne0$ with probability one. This avoids the exact missing-component [hyperplane](vector-space.md#hyperplane), but does not guarantee a large component or fast convergence. [Floating-point arithmetic](floating-point-arithmetic.md) may seed a missing component, yet a structurally preserved zero can remain zero, so accidental perturbations are not a convergence guarantee.

## Gaussian elimination

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_elimination)

Gaussian elimination applies elementary row operations to reduce a linear system to triangular form. Dense elimination uses $O(n^3)$ arithmetic operations.

[Gaussian elimination](#gaussian-elimination) solves a [linear system](linear-algebra.md#system-of-linear-equations) by removing one unknown from later equations at each step. Write the coefficients and right-hand side together as an [augmented matrix](linear-algebra.md#augmented-matrix) $[A\mid b]$. Apply the same [elementary row operations](#elementary-row-operation) to both parts until the coefficients form a [row echelon form](#row-echelon-form); for a square [invertible matrix](linear-algebra.md#invertible-matrix), this gives an [upper triangular matrix](linear-algebra.md#upper-triangular-matrix) system. Then [back substitution](linear-algebra.md#back-substitution) recovers the unknowns from the last equation upward. The useful simplification is that each successive equation involves fewer unknowns, while the set of solutions stays the same.

Why do [elementary row operations](#elementary-row-operation) preserve solutions? Interchanging equations changes only their order. Multiplying an equation by a nonzero [scalar](vector-space.md#scalar) can be undone by division. Replacing equation $i$ by itself plus $c$ times equation $j$, with $i\ne j$, can be undone by adding $-c$ times the unchanged equation $j$. Equivalently, an [elementary matrix](#elementary-matrix) $E$ is an [invertible matrix](linear-algebra.md#invertible-matrix), so $Ax=b$ if and only if $EAx=Eb$. Applying an operation to $A$ without also applying it to $b$ loses this equivalence.

At step $k$, choose a nonzero [pivot element](#pivot-element) $a_{kk}$ after any row interchange. For every $i>k$, form the [elimination multiplier](#elimination-multiplier) $m_i=a_{ik}/a_{kk}$ and perform the [elementary row operation](#elementary-row-operation) $R_i\leftarrow R_i-m_iR_k$. Its coefficient in column $k$ becomes $a_{ik}-(a_{ik}/a_{kk})a_{kk}=0$ in exact arithmetic. Later operations combine rows that already have zeros in earlier columns, so those zeros survive. If an active column has no nonzero candidate, general [row echelon form](#row-echelon-form) reduction skips it; a square [invertible matrix](linear-algebra.md#invertible-matrix) always has a candidate at each step with suitable row interchanges. [Partial pivoting](#columnwise-partial-pivoting) also considers [roundoff error](numerical-analysis.md#round-off-error) when selecting the candidate.[Fundamentals of Numerical Computation by Tobin A. Driscoll and others; §2.6.1, Definition 2.6.1: select the largest absolute candidate; §2.6.3: permute the right-hand side too](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/2-6-row-pivoting)

For a dense $n\times n$ [matrix](vector-space.md#matrix) with one right-hand side, the classical [algorithm](algorithm.md) uses $\tfrac23n^3+O(n^2)$ [arithmetic operations](numerical-analysis.md#arithmetic-operation) over the [real numbers](arithmetic.md#real-number), counting each [addition](arithmetic.md#addition), [subtraction](arithmetic.md#subtraction), [multiplication](arithmetic.md#multiplication) and [division](arithmetic.md#division-mathematics) as one. At step $k$, the coefficient update has $(n-k)^2$ entries, each costing one [multiplication](arithmetic.md#multiplication) and one [subtraction](arithmetic.md#subtraction); the [elimination multipliers](#elimination-multiplier), right-hand-side updates and [back substitution](linear-algebra.md#back-substitution) contribute lower-order terms. Searching for [partial pivoting](#columnwise-partial-pivoting) adds $O(n^2)$ comparisons, and storing the dense coefficients uses $O(n^2)$ space. These assumptions exclude the different storage and work patterns of [sparse Gaussian elimination](#sparse-gaussian-elimination); the exact loop counts appear in [LU factorization and solve costs](#lu-factorization-and-solve-costs). Here $O$ denotes [Big O notation](real-analysis.md#big-o-notation).

Recording the same steps as an [LU decomposition](#lu-decomposition) makes [Reusing LU factors for multiple right-hand sides](#reusing-lu-factors-for-multiple-right-hand-sides) possible. This is useful whenever the coefficients stay fixed while the forcing [vector](vector-space.md#vector) changes: the expensive elimination is done once. The choice of [pivot element](#pivot-element) matters even when the [linear system](linear-algebra.md#system-of-linear-equations) is well conditioned, as [Tiny-pivot roundoff in Gaussian elimination](#tiny-pivot-roundoff-in-gaussian-elimination) demonstrates.

### Bareiss algorithm

↑ **Parent:** [Gaussian elimination](#gaussian-elimination)

A fraction-free elimination [algorithm](algorithm.md) for exact [determinants](multilinear-algebra.md#determinant). At each stage it divides a cross-multiplied update by the preceding pivot; the determinantal identities underlying the method make this division exact when its pivot assumptions hold. Pivoting handles zero pivots.

### Gaussian elimination with a row swap

↑ **Parent:** [Gaussian elimination](#gaussian-elimination)

Consider this original [linear system](linear-algebra.md#system-of-linear-equations) and its [augmented matrix](linear-algebra.md#augmented-matrix):

$$
A=\begin{pmatrix}0&2&1\\1&-2&-3\\2&3&1\end{pmatrix},\qquad b=\begin{pmatrix}3\\0\\7\end{pmatrix},\qquad [A\mid b]=\left[\begin{array}{rrr|r}0&2&1&3\\1&-2&-3&0\\2&3&1&7\end{array}\right].
$$

The first diagonal entry is zero, so it cannot serve as a [pivot element](#pivot-element). Interchange $R_1$ and $R_2$ to obtain a [pivot element](#pivot-element) of one:

$$
\left[\begin{array}{rrr|r}1&-2&-3&0\\0&2&1&3\\2&3&1&7\end{array}\right].
$$

This chooses a convenient nonzero entry for exact arithmetic; [partial pivoting](#columnwise-partial-pivoting) would instead interchange $R_1$ and $R_3$, selecting the largest [absolute value](real-analysis.md#absolute-value), two. For our chosen ordering, the first-column [elimination multipliers](#elimination-multiplier) are $m_2=0$ and $m_3=2$. The [elementary row operation](#elementary-row-operation) $R_3\leftarrow R_3-2R_1$ gives

$$
\left[\begin{array}{rrr|r}1&-2&-3&0\\0&2&1&3\\0&7&7&7\end{array}\right].
$$

The next [pivot element](#pivot-element) is two and the next [elimination multiplier](#elimination-multiplier) is $7/2$. Applying $R_3\leftarrow R_3-\tfrac72R_2$ gives the [upper triangular matrix](linear-algebra.md#upper-triangular-matrix) system

$$
\left[\begin{array}{rrr|r}1&-2&-3&0\\0&2&1&3\\0&0&\tfrac72&-\tfrac72\end{array}\right].
$$

Every operation also changed the right-hand side. [Back substitution](linear-algebra.md#back-substitution) now gives

$$
x_3=\frac{-7/2}{7/2}=-1,\qquad x_2=\frac{3-x_3}{2}=2,\qquad x_1=2x_2+3x_3=1.
$$

Checking the original equations, rather than only the reduced ones, verifies the answer by [matrix multiplication](vector-space.md#matrix-multiplication):

$$
A\begin{pmatrix}1\\2\\-1\end{pmatrix}=\begin{pmatrix}4-1\\1-4+3\\2+6-1\end{pmatrix}=b.
$$

Thus a zero first diagonal entry was a row-order obstruction, not a [singular matrix](linear-algebra.md#singular-matrix). Indeed, the diagonal product of the final [upper triangular matrix](linear-algebra.md#upper-triangular-matrix) is $7$; the single row interchange makes $\det A=-7$, since the two row additions preserve the [determinant](multilinear-algebra.md#determinant).

<a id="image-a-row-interchange-supplies-the-first-pivot-element-successive-elementary-row-operations-create-zeros-then-back-substitution-gives-1-2-1-t"></a>
![](gaussian-elimination-row-swap-pivots.png)

**[Figure 5](#image-a-row-interchange-supplies-the-first-pivot-element-successive-elementary-row-operations-create-zeros-then-back-substitution-gives-1-2-1-t). A row interchange supplies the first pivot element; successive elementary row operations create zeros, then back substitution gives $(1,2,-1)^T$**.

### Pivot element

↑ **Parent:** [Gaussian elimination](#gaussian-elimination)

A [pivot element](#pivot-element) is the current diagonal entry used to eliminate entries below it in [Gaussian elimination](#gaussian-elimination), after any row interchange. At step $k$ it is $a_{kk}^{(k-1)}$, where $A^{(k-1)}$ is the current reduced [matrix](vector-space.md#matrix). Computing [elimination multipliers](#elimination-multiplier) requires this entry to be nonzero. A zero [pivot element](#pivot-element) can reflect an unsuitable row order even for an [invertible matrix](linear-algebra.md#invertible-matrix), as [Pivoted LU decomposition](#pivoted-lu-decomposition) illustrates.

### Elimination multiplier

↑ **Parent:** [Gaussian elimination](#gaussian-elimination)

For $i>k$, an [elimination multiplier](#elimination-multiplier) is the [scalar](vector-space.md#scalar) $l_{ik}=a_{ik}^{(k-1)}/a_{kk}^{(k-1)}$ used in the [elementary row operation](#elementary-row-operation) $R_i\leftarrow R_i-l_{ik}R_k$. This creates a zero below the [pivot element](#pivot-element). The remaining entries change by $a_{ij}\leftarrow a_{ij}-l_{ik}a_{kj}$ for $j>k$. Storing these [elimination multipliers](#elimination-multiplier) gives the subdiagonal entries of $L$ in [LU decomposition](#lu-decomposition); later row interchanges must also reorder the already stored coefficients.

### Sparse Gaussian elimination

↑ **Parent:** [Gaussian elimination](#gaussian-elimination)

[Sparse Gaussian elimination](#sparse-gaussian-elimination) solves a [linear system](linear-algebra.md#system-of-linear-equations) by [Gaussian elimination](#gaussian-elimination) while exploiting its [sparse matrix](vector-space.md#sparse-matrix) structure to avoid storing zeros and performing unnecessary [arithmetic operations](numerical-analysis.md#arithmetic-operation). The catch is that zeros in the input need not remain zero: eliminating a shared unknown can couple two equations that previously had no direct coupling. These new positions are [fill-in](#fill-in), and their number can depend strongly on the order of elimination.

For a real [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix), the usual direct method is a [Cholesky decomposition](quadratic-form.md#cholesky-decomposition). Choose an ordering, use [symbolic factorization](#symbolic-factorization) to allocate the predicted factor entries, compute their values, then solve two [triangular systems](linear-algebra.md#triangular-system). [Compressed sparse storage](vector-space.md#compressed-sparse-storage) makes the reduced storage useful. General [LU decomposition](#lu-decomposition) may also need numerical [partial pivoting](#columnwise-partial-pivoting), so an ordering chosen for sparsity can change during factorization.[Applications of Parallel Computers, CS267, Spring 1996; CS267, Lecture 27, 23 April 1996, Cholesky versus LU Decomposition: distinction between numerical pivot selection and advance ordering, and phases 1–4; Sparse Matrix Storage Schemes](mathematics-bibliography.md#applications-of-parallel-computers-cs267-spring-1996/lecture-27-sparse-gaussian-elimination)

For a fixed ordering, let $P$ be the [permutation matrix](vector-space.md#permutation-matrix) that puts the unknowns in that order. Permute both rows and columns:

$$
B=PAP^T=CC^T,\qquad Cy=Pb,\qquad C^Tz=y,\qquad x=P^Tz.
$$

Here $C$ is the [lower triangular matrix](linear-algebra.md#lower-triangular-matrix) in the [Cholesky decomposition](quadratic-form.md#cholesky-decomposition) of $B$; $z=Px$. [Forward substitution](#forward-substitution) and [back substitution](linear-algebra.md#back-substitution) give the original solution. The simultaneous permutation preserves the [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) property because $v^TBv=(P^Tv)^TA(P^Tv)>0$ for every nonzero [vector](vector-space.md#vector) $v$. A row permutation alone generally loses the [symmetric matrix](linear-algebra.md#symmetric-matrix) structure.

The local mechanism is a [Schur complement](linear-algebra.md#schur-complement). If the active [pivot element](#pivot-element) is $a_{kk}$, then for remaining indices $i,j$,

$$
a_{ij}^{\mathrm{new}}=a_{ij}-\frac{a_{ik}a_{kj}}{a_{kk}}.
$$

Even when $a_{ij}=0$, two nonzero couplings through $k$ make the second term nonzero. Thus the [elimination graph](#elimination-graph) removes $k$ and joins its remaining neighbors into a [clique](graph-theory.md#clique-graph-theory). The [fill-path criterion for symmetric elimination](#fill-path-criterion-for-symmetric-elimination) extends this local rule across several steps. The [elimination tree](#elimination-tree) organizes the resulting dependencies; the [minimum degree algorithm](#minimum-degree-algorithm) and [nested dissection](#nested-dissection) choose orderings to control them.

This connection between [graphs](graph.md) and [linear systems](linear-algebra.md#system-of-linear-equations) was already explicit in [Donald J. Rose](mathematics-author.md#donald-j-rose), [R. Endre Tarjan](computer-science.md#robert-tarjan) and [George S. Lueker](mathematics-author.md#george-s-lueker)'s 1976 study of [fill-in](#fill-in) and [perfect elimination orderings](graph-theory.md#perfect-elimination-ordering).[Abstract: symmetric positive-definite systems, fill calculation for a prescribed ordering, and algorithms for special orderings; publication information, June 1976](mathematics-bibliography.md#algorithmic-aspects-of-vertex-elimination-on-graphs-by-donald-j-rose-and-others)

#### Sparse elimination of a four-leaf star

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

Take a [star graph](bipartite-graph.md#star-graph-theory) $G$ with center $c$ and four leaves $1,2,3,4$. Let $L_G$ be its [Laplacian matrix](graph-theory.md#laplacian-matrix) and $I$ the [identity matrix](vector-space.md#identity-matrix). In the order $(c,1,2,3,4)$, the original example is

$$
A=I+L_G=\begin{pmatrix}
5&-1&-1&-1&-1\\
-1&2&0&0&0\\
-1&0&2&0&0\\
-1&0&0&2&0\\
-1&0&0&0&2
\end{pmatrix}.
$$

For a nonzero [vector](vector-space.md#vector) $u$, its [quadratic form](quadratic-form.md) is

$$
u^TAu=u_c^2+\sum_{i=1}^4u_i^2+\sum_{i=1}^4(u_c-u_i)^2>0.
$$

Thus $A$ is a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) and either ordering below admits a [Cholesky decomposition](quadratic-form.md#cholesky-decomposition). Changing the ordering changes the work, rather than the mathematical solvability.

**Center first.** Eliminating $c$ with [pivot element](#pivot-element) $5$ leaves the [Schur complement](linear-algebra.md#schur-complement)

$$
S=2I_4-\frac15\mathbf1\mathbf1^T
=\frac15\begin{pmatrix}9&-1&-1&-1\\-1&9&-1&-1\\-1&-1&9&-1\\-1&-1&-1&9\end{pmatrix},
\qquad \mathbf1=(1,1,1,1)^T.
$$

Every pair of leaves now has coupling $-1/5$: six new [edges](graph-theory.md#edge-of-a-graph), hence six undirected [fill-in](#fill-in) positions. The four remaining [vertices](graph.md#vertex-graph-theory) form a [clique](graph-theory.md#clique-graph-theory). In the [Cholesky decomposition](quadratic-form.md#cholesky-decomposition), the first column has $C_{cc}=\sqrt5$ and $C_{ic}=-1/\sqrt5$. The rest of the [lower triangular matrix](linear-algebra.md#lower-triangular-matrix) is dense. To check that later cancellation does not remove its entries, after $r$ leaves have also been eliminated, the active leaf block is

$$
2I_{4-r}-\alpha_r\mathbf1\mathbf1^T,\qquad
\alpha_r=\frac{2}{10-r},\qquad 0\leq r\leq3.
$$

Indeed a leaf step sends $\alpha$ to $\alpha+\alpha^2/(2-\alpha)$. All active off-diagonal entries remain negative. The successive [pivot elements](#pivot-element) in ordinary symmetric [Gaussian elimination](#gaussian-elimination), equivalently the squared diagonals in the [Cholesky decomposition](quadratic-form.md#cholesky-decomposition), are

$$
5,\quad\frac95,\quad\frac{16}9,\quad\frac74,\quad\frac{12}7.
$$

The [Cholesky decomposition](quadratic-form.md#cholesky-decomposition) therefore stores $5+4+3+2+1=15$ nonzero entries, including its diagonal.

**Leaves first.** Permute to $(1,2,3,4,c)$. Each leaf has only one remaining neighbor, so its elimination changes only the center's diagonal, reducing it by $(-1)^2/2=1/2$. The successive [pivot elements](#pivot-element) are $2,2,2,2,3$, and the exact [Cholesky decomposition](quadratic-form.md#cholesky-decomposition) is

$$
PAP^T=CC^T,\qquad
C=\begin{pmatrix}
\sqrt2&0&0&0&0\\
0&\sqrt2&0&0&0\\
0&0&\sqrt2&0&0\\
0&0&0&\sqrt2&0\\
-1/\sqrt2&-1/\sqrt2&-1/\sqrt2&-1/\sqrt2&\sqrt3
\end{pmatrix}.
$$

There is no [fill-in](#fill-in), and only $5+4=9$ nonzero entries in $C$. This is a concrete instance of [leaf elimination of a tree-pattern positive-definite matrix](#leaf-elimination-of-a-tree-pattern-positive-definite-matrix); its general proof explains why the same idea works on every [tree](tree-graph-theory.md) pattern. The [minimum degree algorithm](#minimum-degree-algorithm) also chooses a leaf at every nontrivial stage of this particular example, but that success gives no general optimality guarantee.

<a id="image-eliminating-the-center-of-a-four-leaf-star-graph-creates-a-clique-eliminating-leaves-creates-no-fill-in"></a>
![](sparse-star-elimination-graphs.png)

**[Figure 6](#image-eliminating-the-center-of-a-four-leaf-star-graph-creates-a-clique-eliminating-leaves-creates-no-fill-in). Eliminating the center of a four-leaf star graph creates a clique; eliminating leaves creates no fill-in**.

<a id="image-the-same-symmetric-positive-definite-matrix-has-15-or-nine-nonzero-cholesky-decomposition-factor-entries-depending-on-its-ordering"></a>
![](sparse-star-cholesky-patterns.png)

**[Figure 7](#image-the-same-symmetric-positive-definite-matrix-has-15-or-nine-nonzero-cholesky-decomposition-factor-entries-depending-on-its-ordering). The same symmetric positive-definite matrix has 15 or nine nonzero Cholesky decomposition factor entries, depending on its ordering**.

The input has 13 nonzero [matrix elements](vector-space.md#matrix-element) when both symmetric halves are counted, or nine in its lower triangle. The six added undirected [edges](graph-theory.md#edge-of-a-graph) correspond to six added positions in one triangular factor, or 12 positions if both symmetric halves of the filled pattern are displayed. Comparing all 13 input entries directly with the 15 entries of $C$ would mix counting conventions.

#### Leaf elimination of a tree-pattern positive-definite matrix

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

Associate an undirected graph with a symmetric matrix's off-diagonal nonzero pattern. Eliminating vertex $i$ updates the remaining matrix by $a_{jk}\mapsto a_{jk}-a_{ji}a_{ik}/a_{ii}$. Only pairs of neighbors of $i$ can acquire [fill-in](#fill-in). If the graph is a tree, remove leaves successively: each eliminated vertex has at most one remaining neighbor, so only a diagonal entry can change. Every [Schur complement](linear-algebra.md#schur-complement) of a [positive-definite matrix](quadratic-form.md#positive-definite-matrix) is positive definite, so no zero pivot forces a different ordering. Leaf removal therefore constructs a [perfect elimination ordering](graph-theory.md#perfect-elimination-ordering) and a fill-free factorization.

#### Symbolic factorization

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

[Symbolic factorization](#symbolic-factorization) computes possible nonzero positions and update dependencies from a [sparse matrix](vector-space.md#sparse-matrix) pattern and ordering before calculating numerical factor values. The [elimination graph](#elimination-graph) predicts fill and the [elimination tree](#elimination-tree) organizes dependencies. Numerical pivoting or exceptional cancellation can make the computed factor pattern differ from this structural prediction.

#### Elimination tree

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

For a symmetric factorization in a fixed ordering, the [elimination tree](#elimination-tree) assigns the displayed parent to a column of the lower-triangular factor when that set is nonempty. A column with no later entry is a root. The tree records dependencies of descendant updates on later pivots, supports symbolic factor allocation, and exposes parallel subtrees. It describes the factorization ordering, not merely a spanning tree of the original [matrix graph](#matrix-graph).

#### Nested dissection

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

A [vertex separator](graph-theory.md#vertex-separator) divides the remaining unknowns into disconnected subdomains. Nested dissection recursively eliminates each subdomain before its separator, keeping interaction localized until late in the factorization. For a regular two-dimensional mesh with $N$ unknowns, separators have size $O(\sqrt N)$; the resulting direct factorization uses $O(N^{3/2})$ work and $O(N\log N)$ storage under the usual geometric separator assumptions.

#### Minimum degree algorithm

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

At each step choose a remaining vertex of minimum degree in the current [elimination graph](#elimination-graph). This heuristic reduces the size of the immediate [Schur complement](linear-algebra.md#schur-complement) update and often reduces [fill-in](#fill-in), but does not guarantee a globally optimal ordering. Its degrees must reflect earlier fill, rather than just the original [graph](graph.md).

#### Fill-in

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

[Fill-in](#fill-in) consists of new nonzero positions created by [Gaussian elimination](#gaussian-elimination), absent from the original [sparse matrix](vector-space.md#sparse-matrix) in the same ordering. For a [Cholesky decomposition](quadratic-form.md#cholesky-decomposition) $PAP^T=CC^T$, compare $C$ with the lower triangle of $PAP^T$, not with the unpermuted input. Each new undirected [edge](graph-theory.md#edge-of-a-graph) of the [elimination graph](#elimination-graph) contributes one structural position in $C$. The [sparse elimination of a four-leaf star](#sparse-elimination-of-a-four-leaf-star) gives six such positions when the center is eliminated first, and none when the leaves are eliminated first.

[Symbolic factorization](#symbolic-factorization) predicts possible nonzeros from the pattern alone. An initially zero $a_{ij}$ becomes nonzero in a single scalar step if both $a_{ik}$ and $a_{kj}$ are nonzero; however, at later steps several contributions can cancel. For an exact example, let

$$
H=\begin{pmatrix}2&1&1&0\\1&2&0&1\\1&0&3&-1/3\\0&1&-1/3&3\end{pmatrix}.
$$

Eliminate indices $1,2$ in that order. The first [Schur complement](linear-algebra.md#schur-complement), in order $(2,3,4)$, is

$$
\begin{pmatrix}3/2&-1/2&1\\-1/2&5/2&-1/3\\1&-1/3&3\end{pmatrix}.
$$

The second [pivot element](#pivot-element) updates the $(3,4)$ entry to $-1/3-(-1/2)(1)/(3/2)=0$. The remaining block is $\operatorname{diag}(7/3,7/3)$, so all four [pivot elements](#pivot-element) are positive and $H$ is a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix). The [elimination graph](#elimination-graph) retains the structural [edge](graph-theory.md#edge-of-a-graph) $3-4$, but this exact choice of coefficients makes the numerical entry vanish. A small change to $H_{34}=H_{43}$ generally removes the cancellation.

Such an exact zero is different from discarding a small value computed with [floating-point arithmetic](floating-point-arithmetic.md). The [symbolic factorization](#symbolic-factorization) deliberately reserves space for possible entries without depending on special numerical identities. A [perfect elimination ordering](graph-theory.md#perfect-elimination-ordering) creates no structural [fill-in](#fill-in) at all; an ordering with cancellations need not have that property.

#### Matrix graph

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

For a symmetric [sparse matrix](vector-space.md#sparse-matrix), its [matrix graph](#matrix-graph) has one vertex per unknown and an edge $i-j$ whenever the off-diagonal entry $a_{ij}$ is structurally nonzero. Simultaneous row and column permutation relabels this [graph](graph.md). Nonsymmetric patterns are instead represented by directed or bipartite [graphs](graph.md) when row and column roles must be distinguished.

##### Elimination graph

↑ **Parent:** [Matrix graph](#matrix-graph)

One step of symmetric [Gaussian elimination](#gaussian-elimination) removes the pivot vertex and connects its remaining neighbors into a [clique](graph-theory.md#clique-graph-theory). The rule follows from the [Schur complement](linear-algebra.md#schur-complement) update $a_{ij}\leftarrow a_{ij}-a_{ik}a_{kj}/a_{kk}$. Repeating it predicts the generic factor sparsity; exceptional numerical cancellations can remove structurally predicted entries.

###### Fill-path criterion for symmetric elimination

↑ **Parent:** [Elimination graph](#elimination-graph)

After eliminating a vertex set $E$, a generic edge between remaining vertices $i,j$ exists exactly when the original [matrix graph](#matrix-graph) contains a path from $i$ to $j$ whose internal vertices all belong to $E$. Inductively, the new edges at pivot $k$ concatenate two such paths through $k$; conversely split any allowed path at $k$, or retain it when it avoids $k$. This characterizes fill by [graph](graph.md) reachability.

### Columnwise partial pivoting

↑ **Parent:** [Gaussian elimination](#gaussian-elimination)

At each step of [Gaussian elimination](#gaussian-elimination), select the largest absolute entry in the uneliminated part of the current column and interchange rows to put it on the diagonal. A nonsingular trailing [Schur complement](linear-algebra.md#schur-complement) has a nonzero entry in its first column, so this procedure always finds a nonzero pivot in exact arithmetic. The [permutation matrix](vector-space.md#permutation-matrix) $P$ records row interchanges; earlier multipliers must be interchanged too when assembling the lower-triangular factor. This yields the [LU decomposition](#lu-decomposition) $PA=LU$ with unit diagonal in $L$. Searching within columns and interchanging rows is distinct from interchanging columns.

#### Tiny-pivot roundoff in Gaussian elimination

↑ **Parent:** [Columnwise partial pivoting](#columnwise-partial-pivoting)

A nonzero [pivot element](#pivot-element) can still be a poor numerical choice. [Partial pivoting](#columnwise-partial-pivoting) bounds the [absolute values](real-analysis.md#absolute-value) of the [elimination multipliers](#elimination-multiplier) by one in exact arithmetic, because each numerator is no larger than the selected denominator. This usually improves [numerical stability](numerical-analysis.md#stability-of-a-numerical-method), but does not prevent every possible growth of intermediate entries or guarantee accurate answers for every [linear system](linear-algebra.md#system-of-linear-equations).[Fundamentals of Numerical Computation by Tobin A. Driscoll and others; §2.6.4, Example 2.6.6, equation (2.6.3) and concluding discussion: small-pivot instability and the limits of pivoting](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/2-6-row-pivoting)

To see the mechanism without depending on hardware, define a toy [floating-point arithmetic](floating-point-arithmetic.md) model. The operator $\operatorname{fl}_3(z)$ rounds an exact [real number](arithmetic.md#real-number) to the nearest value with three significant decimal digits; halfway cases choose the even final digit, and $\operatorname{fl}_3(0)=0$. Allow an unbounded exponent range. Round the inputs and the result of every [addition](arithmetic.md#addition), [subtraction](arithmetic.md#subtraction), [multiplication](arithmetic.md#multiplication) and [division](arithmetic.md#division-mathematics) separately; a product followed by a [subtraction](arithmetic.md#subtraction) rounds twice. This is a prescribed arithmetic model, not a measurement of a physical computer. All inputs in the following original example are represented exactly:

$$
\varepsilon=10^{-6},\qquad A=\begin{pmatrix}\varepsilon&1\\1&1\end{pmatrix},\qquad b=\begin{pmatrix}1\\2\end{pmatrix}.
$$

Without a row interchange, the [elimination multiplier](#elimination-multiplier) is $m=\operatorname{fl}_3(1/\varepsilon)=10^6$. The last coefficient and right-hand side become

$$
\widehat u_{22}=\operatorname{fl}_3\bigl(1-\operatorname{fl}_3(m\cdot1)\bigr)=\operatorname{fl}_3(-999999)=-10^6,
$$



$$
\widehat c_2=\operatorname{fl}_3\bigl(2-\operatorname{fl}_3(m\cdot1)\bigr)=\operatorname{fl}_3(-999998)=-10^6.
$$

Two distinct exact values now have the same rounded representation. [Back substitution](linear-algebra.md#back-substitution) therefore returns

$$
\widehat x_2=\operatorname{fl}_3(\widehat c_2/\widehat u_{22})=1,\qquad \widehat x_1=\operatorname{fl}_3\left(\frac{\operatorname{fl}_3(1-\operatorname{fl}_3(1\cdot\widehat x_2))}{\varepsilon}\right)=0.
$$

The small difference carrying information about $x_1$ was lost during elimination; the final [subtraction](arithmetic.md#subtraction) only exposes that loss. Dividing by the tiny [pivot element](#pivot-element) amplifies sensitivity to the lost information.

With [partial pivoting](#columnwise-partial-pivoting), interchange the two rows, including their right-hand sides, to start from $\left[\begin{smallmatrix}1&1&2\\\varepsilon&1&1\end{smallmatrix}\right]$. Now $m=\operatorname{fl}_3(\varepsilon/1)=\varepsilon$, and the rounded updates are

$$
\widehat u_{22}=\operatorname{fl}_3\bigl(1-\operatorname{fl}_3(\varepsilon\cdot1)\bigr)=\operatorname{fl}_3(0.999999)=1,
$$



$$
\widehat c_2=\operatorname{fl}_3\bigl(1-\operatorname{fl}_3(\varepsilon\cdot2)\bigr)=\operatorname{fl}_3(0.999998)=1.
$$

[Back substitution](linear-algebra.md#back-substitution) gives $\widehat x_2=\operatorname{fl}_3(1/1)=1$ and $\widehat x_1=\operatorname{fl}_3(\operatorname{fl}_3(2-\operatorname{fl}_3(1\cdot1))/1)=1$. Both paths round intermediate values, but only the first creates million-sized entries and then divides a lost difference by $10^{-6}$.

The true solution follows from the original second equation $x_2=2-x_1$:

$$
x_* =\begin{pmatrix}\dfrac{1}{1-\varepsilon}\\[2pt]\dfrac{1-2\varepsilon}{1-\varepsilon}\end{pmatrix}=\begin{pmatrix}1.000001000001\ldots\\0.999998999999\ldots\end{pmatrix}.
$$

Evaluate the [linear-system residual](gradient-descent.md#linear-system-residual) $r=b-A\widehat x$ against the original data in exact arithmetic, separately from the three-digit solve. With $\|v\|_\infty=\max_i|v_i|$, the [maximum norm](normed-vector-space.md#supremum-norm), the results are

$$
\begin{array}{c|c|c|c}
\text{procedure}&\widehat x&r&\|\widehat x-x_*\|_\infty/\|x_*\|_\infty\\\hline
\text{no row interchange}&(0,1)^T&(0,1)^T&1\\
\text{partial pivoting}&(1,1)^T&(-10^{-6},0)^T&10^{-6}
\end{array}
$$

The respective relative [linear-system residuals](gradient-descent.md#linear-system-residual) $\|r\|_\infty/\|b\|_\infty$ are $1/2$ and $5\times10^{-7}$. Computing the diagnostic in higher precision matters: a check made only against the rounded reduced equations would miss the original error.

<a id="image-the-same-three-digit-floating-point-arithmetic-model-gives-0-1-t-without-a-row-interchange-and-1-1-t-with-partial-pivoting-exact-linear-system-residuals-expose-the-difference"></a>
![](gaussian-elimination-tiny-pivot-roundoff.png)

**[Figure 8](#image-the-same-three-digit-floating-point-arithmetic-model-gives-0-1-t-without-a-row-interchange-and-1-1-t-with-partial-pivoting-exact-linear-system-residuals-expose-the-difference). The same three-digit floating-point arithmetic model gives $(0,1)^T$ without a row interchange and $(1,1)^T$ with partial pivoting; exact linear-system residuals expose the difference**.

This [matrix](vector-space.md#matrix) is well conditioned in the [maximum norm](normed-vector-space.md#supremum-norm): its induced [matrix norm](vector-space.md#matrix-norm) is $\|A\|_\infty=2$, while

$$
A^{-1}=\frac{1}{1-\varepsilon}\begin{pmatrix}-1&1\\1&-\varepsilon\end{pmatrix},\qquad \kappa_\infty(A)=\|A\|_\infty\|A^{-1}\|_\infty=\frac{4}{1-\varepsilon}\approx4.000004.
$$

The failure therefore belongs to this unpivoted [algorithm](algorithm.md), rather than a large [condition number](quadratic-form.md#condition-number). In general, however, [partial pivoting](#columnwise-partial-pivoting) cannot remove sensitivity inherent in the data. For any approximate solution of an [invertible matrix](linear-algebra.md#invertible-matrix) system, $\widehat x-x_*=-A^{-1}r$; the induced [matrix norm](vector-space.md#matrix-norm) inequality and $\|b\|\leq\|A\|\|x_*\|$ give

$$
\frac{\|\widehat x-x_*\|}{\|x_*\|}\leq\kappa(A)\frac{\|r\|}{\|b\|}.
$$

A small [linear-system residual](gradient-descent.md#linear-system-residual) controls solution error only in conjunction with the [condition number](quadratic-form.md#condition-number); [numerical stability](numerical-analysis.md#stability-of-a-numerical-method) and sensitivity are different questions.[Fundamentals of Numerical Computation by Tobin A. Driscoll and others; Definition 2.8.1, equation (2.8.5); §2.8.1, Theorem 2.8.1, equation (2.8.6): condition number and right-hand-side sensitivity; the residual identity above applies that bound](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/2-8-conditioning-of-linear-systems)

### Row echelon form

↑ **Parent:** [Gaussian elimination](#gaussian-elimination)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Row_echelon_form)

A [matrix](vector-space.md#matrix) over a [field](algebra.md#field) $\mathbb F$ is in [row echelon form](#row-echelon-form) when all zero rows follow the nonzero rows, each nonzero row's first nonzero entry lies strictly to the right of the preceding row's first nonzero entry, and all entries below each such leading entry vanish. These leading entries are its [pivot elements](#pivot-element). They need not be one, and entries above them need not vanish.[Interactive Linear Algebra by Dan Margalit and others; §1.2.2, Echelon Forms: three echelon conditions and definition of a pivot](mathematics-bibliography.md#interactive-linear-algebra-by-dan-margalit-and-others/row-reduction)

The staircase turns a [linear system](linear-algebra.md#system-of-linear-equations) into a sequence of simpler equations. For example,

$$
U=\begin{pmatrix}1&2&-1\\0&1&3\\0&0&0\\0&0&0\end{pmatrix}
$$

is in [row echelon form](#row-echelon-form), with [pivot columns](vector-space.md#pivot-column) 1 and 2. Its second equation determines $x_2$ once $x_3$ is chosen; its first then determines $x_1$ by [back substitution](linear-algebra.md#back-substitution). It is not in [reduced row echelon form](#reduced-row-echelon-form), because the second [pivot column](vector-space.md#pivot-column) contains a nonzero entry above its [pivot element](#pivot-element). Neither being square nor having a nonzero entry in every row is required.

[Elementary row operations](#elementary-row-operation) bring every [matrix](vector-space.md#matrix) to [row echelon form](#row-echelon-form): choose a nonzero entry in the leftmost available nonzero column, interchange rows, clear entries below it, and repeat on the remaining rows and later columns. Skip columns with no remaining nonzero entry. Clearing above each [pivot element](#pivot-element) and scaling it to one completes [reduced row echelon form](#reduced-row-echelon-form).[Interactive Linear Algebra by Dan Margalit and others; §1.2.3, The Row Reduction Algorithm, forward steps and Last Step](mathematics-bibliography.md#interactive-linear-algebra-by-dan-margalit-and-others/row-reduction)

The nonzero rows of an [row echelon form](#row-echelon-form) are [linearly independent](vector-space.md#linear-independence): in a vanishing [linear combination](vector-space.md#linear-combination), inspecting the first [pivot column](vector-space.md#pivot-column) forces the first coefficient to be zero, then the next forces the second, and so on. They give a [basis](vector-space.md#basis) of the original [row space](vector-space.md#row-space). The number of [pivot elements](#pivot-element) is both the [row rank](vector-space.md#row-rank) and the [column rank](vector-space.md#column-rank). To recover a [basis](vector-space.md#basis) of the original [column space](vector-space.md#column-space), select the corresponding original [pivot columns](vector-space.md#pivot-column); the reduced column [vectors](vector-space.md#vector) generally belong to a different [column space](vector-space.md#column-space).

Here the arithmetic is exact in the specified [field](algebra.md#field). For [floating-point arithmetic](floating-point-arithmetic.md), deciding whether a computed entry counts as zero requires a numerical criterion; see [Tiny-pivot roundoff in Gaussian elimination](#tiny-pivot-roundoff-in-gaussian-elimination) and [condition number](quadratic-form.md#condition-number). An exact [row echelon form](#row-echelon-form) classification alone does not settle [numerical stability](numerical-analysis.md#stability-of-a-numerical-method).

#### Row-equivalent matrices

↑ **Parent:** [Row echelon form](#row-echelon-form)

Two [matrices](vector-space.md#matrix) of the same size over the same [field](algebra.md#field) are [row-equivalent matrices](#row-equivalent-matrices) if a sequence of [elementary row operations](#elementary-row-operation) transforms one into the other.[Interactive Linear Algebra by Dan Margalit and others; §1.2.1, definition of row equivalence](mathematics-bibliography.md#interactive-linear-algebra-by-dan-margalit-and-others/row-reduction) Every operation is reversible, so they have the same [row space](vector-space.md#row-space) and the same column [linear relations](vector-space.md#linear-relation). Writing the entire sequence as multiplication by an [invertible matrix](linear-algebra.md#invertible-matrix) gives $R=EA$ and

$$
Az=0\ \Longleftrightarrow\ Rz=0,\qquad
Ax=b\ \Longleftrightarrow\ Rx=Eb.
$$

Thus the [kernel](kernel-of-a-linear-map.md) is preserved. For a nonzero right-hand side, perform every operation on the whole [augmented matrix](linear-algebra.md#augmented-matrix) $[A\mid b]$: changing the coefficients while keeping $b$ fixed generally changes the solutions. The [column space](vector-space.md#column-space) instead transforms to $E\operatorname{col}A$, which need not equal $\operatorname{col}A$.

#### Row reduction with a parameterized right-hand side

↑ **Parent:** [Row echelon form](#row-echelon-form)

Work over the [rational numbers](number-theory.md#rational-number), allowing unknowns in the [real numbers](arithmetic.md#real-number) when interpreting the geometry. Consider four equations in three unknowns:

$$
A=\begin{pmatrix}1&2&-1\\2&5&1\\3&7&0\\1&3&2\end{pmatrix},\qquad
b(\tau)=\begin{pmatrix}1\\4\\\tau\\3\end{pmatrix},\qquad Ax=b(\tau).
$$

The third row of $A$ is the sum of its first two rows, and the fourth is their difference, second minus first. The same relations must hold on the right: consistency requires $\tau=1+4=5$ and $3=4-1$. The latter condition already holds. [Gaussian elimination](#gaussian-elimination) makes this compatibility test explicit while exposing the remaining freedom.

Apply the [elementary row operations](#elementary-row-operation) in this order, using each row's current value:

$$
R_2\leftarrow R_2-2R_1,\quad R_3\leftarrow R_3-3R_1,\quad R_4\leftarrow R_4-R_1,
$$

then $R_3\leftarrow R_3-R_2$ and $R_4\leftarrow R_4-R_2$. The resulting [augmented matrix](linear-algebra.md#augmented-matrix) is in [row echelon form](#row-echelon-form) for every $\tau$:

$$
\left[\begin{array}{rrr|r}1&2&-1&1\\0&1&3&2\\0&0&0&\tau-5\\0&0&0&0\end{array}\right].
$$

When $\tau\ne5$, the third row has its [pivot element](#pivot-element) in the augmented column. It says $0=\tau-5$, so the [linear system](linear-algebra.md#system-of-linear-equations) has no solution. When $\tau=5$, that entire row vanishes and only two [pivot elements](#pivot-element) remain. More equations than unknowns therefore do not force a unique solution: some equations may repeat information.

The final operation $R_1\leftarrow R_1-2R_2$ reduces the coefficient block to

$$
R=\begin{pmatrix}1&0&-7\\0&1&3\\0&0&0\\0&0&0\end{pmatrix},\qquad
Eb(\tau)=\begin{pmatrix}-3\\2\\\tau-5\\0\end{pmatrix}.
$$

The product of all six [elementary matrices](#elementary-matrix) is

$$
E=\begin{pmatrix}5&-2&0&0\\-2&1&0&0\\-1&-1&1&0\\1&-1&0&1\end{pmatrix},\qquad EA=R.
$$

Direct [matrix multiplication](vector-space.md#matrix-multiplication) verifies both displayed transformations. Its [determinant](multilinear-algebra.md#determinant) is one, so this transformation is reversible. In particular, the third row of $E$ extracts the discrepancy between the third equation and the sum of the first two.

<a id="image-row-echelon-form-exposes-compatibility-a-right-hand-side-pivot-element-distinguishes-inconsistency-from-a-free-variable-in-a-linear-system"></a>
![](row-echelon-parameter-pivots.png)

**[Figure 9](#image-row-echelon-form-exposes-compatibility-a-right-hand-side-pivot-element-distinguishes-inconsistency-from-a-free-variable-in-a-linear-system). Row echelon form exposes compatibility; a right-hand-side pivot element distinguishes inconsistency from a free variable in a linear system**.

For $\tau=5$, $[R\mid Eb]$ is the [reduced row echelon form](#reduced-row-echelon-form) of the full [augmented matrix](linear-algebra.md#augmented-matrix). For $\tau\ne5$, only its coefficient block is reduced: scale the third row by $1/(\tau-5)$ and clear the entries above its augmented [pivot element](#pivot-element). The full [reduced row echelon form](#reduced-row-echelon-form) is then

$$
\left[\begin{array}{rrr|r}1&0&-7&0\\0&1&3&0\\0&0&0&1\\0&0&0&0\end{array}\right].
$$

The last column is part of the [matrix](vector-space.md#matrix) when testing the echelon conditions. Calling $[R\mid Eb]$ fully reduced before clearing that column would miss this distinction.

#### Reduced row echelon form

↑ **Parent:** [Row echelon form](#row-echelon-form)

A [row echelon form](#row-echelon-form) is in [reduced row echelon form](#reduced-row-echelon-form) when every [pivot element](#pivot-element) is one and is the only nonzero entry in its column.[Interactive Linear Algebra by Dan Margalit and others; §1.2.2, reduced echelon conditions 4 and 5](mathematics-bibliography.md#interactive-linear-algebra-by-dan-margalit-and-others/row-reduction) This extra reduction displays each pivot unknown directly in terms of the [free variables in a linear system](linear-algebra.md#free-variable-in-a-linear-system). The zero [matrix](vector-space.md#matrix) also satisfies the definition: it has no [pivot elements](#pivot-element).

Every [matrix](vector-space.md#matrix) has exactly one [reduced row echelon form](#reduced-row-echelon-form) under [elementary row operations](#elementary-row-operation), with its size and column order held fixed.[Interactive Linear Algebra by Dan Margalit and others; §1.2.3, theorem preceding the Row Reduction Algorithm](mathematics-bibliography.md#interactive-linear-algebra-by-dan-margalit-and-others/row-reduction) Ordinary [row echelon form](#row-echelon-form) is not unique: multiplying a nonzero row by two over the [rational numbers](number-theory.md#rational-number) keeps the staircase but changes the [matrix](vector-space.md#matrix). The reduced conditions remove that freedom.

For a fixed number of columns, each [row space](vector-space.md#row-space) has a unique reduced [matrix](vector-space.md#matrix) after zero rows are removed; at a fixed full size, the number of appended zero rows is also determined. Thus [reduced row echelon form](#reduced-row-echelon-form) represents a [vector subspace](vector-space.md#vector-subspace) independently of the starting [basis](vector-space.md#basis). This is the uniqueness used by [Gaussian binomial coefficients](binomial-coefficient.md#gaussian-binomial-coefficient) to count [vector subspaces](vector-space.md#vector-subspace) over a [finite field](algebra.md#finite-field).

The fixed column order matters. [Elementary column operations](vector-space.md#elementary-column-operation) can change the [row space](vector-space.md#row-space), the [kernel](kernel-of-a-linear-map.md) and the resulting [reduced row echelon form](#reduced-row-echelon-form). For instance, swapping the columns of $(1\ \ 2)$ over the [rational numbers](number-theory.md#rational-number) gives $(2\ \ 1)$, whose [reduced row echelon form](#reduced-row-echelon-form) is $(1\ \ 1/2)$ instead of $(1\ \ 2)$. When solving a [linear system](linear-algebra.md#system-of-linear-equations), a column interchange also requires tracking the corresponding interchange of unknowns.

##### Reading solutions from reduced row echelon form

↑ **Parent:** [Reduced row echelon form](#reduced-row-echelon-form)

For [row reduction with a parameterized right-hand side](#row-reduction-with-a-parameterized-right-hand-side) at $\tau=5$, the nonzero reduced equations are

$$
x_1-7x_3=-3,\qquad x_2+3x_3=2.
$$

Column 3 has no [pivot element](#pivot-element), so $x_3$ is a [free variable in a linear system](linear-algebra.md#free-variable-in-a-linear-system). Taking $x_3=t$ gives every solution:

$$
x=x_0+tv,\qquad x_0=\begin{pmatrix}-3\\2\\0\end{pmatrix},\quad v=\begin{pmatrix}7\\-3\\1\end{pmatrix},\quad t\in\mathbb R.
$$

There is no further restriction on $t$. Independent substitution into the original [linear system](linear-algebra.md#system-of-linear-equations) gives

$$
Ax_0=\begin{pmatrix}1\\4\\5\\3\end{pmatrix},\qquad Av=\begin{pmatrix}7-6-1\\14-15+1\\21-21\\7-9+2\end{pmatrix}=0.
$$

Conversely, the two reduced equations force exactly these coordinate formulas, so no solutions have been omitted. The same computation with zero right-hand side gives the [kernel](kernel-of-a-linear-map.md) $\ker A=\operatorname{span}\{v\}$. Its [dimension](vector-space.md#dimension-vector-space) is one. The [rank-nullity theorem](kernel-of-a-linear-map.md#rank-nullity-theorem) appears here as $2+1=3$: two [pivot columns](vector-space.md#pivot-column) and one freely chosen coordinate account for the three unknowns.[Interactive Linear Algebra by Dan Margalit and others; §2.9, Rank Theorem and preceding pivot-column/free-variable count](mathematics-bibliography.md#interactive-linear-algebra-by-dan-margalit-and-others/the-rank-theorem)

<a id="image-one-free-variable-in-a-linear-system-traces-an-affine-solution-space-of-a-linear-equation-parallel-to-its-kernel"></a>
![](row-echelon-affine-solution-line.png)

**[Figure 10](#image-one-free-variable-in-a-linear-system-traces-an-affine-solution-space-of-a-linear-equation-parallel-to-its-kernel). One free variable in a linear system traces an affine solution space of a linear equation parallel to its kernel**.

In general a consistent [linear system](linear-algebra.md#system-of-linear-equations) has solution set $x_0+\ker A$. Subtracting $Ax_0=b$ from $Ax=b$ proves this description in both directions. The particular solution places the [affine subspace](vector-space.md#affine-subspace), and the [kernel](kernel-of-a-linear-map.md) supplies its directions.[Interactive Linear Algebra by Dan Margalit and others; §2.4.2, Key Observation and its proof: translate homogeneous solutions by any particular solution](mathematics-bibliography.md#interactive-linear-algebra-by-dan-margalit-and-others/solution-sets) Over the [real numbers](arithmetic.md#real-number) this example is an entire line; over the [rational numbers](number-theory.md#rational-number) the same formula uses rational $t$. A [free variable in a linear system](linear-algebra.md#free-variable-in-a-linear-system) over a [finite field](algebra.md#finite-field) instead has only finitely many choices.

The [pivot columns](vector-space.md#pivot-column) identify a different object: the original [column space](vector-space.md#column-space). Here they select

$$
a_1=(1,2,3,1)^T,\qquad a_2=(2,5,7,3)^T,
$$

which form its [basis](vector-space.md#basis), while $a_3=-7a_1+3a_2$. The corresponding reduced columns are $(1,0,0,0)^T$ and $(0,1,0,0)^T$; their [linear span](vector-space.md#linear-span) is a different [plane](geometry-and-topology.md#plane). For example, every original output satisfies $y_3=y_1+y_2$, but $(1,0,0,0)^T$ does not. Since $E$ is an [invertible matrix](linear-algebra.md#invertible-matrix), column [linear relations](vector-space.md#linear-relation) survive $EA=R$ even though the output [vectors](vector-space.md#vector) move. This is why choosing original columns at the reduced pivot positions works.

##### Uniqueness of reduced row echelon form

↑ **Parent:** [Reduced row echelon form](#reduced-row-echelon-form)

Here is a short proof that uses only the [row space](vector-space.md#row-space). For a [vector subspace](vector-space.md#vector-subspace) $W\subseteq\mathbb F^n$, let $d_j$ be the [dimension](vector-space.md#dimension-vector-space) of its [projection map](function.md#projection-map) onto the first $j$ coordinates, with $d_0=0$. In any [reduced row echelon form](#reduced-row-echelon-form) with [row space](vector-space.md#row-space) $W$, $d_j$ counts the [pivot columns](vector-space.md#pivot-column) among those first $j$ columns: later-pivot rows project to zero, while earlier-pivot rows remain [linearly independent](vector-space.md#linear-independence). Thus the positions where $d_j-d_{j-1}=1$ determine all pivot positions from $W$ alone.

If those positions are $p_1,\ldots,p_r$, the map sending $w\in W$ to $(w_{p_1},\ldots,w_{p_r})$ is an [isomorphism](algebra.md#isomorphism) $W\to\mathbb F^r$: the reduced nonzero rows map to the [standard basis](vector-space.md#standard-basis). Its $i$th row is therefore the unique [vector](vector-space.md#vector) of $W$ with pivot-coordinate values equal to the $i$th [standard basis](vector-space.md#standard-basis) vector. Any other [reduced row echelon form](#reduced-row-echelon-form) with that [row space](vector-space.md#row-space) has identical nonzero rows in identical order. At a fixed [matrix](vector-space.md#matrix) size, the remaining rows must be zero. Together with existence by [Gaussian elimination](#gaussian-elimination), this proves uniqueness.

### Elementary row operation

↑ **Parent:** [Gaussian elimination](#gaussian-elimination)

An [elementary row operation](#elementary-row-operation) interchanges two rows of a [matrix](vector-space.md#matrix), multiplies one row by a nonzero scalar, or adds a scalar multiple of another row to it. These invertible operations are used in [Gaussian elimination](#gaussian-elimination). For a square [matrix](vector-space.md#matrix), interchange changes the sign of its [determinant](multilinear-algebra.md#determinant), multiplication scales its [determinant](multilinear-algebra.md#determinant) by the same scalar, and adding another row leaves its [determinant](multilinear-algebra.md#determinant) unchanged, by multilinearity and alternation.

#### Elementary matrix

↑ **Parent:** [Elementary row operation](#elementary-row-operation)

An elementary matrix is obtained by applying one [elementary row operation](#elementary-row-operation) to the [identity matrix](vector-space.md#identity-matrix). Multiplying $A$ by it on the left performs the same row operation on $A$. Such a [matrix](vector-space.md#matrix) is invertible: reverse a row swap, reverse a nonzero row scaling by its reciprocal, or reverse adding a multiple of another row by adding its negative. Right multiplication gives an [elementary column operation](vector-space.md#elementary-column-operation). In particular these operations preserve [matrix rank](vector-space.md#matrix-rank).

## LU decomposition

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/LU_decomposition)

An [LU decomposition](#lu-decomposition) writes a [square matrix](vector-space.md#square-matrix) as $A=LU$, with $L$ a [lower triangular matrix](linear-algebra.md#lower-triangular-matrix) and $U$ an [upper triangular matrix](linear-algebra.md#upper-triangular-matrix). We use a [unit triangular matrix](#unit-triangular-matrix) $L$, meaning $l_{ii}=1$. The factors record [Gaussian elimination](#gaussian-elimination): $U$ contains the reduced equations, while $L$ stores the [elimination multipliers](#elimination-multiplier) needed to reconstruct the original equations. This makes [Reusing LU factors for multiple right-hand sides](#reusing-lu-factors-for-multiple-right-hand-sides) inexpensive.[§2.4.3, Definition 2.4.2 and equation (2.4.7): unit lower triangular L and upper triangular U](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others)

For an [invertible matrix](linear-algebra.md#invertible-matrix), unpivoted [LU decomposition](#lu-decomposition) requires nonzero [pivot elements](#pivot-element) at every elimination step; invertibility alone does not guarantee this. In general use [Pivoted LU decomposition](#pivoted-lu-decomposition), with the explicit convention $PA=LU$ and a [permutation matrix](vector-space.md#permutation-matrix) $P$. Once the factors exist, solving a [linear system](linear-algebra.md#system-of-linear-equations) $Ax=b$ needs [forward substitution](#forward-substitution) followed by [back substitution](linear-algebra.md#back-substitution), rather than forming a [matrix inverse](matrix-inverse.md).

### Computed three-by-three LU decomposition

↑ **Parent:** [LU decomposition](#lu-decomposition)

Here is an original example of [Gaussian elimination](#gaussian-elimination) that can be checked entirely with [integers](integer.md). Start with

$$
A=\begin{pmatrix}2&1&1\\4&5&3\\-2&8&4\end{pmatrix}.
$$

The first [pivot element](#pivot-element) is $2$. The [elimination multipliers](#elimination-multiplier) are $l_{21}=4/2=2$ and $l_{31}=-2/2=-1$. Apply the [elementary row operations](#elementary-row-operation) $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3+R_1$ to obtain

$$
A^{(1)}=\begin{pmatrix}2&1&1\\0&3&1\\0&9&5\end{pmatrix}.
$$

Now the second [pivot element](#pivot-element) is $3$, and $l_{32}=9/3=3$. The [elementary row operation](#elementary-row-operation) $R_3\leftarrow R_3-3R_2$ gives

$$
U=\begin{pmatrix}2&1&1\\0&3&1\\0&0&2\end{pmatrix},\qquad L=\begin{pmatrix}1&0&0\\2&1&0\\-1&3&1\end{pmatrix},\qquad LU=A.
$$

Importantly, $l_{32}$ comes from the current reduced [matrix](vector-space.md#matrix), not the original entry $a_{32}=8$. To reconstruct $A$ from $U$, its second row is twice the first row of $U$ plus the second; its third row is minus the first row of $U$ plus three times the second plus the third. These are exactly the coefficients in the [lower triangular matrix](linear-algebra.md#lower-triangular-matrix) $L$.

<a id="image-gaussian-elimination-turns-a-three-by-three-matrix-into-an-upper-triangular-matrix-while-elimination-multipliers-are-stored-in-a-lower-triangular-matrix"></a>
![](lu-elimination-structure.png)

**[Figure 11](#image-gaussian-elimination-turns-a-three-by-three-matrix-into-an-upper-triangular-matrix-while-elimination-multipliers-are-stored-in-a-lower-triangular-matrix). Gaussian elimination turns a three-by-three matrix into an upper triangular matrix, while elimination multipliers are stored in a lower triangular matrix**.

The unpivoted calculation here illustrates the structure of [LU decomposition](#lu-decomposition); applying [partial pivoting](#columnwise-partial-pivoting) to this particular $A$ would choose a different first row and different factors. Both procedures can represent the same [linear system](linear-algebra.md#system-of-linear-equations) when their [permutation matrices](vector-space.md#permutation-matrix) are handled consistently.

### Unit triangular matrix

↑ **Parent:** [LU decomposition](#lu-decomposition)

A [unit triangular matrix](#unit-triangular-matrix) is a [triangular matrix](linear-algebra.md#triangular-matrix) whose diagonal entries are all one. It is an [invertible matrix](linear-algebra.md#invertible-matrix) with [determinant](multilinear-algebra.md#determinant) one. In the convention used for [LU decomposition](#lu-decomposition), $L$ is a unit [lower triangular matrix](linear-algebra.md#lower-triangular-matrix), so [forward substitution](#forward-substitution) needs no division by its diagonal entries.

### Triangular solves for LU decomposition

↑ **Parent:** [LU decomposition](#lu-decomposition)

Given [Pivoted LU decomposition](#pivoted-lu-decomposition) $PA=LU$, the [linear system](linear-algebra.md#system-of-linear-equations) $Ax=b$ is equivalent to $LUx=Pb$. Introduce the intermediate [vector](vector-space.md#vector) $y=Ux$: first use [forward substitution](#forward-substitution) to solve $Ly=Pb$, then [back substitution](linear-algebra.md#back-substitution) to solve $Ux=y$. With unpivoted [LU decomposition](#lu-decomposition), $P=I$ is the [identity matrix](vector-space.md#identity-matrix), so the first right-hand side is simply $b$.[§2.4.4, equation (2.4.8) and Algorithm 2.4.2, and §2.6.3: two triangular solves and permutation of b](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others)

For the factors in [Computed three-by-three LU decomposition](#computed-three-by-three-lu-decomposition) and $b=(7,23,26)^T$, [forward substitution](#forward-substitution) gives

$$
y_1=7,\qquad y_2=23-2(7)=9,\qquad y_3=26+7-3(9)=6.
$$

Then [back substitution](linear-algebra.md#back-substitution) gives

$$
x_3=6/2=3,\qquad x_2=(9-3)/3=2,\qquad x_1=(7-2-3)/2=1.
$$

Direct [matrix multiplication](vector-space.md#matrix-multiplication) verifies $A(1,2,3)^T=(7,23,26)^T$. More generally, the [back substitution](linear-algebra.md#back-substitution) recurrence is

$$
x_i=\frac{y_i-\sum_{j=i+1}^{n}u_{ij}x_j}{u_{ii}},\qquad i=n,n-1,\ldots,1.
$$

The direction matters: the last row contains only $x_n$, whereas the first row generally involves every unknown. No dense [matrix inverse](matrix-inverse.md) is needed for either triangular solve.

#### Forward substitution

↑ **Parent:** [Triangular solves for LU decomposition](#triangular-solves-for-lu-decomposition)

[Forward substitution](#forward-substitution) solves a [linear system](linear-algebra.md#system-of-linear-equations) $Ly=c$ with a [lower triangular matrix](linear-algebra.md#lower-triangular-matrix) $L$ and nonzero diagonal, from the first row downward:

$$
y_i=\frac{c_i-\sum_{j=1}^{i-1}l_{ij}y_j}{l_{ii}},\qquad i=1,\ldots,n.
$$

The first [sum](arithmetic.md#sum) is empty, so $y_1=c_1/l_{11}$. Each subsequent row uses only components already found. For a [unit triangular matrix](#unit-triangular-matrix) $L$, omit the division because $l_{ii}=1$. The complementary procedure, [back substitution](linear-algebra.md#back-substitution), solves an [upper triangular matrix](linear-algebra.md#upper-triangular-matrix) system from the last row upward.[§2.3.2, equations (2.3.7)–(2.3.9), and §2.3.3, Algorithms 2.3.1–2.3.2: forward and backward substitution](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others)

### Pivoted LU decomposition

↑ **Parent:** [LU decomposition](#lu-decomposition)

We fix the convention $PA=LU$: the [permutation matrix](vector-space.md#permutation-matrix) $P$ acts on the rows of $A$, and the same row ordering must be applied to $b$ before the [Triangular solves for LU decomposition](#triangular-solves-for-lu-decomposition). Equivalently, $A=P^TLU$, since $P^{-1}=P^T$. LAPACK documents its factors as $A=PLU$ instead, so check the defining equation rather than just the letter $P$.[LAPACK DGETRS, A argument: factors from DGETRF satisfy $A=PLU$](mathematics-bibliography.md#dgetrs-lapack-3-3-1-by-lapack-project) [Partial pivoting](#columnwise-partial-pivoting) selects the largest absolute candidate in the current column, among rows $k,\ldots,n$, before forming [elimination multipliers](#elimination-multiplier).[§2.6.1, Definition 2.6.1; §2.6.2, Definition 2.6.2 and equation (2.6.1): pivot selection and reordered-row factorization](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others)

A zero first [pivot element](#pivot-element) does not imply a [singular matrix](linear-algebra.md#singular-matrix). For example,

$$
A_0=\begin{pmatrix}0&1\\2&3\end{pmatrix},\qquad \det A_0=-2,\qquad P=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad PA_0=\underbrace{\begin{pmatrix}1&0\\0&1\end{pmatrix}}_{L}\underbrace{\begin{pmatrix}2&3\\0&1\end{pmatrix}}_{U}.
$$

Unpivoted [Gaussian elimination](#gaussian-elimination) would divide $2$ by zero. Indeed, no $A_0=LU$ with a unit [lower triangular matrix](linear-algebra.md#lower-triangular-matrix) $L$ exists: $u_{11}=0$ would force $(LU)_{21}=l_{21}u_{11}=0$, contradicting $(A_0)_{21}=2$. One row interchange resolves the obstruction. For $b_0=(1,5)^T$, use $Pb_0=(5,1)^T$; [back substitution](linear-algebra.md#back-substitution) then gives $x=(1,1)^T$. Using the original $b_0$ with these factors would solve a different [linear system](linear-algebra.md#system-of-linear-equations).

[Partial pivoting](#columnwise-partial-pivoting) bounds each [elimination multiplier](#elimination-multiplier) by one in absolute value in exact arithmetic. This helps control [roundoff error](numerical-analysis.md#round-off-error), but intermediate entries can still grow; it is not an unconditional guarantee of [numerical stability](numerical-analysis.md#stability-of-a-numerical-method) for every [matrix](vector-space.md#matrix).[§2.6.4, Example 2.6.6 and the concluding discussion: stability of unpivoted and pivoted factorization](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others) It also does not remove the original problem's [condition number](quadratic-form.md#condition-number). For the [diagonal matrix](linear-algebra.md#diagonal-matrix) $D=\operatorname{diag}(1,\varepsilon)$ with $0<\varepsilon<1$, the [condition number](quadratic-form.md#condition-number) in the [Euclidean norm](normed-vector-space.md#euclidean-norm) is $\kappa_2(D)=1/\varepsilon$. Row permutations preserve this [condition number](quadratic-form.md#condition-number), because they preserve [Euclidean norms](normed-vector-space.md#euclidean-norm). Even an exact solve changes from $(1,1)^T$ to $(1,1+\eta/\varepsilon)^T$ when the right-hand side changes from $(1,\varepsilon)^T$ to $(1,\varepsilon+\eta)^T$. This sensitivity is a property of the [linear system](linear-algebra.md#system-of-linear-equations), not a zero-[pivot element](#pivot-element) failure.[§2.8, Definition 2.8.1, and §2.8.1, Theorem 2.8.1, equations (2.8.5)–(2.8.6): condition number and right-hand-side sensitivity](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others)

### Reusing LU factors for multiple right-hand sides

↑ **Parent:** [LU decomposition](#lu-decomposition)

When a fixed [matrix](vector-space.md#matrix) $A$ is used with several forcing or measurement [vectors](vector-space.md#vector), compute its [Pivoted LU decomposition](#pivoted-lu-decomposition) once. Collect $r$ right-hand sides into the columns of $B=(b^{(1)}\ \cdots\ b^{(r)})$, and the corresponding solutions into $X$. Then

$$
AX=B,\qquad LY=PB,\qquad UX=Y.
$$

Each column undergoes the same row permutation, [forward substitution](#forward-substitution) and [back substitution](linear-algebra.md#back-substitution). Neither $L$, $U$ nor $P$ depends on $B$. This is the useful separation between preparing a [linear system](linear-algebra.md#system-of-linear-equations) and applying its solution procedure repeatedly. LAPACK implements it by taking previously computed factors, permuting all right-hand sides, and performing the two triangular solves.[LAPACK DGETRS, version 3.3.1, April 2011, Purpose, NRHS and B arguments, and nontransposed branch: DLASWP followed by lower-unit and upper-nonunit DTRSM calls](mathematics-bibliography.md#dgetrs-lapack-3-3-1-by-lapack-project)

For the unpivoted factors in [Computed three-by-three LU decomposition](#computed-three-by-three-lu-decomposition), take

$$
B=\begin{pmatrix}7&0&4\\23&2&6\\26&4&-8\end{pmatrix},\qquad Y=\begin{pmatrix}7&0&4\\9&2&-2\\6&-2&2\end{pmatrix},\qquad X=\begin{pmatrix}1&0&2\\2&1&-1\\3&-1&1\end{pmatrix}.
$$

Direct [matrix multiplication](vector-space.md#matrix-multiplication) checks all three identities $LY=B$, $UX=Y$ and $AX=B$. The first column reproduces the previous solve; the other two use exactly the same factors. New right-hand sides can also arrive one at a time. If $A$ changes, these stored factors generally need to be recomputed.

<a id="image-one-row-permutation-fixes-a-zero-pivot-element-each-new-right-hand-side-reuses-the-same-lu-decomposition-and-two-triangular-solves"></a>
![](lu-pivot-repeated-solves.png)

**[Figure 12](#image-one-row-permutation-fixes-a-zero-pivot-element-each-new-right-hand-side-reuses-the-same-lu-decomposition-and-two-triangular-solves). One row permutation fixes a zero pivot element; each new right-hand side reuses the same LU decomposition and two triangular solves**.

### LU factorization and solve costs

↑ **Parent:** [LU decomposition](#lu-decomposition)

For classical dense [Gaussian elimination](#gaussian-elimination) over the [real numbers](arithmetic.md#real-number), count each scalar [addition](arithmetic.md#addition), [subtraction](arithmetic.md#subtraction), [multiplication](arithmetic.md#multiplication) or [division](arithmetic.md#division-mathematics) as one [arithmetic operation](numerical-analysis.md#arithmetic-operation). At step $k$, there are $n-k$ [elimination multipliers](#elimination-multiplier) to divide out and $(n-k)^2$ remaining entries, each requiring one [multiplication](arithmetic.md#multiplication) and one [subtraction](arithmetic.md#subtraction). Thus this implementation's unpivoted factorization count is

$$
F(n)=\sum_{k=1}^{n-1}\bigl((n-k)+2(n-k)^2\bigr)=\frac{n(n-1)(4n+1)}6=\frac23n^3+O(n^2).
$$

Here $O$ uses [Big O notation](real-analysis.md#big-o-notation). [Partial pivoting](#columnwise-partial-pivoting) adds $O(n^2)$ comparisons and row movement, leaving the leading arithmetic count unchanged. The leading $\tfrac23n^3$ count agrees with the standard dense [LU decomposition](#lu-decomposition) analysis.[§2.5.2, Definition 2.5.2; §2.5, equations (2.5.7)–(2.5.8) and Theorem 2.5.1; lower-order counts depend on implementation](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others)

With unit $L$, [forward substitution](#forward-substitution) uses $n(n-1)$ [arithmetic operations](numerical-analysis.md#arithmetic-operation). [Back substitution](linear-algebra.md#back-substitution) uses another $n(n-1)$ plus $n$ diagonal divisions. Together these cost $2n^2-n$ per right-hand side; applying a stored row permutation moves $n$ entries and requires no scalar arithmetic. In [Big O notation](real-analysis.md#big-o-notation), [Reusing LU factors for multiple right-hand sides](#reusing-lu-factors-for-multiple-right-hand-sides) therefore costs

$$
\frac23n^3+2rn^2+O(n^2+rn),
$$

whereas refactorizing for each of the $r$ right-hand sides costs $\tfrac23rn^3+O(rn^2)$. For $n=1000$ and $r=10$, the leading counts are about $6.87\times10^8$ versus $6.69\times10^9$ [arithmetic operations](numerical-analysis.md#arithmetic-operation), nearly a tenfold saving. These are operation counts, not measured runtimes: memory access and optimized [matrix multiplication](vector-space.md#matrix-multiplication) also affect speed.[§2.5.2, Important note after Definition 2.5.2: flop counts are a rough runtime model; the numerical comparison here is an original calculation](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others)

## LDL decomposition

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra.md)

An LDL decomposition of a real symmetric matrix is

$$
A=LDL^T,
$$

where $L$ is unit lower triangular and $D$ is diagonal. Symmetric elimination computes it one [Schur complement](linear-algebra.md#schur-complement) at a time. The matrix is positive definite exactly when every diagonal pivot in $D$ is positive.

## Eigenpair residual

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra.md)

For an approximate eigenpair $(\widetilde\lambda,\widetilde v)$, the residual is

$$
r=A\widetilde v-\widetilde\lambda\widetilde v.
$$

### Backward error of an approximate eigenpair

↑ **Parent:** [Eigenpair residual](#eigenpair-residual)

If $\|\widetilde v\|_2=1$, the smallest operator-norm perturbation that makes $(\widetilde\lambda,\widetilde v)$ an exact eigenpair has norm $\|r\|_2$. One such rank-one perturbation is

$$
E=-r\widetilde v^T.
$$

## Householder QR decomposition

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Householder_QR_decomposition)

Successive Householder reflections zero subdiagonal column entries and factor a matrix into an orthogonal factor and an upper-triangular factor.

### Householder reduction of an overdetermined consistent system

↑ **Parent:** [Householder QR decomposition](#householder-qr-decomposition)

For full column rank $A\in\mathbb R^{m\times n}$, a full [QR factorization](inner-product.md#qr-decomposition) gives $Q^TA=(R_1,0)^T$ with invertible upper triangular $R_1$. The equation $Ax=b$ is consistent exactly when the final $m-n$ entries of $Q^Tb$ vanish. If consistent, [back substitution](linear-algebra.md#back-substitution) gives its unique solution. This separates consistency from uniqueness in overdetermined systems.

## Householder tridiagonalization

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Householder_tridiagonalization)

Orthogonal Householder similarities reduce a real symmetric matrix to symmetric tridiagonal form.

### Skew-symmetric Householder tridiagonalization

↑ **Parent:** [Householder tridiagonalization](#householder-tridiagonalization)

An [orthogonal](inner-product.md#orthogonal-vectors) similarity preserves skew symmetry, so upper-Hessenberg reduction of a real [skew-symmetric matrix](linear-algebra.md#skew-symmetric-matrix) is automatically tridiagonal with zero diagonal. For a [Householder reflection](linear-algebra.md#householder-transformation), the scalar $v^TAv$ vanishes, eliminating the fourth term of the general similarity update. Storing only one triangle and using the displayed skew rank-two update costs $2n^3/3+O(n^2)$ scalar products, the same leading product count as optimized symmetric tridiagonalization; the simplification saves lower-order work.

## Unshifted QR algorithm

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra.md)

The unshifted QR algorithm factors $A_k=Q_kR_k$ and forms $A_{k+1}=R_kQ_k=Q_k^TA_kQ_k$, preserving eigenvalues while driving the matrix toward block diagonal form.

This is the zero-shift case of the [QR algorithm](numerical-analysis.md#qr-algorithm).

### Accumulated QR factorization identity

↑ **Parent:** [Unshifted QR algorithm](#unshifted-qr-algorithm)

Let

$$
\overline Q_k=Q_0Q_1\cdots Q_k,
\qquad
\overline R_k=R_kR_{k-1}\cdots R_0.
$$

Then

$$
A_{k+1}=\overline Q_k^TA\overline Q_k,
\qquad
A^{k+1}=\overline Q_k\overline R_k.
$$

Thus $\overline Q_k\overline R_k$ is a [QR decomposition](inner-product.md#qr-decomposition) of the matrix power $A^{k+1}$. In particular, the first $r$ columns of $\overline Q_k$ span the same subspace as the first $r$ columns of $A^{k+1}$ whenever those columns are independent.

### Symmetric bandwidth preservation under QR iteration

↑ **Parent:** [Unshifted QR algorithm](#unshifted-qr-algorithm)

An unshifted QR step preserves the bandwidth of a real symmetric banded matrix. A Givens-rotation implementation exposes this as bulges created during triangularization and removed when the factors are multiplied in reverse order.

### Simultaneous iteration interpretation of the QR algorithm

↑ **Parent:** [Unshifted QR algorithm](#unshifted-qr-algorithm)

The accumulated orthogonal factor in QR iteration is the $Q$ factor of a matrix power, so its leading columns span the same spaces as simultaneous power iteration.

#### Two-column dominant-subspace condition

↑ **Parent:** [Simultaneous iteration interpretation of the QR algorithm](#simultaneous-iteration-interpretation-of-the-qr-algorithm)

Let a real [symmetric matrix](linear-algebra.md#symmetric-matrix) have an [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) $w_1,\ldots,w_n$, with

$$
|\lambda_1|\leq\cdots\leq|\lambda_{n-2}|<
|\lambda_{n-1}|=|\lambda_n|.
$$

Write two starting vectors as

$$
u=\sum_i b_iw_i,
\qquad
v=\sum_i c_iw_i.
$$

For two-column [subspace iteration](linear-operator-theory.md#subspace-iteration) to recover  
$\operatorname{span}(w_{n-1},w_n)$, the two projections onto that dominant subspace must be independent. The exact condition is

$$
\det\begin{pmatrix}
b_{n-1}&c_{n-1}\\
b_n&c_n
\end{pmatrix}
=b_{n-1}c_n-b_nc_{n-1}\ne0.
$$

Requiring each of the four coefficients to be nonzero does not imply this determinant condition.

### Block deflation in the QR algorithm

↑ **Parent:** [Unshifted QR algorithm](#unshifted-qr-algorithm)

When an off-block subdiagonal entry tends to zero, QR iteration asymptotically separates the corresponding invariant spectral blocks even if eigenvalues within one block have equal modulus.

## Stationary iterative method for a linear system

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra.md)

A stationary iteration has the form

$$
x^{(k+1)}=Hx^{(k)}+v,
$$

with a fixed iteration matrix $H$. It converges for every initial vector exactly when the [spectral radius](analysis.md#spectral-radius) satisfies $\rho(H)<1$.

This is an [iterative method](numerical-analysis.md#iterative-method) whose update matrix remains fixed.

### Semiconvergence of cyclic Poisson iterations

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)

The periodic second-difference [circulant matrix](linear-algebra.md#circulant-matrix) has constant [null space](kernel-of-a-linear-map.md), so solvability requires $\sum b_j=0$. Its [Jacobi method](#jacobi-method) has eigenvalues $\cos(2\pi j/n)$: for odd $n$ it converges to some solution, while for even $n$ an alternating mode oscillates unless absent from the error. Lexicographic [Gauss-Seidel iteration](#gauss-seidel-method) converges to some solution for every compatible right-hand side and every initial vector. For $K=-A=D+L+U$, a coordinate sweep decreases the energy $e^TKe/2$ by the sum of squared coordinate changes. This excludes all nonconstant unit-modulus eigenmodes. The constant unit eigenvalue is simple, since the invariant left vector $w=(0,1,\ldots,1,2)^T$ has $w^T\mathbf1=n\ne0$. Neither method is a strict contraction to a unique solution without fixing the constant nullspace.

### Richardson iteration

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)

For a real symmetric positive definite [matrix](vector-space.md#matrix) $A$, the error in each [eigenvector](linear-operator-theory.md#eigenvector) direction is multiplied by $1-\tau\lambda$. Convergence from every initial vector is therefore equivalent to $0<\tau<2/\lambda_{\max}$. At either endpoint there is a nondecaying error direction. The optimal constant parameter is $2/(\lambda_{\min}+\lambda_{\max})$, giving contraction factor $(\lambda_{\max}-\lambda_{\min})/(\lambda_{\max}+\lambda_{\min})$.

### Gauss-Seidel method

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss–Seidel_method)

With $A=D+L+U$, the [Gauss-Seidel method](#gauss-seidel-method) solves $(D+L)x^{(k+1)}=b-Ux^{(k)}$. It uses each newly computed coordinate immediately in the remaining [triangular solve](linear-algebra.md#triangular-solve). It is [successive over-relaxation](#successive-over-relaxation) with parameter one, and converges from every start when $A$ is a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix).

To solve a [linear system](linear-algebra.md#system-of-linear-equations) $Ax=b$, split its [matrix](vector-space.md#matrix) into the [diagonal matrix](linear-algebra.md#diagonal-matrix) $D$ and the strictly lower and upper parts $L,U$, retaining their actual signs. Every diagonal entry must be nonzero. A sweep updates coordinates in order:

$$
x_i^{(k+1)}=\frac{b_i-\sum_{j<i}a_{ij}x_j^{(k+1)}-\sum_{j>i}a_{ij}x_j^{(k)}}{a_{ii}}.
$$

The [Jacobi method](#jacobi-method) uses the old [vector](vector-space.md#vector) throughout; the [Gauss-Seidel method](#gauss-seidel-method) reuses each fresh coordinate. Thus the update order is part of the method.[Math 221, Matrix Computations, Fall 2009; Gauss-Seidel: component loop, splitting and update-order remark, web lines 372–380](mathematics-bibliography.md#math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009)

The [matrix splitting](#matrix-splitting) has $M=D+L$, $N=-U$, so its [iteration matrix](#iteration-matrix) is

$$
H=-(D+L)^{-1}U,\qquad x^{(k+1)}=Hx^{(k)}+(D+L)^{-1}b.
$$

Compute the update by [forward substitution](#forward-substitution) with the [lower triangular matrix](linear-algebra.md#lower-triangular-matrix) $D+L$, rather than forming a [matrix inverse](matrix-inverse.md). For a [sparse matrix](vector-space.md#sparse-matrix), a sweep only visits stored entries and can overwrite the working [vector](vector-space.md#vector). Dependencies on fresh coordinates constrain parallel execution. This makes the [Gauss-Seidel method](#gauss-seidel-method) an inexpensive solver component, including in a [multigrid method](multigrid-method.md).[Math 221, Matrix Computations, Fall 2009; Basic iterative methods, cheap splitting requirement; Gauss-Seidel loop and red-black ordering; opening list of solver building blocks](mathematics-bibliography.md#math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009)

#### Gauss-Seidel iteration for a two-variable positive-definite system

↑ **Parent:** [Gauss-Seidel method](#gauss-seidel-method)

Consider the original [linear system](linear-algebra.md#system-of-linear-equations)

$$
A\begin{pmatrix}x\\y\end{pmatrix}=b,\qquad A=\begin{pmatrix}4&1\\1&3\end{pmatrix},\qquad b=\begin{pmatrix}1\\2\end{pmatrix},\qquad \begin{pmatrix}x_*\\y_*\end{pmatrix}=\begin{pmatrix}1/11\\7/11\end{pmatrix}.
$$

Direct substitution verifies the solution. The [matrix](vector-space.md#matrix) is a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix): [completing the square](polynomial.md#completing-the-square) in its [quadratic form](quadratic-form.md) gives $4x^2+2xy+3y^2=4(x+y/4)^2+11y^2/4>0$ for every nonzero [vector](vector-space.md#vector). It is also a [strictly diagonally dominant matrix](vector-space.md#strictly-diagonally-dominant-matrix).

Starting from $(x^{(0)},y^{(0)})=(0,0)$, update the first row and then the second:

$$
x^{(k+1)}=\frac{1-y^{(k)}}4,\qquad y^{(k+1)}=\frac{2-x^{(k+1)}}3.
$$

The first sweep gives $x^{(1)}=1/4$ and $y^{(1)}=(2-1/4)/3=7/12$. The next gives $x^{(2)}=(1-7/12)/4=5/48$ and $y^{(2)}=(2-5/48)/3=91/144$. The second row uses $1/4$ during the first sweep, even though the initial first coordinate was zero.

<a id="image-fresh-and-stale-inputs-in-the-first-sweep-of-the-original-two-variable-linear-system"></a>
![](gauss-seidel-two-row-fresh-updates.png)

**[Figure 13](#image-fresh-and-stale-inputs-in-the-first-sweep-of-the-original-two-variable-linear-system). Fresh and stale inputs in the first sweep of the original two-variable linear system**.

With a stale first coordinate, the [Jacobi method](#jacobi-method) would instead give $(1/4,2/3)$ after the first sweep. Both methods have the same [fixed point](function.md#fixed-point), but changing when coordinates become available changes the entire sequence of [vectors](vector-space.md#vector).

##### Exact error contraction of a two-variable Gauss-Seidel iteration

↑ **Parent:** [Gauss-Seidel iteration for a two-variable positive-definite system](#gauss-seidel-iteration-for-a-two-variable-positive-definite-system)

For the [Gauss-Seidel iteration for a two-variable positive-definite system](#gauss-seidel-iteration-for-a-two-variable-positive-definite-system), define the [forward error](numerical-analysis.md#forward-error) by $e_x^{(k)}=x^{(k)}-x_*$ and $e_y^{(k)}=y^{(k)}-y_*$. Subtract the two exact solution equations from the two update equations:

$$
e_x^{(k+1)}=-\frac14e_y^{(k)},\qquad e_y^{(k+1)}=-\frac13e_x^{(k+1)}=\frac1{12}e_y^{(k)}.
$$

The fresh first coordinate passes the old second-coordinate error through two successive factors. The [iteration matrix](#iteration-matrix) is therefore

$$
H=\begin{pmatrix}0&-1/4\\0&1/12\end{pmatrix},\qquad \det(tI-H)=t(t-1/12),\qquad \rho(H)=1/12.
$$

Its [eigenvalues](linear-operator-theory.md#eigenvalue) are $0$ and $1/12$, as seen from the [determinant](multilinear-algebra.md#determinant). The zero [eigenvalue](linear-operator-theory.md#eigenvalue) explains why the old first-coordinate error disappears completely: the first row overwrites it. After one sweep, every remaining [forward error](numerical-analysis.md#forward-error) lies on the [eigenvector](linear-operator-theory.md#eigenvector) line spanned by $(-3,1)^T$.

For this zero start, $e_y^{(0)}=-7/11$, so the exact [vectors](vector-space.md#vector) for $k\geq1$ are

$$
\begin{pmatrix}x^{(k)}\\y^{(k)}\end{pmatrix}=\begin{pmatrix}1/11\\7/11\end{pmatrix}+\frac{7}{11\,12^k}\begin{pmatrix}3\\-1\end{pmatrix},\qquad \|e^{(k)}\|_2=\frac{7\sqrt{10}}{11\,12^k}.
$$

The [Euclidean norm](normed-vector-space.md#euclidean-norm) of the [forward error](numerical-analysis.md#forward-error) decreases by exactly $1/12$ per sweep from $k=1$ onward. The first decrease is different because the initial error has not yet reached that [eigenvector](linear-operator-theory.md#eigenvector) line. Each row update moves horizontally or vertically in the coordinate plane; sweep endpoints then approach the solution along one straight line.

<a id="image-computed-row-by-row-gauss-seidel-method-trajectory-and-exact-forward-error-contraction-for-the-original-two-variable-linear-system"></a>
![](gauss-seidel-two-variable-trajectory-contraction.png)

**[Figure 14](#image-computed-row-by-row-gauss-seidel-method-trajectory-and-exact-forward-error-contraction-for-the-original-two-variable-linear-system). Computed row-by-row Gauss-Seidel method trajectory and exact forward error contraction for the original two-variable linear system**.

The [linear-system residual](gradient-descent.md#linear-system-residual) is an independent way to check the calculation. Completing a sweep satisfies the second row exactly, but changing $y$ disturbs the first row:

$$
r^{(k)}=b-A\begin{pmatrix}x^{(k)}\\y^{(k)}\end{pmatrix}=\begin{pmatrix}y^{(k-1)}-y^{(k)}\\0\end{pmatrix}=\begin{pmatrix}-7/12^k\\0\end{pmatrix}\qquad(k\geq1).
$$

Thus a zero residual in the last updated row alone does not certify a solution; inspect the complete [linear-system residual](gradient-descent.md#linear-system-residual).

For the same [matrix](vector-space.md#matrix), the stale schedule of the [Jacobi method](#jacobi-method) gives the [iteration matrix](#iteration-matrix)

$$
B=\begin{pmatrix}0&-1/4\\-1/3&0\end{pmatrix},\qquad B^2=\frac1{12}I,\qquad \rho(B)=\frac1{\sqrt{12}}.
$$

Here its [eigenvalues](linear-operator-theory.md#eigenvalue) are $\pm1/\sqrt{12}$, whereas the fresh schedule gives $\rho(H)=\rho(B)^2$. This comparison belongs to this particular [linear system](linear-algebra.md#system-of-linear-equations); it is not a universal relation between the two methods' [spectral radii](analysis.md#spectral-radius).

#### Gauss-Seidel convergence from diagonal dominance and positive definiteness

↑ **Parent:** [Gauss-Seidel method](#gauss-seidel-method)

A [strictly diagonally dominant matrix](vector-space.md#strictly-diagonally-dominant-matrix) or a real [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) guarantees convergence of the [Gauss-Seidel method](#gauss-seidel-method) from every initial [vector](vector-space.md#vector). These are sufficient conditions.[Math 221, Matrix Computations, Fall 2009; Theorem 1, strict row diagonal dominance, web lines 462–465; Theorem 3, positive-definite SOR and its ω = 1 specialization, web lines 490–493](mathematics-bibliography.md#math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009)

For [strict diagonal dominance](vector-space.md#strictly-diagonally-dominant-matrix), put

$$
q=\max_i\frac{\sum_{j\ne i}|a_{ij}|}{|a_{ii}|}<1,\qquad E=\|e^{(k)}\|_\infty.
$$

Induct through a sweep. Old coordinates have absolute error at most $E$; previously updated coordinates have absolute error at most $qE\leq E$. The component update and the [triangle inequality](topological-analysis.md#triangle-inequality) therefore bound the new error by $qE$. This proves $\|e^{(k+1)}\|_\infty\leq q\|e^{(k)}\|_\infty$, a [maximum norm](normed-vector-space.md#supremum-norm) contraction.

For a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix), write $A=D+L+L^T$. The [Householder-John theorem](#householder-john-theorem) applies to $M=D+L$ and $N=-L^T$, because $M^T+N=D$ is a [positive-definite matrix](quadratic-form.md#positive-definite-matrix). Hence the [iteration matrix](#iteration-matrix) has [spectral radius](analysis.md#spectral-radius) less than one, which gives the [convergence criterion for a stationary iteration](#convergence-criterion-for-a-stationary-iteration).

There is also a geometric reason fresh updates help: the [Gauss-Seidel method](#gauss-seidel-method) is exact [coordinate descent](convex-optimization.md#coordinate-descent) on the [convex quadratic function](real-analysis.md#convex-quadratic-function)

$$
F(z)=\frac12z^TAz-b^Tz,\qquad F(z)-F(x_*)=\frac12(z-x_*)^TA(z-x_*).
$$

Holding the other coordinates fixed, minimizing in coordinate $i$ gives the corresponding row update. A change $\delta_i$ lowers $F$ by exactly $a_{ii}\delta_i^2/2$. Each fresh coordinate is therefore the minimizer for the current [vector](vector-space.md#vector), and a complete sweep lowers the [quadratic form](quadratic-form.md) error unless every coordinate already solves its row. This explains the method's beauty without implying monotone decrease in every [vector norm](normed-vector-space.md#norm).

##### Gauss-Seidel iteration can diverge for an invertible matrix

↑ **Parent:** [Gauss-Seidel convergence from diagonal dominance and positive definiteness](#gauss-seidel-convergence-from-diagonal-dominance-and-positive-definiteness)

An [invertible matrix](linear-algebra.md#invertible-matrix) and nonzero diagonal entries make the update well defined, but do not guarantee convergence. For the original [linear system](linear-algebra.md#system-of-linear-equations)

$$
A=\begin{pmatrix}1&2\\2&1\end{pmatrix},\qquad b=\begin{pmatrix}1\\1\end{pmatrix},\qquad x_*=\begin{pmatrix}1/3\\1/3\end{pmatrix},\qquad \det A=-3,
$$

the [Gauss-Seidel method](#gauss-seidel-method) updates $x^{(k+1)}=1-2y^{(k)}$ and $y^{(k+1)}=1-2x^{(k+1)}=-1+4y^{(k)}$. Starting at zero gives $(1,-1)$, then $(3,-5)$. The second-coordinate [forward error](numerical-analysis.md#forward-error) is $e_y^{(k)}=-4^k/3$, and the [iteration matrix](#iteration-matrix) $H=\begin{pmatrix}0&-2\\0&4\end{pmatrix}$ has [spectral radius](analysis.md#spectral-radius) $4$. The [linear system](linear-algebra.md#system-of-linear-equations) has a unique solution while this particular [stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system) diverges.

### Successive over-relaxation

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Successive_over-relaxation)

For a splitting $A=D+L+U$, [successive over-relaxation](#successive-over-relaxation) updates

$$
(D+\omega L)x^{(k+1)}=[(1-\omega)D-\omega U]x^{(k)}+\omega b.
$$

It reduces to the [Gauss-Seidel method](#gauss-seidel-method) at $\omega=1$. If $A$ is symmetric positive definite, the [Householder-John theorem](#householder-john-theorem) applies to $M=D/\omega+L$, $N=(1/\omega-1)D-U$, since $M^T+N=(2/\omega-1)D$ is positive definite for $0<\omega<2$.

### Iteration matrix

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)

For a stationary iteration $x^{(k+1)}=Hx^{(k)}+v$, the matrix $H$ propagates the error by $e^{(k+1)}=He^{(k)}$. Convergence from every initial error is equivalent to $\rho(H)<1$.

For a [matrix splitting](#matrix-splitting) $A=M-N$, the [iteration matrix](#iteration-matrix) is $H=M^{-1}N=I-M^{-1}A$, where $I$ is the [identity matrix](vector-space.md#identity-matrix). If $Ax_*=b$, subtracting its [fixed point](function.md#fixed-point) equation from the update gives

$$
e^{(k)}=x^{(k)}-x_*,\qquad e^{(k+1)}=He^{(k)},\qquad e^{(k)}=H^ke^{(0)}.
$$

Thus $b$ determines the [fixed point](function.md#fixed-point), while $H$ determines how the [forward error](numerical-analysis.md#forward-error) moves. An [eigenvector](linear-operator-theory.md#eigenvector) $v$ with [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda$ is an error direction whose coefficient is multiplied by $\lambda$ on every step. A negative real [eigenvalue](linear-operator-theory.md#eigenvalue) reverses its sign; a zero [eigenvalue](linear-operator-theory.md#eigenvalue) removes that component in one step.

#### Convergence criterion for a stationary iteration

↑ **Parent:** [Iteration matrix](#iteration-matrix)

A [stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system) converges to its specified [fixed point](function.md#fixed-point) for every initial [vector](vector-space.md#vector) if and only if its [iteration matrix](#iteration-matrix) satisfies $\rho(H)<1$, where the [spectral radius](analysis.md#spectral-radius) is the largest [modulus](complex-analysis.md#modulus) of an [eigenvalue](linear-operator-theory.md#eigenvalue).[Math 221, Matrix Computations, Fall 2009; Basic iterative methods: theorem following the spectral-radius lemmas, before the Jacobi update](mathematics-bibliography.md#math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009)

For a [diagonalizable matrix](linear-operator-theory.md#diagonalizable-matrix), write $H=V\Lambda V^{-1}$. Then $H^k=V\Lambda^kV^{-1}$, so each [eigenvector](linear-operator-theory.md#eigenvector) coefficient tends to zero exactly when its [eigenvalue](linear-operator-theory.md#eigenvalue) has [modulus](complex-analysis.md#modulus) less than one. For a general [matrix](vector-space.md#matrix), the [Jordan normal form](linear-operator-theory.md#jordan-normal-form) gives the same result: a [Jordan block](linear-operator-theory.md#jordan-block) $J=\lambda I+K$ with a [nilpotent matrix](linear-operator-theory.md#nilpotent-matrix) $K$ of size $m$ satisfies

$$
J^k=\sum_{j=0}^{\min(k,m-1)}\binom{k}{j}\lambda^{k-j}K^j.
$$

If $0<|\lambda|<1$, every coefficient tends to zero because [exponential decay](analysis.md#exponential-decay) beats any fixed [polynomial](polynomial.md) in $k$; if $\lambda=0$, the block vanishes once $k\geq m$. Conversely, an [eigenvector](linear-operator-theory.md#eigenvector) with $|\lambda|\geq1$ provides an initial error that cannot tend to zero. For a real [matrix](vector-space.md#matrix) with complex [eigenvalues](linear-operator-theory.md#eigenvalue), the same obstruction appears in the real [invariant subspace](representation-theory.md#invariant-subspace) spanned by the real and imaginary parts of an [eigenvector](linear-operator-theory.md#eigenvector).

The words "every initial [vector](vector-space.md#vector)" matter. For example, $H=\operatorname{diag}(3/2,1/2)$ fails the criterion, but $e^{(0)}=(0,1)^T$ still tends to zero. Here a generic initial error has a nonzero first coordinate and diverges; the exceptional errors lie on the second coordinate axis. With $H=\operatorname{diag}(-1,1/2)$, generic errors oscillate rather than diverge in [norm](normed-vector-space.md#norm), while the same exceptional axis still converges. Both are valid [matrix splittings](#matrix-splitting) with $M=I$ and $A=I-H$. In general the convergent errors form the [direct sum](vector-space.md#direct-sum) of the [generalized eigenspaces](linear-operator-theory.md#generalized-eigenspace) for $|\lambda|<1$; if $\rho(H)\geq1$, this is a proper [linear subspace](vector-space.md#vector-subspace).

A small [spectral radius](analysis.md#spectral-radius) describes eventual convergence, but does not imply that the [Euclidean norm](normed-vector-space.md#euclidean-norm) of the error decreases on every step for a [non-normal matrix](linear-operator-theory.md#non-normal-matrix). An [operator norm](continuous-dual-space.md#operator-norm) bound $\|H\|<1$ does give the stepwise estimate $\|e^{(k)}\|\leq\|H\|^k\|e^{(0)}\|$. For a real [symmetric matrix](linear-algebra.md#symmetric-matrix), the [matrix 2-norm](continuous-dual-space.md#matrix-2-norm) equals its [spectral radius](analysis.md#spectral-radius), making this particularly direct.

#### Residual and forward error in a stationary iteration

↑ **Parent:** [Iteration matrix](#iteration-matrix)

The [linear-system residual](gradient-descent.md#linear-system-residual) $r^{(k)}=b-Ax^{(k)}$ is computable without knowing $x_*$. The [forward error](numerical-analysis.md#forward-error) $e^{(k)}=x^{(k)}-x_*$ is the actual difference from the desired solution. For an [invertible matrix](linear-algebra.md#invertible-matrix),

$$
r^{(k)}=-Ae^{(k)},\qquad e^{(k)}=-A^{-1}r^{(k)}.
$$

Keeping $A$ fixed, the approximate [vector](vector-space.md#vector) exactly solves $Ax^{(k)}=b+\delta b$ with $\delta b=-r^{(k)}$. Thus, for $b\ne0$, $\|r^{(k)}\|/\|b\|$ is the relative [backward error](numerical-analysis.md#backward-error) when only the right-hand side may change. For a [vector norm](normed-vector-space.md#norm) and its induced [operator norm](continuous-dual-space.md#operator-norm),

$$
\frac{\|e^{(k)}\|}{\|x_*\|}\leq\kappa(A)\frac{\|r^{(k)}\|}{\|b\|},\qquad \kappa(A)=\|A\|\,\|A^{-1}\|.
$$

A small relative [linear-system residual](gradient-descent.md#linear-system-residual) ensures a small relative [forward error](numerical-analysis.md#forward-error) when the [condition number](quadratic-form.md#condition-number) is moderate; an ill-conditioned [matrix](vector-space.md#matrix) can amplify it. The bound follows directly from $e=-A^{-1}r$ and $\|b\|=\|Ax_*\|\leq\|A\|\|x_*\|$.[Fundamentals of Numerical Computation by Tobin A. Driscoll and others; §2.8.1, Theorem 2.8.1, equation (2.8.6), right-hand-side perturbation bound applied with Δb = −r](mathematics-bibliography.md#fundamentals-of-numerical-computation-by-tobin-a-driscoll-and-others/2-8-conditioning-of-linear-systems)

For the [Jacobi iteration for a three-variable tridiagonal system](#jacobi-iteration-for-a-three-variable-tridiagonal-system), the first [linear-system residual](gradient-descent.md#linear-system-residual) is $(1,3,1)^T$, while the first [forward error](numerical-analysis.md#forward-error) is $(-1/2,-1,-1/2)^T$. In the [Euclidean norm](normed-vector-space.md#euclidean-norm), the relative [forward error](numerical-analysis.md#forward-error) is $\sqrt{3/28}\approx0.3273$ and the relative [linear-system residual](gradient-descent.md#linear-system-residual) is $\sqrt{11/120}\approx0.3028$. Its [spectral condition number of a positive-definite matrix](quadratic-form.md#spectral-condition-number-of-a-positive-definite-matrix) is $(4+\sqrt2)/(4-\sqrt2)\approx2.094$, so the bound is about $0.6340$. The bound is a guarantee, not an equality. In [floating-point arithmetic](floating-point-arithmetic.md), recompute the [linear-system residual](gradient-descent.md#linear-system-residual) from the current [vector](vector-space.md#vector) when checking termination; a small update alone need not certify a small [forward error](numerical-analysis.md#forward-error).

### Matrix splitting

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_splitting)

A splitting $A=M-N$ with invertible $M$ produces

$$
x^{(k+1)}=M^{-1}Nx^{(k)}+M^{-1}b.
$$

A [matrix splitting](#matrix-splitting) chooses an easy part $M$ of a [matrix](vector-space.md#matrix) and corrects for the remaining part $N$. To solve the [linear system](linear-algebra.md#system-of-linear-equations) $Ax=b$, first rewrite it as $Mx=Nx+b$, then use the old [vector](vector-space.md#vector) on the right and solve for the new [vector](vector-space.md#vector) on the left. The [matrix inverse](matrix-inverse.md) notation describes the update mathematically; each step should solve with $M$ rather than construct its [matrix inverse](matrix-inverse.md).[Math 221, Matrix Computations, Fall 2009; Basic iterative methods: definition A = M − K and recurrence (\*), with the two conditions for a useful splitting](mathematics-bibliography.md#math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009)

The same identity also yields a correction based on the [linear-system residual](gradient-descent.md#linear-system-residual):

$$
x^{(k+1)}=x^{(k)}+M^{-1}(b-Ax^{(k)}),\qquad H=I-M^{-1}A.
$$

This connects a [matrix splitting](#matrix-splitting) to [matrix preconditioning](#matrix-preconditioning): $M^{-1}$ rescales the imbalance before adding a correction. Choosing $M=A$ gives $H=0$ and the exact solution in one step, but requires solving the original [linear system](linear-algebra.md#system-of-linear-equations); choosing $M$ cheaply matters as much as the [convergence criterion for a stationary iteration](#convergence-criterion-for-a-stationary-iteration).

With the sign convention $A=D+L+U$, $D$ is the [diagonal matrix](linear-algebra.md#diagonal-matrix) of diagonal entries and $L,U$ contain the actual lower and upper entries, without reversing their signs. The [Jacobi method](#jacobi-method) uses $M=D$, $N=-(L+U)$; the [Gauss-Seidel method](#gauss-seidel-method) uses $M=D+L$, $N=-U$. The first requires only division by diagonal entries; the second uses a [lower triangular matrix](linear-algebra.md#lower-triangular-matrix) and [forward substitution](#forward-substitution). These choices explain their different information flows.

#### Householder-John theorem

↑ **Parent:** [Matrix splitting](#matrix-splitting)

Let $A=M-N$ be Hermitian positive definite. If $M^*+N$ is also Hermitian positive definite, then $M$ is invertible and

$$
\rho(M^{-1}N)<1.
$$

Thus the stationary iteration associated with the splitting converges from every initial vector.

### Jacobi method

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobi_method)

Writing $A=D+L+U$, where $D$ is diagonal and $L,U$ are strictly triangular, the Jacobi iteration is

$$
x^{(k+1)}=D^{-1}\left(b-(L+U)x^{(k)}\right).
$$

The [Jacobi method](#jacobi-method) solves a [linear system](linear-algebra.md#system-of-linear-equations) by updating every coordinate from the same old [vector](vector-space.md#vector). It requires every diagonal entry $a_{ii}$ to be nonzero. Isolating coordinate $i$ in row $i$ gives the simultaneous rule

$$
x_i^{(k+1)}=\frac{b_i-\sum_{j\ne i}a_{ij}x_j^{(k)}}{a_{ii}},\qquad B=-D^{-1}(L+U)=I-D^{-1}A.
$$

Here $B$ is the [iteration matrix](#iteration-matrix). A sweep computes a complete new [vector](vector-space.md#vector) before replacing the old one, so its coordinate updates can run independently.[Math 221, Matrix Computations, Fall 2009; Jacobi: component loop and splitting immediately before Gauss-Seidel](mathematics-bibliography.md#math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009)

For a [sparse matrix](vector-space.md#sparse-matrix), a sweep needs work proportional to the stored nonzero entries, while [Gaussian elimination](#gaussian-elimination) may create [fill-in](#fill-in). The [Jacobi method](#jacobi-method) is therefore a simple starting point for large [linear systems](linear-algebra.md#system-of-linear-equations), and the [weighted Jacobi method](#weighted-jacobi-method) supplies a useful building block of a [multigrid method](multigrid-method.md). Its beauty is that a local row correction becomes a global [eigenvalue](linear-operator-theory.md#eigenvalue) question: the [convergence criterion for a stationary iteration](#convergence-criterion-for-a-stationary-iteration) is exactly $\rho(B)<1$.

#### Jacobi iteration for a three-variable tridiagonal system

↑ **Parent:** [Jacobi method](#jacobi-method)

Consider the original [linear system](linear-algebra.md#system-of-linear-equations) with a [symmetric matrix](linear-algebra.md#symmetric-matrix) that is also a [tridiagonal matrix](vector-space.md#tridiagonal-matrix):

$$
A=\begin{pmatrix}4&-1&0\\-1&4&-1\\0&-1&4\end{pmatrix},\qquad x_*=\begin{pmatrix}1\\2\\3\end{pmatrix},\qquad b=Ax_*=\begin{pmatrix}2\\4\\10\end{pmatrix}.
$$

Here $D=4I$ and the [Jacobi method](#jacobi-method) reads

$$
x_1^{(k+1)}=\frac{2+x_2^{(k)}}4,\qquad x_2^{(k+1)}=\frac{4+x_1^{(k)}+x_3^{(k)}}4,\qquad x_3^{(k+1)}=\frac{10+x_2^{(k)}}4.
$$

Starting from $x^{(0)}=0$, the first three [vectors](vector-space.md#vector) are

$$
x^{(1)}=\begin{pmatrix}1/2\\1\\5/2\end{pmatrix},\qquad x^{(2)}=\begin{pmatrix}3/4\\7/4\\11/4\end{pmatrix},\qquad x^{(3)}=\begin{pmatrix}15/16\\15/8\\47/16\end{pmatrix}.
$$

Every right-hand side uses superscript $k$, including the middle row, even when a new first coordinate has already been computed.

<a id="image-simultaneous-old-to-new-component-updates-in-the-jacobi-method-compared-with-immediate-reuse-in-the-gauss-seidel-method"></a>
![](jacobi-simultaneous-component-update.png)

**[Figure 15](#image-simultaneous-old-to-new-component-updates-in-the-jacobi-method-compared-with-immediate-reuse-in-the-gauss-seidel-method). Simultaneous old-to-new component updates in the Jacobi method, compared with immediate reuse in the Gauss-Seidel method**.

For comparison, a first [Gauss-Seidel method](#gauss-seidel-method) sweep in coordinate order $1,2,3$ gives

$$
x_1^{(1)}=\frac24=\frac12,\qquad x_2^{(1)}=\frac{4+1/2+0}4=\frac98,\qquad x_3^{(1)}=\frac{10+9/8}4=\frac{89}{32}.
$$

The new first coordinate enters the middle update, and the new second coordinate enters the final update. Accidentally overwriting old coordinates during a [Jacobi method](#jacobi-method) sweep therefore changes the mathematical method.

##### Error modes of a three-variable Jacobi iteration

↑ **Parent:** [Jacobi iteration for a three-variable tridiagonal system](#jacobi-iteration-for-a-three-variable-tridiagonal-system)

For the [Jacobi iteration for a three-variable tridiagonal system](#jacobi-iteration-for-a-three-variable-tridiagonal-system),

$$
B=\frac14\begin{pmatrix}0&1&0\\1&0&1\\0&1&0\end{pmatrix}.
$$

An [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) is

$$
u_+=\frac12\begin{pmatrix}1\\\sqrt2\\1\end{pmatrix},\qquad u_0=\frac1{\sqrt2}\begin{pmatrix}1\\0\\-1\end{pmatrix},\qquad u_-=\frac12\begin{pmatrix}1\\-\sqrt2\\1\end{pmatrix},
$$

with [eigenvalues](linear-operator-theory.md#eigenvalue) $q=\sqrt2/4$, $0$, and $-q$, respectively. These are error modes: their shapes persist under the [iteration matrix](#iteration-matrix), while their coefficients change. Direct multiplication verifies them, or expansion of the [determinant](multilinear-algebra.md#determinant) gives $\det(tI-B)=t(t^2-1/8)$. Thus $\rho(B)=q<1$ and convergence holds for every starting [vector](vector-space.md#vector).

With $x^{(0)}=0$, the initial [forward error](numerical-analysis.md#forward-error) has coefficients

$$
e^{(0)}=-x_*=c_+u_++c_0u_0+c_-u_-,\qquad c_+=-2-\sqrt2,\quad c_0=\sqrt2,\quad c_-=-2+\sqrt2.
$$

For $k\geq1$,

$$
e^{(k)}=c_+q^ku_++c_-(-q)^ku_-,\qquad \|e^{(k)}\|_2=2\sqrt3\,q^k.
$$

The zero mode disappears after one sweep; the negative mode alternates in sign. The [Euclidean norm](normed-vector-space.md#euclidean-norm) drops by exactly $q$ per sweep from $k=1$ onward. The first [norm](normed-vector-space.md#norm) drop is different because $\|e^{(0)}\|_2=\sqrt{14}$ includes the zero mode. A starting error proportional to $u_0$ would disappear entirely in one sweep, faster than the [spectral radius](analysis.md#spectral-radius) predicts for generic errors.

<a id="image-computed-jacobi-method-error-curves-and-eigenvector-modes-for-the-original-three-variable-tridiagonal-matrix"></a>
![](jacobi-tridiagonal-error-modes.png)

**[Figure 16](#image-computed-jacobi-method-error-curves-and-eigenvector-modes-for-the-original-three-variable-tridiagonal-matrix). Computed Jacobi method error curves and eigenvector modes for the original three-variable tridiagonal matrix**.

The curves are computed iterates and exact formulas for this [linear system](linear-algebra.md#system-of-linear-equations). Since $A=4(I-B)$, the same [eigenvectors](linear-operator-theory.md#eigenvector) have [eigenvalues](linear-operator-theory.md#eigenvalue) $4-\sqrt2$, $4$, and $4+\sqrt2$ for $A$. They prove that $A$ is a [positive-definite matrix](quadratic-form.md#positive-definite-matrix), and give the [condition number](quadratic-form.md#condition-number) used in [residual and forward error in a stationary iteration](#residual-and-forward-error-in-a-stationary-iteration).

#### Jacobi convergence from strict diagonal dominance

↑ **Parent:** [Jacobi method](#jacobi-method)

A [strictly diagonally dominant matrix](vector-space.md#strictly-diagonally-dominant-matrix) guarantees convergence of the [Jacobi method](#jacobi-method) for every initial [vector](vector-space.md#vector).[Math 221, Matrix Computations, Fall 2009; Theorem 1 on strict row diagonal dominance and its proof beginning “Split A = D − (D − A)”](mathematics-bibliography.md#math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009)

Indeed, using the [maximum norm](normed-vector-space.md#supremum-norm) $\|v\|_\infty=\max_i|v_i|$, the induced [operator norm](continuous-dual-space.md#operator-norm) is the largest absolute row sum. The [Jacobi method](#jacobi-method) has $b_{ii}=0$ and $b_{ij}=-a_{ij}/a_{ii}$ for $j\ne i$, so

$$
\rho(B)\leq\|B\|_\infty=\max_i\frac{\sum_{j\ne i}|a_{ij}|}{|a_{ii}|}<1,\qquad \|e^{(k)}\|_\infty\leq\|B\|_\infty^k\|e^{(0)}\|_\infty.
$$

This gives a cheap sufficient check without computing any [eigenvalues](linear-operator-theory.md#eigenvalue). For the [Jacobi iteration for a three-variable tridiagonal system](#jacobi-iteration-for-a-three-variable-tridiagonal-system), the absolute row sums of $B$ are $1/4,1/2,1/4$, giving $\|B\|_\infty=1/2$. The true [spectral radius](analysis.md#spectral-radius) $\sqrt2/4$ gives a sharper eventual rate.

Strict [diagonal dominance](algebra.md#diagonal-dominance) is sufficient, not necessary: $A=\begin{pmatrix}1&2\\1/10&1\end{pmatrix}$ violates it in the first row, but its [Jacobi method](#jacobi-method) has [eigenvalues](linear-operator-theory.md#eigenvalue) $\pm1/\sqrt5$ and converges. Conversely, being a [positive-definite matrix](quadratic-form.md#positive-definite-matrix) alone is insufficient: the [Jacobi convergence for a three-by-three equicorrelation matrix](#jacobi-convergence-for-a-three-by-three-equicorrelation-matrix) with $\alpha=3/4$ has positive [eigenvalues](linear-operator-theory.md#eigenvalue) $5/2,1/4,1/4$ for $A$, but [spectral radius](analysis.md#spectral-radius) $3/2$ for its [iteration matrix](#iteration-matrix). The extra [tridiagonal matrix](vector-space.md#tridiagonal-matrix) structure in [Jacobi convergence for a symmetric positive-definite tridiagonal matrix](#jacobi-convergence-for-a-symmetric-positive-definite-tridiagonal-matrix) is therefore substantive.

#### Skew-tridiagonal Jacobi and Gauss-Seidel iterations

↑ **Parent:** [Jacobi method](#jacobi-method)

For $A=\mu^{-1}I+U-U^T$, with $U$ the four-dimensional unit superdiagonal, the [Jacobi method](#jacobi-method) has eigenvalues $2i\mu\cos(j\pi/5)$, $j=1,\ldots,4$. The [Gauss-Seidel method](#gauss-seidel-method) has two zero eigenvalues and $-\mu^2(3\pm\sqrt5)/2$. Therefore both methods converge for every starting vector exactly when $0<|\mu|<(\sqrt5-1)/2$. This equality of convergence ranges follows from their spectra, not from positive-definiteness of the nonsymmetric coefficient matrix.

#### Weighted Jacobi method

↑ **Parent:** [Jacobi method](#jacobi-method)

With relaxation parameter $\omega$, weighted Jacobi updates by

$$
x^{(\nu+1)}
=x^{(\nu)}+\omega D^{-1}(b-Ax^{(\nu)}).
$$

Its [iteration matrix](#iteration-matrix) is $H_\omega=I-\omega D^{-1}A$.

Equivalently, the [weighted Jacobi method](#weighted-jacobi-method) takes a weighted average of the old [vector](vector-space.md#vector) and its full [Jacobi method](#jacobi-method) update: $x^{(k+1)}=(1-\omega)x^{(k)}+\omega x_{\mathrm{Jacobi}}^{(k+1)}$. If $Bv=\lambda v$, its [iteration matrix](#iteration-matrix) multiplies that [eigenvector](linear-operator-theory.md#eigenvector) by $1-\omega+\omega\lambda$. For the diagonal-4 [Jacobi iteration for a three-variable tridiagonal system](#jacobi-iteration-for-a-three-variable-tridiagonal-system), the factors are $1-\omega$ and $1-\omega\pm\omega\sqrt2/4$; a [Poisson equation](partial-differential-equation.md#poisson-s-equation) smoothing parameter must not be inferred from this different [matrix](vector-space.md#matrix).

##### Weighted Jacobi eigenvalues for a square Dirichlet grid

↑ **Parent:** [Weighted Jacobi method](#weighted-jacobi-method)

For the five-point discretization of $-\Delta+c$ on the unit square, the weighted iteration [eigenvalues](linear-operator-theory.md#eigenvalue) are $1-\omega[4\sin^2(\pi kh/2)+4\sin^2(\pi lh/2)+ch^2]/(4+ch^2)$. A fixed parameter converges for every mesh when $0<\omega\leq1$, but $\omega=1$ poorly damps the highest frequencies.

##### Weighted Jacobi method for the one-dimensional Poisson equation

↑ **Parent:** [Weighted Jacobi method](#weighted-jacobi-method)

For the centered second-difference matrix with diagonal $-2$ and off-diagonals $1$, the weighted-Jacobi eigenvalues are

$$
\lambda_k(\omega)
=1-\omega+\omega\cos\frac{k\pi}{n+1},
\qquad 1\leq k\leq n.
$$

The method converges for every grid size exactly when $0<\omega\leq1$.

Multiplying both $A$ and $b$ by $-1$ leaves $D^{-1}A$ and the [weighted Jacobi method](#weighted-jacobi-method) unchanged. Thus the same formula applies to the positive second-difference [matrix](vector-space.md#matrix) $T_n$ with diagonal $2$ and neighboring entries $-1$, the [finite difference](finite-difference.md) form of the one-dimensional [Poisson equation](partial-differential-equation.md#poisson-s-equation) with [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition). Its [eigenvectors](linear-operator-theory.md#eigenvector) have components $\sin(jk\pi/(n+1))$, and $D^{-1}T_n$ has [eigenvalues](linear-operator-theory.md#eigenvalue) $1-\cos(k\pi/(n+1))$. At $\omega=2/3$, upper-half modes have factors between $-1/3$ and $1/3$, while low-frequency factors remain close to one on fine grids. This explains why the [weighted Jacobi method](#weighted-jacobi-method) helps a [multigrid method](multigrid-method.md) by reducing oscillatory errors, even when it is a slow solver on its own.[Error eigenvector expansion, coefficient 1/3 + (2/3) cos(jπ/2^i), and concluding upper-half-frequency attenuation statement](mathematics-bibliography.md#cs267-supplemental-notes-for-lecture-17-how-multigrid-damps-high-frequencies-by-james-demmel)

###### High-frequency smoothing factor of weighted Jacobi

↑ **Parent:** [Weighted Jacobi method for the one-dimensional Poisson equation](#weighted-jacobi-method-for-the-one-dimensional-poisson-equation)

For modes with $k/(n+1)\in[1/2,1]$ and large $n$, the worst attenuation factor is

$$
\mu_\omega=\max\{|1-\omega|,|1-2\omega|\}.
$$

It is minimized by $\omega=2/3$, for which $\mu_\omega=1/3$.

###### Exact finite-grid high-frequency Jacobi smoothing optimum

↑ **Parent:** [High-frequency smoothing factor of weighted Jacobi](#high-frequency-smoothing-factor-of-weighted-jacobi)

For the one-dimensional Dirichlet second-difference grid, high sine modes have eigenvalues $1-\omega t_k$, with $t_k=1-\cos(k\pi/(n+1))$ and $k\geq\lceil(n+1)/2\rceil$. Let $a$ and $b$ be the smallest and largest of these $t_k$. Convexity gives attenuation $\max(|1-\omega a|,|1-\omega b|)$. Balancing its endpoint values with opposite signs gives the displayed exact minimax choice. For odd $n$, $a=1$; for even $n$, $a=1+\sin(\pi/[2(n+1)])$, and always $b=1+\cos(\pi/(n+1))$. Only in the large-grid or uniform-in-grid limit do these become $\omega_*=2/3$, $\mu_*=1/3$.

#### Jacobi convergence for a three-by-three equicorrelation matrix

↑ **Parent:** [Jacobi method](#jacobi-method)

For a three-by-three matrix with diagonal entries one and every off-diagonal entry $\alpha$, the [Jacobi method](#jacobi-method) iteration matrix has eigenvalue $-2\alpha$ on the all-ones vector and eigenvalue $\alpha$ with multiplicity two on its orthogonal complement. Its [spectral radius](analysis.md#spectral-radius) is $2|\alpha|$, so Jacobi iteration converges exactly when $|\alpha|<1/2$.

#### Jacobi convergence for a symmetric positive-definite tridiagonal matrix

↑ **Parent:** [Jacobi method](#jacobi-method)

If $A=D+L+L^T$ is symmetric positive definite and tridiagonal, set $S=\operatorname{diag}(1,-1,1,-1,\ldots)$. Then

$$
SAS=D-L-L^T
$$

is positive definite. Applying the [Householder-John theorem](#householder-john-theorem) to $M=D$ and $N=-(L+L^T)$ proves that the Jacobi iteration converges.

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (2)

- [Iterative method](numerical-analysis.md#iterative-method)
- [Normal equations for linear least squares](linear-regression.md#normal-equations-for-linear-least-squares)
