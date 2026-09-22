<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The reduced [row echelon form](../../../../../row-echelon-form.md) gives

$$
x_1+x_3+x_4=0,\qquad x_2-x_3+x_4=0.
$$

Choose the free variables $x_3=s,x_4=t$. Then

$$
x=s\begin{pmatrix}-1\\1\\1\\0\end{pmatrix}+t\begin{pmatrix}-1\\-1\\0\\1\end{pmatrix}.
$$

The coefficient [vectors](../../../../../vector.md) are [linearly independent](../../../../../linear-independence.md), because their third and fourth entries give independent coordinates. Consequently

$$
\boxed{\operatorname{Null}(A)\text{ has basis }\left\{\begin{pmatrix}-1\\1\\1\\0\end{pmatrix},\begin{pmatrix}-1\\-1\\0\\1\end{pmatrix}\right\},\qquad\dim\operatorname{Null}(A)=2.}
$$

Substitution in the original [matrix](../../../../../matrix.md) verifies $Ax=0$ for both [basis vectors](../../../../../basis-vector.md). The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) supplies the independent dimension check $2+2=4$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [5](../../5.md)
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
