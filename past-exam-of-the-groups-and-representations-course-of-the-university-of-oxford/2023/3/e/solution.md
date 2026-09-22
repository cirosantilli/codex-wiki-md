<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Number the [simple roots](../../../../simple-root.md) of the $A_4$ [root system](../../../../root-system.md) consecutively along its [Dynkin diagram](../../../../dynkin-diagram.md). For a [Young diagram](../../../../young-diagram.md) with row lengths $r_i$, its [highest weight](../../../../highest-weight-of-a-representation.md) has [Dynkin labels](../../../../dynkin-label.md) $a_i=r_i-r_{i+1}$. The three [irreducible representations](../../../../irreducible-representation.md) have the following [Young diagrams](../../../../young-diagram.md), which can be filled increasingly down the column to give [Young tableaux](../../../../young-tableau.md):

$$
\begin{array}{c|c|c|c}
&\text{column of boxes}&\text{tensor}&\text{highest-weight labels}\\\hline
\mathbf5&\boxed{1}&v^i&(1,0,0,0)\\
\overline{\mathbf5}&\begin{matrix}\boxed{1}\\\boxed{2}\\\boxed{3}\\\boxed{4}\end{matrix}
&w^{[i_1i_2i_3i_4]}\ \text{or }\widetilde v_i&(0,0,0,1)\\
\mathbf{10}&\begin{matrix}\boxed{1}\\\boxed{2}\end{matrix}
&T^{ij}=-T^{ji}&(0,1,0,0)
\end{array}
$$

Here $i=1,\ldots,5$, $v^i\mapsto U^i{}_jv^j$, and $T^{ij}\mapsto U^i{}_kU^j{}_lT^{kl}$. Contraction with the invariant alternating [tensor](../../../../tensor.md) identifies $\widetilde v_i=(1/4!)\epsilon_{ii_1i_2i_3i_4}w^{i_1i_2i_3i_4}$, giving the [dual representation](../../../../dual-representation.md) of $\mathbf5$. The dimensions follow from $\binom51=5$, $\binom54=5$, $\binom52=10$.

Use the [centralizer](../../../../centralizer.md) and [circle group](../../../../circle-group.md) normalization of [solution](../d/solution.md). The first three components have [U(1) charge](../../../../u-1-charge.md) $-2$ and the last two have [U(1) charge](../../../../u-1-charge.md) $3$, so the [branching of a representation](../../../../branching-of-a-representation.md) is

$$
\boxed{\mathbf5\longrightarrow(\mathbf3,\mathbf1)_{-2}\oplus(\mathbf1,\mathbf2)_3,\qquad
\overline{\mathbf5}\longrightarrow(\overline{\mathbf3},\mathbf1)_2\oplus(\mathbf1,\mathbf2)_{-3}.}
$$

For the [dual representation](../../../../dual-representation.md), both [U(1) charges](../../../../u-1-charge.md) reverse and the $SU(3)$ [representation](../../../../group-representation.md) is conjugated; the $SU(2)$ doublet is equivalent to its conjugate. Taking the [exterior square](../../../../exterior-square.md) of the first decomposition gives three types of antisymmetric [tensor](../../../../tensor.md) components: $T^{ab}$, $T^{a\alpha}$, and $T^{\alpha\beta}$, where $a,b=1,2,3$ and $\alpha,\beta=4,5$. Their [U(1) charges](../../../../u-1-charge.md) add, and $\Lambda^2\mathbf3=\overline{\mathbf3}$, $\Lambda^2\mathbf2=\mathbf1$. Hence

$$
\boxed{\mathbf{10}\longrightarrow
(\overline{\mathbf3},\mathbf1)_{-4}\oplus(\mathbf3,\mathbf2)_1\oplus(\mathbf1,\mathbf1)_6.}
$$

The dimensions are $3+6+1=10$. These product labels describe genuine [representations](../../../../group-representation.md) of the quotient [group](../../../../group-split.md) in [solution](../d/solution.md): every element of its $\mathbb Z_6$ [kernel](../../../../kernel-of-a-linear-map-split.md) acts trivially on each summand.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
