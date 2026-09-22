<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First add row 1 to rows 2 and 3. This is the product of two [elementary matrices](../../../../../elementary-matrix.md), written compactly as

$$
E_1=\begin{pmatrix}1&0&0&0\\1&1&0&0\\1&0&1&0\\0&0&0&1\end{pmatrix},\qquad E_1A=\begin{pmatrix}1&-1&0&1\\0&0&0&2\\0&-1&1&2\\0&-2&-1&2\end{pmatrix}.
$$

Swap rows 2 and 4 with $P$, then subtract half of the new row 2 from row 3 with $E_2$:

$$
P=\begin{pmatrix}1&0&0&0\\0&0&0&1\\0&0&1&0\\0&1&0&0\end{pmatrix},\qquad E_2=\begin{pmatrix}1&0&0&0\\0&1&0&0\\0&-1/2&1&0\\0&0&0&1\end{pmatrix}.
$$

This gives the upper triangular matrix

$$
\boxed{U=E_2PE_1A=\begin{pmatrix}1&-1&0&1\\0&-2&-1&2\\0&0&3/2&1\\0&0&0&2\end{pmatrix}.}
$$

Because $P^{-1}=P$, rearranging yields the convention **$A=PLU$**, where

$$
\boxed{L=PE_1^{-1}PE_2^{-1}=\begin{pmatrix}1&0&0&0\\0&1&0&0\\-1&1/2&1&0\\-1&0&0&1\end{pmatrix}.}
$$

The conjugation by $P$ moves the earlier elimination multipliers to the appropriate rows. Ignoring this permutation when forming $L$ would give an incorrect [PLU factorization](../../../../../plu-factorization.md). Here the same permutation is its own inverse, so $PA=LU$ also holds.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
