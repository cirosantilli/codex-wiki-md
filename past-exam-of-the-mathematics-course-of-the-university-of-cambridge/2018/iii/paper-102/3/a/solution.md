<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write an element of the diagonal [Cartan subalgebra](../../../../../../cartan-subalgebra.md) as

$$
H(t)=\operatorname{diag}(t_1,t_2,t_3,-t_1,-t_2,-t_3),\qquad
\varepsilon_i(H(t))=t_i.
$$

The [root system](../../../../../../root-system.md) of this [Special orthogonal Lie algebra](../../../../../../special-orthogonal-lie-algebra.md) is

$$
\boxed{\Phi=\{\pm\varepsilon_i\pm\varepsilon_j:1\leq i<j\leq3\}.}
$$

Thus the maps requested are $H(t)\mapsto\pm t_i\pm t_j$, with the two signs independent. This is the [D3 root system](../../../../../../d3-root-system.md), with twelve roots.

For a direct check, the defining matrix identity gives the block form $X=\begin{pmatrix}A&B\\C&-A^T\end{pmatrix}$ with $B^T=-B$ and $C^T=-C$. If $E_{ij}$ denotes a [matrix unit](../../../../../../matrix-unit.md), the [root space](../../../../../../root-space.md) for $\varepsilon_i-\varepsilon_j$ is spanned by $E_{ij}-E_{j+3,i+3}$; those for $\varepsilon_i+\varepsilon_j$ and $-\varepsilon_i-\varepsilon_j$ are spanned respectively by $E_{i,j+3}-E_{j,i+3}$ and $E_{i+3,j}-E_{j+3,i}$. Commuting these with $H(t)$ gives exactly the displayed maps.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
