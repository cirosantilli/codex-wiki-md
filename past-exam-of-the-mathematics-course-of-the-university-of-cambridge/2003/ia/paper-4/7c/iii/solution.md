<h1 id="7c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The same recurrence [matrix](../../../../../../matrix.md) has

$$
A^5=A^3A^2=\begin{pmatrix}8&5\\5&3\end{pmatrix}\equiv3I\pmod5.
$$

Therefore $\mathbf v_{n+5}\equiv3\mathbf v_n\pmod5$, and in particular $F_{n+5}\equiv3F_n\pmod5$. Starting from $F_0=0$ and iterating,

$$
F_{5j}\equiv3^jF_0=0\pmod5.
$$

Consequently **every nonnegative index divisible by five has a Fibonacci number divisible by five**, including index zero. This directly proves the requested divisibility without assuming a general Fibonacci divisibility theorem.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
