<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the lower antisymmetric block shown in the original PDF. Write $M=\operatorname{diag}(aK,bJ)$ with

$$
K=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad J=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\qquad K^2=I,\quad J^2=-I.
$$

Powers preserve the block structure. Splitting the [matrix exponential](../../../../../matrix-exponential.md) series into even and odd powers gives $e^{aK}=I\cosh a+K\sinh a$. For the other block, the [matrix exponential when the square is minus the identity](../../../../../matrix-exponential-when-the-square-is-minus-the-identity.md) gives $e^{bJ}=I\cos b+J\sin b$. Therefore

$$
\boxed{e^M=\begin{pmatrix}\cosh a&\sinh a&0&0\\\sinh a&\cosh a&0&0\\0&0&\cos b&\sin b\\0&0&-\sin b&\cos b\end{pmatrix}.}
$$

The upper block is hyperbolic and the lower block is a rotation. The transcription's altered last row and hyperbolic functions in the lower block would describe a different problem.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
