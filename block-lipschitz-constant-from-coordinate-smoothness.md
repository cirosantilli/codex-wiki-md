# Block Lipschitz constant from coordinate smoothness

↑ **Parent:** [Lipschitz gradient](lipschitz-gradient.md)

For a continuously [differentiable](differentiable-function.md) [convex function](convex-function.md) on $\mathbb R^n$ with [coordinate Lipschitz continuity](coordinate-lipschitz-continuity.md) constants $L_i$, its [block coordinate gradient](block-coordinate-gradient.md) is [Lipschitz continuous](lipschitz-continuity.md) along each corresponding [coordinate subspace](coordinate-subspace.md), with constant at most $S_{\mathcal B}=\sum_{i\in\mathcal B}L_i$.

To prove this without assuming a [Hessian matrix](hessian-matrix.md), put $\delta_{\mathcal B}=\nabla_{\mathcal B}f(x)-\nabla_{\mathcal B}f(y)$. Sum the [coordinate derivative bound by Bregman divergence](coordinate-derivative-bound-by-bregman-divergence.md) over the block, then repeat with $x,y$ interchanged and average:

$$
\|\delta_{\mathcal B}\|^2\leq S_{\mathcal B}\big(D_f(x,y)+D_f(y,x)\big)
=S_{\mathcal B}(\nabla f(x)-\nabla f(y))^T(x-y).
$$

If $x-y$ is supported in the block, the [dot product](dot-product.md) uses only $\delta_{\mathcal B}$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) and cancellation of its [Euclidean norm](euclidean-norm.md) give the result, including the zero case separately. Taking the full block supplies a global [Lipschitz gradient](lipschitz-gradient.md) constant $\sum_iL_i$.

```
Target: convex-optimization.bigb, under Coordinate descent.
```

## ↑ Ancestors (7)

1. [Lipschitz gradient](lipschitz-gradient.md)
2. [Gradient descent](gradient-descent-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/3/c/solution.md)
