<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For a [diagonal matrix](../../../diagonal-matrix.md), each diagonal entry separately obeys $d^2+2d-15=(d-3)(d+5)=0$. Hence all four possibilities are

$$
\boxed{\operatorname{diag}(3,3),\quad\operatorname{diag}(3,-5),\quad
\operatorname{diag}(-5,3),\quad\operatorname{diag}(-5,-5).}
$$

For the second form, $X^2=I$ gives

$$
(aI+bX)^2+2(aI+bX)
=(a^2+b^2+2a)I+2b(a+1)X.
$$

Because $I,X$ are linearly independent and $b\ne0$, the $X$ coefficient forces $a=-1$; the $I$ coefficient then gives $b^2=16$. Thus

$$
\boxed{A=-I\pm4X=\begin{pmatrix}-1&\pm4\\\pm4&-1\end{pmatrix}.}
$$

Both constants are nonzero, as required.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2016 resit](../../2016-resit-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
