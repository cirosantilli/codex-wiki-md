<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $SU(4)$, [Dynkin labels](../../../../dynkin-label.md) $(a,b,c)$ correspond to a [Young diagram](../../../../young-diagram.md) with row lengths $(a+b+c,b+c,c)$. Numbered boxes below give representative [Young tableaux](../../../../young-tableau.md); they specify the shapes, not additional component values:

$$
\begin{array}{c|c|c|c}
\text{Dynkin labels}&\text{tableau}&\text{dimension}&\text{tensor realization}\\\hline
(1,0,0)&\boxed{1}&4&v^i\\[5pt]
(0,1,0)&\begin{array}{l}\boxed{1}\\[-3pt]\boxed{2}\end{array}&6&A^{ij}=-A^{ji}\\[8pt]
(0,0,1)&\begin{array}{l}\boxed{1}\\[-3pt]\boxed{2}\\[-3pt]\boxed{3}\end{array}&4&B^{ijk}=B^{[ijk]}\ \leftrightarrow\ b_i\\[11pt]
(1,0,1)&\begin{array}{l}\boxed{1}\,\boxed{2}\\[-3pt]\boxed{3}\\[-3pt]\boxed{4}\end{array}&15&X^i{}_j,\quad X^i{}_i=0
\end{array}
$$

Here the [dimensions](../../../../dimension-vector-space.md) are $4$, $\binom42=6$, $\binom43=4$, and $4^2-1=15$. The third is the [dual representation](../../../../dual-representation.md) $\overline{\mathbf4}$: the invariant volume [tensor](../../../../tensor.md) identifies $b_l=\epsilon_{lijk}B^{ijk}/3!$. The last is the [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md), equivalent to the shape $(2,1,1)$ [Young symmetrizer](../../../../young-symmetrizer.md) construction after converting its three-box column to one lower index and removing the [trace](../../../../matrix-trace.md).

For $U\in SU(4)$, the [tensor](../../../../tensor.md) transformation laws are

$$
\boxed{\begin{aligned}
v'^i&=U^i{}_jv^j,\\
A'^{ij}&=U^i{}_kU^j{}_lA^{kl},\\
B'^{ijk}&=U^i{}_lU^j{}_mU^k{}_nB^{lmn},\\
b'_i&=b_j(U^{-1})^j{}_i,\\
X'^i{}_j&=U^i{}_kX^k{}_l(U^{-1})^l{}_j.
\end{aligned}}
$$

These preserve antisymmetry and tracelessness. The [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md) can be treated as complex traceless [matrices](../../../../matrix.md); a real adjoint [scalar field](../../../../scalar-field.md) is conventionally represented by Hermitian traceless [matrices](../../../../matrix.md) with the same conjugation action.

Adding one box to the one-box [Young diagram](../../../../young-diagram.md) gives row shapes $(2)$ and $(1,1)$. Thus the first [tensor product](../../../../tensor-product.md) splits into the [symmetric square](../../../../symmetric-square.md) and [exterior square](../../../../exterior-square.md):

$$
\boxed{(1,0,0)\otimes(1,0,0)=(2,0,0)\oplus(0,1,0),\qquad
\mathbf4\otimes\mathbf4=\mathbf{10}\oplus\mathbf6.}
$$

Their [tensors](../../../../tensor.md) are respectively $S^{ij}=S^{ji}$ and $A^{ij}=-A^{ji}$. Adding one box to the three-box column gives shapes $(2,1,1)$ and $(1,1,1,1)$. The full four-box column is the [determinant representation](../../../../determinant-representation.md), trivial because $\det U=1$. Consequently

$$
\boxed{(1,0,0)\otimes(0,0,1)=(1,0,1)\oplus(0,0,0),\qquad
\mathbf4\otimes\overline{\mathbf4}=\mathbf{15}\oplus\mathbf1.}
$$

For a mixed [tensor](../../../../tensor.md) $T^i{}_j$, the corresponding pieces are $T^i{}_j-\tfrac14\delta^i{}_jT^k{}_k$ and $\tfrac14\delta^i{}_jT^k{}_k$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
