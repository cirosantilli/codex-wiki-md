<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use banded [Gaussian elimination](../../../../../gaussian-elimination.md) followed by [back substitution](../../../../../back-substitution.md). To distinguish the right-hand side from the upper-diagonal coefficients $b_i$, write it as $r_i$. If the modified [pivot elements](../../../../../pivot-element.md) are nonzero, the [tridiagonal elimination recurrences](../../../../../tridiagonal-elimination-recurrences.md) are

$$
p_1=a_1,\quad q_1=r_1,\qquad m_i=\frac{c_{i-1}}{p_{i-1}},\quad p_i=a_i-m_ib_{i-1},\quad q_i=r_i-m_iq_{i-1}\quad(2\le i\le n).
$$

They eliminate just the one entry below each [pivot element](../../../../../pivot-element.md). Solve the resulting upper [bidiagonal matrix](../../../../../bidiagonal-matrix.md) system by

$$
x_n=q_n/p_n,\qquad x_i=(q_i-b_ix_{i+1})/p_i\quad(i=n-1,\ldots,1).
$$

There is a bounded number of [arithmetic operations](../../../../../arithmetic-operation.md) per row in each sweep, giving **$O(n)$ [arithmetic operations](../../../../../arithmetic-operation.md) and $O(n)$ storage**. The unpivoted recurrences cost $8n-7$ [arithmetic operations](../../../../../arithmetic-operation.md) under the usual scalar-operation count.

For a general [tridiagonal matrix](../../../../../tridiagonal-matrix.md), nonsingularity alone does not guarantee these [pivot elements](../../../../../pivot-element.md). If a zero or unsafe [pivot element](../../../../../pivot-element.md) occurs, use [partial pivoting](../../../../../columnwise-partial-pivoting.md) between the current row and the next row. These are the only possible nonzero candidates in the current column; adjacent row swaps introduce at most a second upper diagonal. Tracking that [fill-in](../../../../../fill-in.md) keeps both [Gaussian elimination](../../../../../gaussian-elimination.md) and [back substitution](../../../../../back-substitution.md) at $O(n)$ [arithmetic operations](../../../../../arithmetic-operation.md). For example, $\begin{pmatrix}0&1\\1&0\end{pmatrix}$ is invertible but requires a row swap. If the input is singular, report a zero final [pivot element](../../../../../pivot-element.md); a unique solution cannot be promised, and compatibility or free-variable analysis is a separate issue. No nonsingularity or safe-pivot assumption is silently inferred from the word [tridiagonal](../../../../../tridiagonal-matrix.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
