<h1 id="20c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write the amended primal as $\min c^{\mathsf T}x$ with $Ax\le b$, $x\ge0$. A convenient [linear programming duality](../../../../../../linear-programming-duality.md) convention uses $y\le0$ and gives $\max b^{\mathsf T}y$ subject to $A^{\mathsf T}y\le c$. Explicitly the dual is

$$
\begin{aligned}
\text{maximize }&5y_1+8y_2+5y_3,\\
\text{subject to }&-2y_1+4y_2+5y_3\le2,\\
&2y_1+2y_2-4y_3\le-3,\\
&4y_1-5y_2+\tfrac12y_3\le-5,\qquad y_1,y_2,y_3\le0.
\end{aligned}
$$

The optimal dual vector is the negative of the three payoff-row slack coefficients:

$$
\boxed{y^*=(-\tfrac{173}{120},-\tfrac{19}{120},-\tfrac1{20}),\qquad b^{\mathsf T}y^*=-\tfrac{349}{40}.}
$$

Indeed substitution gives $A^{\mathsf T}y^*=(2,-3,-5)^{\mathsf T}=c$, so all dual inequalities hold. To certify optimality directly by [weak duality](../../../../../../weak-duality.md), for any feasible primal and dual vectors,

$$
c^{\mathsf T}x\ge y^{\mathsf T}Ax\ge y^{\mathsf T}b,
$$

where the second inequality uses $Ax\le b$ and $y\le0$. Our feasible primal and dual vectors have equal values $-349/40$, so neither can be improved. This is a [linear programming optimality certificate](../../../../../../linear-programming-optimality-certificate.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [20C](../../20c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
