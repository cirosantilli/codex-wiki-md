<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\mu>0$, the [logarithmic barrier](../../../../logarithmic-barrier.md) objective is

$$
\boxed{f_\mu(x)=f(x)-\mu\sum_{i=1}^p\log c_i(x)},\qquad D=\{x:c_i(x)>0\text{ for all }i\}.
$$

The [domain of a function](../../../../domain-of-a-function.md) $D$ is a nonempty [convex set](../../../../convex-set-split.md) by the same [concavity](../../../../concave-function.md) argument as in part (a), with strict inequalities. Differentiating twice on $D$ gives

$$
\nabla^2f_\mu(x)=\nabla^2f(x)-\mu\sum_i\frac{\nabla^2c_i(x)}{c_i(x)}+\mu\sum_i\frac{\nabla c_i(x)\nabla c_i(x)^T}{c_i(x)^2}.
$$

Here $\nabla^2f\succeq0$ by [convexity](../../../../convex-function.md), $-\nabla^2c_i\succeq0$ by [concavity](../../../../concave-function.md), and each [outer product](../../../../outer-product.md) is a [positive semidefinite matrix](../../../../positive-semidefinite-matrix.md). Hence $\nabla^2f_\mu\succeq0$, proving [convexity](../../../../convex-function.md) on $D$.

The domain qualification matters: the displayed real-valued [logarithm](../../../../logarithm.md) expression is not defined on all of $\mathbb R^n$. The precise whole-space version is the extended-real [convex function](../../../../convex-function.md) equal to $f_\mu$ on $D$ and $+\infty$ outside $D$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
