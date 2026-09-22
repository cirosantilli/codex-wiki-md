<h1 id="t/t2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The dual prices $u,v\geq0$ solve

$$
\boxed{\min 6u+11v,\qquad4u+2v\geq5,\quad2u+3v\geq6,\quad2v\geq3.}
$$

The optimal tableau gives $(u,v)=c_B^TB^{-1}=(6,3)B^{-1}=(3/4,3/2)$. This [vector](../../../../../vector.md) is dual feasible and has objective $21$, equal to the primal value, proving optimality.

Thus an extra unit of R is worth $3/4$ while the current [basis](../../../../../basis.md) stays feasible. Increasing its supply by $\delta$ changes the basic values to

$$
B^{-1}\begin{pmatrix}6+\delta\\11\end{pmatrix}
=\begin{pmatrix}3+\delta/2\\1-3\delta/4\end{pmatrix}.
$$

For increases, feasibility is retained exactly up to $\delta=4/3$. Therefore the firm can buy **up to $4/3$ extra units at a marginal value of $3/4$ per unit**. The reduced profits do not change during this right-hand-side variation.

For the proposed fourth good, the reduced profit is $8-(4u+4v)=8-9=-1$. Its profit is below the resource opportunity cost, so **it is not worth producing at the current optimum**. The old dual solution also satisfies the new good's inequality, certifying that introducing it cannot improve the optimum.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [T2](../../t2.md)
3. [T](../../../t.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
