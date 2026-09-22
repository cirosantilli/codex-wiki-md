<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A practical choice is a [BFGS method](../../../../../../bfgs-method.md), using exact [gradients](../../../../../../gradient.md) and a [line search](../../../../../../line-search.md). At dimension $d=100$, its $d$-by-$d$ inverse-[Hessian matrix](../../../../../../hessian-matrix.md) approximation is small, whereas forming a million rank-one contributions to the exact [Hessian matrix](../../../../../../hessian-matrix.md) is expensive. If $F(x)=\sum_i e^{\|x-a_i\|^2}$, the explicit [derivatives](../../../../../../derivative.md) are

$$
\nabla F=2\sum_i e^{\|x-a_i\|^2}(x-a_i),\qquad
H_F=\sum_i e^{\|x-a_i\|^2}\bigl(4(x-a_i)(x-a_i)^T+2I\bigr).
$$

The positive-definite [Hessian matrix](../../../../../../hessian-matrix.md) and [coercivity](../../../../../../coercive-function.md) show that the objective has one global minimizer.

For numerical stability one can minimize $\Phi=\log F$ instead, which has exactly the same minimizer. Put $r_i=\|x-a_i\|^2$, $w_i=e^{r_i}/\sum_j e^{r_j}$, and $\bar a=\sum_iw_i a_i$. Then the [logarithmic gradient of an exponential squared-distance sum](../../../../../../logarithmic-gradient-of-an-exponential-squared-distance-sum.md) gives

$$
g(x):=\nabla\Phi(x)=2(x-\bar a),\qquad
\nabla^2\Phi=2I+4\sum_iw_i(a_i-\bar a)(a_i-\bar a)^T\succeq2I.
$$

Evaluate the weights as $e^{r_i-r_{\max}}/\sum_j e^{r_j-r_{\max}}$ to avoid [floating-point overflow](../../../../../../floating-point-overflow.md). A [quasi-Newton method](../../../../../../quasi-newton-method.md) step is

$$
x_{n+1}=x_n-\alpha_nH_n g(x_n),
$$

where $H_n$ is the positive-definite inverse-[Hessian matrix](../../../../../../hessian-matrix.md) approximation updated by [BFGS](../../../../../../bfgs-method.md), and $\alpha_n$ is chosen by a [line search](../../../../../../line-search.md), for example one satisfying the [Wolfe conditions](../../../../../../wolfe-conditions.md). Under the standard smoothness and nondegeneracy assumptions at this strongly convex minimizer, full-memory [BFGS](../../../../../../bfgs-method.md) has **local [superlinear convergence](../../../../../../superlinear-convergence.md)**. An exact [Newton's method in optimization](../../../../../../newton-s-method-in-optimization.md) would have local [quadratic convergence](../../../../../../quadratic-convergence.md), but pays for those much more expensive exact second [derivatives](../../../../../../derivative.md).[Opening construction and BFGS update: approximate Hessians from [gradients](../../../../../../gradient.md); dense update cost of order d squared](../../../../../../quasi-newton-methods-by-neos-guide.md)

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
