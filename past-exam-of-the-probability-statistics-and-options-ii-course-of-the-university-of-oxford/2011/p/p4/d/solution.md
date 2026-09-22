<h1 id="p/p4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Multiplying the system by $Q^T$ turns it into $Rx=Q^Tb$. For nonsingular $A$, compute the transformed right side and solve the upper triangular system by [back substitution](../../../../../back-substitution.md). [Orthogonal](../../../../../orthogonal-vectors.md) transformations preserve Euclidean lengths and do not amplify errors in that transformation.

If $A$ is singular,

$$
0=\det A=\det Q\det R=\det Q\prod_{i=1}^nr_{ii}.
$$

Since $\det Q=\pm1$, at least one diagonal entry of $R$ is zero. The resulting triangular system must then be checked for consistency and any free variables, rather than applying divisions by zero.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
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
