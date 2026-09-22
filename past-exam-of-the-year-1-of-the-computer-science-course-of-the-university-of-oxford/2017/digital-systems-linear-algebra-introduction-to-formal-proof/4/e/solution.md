<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [Gram-Schmidt process](../../../../../gram-schmidt-process.md) first gives $u_1=a_1=(1,1,1,1)^T$, of norm two. Next $a_1^Ta_2/(a_1^Ta_1)=2$, so

$$
u_2=a_2-2u_1=(1,-1,-1,1)^T.
$$

For the third column, both coefficients onto $u_1,u_2$ equal one, giving

$$
u_3=a_3-u_1-u_2=(1,-1,1,-1)^T.
$$

These three nonzero vectors are mutually [orthogonal](../../../../../orthogonal-vectors.md) and each has norm two. The resulting [orthonormal basis](../../../../../orthonormal-basis.md) is

$$
\boxed{q_1=\frac12\begin{pmatrix}1\\1\\1\\1\end{pmatrix},\quad
q_2=\frac12\begin{pmatrix}1\\-1\\-1\\1\end{pmatrix},\quad
q_3=\frac12\begin{pmatrix}1\\-1\\1\\-1\end{pmatrix}.}
$$

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
