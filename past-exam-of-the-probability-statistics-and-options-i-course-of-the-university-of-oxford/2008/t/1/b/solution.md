<h1 id="t/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The identity columns in the final tableau correspond to basic variables $x_2,x_3$. Their original basis matrix is

$$
B=\begin{pmatrix}2&1\\2&2\end{pmatrix},\qquad
B^{-1}=\begin{pmatrix}1&-1/2\\-1&1\end{pmatrix},
$$

also visible directly in the two slack columns. Multiply the original constraint tableau and right side by $B^{-1}$ to obtain the missing entries. Subtract four times the first row and three times the second from the initial objective row, using the basic costs. The completed [simplex tableau](../../../../../simplex-tableau.md) is

$$
\boxed{\begin{array}{rrrrr|r}
3/2&1&0&1&-1/2&1\\
-1&0&1&-1&1&2\\ \hline
-2&0&0&-1&-1&-10
\end{array}.}
$$

The last row uses the supplied convention of reduced costs $c_j-c_B^TB^{-1}A_j$, so its final right side is minus the objective. Setting the nonbasic variables to zero gives

$$
\boxed{(x_1,x_2,x_3)=(0,1,2),\qquad f_{\max}=10.}
$$

The dual feasible vector $y=(1,1)$ has $A^Ty=(3,4,3)^T\geq(1,4,3)^T$ and objective $4+6=10$. Part (a) independently certifies the optimum and confirms the objective-row sign.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [T](../../../t.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
