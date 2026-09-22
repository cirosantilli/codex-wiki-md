# Boundary-matrix construction of an ordinary differential Green function

↑ **Parent:** [Green's function](green-s-function-split.md)

Let $h_1,\ldots,h_n$ be a [basis](basis.md) of [homogeneous solutions](homogeneous-solution.md) of a linear ordinary [differential operator](differential-operator.md) $L$ of order $n$. Let $B_1,\ldots,B_n$ be independent homogeneous linear [boundary conditions](boundary-condition.md), which may be coupled. Suppose a [fundamental solution](fundamental-solution-of-a-linear-differential-operator.md) $G_0(x,\xi)$ satisfies $L_xG_0=\delta(x-\xi)$. Define the boundary [matrix](matrix.md) $M_{ij}=B_i h_j$ and $b_i(\xi)=B_iG_0(\cdot,\xi)$. If $M$ is invertible, then

$$
G(x,\xi)=G_0(x,\xi)-\sum_{j=1}^n h_j(x)\bigl[M^{-1}b(\xi)\bigr]_j.
$$

The added terms are [homogeneous solutions](homogeneous-solution.md), so the [Dirac delta](dirac-delta-function.md) source is preserved. Applying the boundary operators gives $b-MM^{-1}b=0$. Any two such [Green functions](green-s-function-split.md) differ, for fixed source position, by a [homogeneous solution](homogeneous-solution.md) with [coefficient](coefficient.md) vector in the [null space](kernel-of-a-linear-map-split.md) of $M$; invertibility therefore proves [uniqueness](uniqueness.md). A singular boundary [matrix](matrix.md) signals a nontrivial [homogeneous solution](homogeneous-solution.md) satisfying the endpoint conditions, where a compatibility condition and a nonunique inverse may arise. For $L=D^2$, one convenient [fundamental solution](fundamental-solution-of-a-linear-differential-operator.md) is $(x-\xi)H(x-\xi)$.

## ↑ Ancestors (5)

1. [Green's function](green-s-function-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-differential-equations-2-course-of-the-university-of-oxford/2015/1/c/solution.md)
