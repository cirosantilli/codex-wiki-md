<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md) basis at $c_1,c_2$ is

$$
\ell_1(s)=\frac{s-c_2}{c_1-c_2},
\qquad
\ell_2(s)=\frac{s-c_1}{c_2-c_1}.
$$

The [collocation Runge-Kutta method](../../../../../../collocation-runge-kutta-method.md) has stages and update

$$
Y_i=y_n+h\sum_{j=1}^2a_{ij}f(Y_j),
\qquad
y_{n+1}=y_n+h\sum_{j=1}^2b_jf(Y_j),
$$

where $a_{ij}=\int_0^{c_i}\ell_j(s)ds$ and $b_j=\int_0^1\ell_j(s)ds$. Explicitly,

$$
A=\begin{pmatrix}
\dfrac{c_1(c_1/2-c_2)}{c_1-c_2}&\dfrac{c_1^2}{2(c_1-c_2)}\\[6pt]
-\dfrac{c_2^2}{2(c_1-c_2)}&\dfrac{c_2(c_2/2-c_1)}{c_2-c_1}
\end{pmatrix},
\qquad
b=\begin{pmatrix}
\dfrac{1/2-c_2}{c_1-c_2}\\[5pt]
\dfrac{1/2-c_1}{c_2-c_1}
\end{pmatrix}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
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
