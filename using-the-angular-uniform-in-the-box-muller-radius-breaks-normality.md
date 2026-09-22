# Using the angular uniform in the Box-Muller radius breaks normality

↑ **Parent:** [Box-Muller transform](box-muller-transform.md)

If $V$ is uniform on $(0,1)$, the displayed random variable is not standard normal. For $V\leq1/2$ it is nonnegative; for $V>1/2$, its radius is at most $\sqrt{2\log2}$, so it is always bounded below by $-\sqrt{2\log2}$. A [standard normal distribution](standard-normal-distribution.md) has an unbounded lower tail.

The [Box-Muller transform](box-muller-transform.md) instead uses a common radius $\sqrt{-2\log U}$ independent of the angle $2\pi V$ in both Cartesian coordinates. Their polar density is $re^{-r^2/2}/(2\pi)$, and dividing by the coordinate Jacobian $r$ gives the product of two standard normal densities. Changing a logarithm's uniform input changes the distribution, even if the resulting expression superficially resembles that formula.

## ↑ Ancestors (6)

1. [Box-Muller transform](box-muller-transform.md)
2. [Monte Carlo method](monte-carlo-method-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
