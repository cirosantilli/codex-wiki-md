<h1 id="4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Eliminate the first column using multipliers $3$ and $2$. The two residual rows have second entries zero and four, so interchange their order for the next [pivot](../../../../../../pivotal-quantity.md). One resulting [Pivoted LU decomposition](../../../../../../pivoted-lu-decomposition.md) is

$$
\boxed{P=\begin{pmatrix}1&0&0\\0&0&1\\0&1&0\end{pmatrix},\quad
L=\begin{pmatrix}1&0&0\\2&1&0\\3&0&1\end{pmatrix},\quad
U=\begin{pmatrix}3&1&4\\0&4&-2\\0&0&-11\end{pmatrix}.}
$$

The factors below the first [pivot](../../../../../../pivotal-quantity.md) must follow the permuted row order, which is why $L$ contains $2$ before $3$. Direct multiplication gives rows $(3,1,4)$, $(6,6,6)$ and $(9,3,1)$ in both $PA$ and $LU$. This checks the permutation convention rather than confusing $PA=LU$ with a different placement of $P$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
