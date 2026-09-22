<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The initial [vector](../../../../../vector.md) records both initial [Fibonacci numbers](../../../../../fibonacci-number.md): $V_1=(U_2,U_1)^\top=(1,1)^\top$. For $n\ge2$,

$$
AV_{n-1}=\begin{pmatrix}1&1\\1&0\end{pmatrix}\begin{pmatrix}U_n\\U_{n-1}\end{pmatrix}=\begin{pmatrix}U_n+U_{n-1}\\U_n\end{pmatrix}=V_n.
$$

Conversely this [vector](../../../../../vector.md) recurrence forces the second component to be the preceding first component and forces their sum to be the next first component, recovering the [scalar](../../../../../scalar.md) recurrence and its initial conditions. Iterating, or using [mathematical induction](../../../../../mathematical-induction.md), yields **$V_n=A^{n-1}(1,1)^\top$** for every $n\ge1$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
