# Four-tile mixed-boundary transplantation between a disk and a nonorientable surface

↑ **Parent:** [Transplantation theorem](transplantation-theorem.md)

Take four congruent octagonal [regular polygons](regular-polygon.md) with four alternate sides labelled $a,b,c,d$. The intervening sides have [Neumann boundary conditions](neumann-boundary-condition.md). Pair equal face parameters in the positive reference boundary direction. The complete gluing data are

$$
\begin{array}{c|c|c|c|c}
\text{face}&\text{pairs in }D&\text{Dirichlet tiles in }D&\text{pairs in }B&\text{Dirichlet tiles in }B\\ \hline
a&23&\varnothing&13&\varnothing\\
b&12&\varnothing&12&\varnothing\\
c&01&\{2,3\}&02&\{1,3\}\\
d&\varnothing&\{1,3\}&01,\ 23&\varnothing
\end{array}
$$

All unpaired labelled faces not in a Dirichlet column also have [Neumann boundary conditions](neumann-boundary-condition.md). Encode these rules by [signed permutation matrices](signed-permutation-matrix.md), using a positive swap for a paired interface and diagonal $-1$ or $+1$ for an unpaired [Dirichlet boundary condition](dirichlet-boundary-condition.md) or [Neumann boundary condition](neumann-boundary-condition.md). The four-by-four [Hadamard matrix](hadamard-matrix.md) $C$ above satisfies $CM_s=N_sC$ for every label. Explicitly, if its columns are $h_0,h_1,h_2,h_3$, applying $N_a,N_b,N_c,N_d$ gives respectively $(h_0,h_1,h_3,h_2)$, $(h_0,h_2,h_1,h_3)$, $(h_1,h_0,-h_2,-h_3)$, and $(h_0,-h_1,h_2,-h_3)$, which are exactly the columns of the corresponding $CM_s$. On every intervening face the face matrix is the identity.

Since $C^TC=4I$, the [orthogonal matrix](orthogonal-matrix.md) $C/2$ preserves the $L^2$ [inner product](inner-product.md) and the sum of Dirichlet energies. Its intertwining relations map matching [Sobolev traces](trace-operator.md) and zero Dirichlet traces bijectively to those of the other assembly. It therefore preserves the [quadratic form](quadratic-form.md) domains and the forms themselves. The associated [self-adjoint operators](self-adjoint-operator.md) are unitarily equivalent, proving equality of all [eigenvalues](eigenvalue.md) with their [multiplicities](multiplicity-mathematics.md) for the specified [mixed boundary conditions](mixed-boundary-condition.md).

The [topology of disk tiles glued along disjoint boundary arcs](topology-of-disk-tiles-glued-along-disjoint-boundary-arcs.md) shows that $D$, whose gluing [graph](graph-split.md) is $0,1,2,3$ in a path, is a [closed disc](closed-disc.md) and is [simply connected](simply-connected-space.md) and [orientable](orientable-surface.md). The gluing [graph](graph-split.md) of $B$ has edges $13,12,02,01,23$; it is connected with two independent cycles, so $\chi(B)=-1$ and $\pi_1(B)\cong F_2$. Its odd cycle $1,2,3,1$ makes it a [nonorientable surface](non-orientable-surface.md). Each assembled surface has nonempty polygonal boundary. This explicitly realizes isospectrality between a simply-connected orientable bordered surface and a nonorientable, non-simply-connected one. The boundary corners and [mixed boundary conditions](mixed-boundary-condition.md) are essential qualifications; it does not contradict the [Euler characteristic from the heat trace of a bordered surface](euler-characteristic-from-the-heat-trace-of-a-bordered-surface.md) for smooth boundaries and pure boundary conditions.

## ↑ Ancestors (9)

1. [Transplantation theorem](transplantation-theorem.md)
2. [Isospectral manifolds](isospectral-manifolds.md)
3. [Spectral geometry](spectral-geometry.md)
4. [Riemannian geometry](riemannian-geometry-split.md)
5. [Differential geometry](differential-geometry-split.md)
6. [Geometry and topology](geometry-and-topology-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Hadamard matrix](hadamard-matrix.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-19/2/solution.md)
