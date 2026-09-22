# Logarithmic water filling

↑ **Parent:** [Water-filling algorithm](water-filling-algorithm.md)

To maximize $\sum_i\log(\alpha_i+x_i)$ for positive baselines, nonnegative allocations and a positive budget $B$, the [KKT conditions](karush-kuhn-tucker-conditions.md) equalize the shifted values on allocated coordinates. The unique water level solves $\sum_i(\tau-\alpha_i)_+=B$. Inactive coordinates have baselines at least the water level. [Strict convexity](strictly-convex-function.md) of the negative objective ensures uniqueness, and sorting the baselines gives an efficient [water-filling algorithm](water-filling-algorithm.md).

## ↑ Ancestors (6)

1. [Water-filling algorithm](water-filling-algorithm.md)
2. [Convex optimization](convex-optimization-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-38/1/a/solution.md)
