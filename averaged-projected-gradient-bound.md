# Averaged projected-gradient bound

↑ **Parent:** [Projected gradient descent](projected-gradient-descent.md)

If $\|\nabla F(x_i)\|\leq G$ and $\|x_1-x_*\|\leq D$, then

$$
F\left(\frac1k\sum_{i=1}^kx_i\right)-F(x_*)
\leq\frac{D^2}{2\eta k}+\frac{\eta G^2}{2}.
$$

It follows by expanding the squared distance after each projected step, using nonexpansiveness of projection, summing the resulting inequalities, and applying convexity.

## ↑ Ancestors (6)

1. [Projected gradient descent](projected-gradient-descent.md)
2. [Convex optimization](convex-optimization-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/30l/c/solution.md)
