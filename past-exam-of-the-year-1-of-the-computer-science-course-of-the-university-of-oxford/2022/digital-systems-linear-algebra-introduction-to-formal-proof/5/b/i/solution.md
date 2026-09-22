<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $D=\operatorname{diag}(d_1,d_2,d_3)$, the upper entry of $D^{-1}AD$ in positions $i,i+1$ is $b_id_{i+1}/d_i$, and the corresponding lower entry is $c_id_i/d_{i+1}$. They are equal when $(d_{i+1}/d_i)^2=c_i/b_i$. All coefficients used here are positive, so choose

$$
\boxed{D=\operatorname{diag}\left(1,\sqrt{c_1/b_1},\sqrt{c_1c_2/(b_1b_2)}\right).}
$$

Direct [matrix multiplication](../../../../../../matrix-multiplication.md) gives the [symmetric matrix](../../../../../../symmetric-matrix.md)

$$
D^{-1}AD=\begin{pmatrix}
a_1&\sqrt{b_1c_1}&0\\
\sqrt{b_1c_1}&a_2&\sqrt{b_2c_2}\\
0&\sqrt{b_2c_2}&a_3
\end{pmatrix}.
$$

Its pattern remains [tridiagonal](../../../../../../tridiagonal-matrix.md). This is [positive diagonal symmetrization of a tridiagonal matrix](../../../../../../positive-diagonal-symmetrization-of-a-tridiagonal-matrix.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
