<h1 id="40e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

After multiplying the five-point equations by $-1$ if necessary, their matrix $A$ is symmetric positive definite. For any ordering write $A=D+L+L^T$, where $D=4I$. Gauss-Seidel method uses $M=D+L$ and has iteration matrix $-M^{-1}L^T$. In part (a) take $B=L^T$; then $A-B=M$ and

$$
A-B-B^T=D,
$$

which is positive definite. Therefore the iteration matrix has spectral radius below one for every ordering, proving convergence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40E](../../40e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
