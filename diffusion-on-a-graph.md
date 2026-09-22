# Diffusion on a graph

↑ **Parent:** [Laplacian matrix](laplacian-matrix.md)

The continuous-time [diffusion](diffusion.md) model on a finite [undirected graph](undirected-graph.md) uses the [Graph Laplacian](laplacian-matrix.md) in the [ordinary differential equation](ordinary-differential-equation.md)

$$
\dot x=-Lx,\qquad \dot x_i=\sum_{j:\{i,j\}\in E}(x_j-x_i).
$$

Across each [edge](edge-of-a-graph.md), the higher value sends an amount proportional to the difference to the lower value. The two contributions cancel in the sum over [vertices](vertex-graph-theory.md), giving [conservation of mass](mass-conservation.md):

$$
\frac{d}{dt}\sum_i x_i(t)=-\mathbf1^TLx(t)=0.
$$

If the entries represent masses, start with nonnegative entries; signed entries can instead describe deviations from a common level. For the three-[vertex](vertex-graph-theory.md) [path graph](path-graph.md), the initial [vector](vector.md) $x(0)=(1,0,-1)^T$ is an [eigenvector](eigenvector.md) with [eigenvalue](eigenvalue.md) one, so the exact solution is

$$
x(t)=e^{-t}(1,0,-1)^T.
$$

More generally, an [eigenvector](eigenvector.md) with [eigenvalue](eigenvalue.md) $\lambda$ decays by $e^{-\lambda t}$. The [spectral theorem for real symmetric matrices](spectral-theorem-for-real-symmetric-matrices.md) supplies an [orthonormal basis](orthonormal-basis.md) of these [eigenvectors](eigenvector.md), and the [kernel of a graph Laplacian](kernel-of-a-graph-laplacian.md) identifies the surviving terms. On a nonempty [connected graph](connected-graph.md),

$$
\lim_{t\to\infty}x(t)=\bar x\mathbf1,\qquad \bar x=\frac1{|V|}\sum_i x_i(0).
$$

The limiting value is the original [arithmetic mean](arithmetic-mean.md). On a disconnected [graph](graph-split.md), each [connected component of a graph](component-graph-theory.md) converges to its own original [arithmetic mean](arithmetic-mean.md). The same [matrix](matrix.md) therefore measures neighbour disagreement, detects disconnected regions and governs relaxation toward agreement.

## ↑ Ancestors (6)

1. [Laplacian matrix](laplacian-matrix.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
