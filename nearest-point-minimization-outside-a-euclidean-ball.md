# Nearest-point minimization outside a Euclidean ball

↑ **Parent:** [Constrained optimization](constrained-optimization.md)

Suppose $0<\|a\|<R$ in a [Euclidean space](euclidean-norm.md). Among points outside or on the radius-$R$ ball centred at zero, the unique closest point to $a$ is $x_*=Ra/\|a\|$. Its squared distance is $(R-\|a\|)^2$.

Indeed, the [reverse triangle inequality](reverse-triangle-inequality.md) gives $\|x-a\|\geq\|x\|-\|a\|\geq R-\|a\|$. Equality requires $\|x\|=R$ and $x$ pointing in the same direction as $a$, giving the stated unique point. If $a=0$, every point on the sphere is a minimizer. If $\|a\|\geq R$, the point $a$ itself is feasible and the minimum distance is zero.

The exterior is not a [convex set](convex-set-split.md), so a direct geometric argument is useful: it certifies the global answer without treating every candidate satisfying the [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md) as a minimum.

## ↑ Ancestors (6)

1. [Constrained optimization](constrained-optimization.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/5/b/solution.md)
