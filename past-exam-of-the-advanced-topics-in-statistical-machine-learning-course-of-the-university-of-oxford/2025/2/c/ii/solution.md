<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Under the stated infinite-width scaling and freezing assumptions, the deterministic limiting [kernel matrix](../../../../../kernel-matrix.md) has entries

$$
\boxed{H^*_{ij}=\mathbb E_{\theta(0)\sim P}\left\langle\nabla_\theta f(\theta(0),x_i),\nabla_\theta f(\theta(0),x_j)\right\rangle=k_{\rm NTK}(x_i,x_j)}.
$$

For a sequence of finite-width networks, this expectation is interpreted in the stated width limit. The resulting [neural tangent kernel](../../../../../neural-tangent-kernel.md) is a [positive-semidefinite kernel](../../../../../positive-semidefinite-kernel-split.md), since every finite coefficient [vector](../../../../../vector.md) $a$ gives $a^TH^*a=\mathbb E\|\sum_i a_i\nabla_\theta f(\theta(0),x_i)\|_2^2\geq0$.

The prediction [gradient flow](../../../../../gradient-flow.md) is linear:

$$
\boxed{\dot u=H^*(y-u),\qquad u(t)=y+e^{-tH^*}(u(0)-y)}.
$$

The [matrix exponential](../../../../../matrix-exponential.md) solves the constant-coefficient system because the residual $u-y$ satisfies $\frac d{dt}(u-y)=-H^*(u-y)$. Each positive-[eigenvalue](../../../../../eigenvalue.md) component decays exponentially; a component in the [null space](../../../../../kernel-of-a-linear-map-split.md) of $H^*$ stays at its initial residual. Thus $u(t)\to y$ for every initial prediction if $H^*$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md). The limiting [kernel matrix](../../../../../kernel-matrix.md) being deterministic does not require $u(0)$ to be deterministic.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
