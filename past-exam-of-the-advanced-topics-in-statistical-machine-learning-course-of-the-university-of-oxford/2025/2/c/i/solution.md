<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $J(t)$ be the $n\times d$ [Jacobian matrix](../../../../../jacobian-matrix.md) with row $J_i(t)=\nabla_\theta f(\theta(t),x_i)^T$. Differentiating the squared-error [loss function](../../../../../loss-function.md) gives

$$
\nabla_\theta\ell(\theta(t))=\sum_i(u_i(t)-y_i)\nabla_\theta f(\theta(t),x_i)=J(t)^T(u(t)-y).
$$

The parameter [gradient flow](../../../../../gradient-flow.md) is consequently $\dot\theta=J^T(y-u)$. The [chain rule](../../../../../chain-rule.md) then gives

$$
\boxed{\dot u(t)=H(t)(y-u(t)),\qquad H(t)=J(t)J(t)^T},
$$

where, explicitly,

$$
\boxed{H_{ij}(t)=\left\langle\nabla_\theta f(\theta(t),x_i),\nabla_\theta f(\theta(t),x_j)\right\rangle_{\mathbb R^d}}.
$$

It is a [Gram matrix](../../../../../gram-matrix.md) and therefore a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md): $v^TH(t)v=\|J(t)^Tv\|_2^2\geq0$. These derivatives are understood wherever the network is differentiable; for piecewise differentiable activations the same calculation applies along differentiable portions of the trajectory.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
