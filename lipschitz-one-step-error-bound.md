# Lipschitz one-step error bound

↑ **Parent:** [Global discretization error](global-discretization-error.md)

Suppose the increment function of a [one-step method](one-step-method.md) is [Lipschitz continuous](lipschitz-continuity.md) in its solution argument with constant $K>0$, uniformly in time and step size. Let $e_n=y(x_n)-y_n$ be the [global error](global-discretization-error.md), and let $hT_n$ be the exact-start [local truncation error](local-truncation-error.md). The [triangle inequality](triangle-inequality.md) gives $|e_{n+1}|\leq(1+hK)|e_n|+h|T_n|$. Iterating and summing a [geometric series](geometric-series.md) proves the displayed estimate. Since $(1+hK)^n\leq e^{Knh}$, uniformly bounded $K$ and [consistency error](normalized-local-truncation-error.md) $O(h^p)$ give [global error](global-discretization-error.md) $O(h^p)$ on a fixed time interval when $e_0=O(h^p)$. Here $O$ denotes [Big O notation](big-o-notation.md). This is a constant-step form of the [discrete Gronwall inequality](discrete-gronwall-inequality.md).

## ↑ Ancestors (6)

1. [Global discretization error](global-discretization-error.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Explicit midpoint method](explicit-midpoint-method.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-numerical-solution-of-differential-equations-course-of-the-university-of-oxford/2020/1/b/solution.md)
- [Solution](past-exam-of-the-numerical-solution-of-differential-equations-course-of-the-university-of-oxford/2011/a/1/b/solution.md)
