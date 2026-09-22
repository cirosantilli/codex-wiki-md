<h1 id="6/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

From the zero initial [vector](../../../../../../vector.md), the [linear-system residual](../../../../../../linear-system-residual.md) is $r_0=(1,1)^T$. Then $r_0^Tr_0=2$, $Ar_0=(5,13)^T$, and $r_0^TAr_0=18$. The step is $\alpha_0=1/9$, giving

$$
\boxed{x_1=\begin{pmatrix}1/9\\1/9\end{pmatrix}.}
$$

As a check, the new residual is $(4/9,-4/9)^T$, orthogonal to the preceding residual as expected after this exact line search. It is nonzero, so one iteration has not already solved the system.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof resit](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
