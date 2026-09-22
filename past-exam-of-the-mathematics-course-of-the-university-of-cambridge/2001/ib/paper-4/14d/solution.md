<h1 id="14d/solution">Solution</h1>

↑ **Parent:** [14D](../14d.md)

Measure quantities in thousands of copies. Use five supply rows: initial inventory, regular production in month 1, overtime in month 1, regular production in month 2, overtime in month 2. Their supplies/capacities are $(10,40,150,40,150)$. The three demand columns are the two due dates and a dummy column for unused capacity, with demands $(40,60,290)$, balancing the total supply $390$.

The [transportation problem](../../../../../transportation-problem.md) has cost [matrix](../../../../../matrix.md)

$$
C=\begin{pmatrix}
0&20&40\\
400&420&0\\
450&470&0\\
\infty&400&0\\
\infty&450&0
\end{pmatrix}.
$$

An infinite entry prohibits delivering a later month's production to an earlier deadline. The extra $20$ in the second column of the early rows accounts for holding stock through the first month. For production rows, the dummy column represents capacity not used, not copies actually printed. Initial inventory assigned to the dummy column would instead remain in stock through both months, costing $40$; this distinguishes physical inventory from optional production capacity. No gratuitous disposal is needed in the optimum.

Let $x_{ij}\ge0$ have the stated row and column sums, with the forbidden entries zero, and minimize $\sum c_{ij}x_{ij}$. A feasible solution is

$$
\boxed{X=\begin{pmatrix}10&0&0\\30&10&0\\0&0&150\\0&40&0\\0&10&140\end{pmatrix}.}
$$

Thus regular production is $40$ in each month; overtime is zero then $10$; first-month closing inventory is $10$, and final inventory is zero. Its total production-plus-holding cost is

$$
\boxed{40(400)+40(400)+10(450)+10(20)=36{,}700.}
$$

To prove optimality, use [transportation dual potentials](../../../../../transportation-dual-potentials.md) $u=(-430,-30,0,-50,0)$ for rows and $v=(430,450,0)$ for columns. Every allowed edge satisfies $u_i+v_j\le c_{ij}$. Multiplying by any feasible shipment and summing gives the lower bound

$$
\sum c_{ij}x_{ij}\ge\sum_i u_i s_i+\sum_jv_jd_j
=-4300-1200-2000+17200+27000=36{,}700.
$$

The proposed shipment attains it, so the schedule is optimal. The dual calculation certifies the minimum without depending on an unshown transportation-simplex iteration.

## ↑ Ancestors (10)

1. [14D](../14d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
