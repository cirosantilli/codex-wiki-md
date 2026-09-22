<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [cyclic rotation](../../../../../cyclic-rotation.md) moves the first character to the end without changing the cyclic order of the remaining characters. Starting with the specified terminator-first row and repeatedly rotating left gives the following [matrix](../../../../../matrix.md); its row order is only a construction order, not a sorting order:

$$
R=\begin{pmatrix}
\char36{}&A&C&A&A&C&G\\
A&C&A&A&C&G&\char36{}\\
C&A&A&C&G&\char36{}&A\\
A&A&C&G&\char36{}&A&C\\
A&C&G&\char36{}&A&C&A\\
C&G&\char36{}&A&C&A&A\\
G&\char36{}&A&C&A&A&C
\end{pmatrix}.
$$

Under [lexicographic order](../../../../../lexicographic-order.md), compare characters from left to right, using $\char36{}\lt A\lt C\lt G$. The sorted [cyclic rotation](../../../../../cyclic-rotation.md) [matrix](../../../../../matrix.md) is therefore

$$
B=\begin{pmatrix}
\char36{}&A&C&A&A&C&G\\
A&A&C&G&\char36{}&A&C\\
A&C&A&A&C&G&\char36{}\\
A&C&G&\char36{}&A&C&A\\
C&A&A&C&G&\char36{}&A\\
C&G&\char36{}&A&C&A&A\\
G&\char36{}&A&C&A&A&C
\end{pmatrix}.
$$

The [Burrows-Wheeler transform](../../../../../burrows-wheeler-transform.md) is the last column, read downwards, so **the transformed string** is

$$
\boxed{\operatorname{BWT}(S_1)=\texttt{GC\char36{}AAAC}}.
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
