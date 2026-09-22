# Newton minimization of the square-root norm

↑ **Parent:** [Newton's method in optimization](newton-s-method-in-optimization.md)

For the [Euclidean norm](euclidean-norm.md) on $\mathbb R^d$, the regularized radial [function](function-split.md) $f(z)=\sqrt{1+\|z\|^2}$ has [gradient](gradient.md) $z/f$ and [Hessian](hessian-matrix.md) $I/f-zz^T/f^3$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) makes its [Hessian](hessian-matrix.md) a [positive-definite matrix](positive-definite-matrix.md), so $f$ is strictly [convex](convex-function.md) with unique [minimum](minimum-of-a-subset-of-a-total-order.md) at zero. Its [inverse matrix](matrix-inverse-split.md) is $f(I+zz^T)$: multiplication verifies this using $(zz^T)^2=\|z\|^2zz^T$ and $f^2=1+\|z\|^2$. Substitution in [Newton's method in optimization](newton-s-method-in-optimization.md) therefore gives $z_{k+1}=-\|z_k\|^2z_k$. Consequently $\|z_{k+1}\|=\|z_k\|^3$: nonzero starts in the open unit ball have exact [cubic convergence](cubic-convergence.md), starts on the unit sphere alternate between opposite points, and starts outside it diverge. This example separates strict [convexity](convex-function.md) from global [convergence](convergence.md) of an undamped iteration.

## ↑ Ancestors (5)

1. [Newton's method in optimization](newton-s-method-in-optimization.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability-resit/6/e/solution.md)
