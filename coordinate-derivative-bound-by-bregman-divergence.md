# Coordinate derivative bound by Bregman divergence

↑ **Parent:** [Lipschitz gradient](lipschitz-gradient.md)

Suppose $f$ is a [differentiable](differentiable-function.md) [convex function](convex-function.md) with [coordinate Lipschitz continuity](coordinate-lipschitz-continuity.md) constant $L_i>0$. Put $\phi(u)=D_f(u,y)=f(u)-f(y)-\nabla f(y)^T(u-y)$, the [Bregman divergence](bregman-divergence.md) from the supporting [affine function](affine-function.md) at $y$. The [subgradient inequality](subgradient-inequality.md) gives $\phi\geq0$, and its coordinate [Lipschitz constant](lipschitz-constant.md) is still $L_i$. The coordinate [descent lemma](descent-lemma.md) with [step size](step-size.md) $1/L_i$ yields

$$
0\leq\phi\left(x-\frac{\partial_i\phi(x)}{L_i}e_i\right)\leq\phi(x)-\frac{[\partial_i\phi(x)]^2}{2L_i}.
$$

Since $\partial_i\phi(x)=\partial_i f(x)-\partial_i f(y)$, rearrangement proves the bound. Continuous [differentiability](differentiability.md) suffices; a [Hessian matrix](hessian-matrix.md) is unnecessary.

```
Target: gradient-descent.bigb, under Lipschitz gradient.
```

## ↑ Ancestors (7)

1. [Lipschitz gradient](lipschitz-gradient.md)
2. [Gradient descent](gradient-descent-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Block Lipschitz constant from coordinate smoothness](block-lipschitz-constant-from-coordinate-smoothness.md)
- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/3/c/solution.md)
