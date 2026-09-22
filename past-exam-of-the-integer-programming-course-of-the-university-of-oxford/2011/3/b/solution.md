<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For any feasible assignment, the unit row and column sums give

$$
\begin{aligned}
\sum_{i,j}\bar c_{ij}x_{ij}
&=\sum_{i,j}c_{ij}x_{ij}-\sum_i u_i\sum_jx_{ij}-\sum_jv_j\sum_ix_{ij}\\
&=\sum_{i,j}c_{ij}x_{ij}-\sum_iu_i-\sum_jv_j.
\end{aligned}
$$

Thus the transformed objective differs by the fixed constant

$$
\boxed{-\sum_i u_i-\sum_jv_j.}
$$

Every feasible assignment shifts by that same amount, so all objective comparisons and all optimal assignments remain unchanged. The calculation also holds for fractional feasible points of the assignment LP relaxation. The numbers $u_i,v_j$ are [assignment dual potentials](../../../../assignment-dual-potentials.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
