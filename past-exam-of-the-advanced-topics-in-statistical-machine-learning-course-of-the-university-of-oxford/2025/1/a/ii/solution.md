<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $h(\theta)=\log p(\mathcal D\mid\theta)+\log p(\theta)$. Choose an interior [maximum a posteriori estimate](../../../../../maximum-a-posteriori-estimate.md), a globally maximizing [posterior mode](../../../../../maximum-a-posteriori-estimate.md)

$$
\mu\in\operatorname*{arg\,max}_{\theta}h(\theta),\qquad \nabla h(\mu)=0.
$$

Suppose $h$ is twice continuously differentiable near $\mu$ and its negative [Hessian matrix](../../../../../hessian-matrix.md) $A=-\nabla^2h(\mu)$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md). The second-order [Taylor expansion](../../../../../taylor-expansion.md) is

$$
h(\theta)\simeq h(\mu)-\frac12(\theta-\mu)^TA(\theta-\mu).
$$

Exponentiating and normalizing this local approximation gives the [Laplace approximation](../../../../../laplace-approximation.md)

$$
\boxed{p(\theta\mid\mathcal D)\simeq\mathcal N(\theta;\mu,\Sigma),\qquad \Sigma=A^{-1}=-\bigl[\nabla^2h(\mu)\bigr]^{-1}}.
$$

Thus the approximate [mean](../../../../../expected-value-split.md) is the [posterior mode](../../../../../maximum-a-posteriori-estimate.md), and the approximate [covariance matrix](../../../../../covariance-matrix.md) is the inverse local curvature. This [normal approximation](../../../../../normal-approximation.md) is useful when most [posterior probability](../../../../../posterior-probability.md) is concentrated around this mode. A boundary mode, singular curvature, or several substantial modes requires a modified approximation.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
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
