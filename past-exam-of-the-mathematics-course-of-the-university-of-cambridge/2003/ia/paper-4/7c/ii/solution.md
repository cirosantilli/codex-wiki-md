<h1 id="7c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $\mathbf v_n=(F_{n+1},F_n)^T$. The [Fibonacci recurrence matrix modulo an integer](../../../../../../fibonacci-recurrence-matrix-modulo-an-integer.md) is $A=\begin{pmatrix}1&1\\1&0\end{pmatrix}$, so $\mathbf v_{n+r}=A^r\mathbf v_n$. Direct [matrix multiplication](../../../../../../matrix-multiplication.md) gives

$$
A^3=\begin{pmatrix}3&2\\2&1\end{pmatrix}\equiv I\pmod2,\qquad A^8=\begin{pmatrix}34&21\\21&13\end{pmatrix}\equiv I\pmod3.
$$

Taking the second coordinate proves

$$
\boxed{F_{n+3}\equiv F_n\pmod2,\qquad F_{n+8}\equiv F_n\pmod3},\qquad n\geq0.
$$

For explicit arithmetic behind the second power, squaring $A^2=\begin{pmatrix}2&1\\1&1\end{pmatrix}$ gives $A^4=\begin{pmatrix}5&3\\3&2\end{pmatrix}$, whose square is the displayed $A^8$. Thus the modular period assertions follow from calculations and the recurrence, not from quoting a period theorem.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7C](../../7c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
