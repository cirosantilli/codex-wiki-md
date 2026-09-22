# Convex optimization

↑ **Parent:** [Mathematical optimization](mathematical-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convex_optimization)

Convex optimization minimizes a convex objective over a convex feasible set.

**Table of contents**

- [Pari-mutuel expected-return allocation](#pari-mutuel-expected-return-allocation)
- [Separation oracle](#separation-oracle)
  - [Path-constraint separation by shortest paths](#path-constraint-separation-by-shortest-paths)
- [Chambolle–Pock algorithm](#chambolle-pock-algorithm)
  - [Convergence of primal-dual hybrid gradient](#convergence-of-primal-dual-hybrid-gradient)
- [Convex positively one-homogeneous functional](#convex-positively-one-homogeneous-functional)
  - [Generalized eigenfunction in the forward-operator metric](#generalized-eigenfunction-in-the-forward-operator-metric)
- [Conic optimization](#conic-optimization)
  - [Farkas' lemma](#farkas-lemma)
    - [Robust infeasibility under uniform constraint relaxation](#robust-infeasibility-under-uniform-constraint-relaxation)
    - [Farkas certificate for linear inequalities](#farkas-certificate-for-linear-inequalities)
      - [Normalized integer Farkas infeasibility gap](#normalized-integer-farkas-infeasibility-gap)
  - [Interior-point method](#interior-point-method)
    - [Homogeneous self-dual embedding of a linear program](#homogeneous-self-dual-embedding-of-a-linear-program)
    - [Conic phase-I problem](#conic-phase-i-problem)
    - [Self-concordant barrier](#self-concordant-barrier)
      - [Logarithmically homogeneous barrier](#logarithmically-homogeneous-barrier)
        - [Legendre dual cone barrier](#legendre-dual-cone-barrier)
      - [Dikin ellipsoid](#dikin-ellipsoid)
      - [Central path](#central-path)
        - [Central-path Newton system](#central-path-newton-system)
  - [Conic dual problem](#conic-dual-problem)
  - [Completely positive optimization](#completely-positive-optimization)
  - [Copositive optimization](#copositive-optimization)
    - [Copositive reformulation of an orthant Rayleigh minimum](#copositive-reformulation-of-an-orthant-rayleigh-minimum)
- [Robust optimization](#robust-optimization)
  - [Robust linear optimization over the probability simplex](#robust-linear-optimization-over-the-probability-simplex)
  - [Polyhedral uncertainty set](#polyhedral-uncertainty-set)
- [Convex analysis](#convex-analysis)
  - [Infimal convolution](#infimal-convolution)
    - [Finite-valued infimal convolution](#finite-valued-infimal-convolution)
      - [Infimal-convolution dual subgradients](#infimal-convolution-dual-subgradients)
    - [Conjugate of an infimal convolution](#conjugate-of-an-infimal-convolution)
- [Proportional fairness](#proportional-fairness)
  - [Inactive routes in proportional fairness](#inactive-routes-in-proportional-fairness)
  - [Proportionally fair allocation on a four-cycle](#proportionally-fair-allocation-on-a-four-cycle)
    - [Opposite-route reduction for a proportionally fair four-cycle](#opposite-route-reduction-for-a-proportionally-fair-four-cycle)
  - [Weighted logarithmic utility](#weighted-logarithmic-utility)
- [Semidefinite programming](#semidefinite-programming)
  - [Semidefinite relaxation of binary quadratic optimization](#semidefinite-relaxation-of-binary-quadratic-optimization)
  - [Semidefinite relaxation of slab-constrained quadratic maximization](#semidefinite-relaxation-of-slab-constrained-quadratic-maximization)
    - [Rademacher rounding for a semidefinite relaxation](#rademacher-rounding-for-a-semidefinite-relaxation)
      - [Logarithmic approximation bound for slab-constrained quadratic maximization](#logarithmic-approximation-bound-for-slab-constrained-quadratic-maximization)
- [Water-filling algorithm](#water-filling-algorithm)
  - [Logarithmic water filling](#logarithmic-water-filling)
- [Coordinate descent](#coordinate-descent)
- [Convex conjugate](#convex-conjugate)
  - [Utility conjugate](#utility-conjugate)
    - [Dual differentiability with nonvanishing utility curvature](#dual-differentiability-with-nonvanishing-utility-curvature)
  - [Convex conjugate of x log x](#convex-conjugate-of-x-log-x)
  - [Biconjugate](#biconjugate)
  - [Affine covariance of the convex conjugate](#affine-covariance-of-the-convex-conjugate)
  - [Concave Legendre dual](#concave-legendre-dual)
    - [Lower conjugate](#lower-conjugate)
      - [Concave biconjugate](#concave-biconjugate)
    - [Inverse-flux quadratic bounds](#inverse-flux-quadratic-bounds)
  - [Convex conjugate of a constrained quadratic](#convex-conjugate-of-a-constrained-quadratic)
  - [Fenchel-Moreau theorem](#fenchel-moreau-theorem)
    - [Biconjugation as closed convexification](#biconjugation-as-closed-convexification)
  - [Fenchel–Young inequality](#fenchel-young-inequality)
    - [Fenchel–Young gap](#fenchel-young-gap)
- [Subdifferential](#subdifferential)
  - [Fermat rule for convex minimization](#fermat-rule-for-convex-minimization)
  - [Monotonicity of a convex subdifferential](#monotonicity-of-a-convex-subdifferential)
  - [Forward subgradient step](#forward-subgradient-step)
  - [Partial subdifferential](#partial-subdifferential)
  - [Subgradient inversion under convex conjugacy](#subgradient-inversion-under-convex-conjugacy)
  - [Subdifferential under scalar affine composition](#subdifferential-under-scalar-affine-composition)
  - [Subdifferential of the L1 norm](#subdifferential-of-the-l1-norm)
  - [Subdifferential sum rule](#subdifferential-sum-rule)
- [Absolutely one-homogeneous functional](#absolutely-one-homogeneous-functional)
  - [Generalized singular vector](#generalized-singular-vector)
  - [Euler identity for a convex one-homogeneous functional](#euler-identity-for-a-convex-one-homogeneous-functional)
  - [Eigenfunction of an absolutely one-homogeneous functional](#eigenfunction-of-an-absolutely-one-homogeneous-functional)
- [Stiemke theorem](#stiemke-theorem)
- [Projected gradient descent](#projected-gradient-descent)
  - [Projected subgradient method](#projected-subgradient-method)
  - [Averaged projected-gradient bound](#averaged-projected-gradient-bound)
- [Step size](#step-size)
- [Proximal operator](#proximal-operator)
  - [Radial soft thresholding](#radial-soft-thresholding)
  - [Banach-space proximal minimization](#banach-space-proximal-minimization)
  - [Proximal operator under affine rescaling](#proximal-operator-under-affine-rescaling)
  - [Moreau envelope](#moreau-envelope)
    - [Moreau envelope of the Euclidean norm](#moreau-envelope-of-the-euclidean-norm)
    - [Gradient of a Moreau envelope](#gradient-of-a-moreau-envelope)
    - [Moreau smoothing of a negative log-density](#moreau-smoothing-of-a-negative-log-density)
    - [Squared distance to a convex set](#squared-distance-to-a-convex-set)
      - [Conjugate of the squared distance to a convex set](#conjugate-of-the-squared-distance-to-a-convex-set)
  - [Moreau decomposition](#moreau-decomposition)
    - [Proximal operator of a support function](#proximal-operator-of-a-support-function)
  - [Proximal gradient method](#proximal-gradient-method)
    - [Alternating proximal-gradient operator](#alternating-proximal-gradient-operator)
      - [Implicit nonsmooth block in alternating proximal-gradient iteration](#implicit-nonsmooth-block-in-alternating-proximal-gradient-iteration)
      - [Mixed-point norm identity for alternating updates](#mixed-point-norm-identity-for-alternating-updates)
    - [Iterative soft-thresholding algorithm](#iterative-soft-thresholding-algorithm)
- [Subgradient method](#subgradient-method)
- [Log-sum-exp function](#log-sum-exp-function)
  - [Smooth maximum](#smooth-maximum)
- [Nesterov accelerated gradient method](#nesterov-accelerated-gradient-method)
- [Monotone operator](#monotone-operator)
  - [Cocoercivity](#cocoercivity)
    - [Baillon–Haddad theorem](#baillon-haddad-theorem)
  - [Resolvent of a monotone operator](#resolvent-of-a-monotone-operator)
  - [Maximal monotone operator](#maximal-monotone-operator)
  - [Nonexpansive mapping](#nonexpansive-mapping)
    - [Averaged operator](#averaged-operator)
      - [Browder convergence theorem for averaged operators](#browder-convergence-theorem-for-averaged-operators)
      - [Averaged-operator inequality](#averaged-operator-inequality)
  - [Firmly nonexpansive mapping](#firmly-nonexpansive-mapping)
  - [Proximal point algorithm](#proximal-point-algorithm)
    - [Douglas–Rachford method](#douglas-rachford-method)
      - [Product-space reformulation of convex feasibility](#product-space-reformulation-of-convex-feasibility)
    - [Preconditioned proximal point algorithm](#preconditioned-proximal-point-algorithm)
- [Primal-dual optimal point](#primal-dual-optimal-point)
- [Equality-constrained convex optimization](#equality-constrained-convex-optimization)
- [Proximal gradient methods for learning](#proximal-gradient-methods-for-learning)

## Pari-mutuel expected-return allocation

↑ **Parent:** [Convex optimization](convex-optimization.md)

For positive existing stakes $s_i$ and budget $b$, maximizing $\sum_i p_ix_i/(s_i+x_i)$ is equivalent to minimizing $\sum_i p_is_i/(s_i+x_i)$. A positive multiplier $\tau$ chosen so that $\sum_i x_i=b$ gives the displayed allocation. Each coordinate minimizes $p_is_i/(s_i+x)+\tau x$ on $x\ge0$, which proves global optimality by [Lagrangian sufficiency theorem](mathematical-optimization.md#lagrange-sufficiency-theorem). Its active set is ordered by $p_i/s_i$. Zero existing stakes require a separate payoff convention and can cause nonattainment; the positive-stake formula should not be extended through undefined ratios.

## Separation oracle

↑ **Parent:** [Convex optimization](convex-optimization.md)

A [separation oracle](#separation-oracle) either certifies that a supplied point belongs to a convex feasible set or returns a violated linear inequality whose half-space contains the whole feasible set. Its running time can be small even when the set has exponentially many defining inequalities. Together with rational encoding bounds and an outer bound, this permits [polynomial time](computer-science.md#polynomial-time) [ellipsoid method](mathematical-optimization.md#ellipsoid-method) feasibility and optimization.

### Path-constraint separation by shortest paths

↑ **Parent:** [Separation oracle](#separation-oracle)

After testing nonnegative edge coordinates and any explicit box or budget inequalities, treat those coordinates as lengths. A shortest path of length below one supplies a violated path inequality; a minimum length at least one certifies all path inequalities. If no source-to-target path exists, all those inequalities are vacuous. Thus a [polynomial time](computer-science.md#polynomial-time) [shortest path problem](graph-theory.md#shortest-path-problem) calculation separates an exponentially constrained [linear program](mathematical-optimization.md#linear-programming).

<h2 id="chambolle-pock-algorithm">Chambolle–Pock algorithm</h2>

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chambolle–Pock_algorithm)

For a [saddle point](analysis.md#saddle-point) problem $\min_u\max_v\{F(u)+\langle Du,v\rangle-G(v)\}$, one update ordering is

$$
u^{k+1}=\operatorname{prox}_{\tau F}(u^k-\tau D^*v^k),\qquad v^{k+1}=\operatorname{prox}_{\sigma G}(v^k+\sigma D(2u^{k+1}-u^k)).
$$

The [proximal operators](#proximal-operator) treat both nonsmooth convex terms, while the extrapolation $2u^{k+1}-u^k$ couples the primal and dual variables. The primal objective is $F(u)+G^*(Du)$, with $G^*$ the [convex conjugate](#convex-conjugate). A dual-first ordering is obtained by exchanging roles; consistent indexing is needed when comparing the formulas.

### Convergence of primal-dual hybrid gradient

↑ **Parent:** [Chambolle–Pock algorithm](#chambolle-pock-algorithm)

For proper [lower semicontinuous](calculus.md#lower-semicontinuity) [convex functions](real-analysis.md#convex-function) on finite-dimensional [Hilbert spaces](hilbert-space.md), a nonempty [saddle point](analysis.md#saddle-point) set, and constant positive steps satisfying the displayed inequality, the [primal-dual hybrid gradient method](#chambolle-pock-algorithm) with extrapolation parameter one converges to a saddle point. The strict condition controls the bilinear coupling by the [operator norm](continuous-dual-space.md#operator-norm). It does not remove the need for existence of a saddle point. The fixed-step theorem and assumptions are recalled in [Malitsky and Pock, A first-order primal-dual algorithm with linesearch, Section 1](https://arxiv.org/pdf/1608.08883).

## Convex positively one-homogeneous functional

↑ **Parent:** [Convex optimization](convex-optimization.md)

This is a [proper convex function](real-analysis.md#proper-convex-function) that has degree-one [positive homogeneity](real-analysis.md#positively-homogeneous-function-degree-one), with $J(0)=0$. It need not be even or nonnegative; linear functionals are examples. Its [subdifferential](#subdifferential) satisfies

$$
p\in\partial J(u)\iff \langle p,u\rangle=J(u)\ \text{and}\ \langle p,z\rangle\leq J(z)\ \text{for every }z.
$$

The two tests $z=0$ and $z=2u$ prove equality; the [subgradient inequality](real-analysis.md#subgradient-inequality) then gives the global upper bound. Conversely that bound and equality prove the subgradient condition. Hence a [subgradient](real-analysis.md#subgradient) at $u$ also supports every nonnegative multiple of $u$. Requiring $J(-u)=J(u)$ gives an [absolutely one-homogeneous functional](#absolutely-one-homogeneous-functional).

### Generalized eigenfunction in the forward-operator metric

↑ **Parent:** [Convex positively one-homogeneous functional](#convex-positively-one-homogeneous-functional)

A nonzero $u$ satisfying this relation, with $Ku\ne0$, generalizes the [eigenfunction of an absolutely one-homogeneous functional](#eigenfunction-of-an-absolutely-one-homogeneous-functional) to the quadratic geometry induced by the forward map. Pairing with $u$ yields $\lambda=J(u)/\|Ku\|^2$. With unit data norm it is a [generalized singular vector](#generalized-singular-vector). If $\lambda>0$, $0\leq\alpha\lambda\leq1$ and the exact data are $Ku$, the vector $(1-\alpha\lambda)u$ minimizes the quadratic [variational regularization](inverse-problem.md#variational-regularization) objective. Substitute its raywise [subgradient](real-analysis.md#subgradient) into the [subgradient optimality condition](real-analysis.md#subgradient-optimality-condition). Every minimizing branch has the same predicted data, and injectivity of $K$ gives equality of vectors. The [Bregman distance](inverse-problem.md#bregman-divergence) along this ray is zero even though the reconstruction is shrunk. For nonnegative $J$ the branch continues as $(1-\alpha\lambda)_+u$; nonnegativity supplies $0\in\partial J(0)$ for the threshold argument.

Background on these generalized singular vectors: [Benning and Burger, Ground States and Singular Vectors of Convex Variational Regularization Methods](https://arxiv.org/abs/1211.2057).

## Conic optimization

↑ **Parent:** [Convex optimization](convex-optimization.md)

Optimization of a [linear function](vector-space.md#linear-function) subject to affine constraints and membership in a [closed convex cone](mathematical-optimization.md#closed-convex-cone). Choosing the [positive semidefinite cone](mathematical-optimization.md#positive-semidefinite-cone) gives [semidefinite programming](#semidefinite-programming); other choices include [copositive optimization](#copositive-optimization) and [completely positive optimization](#completely-positive-optimization). [Dual cones](toric-geometry.md#dual-cone) produce scalar-product bounds on feasible objectives.

### Farkas' lemma

↑ **Parent:** [Conic optimization](#conic-optimization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Farkas'_lemma)

Exactly one of the two displayed systems is feasible. [Closedness of finitely generated cones](mathematical-optimization.md#closedness-of-finitely-generated-cones) and the [Fenchel-Moreau theorem](#fenchel-moreau-theorem) applied to a cone's [indicator functional](inverse-problem.md#indicator-functional-of-a-constraint-set) provide a proof through its polar cone. It yields a nonnegative multiplier certificate when a finite system of linear inequalities is inconsistent.

#### Robust infeasibility under uniform constraint relaxation

↑ **Parent:** [Farkas' lemma](#farkas-lemma)

Suppose a [linear program](mathematical-optimization.md#linear-programming) has a [Farkas' lemma](#farkas-lemma) certificate $\lambda\geq0$, $A^T\lambda\geq0$, $b^T\lambda=-1$. A purported [feasible point](mathematical-optimization.md#feasible-point) of $Ax\leq b+\varepsilon\mathbf1$, $x\geq0$ would imply $0\leq\lambda^TAx\leq-1+\varepsilon\sum_i\lambda_i$. Hence every relaxation below the displayed positive threshold remains infeasible. For rational inputs, bounds on the encoding length of a certificate supply the precision gap used by the [ellipsoid method](mathematical-optimization.md#ellipsoid-method).

#### Farkas certificate for linear inequalities

↑ **Parent:** [Farkas' lemma](#farkas-lemma)

Such a vector certifies that $Cx\leq d$ has no solution: the nonnegative weighted sum of the constraints would give $0\leq d^Ty<0$. Conversely, [Farkas' lemma](#farkas-lemma) supplies one whenever the system is inconsistent.

##### Normalized integer Farkas infeasibility gap

↑ **Parent:** [Farkas certificate for linear inequalities](#farkas-certificate-for-linear-inequalities)

Suppose $A,b$ have integer entries of absolute value at most $U\geq1$, $A$ has $n$ columns, and $Ax\geq b$ is infeasible. A [Farkas certificate for linear inequalities](#farkas-certificate-for-linear-inequalities) can be chosen with $\lambda\geq0$, $A^T\lambda=0$, $\mathbf1^T\lambda=1$ and the displayed lower bound. Normalize an infeasibility certificate to obtain the last equality, then maximize $b^T\lambda$ over the resulting compact [linear polyhedron](mathematical-optimization.md#linear-polyhedron). A maximizing [extreme point](mathematical-optimization.md#extreme-point) has at most $n+1$ positive entries: otherwise the augmented columns $(A_i^T,1)$ on its support would be dependent, allowing feasible perturbations in both directions. For its $k\leq n+1$ independent supported columns, select $k$ independent equations. [Cramer's rule](linear-algebra.md#cramer-s-rule) expresses the supported entries with a common nonzero integer determinant denominator. That determinant has absolute value at most $k!U^k\leq[(n+1)U]^{n+1}$. The positive value $b^T\lambda$ therefore has a positive integer numerator over a denominator of at most this size, proving the bound.

### Interior-point method

↑ **Parent:** [Conic optimization](#conic-optimization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interior-point_method)

An interior-point method solves constrained [mathematical optimization](mathematical-optimization.md) problems by maintaining variables in the interiors of their feasible cones or inequality domains. Barrier derivatives are defined there, and damped [Newton methods](mathematical-optimization.md#newton-s-method-in-optimization) keep subsequent iterates in their domains. A [central path](#central-path) gives a family of barrier-regularized optima whose duality gap approaches zero; a [conic phase-I problem](#conic-phase-i-problem) can supply a strict feasible starting point.

#### Homogeneous self-dual embedding of a linear program

↑ **Parent:** [Interior-point method](#interior-point-method)

For a [linear program](mathematical-optimization.md#linear-programming) $\min\{c^Tx:Ax=b,\ x\ge0\}$ and its [dual linear program](mathematical-optimization.md#dual-linear-program), write $e=\mathbf1$, $\bar b=b-Ae$, $\bar c=c-e$, and $\bar z=c^Te+1$. Introduce $x,s\ge0$, $\tau,\kappa,\theta,\rho\ge0$, and a free multiplier $\lambda$ satisfying

$$
Ax-b\tau+\bar b\theta=0,\quad
-A^T\lambda+c\tau-s-\bar c\theta=0,\quad
b^T\lambda-c^Tx-\kappa+\bar z\theta=0,\quad
-\bar b^T\lambda+\bar c^Tx-\bar z\tau+(n+1)\rho=0.
$$

The point $x=s=e$, $\tau=\kappa=\theta=\rho=1$, $\lambda=0$ is strictly positive in all constrained coordinates. Multiplying the first three equations by $\lambda^T,x^T,\tau$ respectively and adding gives the displayed identity. Minimizing $\theta$ has value zero: primal-dual optimal solutions or certificates from [Farkas' lemma](#farkas-lemma) give zero-$\theta$ solutions after selecting positive $\rho$ and scaling. At $\theta=0$, $\tau>0$ gives an optimal primal-dual pair by division by $\tau$, while $\kappa>0$ gives a primal infeasibility or dual infeasibility certificate. A point with $\tau=\kappa=0$ is not decisive; choosing a [relative interior](mathematical-optimization.md#relative-interior) point of the [optimal face of a linear program](mathematical-optimization.md#optimal-face-of-a-linear-program) avoids that degeneracy because the face contains a point with $\tau+\kappa>0$.

#### Conic phase-I problem

↑ **Parent:** [Interior-point method](#interior-point-method)

An auxiliary conic optimization problem searches for strict feasibility before following a [central path](#central-path). Given $e\in\operatorname{int}K$, minimizing $t$ subject to $Ax-b+te\in K$ and $t\geq-1$ has a strict feasible start for sufficiently large $t$. Any feasible solution with $t<0$ certifies $Ax-b\in\operatorname{int}K$. If the original problem is strictly feasible, a small negative $t$ is feasible. Equality constraints and dual feasibility require their corresponding auxiliary procedures.

#### Self-concordant barrier

↑ **Parent:** [Interior-point method](#interior-point-method)

A convex three-times differentiable barrier $F$ is self-concordant when

$$
|D^3F(x)[h,h,h]|\leq2\bigl(D^2F(x)[h,h]\bigr)^{3/2}.
$$

A barrier of parameter $\nu$ additionally satisfies $|DF(x)[h]|\leq\sqrt{\nu D^2F(x)[h,h]}$ and diverges at the domain boundary. Logarithmically homogeneous cone barriers satisfy $F(tx)=F(x)-\nu\log t$. The orthant barrier $-\sum_i\log x_i$ has parameter equal to the dimension, while the Lorentz-cone barrier $-\log(t^2-\|z\|^2)$ on $t>\|z\|$ has parameter two. Their Hessians define [Dikin ellipsoids](#dikin-ellipsoid) and control interior Newton steps.

##### Logarithmically homogeneous barrier

↑ **Parent:** [Self-concordant barrier](#self-concordant-barrier)

A cone barrier with this scaling law satisfies $\langle\nabla F(s),s\rangle=-\nu$ and $\nabla F(ts)=t^{-1}\nabla F(s)$. Therefore a [central path](#central-path) with $y=-\mu\nabla F(s)$ has primal-dual gap $\nu\mu$. A product of orthant and [Lorentz cone](mathematical-optimization.md#second-order-cone) canonical barriers adds their parameters.

###### Legendre dual cone barrier

↑ **Parent:** [Logarithmically homogeneous barrier](#logarithmically-homogeneous-barrier)

For a [logarithmically homogeneous barrier](#logarithmically-homogeneous-barrier) on a [proper cone](mathematical-optimization.md#proper-cone), the [convex conjugate](#convex-conjugate) with reversed argument defines a barrier on the interior [dual cone](toric-geometry.md#dual-cone). The inverse gradient relation makes $y=-\mu\nabla F(s)$ equivalent to $s=-\mu\nabla F_\dagger(y)$. This gives a joint primal-dual [central path](#central-path) without assuming the barrier is identical on a self-dual cone.

##### Dikin ellipsoid

↑ **Parent:** [Self-concordant barrier](#self-concordant-barrier)

For a nondegenerate [self-concordant barrier](#self-concordant-barrier), the open local Hessian ball

$$
\{x+h:h^\top\nabla^2F(x)h<1\}
$$

is contained in its barrier domain. This is the Dikin ellipsoid. It supplies a quantitative way to ensure that a damped [Newton method](mathematical-optimization.md#newton-s-method-in-optimization) stays interior, without relying on Euclidean distance to a possibly curved boundary.

##### Central path

↑ **Parent:** [Self-concordant barrier](#self-concordant-barrier)

For a strictly feasible primal-dual [conic optimization](#conic-optimization) problem and a logarithmically homogeneous barrier, the central path consists of solutions

$$
s=Ax-b\in\operatorname{int}K,\quad A^\top y=c,\quad y\in\operatorname{int}K^*,\quad y=-\mu\nabla F(s),\quad\mu>0.
$$

The primal-dual gap is $\langle s,y\rangle=\nu\mu$. Existence requires appropriate feasibility and boundedness hypotheses, rather than merely a full-rank constraint matrix. Linearizing these equations gives a [central-path Newton system](#central-path-newton-system).

###### Central-path Newton system

↑ **Parent:** [Central path](#central-path)

At a target barrier parameter $\mu$, let $r_p=Ax-b-s$, $r_d=A^\top y-c$, $r_c=y+\mu\nabla F(s)$. The Newton direction solves

$$
A\Delta x-\Delta s=-r_p,\quad A^\top\Delta y=-r_d,\quad\Delta y+\mu\nabla^2F(s)\Delta s=-r_c.
$$

Full column rank of $A$ and a positive-definite barrier Hessian give a positive-definite reduced matrix. Backtracking must keep both cone variables interior; solving the linear equations alone does not guarantee that a full step stays inside the cones.

### Conic dual problem

↑ **Parent:** [Conic optimization](#conic-optimization)

For $\min_x c^\top x$ subject to $Ax-b\in K$, the [Lagrangian dual problem](mathematical-optimization.md#lagrangian-dual-problem) is $\max_y b^\top y$ subject to $A^\top y=c$ and $y\in K^*$. At feasible primal-dual points, the gap is $\langle Ax-b,y\rangle\geq0$. A self-dual cone has $K^*=K$, but self-duality alone does not imply feasibility or [strong duality](mathematical-optimization.md#strong-duality).

### Completely positive optimization

↑ **Parent:** [Conic optimization](#conic-optimization)

[Conic optimization](#conic-optimization) using the [completely positive cone](mathematical-optimization.md#completely-positive-cone). For a real [symmetric matrix](linear-algebra.md#symmetric-matrix) $Q$, the trace-normalized program $\min\{\langle Q,X\rangle_F:X\in\operatorname{CP}_n,\ \operatorname{tr}X=1\}$ minimizes a weighted average of nonnegative-unit-vector [Rayleigh quotients](linear-operator-theory.md#rayleigh-quotient). The weights are the squared norms of the factors in $X=\sum_jx_jx_j^T$. Hence a minimizing rank-one factor attains the same value as the original orthant minimum.

### Copositive optimization

↑ **Parent:** [Conic optimization](#conic-optimization)

[Conic optimization](#conic-optimization) using the [copositive cone](mathematical-optimization.md#copositive-cone). The constraint $Q-\lambda I\in\operatorname{COP}_n$ supplies an exact reformulation of a [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) minimum on the [nonnegative orthant](mathematical-optimization.md#nonnegative-orthant). Exact conic formulation does not itself provide an efficient membership algorithm.

#### Copositive reformulation of an orthant Rayleigh minimum

↑ **Parent:** [Copositive optimization](#copositive-optimization)

Let $\alpha=\min\{x^TQx:x\geq0,\ \|x\|_2=1\}$ for a real [symmetric matrix](linear-algebra.md#symmetric-matrix) $Q$. Compactness gives attainment. Homogeneity shows $Q-\lambda I$ is a [copositive matrix](linear-algebra.md#copositive-matrix) exactly when $\lambda\leq\alpha$, proving

$$
\alpha=\max\{\lambda:Q-\lambda I\in\operatorname{COP}_n\}.
$$

Its [conic program](#conic-optimization) dual is the trace-normalized [completely positive optimization](#completely-positive-optimization) problem. A minimizing [vector](vector-space.md#vector) gives $X=xx^T$, which certifies equality and dual attainment directly. In general $\alpha$ differs from the unrestricted smallest [eigenvalue](linear-operator-theory.md#eigenvalue).

## Robust optimization

↑ **Parent:** [Convex optimization](convex-optimization.md)

Robust optimization chooses a decision while accounting for every parameter in a prescribed uncertainty set. A worst-case maximization takes the form $\sup_x\inf_{r\in\mathcal U}F(x,r)$ with the decision chosen before the uncertain parameter. With affine dependence on the uncertainty, the [support function](mathematical-optimization.md#support-function) and [linear programming duality](mathematical-optimization.md#linear-programming-duality) often replace the inner optimization by explicit constraints.

### Robust linear optimization over the probability simplex

↑ **Parent:** [Robust optimization](#robust-optimization)

Worst-case linear revenue over a [polyhedral uncertainty set](#polyhedral-uncertainty-set) is optimized by the linear program

$$
\max_{x,\alpha,\beta}\ r_0^Tx-\mathbf1^T(\alpha+\beta),\qquad x\in\Delta_n,\quad\alpha,\beta\ge0,\quad P^T(\alpha-\beta)=x.
$$

Here $\Delta_n$ is the [probability simplex](algebraic-topology.md#probability-simplex). Finite decisions are exactly its intersection with $\operatorname{range}P^T$. If this intersection is empty, all decisions have worst-case value $-\infty$ and the displayed linear program is infeasible; its supremum over the empty feasible set is also $-\infty$. Full column rank of $P$ suffices to make all simplex decisions finite.

### Polyhedral uncertainty set

↑ **Parent:** [Robust optimization](#robust-optimization)

A polyhedral uncertainty set is specified by finitely many linear inequalities. The displayed centered example is the inverse image of a box under a linear map. It is nonempty because it contains $r_0$, and contains every line $r_0+td$ with $d\in\ker P$. Consequently it need not be bounded when $P$ is rank deficient. Its [supremum norm](functional-analysis.md#supremum-norm) constraint is equivalent to $-\mathbf1\le P(r-r_0)\le\mathbf1$.

## Convex analysis

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convex_analysis)

[Convex analysis](#convex-analysis) studies [convex sets](mathematical-optimization.md#convex-set) and [convex functions](real-analysis.md#convex-function), including [epigraphs](calculus-of-variations.md#epigraph), [convex conjugates](#convex-conjugate) and [subdifferentials](#subdifferential).

### Infimal convolution

↑ **Parent:** [Convex analysis](#convex-analysis)

The [infimal convolution](#infimal-convolution) is $(E\mathbin\square F)(u)=\inf_v\{E(v)+F(u-v)\}$. It optimizes a decomposition of $u$ between two costs. It is [convex](real-analysis.md#convex-function) when both costs are [convex functions](real-analysis.md#convex-function), and its [convex conjugate](#convex-conjugate) is $E^*+F^*$ whenever the extended-real operations are well defined.

#### Finite-valued infimal convolution

↑ **Parent:** [Infimal convolution](#infimal-convolution)

If two nonnegative finite-valued [convex functions](real-analysis.md#convex-function) are defined on all of a finite-dimensional space, their [infimal convolution](#infimal-convolution) is finite, [convex](real-analysis.md#convex-function) and continuous everywhere. [Convex perturbation duality](mathematical-optimization.md#convex-perturbation-duality) then gives [strong duality](mathematical-optimization.md#strong-duality) and dual attainment at every argument. It does not require or imply attainment of the primal decomposition infimum.

##### Infimal-convolution dual subgradients

↑ **Parent:** [Finite-valued infimal convolution](#finite-valued-infimal-convolution)

Under the finite-valued assumptions, [subgradients](real-analysis.md#subgradient) of an [infimal convolution](#infimal-convolution) are obtained as its attained dual optimizers. Equivalently $z\in\partial(h^*+k^*)(p)$. Splitting the latter [subdifferential](#subdifferential) into two separate ones needs a [subdifferential sum rule](#subdifferential-sum-rule) qualification; solving the aggregate dual objective avoids that extra assumption.

#### Conjugate of an infimal convolution

↑ **Parent:** [Infimal convolution](#infimal-convolution)

For proper [convex functions](real-analysis.md#convex-function) whose [infimal convolution](#infimal-convolution) is well defined, $(f\mathbin\square g)^*=f^*+g^*$. The proof separates a supremum over independent variables after writing $x=u+y$. No attainment of the infimum is needed.

## Proportional fairness

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proportional_fairness)

A rate allocation is proportionally fair when the sum of proportional changes toward any feasible competitor is nonpositive. If route $r$ has $n_r$ identical active flows, this condition is $\sum_rn_r(\widetilde x_r-x_r)/x_r\leq0$ and is equivalent to maximizing [weighted logarithmic utility](#weighted-logarithmic-utility) subject to capacity constraints.

### Inactive routes in proportional fairness

↑ **Parent:** [Proportional fairness](#proportional-fairness)

When a route has zero active flows, its term is absent from [weighted logarithmic utility](#weighted-logarithmic-utility). Its aggregate allocation is taken to be zero; a per-flow rate on it has no operational meaning and need not be uniquely determined. One must not divide by its zero population. Empty-network and empty-group cases can therefore be treated separately while preserving uniqueness of active-flow rates.

### Proportionally fair allocation on a four-cycle

↑ **Parent:** [Proportional fairness](#proportional-fairness)

For the four routes consisting of adjacent pairs of a unit-capacity four-cycle, put $P=n_1+n_3$, $Q=n_2+n_4$, and $N=P+Q$. Every active route in the first group has total service $P/N$, and every active route in the second has total service $Q/N$. Its per-flow rate is this total divided by its active flow count.

#### Opposite-route reduction for a proportionally fair four-cycle

↑ **Parent:** [Proportionally fair allocation on a four-cycle](#proportionally-fair-allocation-on-a-four-cycle)

Write $z_r=n_rx_r$ for aggregate route service. The four resource constraints are all sums of one odd and one even route service, so they are equivalent to the displayed maximum constraint. For fixed maxima, increasing each active service to its group's maximum improves [weighted logarithmic utility](#weighted-logarithmic-utility). Maximizing $P\log p+Q\log q$ with $p+q\leq1$ gives $p=P/(P+Q)$ and $q=Q/(P+Q)$, where $P=n_1+n_3$, $Q=n_2+n_4$. Inactive routes are omitted; the same formula covers states where one group is empty.

### Weighted logarithmic utility

↑ **Parent:** [Proportional fairness](#proportional-fairness)

The utility $\sum_rn_r\log x_r$ sums logarithmic utilities over individual flows. Its first-order condition gives [proportional fairness](#proportional-fairness). Its negative is a [strictly convex function](real-analysis.md#strictly-convex-function) on active flow rates, giving uniqueness of those rates on a [convex set](mathematical-optimization.md#convex-set) of feasible allocations.

## Semidefinite programming

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semidefinite_programming)

A semidefinite program optimizes a [linear function](vector-space.md#linear-function) subject to equalities between [affine functions](vector-space.md#affine-function) and [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix) inequalities. It generalizes [linear programming](mathematical-optimization.md#linear-programming): a diagonal [matrix](vector-space.md#matrix) is a [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix) exactly when its diagonal entries are nonnegative. [Matrix trace](linear-algebra.md#matrix-trace) expresses the objective as $\langle C,X\rangle=\operatorname{tr}(CX)$ for real [symmetric matrices](linear-algebra.md#symmetric-matrix).

### Semidefinite relaxation of binary quadratic optimization

↑ **Parent:** [Semidefinite programming](#semidefinite-programming)

For real symmetric $A$, replace sign-vector lifts $xx^T$ by all [matrices](vector-space.md#matrix) in the [elliptope](mathematical-optimization.md#elliptope):

$$
\max_{X\succeq0,\ X_{ii}=1}\operatorname{tr}(AX).
$$

Every sign [vector](vector-space.md#vector) gives a feasible rank-one [matrix](vector-space.md#matrix) with the same objective, so the relaxed maximum is an upper bound. The omitted rank-one condition is substantive: an arbitrary feasible [Gram matrix](linear-algebra.md#gram-matrix) need not come from signs.

### Semidefinite relaxation of slab-constrained quadratic maximization

↑ **Parent:** [Semidefinite programming](#semidefinite-programming)

Replacing $xx^T$ by a general [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix) relaxes maximization of $\|x\|_2^2$ subject to $|a_i^Tx|\le1$. The relaxed value is an upper bound because $xx^T$ has trace $\|x\|_2^2$ and satisfies the same quadratic constraints. Both problems are unbounded if the $a_i$ fail to span the ambient space. If they span it, $H=\sum_i a_ia_i^T$ is positive definite and $\lambda_{\min}(H)\operatorname{tr}X\le\operatorname{tr}(HX)\le m$, proving boundedness and attainment of the relaxation.

#### Rademacher rounding for a semidefinite relaxation

↑ **Parent:** [Semidefinite relaxation of slab-constrained quadratic maximization](#semidefinite-relaxation-of-slab-constrained-quadratic-maximization)

Use an orthogonal [eigendecomposition](linear-operator-theory.md#spectral-decomposition) $X=V\Lambda V^T$ and a vector $\xi$ of independent [Rademacher random variables](probability-theory.md#rademacher-distribution). Because $\Lambda$ is diagonal and $\xi_j^2=1$, every sign vector gives $\|\widehat x\|_2^2=\operatorname{tr}X$, without taking an expectation. If the scaling denominator $M$ is positive, then $x$ satisfies every slab constraint and $\|x\|_2^2=\operatorname{tr}X/M^2$. Under spanning constraints and positive trace, $M>0$ automatically. A nonzero $\widehat x$ with $M=0$ instead certifies an unbounded direction.

##### Logarithmic approximation bound for slab-constrained quadratic maximization

↑ **Parent:** [Rademacher rounding for a semidefinite relaxation](#rademacher-rounding-for-a-semidefinite-relaxation)

For spanning slab normals, apply the [maximum of finitely many Rademacher linear forms](probability-theory.md#maximum-of-finitely-many-rademacher-linear-forms) bound to $u_i=(V\Lambda^{1/2})^Ta_i$, whose squared norms are $a_i^TXa_i\le1$. Some sign vector has scaling denominator squared at most $2\log(2m)$. [Rademacher rounding for a semidefinite relaxation](#rademacher-rounding-for-a-semidefinite-relaxation) then produces a feasible vector of squared norm at least the displayed fraction of the SDP optimum. This is an existence guarantee from the [probabilistic method](probabilistic-combinatorics.md#probabilistic-method).

## Water-filling algorithm

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Water-filling_algorithm)

A water-filling algorithm allocates a fixed resource among concave-return channels by choosing one Lagrange multiplier and setting each allocation to a thresholded expression. The multiplier is adjusted until the allocations sum to the resource budget.

### Logarithmic water filling

↑ **Parent:** [Water-filling algorithm](#water-filling-algorithm)

To maximize $\sum_i\log(\alpha_i+x_i)$ for positive baselines, nonnegative allocations and a positive budget $B$, the [KKT conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) equalize the shifted values on allocated coordinates. The unique water level solves $\sum_i(\tau-\alpha_i)_+=B$. Inactive coordinates have baselines at least the water level. [Strict convexity](real-analysis.md#strictly-convex-function) of the negative objective ensures uniqueness, and sorting the baselines gives an efficient [water-filling algorithm](#water-filling-algorithm).

## Coordinate descent

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coordinate_descent)

Coordinate descent minimizes an objective by repeatedly optimizing one coordinate, or one block of coordinates, while holding all others fixed. Exact coordinate minimization is especially simple for separable penalties and quadratic objectives.

## Convex conjugate

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convex_conjugate)

For a function $f$ on a real vector space, its convex conjugate is

$$
f^*(p)=\sup_x\{p\mathbin\cdot x-f(x)\}.
$$

When $f$ is differentiable and strictly convex, the maximizing point satisfies $p=\nabla f(x)$.

### Utility conjugate

↑ **Parent:** [Convex conjugate](#convex-conjugate)

For an increasing concave utility on positive wealth, its [utility conjugate](#utility-conjugate) uses the indicated supremum and is a [convex function](real-analysis.md#convex-function) of the positive price variable. If $F(x)=-U(x)$ on positive $x$, extended by infinity elsewhere, then $\widehat U(y)=F^*(-y)$. Under the [Inada conditions](utility-function.md#inada-conditions) its optimizer is the [inverse marginal utility](utility-function.md#inverse-marginal-utility), and its [derivative](calculus.md#derivative) is the negative of that optimizer. The sign convention is part of the definition.

#### Dual differentiability with nonvanishing utility curvature

↑ **Parent:** [Utility conjugate](#utility-conjugate)

For an increasing [strictly concave](real-analysis.md#strictly-concave-function) differentiable utility satisfying [Inada conditions](utility-function.md#inada-conditions), its utility conjugate has a unique optimizer $I(y)=(U')^{-1}(y)$ and [derivative](calculus.md#derivative) $-I(y)$. The dual is strictly decreasing and [strictly convex](real-analysis.md#strictly-convex-function). Twice [differentiability](analysis.md#differentiability) of the dual additionally follows when $U''$ exists and is strictly negative everywhere. [Strict concavity](real-analysis.md#strict-concavity) alone allows $U''$ to vanish and does not imply this additional assertion.

### Convex conjugate of x log x

↑ **Parent:** [Convex conjugate](#convex-conjugate)

For $f(x)=x\log x$ on $x>0$, strict convexity and the stationary condition $p=1+\log x$ give the displayed [convex conjugate](#convex-conjugate) for every real $p$. Biconjugation recovers $f$ on its original positive domain. Its closed extended-real extension has value zero at zero and infinity on negative arguments.

### Biconjugate

↑ **Parent:** [Convex conjugate](#convex-conjugate)

The [biconjugate](#biconjugate) of $f$ is the [convex conjugate](#convex-conjugate) of its [convex conjugate](#convex-conjugate):

$$
f^{**}(x)=\sup_p\{\langle p,x\rangle-f^*(p)\}.
$$

It is the supremum of all [affine minorants](real-analysis.md#affine-minorant). For a proper function with an affine minorant, the [Fenchel-Moreau theorem](#fenchel-moreau-theorem) identifies it with the closed convex envelope; a proper [lower semicontinuous](calculus.md#lower-semicontinuity) [convex function](real-analysis.md#convex-function) equals its biconjugate.

### Affine covariance of the convex conjugate

↑ **Parent:** [Convex conjugate](#convex-conjugate)

If $g(x)=\lambda f(x-x_0)-\mu$ with $\lambda>0$, substitution into the supremum defining the [convex conjugate](#convex-conjugate) gives

$$
g^*(p)=\lambda f^*(p/\lambda)+p^Tx_0+\mu.
$$

The positivity of $\lambda$ allows it to pass through the supremum without reversing it. Negative scaling need not obey this rule for the convex conjugate, even when a formal stationary-value transform does.

### Concave Legendre dual

↑ **Parent:** [Convex conjugate](#convex-conjugate)

For a differentiable strictly [concave function](real-analysis.md#concave-function) $f$ whose derivative is a bijection of $\mathbb R$, define

$$
g(z)=\inf_{s\in\mathbb R}\{zs-f(s)\}=zh(z)-f(h(z)),\qquad h=(f')^{-1}.
$$

The unique minimizing point is $h(z)$, and $g'=h$ follows by comparing minimizers at adjacent arguments, even when $h$ is not differentiable. This dual is concave and equals $-(-f)^*(-z)$ in terms of the [convex conjugate](#convex-conjugate). If $f''<0$, then $g''=1/f''(h)$. For $f(s)=cs-s^2/2$, $g(z)=-(z-c)^2/2$.

#### Lower conjugate

↑ **Parent:** [Concave Legendre dual](#concave-legendre-dual)

The [lower conjugate](#lower-conjugate) uses an infimum, unlike the supremum defining a [convex conjugate](#convex-conjugate). For any $F$, $F_*(\tau)=-(-F)^*(-\tau)$ and $F(e)\le\tau:e-F_*(\tau)$. The inequality is informative only when the [lower conjugate](#lower-conjugate) is finite. If the infimum is attained uniquely and the dual is differentiable, $DF_*(\tau)$ is its minimizing argument. This sign convention is useful for upper comparison-energy bounds.

##### Concave biconjugate

↑ **Parent:** [Lower conjugate](#lower-conjugate)

The [concave biconjugate](#concave-biconjugate) is an upper envelope of $F$, and equals $F$ for a proper closed [concave function](real-analysis.md#concave-function) under the usual duality hypotheses. It equals $-(-F)^{**}$ in terms of the ordinary [biconjugate](#biconjugate). If $e=DF_*(\tau)$, differentiability and concavity of $F_*$ imply $F_*(\tau)+F_{**}(e)=\tau:e$. For a finite differentiable dual the equality follows because $\tau$ minimizes $s:e-F_*(s)$.

#### Inverse-flux quadratic bounds

↑ **Parent:** [Concave Legendre dual](#concave-legendre-dual)

Suppose $f(0)=0$, $f'(0)=c$, $h=(f')^{-1}$ is differentiable, and $k_-<h'/2<k_+<0$. Then $h(c)=g(c)=0$ for the [concave Legendre dual](#concave-legendre-dual) $g$, and

$$
k_-\le\frac{h(z)}{2(z-c)}\le k_+\quad(z\ne c),\qquad k_-(z-c)^2\le g(z)\le k_+(z-c)^2.
$$

Integrate the derivative bounds from $c$ to $z$, then integrate $g'=h$. Multiplying the first inequality by a negative $z-c$ reverses both comparisons. A bound valid without cases is $|h(z)|\le-2k_-|z-c|$.

### Convex conjugate of a constrained quadratic

↑ **Parent:** [Convex conjugate](#convex-conjugate)

Maximize $px-x^2/2$ over $|x|\leq1$. The maximizer is $x=\max(-1,\min(p,1))$, giving the displayed [Huber loss](statistical-inference.md#huber-loss). The [indicator functional of a constraint set](inverse-problem.md#indicator-functional-of-a-constraint-set) is zero on the interval and infinity outside; it is not the zero-one indicator used in [measure theory](measure-theory.md).

### Fenchel-Moreau theorem

↑ **Parent:** [Convex conjugate](#convex-conjugate)

A proper lower-semicontinuous convex functional on a real [Banach space](banach-space.md) equals its biconjugate, with the canonical embedding in the bidual understood. One inequality follows from the [Fenchel–Young inequality](#fenchel-young-inequality); separation of a point below the closed convex epigraph gives the opposite inequality. This is the closed-convex analogue of recovering a function from all its affine supporting functions.

#### Biconjugation as closed convexification

↑ **Parent:** [Fenchel-Moreau theorem](#fenchel-moreau-theorem)

For a proper extended-real [function](function.md) with an [affine minorant](real-analysis.md#affine-minorant), [biconjugate](#biconjugate) gives its greatest lower-semicontinuous [convex](real-analysis.md#convex-function) minorant. Geometric separation of its [epigraph](calculus-of-variations.md#epigraph) turns containing [closed half-spaces](mathematical-optimization.md#closed-half-space) into affine lower bounds. Vertical half-spaces are recovered by adding multiples of a domain-separating inequality to one fixed affine minorant.

<h3 id="fenchel-young-inequality">Fenchel–Young inequality</h3>

↑ **Parent:** [Convex conjugate](#convex-conjugate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fenchel–Young_inequality)

For a proper convex function $f$ and its [convex conjugate](#convex-conjugate) $f^*$,

$$
f(x)+f^*(p)\geq p\mathbin\cdot x.
$$

Equality holds exactly when $p\in\partial f(x)$, or equivalently $x\in\partial f^*(p)$.

<h4 id="fenchel-young-gap">Fenchel–Young gap</h4>

↑ **Parent:** [Fenchel–Young inequality](#fenchel-young-inequality)

For a [proper convex function](real-analysis.md#proper-convex-function) $\Phi$ and its [convex conjugate](#convex-conjugate) $\Phi^*$, this gap is nonnegative by the [Fenchel–Young inequality](#fenchel-young-inequality). It vanishes exactly when $y\in\partial\Phi(x)$. Its integral against a [transport plan](mathematical-optimization.md#transport-plan) is the difference between the half-squared-distance cost and the value of the integrable [Kantorovich potentials](mathematical-optimization.md#kantorovich-potential) $u=|x|^2/2-\Phi$, $v=|y|^2/2-\Phi^*$.

## Subdifferential

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subdifferential)

For a convex function $f$, the subdifferential at $x$ is

$$
\partial f(x)=\{g:f(y)\geq f(x)+g^T(y-x)\text{ for every }y\}.
$$

The point $x$ minimizes $f$ exactly when $0\in\partial f(x)$.

### Fermat rule for convex minimization

↑ **Parent:** [Subdifferential](#subdifferential)

For a proper [convex function](real-analysis.md#convex-function) finite at $x$, global minimality is equivalent to $0\in\partial f(x)$. This follows immediately from the defining [subgradient inequality](real-analysis.md#subgradient-inequality). Combined with a [subdifferential sum rule](#subdifferential-sum-rule), it converts a convex minimization problem into an inclusion, for example the equation defining a [proximal operator](#proximal-operator).

### Monotonicity of a convex subdifferential

↑ **Parent:** [Subdifferential](#subdifferential)

Adding the two [subgradient inequalities](real-analysis.md#subgradient-inequality) for $p\in\partial f(x)$ and $q\in\partial f(y)$ gives

$$
\langle p-q,x-y\rangle\geq0.
$$

Thus the [subdifferential](#subdifferential) is a [monotone operator](#monotone-operator). This inequality proves uniqueness of its resolvent: two solutions of $z\in x+\tau\partial f(x)$ must coincide when $\tau>0$.

### Forward subgradient step

↑ **Parent:** [Subdifferential](#subdifferential)

For a [convex function](real-analysis.md#convex-function) and $\tau>0$, the forward step is the set-valued explicit update $F_{\tau f}(x)=\{x-\tau p:p\in\partial f(x)\}$. It reduces to the usual gradient step when differentiable. In contrast, a backward step uses a [subgradient](real-analysis.md#subgradient) at the new point and is the [proximal operator](#proximal-operator) for a proper closed convex function.

### Partial subdifferential

↑ **Parent:** [Subdifferential](#subdifferential)

For a convex scalar function $f(x,y)$, the partial subdifferential $\partial_y f(x,y)$ means the [subdifferential](#subdifferential) of $v\mapsto f(x,v)$ at $v=y$. It is not differentiation of a set-valued subdifferential. If this section is differentiable, the partial subdifferential is the singleton containing $\nabla_yf(x,y)$.

### Subgradient inversion under convex conjugacy

↑ **Parent:** [Subdifferential](#subdifferential)

For a proper lower-semicontinuous convex functional on a real [Hilbert space](hilbert-space.md), $p\in\partial J(u)$ means $\langle v,p\rangle-J(v)\leq\langle u,p\rangle-J(u)$ for all $v$. Taking the supremum gives equality in the [Fenchel–Young inequality](#fenchel-young-inequality): $J(u)+J^*(p)=\langle u,p\rangle$. Apply the same argument to $J^*$ and use the [Fenchel-Moreau theorem](#fenchel-moreau-theorem) $J^{**}=J$ to obtain the reciprocal [subgradient](real-analysis.md#subgradient) condition.

### Subdifferential under scalar affine composition

↑ **Parent:** [Subdifferential](#subdifferential)

For a finite [convex function](real-analysis.md#convex-function) $h:\mathbb R\to\mathbb R$, the [function](function.md) $f(x)=h(c^Tx+b)$ is [convex](real-analysis.md#convex-function). The [subgradient inequality](real-analysis.md#subgradient-inequality) gives $c\partial h(u)\subseteq\partial f(x)$, where $u=c^Tx+b$. Conversely, every [subgradient](real-analysis.md#subgradient) $g$ of $f$ annihilates $\ker c^T$, because $f$ is constant on lines in those directions. For $c\ne0$, write $g=cv$ and test the subgradient inequality at $y=x+(t-u)c/\|c\|_2^2$; this proves $v\in\partial h(u)$. For $c=0$, $f$ is constant and both sides are $\{0\}$ since a finite [convex](real-analysis.md#convex-function) [function](function.md) on the real line has a nonempty [subdifferential](#subdifferential) everywhere.

### Subdifferential of the L1 norm

↑ **Parent:** [Subdifferential](#subdifferential)

The [subdifferential](#subdifferential) of the [L1 norm](functional-analysis.md#l1-norm) consists of vectors $z$ with $z_j=\operatorname{sgn}(\beta_j)$ when $\beta_j\ne0$ and $z_j\in[-1,1]$ when $\beta_j=0$. These coordinate conditions give the [Karush-Kuhn-Tucker conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions) for [Lasso](probability-and-statistics.md#lasso) and [Square-root Lasso](probability-and-statistics.md#square-root-lasso).

### Subdifferential sum rule

↑ **Parent:** [Subdifferential](#subdifferential)

For proper convex functions under a standard relative-interior qualification,

$$
\partial(f+g)(x)=\partial f(x)+\partial g(x).
$$

In particular, if $f$ is differentiable at $x$, then $\partial(f+g)(x)=\nabla f(x)+\partial g(x)$.

## Absolutely one-homogeneous functional

↑ **Parent:** [Convex optimization](convex-optimization.md)

A functional $J$ is absolutely one-homogeneous when $J(cu)=|c|J(u)$ for every scalar $c$. For a convex such functional,

$$
p\in\partial J(u)
\quad\Longleftrightarrow\quad
\langle p,u\rangle=J(u)
\text{ and }
\langle p,v\rangle\leq J(v)\text{ for every }v.
$$

### Generalized singular vector

↑ **Parent:** [Absolutely one-homogeneous functional](#absolutely-one-homogeneous-functional)

Let $K:U\to V$ be a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) from a real [Banach space](banach-space.md) to a real [Hilbert space](hilbert-space.md), and let $J$ be a proper lower-semicontinuous convex [absolutely one-homogeneous functional](#absolutely-one-homogeneous-functional) on $U$. The normalization and source relation imply $\lambda=J(u_\lambda)$ by the [Euler identity for a convex one-homogeneous functional](#euler-identity-for-a-convex-one-homogeneous-functional). For the [norm](functional-analysis.md#norm) penalty $J(u)=\|u\|$ on a [Hilbert space](hilbert-space.md), its nonzero-point [subgradient](real-analysis.md#subgradient) is $u/\|u\|$. Hence $K^*Ku_\lambda=u_\lambda/\|u_\lambda\|^2$: $v=u_\lambda/\|u_\lambda\|$ is a [right singular vector](linear-algebra.md#right-singular-vector) with [singular value](linear-algebra.md#singular-value) $\sigma=1/\|u_\lambda\|$, and $Ku_\lambda$ is the corresponding [left singular vector](linear-algebra.md#left-singular-vector). Thus the definition recovers the ordinary operator singular-vector relation using the one-homogeneous norm penalty. Uniqueness of the vector from its data requires extra hypotheses on $K$ and $J$.

### Euler identity for a convex one-homogeneous functional

↑ **Parent:** [Absolutely one-homogeneous functional](#absolutely-one-homogeneous-functional)

For an [absolutely one-homogeneous functional](#absolutely-one-homogeneous-functional) $J$ that is convex and $p\in\partial J(u)$,

$$
J(u)=\langle p,u\rangle.
$$

The [subgradient inequality](real-analysis.md#subgradient-inequality) at zero gives $\langle p,u\rangle\geq J(u)$, and at $2u$ gives the reverse inequality. This is an Euler identity that needs no differentiability.

### Eigenfunction of an absolutely one-homogeneous functional

↑ **Parent:** [Absolutely one-homogeneous functional](#absolutely-one-homogeneous-functional)

A nonzero vector $f$ is an eigenfunction of an absolutely one-homogeneous convex functional $J$ with eigenvalue $\lambda$ when $\lambda f\in\partial J(f)$. This nonlinear analogue of an [eigenvector](linear-operator-theory.md#eigenvector) underlies exact shrinkage formulas for several variational flows and proximal maps.

## Stiemke theorem

↑ **Parent:** [Convex optimization](convex-optimization.md)

For a real matrix $P$, exactly one of the following holds: there is $\phi$ with $P\phi\geq0$ and $P\phi\ne0$, or there is $q>0$ with $P^Tq=0$. Separating $\operatorname{Im}P$ from the standard simplex proves the result; $q$ may then be normalized to sum to one.

This is an alternative related to [Farkas' lemma](#farkas-lemma). It is not the strict-primal Gordan alternative: for the column matrix $(1,0)^T$, a nonnegative nonzero primal vector exists, while a componentwise strictly positive one does not.

## Projected gradient descent

↑ **Parent:** [Convex optimization](convex-optimization.md)

For a convex set $C$ and a differentiable convex objective $F$, projected gradient descent uses

$$
x_{i+1}=\Pi_C(x_i-\eta\nabla F(x_i)).
$$

This is the [proximal gradient method](#proximal-gradient-method) when the nonsmooth term is the indicator of the feasible convex set, whose proximal operator is the metric projection.

### Projected subgradient method

↑ **Parent:** [Projected gradient descent](#projected-gradient-descent)

The projected subgradient method minimizes a possibly nonsmooth [convex function](real-analysis.md#convex-function) over a closed [convex set](mathematical-optimization.md#convex-set) $C$ by iterating $x_{i+1}=\Pi_C(x_i-t_i g_i)$ with $g_i\in\partial f(x_i)$. Nonexpansiveness of [Euclidean projection onto a convex set](mathematical-optimization.md#euclidean-projection-onto-a-convex-set) and the [subgradient inequality](real-analysis.md#subgradient-inequality) give its basic convergence bound.

### Averaged projected-gradient bound

↑ **Parent:** [Projected gradient descent](#projected-gradient-descent)

If $\|\nabla F(x_i)\|\leq G$ and $\|x_1-x_*\|\leq D$, then

$$
F\left(\frac1k\sum_{i=1}^kx_i\right)-F(x_*)
\leq\frac{D^2}{2\eta k}+\frac{\eta G^2}{2}.
$$

It follows by expanding the squared distance after each projected step, using nonexpansiveness of projection, summing the resulting inequalities, and applying convexity.

## Step size

↑ **Parent:** [Convex optimization](convex-optimization.md)

The step size of an iterative optimization algorithm controls the distance moved in one update. Convergence conditions balance sufficient progress against instability from steps that are too large.

## Proximal operator

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proximal_operator)

For a proper lower-semicontinuous convex function $f$, the proximal operator is $\operatorname{prox}_f(y)=\arg\min_x\{f(x)+\lVert x-y\rVert^2/2\}$. Its optimality condition is $y-x\in\partial f(x)$.

### Radial soft thresholding

↑ **Parent:** [Proximal operator](#proximal-operator)

The [proximal map](#proximal-operator) of $\tau\|\cdot\|_2$ sends $x$ to $(1-\tau/\|x\|_2)_+x$, with zero assigned at $x=0$. This removes vectors inside the radius-$\tau$ ball and shortens all larger vectors by a fixed radial distance. It is useful for groupwise sparsity.

### Banach-space proximal minimization

↑ **Parent:** [Proximal operator](#proximal-operator)

On a [Banach space](banach-space.md) one can define the set of minimizers of $E(x)+\|x-q\|^2/2$, but existence and uniqueness need additional geometry or coercivity hypotheses. The optimality condition is $0\in\partial E(x)+\mathcal J(x-q)$, with the [duality mapping](banach-space.md#duality-mapping) $\mathcal J=\partial(\|\cdot\|^2/2)$. The Hilbert completion-of-square shift by a dual vector does not generalize unchanged. On $(\mathbb R^2,\|\cdot\|_1)$ with $E(x)=x_1+x_2$ and $q=0$, every $x_1,x_2\leq0$ with $x_1+x_2=-1$ is a minimizer; the vector $(-1,-1)$ is not one.

### Proximal operator under affine rescaling

↑ **Parent:** [Proximal operator](#proximal-operator)

For a real [Hilbert space](hilbert-space.md), $E(x)=\alpha J(cx-y)+\langle x,z\rangle$, $\alpha>0$ and $c\ne0$, identify $z$ with its vector by the [Riesz representation theorem](hilbert-space.md#riesz-representation-theorem). Completing the square in $\|x-q\|^2/2+\langle x,z\rangle$ shifts the input to $q-z$. Substitute $v=cx-y$ and multiply by $c^2$ to obtain the displayed formula, valid also for negative $c$. If $c=0$ and $J(-y)<\infty$, the answer is $q-z$; if $J(-y)=\infty$, the objective is identically infinite and no proper proximal problem remains.

### Moreau envelope

↑ **Parent:** [Proximal operator](#proximal-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moreau_envelope)

The Moreau envelope of a proper closed convex function is

$$
M_tf(x)=\min_u\left\{f(u)+\frac1{2t}\|u-x\|^2\right\}.
$$

It is differentiable even when $f$ is not, with $\nabla M_tf(x)=[x-\operatorname{prox}_{tf}(x)]/t$ and $1/t$-Lipschitz gradient.

#### Moreau envelope of the Euclidean norm

↑ **Parent:** [Moreau envelope](#moreau-envelope)

For $r=\|x\|_2$, the [Moreau envelope](#moreau-envelope) of the [Euclidean norm](functional-analysis.md#euclidean-norm) is $r^2/(2\tau)$ when $r\leq\tau$ and $r-\tau/2$ otherwise. Its gradient is $x/\tau$ in the core and $x/r$ outside. The approximation error is between zero and $\tau/2$.

#### Gradient of a Moreau envelope

↑ **Parent:** [Moreau envelope](#moreau-envelope)

For proper [lower semicontinuous](calculus.md#lower-semicontinuity) [convex functions](real-analysis.md#convex-function), the [Moreau envelope](#moreau-envelope) has gradient $\nabla f_\tau=(I-\operatorname{prox}_{\tau f})/\tau$. This follows by [subgradient inversion under convex conjugacy](#subgradient-inversion-under-convex-conjugacy) and the quadratic conjugate. Firm nonexpansiveness of the proximal residual makes the gradient $1/\tau$-Lipschitz continuous.

#### Moreau smoothing of a negative log-density

↑ **Parent:** [Moreau envelope](#moreau-envelope)

For a [proper convex function](real-analysis.md#proper-convex-function) with [sequential lower semicontinuity](calculus.md#sequential-lower-semicontinuity) $U=-\log\mu$, form $U_\lambda(x)=\inf_y\{U(y)+\lambda\|x-y\|^2\}$ with $\lambda>0$. The [Moreau envelope](#moreau-envelope) theorem gives $\nabla U_\lambda(x)=2\lambda(x-\operatorname{prox}_{U/(2\lambda)}(x))$. If $e^{-U_\lambda}$ is integrable, it defines a smooth surrogate [probability density function](continuous-probability-distribution.md#probability-density-function). Infimizing the [logarithm](calculus.md#logarithm) of a [probability density function](continuous-probability-distribution.md#probability-density-function) with a positive quadratic penalty has the opposite sign and does not generally smooth it. For the [Laplace distribution](continuous-probability-distribution.md#laplace-distribution), that incorrect operation leaves $-\log2-|x|-1/(4\lambda)$, which is not differentiable at zero.

#### Squared distance to a convex set

↑ **Parent:** [Moreau envelope](#moreau-envelope)

For a nonempty closed convex set $C$, the squared-distance function is the [Moreau envelope](#moreau-envelope) of its [indicator functional of a constraint set](inverse-problem.md#indicator-functional-of-a-constraint-set). It is convex and differentiable with

$$
\nabla d_C(x)=x-P_Cx,
$$

and this gradient is one-Lipschitz.

##### Conjugate of the squared distance to a convex set

↑ **Parent:** [Squared distance to a convex set](#squared-distance-to-a-convex-set)

The [squared distance to a convex set](#squared-distance-to-a-convex-set) is the [infimal convolution](#infimal-convolution) of the set's [indicator functional of a constraint set](inverse-problem.md#indicator-functional-of-a-constraint-set) and the half-squared [Hilbert space](hilbert-space.md) [norm](functional-analysis.md#norm). Its [convex conjugate](#convex-conjugate) is the sum of the half-squared [norm](functional-analysis.md#norm) and the [support function](mathematical-optimization.md#support-function) of the set.

### Moreau decomposition

↑ **Parent:** [Proximal operator](#proximal-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moreau_decomposition)

For $t>0$, the generalized Moreau decomposition is $\operatorname{prox}_{tf}(y)=y-t\operatorname{prox}_{t^{-1}f^*}(y/t)$, where $f^*$ is the [convex conjugate](#convex-conjugate).

#### Proximal operator of a support function

↑ **Parent:** [Moreau decomposition](#moreau-decomposition)

For a nonempty closed convex set $C$, the [Moreau decomposition](#moreau-decomposition) and $\sigma_C^*=\iota_C$ give $\operatorname{prox}_{t\sigma_C}(y)=y-t\Pi_C(y/t)$.

### Proximal gradient method

↑ **Parent:** [Proximal operator](#proximal-operator)

The proximal gradient method minimizes $g+h$, where $g$ has an $L$-Lipschitz gradient and $h$ is convex with a tractable [proximal operator](#proximal-operator), by $x_{r+1}=\operatorname{prox}_{\alpha h}(x_r-\alpha\nabla g(x_r))$. A standard choice $0<\alpha\leq1/L$ gives objective error $O(1/r)$ in the general convex case.

This basic forward-backward update is one of the [proximal gradient methods for learning](#proximal-gradient-methods-for-learning).

#### Alternating proximal-gradient operator

↑ **Parent:** [Proximal gradient method](#proximal-gradient-method)

For a jointly smooth [convex function](real-analysis.md#convex-function) $f(x,y)$, update $y$ implicitly by its proximal minimization at fixed $x$, then update $x$ explicitly with the gradient at the mixed point $(x,y^+)$. The combined map is $(\tau L/2)$-averaged for $0<\tau L<2$, as follows by applying [cocoercivity](#cocoercivity) at two mixed points. Its fixed points are precisely the minimizers. If a minimizer exists, averaged iteration proves convergence.

##### Implicit nonsmooth block in alternating proximal-gradient iteration

↑ **Parent:** [Alternating proximal-gradient operator](#alternating-proximal-gradient-operator)

For $f(x,y)=h(x,y)+\phi(y)$, where $h$ is convex with an $L_h$-[Lipschitz gradient](numerical-analysis.md#lipschitz-gradient) and $\phi$ is convex, use a proximal $y$-step for the full section and an explicit $x$-step for $h$. Monotonicity of the two selected [subgradients](real-analysis.md#subgradient) of $\phi$ combines with [cocoercivity](#cocoercivity) of $\nabla h$ to make the full update firmly nonexpansive for $0<\tau L_h\leq1$. Existence of a minimizer then gives convergence, even though the full objective is not smooth.

##### Mixed-point norm identity for alternating updates

↑ **Parent:** [Alternating proximal-gradient operator](#alternating-proximal-gradient-operator)

For two mixed points with difference $(p,q)$ and gradient difference $(a,b)$, the input difference is $(p,q+\tau b)$ and the output difference is $(p-\tau a,q)$. Their squared-norm difference is $-2\tau(\langle p,a\rangle+\langle q,b\rangle)+\tau^2(\|a\|^2-\|b\|^2)$. This exact identity is a reusable way to prove averagedness without assuming the two block maps are individually nonexpansive.

#### Iterative soft-thresholding algorithm

↑ **Parent:** [Proximal gradient method](#proximal-gradient-method)

The iterative soft-thresholding algorithm applies the [proximal gradient method](#proximal-gradient-method) to $\|x\|_1+\tfrac12\|Ax-y\|_2^2$:

$$
x^{k+1}=S_\tau(x^k-\tau A^T(Ax^k-y)),\qquad0<\tau\le\|A\|_{2\to2}^{-2}.
$$

Here $S_\tau$ is coordinatewise [soft thresholding](probability-and-statistics.md#soft-thresholding). The objective is [convex](real-analysis.md#convex-function) and coercive, so iterates converge to a minimizer in finite dimensions; uniqueness requires additional hypotheses.

## Subgradient method

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subgradient_method)

The subgradient method minimizes a possibly nonsmooth [convex function](real-analysis.md#convex-function) by choosing $g_k\in\partial f(x_k)$ and iterating

$$
x_{k+1}=x_k-t_kg_k.
$$

If the [subgradients](real-analysis.md#subgradient) are bounded by $G$ and a minimizer is within distance $R$ of $x_0$, a suitable constant or diminishing [step size](#step-size) finds objective error at most $\epsilon$ in $O(R^2G^2/\epsilon^2)$ iterations.

## Log-sum-exp function

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Log-sum-exp_function)

For $z\in\mathbb R^m$ and $\beta>0$, the scaled log-sum-exp function is

$$
\operatorname{LSE}_\beta(z)
=\frac1\beta\log\sum_{i=1}^m e^{\beta z_i}.
$$

It is a smooth [convex function](real-analysis.md#convex-function) satisfying

$$
\max_i z_i\leq\operatorname{LSE}_\beta(z)
\leq\max_i z_i+\frac{\log m}{\beta}.
$$

### Smooth maximum

↑ **Parent:** [Log-sum-exp function](#log-sum-exp-function)

Composing the [log-sum-exp function](#log-sum-exp-function) with finitely many [affine functions](vector-space.md#affine-function) gives a differentiable approximation to their pointwise maximum. Increasing the inverse-temperature parameter $\beta$ reduces the uniform approximation error while increasing the [Lipschitz gradient](numerical-analysis.md#lipschitz-gradient) constant.

## Nesterov accelerated gradient method

↑ **Parent:** [Convex optimization](convex-optimization.md)

For a convex objective with an $L$-Lipschitz [gradient](calculus.md#gradient), Nesterov's accelerated gradient method reaches objective error $\delta$ in $O(\sqrt{LR^2/\delta})$ iterations when a minimizer lies within distance $R$ of the initial point.

This is an accelerated variant of [gradient descent](numerical-analysis.md#gradient-descent); it should not be identified with every first-order or proximal gradient method.

## Monotone operator

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monotone_operator)

An operator $F$ on an [inner product space](linear-algebra.md#inner-product-space) is monotone when

$$
\langle F(v)-F(w),v-w\rangle\geq0
$$

for every $v,w$. The [gradient](calculus.md#gradient) of every differentiable [convex function](real-analysis.md#convex-function) is monotone.

### Cocoercivity

↑ **Parent:** [Monotone operator](#monotone-operator)

An operator $G$ is $\beta$-cocoercive when $\langle Gz-Gw,z-w\rangle\geq\beta\|Gz-Gw\|^2$ with $\beta>0$. This strengthens monotonicity and implies a Lipschitz constant $1/\beta$ by the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). Gradient maps of smooth [convex functions](real-analysis.md#convex-function) provide an important converse through the [Baillon–Haddad theorem](#baillon-haddad-theorem).

<h4 id="baillon-haddad-theorem">Baillon–Haddad theorem</h4>

↑ **Parent:** [Cocoercivity](#cocoercivity)

On the whole Euclidean space, an $L$-[Lipschitz gradient](numerical-analysis.md#lipschitz-gradient) of a [convex function](real-analysis.md#convex-function) is $1/L$-cocoercive. Subtract the supporting affine function at one point, apply the [descent lemma](numerical-analysis.md#descent-lemma) to a gradient step at the other point, then interchange the points and add. The conclusion needs convexity but no second derivative.

### Resolvent of a monotone operator

↑ **Parent:** [Monotone operator](#monotone-operator)

For an operator $A$, its resolvent with step $\tau>0$ is $J_{\tau A}=(I+\tau A)^{-1}$. A [maximal monotone operator](#maximal-monotone-operator) has an everywhere-defined single-valued [firmly nonexpansive mapping](#firmly-nonexpansive-mapping) as its resolvent. For $A=\partial f$, the resolvent is the [proximal map](#proximal-operator) of $\tau f$. This monotone-operator resolvent uses a different convention from the spectral resolvent of a linear operator.

### Maximal monotone operator

↑ **Parent:** [Monotone operator](#monotone-operator)

A [monotone operator](#monotone-operator) is maximal when its graph has no proper enlargement that is still monotone. In Euclidean or Hilbert space, its [resolvent of a monotone operator](#resolvent-of-a-monotone-operator) is single-valued and everywhere defined for every positive step. Subdifferentials of proper [lower semicontinuous](calculus.md#lower-semicontinuity) [convex functions](real-analysis.md#convex-function) are fundamental examples.

### Nonexpansive mapping

↑ **Parent:** [Monotone operator](#monotone-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nonexpansive_mapping)

A mapping $T$ on a [normed vector space](functional-analysis.md#normed-vector-space) is nonexpansive when $\|T(v)-T(w)\|\leq\|v-w\|$ for every $v,w$.

#### Averaged operator

↑ **Parent:** [Nonexpansive mapping](#nonexpansive-mapping)

An operator is $\alpha$-averaged for $0<\alpha<1$ when $T=(1-\alpha)I+\alpha R$ for a [nonexpansive mapping](#nonexpansive-mapping) $R$. Averaging controls the update residual and enables fixed-point iteration. A [firmly nonexpansive mapping](#firmly-nonexpansive-mapping) is exactly a $1/2$-averaged operator.

##### Browder convergence theorem for averaged operators

↑ **Parent:** [Averaged operator](#averaged-operator)

In finite-dimensional Euclidean space, iterating an [averaged operator](#averaged-operator) with a nonempty fixed-point set converges in norm to a fixed point from every start. The [averaged-operator inequality](#averaged-operator-inequality) proves boundedness and a vanishing residual; compactness produces a fixed cluster point and [Fejér monotonicity](real-analysis.md#fejer-monotonicity) turns subsequential convergence into convergence of the full sequence. A fixed point must exist.

##### Averaged-operator inequality

↑ **Parent:** [Averaged operator](#averaged-operator)

The defining averaging representation is equivalent to $\|Tz-Tw\|^2\leq\|z-w\|^2-(1-\alpha)\|(I-T)z-(I-T)w\|^2/\alpha$. Expanding the norm of the convex combination proves both directions. Substituting a fixed point for $w$ gives [Fejér monotonicity](real-analysis.md#fejer-monotonicity) and summability of squared residuals.

### Firmly nonexpansive mapping

↑ **Parent:** [Monotone operator](#monotone-operator)

A mapping $T$ on an [inner product space](linear-algebra.md#inner-product-space) is firmly nonexpansive when

$$
\|T(v)-T(w)\|^2
\leq\langle T(v)-T(w),v-w\rangle.
$$

Every firmly nonexpansive mapping is [nonexpansive](#nonexpansive-mapping), and the resolvent of a maximal [monotone operator](#monotone-operator) is firmly nonexpansive.

### Proximal point algorithm

↑ **Parent:** [Monotone operator](#monotone-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proximal_point_algorithm)

The proximal point algorithm seeks a zero of a [monotone operator](#monotone-operator) $F$ by repeatedly applying its resolvent:

$$
w_{k+1}=(I+\lambda F)^{-1}w_k.
$$

For $F=\partial f$, this is iteration of a [proximal operator](#proximal-operator).

<h4 id="douglas-rachford-method">Douglas–Rachford method</h4>

↑ **Parent:** [Proximal point algorithm](#proximal-point-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Douglas–Rachford_method)

For two proximal maps $P_f,P_h$, define reflected maps $R_f=2P_f-I$ and $R_h=2P_h-I$. The Douglas--Rachford fixed-point map is

$$
T=\frac12(I+R_fR_h)=I-P_h+P_f(2P_h-I).
$$

Because reflected proximal maps are nonexpansive, $T$ is firmly nonexpansive.

##### Product-space reformulation of convex feasibility

↑ **Parent:** [Douglas–Rachford method](#douglas-rachford-method)

Finding a point in $\bigcap_{j=1}^\ell C_j$ is equivalent to intersecting the product $C_1\times\cdots\times C_\ell$ with the diagonal subspace in $(\mathbb R^n)^\ell$. Projection onto the product is componentwise, while projection onto the diagonal replaces every component by their average.

#### Preconditioned proximal point algorithm

↑ **Parent:** [Proximal point algorithm](#proximal-point-algorithm)

Given a [positive-definite matrix](linear-algebra.md#positive-definite-matrix) $M$, the preconditioned proximal point map is

$$
T=(M+F)^{-1}M.
$$

It is firmly nonexpansive in the weighted [inner product](linear-algebra.md#inner-product) $\langle v,w\rangle_M=\langle v,Mw\rangle$ whenever $F$ is [monotone](#monotone-operator).

## Primal-dual optimal point

↑ **Parent:** [Convex optimization](convex-optimization.md)

A primal-dual optimal point consists of a feasible solution of an optimization problem and a feasible solution of its [Lagrangian dual problem](mathematical-optimization.md#lagrangian-dual-problem) whose objective values agree. Under differentiability and suitable convexity, such points satisfy the [Karush-Kuhn-Tucker conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions).

## Equality-constrained convex optimization

↑ **Parent:** [Convex optimization](convex-optimization.md)

An equality-constrained convex optimization problem has the form

$$
\min_x f(x)\quad\text{subject to }Ax=b,
$$

where $f$ is [convex](real-analysis.md#convex-function) and the constraint is [affine](vector-space.md#affine-function). Its stationarity and feasibility equations can be combined into a monotone primal-dual operator.

## Proximal gradient methods for learning

↑ **Parent:** [Convex optimization](convex-optimization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proximal_gradient_methods_for_learning)

These methods optimize a smooth loss plus a term with a tractable proximal operator, such as a sparsity regularizer or a convex-set indicator. The basic [proximal gradient method](#proximal-gradient-method) combines a gradient step with a proximal step; projected gradient and accelerated variants are related members of the family.

## ↑ Ancestors (4)

1. [Mathematical optimization](mathematical-optimization.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (15)

- [Beckmann potential](queueing-theory.md#beckmann-potential)
- [Box-constrained TV-L1 denoising](inverse-problem.md#box-constrained-tv-l1-denoising)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-35.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-30.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-38.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3.md#21h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-325.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-213.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-348.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-205.md#6/a/solution)
- [Proximity time of translating line segments](mathematical-optimization.md#proximity-time-of-translating-line-segments)
- [Strong duality](mathematical-optimization.md#strong-duality)
