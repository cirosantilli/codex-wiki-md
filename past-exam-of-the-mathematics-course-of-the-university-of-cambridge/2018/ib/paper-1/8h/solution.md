<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

A [transportation problem](../../../../../transportation-problem.md) minimizes $\sum_{ij}c_{ij}x_{ij}$ subject to nonnegative shipments, prescribed row supplies, and prescribed column demands.

One optimal shipment table is

$$
\boxed{
\begin{pmatrix}
0&4&6\\
0&0&8\\
3&5&0
\end{pmatrix},}
$$

which has the required row sums $(10,8,8)$ and column sums $(3,9,14)$ and costs $4(3)+6(1)+8(3)+3(3)+5(5)=\boxed{76}$.

For an optimality certificate, take row potentials $(1,3,3)$ and column potentials $(0,2,0)$. Their sums equal costs in occupied cells and do not exceed any cost:

$$
\begin{pmatrix}1&3&1\\3&5&3\\3&5&3\end{pmatrix}
\leq
\begin{pmatrix}4&3&1\\6&10&3\\3&5&7\end{pmatrix}.
$$

The dual value is $10+24+24+18=76$, so [linear programming duality](../../../../../linear-programming-duality.md) proves optimality.

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
