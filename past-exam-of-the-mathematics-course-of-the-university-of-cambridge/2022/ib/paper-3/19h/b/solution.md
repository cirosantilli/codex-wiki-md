<h1 id="19h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The stated plan is

$$
X=
\begin{pmatrix}
3&0&3&0\\
0&4&0&0\\
0&1&4&3
\end{pmatrix}.
$$

Its six positive cells form a spanning tree of the supplier--consumer bipartite graph, so it is basic and feasible. Taking $u_1=0$, the basic-cell equations $u_i+v_j=c_{ij}$ give

$$
u=(0,-4,-3),
\qquad v=(1,5,4,4).
$$

The complete matrix of [reduced costs](../../../../../../reduced-cost.md) $\bar c_{ij}=c_{ij}-u_i-v_j$ is

$$
\overline C=
\begin{pmatrix}
0&-2&0&2\\
4&0&2&4\\
6&0&0&0
\end{pmatrix}.
$$

The negative entry $\bar c_{12}=-2$ proves that the plan is not optimal.

Enter cell $(1,2)$. The alternating cycle is

$$
(1,2)^+,(1,3)^-,(3,3)^+,(3,2)^-,
$$

and the step is $\theta=\min(3,1)=1$. The new plan is

$$
X'=
\begin{pmatrix}
3&1&2&0\\
0&4&0&0\\
0&0&5&3
\end{pmatrix},
$$

whose cost is $26$, down from $28$. New potentials are

$$
u=(0,-2,-3),
\qquad v=(1,3,4,4),
$$

and the reduced-cost matrix is

$$
\overline C'=
\begin{pmatrix}
0&0&0&2\\
2&0&0&2\\
6&2&0&0
\end{pmatrix}.
$$

Every reduced cost is nonnegative, so the [transportation optimality criterion](../../../../../../transportation-problem.md) shows that

$$
\boxed{X'\text{ is optimal, with total cost }26}.
$$

The zero reduced cost in cell $(2,3)$ also indicates an alternative optimum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19H](../../19h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
