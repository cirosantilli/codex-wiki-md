<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Back-substitute in the [Euclidean algorithm](../../../../../../../euclidean-algorithm.md) to obtain an [integer linear combination](../../../../../../../integer-linear-combination.md):

$$
\begin{aligned}
9&=45-36=45-(306-6\cdot45)\\
&=7\cdot45-306=7(657-2\cdot306)-306\\
&=7\cdot657-15\cdot306.
\end{aligned}
$$

Multiplying by $3$ gives the particular solution $(x_0,y_0)=(-45,21)$ of the [linear Diophantine equation](../../../../../../../linear-diophantine-equation.md). Subtracting it from any other solution and dividing by $9$ gives

$$
34(x+45)+73(y-21)=0.
$$

The [integers](../../../../../../../integer-split.md) $34$ and $73$ are [coprime](../../../../../../../coprime-integers.md), so $73$ divides $x+45$. Writing $x+45=73t$ forces $y-21=-34t$. Conversely these expressions satisfy the original equation for every [integer](../../../../../../../integer-split.md) $t$. Thus [all solutions of a linear Diophantine equation](../../../../../../../all-solutions-of-a-linear-diophantine-equation.md) here are

$$
\boxed{(x,y)=(-45+73t,\ 21-34t),\qquad t\in\mathbb Z.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics IV resit](../../../../mathematics-iv-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
