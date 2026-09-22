<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A standard form of the [Zoutendijk theorem](../../../../zoutendijk-theorem.md) assumes that $f$ is continuously differentiable and bounded below on the starting level set, that its [gradient](../../../../gradient.md) is Lipschitz on a neighborhood of that set, and that the steps satisfy fixed [Wolfe conditions](../../../../wolfe-conditions.md). For [descent directions](../../../../descent-direction.md) $p_k$, define

$$
\cos\theta_k=-\frac{\nabla f(x_k)^Tp_k}{\|\nabla f(x_k)\|\,\|p_k\|}.
$$

Then

$$
\boxed{\sum_k\cos^2\theta_k\,\|\nabla f(x_k)\|^2<\infty.}
$$

In particular, if $\cos\theta_k\geq\delta>0$, then $\nabla f(x_k)\to0$. This last angle hypothesis is needed to turn the general descent theorem into [gradient](../../../../gradient.md) [convergence](../../../../convergence.md).

For this quadratic, $f\geq0$, the [Hessian matrix](../../../../hessian-matrix.md) is the constant [positive-definite matrix](../../../../positive-definite-matrix.md) $H$, and the [gradient](../../../../gradient.md) is globally Lipschitz with constant $L=2\max(c^{-2},d^{-2})$. Its level sets are compact. Thus all objective-function hypotheses hold; Wolfe holds for the exact steps with the parameters above. The direction hypothesis will be verified for alternating exact coordinate minimization in the next part.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
