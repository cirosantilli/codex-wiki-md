<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $c_1=1/2$ and $c_2=c\ne1/2$. The weights and stage matrix become

$$
b=(1,0)^T,
\qquad
A=\begin{pmatrix}
\dfrac{4c-1}{4(2c-1)}&-\dfrac1{4(2c-1)}\\[5pt]
\dfrac{c^2}{2c-1}&\dfrac{c(c-1)}{2c-1}
\end{pmatrix}.
$$

For [algebraic stability of a Runge-Kutta method](../../../../../../algebraic-stability-of-a-runge-kutta-method.md),

$$
M_{ij}=b_ia_{ij}+b_ja_{ji}-b_ib_j,
$$

so

$$
M=\begin{pmatrix}
\dfrac1{2(2c-1)}&-\dfrac1{4(2c-1)}\\[5pt]
-\dfrac1{4(2c-1)}&0
\end{pmatrix}.
$$

A positive-semidefinite matrix with a zero diagonal entry must have every entry in that row and column equal to zero. Here the off-diagonal entry never vanishes for finite $c\ne1/2$. Therefore there is no admissible value of $c_2$ for which the method is algebraically stable.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
