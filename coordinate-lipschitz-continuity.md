# Coordinate Lipschitz continuity

↑ **Parent:** [Lipschitz gradient](lipschitz-gradient.md)

The displayed estimate, for all $x$ and real $t$, defines a coordinate [Lipschitz constant](lipschitz-constant.md) $L_i$ for the [partial derivative](partial-derivative.md) in coordinate $i$. It implies the coordinate [descent lemma](descent-lemma.md)

$$
f(x+te_i)\leq f(x)+t\partial_i f(x)+\frac{L_i}{2}t^2
$$

by the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) and integration of the [Lipschitz continuity](lipschitz-continuity.md) estimate. Subtracting an [affine function](affine-function.md) leaves these constants unchanged.

The apparently weaker estimate along the singleton negative [gradient](gradient.md) direction is equivalent when every real [step size](step-size.md) is allowed: if the initial [partial derivative](partial-derivative.md) is nonzero, any displacement can be written $-\alpha\partial_i f(x)e_i$; if it is zero but the final [partial derivative](partial-derivative.md) is nonzero, reverse the endpoints; if both vanish the estimate is trivial.

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

## ← Incoming links (4)

- [Block Lipschitz constant from coordinate smoothness](block-lipschitz-constant-from-coordinate-smoothness.md)
- [Coordinate derivative bound by Bregman divergence](coordinate-derivative-bound-by-bregman-divergence.md)
- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/3/b/solution.md)
- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/3/c/solution.md)
