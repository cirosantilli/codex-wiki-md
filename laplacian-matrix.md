# Laplacian matrix

↑ **Parent:** [Graph theory](graph-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laplacian_matrix)

The [Graph Laplacian](laplacian-matrix.md) converts local differences along [edges](edge-of-a-graph.md) into a [linear map](linear-map.md). Throughout this section, $G=(V,E)$ is a finite [undirected graph](undirected-graph.md) with no [self-loops](loop-graph-theory.md) or repeated [edges](edge-of-a-graph.md), and each [edge](edge-of-a-graph.md) has weight one. In a fixed order of [vertices](vertex-graph-theory.md), let $A$ be the [adjacency matrix](adjacency-matrix.md) and $D$ the [degree matrix](degree-matrix.md). The combinatorial [Graph Laplacian](laplacian-matrix.md) is

$$
L=D-A,\qquad (Lx)_i=\sum_{j:\{i,j\}\in E}(x_i-x_j).
$$

Thus the value at a [vertex](vertex-graph-theory.md) is compared with its neighbours. Every row sums to zero, so $L\mathbf1=0$: a constant [vector](vector.md) produces no differences. This definition and the associated [Graph Laplacian quadratic form](graph-laplacian-quadratic-form.md) are developed in Spielman's authored survey.[Spielman, Spectral Graph Theory, Sections 16.3.1–16.3.2](https://www.cs.yale.edu/homes/spielman/PAPERS/SGTChapter.pdf)

For the three-[vertex](vertex-graph-theory.md) [path graph](path-graph.md) $A-B-C$, the [vertex degrees](degree-graph-theory.md) are $1,2,1$, and in that order

$$
A=\begin{pmatrix}0&1&0\\1&0&1\\0&1&0\end{pmatrix},\qquad
D=\begin{pmatrix}1&0&0\\0&2&0\\0&0&1\end{pmatrix},\qquad
L=\begin{pmatrix}1&-1&0\\-1&2&-1\\0&-1&1\end{pmatrix}.
$$

Direct multiplication gives three [eigenvectors](eigenvector.md) and their [eigenvalues](eigenvalue.md):

$$
L\begin{pmatrix}1\\1\\1\end{pmatrix}=0,\qquad
L\begin{pmatrix}1\\0\\-1\end{pmatrix}=\begin{pmatrix}1\\0\\-1\end{pmatrix},\qquad
L\begin{pmatrix}1\\-2\\1\end{pmatrix}=3\begin{pmatrix}1\\-2\\1\end{pmatrix}.
$$

The constant [eigenvector](eigenvector.md) has [eigenvalue](eigenvalue.md) zero; the other two describe progressively stronger neighbour disagreement. Dividing these [eigenvectors](eigenvector.md) by $\sqrt3,\sqrt2,\sqrt6$, respectively, gives an [orthonormal basis](orthonormal-basis.md). The four-[vertex](vertex-graph-theory.md) [cycle graph](cycle-graph.md) is already worked out under [circulant matrix](circulant-matrix.md), where [Fourier diagonalization of a circulant matrix](fourier-diagonalization-of-a-circulant-matrix.md) gives its [eigenvalues](eigenvalue.md).

Every formula here uses $L=D-A$ without degree normalization. For comparison, Chung's treatment uses the degree-scaled [matrix](matrix.md) $D^{-1/2}LD^{-1/2}$, with a convention for isolated [vertices](vertex-graph-theory.md); its [eigenvalues](eigenvalue.md) must not be substituted into the examples here.[Chung, Lectures on Spectral Graph Theory, Section 1.2](https://www.math.ucsd.edu/~fan/cbms.pdf)

**Table of contents**

- [Weighted graph Laplacian](weighted-graph-laplacian.md)
- [Degree matrix](degree-matrix.md)
- [Graph Laplacian quadratic form](graph-laplacian-quadratic-form.md)
- [Kernel of a graph Laplacian](kernel-of-a-graph-laplacian.md)
- [Diffusion on a graph](diffusion-on-a-graph.md)
- [Laplacian spectrum of a complete graph](laplacian-spectrum-of-a-complete-graph.md)

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Spectral graph theory](spectral-graph-theory.md)
