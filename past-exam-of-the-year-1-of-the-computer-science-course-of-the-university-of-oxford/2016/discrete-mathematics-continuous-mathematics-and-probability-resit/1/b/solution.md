<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By definition the [symmetric difference](../../../../../symmetric-difference.md) is $A\oplus B=(A\setminus B)\cup(B\setminus A)$. Put $D=A\oplus B$ and $E=A\cap B$. Distribution of [set intersection](../../../../../set-intersection.md) over [set union](../../../../../set-union.md) gives

$$
D\cap E=(A\cap B^c\cap A\cap B)\cup(B\cap A^c\cap A\cap B)=\varnothing.
$$

For disjoint [sets](../../../../../set-split.md), [set difference](../../../../../set-difference.md) removes nothing, so $D\oplus E=(D\setminus E)\cup(E\setminus D)=D\cup E$. Consequently

$$
\begin{aligned}
(A\oplus B)\oplus(A\cap B)
&=(A\cap B^c)\cup(B\cap A^c)\cup(A\cap B)\\
&=A\cup(B\cap A^c)\\
&=(A\cup B)\cap(A\cup A^c)\\
&=\boxed{A\cup B}.
\end{aligned}
$$

Here the second equality combines $A\cap B^c$ with $A\cap B$; the last uses $A\cup A^c=\mathcal U$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Discrete mathematics, continuous mathematics and probability (resit)](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
