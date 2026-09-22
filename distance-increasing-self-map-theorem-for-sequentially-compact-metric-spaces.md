# Distance-increasing self-map theorem for sequentially compact metric spaces

↑ **Parent:** [Sequentially compact space](sequentially-compact-space.md)

Every [continuous](continuous-function.md) map $T:X\to X$ on a [sequentially compact space](sequentially-compact-space.md) with a [metric](metric.md) satisfying $d(Tx,Ty)\geq d(x,y)$ is a surjective [isometry](isometry.md).

A [convergent subsequence](convergent-subsequence.md) of the paired orbit $(T^kx,T^ky)$ has two late terms arbitrarily close. Removing their common number of iterates by the distance inequality shows that $(x,y)$ returns arbitrarily close to itself after a common positive time $n$. Thus $d(Tx,Ty)\leq d(T^nx,T^ny)\leq d(x,y)+2\epsilon$, and letting $\epsilon\downarrow0$ proves the [isometry](isometry.md) claim. For each $x$, choose return times $n_k\geq1$ with $T^{n_k}x\to x$. A [convergent subsequence](convergent-subsequence.md) of $T^{n_k-1}x$ has limit $z$, and [continuity](continuous-function.md) gives $Tz=x$. This proves surjectivity.

## ↑ Ancestors (5)

1. [Sequentially compact space](sequentially-compact-space.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-metric-spaces-and-complex-analysis-course-of-the-university-of-oxford/2023/2/c/ii/solution.md)
