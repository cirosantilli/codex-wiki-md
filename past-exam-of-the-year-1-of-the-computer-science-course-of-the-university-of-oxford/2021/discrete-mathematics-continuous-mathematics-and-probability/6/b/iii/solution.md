<h1 id="6/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $T(x)$ be the weighted average on the right, and define $F$ and $\Phi=\log F$ as in part (i). Their explicit [gradient](../../../../../../gradient.md) identity is

$$
\nabla\Phi(x)=2(x-T(x)).
$$

Therefore the displayed equation is exactly the [stationary point](../../../../../../stationary-point.md) equation for the strongly convex $\Phi$. It has one solution, which is the unique minimizer from part (i). **Reuse the BFGS iteration**, with

$$
x_{n+1}=x_n-2\alpha_nH_n(x_n-T(x_n)).
$$

The [gradient](../../../../../../gradient.md) is explicit, the weights can again be scaled by their largest exponent, and the usual full-memory [BFGS](../../../../../../bfgs-method.md) assumptions give **local [superlinear convergence](../../../../../../superlinear-convergence.md)**.

Simply setting $x_{n+1}=T(x_n)$ is not automatically a convergent [fixed-point iteration](../../../../../../fixed-point-iteration.md). Differentiating the normalized weights gives

$$
J_T(x)=-2\sum_iw_i(a_i-T(x))(a_i-T(x))^T,
$$

whose [operator norm](../../../../../../operator-norm.md) need not be below $1$. For example, in one dimension with centres $-1,1$, $T(x)=-\tanh(2x)$ and $T'(0)=-2$: the desired fixed point is locally repelling for that naive iteration. If exact second [derivatives](../../../../../../derivative.md) are affordable, [multivariable Newton iteration](../../../../../../multivariable-newton-iteration.md) on $x-T(x)=0$ is another valid choice, with [Jacobian matrix](../../../../../../jacobian-matrix.md) $I-J_T$ as given above and local [quadratic convergence](../../../../../../quadratic-convergence.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
