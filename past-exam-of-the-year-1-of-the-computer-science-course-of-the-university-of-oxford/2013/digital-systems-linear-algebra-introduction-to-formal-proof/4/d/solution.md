<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Perform the [elementary row operations](../../../../../elementary-row-operation.md) **from the bottom upwards**:

$$
R_4\gets R_4-tR_3,\qquad R_3\gets R_3-tR_2,\qquad R_2\gets R_2-tR_1.
$$

This order matters because each subtraction uses the predecessor's original row. For example,

$$
(t^3,t^2,t,1)-t(t^2,t,1,t)=(0,0,0,1-t^2).
$$

The other two differences are $(0,0,1-t^2,t-t^3)$ and $(0,1-t^2,t-t^3,t^2-t^4)$. Thus the required [upper triangular matrix](../../../../../upper-triangular-matrix.md) is

$$
\boxed{U=\begin{pmatrix}
1&t&t^2&t^3\\
0&1-t^2&t(1-t^2)&t^2(1-t^2)\\
0&0&1-t^2&t(1-t^2)\\
0&0&0&1-t^2
\end{pmatrix}.}
$$

These [elementary row operations](../../../../../elementary-row-operation.md) use no division, so the reduction remains valid for all [real numbers](../../../../../real-number.md) $t$, including $t=\pm1$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
