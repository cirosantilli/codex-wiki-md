# Compact subset of an open set has positive distance from its complement

↑ **Parent:** [Distance between two sets](distance-between-two-sets.md)

In a [metric space](metric-space.md) $X$, let the nonempty [compact set](compact-space.md) $K$ lie in the [open set](open-set.md) $\Omega$. If $F=X\setminus\Omega$ is nonempty, the [distance to a set](distance-to-a-set.md) $d(x,F)$ is a [continuous function](continuous-function.md) of $x$: the [triangle inequality](triangle-inequality.md) gives $|d(x,F)-d(y,F)|\leq d(x,y)$. Since $F$ is a [closed set](closed-set.md), this distance is strictly positive on $K$. The [extreme value theorem](extreme-value-theorem.md) attains its minimum on $K$, so

$$
d(K,F)=\min_{x\in K}d(x,F)>0.
$$

If $F$ is empty, the extended-real convention gives $d(K,F)=+\infty$. This result provides a single positive neighbourhood radius that stays inside $\Omega$ at every point of $K$. Compactness is essential: in the real line $K=\{1/n:n\geq1\}\subset(0,2)$ has zero [distance between two sets](distance-between-two-sets.md) from $(-\infty,0]\cup[2,\infty)$, although each point of $K$ has positive [distance to a set](distance-to-a-set.md) from that [complement](complement-of-a-set.md).

## ↑ Ancestors (8)

1. [Distance between two sets](distance-between-two-sets.md)
2. [Distance to a set](distance-to-a-set.md)
3. [Metric space](metric-space.md)
4. [Topological analysis](topological-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford/2012/4/c/solution.md)
