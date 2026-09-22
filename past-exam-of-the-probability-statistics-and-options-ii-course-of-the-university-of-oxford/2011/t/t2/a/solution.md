<h1 id="t/t2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With nonnegative production amounts $x_1,x_2,x_3$, the primal linear programme is

$$
\boxed{\max 5x_1+6x_2+3x_3,\qquad4x_1+2x_2\leq6,\quad2x_1+3x_2+2x_3\leq11.}
$$

Introduce slacks $s_R,s_S\geq0$. The initial basic variables are the slacks, and the reduced profits of the goods are $5,6,3$. The greatest is six, so $x_2$ enters. The [ratio test](../../../../../ratio-test.md) compares $6/2=3$ and $11/3$, so $s_R$ leaves. The resulting dictionary is

$$
x_2+2x_1+\tfrac12s_R=3,\qquad
s_S-4x_1+2x_3-\tfrac32s_R=2,
$$

with profit $18-7x_1+3x_3-3s_R$. The greatest positive reduced profit is now three, so $x_3$ enters; its only positive pivot coefficient is two in the second row, and $s_S$ leaves. The final tableau, expressed as equations, is

$$
\begin{aligned}
x_2+2x_1+\tfrac12s_R&=3,\\
x_3-2x_1-\tfrac34s_R+\tfrac12s_S&=1,\\
P&=21-x_1-\tfrac34s_R-\tfrac32s_S.
\end{aligned}
$$

All nonbasic reduced profits are nonpositive, proving optimality at

$$
\boxed{(x_1,x_2,x_3)=(0,3,1),\qquad P=21.}
$$

The ordered optimal [basis](../../../../../basis.md) is $(x_2,x_3)$, hence

$$
\boxed{B=\begin{pmatrix}2&0\\3&2\end{pmatrix},\qquad
B^{-1}=\begin{pmatrix}1/2&0\\-3/4&1/2\end{pmatrix}.}
$$

The inverse is read from the two slack columns of the final basic equations.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [T2](../../t2.md)
3. [T](../../../t.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
