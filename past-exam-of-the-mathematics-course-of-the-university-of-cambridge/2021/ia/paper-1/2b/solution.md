<h1 id="2b/solution">Solution</h1>

↑ **Parent:** [2B](../2b.md)

Let $P_B,P_{B'},P_C,P_{C'}$ have the corresponding basis vectors as columns in standard coordinates. From the PDF,

$$
P_B=\begin{pmatrix}0&-2\\2&0\end{pmatrix},
\quad
P_{B'}=\begin{pmatrix}1&1\\1&-1\end{pmatrix},
\quad
P_C=\begin{pmatrix}1&0&0\\1&1&0\\0&0&1\end{pmatrix},
\quad
P_{C'}=I_3.
$$

The [matrix representation of a linear map](../../../../../matrix-representation-of-a-linear-map.md) in standard coordinates is $P_CAP_B^{-1}$. The [change of basis](../../../../../change-of-basis.md) formula therefore gives

$$
A'=P_{C'}^{-1}P_CAP_B^{-1}P_{B'}.
$$

Multiplication yields

$$
\boxed{
A'=
\begin{pmatrix}
3/2&-1/2\\
5/2&-3/2\\
-1&0
\end{pmatrix}}.
$$

## ↑ Ancestors (10)

1. [2B](../2b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
