# Periodic Poisson equation on a four-point cycle

↑ **Parent:** [Circulant matrix](circulant-matrix.md)

Consider the discrete [linear system](system-of-linear-equations.md) $Lx=b$ with

$$
L=\begin{pmatrix}
2&-1&0&-1\\
-1&2&-1&0\\
0&-1&2&-1\\
-1&0&-1&2
\end{pmatrix},
\qquad b=(1,0,-1,0)^T.
$$

This is a finite periodic analogue of the [Poisson equation](poisson-s-equation.md), using the negative second [finite difference](finite-difference-split.md) with unit grid spacing. It is also a [Graph Laplacian](laplacian-matrix.md) equation on a [cycle graph](cycle-graph.md); no continuum approximation is being claimed here.

<a id="image-balanced-forcing-and-the-mean-zero-solution-on-a-four-node-ring"></a>
![](periodic-circulant-poisson-solution.png)

**[Figure 15](#image-balanced-forcing-and-the-mean-zero-solution-on-a-four-node-ring). Balanced forcing and the mean-zero solution on a four-node ring**.

Summing the four equations gives zero on the left, since each value occurs twice positively and twice negatively. A necessary condition is therefore $\sum_n b_n=0$. The [Fourier diagonalization of a circulant matrix](fourier-diagonalization-of-a-circulant-matrix.md) shows that this is also sufficient: the only zero [eigenvalue](eigenvalue.md) of $L$ is the constant mode $k=0$, and $\widehat b_0=\sum_n b_n$.

For the displayed forcing, the [discrete Fourier transform](discrete-fourier-transform-split.md) gives

$$
\widehat b=(0,2,0,2)^T,
\qquad
(\lambda_0,\lambda_1,\lambda_2,\lambda_3)=(0,2,4,2).
$$

Divide only at the three nonzero [eigenvalues](eigenvalue.md), and choose $\widehat x_0=0$ to impose zero [arithmetic mean](arithmetic-mean.md):

$$
\widehat x=(0,1,0,1)^T,
\qquad
\boxed{x=(1/2,0,-1/2,0)^T.}
$$

Direct substitution gives $Lx=(1,0,-1,0)^T$. All other [vectors](vector.md) satisfying the [linear system](system-of-linear-equations.md) are $x+a(1,1,1,1)^T$, because the [kernel](kernel-of-a-linear-map-split.md) is the space of constant [vectors](vector.md). Thus balanced forcing determines the differences between values, while a reference level is an extra choice. This small model explains why a periodic [Poisson equation](poisson-s-equation.md) needs both a compatibility condition and a normalization.

## ↑ Ancestors (6)

1. [Circulant matrix](circulant-matrix.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
