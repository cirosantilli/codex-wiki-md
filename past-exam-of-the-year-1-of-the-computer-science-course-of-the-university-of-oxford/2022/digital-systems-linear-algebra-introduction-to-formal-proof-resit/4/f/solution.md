<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The initial vector decomposes especially simply in the [eigenbasis](../../../../../eigenbasis.md):

$$
\begin{pmatrix}1\\2\end{pmatrix}=v_\varphi+v_\psi,
$$

because $\varphi+\psi=1$. Applying $A^n$ multiplies the two [eigenvectors](../../../../../eigenvector.md) by $\varphi^n$ and $\psi^n$. Part (b) then yields

$$
\begin{pmatrix}L_{n+1}\\L_n\end{pmatrix}=\varphi^n\begin{pmatrix}\varphi\\1\end{pmatrix}+\psi^n\begin{pmatrix}\psi\\1\end{pmatrix}.
$$

Reading the second coordinate gives the [Lucas closed form](../../../../../lucas-closed-form.md)

$$
\boxed{L_n=\varphi^n+\psi^n=\left(\frac{1+\sqrt5}{2}\right)^n+\left(\frac{1-\sqrt5}{2}\right)^n\quad(n\geq0).}
$$

At $n=0$ this is 2 and at $n=1$ it is 1. Each summand obeys the same [recurrence relation](../../../../../recurrence-relation.md), which independently verifies the formula and explains why the irrational parts cancel to give an [integer](../../../../../integer-split.md).

## ↑ Ancestors (12)

1. [F](../f.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
