<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

Let $x_{ij}\geq0$ be shipments, with column sums eight and row sums at most the four capacities. Total demand is $32$, below total capacity $36$, so unused capacity is allowed. This is a [transportation problem](../../../../../transportation-problem.md) with capacity inequalities; equivalently add a dummy shop demanding four units with zero shipping cost.

Using the original PDF's cost $c_{12}=10$, take the [feasible solution](../../../../../feasible-point.md)

$$
\boxed{X=\begin{pmatrix}0&0&0&7\\8&0&0&0\\0&7&0&1\\0&1&8&0\end{pmatrix}.}
$$

Its row totals are $(7,8,8,9)$ and all column totals are eight. Four units of capacity remain unused at the second factory. Its shipping cost is $35+32+28+2+7+16=\boxed{120}$.

To prove that the cost is a [global minimum](../../../../../global-minimum.md), use the [transportation dual certificate with capacity inequalities](../../../../../transportation-dual-certificate-with-capacity-inequalities.md). If row potentials satisfy $u_i\leq0$ and $u_i+v_j\leq c_{ij}$, every [feasible solution](../../../../../feasible-point.md) satisfies

$$
\sum_{i,j}c_{ij}x_{ij}\geq\sum_i u_i\sum_jx_{ij}+\sum_jv_j\sum_ix_{ij}\geq\sum_i u_i s_i+8\sum_jv_j,
$$

where $s=(7,12,8,9)$. The second inequality uses the sign of $u_i$: multiplying a capacity upper bound by a nonpositive number reverses it. Choose $u=(0,0,-3,0)$ and $v=(4,7,2,5)$. The [reduced costs](../../../../../reduced-cost.md) are

$$
(c_{ij}-u_i-v_j)=\begin{pmatrix}2&3&1&0\\0&1&4&7\\2&0&10&0\\1&0&0&1\end{pmatrix},
$$

so every entry is nonnegative. The lower bound is $-24+8(4+7+2+5)=120$, equal to the displayed shipping cost. **The minimum shipping cost is $120$.**

For the [production costs in a transportation problem](../../../../../production-costs-in-a-transportation-problem.md), add the production cost of each factory to every real shipment from that factory. Unused capacity incurs no production cost, so the dummy-shop costs remain zero. The resulting real-shop cost matrix is

$$
C'=\begin{pmatrix}9&13&6&8\\6&10&8&14\\7&8&13&6\\10&12&7&11\end{pmatrix}.
$$

A [feasible solution](../../../../../feasible-point.md) is

$$
\boxed{X'=\begin{pmatrix}0&0&3&4\\8&4&0&0\\0&4&0&4\\0&0&5&0\end{pmatrix}.}
$$

Its row totals are $(7,12,8,5)$ and column totals remain eight, leaving four units unused at the fourth factory. Its combined cost is $18+32+48+40+32+24+35=229$.

For a matching [transportation dual certificate with capacity inequalities](../../../../../transportation-dual-certificate-with-capacity-inequalities.md), take $u'=(-1,-1,-3,0)$ and $v'=(7,11,7,9)$. Their [reduced costs](../../../../../reduced-cost.md) are

$$
(C'_{ij}-u'_i-v'_j)=\begin{pmatrix}3&3&0&0\\0&0&2&6\\3&0&9&0\\3&1&0&2\end{pmatrix},
$$

all nonnegative. The lower bound is $-7-12-24+8(7+11+7+9)=229$. Thus **the minimum combined production and shipping cost is $229$**, and the second allocation attains it.

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
