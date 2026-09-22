# Gradient descent

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gradient_descent)

[Gradient descent](gradient-descent-split.md) is an [iterative method](iterative-method.md) for minimizing a [differentiable function](differentiable-function.md) $f$: choose an initial [vector](vector.md) $x_0$ and repeatedly move opposite its [gradient](gradient.md).[§9.3, p. 466, Algorithm 9.3: negative-gradient direction and a separately chosen step size](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

With a fixed positive [step size](step-size.md) $\eta$, the update is

$$
x_{k+1}=x_k-\eta\nabla f(x_k),\qquad k=0,1,2,\ldots.
$$

The direction and the [step size](step-size.md) play different roles: the [gradient](gradient.md) supplies local information about increase, while $\eta$ determines how far that information is trusted. A varying [step size](step-size.md) gives $\eta_k$ instead; [exact line search for a positive-definite quadratic](exact-line-search-for-a-positive-definite-quadratic.md) chooses it by minimizing along the current direction.

Why is this the steepest direction? For a unit [vector](vector.md) $v$ in the [Euclidean norm](euclidean-norm.md), the [directional derivative](directional-derivative.md) is $\langle\nabla f(x),v\rangle$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) bounds it below by $-\|\nabla f(x)\|_2$, attained by $v=-\nabla f(x)/\|\nabla f(x)\|_2$ when the [gradient](gradient.md) is nonzero. This is steepest descent relative to the [Euclidean norm](euclidean-norm.md); changing the [norm](norm.md) can change the steepest direction. A finite step need not decrease $f$, because a [directional derivative](directional-derivative.md) describes infinitesimal motion.

For the [quadratic form](quadratic-form-split.md) with linear term $F(x)=x^TAx/2-b^Tx$, assuming $A$ is a [symmetric matrix](symmetric-matrix.md), the negative [gradient](gradient.md) is the [linear-system residual](linear-system-residual.md) $r=b-Ax$. Thus [gradient descent](gradient-descent-split.md) turns the [linear system](system-of-linear-equations.md) $Ax=b$ into repeated residual corrections; a [positive-definite matrix](positive-definite-matrix.md) makes its solution the unique [global minimum](global-minimum.md). This is useful when applying the [linear map](linear-map.md) $x\mapsto Ax$ is affordable but directly solving the [linear system](system-of-linear-equations.md) is costly.

The attraction is that a [gradient](gradient.md) evaluation gives an entire update without solving a new [linear system](system-of-linear-equations.md). The difficulty is choosing a [step size](step-size.md) that progresses along gently curved directions without overshooting steep ones. [Fixed-step gradient descent on a positive-definite quadratic](fixed-step-gradient-descent-on-a-positive-definite-quadratic.md) makes this tension exact: every [eigenvector](eigenvector.md) direction has its own multiplier, determined by its [eigenvalue](eigenvalue.md). The resulting [condition number](condition-number.md) dependence explains why a narrow valley can slow even an inexpensive [iterative method](iterative-method.md).

The simplicity of the [gradient](gradient.md) update and its sensitivity to the [condition number](condition-number.md) of the [Hessian matrix](hessian-matrix.md) are central practical features.[§9.3.1, pp. 466–468, and §9.3.2, p. 475, Conclusions: convergence and conditioning](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

**Table of contents**

- [Fixed-step gradient descent on a positive-definite quadratic](fixed-step-gradient-descent-on-a-positive-definite-quadratic.md)
  - [Optimal fixed step for quadratic gradient descent](optimal-fixed-step-for-quadratic-gradient-descent.md)
- [Gradient ascent](gradient-ascent.md)
- [Stochastic gradient descent](stochastic-gradient-descent.md)
  - [Projected stochastic gradient descent](projected-stochastic-gradient-descent.md)
  - [Unbiased stochastic gradient](unbiased-stochastic-gradient.md)
- [Lipschitz gradient](lipschitz-gradient.md)
  - [Descent lemma](descent-lemma.md)
- [Exact line search for a positive-definite quadratic](exact-line-search-for-a-positive-definite-quadratic.md)
- [Conjugate gradient method](conjugate-gradient-method.md)
  - [Linear-system residual](linear-system-residual.md)
  - [Conjugate-gradient residual orthogonality](conjugate-gradient-residual-orthogonality.md)
  - [Preconditioned conjugate gradient method](preconditioned-conjugate-gradient-method.md)
    - [Exact inverse-square-root preconditioner](exact-inverse-square-root-preconditioner.md)
  - [Krylov subspace](krylov-subspace.md)
    - [Krylov dimension from spectral components](krylov-dimension-from-spectral-components.md)
  - [Finite termination of the conjugate gradient method](finite-termination-of-the-conjugate-gradient-method.md)
- [Heavy-ball method](heavy-ball-method.md)
  - [Heavy-ball residual recurrence](heavy-ball-residual-recurrence.md)
  - [Heavy-ball error propagation matrix](heavy-ball-error-propagation-matrix.md)
    - [Heavy-ball rate for a two-eigenvalue diagonal quadratic](heavy-ball-rate-for-a-two-eigenvalue-diagonal-quadratic.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Derivative](derivative.md)
- [Descent lemma](descent-lemma.md)
- [Fixed-step gradient descent on a positive-definite quadratic](fixed-step-gradient-descent-on-a-positive-definite-quadratic.md)
- [Gradient](gradient.md)
- [Gradient ascent](gradient-ascent.md)
- [Gradient descent](gradient-descent-split.md)
- [Nesterov accelerated gradient method](nesterov-accelerated-gradient-method.md)
- [Nonlinear programming](nonlinear-programming.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/15/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-325/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-335/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1/7h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1/41c/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-339/1/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-335/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-3/19h/solution.md)
- [Squared-error backpropagation](squared-error-backpropagation.md)
- [Symmetric preconditioning as energy geometry](symmetric-preconditioning-as-energy-geometry.md)
