<h1 id="18h/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $(y,t)$ be a basic feasible solution of $R$. Part (ii) gives $t>0$, and put $x=y/t$. We already know that $x$ is feasible for $P$.

Suppose the columns $A_i$ with $y_i>0$ were linearly dependent. Then some nonzero $h$, supported on those indices, would satisfy $Ah=0$. Put

$$
q=d^Th,\qquad
\delta y=h-qy,\qquad
\delta t=-qt.
$$

Since $d^Ty=1$ and $Ay=bt$,

$$
d^T\delta y=0,
\qquad
A\delta y-b\delta t=0.
$$

The vector $(\delta y,\delta t)$ is nonzero and is supported only on positive variables of $(y,t)$. It is therefore a linear dependence among the active constraint columns of $R$, contradicting that $(y,t)$ is basic. Hence the active columns $A_i$ are linearly independent, and

$$
x=\frac yt\in\mathcal B.
$$

By the [Fundamental theorem of linear programming](../../../../../../../fundamental-theorem-of-linear-programming.md), $R$ has an optimal basic feasible solution. Its image $x\in\mathcal B$ has the same objective ratio, by part (ii). Conversely, every $x\in\mathcal B$ is feasible for $Q$ and maps to a feasible point of $R$. Since $x^*$ solves $Q$,

$$
\boxed{
\frac{c^Tx^*}{d^Tx^*}
=\max_{x\in\mathcal B}\frac{c^Tx}{d^Tx}
}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [18H](../../../18h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
