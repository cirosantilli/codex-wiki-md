<h1 id="15h/solution">Solution</h1>

↑ **Parent:** [15H](../15h.md)

A balanced [transportation problem](../../../../../transportation-problem.md) chooses nonnegative shipments $x_{ij}$ minimizing $\sum_{ij}c_{ij}x_{ij}$, subject to $\sum_jx_{ij}=s_i$ and $\sum_ix_{ij}=d_j$, where the total supply equals total demand. For multipliers $u_i,v_j$, its [Lagrangian](../../../../../lagrangian.md) is

$$
\mathcal L=\sum_{ij}c_{ij}x_{ij}+\sum_i u_i\left(s_i-\sum_jx_{ij}\right)+\sum_jv_j\left(d_j-\sum_ix_{ij}\right)=\sum_i u_is_i+\sum_jv_jd_j+\sum_{ij}(c_{ij}-u_i-v_j)x_{ij}.
$$

Taking its infimum over $x_{ij}\geq0$ produces the [linear programming duality](../../../../../linear-programming-duality.md) problem of maximizing $\sum_i u_is_i+\sum_jv_jd_j$ subject to $u_i+v_j\leq c_{ij}$. These are the [transportation dual potentials](../../../../../transportation-dual-potentials.md).

The [transportation simplex algorithm](../../../../../transportation-simplex-algorithm.md) starts with a feasible [transportation spanning tree](../../../../../transportation-spanning-tree.md) of $m+n-1$ basic entries, obtainable by filling the north-west available cell with the smaller remaining supply or demand. Set $u_i+v_j=c_{ij}$ on basic cells; this determines all potentials up to adding a constant to all $u_i$ and subtracting it from all $v_j$. If all nonbasic reduced costs $r_{ij}=c_{ij}-u_i-v_j$ are nonnegative, feasibility and the dual bound prove optimality. Otherwise let a negative-cost cell enter. It closes a unique cycle in the basic tree. Alternate additions and subtractions around that cycle and choose the largest amount preserving nonnegativity, namely the minimum shipment on the subtraction cells. A cell that reaches zero leaves the basis. The cost changes by the entering reduced cost times the pivot amount. Zero basic cells and an anti-cycling rule can handle degeneracy; all pivots below are nondegenerate.

The north-west initial shipment matrix is

$$
X_0=\begin{pmatrix}14&22&0\\0&46&38\\0&0&40\end{pmatrix},\qquad C_0=1156.
$$

With $u_1=0$, its [transportation dual potentials](../../../../../transportation-dual-potentials.md) are $u=(0,1,0)$ and $v=(5,9,5)$. The most negative reduced cost is $r_{32}=-7$. The cycle is $+(3,2),-(3,3),+(2,3),-(2,2)$; the pivot amount is $\min(40,46)=40$. Hence

$$
X_1=\begin{pmatrix}14&22&0\\0&6&78\\0&40&0\end{pmatrix},\qquad C_1=1156-7\cdot40=876.
$$

Now $u=(0,1,-7)$ and $v=(5,9,5)$. Enter $(1,3)$, of reduced cost $-4$, on cycle $+(1,3),-(1,2),+(2,2),-(2,3)$. The amount is $\min(22,78)=22$, giving

$$
X_2=\begin{pmatrix}14&0&22\\0&28&56\\0&40&0\end{pmatrix},\qquad C_2=876-4\cdot22=788.
$$

The new potentials are $u=(0,5,-3)$ and $v=(5,5,1)$. Enter $(2,1)$, of reduced cost $-7$, on cycle $+(2,1),-(1,1),+(1,3),-(2,3)$. The amount is $\min(14,56)=14$. Thus

$$
\boxed{X_* =\begin{pmatrix}0&0&36\\14&28&42\\0&40&0\end{pmatrix},\qquad C_*=788-7\cdot14=690.}
$$

To certify optimality in the original [transportation problem](../../../../../transportation-problem.md), take $u=(0,5,-3)$ and $v=(-2,5,1)$. Their entire reduced-cost matrix is

$$
(c_{ij}-u_i-v_j)=\begin{pmatrix}7&4&0\\0&0&0\\12&0&7\end{pmatrix}\geq0.
$$

They satisfy [dual feasibility](../../../../../dual-feasibility.md), and their value is $5\cdot84-3\cdot40-2\cdot14+5\cdot68+78=690$, equal to the shipment cost. **The minimum transportation cost is therefore $690$**, with no unproved optimality assertion from the iterations alone.

## ↑ Ancestors (10)

1. [15H](../15h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
