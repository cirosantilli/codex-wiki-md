# Hessian of the Euclidean norm

↑ **Parent:** [Euclidean norm](euclidean-norm.md)

For a nonzero [vector](vector.md) $x\in\mathbb R^n$, put $r=|x|$ and $\hat x=x/r$. The [gradient](gradient.md) of the [Euclidean norm](euclidean-norm.md) is $\nabla r=\hat x$. Differentiate its components to obtain the [Hessian matrix](hessian-matrix.md)

$$
\partial_i\partial_jr=\frac{\delta_{ij}}r-\frac{x_ix_j}{r^3},\qquad D^2r=\frac1r(I-\hat x\hat x^T).
$$

The factor $I-\hat x\hat x^T$ is the [orthogonal projection matrix](orthogonal-projection-matrix.md) onto the [orthogonal complement](orthogonal-complement.md) of the radial direction. Thus the [Hessian matrix](hessian-matrix.md) has [eigenvalue](eigenvalue.md) zero radially and $1/r$ on each tangential direction, explaining the [convexity](convex-function.md) of the [Euclidean norm](euclidean-norm.md). Taking the [trace](matrix-trace.md) gives $\Delta r=(n-1)/r$ away from the origin. The [Euclidean norm](euclidean-norm.md) is not [differentiable](differentiable-function.md) at the origin: its restriction to any line is a nonzero multiple of the absolute value.

## ↑ Ancestors (7)

1. [Euclidean norm](euclidean-norm.md)
2. [Normed vector space](normed-vector-space-split.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/10/a/solution.md)
