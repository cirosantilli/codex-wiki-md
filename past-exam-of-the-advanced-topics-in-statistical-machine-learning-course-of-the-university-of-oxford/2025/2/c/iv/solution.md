<h1 id="2/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Evaluating the negative [functional gradient](../../../../../functional-gradient.md) at $x_j$ yields

$$
\boxed{\frac{dg_t(x_j)}{dt}=\sum_{i=1}^nk(x_j,x_i)(y_i-g_t(x_i))}.
$$

Thus the evaluation [vector](../../../../../vector.md) $v(t)=(g_t(x_1),\ldots,g_t(x_n))^T$ follows

$$
\boxed{\dot v=K(y-v),\qquad K_{ij}=k(x_i,x_j)=H^*_{ij}}.
$$

This is exactly the limiting prediction dynamics in part (ii). If $v(0)=u(0)$, subtracting the two systems gives $\frac d{dt}(v-u)=-H^*(v-u)$ with zero initial value, so $v(t)=u(t)$ for every $t$.

**An infinitely wide [neural network](../../../../../neural-network.md) in this regime follows the same training-prediction dynamics as [kernel regression](../../../../../kernel-regression.md) with its [neural tangent kernel](../../../../../neural-tangent-kernel.md) and matching initial predictions.** For this squared-error [loss function](../../../../../loss-function.md), the relevant algorithm is [gradient flow](../../../../../gradient-flow.md) in the [Reproducing kernel Hilbert space](../../../../../reproducing-kernel-hilbert-space.md). Matching predictions at arbitrary additional inputs also requires the corresponding cross-input [neural tangent kernel](../../../../../neural-tangent-kernel.md) to freeze and the initial predictions there to match. A finite-width [neural network](../../../../../neural-network.md) can change its [feature map](../../../../../feature-map.md) during training, so the equivalence depends on the assumptions rather than holding for every architecture and parameterization.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
