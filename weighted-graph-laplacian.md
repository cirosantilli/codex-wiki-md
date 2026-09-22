# Weighted graph Laplacian

↑ **Parent:** [Laplacian matrix](laplacian-matrix.md)

For a finite [undirected graph](undirected-graph.md) without [self-loops](loop-graph-theory.md), give each [edge](edge-of-a-graph.md) a symmetric nonnegative weight $w_{ij}=w_{ji}$. In the [weighted graph](weighted-graph.md), set $(A_w)_{ij}=w_{ij}$ for an [edge](edge-of-a-graph.md) and zero otherwise, and $(D_w)_{ii}=\sum_jw_{ij}$ with all other entries zero. The [Weighted graph Laplacian](weighted-graph-laplacian.md) is

$$
L_w=D_w-A_w,\qquad
(L_wx)_i=\sum_jw_{ij}(x_i-x_j),\qquad
x^TL_wx=\sum_{\{i,j\}\in E}w_{ij}(x_i-x_j)^2.
$$

Each [edge](edge-of-a-graph.md) appears once in the [quadratic form](quadratic-form.md). For the [path graph](path-graph.md) $A-B-C$ with weights $w_{AB}=2$ and $w_{BC}=3$,

$$
L_w=\begin{pmatrix}2&-2&0\\-2&5&-3\\0&-3&3\end{pmatrix},\qquad
x=\begin{pmatrix}2\\0\\-1\end{pmatrix},\qquad
x^TL_wx=2(2-0)^2+3(0-(-1))^2=11.
$$

The [Weighted graph Laplacian](weighted-graph-laplacian.md) is still a [positive semidefinite matrix](positive-semidefinite-matrix.md). Its [kernel](kernel-of-a-linear-map.md) consists of [vectors](vector.md) constant on each [connected component of a graph](component-graph-theory.md) after zero-weight [edges](edge-of-a-graph.md) are removed: an [edge](edge-of-a-graph.md) of weight zero imposes no constraint. In an [electrical network](electrical-network.md), taking the weights to be [electrical conductances](electrical-conductance.md) makes $x^TL_wx$ the total power dissipated by [Joule heating](joule-heating.md) when $x$ gives the [voltages](voltage.md) at the [vertices](vertex-graph-theory.md). This physical interpretation explains why stronger connections penalize disagreement more heavily.[Spielman, Spectral Graph Theory, Section 16.3.2: resistor networks](https://www.cs.yale.edu/homes/spielman/PAPERS/SGTChapter.pdf)

## ↑ Ancestors (6)

1. [Laplacian matrix](laplacian-matrix.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Degree matrix](degree-matrix.md)
- [Discrete harmonic function](discrete-harmonic-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-216/1/e/solution.md)
- [Weighted graph Laplacian](weighted-graph-laplacian.md)
