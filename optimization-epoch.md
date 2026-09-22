# Optimization epoch

↑ **Parent:** [Gradient descent](gradient-descent-split.md)

A unit of work corresponding to one full pass through the components used to measure an [iterative method](iterative-method.md). For [coordinate descent](coordinate-descent.md) in $n$ coordinates, count $n$ coordinate [partial derivative](partial-derivative.md) evaluations as an optimization epoch: updates on blocks of size $m$ require $n/m$ updates per optimization epoch. For [stochastic gradient descent](stochastic-gradient-descent.md) on a finite sum of losses, a common different convention counts one evaluation of every loss component. The convention must be specified. Random sampling with replacement need not visit every component during one such unit of work.

```
Target: gradient-descent.bigb, under Gradient descent.
```

## ↑ Ancestors (6)

1. [Gradient descent](gradient-descent-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Epoch complexity](epoch-complexity.md)
- [Solution](past-exam-of-the-optimisation-for-data-science-course-of-the-university-of-oxford/2023/3/d/solution.md)
- [Randomized block coordinate descent](randomized-block-coordinate-descent.md)
