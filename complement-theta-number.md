# Complement theta number

↑ **Parent:** [Lovász number](lovasz-number.md)

For a finite simple [graph](graph-split.md) with at least one vertex, the complement theta number has the equivalent [semidefinite program](semidefinite-programming.md) formulations

$$
\bar\vartheta(G)=\min\left\{t:
\begin{pmatrix}t&\mathbf1^T\\\mathbf1&Z\end{pmatrix}\succeq0,
\ Z_{ii}=1,\ Z_{ij}=0\text{ for }ij\in E(G)\right\}
$$

and

$$
\bar\vartheta(G)=\min\{t:U\succeq0,\ U_{ii}=t-1,\ U_{ij}=-1\text{ for }ij\in E(G)\}.
$$

The [Schur complement](schur-complement.md) and $U=tZ-J$ prove the equivalence; any feasible $t$ is at least one, so division by $t$ is valid. For a [graph](graph-split.md) with an edge, $U/(t-1)$ is the [Gram matrix](gram-matrix.md) of a [strict vector coloring](strict-vector-coloring.md). Consequently $\bar\vartheta(G)$ is the strict vector chromatic number, and an ordinary $k$-[graph colouring](graph-coloring.md) gives $\bar\vartheta(G)\leq k$ by assigning the colors the vertices of a [regular simplex](regular-simplex.md).

## ↑ Ancestors (7)

1. [Lovász number](lovasz-number.md)
2. [Graph coloring](graph-coloring.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-339/2/a/solution.md)
- [Strict vector coloring](strict-vector-coloring.md)
