# Gradient descent

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gradient_descent)

[Gradient descent](gradient-descent.md) is an [iterative method](numerical-analysis.md#iterative-method) for minimizing a [differentiable function](analysis.md#differentiable-function) $f$: choose an initial [vector](vector-space.md#vector) $x_0$ and repeatedly move opposite its [gradient](multivariable-calculus.md#gradient).[§9.3, p. 466, Algorithm 9.3: negative-gradient direction and a separately chosen step size](mathematics-bibliography.md#convex-optimization-by-stephen-boyd-and-lieven-vandenberghe)

With a fixed positive [step size](convex-optimization.md#step-size) $\eta$, the update is

$$
x_{k+1}=x_k-\eta\nabla f(x_k),\qquad k=0,1,2,\ldots.
$$

The direction and the [step size](convex-optimization.md#step-size) play different roles: the [gradient](multivariable-calculus.md#gradient) supplies local information about increase, while $\eta$ determines how far that information is trusted. A varying [step size](convex-optimization.md#step-size) gives $\eta_k$ instead; [exact line search for a positive-definite quadratic](#exact-line-search-for-a-positive-definite-quadratic) chooses it by minimizing along the current direction.

Why is this the steepest direction? For a unit [vector](vector-space.md#vector) $v$ in the [Euclidean norm](normed-vector-space.md#euclidean-norm), the [directional derivative](multivariable-calculus.md#directional-derivative) is $\langle\nabla f(x),v\rangle$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bounds it below by $-\|\nabla f(x)\|_2$, attained by $v=-\nabla f(x)/\|\nabla f(x)\|_2$ when the [gradient](multivariable-calculus.md#gradient) is nonzero. This is steepest descent relative to the [Euclidean norm](normed-vector-space.md#euclidean-norm); changing the [norm](normed-vector-space.md#norm) can change the steepest direction. A finite step need not decrease $f$, because a [directional derivative](multivariable-calculus.md#directional-derivative) describes infinitesimal motion.

For the [quadratic form](quadratic-form.md) with linear term $F(x)=x^TAx/2-b^Tx$, assuming $A$ is a [symmetric matrix](linear-algebra.md#symmetric-matrix), the negative [gradient](multivariable-calculus.md#gradient) is the [linear-system residual](#linear-system-residual) $r=b-Ax$. Thus [gradient descent](gradient-descent.md) turns the [linear system](linear-algebra.md#system-of-linear-equations) $Ax=b$ into repeated residual corrections; a [positive-definite matrix](quadratic-form.md#positive-definite-matrix) makes its solution the unique [global minimum](analysis.md#global-minimum). This is useful when applying the [linear map](vector-space.md#linear-map) $x\mapsto Ax$ is affordable but directly solving the [linear system](linear-algebra.md#system-of-linear-equations) is costly.

The attraction is that a [gradient](multivariable-calculus.md#gradient) evaluation gives an entire update without solving a new [linear system](linear-algebra.md#system-of-linear-equations). The difficulty is choosing a [step size](convex-optimization.md#step-size) that progresses along gently curved directions without overshooting steep ones. [Fixed-step gradient descent on a positive-definite quadratic](#fixed-step-gradient-descent-on-a-positive-definite-quadratic) makes this tension exact: every [eigenvector](linear-operator-theory.md#eigenvector) direction has its own multiplier, determined by its [eigenvalue](linear-operator-theory.md#eigenvalue). The resulting [condition number](quadratic-form.md#condition-number) dependence explains why a narrow valley can slow even an inexpensive [iterative method](numerical-analysis.md#iterative-method).

The simplicity of the [gradient](multivariable-calculus.md#gradient) update and its sensitivity to the [condition number](quadratic-form.md#condition-number) of the [Hessian matrix](multivariable-calculus.md#hessian-matrix) are central practical features.[§9.3.1, pp. 466–468, and §9.3.2, p. 475, Conclusions: convergence and conditioning](mathematics-bibliography.md#convex-optimization-by-stephen-boyd-and-lieven-vandenberghe)

**Table of contents**

- [Residual growth in an indefinite steepest-descent iteration](#residual-growth-in-an-indefinite-steepest-descent-iteration)
- [Gradient descent preserves an eigenline for a cubic product](#gradient-descent-preserves-an-eigenline-for-a-cubic-product)
- [Epoch complexity](#epoch-complexity)
- [Optimization epoch](#optimization-epoch)
- [Fixed-step gradient descent on a positive-definite quadratic](#fixed-step-gradient-descent-on-a-positive-definite-quadratic)
  - [Optimal fixed step for quadratic gradient descent](#optimal-fixed-step-for-quadratic-gradient-descent)
- [Gradient ascent](#gradient-ascent)
- [Stochastic gradient descent](#stochastic-gradient-descent)
  - [Averaged stationarity bound for stochastic gradient descent](#averaged-stationarity-bound-for-stochastic-gradient-descent)
  - [Stochastic gradient noise floor](#stochastic-gradient-noise-floor)
  - [Projected stochastic gradient descent](#projected-stochastic-gradient-descent)
  - [Unbiased stochastic gradient](#unbiased-stochastic-gradient)
    - [Stochastic gradient second-moment identity](#stochastic-gradient-second-moment-identity)
- [Lipschitz gradient](#lipschitz-gradient)
  - [Block Lipschitz constant from coordinate smoothness](#block-lipschitz-constant-from-coordinate-smoothness)
  - [Coordinate derivative bound by Bregman divergence](#coordinate-derivative-bound-by-bregman-divergence)
  - [Coordinate Lipschitz continuity](#coordinate-lipschitz-continuity)
  - [Descent lemma](#descent-lemma)
- [Exact line search for a positive-definite quadratic](#exact-line-search-for-a-positive-definite-quadratic)
  - [Steepest-descent step size](#steepest-descent-step-size)
- [Conjugate gradient method](#conjugate-gradient-method)
  - [Spectral weighting of conjugate gradient error](#spectral-weighting-of-conjugate-gradient-error)
  - [Conjugate direction](#conjugate-direction)
    - [Finite termination of conjugate directions](#finite-termination-of-conjugate-directions)
  - [Conjugate gradient convergence bound](#conjugate-gradient-convergence-bound)
  - [Linear-system residual](#linear-system-residual)
    - [Linear-system residual norm](#linear-system-residual-norm)
  - [Conjugate-gradient residual orthogonality](#conjugate-gradient-residual-orthogonality)
  - [Preconditioned conjugate gradient method](#preconditioned-conjugate-gradient-method)
    - [Exact inverse-square-root preconditioner](#exact-inverse-square-root-preconditioner)
  - [Krylov subspace](#krylov-subspace)
    - [Generalized minimal residual method](#generalized-minimal-residual-method)
      - [One-step restarted GMRES stagnation example](#one-step-restarted-gmres-stagnation-example)
    - [Arnoldi iteration](#arnoldi-iteration)
      - [Lanczos algorithm](#lanczos-algorithm)
      - [Arnoldi decomposition](#arnoldi-decomposition)
    - [Krylov dimension from spectral components](#krylov-dimension-from-spectral-components)
  - [Finite termination of the conjugate gradient method](#finite-termination-of-the-conjugate-gradient-method)
- [Heavy-ball method](#heavy-ball-method)
  - [Heavy-ball residual recurrence](#heavy-ball-residual-recurrence)
  - [Heavy-ball error propagation matrix](#heavy-ball-error-propagation-matrix)
    - [Heavy-ball rate for a two-eigenvalue diagonal quadratic](#heavy-ball-rate-for-a-two-eigenvalue-diagonal-quadratic)

## Residual growth in an indefinite steepest-descent iteration

↑ **Parent:** [Gradient descent](gradient-descent.md)

For this nonsymmetric [matrix](vector-space.md#matrix), consider the formal residual update $r^+=r-(r^Tr)/(r^TAr)Ar$, with nonzero $r=(x,y)^T$. Put $D=2x^2-2xy-2y^2$ and $B=5x^2+4xy+3y^2$. Algebra gives $r^+=(B/D)(-y,x)^T$ when $D\ne0$. But $B+D=7(x+y/7)^2+6y^2/7>0$ and $B-D=3(x+y)^2+2y^2>0$. Hence $B>|D|$ and $\|r^+\|>\|r\|$ for every defined nonzero step. At $D=0$, the quotient is undefined. Thus the iteration cannot converge to zero [linear-system residual](#linear-system-residual) from any nonzero initial residual. This concrete divergence proof distinguishes failure of an algorithm from mere failure to meet a sufficient theorem's hypotheses.

## Gradient descent preserves an eigenline for a cubic product

↑ **Parent:** [Gradient descent](gradient-descent.md)

Let $A$ be real symmetric, let $b$ be a unit [eigenvector](linear-operator-theory.md#eigenvector) satisfying $Ab=\lambda b$, and use scalar [step sizes](convex-optimization.md#step-size) $\alpha_n$. The [gradient](multivariable-calculus.md#gradient) of the displayed [cubic polynomial](polynomial.md#cubic-polynomial) [function](function.md) is

$$
\nabla h(x)=2(x^Tb)Ax+(x^TAx)b.
$$

On the [eigenline](linear-operator-theory.md#eigenline), $\nabla h(tb)=3\lambda t^2b$, so a [gradient descent](gradient-descent.md) update remains on that same line and obeys the scalar recurrence in the title. Induction proves invariance for every iterate starting on the line, including an iterate that reaches zero. This is a statement about the geometry of the updates, not a convergence theorem: when $\lambda\ne0$, the restriction $h(tb)=\lambda t^3$ is unbounded below in one direction.

## Epoch complexity

↑ **Parent:** [Gradient descent](gradient-descent.md)

The number of [optimization epochs](#optimization-epoch) needed to meet a stated accuracy criterion. Comparisons must specify the work counted by an [optimization epoch](#optimization-epoch), the accuracy measure, and whether a random method is controlled in [expectation](expected-value.md) or with a stated [probability](probability-theory.md#probability). Counting coordinate [partial derivatives](multivariable-calculus.md#partial-derivative) is useful for comparing [randomized block coordinate descent](convex-optimization.md#randomized-block-coordinate-descent) with [gradient descent](gradient-descent.md), but need not match elapsed computation time.

```
Target: gradient-descent.bigb, under Stochastic gradient descent.
```

## Optimization epoch

↑ **Parent:** [Gradient descent](gradient-descent.md)

A unit of work corresponding to one full pass through the components used to measure an [iterative method](numerical-analysis.md#iterative-method). For [coordinate descent](convex-optimization.md#coordinate-descent) in $n$ coordinates, count $n$ coordinate [partial derivative](multivariable-calculus.md#partial-derivative) evaluations as an optimization epoch: updates on blocks of size $m$ require $n/m$ updates per optimization epoch. For [stochastic gradient descent](#stochastic-gradient-descent) on a finite sum of losses, a common different convention counts one evaluation of every loss component. The convention must be specified. Random sampling with replacement need not visit every component during one such unit of work.

```
Target: gradient-descent.bigb, under Gradient descent.
```

## Fixed-step gradient descent on a positive-definite quadratic

↑ **Parent:** [Gradient descent](gradient-descent.md)

Consider the original two-dimensional example

$$
f(x_1,x_2)=\frac12(x_1^2+9x_2^2),\qquad x_0=(2,1)^T,\qquad \nabla f(x)=(x_1,9x_2)^T.
$$

The [Hessian matrix](multivariable-calculus.md#hessian-matrix) is $A=\operatorname{diag}(1,9)$, a [symmetric matrix](linear-algebra.md#symmetric-matrix) and [positive-definite matrix](quadratic-form.md#positive-definite-matrix). Its [eigenvectors](linear-operator-theory.md#eigenvector) are the coordinate directions, its [eigenvalues](linear-operator-theory.md#eigenvalue) are $1$ and $9$, and its [Euclidean norm](normed-vector-space.md#euclidean-norm) [condition number](quadratic-form.md#condition-number) is $9$. The unique [global minimum](analysis.md#global-minimum) is $x_*=0$, so the error $e_k=x_k-x_*$ equals $x_k$. The [linear map](vector-space.md#linear-map) $I-\eta A$, with $I$ the [identity matrix](vector-space.md#identity-matrix), gives

$$
x_{1,k}=2(1-\eta)^k,\qquad x_{2,k}=(1-9\eta)^k.
$$

For $\eta=1/5=0.2$, the two coordinate error multipliers are $0.8$ and $-0.8$. Consequently $x_1=(1.6,-0.8)^T$, $x_2=(1.28,0.64)^T$, and the second coordinate changes sign at every step while both shrink. The [Euclidean norm](normed-vector-space.md#euclidean-norm) of the error contracts by $0.8$ each step. The objective gap, which we call the quadratic energy, contracts by its square:

$$
E_k=f(x_k)-f(x_*)=\frac{13}{2}\left(\frac{16}{25}\right)^k,\qquad E_0=6.5,\quad E_1=4.16,\quad E_2=2.6624.
$$

The [level sets](topology.md#level-set) of $f$ are [ellipses](euclidean-geometry.md#ellipse). Oscillation across their narrow direction is compatible with strictly decreasing energy.

<a id="image-original-gradient-descent-iterates-on-f-x-1-2-plus-9x-2-2-2-step-size-0-2-contracts-both-directions-whereas-0-25-expands-the-second"></a>
![](gradient-descent-quadratic-contour-iterates.png)

**[Figure 1](#image-original-gradient-descent-iterates-on-f-x-1-2-plus-9x-2-2-2-step-size-0-2-contracts-both-directions-whereas-0-25-expands-the-second). Original gradient descent iterates on $f=(x_1^2+9x_2^2)/2$: step size $0.2$ contracts both directions, whereas $0.25$ expands the second**.

For $\eta=1/4=0.25$, the coordinate error multipliers become $0.75$ and $-1.25$, giving $x_1=(1.5,-1.25)^T$. The first coordinate still tends to zero, but the second alternates and grows. Direct substitution gives

$$
E_k=2\left(\frac9{16}\right)^k+\frac92\left(\frac{25}{16}\right)^k,\qquad E_1=\frac{261}{32}=8.15625.
$$

Thus a larger positive [step size](convex-optimization.md#step-size) can turn a strictly [convex function](real-analysis.md#convex-function) into a divergent iteration. Energy and error are different quantities: coordinate errors carry signed multipliers, while each coordinate's contribution to energy carries the squared multiplier.

<a id="image-exact-constructed-quadratic-energy-histories-from-2-1-step-sizes-0-1-and-0-2-converge-while-0-25-diverges"></a>
![](gradient-descent-quadratic-energy-histories.png)

**[Figure 2](#image-exact-constructed-quadratic-energy-histories-from-2-1-step-sizes-0-1-and-0-2-converge-while-0-25-diverges). Exact constructed quadratic-energy histories from $(2,1)$: step sizes $0.1$ and $0.2$ converge, while $0.25$ diverges**.

For the general [quadratic form](quadratic-form.md) with linear term

$$
f(x)=\frac12x^TAx-b^Tx,\qquad A=A^T>0,\qquad x_*=A^{-1}b,
$$

the error obeys the same [linear map](vector-space.md#linear-map) $e_{k+1}=(I-\eta A)e_k$. The [spectral theorem for real symmetric matrices](linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) supplies an [orthonormal basis](inner-product.md#orthonormal-basis) of [eigenvectors](linear-operator-theory.md#eigenvector) $q_i$ with positive [eigenvalues](linear-operator-theory.md#eigenvalue) $\lambda_i$. Writing $e_0=\sum_i c_iq_i$ gives the exact solution and energy identity

$$
e_k=\sum_i c_i(1-\eta\lambda_i)^kq_i,\qquad
E_k=\frac12\sum_i\lambda_i c_i^2(1-\eta\lambda_i)^{2k}.
$$

Therefore convergence from every initial [vector](vector-space.md#vector) is equivalent to

$$
|1-\eta\lambda_i|<1\quad\text{for every }i,
\qquad\text{or equivalently}\qquad 0<\eta<\frac2{\lambda_{\max}}.
$$

At $\eta=2/\lambda_{\max}$, a nonzero error component along a largest-[eigenvalue](linear-operator-theory.md#eigenvalue) [eigenvector](linear-operator-theory.md#eigenvector) flips sign without shrinking. Above that threshold it grows. A particular start can still converge if it has zero components in every unstable direction; the interval is the condition for all starts. If $\rho=\max_i|1-\eta\lambda_i|<1$, then $\|e_k\|_2\leq\rho^k\|e_0\|_2$ and $E_k\leq\rho^{2k}E_0$. These bounds follow by summing the squared components in the [orthonormal basis](inner-product.md#orthonormal-basis).

### Optimal fixed step for quadratic gradient descent

↑ **Parent:** [Fixed-step gradient descent on a positive-definite quadratic](#fixed-step-gradient-descent-on-a-positive-definite-quadratic)

For a fixed [symmetric matrix](linear-algebra.md#symmetric-matrix) and [positive-definite matrix](quadratic-form.md#positive-definite-matrix) $A$, what positive [step size](convex-optimization.md#step-size) minimizes the largest coordinate error multiplier over all [eigenvector](linear-operator-theory.md#eigenvector) directions? Let $m=\lambda_{\min}>0$ and $L=\lambda_{\max}$. Since $|1-\eta\lambda|$ is a [convex function](real-analysis.md#convex-function) of $\lambda$, its maximum over the [eigenvalues](linear-operator-theory.md#eigenvalue) occurs at an endpoint:

$$
\rho(\eta)=\max\{|1-\eta m|,|1-\eta L|\}.
$$

Balance the two extremes by solving $1-\eta m=-(1-\eta L)$:

$$
\eta_* = \frac2{m+L},\qquad \rho_* = \frac{L-m}{L+m}=\frac{\kappa-1}{\kappa+1},\qquad \kappa=\frac Lm.
$$

Here $\kappa$ is the [Euclidean norm](normed-vector-space.md#euclidean-norm) [condition number](quadratic-form.md#condition-number) of $A$. This balance is optimal: for $\eta<\eta_*$ the endpoint $1-\eta m$ exceeds $\rho_*$, and for $\eta>\eta_*$ the endpoint $\eta L-1$ exceeds $\rho_*$. The optimal worst-case energy factor is $\rho_*^2$, rather than $\rho_*$. This optimizes a uniform one-step bound; a particular initial error supported on fewer [eigenvectors](linear-operator-theory.md#eigenvector) can have a different best [step size](convex-optimization.md#step-size).

In the example $m=1$, $L=9$, so $\eta_*=0.2$ and $\rho_*^2=0.64$. Both [eigenvalue](linear-operator-theory.md#eigenvalue) directions attain that energy factor, making the displayed history exact. The smaller [step size](convex-optimization.md#step-size) $0.1$ instead gives

$$
E_k=2(0.81)^k+\frac92(0.01)^k.
$$

Its first step reaches $E_1=1.665$, below $4.16$ for $\eta=0.2$, but subsequent progress is limited by the first direction's energy factor $0.81$. By $k=5$, the energies are approximately $0.69736$ and $0.69793$, respectively; by $k=6$, the $0.2$ iteration is ahead. A better first step need not yield a faster long-run history.

As the [condition number](quadratic-form.md#condition-number) grows, $\rho_*$ approaches one: stability in the direction of the largest [eigenvalue](linear-operator-theory.md#eigenvalue) forces small movement along the smallest-[eigenvalue](linear-operator-theory.md#eigenvalue) direction. This is a precise reason to improve scaling or use a method such as the [conjugate gradient method](#conjugate-gradient-method), rather than merely increasing the [step size](convex-optimization.md#step-size). When $m=L$, choosing $\eta=1/m$ eliminates every error component in one step.

## Gradient ascent

↑ **Parent:** [Gradient descent](gradient-descent.md)

[Gradient ascent](#gradient-ascent) seeks a maximum by stepping along the [gradient](multivariable-calculus.md#gradient) of a differentiable objective. It is [gradient descent](gradient-descent.md) applied to $-J$. Taylor expansion gives $J(x+\eta\nabla J)=J(x)+\eta\|\nabla J\|^2+O(\eta^2)$, so sufficiently small positive steps improve the objective when the [gradient](multivariable-calculus.md#gradient) is nonzero. Line search, projection onto admissible controls, and noise-aware [gradient](multivariable-calculus.md#gradient) estimates are common practical modifications; a local stationary result need not be globally optimal.

## Stochastic gradient descent

↑ **Parent:** [Gradient descent](gradient-descent.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stochastic_gradient_descent)

Stochastic gradient descent updates parameters using an unbiased or approximate gradient computed from one observation or a mini-batch rather than the complete data set.

### Averaged stationarity bound for stochastic gradient descent

↑ **Parent:** [Stochastic gradient descent](#stochastic-gradient-descent)

Suppose a fixed-[step size](convex-optimization.md#step-size) [stochastic gradient descent](#stochastic-gradient-descent) iteration satisfies

$$
\mathbb E[f(X^{j+1})\mid X^j]\leq f(X^j)-\frac1{2L}\|\nabla f(X^j)\|^2+\frac M{2L},
$$

and $f$ has a [global minimizer](analysis.md#global-minimizer) $x^*$. Taking [expectations](expected-value.md) and forming a [telescoping sum](arithmetic.md#telescoping-sum) proves the displayed bound with $\Delta_0=f(X^0)-f(x^*)$ and deterministic $X^0$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) then bounds the averaged, or the best, expected [gradient](multivariable-calculus.md#gradient) [Euclidean norm](normed-vector-space.md#euclidean-norm) by $\sqrt{M+2L\Delta_0/k}$. This is a guarantee of stationarity in the indicated senses, rather than a last-iterate convergence assertion. The additive $M$ is a [stochastic gradient noise floor](#stochastic-gradient-noise-floor).

```
Target: real-analysis.bigb, under Strongly convex function.
```

### Stochastic gradient noise floor

↑ **Parent:** [Stochastic gradient descent](#stochastic-gradient-descent)

A residual accuracy level in a bound for [stochastic gradient descent](#stochastic-gradient-descent) with a fixed [step size](convex-optimization.md#step-size) and nonvanishing [gradient](multivariable-calculus.md#gradient) noise. For a [convex function](real-analysis.md#convex-function) with an $L$-[Lipschitz gradient](#lipschitz-gradient), [step size](convex-optimization.md#step-size) $1/L$ and conditional total [variance](variance.md) at most $M$, typical bounds have floors $M$ for averaged squared [gradient](multivariable-calculus.md#gradient) norms, $\sqrt M$ for averaged [gradient](multivariable-calculus.md#gradient) norms, and $M/L$ for the best expected [objective function](mathematical-optimization.md#objective-function) gap. Such floors are upper bounds depending on the analysis and assumptions, rather than claims that these exact values are attained or that every last iterate converges.

```
Target: gradient-descent.bigb, under Stochastic gradient descent.
```

### Projected stochastic gradient descent

↑ **Parent:** [Stochastic gradient descent](#stochastic-gradient-descent)

Projected stochastic gradient descent takes a stochastic-gradient step and then projects the result onto a closed feasible set. For a convex set $C$ it has the form $x_{s+1}=\Pi_C(x_s-\eta_sG_s)$.

### Unbiased stochastic gradient

↑ **Parent:** [Stochastic gradient descent](#stochastic-gradient-descent)

A random vector $G_s$ is an unbiased stochastic gradient at $x_s$ when $\mathbb E[G_s\mid x_s]=\nabla f(x_s)$.

#### Stochastic gradient second-moment identity

↑ **Parent:** [Unbiased stochastic gradient](#unbiased-stochastic-gradient)

For an [unbiased stochastic gradient](#unbiased-stochastic-gradient) $H$ at $X$ with finite conditional second moment, expand $H=\nabla f(X)+(H-\nabla f(X))$ in the squared [Euclidean norm](normed-vector-space.md#euclidean-norm). The cross term has zero [conditional expectation](measure-theory.md#conditional-expectation), which proves the displayed identity. It separates the squared true [gradient](multivariable-calculus.md#gradient) from the total conditional [variance](variance.md) of its random estimate.

```
Target: gradient-descent.bigb, under Stochastic gradient descent.
```

## Lipschitz gradient

↑ **Parent:** [Gradient descent](gradient-descent.md)

A [differentiable function](analysis.md#differentiable-function) has a $\beta$-[Lipschitz gradient](#lipschitz-gradient) on a set $D$ if its [gradient](multivariable-calculus.md#gradient) satisfies [Lipschitz continuity](real-analysis.md#lipschitz-continuity) there:

$$
\|\nabla f(x)-\nabla f(y)\|_2\leq\beta\|x-y\|_2\qquad(x,y\in D),\quad \beta\geq0.
$$

All [norms](normed-vector-space.md#norm) here are the [Euclidean norm](normed-vector-space.md#euclidean-norm). The constant limits how fast the [gradient](multivariable-calculus.md#gradient) changes; it is not a bound on the magnitude of the [gradient](multivariable-calculus.md#gradient). For $f(x)=(x_1^2+9x_2^2)/2$, the [gradient](multivariable-calculus.md#gradient) is the [linear map](vector-space.md#linear-map) $x\mapsto\operatorname{diag}(1,9)x$. Its [operator norm](continuous-dual-space.md#operator-norm) is $9$, so $\beta=9$ works globally and is sharp by taking $x-y=(0,1)^T$. The [gradient](multivariable-calculus.md#gradient) itself is unbounded on the whole [Euclidean space](normed-vector-space.md#euclidean-norm).

If $f$ has a continuous [Hessian matrix](multivariable-calculus.md#hessian-matrix) on an open [convex set](convex-set.md) $D$ and $\|\nabla^2f(z)\|_2\leq\beta$ throughout $D$, integrate that [linear map](vector-space.md#linear-map) along the [line segment](convex-set.md#line-segment) from $x$ to $y$:

$$
\nabla f(y)-\nabla f(x)=\int_0^1\nabla^2f(x+t(y-x))(y-x)\,dt.
$$

The [operator norm](continuous-dual-space.md#operator-norm) bound proves the displayed [Lipschitz continuity](real-analysis.md#lipschitz-continuity). Convexity of the domain keeps the entire [line segment](convex-set.md#line-segment) inside it. Bounding the [Hessian matrix](multivariable-calculus.md#hessian-matrix) only at the endpoints is insufficient.

### Block Lipschitz constant from coordinate smoothness

↑ **Parent:** [Lipschitz gradient](#lipschitz-gradient)

For a continuously [differentiable](analysis.md#differentiable-function) [convex function](real-analysis.md#convex-function) on $\mathbb R^n$ with [coordinate Lipschitz continuity](#coordinate-lipschitz-continuity) constants $L_i$, its [block coordinate gradient](convex-optimization.md#block-coordinate-gradient) is [Lipschitz continuous](real-analysis.md#lipschitz-continuity) along each corresponding [coordinate subspace](vector-space.md#coordinate-subspace), with constant at most $S_{\mathcal B}=\sum_{i\in\mathcal B}L_i$.

To prove this without assuming a [Hessian matrix](multivariable-calculus.md#hessian-matrix), put $\delta_{\mathcal B}=\nabla_{\mathcal B}f(x)-\nabla_{\mathcal B}f(y)$. Sum the [coordinate derivative bound by Bregman divergence](#coordinate-derivative-bound-by-bregman-divergence) over the block, then repeat with $x,y$ interchanged and average:

$$
\|\delta_{\mathcal B}\|^2\leq S_{\mathcal B}\big(D_f(x,y)+D_f(y,x)\big)
=S_{\mathcal B}(\nabla f(x)-\nabla f(y))^T(x-y).
$$

If $x-y$ is supported in the block, the [dot product](inner-product.md#dot-product) uses only $\delta_{\mathcal B}$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and cancellation of its [Euclidean norm](normed-vector-space.md#euclidean-norm) give the result, including the zero case separately. Taking the full block supplies a global [Lipschitz gradient](#lipschitz-gradient) constant $\sum_iL_i$.

```
Target: convex-optimization.bigb, under Coordinate descent.
```

### Coordinate derivative bound by Bregman divergence

↑ **Parent:** [Lipschitz gradient](#lipschitz-gradient)

Suppose $f$ is a [differentiable](analysis.md#differentiable-function) [convex function](real-analysis.md#convex-function) with [coordinate Lipschitz continuity](#coordinate-lipschitz-continuity) constant $L_i>0$. Put $\phi(u)=D_f(u,y)=f(u)-f(y)-\nabla f(y)^T(u-y)$, the [Bregman divergence](inverse-problem.md#bregman-divergence) from the supporting [affine function](vector-space.md#affine-function) at $y$. The [subgradient inequality](real-analysis.md#subgradient-inequality) gives $\phi\geq0$, and its coordinate [Lipschitz constant](real-analysis.md#lipschitz-constant) is still $L_i$. The coordinate [descent lemma](#descent-lemma) with [step size](convex-optimization.md#step-size) $1/L_i$ yields

$$
0\leq\phi\left(x-\frac{\partial_i\phi(x)}{L_i}e_i\right)\leq\phi(x)-\frac{[\partial_i\phi(x)]^2}{2L_i}.
$$

Since $\partial_i\phi(x)=\partial_i f(x)-\partial_i f(y)$, rearrangement proves the bound. Continuous [differentiability](analysis.md#differentiability) suffices; a [Hessian matrix](multivariable-calculus.md#hessian-matrix) is unnecessary.

```
Target: gradient-descent.bigb, under Lipschitz gradient.
```

### Coordinate Lipschitz continuity

↑ **Parent:** [Lipschitz gradient](#lipschitz-gradient)

The displayed estimate, for all $x$ and real $t$, defines a coordinate [Lipschitz constant](real-analysis.md#lipschitz-constant) $L_i$ for the [partial derivative](multivariable-calculus.md#partial-derivative) in coordinate $i$. It implies the coordinate [descent lemma](#descent-lemma)

$$
f(x+te_i)\leq f(x)+t\partial_i f(x)+\frac{L_i}{2}t^2
$$

by the [fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus) and integration of the [Lipschitz continuity](real-analysis.md#lipschitz-continuity) estimate. Subtracting an [affine function](vector-space.md#affine-function) leaves these constants unchanged.

The apparently weaker estimate along the singleton negative [gradient](multivariable-calculus.md#gradient) direction is equivalent when every real [step size](convex-optimization.md#step-size) is allowed: if the initial [partial derivative](multivariable-calculus.md#partial-derivative) is nonzero, any displacement can be written $-\alpha\partial_i f(x)e_i$; if it is zero but the final [partial derivative](multivariable-calculus.md#partial-derivative) is nonzero, reverse the endpoints; if both vanish the estimate is trivial.

```
Target: gradient-descent.bigb, under Lipschitz gradient.
```

### Descent lemma

↑ **Parent:** [Lipschitz gradient](#lipschitz-gradient)

Suppose $f$ is a [differentiable function](analysis.md#differentiable-function) on an open [convex set](convex-set.md) $D\subseteq\mathbb R^n$ and has an $L$-[Lipschitz gradient](#lipschitz-gradient) there, in the [Euclidean norm](normed-vector-space.md#euclidean-norm). For $u,v\in D$, the [descent lemma](#descent-lemma) states

$$
f(v)\leq f(u)+\langle\nabla f(u),v-u\rangle+\frac L2\|v-u\|_2^2.
$$

A bounded continuous [Hessian matrix](multivariable-calculus.md#hessian-matrix) gives one sufficient route to this estimate.[§9.1.2, p. 461, equation (9.13): Hessian upper bound and quadratic upper estimate; §9.3.1, p. 466, equation (9.17): substitution of a negative-gradient step](mathematics-bibliography.md#convex-optimization-by-stephen-boyd-and-lieven-vandenberghe)

For a short proof, put $d=v-u$. The [fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus) along the [line segment](convex-set.md#line-segment) gives

$$
f(v)-f(u)-\langle\nabla f(u),d\rangle
=\int_0^1\langle\nabla f(u+td)-\nabla f(u),d\rangle\,dt.
$$

The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and the [Lipschitz gradient](#lipschitz-gradient) bound make the [integrand](integral.md#integrand) at most $Lt\|d\|_2^2$; its [integral](integral.md) is $L\|d\|_2^2/2$. This proof needs no assumption that $f$ is a [convex function](real-analysis.md#convex-function).

For the [gradient descent](gradient-descent.md) update $v=u-\eta\nabla f(u)$, provided $v\in D$, substitution yields

$$
f(v)\leq f(u)-\eta\left(1-\frac{L\eta}{2}\right)\|\nabla f(u)\|_2^2.
$$

For $L>0$ and $0<\eta<2/L$, this ensures strict decrease whenever the [gradient](multivariable-calculus.md#gradient) is nonzero. At $\eta=2/L$ it guarantees only nonincrease; the quadratic example has a nonshrinking alternating component at this endpoint. At $\eta=1/L$ the guaranteed decrease is $\|\nabla f(u)\|_2^2/(2L)$. A bound valid only on $D$ cannot justify a step leaving $D$.

If a fixed admissible [step size](convex-optimization.md#step-size) is used forever, every iterate stays in $D$, and $f(x_k)$ has a finite lower bound, summing this inequality shows $\sum_k\|\nabla f(x_k)\|_2^2<\infty$, hence $\nabla f(x_k)\to0$. That conclusion alone gives neither convergence of the iterates nor a [global minimum](analysis.md#global-minimum). For example, the smooth [polynomial](polynomial.md) $f(x)=x^4-x^2$ has $f'(0)=0$ and $f''(0)=-2$: [gradient descent](gradient-descent.md) started at zero never moves, although $f(1/\sqrt2)=-1/4<0$. On $D=(-1,1)$, $|f''(x)|\leq10$, so the [Lipschitz gradient](#lipschitz-gradient) hypothesis holds on this domain. [Convex functions](real-analysis.md#convex-function) and [strongly convex functions](real-analysis.md#strongly-convex-function) provide additional structure; the exact quadratic convergence result above uses a [positive-definite matrix](quadratic-form.md#positive-definite-matrix).

## Exact line search for a positive-definite quadratic

↑ **Parent:** [Gradient descent](gradient-descent.md)

For $f(x)=x^TAx/2-b^Tx$ with $A$ positive definite and residual $r=b-Ax$, exact line search along $r$ uses

$$
t=\frac{r^Tr}{r^TAr}.
$$

The objective error contracts by

$$
1-\frac{(r^Tr)^2}{(r^TA^{-1}r)(r^TAr)}
\leq 1-\frac{\lambda_{\min}(A)}{\lambda_{\max}(A)}.
$$

### Steepest-descent step size

↑ **Parent:** [Exact line search for a positive-definite quadratic](#exact-line-search-for-a-positive-definite-quadratic)

For a real [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) $A$ and nonzero [linear-system residual](#linear-system-residual) $r=b-Ax$, minimize $f(x+\alpha r)$ for $f(x)=x^TAx/2-b^Tx$. Differentiating with respect to $\alpha$ gives $-r^Tr+\alpha r^TAr=0$, yielding the displayed positive step. Positive definiteness makes it the unique minimum along the line. Applying the same quotient to a nonsymmetric or indefinite matrix is a formal iteration, but this minimization proof and its convergence consequences no longer apply.

## Conjugate gradient method

↑ **Parent:** [Gradient descent](gradient-descent.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugate_gradient_method)

For a [positive-definite matrix](quadratic-form.md#positive-definite-matrix) $A$, the conjugate gradient method chooses mutually $A$-conjugate search directions. Starting with $r_0=b-Ax_0$ and $p_0=r_0$, it uses

$$
\alpha_k=\frac{r_k^Tr_k}{p_k^TAp_k},\quad
x_{k+1}=x_k+\alpha_kp_k,\quad
r_{k+1}=r_k-\alpha_kAp_k,
$$

and $p_{k+1}=r_{k+1}+\beta_kp_k$ with  
$\beta_k=r_{k+1}^Tr_{k+1}/(r_k^Tr_k)$.

### Spectral weighting of conjugate gradient error

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)

For a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix), choose an orthonormal eigenbasis and write the exact solution as $x=\sum_i\alpha_iv_i$. Starting at zero, the [conjugate gradient method](#conjugate-gradient-method) chooses an admissible polynomial $p(0)=1$ of degree at most the iteration count that minimizes the displayed error. The weights depend on both the eigenvalues and the solution coefficients. For two eigenvalues $1,L$, the first polynomial is $1-\eta t$, with $\eta=(\alpha^2+\beta^2L^2)/(\alpha^2+\beta^2L^3)$. Comparable nonzero coefficients and large $L$ give $\eta\approx1/L$, so the high-eigenvalue error is removed first. A sufficiently tiny high-mode coefficient changes this behavior; the spectrum alone does not determine the first step.

### Conjugate direction

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)

Nonzero [vectors](vector-space.md#vector) are conjugate directions with respect to a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) $A$ when they are pairwise [orthogonal](inner-product.md#orthogonal-vectors) in the [inner product](inner-product.md) $\langle u,v\rangle_A=u^TAv$. They need not be [orthogonal](inner-product.md#orthogonal-vectors) in the ordinary Euclidean [inner product](inner-product.md). They are [linearly independent](vector-space.md#linear-independence): multiplying a vanishing [linear combination](vector-space.md#linear-combination) by $p_j^TA$ isolates its $j$th coefficient times $p_j^TAp_j>0$.

#### Finite termination of conjugate directions

↑ **Parent:** [Conjugate direction](#conjugate-direction)

Let $p_1,\ldots,p_n$ be [conjugate directions](#conjugate-direction) for a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) $A$. Starting from any $x_1$, minimize $x^TAx/2-b^Tx$ successively along those full lines, stopping early if the [linear-system residual](#linear-system-residual) $r_j=b-Ax_j$ vanishes. The [quadratic minimization along a line](polynomial.md#quadratic-minimization-along-a-line) uses $\alpha_j=p_j^Tr_j/(p_j^TAp_j)$ and gives $r_{j+1}=r_j-\alpha_jAp_j$.

This makes $p_j^Tr_{j+1}=0$. For $i<j$, conjugacy preserves $p_i^Tr_{j+1}=p_i^Tr_j$. By [mathematical induction](foundations-of-mathematics.md#mathematical-induction), $r_{j+1}$ is [orthogonal](inner-product.md#orthogonal-vectors) to all preceding search [vectors](vector-space.md#vector). The $n$ [conjugate directions](#conjugate-direction) are [linearly independent](vector-space.md#linear-independence) and hence form a [basis](vector-space.md#basis), so $r_{n+1}=0$. Thus the method reaches the unique solution of the [linear system](linear-algebra.md#system-of-linear-equations) in at most $n$ steps in exact arithmetic. The [conjugate gradient method](#conjugate-gradient-method) generates such directions without storing a complete prescribed [basis](vector-space.md#basis) in advance.

### Conjugate gradient convergence bound

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)

For a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) $H$, the [Conjugate gradient method](#conjugate-gradient-method) minimizes the error in the induced [weighted norm](inner-product.md#weighted-norm) over its affine [Krylov subspace](#krylov-subspace). Writing the error as $p(H)e_0$ gives

$$
\frac{\|e_k\|_H}{\|e_0\|_H}\leq\min_{\deg p\leq k,\ p(0)=1}\max_{\lambda\in[\lambda_{\min},\lambda_{\max}]}|p(\lambda)|.
$$

For $\lambda_{\min}<\lambda_{\max}$, choose the scaled [Chebyshev polynomial](numerical-analysis.md#chebyshev-polynomial) $p(\lambda)=T_k((\lambda_{\max}+\lambda_{\min}-2\lambda)/(\lambda_{\max}-\lambda_{\min}))/T_k((\lambda_{\max}+\lambda_{\min})/(\lambda_{\max}-\lambda_{\min}))$. On the spectral interval its numerator has absolute value at most one. With $\rho=(\sqrt\kappa+1)/(\sqrt\kappa-1)$, the denominator equals $(\rho^k+\rho^{-k})/2\geq\rho^k/2$. This proves the displayed bound. If the two endpoints coincide, $H$ is a positive scalar multiple of the identity and one iteration solves the system exactly.

### Linear-system residual

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)

The residual of an approximate solution $x$ of $Ax=b$ is $r=b-Ax$. It is the unbalanced right-hand side, while the solution error is $x_*-x=A^{-1}r$. The [conjugate gradient method](#conjugate-gradient-method) makes residuals orthogonal to successive [Krylov subspaces](#krylov-subspace).

#### Linear-system residual norm

↑ **Parent:** [Linear-system residual](#linear-system-residual)

The [norm](normed-vector-space.md#norm) of a [linear-system residual](#linear-system-residual), used to measure how closely an approximate solution satisfies its [linear system](linear-algebra.md#system-of-linear-equations). It differs from the solution-error norm $\|x_*-x\|$. Their relationship depends on the [matrix inverse](matrix-inverse.md) and the [condition number](quadratic-form.md#condition-number), so a small residual alone is not a scale-free relative-error guarantee.

### Conjugate-gradient residual orthogonality

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)

At iteration $m$ of the conjugate gradient method,

$$
x_m-x_0\in\mathcal K_m(A,r_0),
\qquad
r_m\perp\mathcal K_m(A,r_0),
$$

and $r_m$ itself lies in $\mathcal K_{m+1}(A,r_0)$. These Galerkin conditions imply finite termination once the Krylov subspace becomes invariant under $A$.

### Preconditioned conjugate gradient method

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)

A symmetric preconditioner transforms $Ax=b$ into

$$
PAP^T\widehat x=Pb,\qquad x=P^T\widehat x.
$$

The aim is to make the transformed positive-definite matrix have clustered eigenvalues while keeping application of $P$ inexpensive.

#### Exact inverse-square-root preconditioner

↑ **Parent:** [Preconditioned conjugate gradient method](#preconditioned-conjugate-gradient-method)

For a positive-definite matrix $A$, choosing $P=A^{-1/2}$ gives $PAP^T=I$, so conjugate gradients terminates in one step. Constructing or applying the exact inverse square root is generally as expensive as solving the original system.

### Krylov subspace

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Krylov_subspace)

The order-$k$ Krylov subspace generated by $A$ and $b$ is

$$
\mathcal K_k(A,b)=\operatorname{span}\{b,Ab,\ldots,A^{k-1}b\}.
$$

#### Generalized minimal residual method

↑ **Parent:** [Krylov subspace](#krylov-subspace)

With zero initial guess, the generalized minimal residual method minimizes the [Euclidean norm](normed-vector-space.md#euclidean-norm) of the [linear-system residual](#linear-system-residual) over each [Krylov subspace](#krylov-subspace). The [Arnoldi decomposition](#arnoldi-decomposition) reduces this to $\min_y\|\widetilde H_ky-\|b\|_2e_1\|_2$, followed by $x_k=Q_ky$. [Givens rotations](numerical-analysis.md#givens-rotation) solve the small problem in $O(k^2)$ operations once the decomposition is available. For an [invertible matrix](linear-algebra.md#invertible-matrix) $A$, the same iterate minimizes the error in the [weighted norm](inner-product.md#weighted-norm) induced by $A^TA$, because $\|Ax-b\|_2=\|x-x_*\|_{A^TA}$.

##### One-step restarted GMRES stagnation example

↑ **Parent:** [Generalized minimal residual method](#generalized-minimal-residual-method)

One step of restarted [GMRES](#generalized-minimal-residual-method) searches along the current residual. In the displayed nonsingular system, the first residual minimization is $\min_\alpha[(1-\alpha)^2+(1+\alpha)^2]$, whose minimizer is zero. Restarting then repeats the same problem forever and never moves. Unrestarted [GMRES](#generalized-minimal-residual-method) instead solves exactly at step two, since $b,Ab$ span the entire space. Thus a smaller search-space cost can come at the price of stagnation; nonsingularity alone does not guarantee progress for one-step restarting.

#### Arnoldi iteration

↑ **Parent:** [Krylov subspace](#krylov-subspace)

Starting with $q_1=b/\|b\|_2$, the Arnoldi iteration constructs an [orthonormal basis](inner-product.md#orthonormal-basis) of successive [Krylov subspaces](#krylov-subspace). At step $j$, orthogonalize $Aq_j$ against $q_1,\ldots,q_j$, and normalize the remainder as $q_{j+1}$ if it is nonzero. The coefficients form an [upper Hessenberg matrix](vector-space.md#upper-hessenberg-matrix) $\widetilde H_k$ and satisfy $AQ_k=Q_{k+1}\widetilde H_k$. A zero remainder means the current [Krylov subspace](#krylov-subspace) is invariant under $A$.

##### Lanczos algorithm

↑ **Parent:** [Arnoldi iteration](#arnoldi-iteration)

For a real [symmetric matrix](linear-algebra.md#symmetric-matrix) $A$, the leading block $Q_k^TAQ_k$ of the [Arnoldi decomposition](#arnoldi-decomposition) is both symmetric and an [upper Hessenberg matrix](vector-space.md#upper-hessenberg-matrix), hence a [tridiagonal matrix](vector-space.md#tridiagonal-matrix). The resulting three-term recurrence is the Lanczos algorithm. If $A$ is a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix), its compression is too, since $y^TQ_k^TAQ_ky=(Q_ky)^TA(Q_ky)>0$ for nonzero $y$.

##### Arnoldi decomposition

↑ **Parent:** [Arnoldi iteration](#arnoldi-iteration)

The factorization produced by the [Arnoldi iteration](#arnoldi-iteration), with [orthonormal](inner-product.md#orthonormal-set) $Q_{k+1}$ and an [upper Hessenberg matrix](vector-space.md#upper-hessenberg-matrix) $\widetilde H_k$. Multiplying by $Q_k^T$ identifies its leading square block as $H_k=Q_k^TAQ_k$.

#### Krylov dimension from spectral components

↑ **Parent:** [Krylov subspace](#krylov-subspace)

For a [diagonalizable](linear-operator-theory.md#diagonalizable-matrix) finite-dimensional operator, write $v=\sum_j u_j$ with nonzero $u_j$ in distinct [eigenspaces](linear-operator-theory.md#eigenspace) of eigenvalues $\lambda_j$. Then $A^rv=\sum_j\lambda_j^ru_j$. The [Vandermonde matrix](galois-theory.md#vandermonde-matrix) of the first $k$ powers is invertible for $k$ distinct eigenvalues, so these powers span exactly the $k$ independent components $u_j$. Thus the stabilized [Krylov subspace](#krylov-subspace) dimension is $k$. It counts distinct spectral components, not the number of nonzero coefficients in an arbitrary eigenbasis: $A=I$, $v=e_1+e_2$ has Krylov dimension one. Equivalently it is the minimum number of eigenvectors needed when those vectors may be chosen freely.

### Finite termination of the conjugate gradient method

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)

In exact arithmetic, conjugate gradients reaches the exact solution in at most the number of distinct eigenvalues of $A$, and therefore in at most $n$ steps for an $n$-dimensional system.

## Heavy-ball method

↑ **Parent:** [Gradient descent](gradient-descent.md)

The heavy-ball iteration adds momentum to gradient descent:

$$
x_{k+1}=x_k-\alpha\nabla F(x_k)+\beta(x_k-x_{k-1}).
$$

### Heavy-ball residual recurrence

↑ **Parent:** [Heavy-ball method](#heavy-ball-method)

For $F(x)=x^TAx/2-b^Tx$ and $r_k=b-Ax_k$,

$$
r_{k+1}=((1+\beta)I-\alpha A)r_k-\beta r_{k-1}.
$$

Thus $r_k$ is a polynomial in $A$ applied to the initial residual and lies in the corresponding [Krylov subspace](#krylov-subspace).

### Heavy-ball error propagation matrix

↑ **Parent:** [Heavy-ball method](#heavy-ball-method)

For $e_k=x^*-x_k$,

$$
\binom{e_{k+1}}{e_k}
=
\begin{pmatrix}
(1+\beta)I-\alpha A&-\beta I\\
I&0
\end{pmatrix}
\binom{e_k}{e_{k-1}}.
$$

If $A$ is diagonal with entries $\lambda_i$, a coordinate permutation turns this matrix into blocks

$$
\begin{pmatrix}1+\beta-\alpha\lambda_i&-\beta\\1&0\end{pmatrix}.
$$

#### Heavy-ball rate for a two-eigenvalue diagonal quadratic

↑ **Parent:** [Heavy-ball error propagation matrix](#heavy-ball-error-propagation-matrix)

For $A=\operatorname{diag}(1,\gamma)$, $\alpha=1/\gamma$, and $\beta=(1-\gamma^{-1/2})^2$, every error-propagation block has spectral radius at most $1-\gamma^{-1/2}$, and equality occurs.

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (31)

- [Delta rule](statistical-learning.md#delta-rule)
- [Derivative](calculus.md#derivative)
- [Descent lemma](#descent-lemma)
- [Epoch complexity](#epoch-complexity)
- [Fixed-step gradient descent on a positive-definite quadratic](#fixed-step-gradient-descent-on-a-positive-definite-quadratic)
- [Gradient](multivariable-calculus.md#gradient)
- [Gradient ascent](#gradient-ascent)
- [Gradient descent](gradient-descent.md)
- [Gradient descent preserves an eigenline for a cubic product](#gradient-descent-preserves-an-eigenline-for-a-cubic-product)
- [Nesterov accelerated gradient method](convex-optimization.md#nesterov-accelerated-gradient-method)
- [Nonlinear programming](mathematical-optimization.md#nonlinear-programming)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#15/d/solution)
- [Solution](past-exam-of-the-computational-neuroscience-course-of-the-university-of-oxford/2022.md#5/solution)
- [Solution](past-exam-of-the-how-to-build-a-brain-from-scratch-course-of-the-university-of-oxford/2022.md#2/solution)
- [Solution](past-exam-of-the-how-to-build-a-brain-from-scratch-course-of-the-university-of-oxford/2022.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-325.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-335.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1.md#7h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1.md#41c/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-339.md#1/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-335.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-3.md#19h/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability.md#6/c/iii/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability.md#6/c/iv/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability-resit.md#5/c/iii/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/discrete-mathematics-probability-and-continuous-mathematics.md#5/c/iii/solution)
- [Squared-error backpropagation](statistical-learning.md#squared-error-backpropagation)
- [Symmetric preconditioning as energy geometry](numerical-linear-algebra.md#symmetric-preconditioning-as-energy-geometry)
