# Metric k-center problem

↑ **Parent:** [Mathematical optimization](mathematical-optimization-split.md)

The [metric k-center problem](metric-k-center-problem.md) chooses at most $k$ centers from a finite [metric space](metric-space.md) to minimize the largest distance from a [point](point-geometry.md) to its nearest center. For $1\leq k\leq|V|$, exactly $k$ centers gives the same optimum: extra centers never increase the radius. The restriction that centers belong to $V$ matters; allowing centers anywhere in an ambient [metric space](metric-space.md) is a different problem.

The basic packing argument is short. If a radius-$r$ solution uses $k$ centers, its $k$ [closed balls](closed-ball.md) cover $V$. Two [points](point-geometry.md) assigned to the same center have distance at most $2r$ by the [triangle inequality](triangle-inequality.md). Thus $k+1$ [points](point-geometry.md) with pairwise distances greater than $2r$ certify that no radius-$r$ solution exists. Greedily selecting a new center only outside all existing radius-$2r$ [closed balls](closed-ball.md) therefore uses at most $k$ centers whenever a radius-$r$ solution exists, and its final covering radius is at most $2r$. The [farthest-first traversal](farthest-first-traversal.md) achieves the same [approximation ratio](approximation-ratio.md) without knowing $r$.

**Table of contents**

- [Farthest-first traversal](farthest-first-traversal.md)

## ↑ Ancestors (4)

1. [Mathematical optimization](mathematical-optimization-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Farthest-first traversal](farthest-first-traversal.md)
- [Metric k-center problem](metric-k-center-problem.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/algorithms/3/d/i/solution.md)
