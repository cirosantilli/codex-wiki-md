<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We construct the two domains explicitly from seven congruent [triangles](../../../../../triangle.md). Let a scalene reference [triangle](../../../../../triangle.md) have sides $a,b,c$ opposite its three labelled vertices. Choose its three side lengths in a small open neighbourhood of $(1,1,1)$, with a fixed strict ordering. Thus the three angles are distinct and lie between $\pi/4$ and $\pi/2$. Each copy keeps these side labels.

For the first assembly glue the following tile pairs, reflecting across the indicated side:

$$
\begin{array}{c|c|c}
\text{side}&\Omega_P&\Omega_L\\ \hline
a&(2,3),(6,7)&(1,3),(5,7)\\
b&(4,6),(5,7)&(2,6),(3,7)\\
c&(1,5),(3,7)&(4,5),(6,7)
\end{array}
$$

Each coloured adjacency graph is a tree with central tile $7$ and three two-tile arms. Place tile $7$ in the plane and obtain every other tile by the prescribed reflections. At the equilateral reference shape the copies have disjoint interiors and form a polygonal disk; the same holds throughout a sufficiently small neighbourhood, since the only contacts between tiles are the prescribed edges and their incident vertices. In particular each assembly is a bounded connected [planar domain](../../../../../planar-domain.md).

<a id="2/image-seven-triangle-point-and-line-assemblies-with-matching-dirichlet-spectra"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-20-drums.png)

**[Figure 1](#2/image-seven-triangle-point-and-line-assemblies-with-matching-dirichlet-spectra). Seven-triangle point and line assemblies with matching Dirichlet spectra**.

To prove equality of spectra, index tiles by the seven nonzero [vectors](../../../../../vector.md) $x\in\mathbb F_2^3$, using $x=(x_1,x_2,x_3)$ with label $x_1+2x_2+4x_3$. Let

$$
s_a=I+E_{12},\qquad s_b=I+E_{23},\qquad s_c=I+E_{31}.
$$

These [involutions](../../../../../involution.md) act on points by $x\mapsto s_sx$ and on nonzero [covectors](../../../../../covector.md) by $y\mapsto s_s^{-T}y=s_s^Ty$. Their swaps are exactly the two columns of the table. Write $P_s,Q_s$ for the corresponding permutation [matrices](../../../../../matrix.md). The [Fano plane](../../../../../fano-plane.md) incidence [matrix](../../../../../matrix.md)

$$
B_{y,x}=\mathbf1_{y\cdot x=0}
$$

satisfies $BP_s=Q_sB$, since incidence is preserved by a linear transformation and its inverse transpose. Each point lies on three lines, while two different points have one common line. Therefore

$$
B^TB=2I+J,
$$

where $J$ is the all-ones [matrix](../../../../../matrix.md), proving that $B$ is invertible.

For the [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md), a glued side has a positive swap and an exposed side has diagonal entry $-1$. Both trees have the same bipartition, with sign [matrix](../../../../../matrix.md)

$$
D=\operatorname{diag}(1,1,-1,1,-1,-1,1).
$$

Their signed reflection [matrices](../../../../../matrix.md) are $M_s=-DP_sD$ and $N_s=-DQ_sD$. On a glued edge its endpoint signs are opposite, so the off-diagonal entries are $+1$; on an exposed edge the entry is $-1$. Consequently the [invertible matrix](../../../../../invertible-matrix.md) $C=DBD$ satisfies

$$
CM_s=N_sC\qquad(s=a,b,c).
$$

We spell out why this gives [isospectrality](../../../../../isospectral-manifolds.md). Pull each function back from the seven tiles to the reference [triangle](../../../../../triangle.md). Its seven boundary values along side $s$ form a [vector](../../../../../vector.md) $u_s$ satisfying $M_su_s=u_s$: this imposes equal values at glued edges and zero values at exposed edges. Outward [normal derivatives](../../../../../normal-derivative.md) of a smooth [eigenfunction](../../../../../eigenfunction.md) satisfy $M_sv_s=-v_s$, giving opposite [normal derivatives](../../../../../normal-derivative.md) on glued edges. The identities above preserve both conditions under $u\mapsto Cu$. Since $C$ is constant, it also commutes with the [scalar](../../../../../scalar.md) [Laplacian](../../../../../laplacian.md) on each [triangle](../../../../../triangle.md).

One can include all weak [eigenfunctions](../../../../../eigenfunction.md) without any corner regularity issue by [orthogonalization of a transplantation matrix](../../../../../orthogonalization-of-a-transplantation-matrix.md). The [matrix](../../../../../matrix.md) $C^TC$ commutes with the symmetric $M_s$, so $O=C(C^TC)^{-1/2}$ is orthogonal and still intertwines $M_s,N_s$. On the disjoint tiles, $O$ preserves the $L^2$ norm and the sum of the [Dirichlet energies](../../../../../dirichlet-energy.md); it maps the [trace](../../../../../matrix-trace.md)-matching form domain $H_0^1(\Omega_P)$ bijectively to $H_0^1(\Omega_L)$. Thus it is a [unitary equivalence](../../../../../unitary-equivalence.md) of the [Dirichlet Laplacians](../../../../../dirichlet-laplacian.md), proving equality of every [eigenvalue](../../../../../eigenvalue.md) with its multiplicity.

Finally, the only reentrant vertices of either polygon are the three vertices of tile $7$, with interior angles four times the corresponding reference-[triangle](../../../../../triangle.md) angles. All other boundary angles are less than $\pi$. These three distinct angles force any hypothetical [isometry](../../../../../isometry.md) to map each labelled central vertex to its counterpart. An [isometry](../../../../../isometry.md) between connected open [planar domains](../../../../../planar-domain.md) is a restriction of a rigid motion: its derivative is orthogonal, and preservation of the flat [Levi-Civita connection](../../../../../levi-civita-connection.md) makes that derivative constant. After aligning the two central [triangles](../../../../../triangle.md), this rigid motion fixes three noncollinear points and is the identity. But the two domains do not coincide: the tile beyond side $a$ of the central [triangle](../../../../../triangle.md) has its next attachment along $b$ in the point assembly and along $c$ in the line assembly. These occupy different open regions. This contradiction proves nonisometry.

Therefore **the three freely varying side lengths give a three-parameter family of nonisometric Dirichlet-isospectral bounded [planar domains](../../../../../planar-domain.md)**. The parameters include scale; no congruence normalization removes it.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
