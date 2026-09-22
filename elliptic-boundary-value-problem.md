# Elliptic boundary value problem

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

An elliptic boundary value problem couples an elliptic differential equation in a domain to [boundary conditions](differential-equation.md#boundary-condition). Its [weak formulation](partial-differential-equation.md#weak-formulation) is often an equation for a [bounded bilinear form](linear-algebra.md#bounded-bilinear-form) on a [Sobolev space](sobolev-space.md).

**Table of contents**

- [Direct spherical-shell H2 estimate](#direct-spherical-shell-h2-estimate)
- [Dirichlet realization of an elliptic operator](#dirichlet-realization-of-an-elliptic-operator)
- [Nonlinear elliptic boundary value problem](#nonlinear-elliptic-boundary-value-problem)
  - [Ordered subsolution and supersolution](#ordered-subsolution-and-supersolution)
    - [Monotone iteration for a semilinear elliptic equation](#monotone-iteration-for-a-semilinear-elliptic-equation)
  - [Small-data existence for a nonlinear elliptic Dirichlet problem](#small-data-existence-for-a-nonlinear-elliptic-dirichlet-problem)
  - [Cubic gradient nonlinearity](#cubic-gradient-nonlinearity)
- [Fredholm alternative for an elliptic Dirichlet problem](#fredholm-alternative-for-an-elliptic-dirichlet-problem)
  - [Small positive zeroth-order perturbation of a Dirichlet problem](#small-positive-zeroth-order-perturbation-of-a-dirichlet-problem)
  - [Boundary compatibility in the self-adjoint Fredholm alternative](#boundary-compatibility-in-the-self-adjoint-fredholm-alternative)
- [Uniformly elliptic operator](#uniformly-elliptic-operator)
  - [Quadratic ellipticity does not bound a nonsymmetric coefficient matrix](#quadratic-ellipticity-does-not-bound-a-nonsymmetric-coefficient-matrix)
  - [Nondivergence-form elliptic operator](#nondivergence-form-elliptic-operator)
  - [Divergence-form elliptic operator](#divergence-form-elliptic-operator)
    - [Constant flux for a one-dimensional divergence-form equation](#constant-flux-for-a-one-dimensional-divergence-form-equation)
    - [Constant shifts of a divergence-form equation](#constant-shifts-of-a-divergence-form-equation)
    - [Homogeneous divergence-form elliptic equation](#homogeneous-divergence-form-elliptic-equation)
    - [Weak supersolution of a divergence-form elliptic equation](#weak-supersolution-of-a-divergence-form-elliptic-equation)
    - [Weak subsolution of a divergence-form elliptic equation](#weak-subsolution-of-a-divergence-form-elliptic-equation)
      - [Local boundedness of weak elliptic subsolutions](#local-boundedness-of-weak-elliptic-subsolutions)
  - [Strict positivity implies coercivity for an elliptic Dirichlet form](#strict-positivity-implies-coercivity-for-an-elliptic-dirichlet-form)
  - [Constant-coefficient elliptic second-derivative estimate](#constant-coefficient-elliptic-second-derivative-estimate)
    - [Perturbation of a constant-coefficient elliptic second-derivative estimate](#perturbation-of-a-constant-coefficient-elliptic-second-derivative-estimate)
      - [Coefficient-freezing interior second-derivative estimate](#coefficient-freezing-interior-second-derivative-estimate)
        - [Interior H2 regularity for continuous nondivergence coefficients](#interior-h2-regularity-for-continuous-nondivergence-coefficients)
  - [Strictly elliptic operator](#strictly-elliptic-operator)
  - [Weak maximum principle for elliptic operators](#weak-maximum-principle-for-elliptic-operators)
    - [Maximum bound for a monotone reaction term](#maximum-bound-for-a-monotone-reaction-term)
    - [Supremum norm barrier for an elliptic Dirichlet problem](#supremum-norm-barrier-for-an-elliptic-dirichlet-problem)
    - [Strong maximum principle for elliptic operators](#strong-maximum-principle-for-elliptic-operators)
    - [Exponential perturbation proof of the weak maximum principle with drift](#exponential-perturbation-proof-of-the-weak-maximum-principle-with-drift)
    - [Failure of the weak maximum principle with a positive zeroth-order coefficient](#failure-of-the-weak-maximum-principle-with-a-positive-zeroth-order-coefficient)
    - [Alexandrov–Bakelman–Pucci estimate](#alexandrov-bakelman-pucci-estimate)
    - [Strong minimum principle for elliptic operators](#strong-minimum-principle-for-elliptic-operators)
  - [Schauder estimates](#schauder-estimates)
    - [Interpolation inequality in Holder spaces](#interpolation-inequality-in-holder-spaces)
    - [Interior Schauder estimate](#interior-schauder-estimate)
      - [Necessity of Hölder forcing for Schauder estimates](#necessity-of-holder-forcing-for-schauder-estimates)
      - [Blow-up compactness proof of an interior Schauder estimate](#blow-up-compactness-proof-of-an-interior-schauder-estimate)
        - [Taylor normalization in elliptic blow-up arguments](#taylor-normalization-in-elliptic-blow-up-arguments)
    - [Boundary Schauder estimate](#boundary-schauder-estimate)
      - [Global Schauder estimate](#global-schauder-estimate)
        - [Compactness of zero-boundary Poisson solutions](#compactness-of-zero-boundary-poisson-solutions)
        - [Compactness proof of a nonnegative elliptic solution estimate](#compactness-proof-of-a-nonnegative-elliptic-solution-estimate)
    - [Simon absorption lemma](#simon-absorption-lemma)
  - [De Giorgi-Nash-Moser theorem](#de-giorgi-nash-moser-theorem)
    - [Compactness of normalized weak elliptic solutions](#compactness-of-normalized-weak-elliptic-solutions)
    - [Moser iteration](#moser-iteration)
      - [Moser product on geometric radii](#moser-product-on-geometric-radii)
      - [Liouville theorem for integrable nonnegative elliptic subsolutions](#liouville-theorem-for-integrable-nonnegative-elliptic-subsolutions)
      - [Weak Harnack inequality](#weak-harnack-inequality)
        - [Propagation of zeros by the weak Harnack inequality](#propagation-of-zeros-by-the-weak-harnack-inequality)
        - [Oscillation decay estimate](#oscillation-decay-estimate)
          - [Inhomogeneous oscillation decay implies Hölder continuity](#inhomogeneous-oscillation-decay-implies-holder-continuity)
        - [Harnack inequality for uniformly elliptic divergence-form equations](#harnack-inequality-for-uniformly-elliptic-divergence-form-equations)
- [Degenerate elliptic operator](#degenerate-elliptic-operator)
  - [Sine-mode expansion for a quadratically degenerate elliptic equation](#sine-mode-expansion-for-a-quadratically-degenerate-elliptic-equation)
    - [Forced zero trace at a quadratically degenerate boundary](#forced-zero-trace-at-a-quadratically-degenerate-boundary)
  - [Failure of a coercive Dirichlet estimate under degeneracy](#failure-of-a-coercive-dirichlet-estimate-under-degeneracy)
- [Method of continuity](#method-of-continuity)
- [Hopf lemma](#hopf-lemma)
  - [Hopf dichotomy with classical regularity away from the zero set](#hopf-dichotomy-with-classical-regularity-away-from-the-zero-set)
  - [Interior sphere condition](#interior-sphere-condition)

## Direct spherical-shell H2 estimate

↑ **Parent:** [Elliptic boundary value problem](elliptic-boundary-value-problem.md)

On a fixed shell $a<r<b$ with $a>0$, put $T=\partial_r^2+2r^{-1}\partial_r$ and $A=\Delta_{S^2}$. If $u$ is smooth and zero on both boundary spheres, direct radial and spherical [integration by parts](calculus.md#integration-by-parts) gives

$$
\|\Delta u\|_2^2=\|Tu\|_2^2+\|r^{-2}Au\|_2^2+2\int_a^b\!\int_{S^2}|\nabla_Su_r|^2-2\int_a^b\!\int_{S^2}r^{-2}|\nabla_Su|^2.
$$

The last term is controlled by the first-order energy estimate. The [spherical Hessian identity](differential-geometry.md#spherical-hessian-identity) controls angular second [derivatives](calculus.md#derivative), and the radial/mixed [derivatives](calculus.md#derivative) follow from $T$ and $\nabla_Su_r$. The polar orthonormal-frame formulas for the Cartesian [Hessian matrix](calculus.md#hessian-matrix) then prove the estimate. Zero boundary values eliminate the radial boundary remainders because every angular [derivative](calculus.md#derivative) of their traces is zero.

## Dirichlet realization of an elliptic operator

↑ **Parent:** [Elliptic boundary value problem](elliptic-boundary-value-problem.md)

A smooth uniformly elliptic differential expression with symmetric Dirichlet [bilinear form](linear-algebra.md#bilinear-form) has an unbounded [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) realization $A_D$ on $L^2(U)$, whose domain is $H^2(U)\cap H_0^1(U)$ on a smooth bounded domain. If the form is strictly positive, the [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) and [elliptic regularity](distribution-theory.md#elliptic-regularity) make $A_D^{-1}$ a bounded map from $L^2$ to $H^2\cap H_0^1$. Its action on $L^2$ is [compact](topology.md#compact-space) by the [Rellich-Kondrachov compactness theorem](sobolev-space.md#rellich-kondrachov-theorem) and self-adjoint by symmetry of the form. The [spectral theorem for compact Hermitian operators](compact-operator.md#spectral-theorem-for-compact-hermitian-operators) therefore gives an [orthonormal basis](linear-algebra.md#orthonormal-basis) of smooth Dirichlet [eigenfunctions](linear-operator-theory.md#eigenfunction) with positive [eigenvalues](linear-operator-theory.md#eigenvalue) tending to infinity.

## Nonlinear elliptic boundary value problem

↑ **Parent:** [Elliptic boundary value problem](elliptic-boundary-value-problem.md)

A nonlinear elliptic boundary value problem contains a nonlinear dependence on the unknown function or its derivatives while retaining an elliptic principal part. Small-data existence can often be proved by applying a [fixed-point theorem](analysis.md#fixed-point-theorem) to the inverse of the linear elliptic part.

### Ordered subsolution and supersolution

↑ **Parent:** [Nonlinear elliptic boundary value problem](#nonlinear-elliptic-boundary-value-problem)

For $Qu=\Delta u-V(u)$, a subsolution and supersolution satisfy $Q\varphi^-\geq0$ and $Q\varphi^+\leq0$, respectively. An ordered pair additionally satisfies $\varphi^-\leq\varphi^+$ throughout the domain, with boundary data $\psi$ between their boundary traces. This interior condition is separate from boundary ordering when $V$ is non-increasing: for $V(s)=-\lambda_1s$, a positive first [Dirichlet Laplacian eigenfunction](partial-differential-equation.md#dirichlet-laplacian-eigenfunction) $e_1$ and $-e_1$ both solve the homogeneous equation and vanish on the boundary, but taking $\varphi^-=e_1$ and $\varphi^+=-e_1$ produces reversed interior barriers.

#### Monotone iteration for a semilinear elliptic equation

↑ **Parent:** [Ordered subsolution and supersolution](#ordered-subsolution-and-supersolution)

For smooth non-increasing $V$ and an [ordered subsolution and supersolution](#ordered-subsolution-and-supersolution), begin with $u_0=\varphi^-$ and solve successive [Poisson equations](partial-differential-equation.md#poisson-equation) with forcing $V(u_k)$ and the fixed boundary data. The [weak maximum principle for elliptic operators](#weak-maximum-principle-for-elliptic-operators) applied to the negatives of consecutive differences gives

$$
\varphi^-\leq u_1\leq u_2\leq\cdots\leq\varphi^+.
$$

The [global Schauder estimate](#global-schauder-estimate) and the [Hölder interpolation inequality](sobolev-space.md#holder-interpolation-inequality) bound the iterates uniformly in $C^{2,\alpha}$. Their bounded [monotone sequence](real-analysis.md#monotone-sequence) converges, and [compact embedding of Hölder spaces](sobolev-space.md#compact-embedding-of-holder-spaces) permits passing to the equation. The uniform [Hölder seminorm](sobolev-space.md#holder-seminorm) bounds retain $C^{2,\alpha}$ regularity of the limit.

### Small-data existence for a nonlinear elliptic Dirichlet problem

↑ **Parent:** [Nonlinear elliptic boundary value problem](#nonlinear-elliptic-boundary-value-problem)

Suppose the inverse $S:C^{0,\alpha}\to C^{2,\alpha}_0$ of a linear [elliptic boundary value problem](elliptic-boundary-value-problem.md) is bounded by $K$, and a nonlinear map satisfies

$$
\|Q(v)\|_{C^{0,\alpha}}\leq C\|v\|_{C^{2,\alpha}}^2+\delta,\qquad
\|Q(v)-Q(w)\|_{C^{0,\alpha}}\leq[C(\|v\|+\|w\|)+\delta]\|v-w\|.
$$

Then $T(v)=S(Q(v)+f)$ maps a sufficiently small closed ball into itself and is a [contraction mapping](analysis.md#contraction-mapping) when $\delta$ and $\|f\|_{C^{0,\alpha}}$ are sufficiently small. The [Banach fixed-point theorem](analysis.md#contraction-mapping-theorem) gives a solution of $Lu=Q(u)+f$ with zero [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition), unique within that ball. Invertibility follows from the [Fredholm alternative for an elliptic Dirichlet problem](#fredholm-alternative-for-an-elliptic-dirichlet-problem) when the homogeneous [null space](linear-algebra.md#kernel-of-a-linear-map) is zero.

### Cubic gradient nonlinearity

↑ **Parent:** [Nonlinear elliptic boundary value problem](#nonlinear-elliptic-boundary-value-problem)

In three dimensions the map $N(u)=|Du|^2u$ sends $H^2$ into $L^2$, because $H^2\hookrightarrow W^{1,4}\cap L^\infty$. On an $H^2$ ball of radius $R$ it is locally Lipschitz with constant $O(R^2)$.

## Fredholm alternative for an elliptic Dirichlet problem

↑ **Parent:** [Elliptic boundary value problem](elliptic-boundary-value-problem.md)

For a uniformly elliptic operator $L$ on a bounded regular domain, exactly one of the following equivalent descriptions applies to its homogeneous [Dirichlet problem](differential-equation.md#dirichlet-boundary-condition). If $\ker L^*=0$, every forcing has a unique solution. Otherwise $Lu=f$ is solvable exactly when $f$ is orthogonal to $\ker L^*$, and any two solutions differ by an element of $\ker L$. Moreover $\dim\ker L=\dim\ker L^*$.

### Small positive zeroth-order perturbation of a Dirichlet problem

↑ **Parent:** [Fredholm alternative for an elliptic Dirichlet problem](#fredholm-alternative-for-an-elliptic-dirichlet-problem)

The zero-boundary problem $\Delta u+cu=f$ is uniquely solvable if $c$ has a sufficiently small positive part depending only on the bounded regular domain. Write $c=c_-+c_+$ with $c_-\leq0$. The [supremum norm barrier for an elliptic Dirichlet problem](#supremum-norm-barrier-for-an-elliptic-dirichlet-problem) gives $\|u\|_\infty\leq C_\Omega\|c_+u\|_\infty$ for a homogeneous solution. If $C_\Omega\|c_+\|_\infty<1$, its kernel is zero and the [Fredholm alternative for an elliptic Dirichlet problem](#fredholm-alternative-for-an-elliptic-dirichlet-problem) gives existence for every forcing and boundary datum.

### Boundary compatibility in the self-adjoint Fredholm alternative

↑ **Parent:** [Fredholm alternative for an elliptic Dirichlet problem](#fredholm-alternative-for-an-elliptic-dirichlet-problem)

For real $c$ and $L=\Delta+c$ on a bounded regular domain, let $N$ be the zero-boundary kernel. The problem $Lu=f$, $u=\psi$ on the boundary is solvable exactly when $\int_\Omega fz+\int_{\partial\Omega}\psi\partial_\nu z=0$ for every $z\in N$. The sign follows from [Green second identity](partial-differential-equation.md#green-second-identity). After subtracting a boundary extension of $\psi$, this is the usual orthogonality of the forcing to the [null space](linear-algebra.md#kernel-of-a-linear-map) of the [self-adjoint](linear-operator-theory.md#self-adjoint-operator) Dirichlet realization. All solutions then differ by an element of $N$.

## Uniformly elliptic operator

↑ **Parent:** [Elliptic boundary value problem](elliptic-boundary-value-problem.md)

A second-order operator with coefficient matrix $A(x)=(a^{ij}(x))$ is uniformly elliptic when some $\lambda>0$ satisfies $a^{ij}(x)\xi_i\xi_j\geq\lambda|\xi|^2$ everywhere.

### Quadratic ellipticity does not bound a nonsymmetric coefficient matrix

↑ **Parent:** [Uniformly elliptic operator](#uniformly-elliptic-operator)

The [quadratic form](linear-algebra.md#quadratic-form) of a matrix only sees its symmetric part. Thus $\lambda|\xi|^2\leq\xi^TA\xi\leq\Lambda|\xi|^2$ need not bound the skew part of a measurable coefficient matrix. For $A=\begin{pmatrix}1&k\\-k&1\end{pmatrix}$ the quadratic form is exactly $|\xi|^2$, regardless of $k$. On a square, take $k(x)=1/|x_1|$ off the line $x_1=0$, with a finite arbitrary value on that line. Two compactly supported smooth functions that equal $x_2$ and $x_1$ near the origin have $(A\nabla u)\cdot\nabla v=k$ there; the purported energy pairing is not integrable. A [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) proof therefore requires bounded full coefficients or another hypothesis that makes the bilinear form bounded. Symmetry supplies the missing matrix bound from the quadratic upper bound.

### Nondivergence-form elliptic operator

↑ **Parent:** [Uniformly elliptic operator](#uniformly-elliptic-operator)

A [nondivergence-form elliptic operator](#nondivergence-form-elliptic-operator) applies its principal coefficients directly to the [Hessian matrix](calculus.md#hessian-matrix): $Lu=a^{ij}D_{ij}u+b^iD_i u+cu$. Only the symmetric part of $a$ contributes to the second-derivative term. [Uniform ellipticity](#uniformly-elliptic-operator) bounds its [quadratic form](linear-algebra.md#quadratic-form) below by $\lambda|\xi|^2$ with a constant $\lambda>0$ independent of position.

### Divergence-form elliptic operator

↑ **Parent:** [Uniformly elliptic operator](#uniformly-elliptic-operator)

A divergence-form elliptic operator is $Lu=D_i(a^{ij}D_j u)$, with bounded measurable coefficients whose symmetric part has a uniform positive lower bound. Its [weak formulation](partial-differential-equation.md#weak-formulation) involves only first [weak derivatives](distribution-theory.md#weak-derivative), so differentiability of the coefficients is unnecessary.

#### Constant flux for a one-dimensional divergence-form equation

↑ **Parent:** [Divergence-form elliptic operator](#divergence-form-elliptic-operator)

On an interval, the weak equation $(au^{\prime})^{\prime}=0$ makes $au^{\prime}$ constant almost everywhere. If $\lambda\leq a\leq\Lambda$, the derivative energy on concentric subintervals satisfies $E(r)\leq(\Lambda/\lambda)^2(r/R)E(R)$. This supplies [dyadic energy decay](partial-differential-equation.md#dyadic-energy-decay) even though a one-dimensional [annulus](topology.md#annulus-mathematics) is disconnected.

#### Constant shifts of a divergence-form equation

↑ **Parent:** [Divergence-form elliptic operator](#divergence-form-elliptic-operator)

If $Lu=\operatorname{div}F+g$ and $L$ contains $\operatorname{div}(bu)+du$, then $L(u-k)=\operatorname{div}(F-kb)+(g-kd)$. Thus shifting a [weak solution](partial-differential-equation.md#weak-solution) to make it nonnegative changes the forcing unless the operator annihilates constants. This bookkeeping is essential in applying the [Weak Harnack inequality](#weak-harnack-inequality) to upper and lower oscillations.

#### Homogeneous divergence-form elliptic equation

↑ **Parent:** [Divergence-form elliptic operator](#divergence-form-elliptic-operator)

For a bounded measurable coefficient [matrix](vector-space.md#matrix) $A$, an $H^1$ [weak solution](partial-differential-equation.md#weak-solution) of $\operatorname{div}(A\nabla u)=0$ satisfies $\int A\nabla u\cdot\nabla\varphi=0$ for every compactly supported smooth [test function](distribution-theory.md#test-function). By density this identity extends to compactly supported $H^1$ tests. If $A$ is symmetric and $\lambda I\le A\le\Lambda I$, [Caccioppoli inequalities](partial-differential-equation.md#caccioppoli-inequality) follow without differentiating $A$.

#### Weak supersolution of a divergence-form elliptic equation

↑ **Parent:** [Divergence-form elliptic operator](#divergence-form-elliptic-operator)

For $Lu=D_i(a^{ij}D_j u)$, a [weak supersolution](#weak-supersolution-of-a-divergence-form-elliptic-equation) satisfies $Lu\leq0$ as a [distribution](distribution-theory.md#distribution-mathematical-analysis), equivalently $\int a^{ij}D_j uD_i\phi\geq0$ for every nonnegative compactly supported [test function](distribution-theory.md#test-function) $\phi$. The [Weak Harnack inequality](#weak-harnack-inequality) applies to nonnegative [weak supersolutions](#weak-supersolution-of-a-divergence-form-elliptic-equation) with this sign convention.

#### Weak subsolution of a divergence-form elliptic equation

↑ **Parent:** [Divergence-form elliptic operator](#divergence-form-elliptic-operator)

For the sign convention $Lu=D_i(a^{ij}D_j u)$, a [weak subsolution](#weak-subsolution-of-a-divergence-form-elliptic-equation) satisfies $Lu\geq0$ as a [distribution](distribution-theory.md#distribution-mathematical-analysis), equivalently $\int a^{ij}D_j uD_i\phi\leq0$ for every nonnegative compactly supported [test function](distribution-theory.md#test-function) $\phi$. A [weak supersolution](#weak-supersolution-of-a-divergence-form-elliptic-equation) has the reversed inequality.

##### Local boundedness of weak elliptic subsolutions

↑ **Parent:** [Weak subsolution of a divergence-form elliptic equation](#weak-subsolution-of-a-divergence-form-elliptic-equation)

For a [uniformly elliptic](#uniformly-elliptic-operator) [divergence-form elliptic operator](#divergence-form-elliptic-operator) with lower-order coefficients in the supercritical [Lebesgue spaces](measure-theory.md#lp-space), truncation tests and [Moser iteration](#moser-iteration) bound the [positive part](function.md#positive-part-of-a-real-valued-function) of a [weak subsolution](#weak-subsolution-of-a-divergence-form-elliptic-equation) on an interior ball by its [Lp norm](real-analysis.md#lp-norm) on a larger ball and the forcing norms. In particular, every [weak subsolution](#weak-subsolution-of-a-divergence-form-elliptic-equation) of the homogeneous equation is locally bounded above. This is the preliminary estimate needed when a [strong maximum principle](#strong-maximum-principle-for-elliptic-operators) is phrased using [essential suprema](measure-theory.md#essential-supremum).

### Strict positivity implies coercivity for an elliptic Dirichlet form

↑ **Parent:** [Uniformly elliptic operator](#uniformly-elliptic-operator)

Let $B[u,v]=\int_U a^{ij}\partial_i u\partial_j v+cuv$ on $H_0^1(U)$ for a bounded smooth domain, smooth symmetric uniformly positive coefficients, and bounded real $c$. If $B[u,u]>0$ for every nonzero $u$, then $B[u,u]\geq\alpha\|u\|_{H^1}^2$ for some $\alpha>0$. If this failed, choose $\|u_j\|_{H^1}=1$ with $B[u_j,u_j]\to0$. The [Rellich-Kondrachov compactness theorem](sobolev-space.md#rellich-kondrachov-theorem) gives a subsequence weakly converging in $H_0^1$ and strongly in $L^2$. The principal energy has [weak lower semicontinuity](functional-analysis.md#weak-lower-semicontinuity), and the potential term converges, so strict positivity forces the limit to be zero. Uniform ellipticity then gives $\|Du_j\|_2\to0$, contradicting normalization. Merely being a [positive semidefinite operator](hilbert-space.md#positive-operator) is insufficient: $-\Delta-\lambda_1$ has a nonzero Dirichlet [eigenfunction](linear-operator-theory.md#eigenfunction) of zero energy.

### Constant-coefficient elliptic second-derivative estimate

↑ **Parent:** [Uniformly elliptic operator](#uniformly-elliptic-operator)

If the constant [symmetric matrix](linear-algebra.md#symmetric-matrix) $A$ satisfies $A\xi\mathbin\cdot\xi\geq\theta|\xi|^2$, then every [smooth function](analysis.md#smooth-function) $u$ with [compact support](function.md#compact-support) satisfies

$$
\theta\|D^2u\|_2\leq\|A^{ij}D_{ij}u\|_2.
$$

Indeed, the [Fourier transform of a derivative](fourier-analysis.md#fourier-transform-of-a-derivative) and the [Plancherel theorem](fourier-analysis.md#plancherel-theorem) turn the squared norms into integrals with [Fourier multipliers](analysis.md#fourier-multiplier) $|\xi|^4$ and $(A\xi\mathbin\cdot\xi)^2$.

#### Perturbation of a constant-coefficient elliptic second-derivative estimate

↑ **Parent:** [Constant-coefficient elliptic second-derivative estimate](#constant-coefficient-elliptic-second-derivative-estimate)

If $\|a^{ij}-A^{ij}\|_\infty<\varepsilon$ for every $i,j$, then the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\|(a^{ij}-A^{ij})D_{ij}u\|_2\leq n\varepsilon\|D^2u\|_2.
$$

Consequently $\varepsilon\leq\theta/(2n)$ preserves half of the estimate's lower bound.

##### Coefficient-freezing interior second-derivative estimate

↑ **Parent:** [Perturbation of a constant-coefficient elliptic second-derivative estimate](#perturbation-of-a-constant-coefficient-elliptic-second-derivative-estimate)

For a [uniformly elliptic operator](#uniformly-elliptic-operator) $Lu=a^{ij}(x)D_{ij}u$ with [continuous](calculus.md#continuous-function) coefficients and $W\Subset U$,

$$
\|D^2u\|_{L^2(W)}\leq C\left(\|Lu\|_{L^2(U)}+\|u\|_{H^1(U)}\right).
$$

[Uniform continuity](topological-analysis.md#uniform-continuity) lets one freeze $a^{ij}$ on sufficiently small [open balls](topology.md#open-ball) and use the [perturbation of a constant-coefficient elliptic second-derivative estimate](#perturbation-of-a-constant-coefficient-elliptic-second-derivative-estimate). A [partition of unity](differential-geometry.md#partition-of-unity) and [cutoff functions](distribution-theory.md#cutoff-function) reduce the global interior estimate to finitely many such balls; derivatives of the cutoffs produce only the displayed lower-order norm.

###### Interior H2 regularity for continuous nondivergence coefficients

↑ **Parent:** [Coefficient-freezing interior second-derivative estimate](#coefficient-freezing-interior-second-derivative-estimate)

Let $L=a^{ij}(x)D_{ij}$ be uniformly elliptic with continuous coefficients. The [coefficient-freezing interior second-derivative estimate](#coefficient-freezing-interior-second-derivative-estimate) extends from smooth functions to the [graph norm](functional-analysis.md#graph-norm) closure of $L$ on $H^1(U)$: if $u_k\to u$ in $H^1(U)$ and $Lu_k\to f$ in $L^2(U)$, then $(u_k)$ is Cauchy in $H^2(W)$ for every $W\Subset U$. Hence $u\in H^2_{\mathrm{loc}}(U)$ and $Lu=f$. Equivalently, the standard local regularization argument gives the same conclusion for [weak solutions](partial-differential-equation.md#weak-solution).

### Strictly elliptic operator

↑ **Parent:** [Uniformly elliptic operator](#uniformly-elliptic-operator)

A second-order operator is strictly elliptic at a point when its symmetric principal coefficient matrix is positive definite there. Uniform ellipticity strengthens this pointwise condition by requiring one positive lower bound throughout the domain.

### Weak maximum principle for elliptic operators

↑ **Parent:** [Uniformly elliptic operator](#uniformly-elliptic-operator)

For a second-order elliptic operator $Lu=a^{ij}D_{ij}u+b^iD_iu+cu$ with $c\leq0$, the inequality $Lu\geq0$ on a bounded domain implies

$$
\max_{\overline\Omega}u\leq\max\{0,\max_{\partial\Omega}u\}.
$$

An exponential barrier reduces the non-strict inequality to a contradiction at a positive interior maximum.

#### Maximum bound for a monotone reaction term

↑ **Parent:** [Weak maximum principle for elliptic operators](#weak-maximum-principle-for-elliptic-operators)

Let $h:\mathbb R\to\mathbb R$ be continuous, odd, strictly increasing and onto. Suppose $u\in C^2(\mathbb R^d)$ tends to zero at infinity and satisfies $-\Delta u+h(u)=f$, with bounded $f$. At a positive maximum $m$ of $u$, $-\Delta u\geq0$, so $h(m)\leq f\leq\|f\|_\infty$. Apply the same argument to $-u$ to obtain the displayed bound, using the maximum-point argument of the [weak maximum principle for elliptic operators](#weak-maximum-principle-for-elliptic-operators). For $h(s)=s+\sin s$, strict monotonicity follows by integrating $h'=1+\cos s$, whose zeros are isolated. Thus $\|u\|_\infty\leq h^{-1}(\|f\|_\infty)\leq\|f\|_\infty+1$. The stronger bound by $\|f\|_\infty$ holds when that norm is at most $\pi$, but need not hold for larger sources.

#### Supremum norm barrier for an elliptic Dirichlet problem

↑ **Parent:** [Weak maximum principle for elliptic operators](#weak-maximum-principle-for-elliptic-operators)

If $c\leq0$, $\Delta u+cu=f$, and $u=\psi$ on the boundary of a bounded domain inside $\{|x_1|<d\}$, let $M=\sup_{\partial\Omega}|\psi|$ and $F=\sup_\Omega|f|$. The nonnegative barrier $v=M+(e^{2d}-e^{x_1+d})F$ satisfies $(\Delta+c)v\leq-F$. Apply the [weak maximum principle for elliptic operators](#weak-maximum-principle-for-elliptic-operators) to $u-v$ and $-u-v$ to get $\|u\|_\infty\leq M+e^{2d}F$.

#### Strong maximum principle for elliptic operators

↑ **Parent:** [Weak maximum principle for elliptic operators](#weak-maximum-principle-for-elliptic-operators)

For a locally [uniformly elliptic operator](#uniformly-elliptic-operator) $L=a^{ij}D_{ij}+b^iD_i+c$ with locally bounded coefficients and $c\leq0$, a $C^2$ function satisfying $Lu\geq0$ on a connected domain cannot attain a nonnegative global maximum inside unless it is constant. If $c=0$, the maximum can have either sign. If the maximum set were proper, choose an interior ball in its complement tangent to that set. The [Hopf boundary point lemma](#hopf-lemma) gives a nonzero normal derivative at the contact point, contradicting the vanishing [gradient](calculus.md#gradient) at an interior maximum.

The [strong minimum principle for elliptic operators](#strong-minimum-principle-for-elliptic-operators) follows by applying this to $-u$. For nonnegative $u$ with $Lu\leq0$, replacing $c$ by $\min(c,0)$ retains the inequality, so the strict positivity-or-zero conclusion does not require an original sign restriction on $c$.

#### Exponential perturbation proof of the weak maximum principle with drift

↑ **Parent:** [Weak maximum principle for elliptic operators](#weak-maximum-principle-for-elliptic-operators)

For $Lu=a^{ij}D_{ij}u+b^iD_iu$ with $a^{ij}\xi_i\xi_j\geq\lambda|\xi|^2$ and $|b^1|<\lambda\ell$, the function $q(x)=e^{-\ell x_1}$ satisfies

$$
Lq=q(\ell^2a^{11}-\ell b^1)>0.
$$

If $Lu\geq0$ had a strict interior maximum above the boundary maximum, then $u+\varepsilon q$ would retain an interior maximum for small $\varepsilon>0$, where ellipticity gives $L(u+\varepsilon q)\leq0$. This contradicts its strictly positive image under $L$.

#### Failure of the weak maximum principle with a positive zeroth-order coefficient

↑ **Parent:** [Weak maximum principle for elliptic operators](#weak-maximum-principle-for-elliptic-operators)

A positive zeroth-order coefficient can destroy the weak maximum principle. On $(0,1)$, the function $u(x)=\sin(\pi x)$ has zero boundary values and a positive interior maximum, but

$$
u''+\pi^2u=0.
$$

<h4 id="alexandrov-bakelman-pucci-estimate">Alexandrov–Bakelman–Pucci estimate</h4>

↑ **Parent:** [Weak maximum principle for elliptic operators](#weak-maximum-principle-for-elliptic-operators)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alexandrov–Bakelman–Pucci_estimate)

The Alexandrov–Bakelman–Pucci estimate bounds the positive maximum of a function by its boundary maximum and an $L^n$ norm of the negative part of a uniformly elliptic operator applied to it. It yields a maximum principle and a sup-norm estimate for elliptic equations with measurable principal coefficients.

#### Strong minimum principle for elliptic operators

↑ **Parent:** [Weak maximum principle for elliptic operators](#weak-maximum-principle-for-elliptic-operators)

Let $L$ be uniformly elliptic with bounded coefficients and nonpositive zeroth-order coefficient. If $u\geq0$, $Lu\leq0$, and $u$ vanishes at an interior point of a connected domain, then $u$ vanishes identically. This is the minimum form of the [strong maximum principle](partial-differential-equation.md#strong-maximum-principle-for-harmonic-functions).

### Schauder estimates

↑ **Parent:** [Uniformly elliptic operator](#uniformly-elliptic-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schauder_estimates)

A Schauder estimate bounds a solution in a Hölder norm two derivatives stronger than the forcing term. For a uniformly elliptic Dirichlet problem with $C^\alpha$ coefficients,

$$
\lVert u\rVert_{C^{2,\alpha}(\overline\Omega)}
\leq C\bigl(\lVert Lu\rVert_{C^\alpha(\overline\Omega)}+\lVert u\rVert_{C^0(\overline\Omega)}\bigr).
$$

#### Interpolation inequality in Holder spaces

↑ **Parent:** [Schauder estimates](#schauder-estimates)

For $u\in C^{l,\alpha}(B_R)$, $0\leq j<l$, and every $\varepsilon>0$,

$$
R^j[D^ju]_{0;B_R}
\leq \varepsilon R^{l+\alpha}[D^lu]_{\alpha;B_R}
+C\varepsilon^{-j/(l+\alpha-j)}[u]_{0;B_R},
$$

with analogous estimates for lower Hölder seminorms. Scaling reduces the result to the unit ball.

#### Interior Schauder estimate

↑ **Parent:** [Schauder estimates](#schauder-estimates)

For $\Omega'\Subset\Omega$ and a uniformly elliptic operator with $C^{0,\alpha}$ coefficients,

$$
\|u\|_{C^{2,\alpha}(\Omega')}\leq C\left(\|u\|_{C^0(\Omega)}+\|Lu\|_{C^{0,\alpha}(\Omega)}\right).
$$

The constant deteriorates as $\Omega'$ approaches the boundary.

<h5 id="necessity-of-holder-forcing-for-schauder-estimates">Necessity of Hölder forcing for Schauder estimates</h5>

↑ **Parent:** [Interior Schauder estimate](#interior-schauder-estimate)

The bounded-forcing norm alone cannot control the [Hölder seminorm](sobolev-space.md#holder-seminorm) of the [Hessian matrix](calculus.md#hessian-matrix). On a unit [Euclidean ball](functional-analysis.md#euclidean-ball) take $u_m=m^{-2}\sin(mx_1)$ and $f_m=\Delta u_m=-\sin(mx_1)$. The [derivative supremum norm](functional-analysis.md#derivative-supremum-norm) $|u_m|_2$ and $\|f_m\|_\infty$ stay bounded, but the [Hessian matrix](calculus.md#hessian-matrix) difference between zero and $\pi/(2m)e_1$ gives $[D^2u_m]_\alpha\geq(2m/\pi)^\alpha$ on $B_{1/2}$.

##### Blow-up compactness proof of an interior Schauder estimate

↑ **Parent:** [Interior Schauder estimate](#interior-schauder-estimate)

A compactness proof of the [interior Schauder estimate](#interior-schauder-estimate) can magnify a pair of points where the [Hölder seminorm](sobolev-space.md#holder-seminorm) of the [Hessian matrix](calculus.md#hessian-matrix) is nearly attained. If the proposed estimate fails, normalize that seminorm to one while lower norms and forcing tend to zero. The separation $r_j$ of the chosen pair tends to zero. Subtract the quadratic [Taylor polynomial](calculus.md#taylor-polynomial) and divide by $r_j^{2+\alpha}$ after rescaling space by $r_j$.

The resulting functions have uniformly bounded Hessian [Hölder seminorms](sobolev-space.md#holder-seminorm) on expanding domains and vanishing Taylor data at zero. [Compact embedding of Hölder spaces](sobolev-space.md#compact-embedding-of-holder-spaces) yields an entire [harmonic function](partial-differential-equation.md#harmonic-function) whose second derivatives have finite global $\alpha$-Hölder seminorms, with $0<\alpha<1$. The [polynomial-growth Liouville theorem for harmonic functions](partial-differential-equation.md#polynomial-growth-liouville-theorem-for-harmonic-functions) makes those derivatives constant, contradicting the normalized nonzero oscillation. The [Simon absorption lemma](#simon-absorption-lemma) removes the residual small multiple of the larger-ball seminorm.

###### Taylor normalization in elliptic blow-up arguments

↑ **Parent:** [Blow-up compactness proof of an interior Schauder estimate](#blow-up-compactness-proof-of-an-interior-schauder-estimate)

Subtracting the quadratic [Taylor polynomial](calculus.md#taylor-polynomial) at the rescaling centre makes the function, [gradient](calculus.md#gradient) and [Hessian matrix](calculus.md#hessian-matrix) vanish there. Dividing by $Ar^{2+\mu}$ preserves the normalized Hölder oscillation of the [Hessian matrix](calculus.md#hessian-matrix) while turning a small forcing-to-oscillation ratio into a harmonic limiting equation. The three vanished Taylor coefficients provide local bounds needed by the [Arzelà-Ascoli theorem](topological-analysis.md#arzela-ascoli-theorem).

#### Boundary Schauder estimate

↑ **Parent:** [Schauder estimates](#schauder-estimates)

For a uniformly elliptic equation on a half-ball with $C^{0,\alpha}$ coefficients and $C^{2,\alpha}$ Dirichlet data $\varphi$ on its flat face,

$$
\|u\|_{C^{2,\alpha}(B_{1/2}^+)}\leq C\left(\|u\|_{C^0(B_1^+)}+\|Lu\|_{C^{0,\alpha}(B_1^+)}+\|\varphi\|_{C^{2,\alpha}(B_1^+)}\right).
$$

##### Global Schauder estimate

↑ **Parent:** [Boundary Schauder estimate](#boundary-schauder-estimate)

On a smooth bounded domain, interior and boundary Schauder estimates combine into a $C^{2,\alpha}$ estimate up to the full boundary. The constant depends on the domain regularity, coefficient norms, and ellipticity constants.

###### Compactness of zero-boundary Poisson solutions

↑ **Parent:** [Global Schauder estimate](#global-schauder-estimate)

On a fixed smooth bounded domain, zero-boundary solutions with forcing in a bounded subset of $C^{0,\mu}$ are uniformly bounded in $C^{2,\mu}$ by a maximum-principle barrier and the [global Schauder estimate](#global-schauder-estimate). The [Arzelà-Ascoli theorem](topological-analysis.md#arzela-ascoli-theorem) gives convergence in $C^2$. A closed Hölder-norm constraint passes to the limit by [lower semicontinuity of a Hölder seminorm](sobolev-space.md#lower-semicontinuity-of-a-holder-seminorm), so the constrained solution set is compact rather than merely [relatively compact](topological-analysis.md#relatively-compact-subset).

###### Compactness proof of a nonnegative elliptic solution estimate

↑ **Parent:** [Global Schauder estimate](#global-schauder-estimate)

For a fixed [uniformly elliptic operator](#uniformly-elliptic-operator) with $C^{0,\mu}$ coefficients on a bounded smooth [connected](geometry-and-topology.md#connected-space) domain, nonnegative solutions with zero [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) satisfy the displayed estimate when $\Omega'$ is nonempty and compactly contained in $\Omega$. If it failed, normalize the global supremum to one. The forcing and the interior infimum then tend to zero. The [global Schauder estimate](#global-schauder-estimate) and [compact embedding of Hölder spaces](sobolev-space.md#compact-embedding-of-holder-spaces) produce a nonzero homogeneous limit with an interior zero, contradicting the [strong minimum principle for elliptic operators](#strong-minimum-principle-for-elliptic-operators). An arbitrary bounded zeroth-order coefficient is allowed: replace $c$ by $\min(c,0)$ for the positivity argument. Keeping global boundary control prevents the normalized maximum from disappearing in the limit.

#### Simon absorption lemma

↑ **Parent:** [Schauder estimates](#schauder-estimates)

The Simon absorption lemma turns a scale-local estimate containing a sufficiently small multiple of the same quantity on a larger ball into a uniform estimate. Its boundary form uses balls intersected with a half-space and is the covering step that absorbs local boundary Hölder seminorms.

### De Giorgi-Nash-Moser theorem

↑ **Parent:** [Uniformly elliptic operator](#uniformly-elliptic-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/De_Giorgi-Nash-Moser_theorem)

If $u\in W^{1,2}(B_1)$ weakly solves $D_i(a^{ij}D_ju)=0$ with bounded measurable uniformly elliptic coefficients, then $u$ is locally Hölder continuous. For $0<\theta<1$, some $\alpha\in(0,1)$ and $C$ depending only on the dimension, ellipticity bounds, and $\theta$ satisfy

$$
\|u\|_{C^{0,\alpha}(B_\theta)}\leq C\|u\|_{L^2(B_1)}.
$$

#### Compactness of normalized weak elliptic solutions

↑ **Parent:** [De Giorgi-Nash-Moser theorem](#de-giorgi-nash-moser-theorem)

For a fixed bounded measurable [uniformly elliptic operator](#uniformly-elliptic-operator) in divergence form, solutions bounded by one have uniform local [Caccioppoli inequalities](partial-differential-equation.md#caccioppoli-inequality) and [Hölder continuity](sobolev-space.md#holder-condition) estimates. A [diagonal subsequence argument](real-analysis.md#diagonal-subsequence-argument) yields a local weak $W^{1,2}$ limit, while the [Arzelà-Ascoli theorem](topological-analysis.md#arzela-ascoli-theorem) gives [uniform convergence](real-analysis.md#uniform-convergence) on a fixed smaller closed [Euclidean ball](functional-analysis.md#euclidean-ball). The weak equation passes to the limit because the coefficients are fixed and bounded. A global supremum normalization does not force the interior limit to be nonzero.

#### Moser iteration

↑ **Parent:** [De Giorgi-Nash-Moser theorem](#de-giorgi-nash-moser-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moser_iteration)

Moser iteration combines a [Caccioppoli inequality](partial-differential-equation.md#caccioppoli-inequality) with the [Sobolev embedding theorem](sobolev-space.md#sobolev-embedding-theorem) to raise an integrability exponent geometrically. On nested balls it turns an $L^p$ bound for a nonnegative subsolution of a uniformly elliptic divergence-form equation into a local supremum bound.

##### Moser product on geometric radii

↑ **Parent:** [Moser iteration](#moser-iteration)

For $q_i=2\alpha^i$, $r_i=1/2+2^{-i-1}$, a [uniform power gain for elliptic solutions](partial-differential-equation.md#uniform-power-gain-for-elliptic-solutions) bounds the successive norms by factors $[DR2^{i+2}]^{\alpha^{-i}}$. Their infinite product is

$$
(DR)^{\alpha/(\alpha-1)}2^{\alpha/(\alpha-1)^2+2\alpha/(\alpha-1)}.
$$

It is finite because both $\sum\alpha^{-i}$ and $\sum i\alpha^{-i}$ converge. Uniform control of the $L^{q_i}$ norms on $B_{1/2}$ then controls the [essential supremum](measure-theory.md#essential-supremum), by comparing with the measure of a set where the function exceeds the proposed bound. A constant independent of $q$ left outside the $2/q$ power at every step would instead give a divergent product.

##### Liouville theorem for integrable nonnegative elliptic subsolutions

↑ **Parent:** [Moser iteration](#moser-iteration)

For $n\geq3$, a nonnegative entire [weak subsolution](#weak-subsolution-of-a-divergence-form-elliptic-equation) of a bounded measurable uniformly elliptic divergence-form equation that belongs to $L^p(\mathbb R^n)$ for some $p>1$ is zero [almost everywhere](measure-theory.md#almost-everywhere). Rescaling the local [Moser iteration](#moser-iteration) estimate gives $\|u\|_{L^\infty(B_{R/2})}\leq CR^{-n/p}\|u\|_{L^p(B_R)}$. Let $R\to\infty$.

##### Weak Harnack inequality

↑ **Parent:** [Moser iteration](#moser-iteration)

The weak estimate for supersolutions is distinct from the sup-to-inf [Harnack inequality for uniformly elliptic divergence-form equations](#harnack-inequality-for-uniformly-elliptic-divergence-form-equations) for solutions.

For a nonnegative weak supersolution of a uniformly elliptic divergence-form equation, a positive $L^q$ mean on a ball is bounded by a constant times the infimum on a smaller concentric ball. The admissible exponent and constant depend only on dimension and the ellipticity bounds.

###### Propagation of zeros by the weak Harnack inequality

↑ **Parent:** [Weak Harnack inequality](#weak-harnack-inequality)

For a nonnegative [weak supersolution](#weak-supersolution-of-a-divergence-form-elliptic-equation) with zero forcing, the [Weak Harnack inequality](#weak-harnack-inequality) makes zero [essential infimum](real-analysis.md#essential-infimum) on an interior ball imply vanishing almost everywhere on that ball. An overlapping ball then has zero [essential infimum](real-analysis.md#essential-infimum) too. Chains of overlapping interior balls propagate the vanishing through a [connected](geometry-and-topology.md#connected-space) domain.

###### Oscillation decay estimate

↑ **Parent:** [Weak Harnack inequality](#weak-harnack-inequality)

For a weak solution of a uniformly elliptic divergence-form equation, local boundedness and the [Weak Harnack inequality](#weak-harnack-inequality) imply

$$
\operatorname{osc}_{B_r}u\leq\theta\operatorname{osc}_{B_{2r}}u
$$

for a universal $0<\theta<1$. Iteration gives local [Hölder continuity](sobolev-space.md#holder-condition).

<h6 id="inhomogeneous-oscillation-decay-implies-holder-continuity">Inhomogeneous oscillation decay implies Hölder continuity</h6>

↑ **Parent:** [Oscillation decay estimate](#oscillation-decay-estimate)

If the essential oscillation on concentric balls obeys $\omega(R/2)\leq\theta\omega(R)+AR^\alpha$ with $0<\theta<1$ and $\alpha>0$, dyadic iteration gives $\omega(r)\leq Cr^\mu$ for every $0<\mu<\min\{\alpha,-\log_2\theta\}$. The resulting decay gives a [Hölder continuous function](sobolev-space.md#holder-condition). Taking the exponent strictly below both decay rates avoids a logarithmic factor when the rates coincide.

###### Harnack inequality for uniformly elliptic divergence-form equations

↑ **Parent:** [Weak Harnack inequality](#weak-harnack-inequality)

A nonnegative weak solution of a uniformly elliptic divergence-form equation satisfies

$$
\sup_{B_r}u\leq C\inf_{B_r}u
$$

whenever a fixed larger concentric ball lies in the domain. Combine the subsolution bound from [Moser iteration](#moser-iteration) with the [Weak Harnack inequality](#weak-harnack-inequality) for supersolutions.

## Degenerate elliptic operator

↑ **Parent:** [Elliptic boundary value problem](elliptic-boundary-value-problem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Degenerate_elliptic_operator)

A degenerate elliptic operator has a positive semidefinite principal form that may lose positive definiteness at some points or jets. The [p-Laplacian](partial-differential-equation.md#p-laplacian) with $p>2$ degenerates where its solution has zero gradient.

### Sine-mode expansion for a quadratically degenerate elliptic equation

↑ **Parent:** [Degenerate elliptic operator](#degenerate-elliptic-operator)

For $u_{xx}+y^2u_{yy}=0$ with zero vertical-side values on $0<x<\pi$, the [Fourier coefficient](fourier-series.md#fourier-coefficient) $b_n(y)$ obeys the [Cauchy-Euler differential equation](differential-equation.md#cauchy-euler-equation) $y^2b_n^{\prime\prime}=n^2b_n$. Boundedness at $y=0$ removes the negative [indicial root](differential-equation.md#indicial-root), leaving $b_n(y)=A_ny^{(1+\sqrt{1+4n^2})/2}$. Bounded top coefficients give absolute convergence of the [Fourier sine series](fourier-series.md#fourier-sine-series) below the top boundary.

#### Forced zero trace at a quadratically degenerate boundary

↑ **Parent:** [Sine-mode expansion for a quadratically degenerate elliptic equation](#sine-mode-expansion-for-a-quadratically-degenerate-elliptic-equation)

For the bounded continuous solutions in the [sine-mode expansion for a quadratically degenerate elliptic equation](#sine-mode-expansion-for-a-quadratically-degenerate-elliptic-equation), every surviving mode tends to zero at $y=0$. The estimate $p_n^+>n$ bounds the absolute sum by a constant times $y/(1-y)$, uniformly in $x$. The lower boundary trace must therefore be zero. Continuous boundary data prescribing a nonzero lower trace and zero vertical sides are incompatible with the equation.

### Failure of a coercive Dirichlet estimate under degeneracy

↑ **Parent:** [Degenerate elliptic operator](#degenerate-elliptic-operator)

For $P=\partial_1^2+\partial_2^2$ in a three-dimensional domain, let $u_k=\phi(x_1,x_2)\chi(x_3)\sin(kx_3)$ with fixed smooth compact support. Then $\|Pu_k\|_2$ remains bounded whereas $\|u_k\|_{H^1}$ grows proportionally to $k$. Thus no uniform estimate $\|u\|_{H^1}\le C\|Pu\|_2$ holds. The missing third-direction coercivity, rather than boundary data, causes the failure.

## Method of continuity

↑ **Parent:** [Elliptic boundary value problem](elliptic-boundary-value-problem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Method_of_continuity)

The method of continuity joins an invertible operator to a target operator through a continuous family. Uniform a priori estimates make the set of invertible parameters both open and closed.

## Hopf lemma

↑ **Parent:** [Elliptic boundary value problem](elliptic-boundary-value-problem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hopf_lemma)

For $L=a^{ij}D_{ij}+b^iD_i$ with bounded coefficients and uniform ellipticity near a boundary point $y$ satisfying the [interior sphere condition](#interior-sphere-condition), suppose $u\in C^2(\Omega)\cap C^0(\Omega\cup\{y\})$ has $Lu\geq0$ and $u(x)<u(y)$ in a tangent [open ball](topology.md#open-ball). With $\mathbf n$ the outward [unit normal](differential-geometry.md#unit-normal) of that ball, $\liminf_{t\downarrow0}[u(y)-u(y-t\mathbf n)]/t>0$. Consequently the outward [normal derivative](differential-geometry.md#normal-derivative) is positive whenever it exists. The given boundary [continuity](calculus.md#continuous-function) alone does not assert that the derivative exists. The minimum version follows by applying this to $-u$; operators with a zeroth-order term require additional sign hypotheses.

### Hopf dichotomy with classical regularity away from the zero set

↑ **Parent:** [Hopf lemma](#hopf-lemma)

Let $v\leq0$ be $C^1$ on a connected domain and $C^2$ away from its zero set, with $\Delta v+v=0$ wherever $v<0$. If negative and zero points coexist, an interior [Euclidean ball](functional-analysis.md#euclidean-ball) in $\{v<0\}$ touches its zero set. On that [Euclidean ball](functional-analysis.md#euclidean-ball) $\Delta v=-v>0$, so the [Hopf boundary point lemma](#hopf-lemma) forces a nonzero derivative at an interior maximum, contrary to $Dv=0$. Thus $v$ is identically zero or strictly negative. Mere [Lipschitz continuity](real-analysis.md#lipschitz-continuity) does not suffice: $-\max\{\sin x_1,0\}$ on $(-1,1)^n$ has both negative and zero regions.

### Interior sphere condition

↑ **Parent:** [Hopf lemma](#hopf-lemma)

A domain satisfies the interior sphere condition at a boundary point if an [open ball](topology.md#open-ball) contained in the domain is tangent to its boundary there. It gives the local barrier geometry for the [Hopf boundary point lemma](#hopf-lemma). The condition at a single point suffices for the corresponding local derivative conclusion.

## ↑ Ancestors (5)

1. [Partial differential equation](partial-differential-equation.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (7)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-49.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-73.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-107.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-105.md#3/ii/solution)
- [Potential-vorticity inversion](geophysical-fluid-dynamics.md#potential-vorticity-inversion)
- [Small-data existence for a nonlinear elliptic Dirichlet problem](#small-data-existence-for-a-nonlinear-elliptic-dirichlet-problem)
- [Stratified quasi-geostrophic inversion](geophysical-fluid-dynamics.md#stratified-quasi-geostrophic-inversion)
