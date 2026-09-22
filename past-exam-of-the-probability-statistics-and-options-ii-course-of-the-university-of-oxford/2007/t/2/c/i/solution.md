<h1 id="t/2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In the usual [linear programming sensitivity within a fixed optimal basis](../../../../../../linear-programming-sensitivity-within-a-fixed-optimal-basis.md), retain the optimal [basis](../../../../../../basis.md) $\{x_1,x_3\}$ while allowing its values to adjust. If the second resource amount is $b$, then

$$
\begin{pmatrix}x_1\\x_3\end{pmatrix}
=\begin{pmatrix}2&5\\1&3\end{pmatrix}^{-1}\begin{pmatrix}33\\b\end{pmatrix}
=\begin{pmatrix}99-5b\\2b-33\end{pmatrix}.
$$

The dual prices remain $(1,1)$, so optimality persists exactly while both [basic variables](../../../../../../basic-variable.md) are nonnegative:

$$
\boxed{\frac{33}{2}\le b\le\frac{99}{5}.}
$$

The optimal profit on that range is $33+b$. At the endpoints the [basis](../../../../../../basis.md) is degenerate but remains optimal. If the wording is instead read as requiring the exact numerical production [vector](../../../../../../vector.md) $(9,0,3)$ to remain unchanged and optimal, only $b=18$ does so; the standard allowable range concerns the [basis](../../../../../../basis.md) and its adjusted solution.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [T](../../../../t.md)
5. [2007](../../../../../2007-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
