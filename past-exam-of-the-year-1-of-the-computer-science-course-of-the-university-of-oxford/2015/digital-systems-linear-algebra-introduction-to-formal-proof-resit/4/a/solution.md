<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Source gap / TODO:** the original printed page 4, confirmed visually, omits the unknown [vector](../../../../../vector.md). It literally equates a $3\times3$ [matrix](../../../../../matrix.md) with a $3\times1$ [vector](../../../../../vector.md), so it does not define a well-formed [system of linear equations](../../../../../system-of-linear-equations.md). The following answer is conditional on the usual intended interpretation $A\mathbf x=(1,k^2,k)^T$; the missing factor is not present in the source.

Under that interpretation, the rows satisfy $r_1-2r_2+r_3=0$. Applying this [linear relation](../../../../../linear-relation.md) to the right-hand side gives the necessary consistency condition

$$
1-2k^2+k=0,\qquad (2k+1)(k-1)=0.
$$

It is sufficient too: the upper-left $2\times2$ [minor](../../../../../minor-linear-algebra.md) has [determinant](../../../../../determinant.md) $4-9=-5\ne0$, so the first two rows are [linearly independent](../../../../../linear-independence.md). The third row is $2r_2-r_1$, and imposes precisely the condition already found. Therefore

$$
\boxed{k=1\quad\text{or}\quad k=-\tfrac12\qquad\text{if the intended equation is }A\mathbf x=(1,k^2,k)^T.}
$$

For completeness, setting $x_3=t$ gives

$$
x_1=\frac{3k^2-2-4t}{5},\qquad x_2=\frac{3-2k^2+t}{5},\qquad t\in\mathbb R,
$$

and direct substitution satisfies all three [linear equations](../../../../../linear-equation.md) exactly for those two values of $k$. An unconditional answer to the malformed printed equality awaits a source correction.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
