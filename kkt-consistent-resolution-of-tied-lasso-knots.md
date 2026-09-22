# KKT-consistent resolution of tied Lasso knots

↑ **Parent:** [Lasso regularization path](lasso-regularization-path.md)

At a positive penalty level, let $E$ be the residual-score equality set, $s_j$ its signs and $N$ the nonzero [regression coefficient](regression-coefficient.md) support. With full column rank, the displayed [strictly convex](strictly-convex-function.md) [quadratic program](quadratic-program.md) selects the direction for a small decrease of the penalty. Existing nonzero [regression coefficients](regression-coefficient.md) have unrestricted tangent components; tied zero [regression coefficients](regression-coefficient.md) may move only with their residual signs. Stationarity gives $X_j^TXv=s_j$ for $j\in N$ and for entering zero coordinates, and $s_jX_j^TXv\geq1$ for tied coordinates that remain zero. These are exactly the first-order [Karush-Kuhn-Tucker conditions for the Lasso](karush-kuhn-tucker-conditions-for-the-lasso.md) along the next segment. Normalize $Xv$ to obtain the corresponding least-angle direction. This resolves simultaneous entries or dropouts without adding a generic-position assumption.

// Target: mathematical-optimization.bigb

## ↑ Ancestors (6)

1. [Lasso regularization path](lasso-regularization-path.md)
2. [Lasso](lasso.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-34/4/solution.md)
