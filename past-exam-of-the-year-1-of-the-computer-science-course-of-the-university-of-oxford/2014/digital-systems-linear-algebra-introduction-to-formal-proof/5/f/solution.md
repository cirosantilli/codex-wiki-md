<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [reduced row echelon form](../../../../../reduced-row-echelon-form.md) yields

$$
x_1-2x_2-x_4+3x_5=0,\qquad x_3+2x_4-2x_5=0.
$$

Take the [free variables in a linear system](../../../../../free-variable-in-a-linear-system.md) to be $s=x_2$, $t=x_4$, $u=x_5$. Then

$$
x=s\begin{pmatrix}2\\1\\0\\0\\0\end{pmatrix}+t\begin{pmatrix}1\\0\\-2\\1\\0\end{pmatrix}+u\begin{pmatrix}-3\\0\\2\\0\\1\end{pmatrix}.
$$

Thus

$$
\boxed{\text{null-space basis }\{(2,1,0,0,0)^{\mathsf T},(1,0,-2,1,0)^{\mathsf T},(-3,0,2,0,1)^{\mathsf T}\},\qquad\dim\operatorname{Null}(A)=3.}
$$

Each listed [vector](../../../../../vector.md) lies in the [null space](../../../../../kernel-of-a-linear-map-split.md), and every solution has the displayed form. Their coordinates in positions 2, 4 and 5 prove [linear independence](../../../../../linear-independence.md). The dimension also follows from the [rank-nullity theorem](../../../../../rank-nullity-theorem.md): $5-2=3$.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
