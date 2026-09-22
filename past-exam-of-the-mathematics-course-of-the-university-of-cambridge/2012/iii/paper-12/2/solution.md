<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Consider two finite assemblies of the same number $n$ of congruent bounded Euclidean tiles. Label their matching faces so the same prescribed face identifications are used in both assemblies. For each face type $c$, encode the first assembly by a symmetric involution $A_c$: a paired face exchanges its two tile indices, an exterior [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) contributes diagonal $-1$, and an exterior [Neumann boundary condition](../../../../../neumann-boundary-condition.md) contributes diagonal $+1$. Let $B_c$ encode the second assembly. Face coordinates are pulled back to the same reference face; if identifications have additional face isometries, these pullbacks must be included in the intertwining operators.

The [transplantation theorem](../../../../../transplantation-theorem.md) says that a constant matrix $C$ with $CA_c=B_cC$ for every face type sends the vector of tile restrictions of a [Laplacian eigenfunction](../../../../../laplacian-eigenfunction.md) on the first assembly to one on the second, by $g=Cf$. If $C$ is invertible, it is a [bijection](../../../../../bijection.md) of each [eigenspace](../../../../../eigenspace.md) and the assemblies are isospectral with multiplicities.

To prove it, each component solves the same interior equation $\Delta f_j=\lambda f_j$, and a constant linear combination solves that equation too. On a face, let $u$ be the vector of boundary values and $v$ the vector of outward [normal derivatives](../../../../../normal-derivative.md). All matching and exterior conditions are exactly

$$
A_cu=u,\qquad A_cv=-v.
$$

For an internal face these equations say that values agree and the two outward derivatives sum to zero. For diagonal $-1$ they impose zero value, and for diagonal $+1$ zero [normal derivative](../../../../../normal-derivative.md). The intertwining identity gives $B_c(Cu)=Cu$ and $B_c(Cv)=-Cv$, so the transplanted functions match and satisfy the correct [boundary conditions](../../../../../boundary-condition.md). Applying $C^{-1}$ proves the [eigenspace](../../../../../eigenspace.md) [bijection](../../../../../bijection.md). At corners the same reasoning is interpreted in the finite-energy weak domain: no value jump and cancellation of normal flux prevent an extra distributional source. It gives the usual self-adjoint Dirichlet/mixed Laplacians on polygonal assemblies.

Here is an explicit [transplantation by reflection parity](../../../../../transplantation-by-reflection-parity.md). Take a rectangle of width $2a$ and height $b$, with the [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) on every exterior side. Cut it at its vertical midline into two congruent half-rectangles, pulling the right-hand half back by reflection. The midline gluing matrix is

$$
S=\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

Replace the connected assembly by the disjoint union of two width-$a$, height-$b$ rectangles: the first has Dirichlet conditions on all sides; the second has Dirichlet on three sides and Neumann on the side representing the cut. Its corresponding matrix is $D=\operatorname{diag}(-1,1)$. The invertible, indeed orthogonal, matrix

$$
\boxed{C=\frac1{\sqrt2}\begin{pmatrix}1&-1\\1&1\end{pmatrix},\qquad CS=DC}
$$

intertwines the midline conditions. Every other face has matrix $-I$ on both assemblies, which automatically intertwines. The [transplantation theorem](../../../../../transplantation-theorem.md) proves equality of the complete [spectra](../../../../../spectrum-functional-analysis.md), although **one surface is connected and the other has two components with the required uniform and mixed conditions**.

Equivalently, odd reflection [eigenfunctions](../../../../../eigenfunction.md) vanish on the cut, while even reflection [eigenfunctions](../../../../../eigenfunction.md) have zero [normal derivative](../../../../../normal-derivative.md) there. A direct separation-of-variables check gives the connected rectangle's [eigenvalues](../../../../../eigenvalue.md)

$$
\pi^2\left(\frac{m^2}{4a^2}+\frac{n^2}{b^2}\right),\qquad m,n\geq1.
$$

Even $m=2j$ gives the fully Dirichlet half-rectangle [spectrum](../../../../../spectrum-functional-analysis.md), and odd $m=2j+1$, $j\geq0$, gives the mixed half-rectangle [spectrum](../../../../../spectrum-functional-analysis.md). The split preserves every multiplicity, including coincidences between different pairs of indices.

<a id="2/image-reflection-splits-a-connected-dirichlet-rectangle-into-a-disjoint-dirichlet-rectangle-and-a-mixed-dirichlet-neumann-rectangle"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-12-reflection-transplantation.png)

**[Figure 1](#2/image-reflection-splits-a-connected-dirichlet-rectangle-into-a-disjoint-dirichlet-rectangle-and-a-mixed-dirichlet-neumann-rectangle). Reflection splits a connected Dirichlet rectangle into a disjoint Dirichlet rectangle and a mixed Dirichlet-Neumann rectangle**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
