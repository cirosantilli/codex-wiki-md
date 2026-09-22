<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A single [eigenbasis](../../../../../eigenbasis.md) works for every choice of the parameters. The columns $v_1=(1,0,0)^T$, $v_2=(1,1,0)^T$, $v_3=(1,1,1)^T$ satisfy

$$
Mv_1=av_1,\qquad Mv_2=bv_2,\qquad Mv_3=cv_3.
$$

They are [linearly independent](../../../../../linear-independence.md) because their column [matrix](../../../../../matrix.md) has determinant one. Thus the [diagonalization](../../../../../diagonalization-of-a-matrix.md) is

$$
\boxed{P=\begin{pmatrix}1&1&1\\0&1&1\\0&0&1\end{pmatrix},\qquad P^{-1}=\begin{pmatrix}1&-1&0\\0&1&-1\\0&0&1\end{pmatrix},\qquad M=P\operatorname{diag}(a,b,c)P^{-1}.}
$$

This formula includes all coincidences among $a,b,c$, so no special repeated-[eigenvalue](../../../../../eigenvalue.md) cases need separate bases.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
