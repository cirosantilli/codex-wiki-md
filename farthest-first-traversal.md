# Farthest-first traversal

↑ **Parent:** [Metric k-center problem](metric-k-center-problem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Farthest-first_traversal)

Starting with an arbitrary [point](point-geometry.md) in a finite [metric space](metric-space.md), repeatedly select a [point](point-geometry.md) maximizing its distance to the selected [set](set-split.md). Maintain each [point](point-geometry.md)'s distance to its nearest selected center; each new center updates all those distances, giving $O(k|V|)$ distance evaluations for $k$ centers.

For the [metric k-center problem](metric-k-center-problem.md), let $R$ be the final covering radius and add a [point](point-geometry.md) realizing $R$ to the $k$ selected centers. Every pair among these $k+1$ [points](point-geometry.md) has distance at least $R$: at each selection the current maximum distance is at least its final value. If the optimum radius is $r^*$, two of these [points](point-geometry.md) belong to the same optimal radius-$r^*$ [closed ball](closed-ball.md), so the [triangle inequality](triangle-inequality.md) gives $R\leq2r^*$. The case $R=0$ is already optimal. This proves a factor-two [approximation algorithm](approximation-algorithm.md).

## ↑ Ancestors (5)

1. [Metric k-center problem](metric-k-center-problem.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Metric k-center problem](metric-k-center-problem.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/algorithms/3/d/ii/solution.md)
