<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the [transition matrix](../../../../../stochastic-matrix.md) once and then again:

$$
x(1)=P\begin{pmatrix}1\\1\\8\end{pmatrix}=\begin{pmatrix}1/2+1/2+4\\1/4+1/2\\1/4+4\end{pmatrix}=\begin{pmatrix}5\\3/4\\17/4\end{pmatrix},
$$



$$
x(2)=P\begin{pmatrix}5\\3/4\\17/4\end{pmatrix}=\begin{pmatrix}5\\5/4+3/8\\5/4+17/8\end{pmatrix}=\begin{pmatrix}5\\13/8\\27/8\end{pmatrix}.
$$

Therefore, in USA, Europe, Rest of World order and in trillions of dollars,

$$
\boxed{x(1)=(5,0.75,4.25)^{\mathsf T},\qquad x(2)=(5,1.625,3.375)^{\mathsf T}.}
$$

Each total remains ten, giving a quick check on the [matrix multiplication](../../../../../matrix-multiplication.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
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
