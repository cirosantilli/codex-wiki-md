<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To invert the [Burrows-Wheeler transform](../../../../../burrows-wheeler-transform.md), begin with six empty rows. At every iteration prepend the supplied last-column characters in their fixed row order, then sort the resulting rows in [lexicographic order](../../../../../lexicographic-order.md). After $k$ iterations the rows contain the length-$k$ prefixes of the sorted [cyclic rotations](../../../../../cyclic-rotation.md). For example, the first two iterations give

$$
\begin{aligned}
T_1&=(\texttt{\char36{}},\texttt{B},\texttt{C},\texttt{E},\texttt{M},\texttt{X}),\\
T_2&=(\texttt{\char36{}M},\texttt{BE},\texttt{CB},\texttt{EX},\texttt{MC},\texttt{X\char36{}}).
\end{aligned}
$$

Each iteration works because sorting the preceding character together with the already reconstructed prefix restores the ordering of the next-longer prefixes. Six iterations give the completed [matrix](../../../../../matrix.md)

$$
B=\begin{pmatrix}
\char36{}&M&C&B&E&X\\
B&E&X&\char36{}&M&C\\
C&B&E&X&\char36{}&M\\
E&X&\char36{}&M&C&B\\
M&C&B&E&X&\char36{}\\
X&\char36{}&M&C&B&E
\end{pmatrix}.
$$

The original linear string is the unique row ending in the terminator, hence

$$
\boxed{S_2=\texttt{MCBEX\char36{}}}.
$$

As a check, the reconstructed [matrix](../../../../../matrix.md)'s final column is precisely the supplied [Burrows-Wheeler transform](../../../../../burrows-wheeler-transform.md).

## ↑ Ancestors (13)

1. [B](../b.md)
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
