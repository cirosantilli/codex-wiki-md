# Star metric centered at a point

↑ **Parent:** [Metric space](metric-space.md)

Given a [metric space](metric-space.md) $(X,d)$ and $a\in X$, define a new [metric](metric.md) by $d_a(x,x)=0$ and $d_a(x,y)=d(x,a)+d(a,y)$ for distinct points. It is the distance obtained by joining every point to a central vertex with its original distance to $a$ as edge length. Symmetry and positive definiteness are immediate. With three distinct points the [triangle inequality](triangle-inequality.md) follows from the extra nonnegative term $2d(z,a)$ in the route through an intermediate point; repeated-point cases are immediate.

Every $b\ne a$ is isolated, since $B_{d_a}(b,d(b,a))=\{b\}$. At the centre, however, $B_{d_a}(a,r)=B_d(a,r)$. Thus a map out of this space is [continuous](continuous-function.md) exactly when it is continuous at $a$ in the original metric. The [closure](closure-topology.md) of $B$ is $B$ together with $a$ if $a\notin B$ and $d(a,B)=0$; otherwise it is simply $B$. This construction isolates every point except the centre while preserving exactly its original neighbourhood filter.

## ↑ Ancestors (6)

1. [Metric space](metric-space.md)
2. [Topological analysis](topological-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2009/e/e3/b/i/solution.md)
