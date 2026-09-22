# Synchronizing the closest points of two lines

↑ **Parent:** [Distance between skew lines](distance-between-skew-lines.md)

For nonparallel directions $\mathbf b_1,\mathbf b_2$ and points $\mathbf a_1,\mathbf a_2$, let $s_1,s_2$ be the independent line parameters at the closest points. Put $\Delta=\mathbf a_2-\mathbf a_1$ and $D=|\mathbf b_1\times\mathbf b_2|^2>0$. Perpendicularity of the connecting vector to both directions gives a two-by-two [linear system](system-of-linear-equations.md). Solving it and subtracting yields

$$
s_2-s_1=-\frac{\Delta\cdot[(\mathbf b_1\times\mathbf b_2)\times(\mathbf b_1-\mathbf b_2)]}{D}.
$$

Particles with positions $\mathbf a_j+\mathbf b_j(t-t_j)$ reach these two points simultaneously exactly when $t_1-t_2=s_2-s_1$. Otherwise, their [closest approach of two uniformly moving particles](closest-approach-of-two-uniformly-moving-particles.md) can exceed the geometric line distance. The formula requires nonparallel directions; it is not an identity obeyed by arbitrary fixed starting times.

## ↑ Ancestors (7)

1. [Distance between skew lines](distance-between-skew-lines.md)
2. [Skew lines](skew-lines.md)
3. [Euclidean geometry](euclidean-geometry-split.md)
4. [Geometry and topology](geometry-and-topology-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
