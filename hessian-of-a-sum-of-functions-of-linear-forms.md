# Hessian of a sum of functions of linear forms

↑ **Parent:** [Hessian matrix](hessian-matrix.md)

For twice differentiable $f:\mathbb R\to\mathbb R$, constant [vectors](vector.md) $a_i$ and constant scalars $y_i$, let $l(x)=\sum_i y_i f(a_i^{\mathsf T}x)$, and let row $i$ of $A$ be $a_i^{\mathsf T}$. The [chain rule](chain-rule.md) gives

$$
\nabla l(x)=\sum_i y_i f'(a_i^{\mathsf T}x)a_i,\qquad
\nabla^2l(x)=\sum_i y_i f''(a_i^{\mathsf T}x)a_i a_i^{\mathsf T}.
$$

The second formula is the displayed [matrix](matrix.md) product because entry $(j,k)$ is the same weighted sum $\sum_i y_i f''(a_i^{\mathsf T}x)a_{ij}a_{ik}$. Signed diagonal factors do not ensure a [positive-definite](positive-definite-bilinear-form.md) [Hessian matrix](hessian-matrix.md). The factorization also gives an efficient [matrix-free Hessian-vector product](matrix-free-hessian-vector-product.md).

## ↑ Ancestors (8)

1. [Hessian matrix](hessian-matrix.md)
2. [Multivariable calculus](multivariable-calculus-split.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability/6/c/ii/solution.md)
