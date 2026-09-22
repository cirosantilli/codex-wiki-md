<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [standard maximum form of a linear program](../../../../../../standard-maximum-form-of-a-linear-program.md) convention $\max c^Tu$ subject to $Mu\leq b$ and $u\geq0$. Split the unrestricted variables as $x=x^+-x^-$ and $y=y^+-y^-$, with all four new variables nonnegative. The resulting [linear program](../../../../../../linear-programming-split.md) is

$$
\begin{aligned}
\max\quad&2x^+-2x^-+3y^+-3y^-+4z+7w\\
\text{subject to}\quad&2x^+-2x^--y^++y^-+5w\leq1,\\
&y^+-y^-+z+w\leq3,\\
&x^+,x^-,y^+,y^-,z,w\geq0.
\end{aligned}
$$

If equality-constraint standard form is preferred, add a nonnegative [slack variable](../../../../../../slack-variable.md) to each inequality.

Give the two inequalities nonnegative [dual variables](../../../../../../dual-variable.md) $\alpha,\beta$. The [dual linear program](../../../../../../dual-linear-program.md) is

$$
\begin{aligned}
\min\quad&\alpha+3\beta\\
\text{subject to}\quad&2\alpha\geq2,\qquad -2\alpha\geq-2,\\
&-\alpha+\beta\geq3,\qquad \alpha-\beta\geq-3,\\
&\beta\geq4,\qquad5\alpha+\beta\geq7,\\
&\alpha,\beta\geq0.
\end{aligned}
$$

The paired inequalities encode equalities for the two original unrestricted variables. Equivalently, the [dual linear program](../../../../../../dual-linear-program.md) has $2\alpha=2$, $-\alpha+\beta=3$, $\beta\geq4$, $5\alpha+\beta\geq7$ and $\alpha,\beta\geq0$. Thus **its only [feasible point](../../../../../../feasible-point.md) is $(\alpha,\beta)=(1,4)$, of [objective function](../../../../../../objective-function.md) value $13$**.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Algorithms](../../../../algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
