<h1 id="b3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Using the paper's named weights $w_i$, take

$$
W=\operatorname{diag}(1,1,1,\tfrac12,\tfrac12),\qquad
A=\begin{pmatrix}1&1\\1&2\\1&3\\1&4\\1&5\end{pmatrix},\qquad
b=\begin{pmatrix}3\\5\\5\\4\\3\end{pmatrix}.
$$

The [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md) for [weighted least squares](../../../../../weighted-least-squares.md) become

$$
\begin{pmatrix}7/2&33/4\\33/4&97/4\end{pmatrix}
\begin{pmatrix}\widehat\beta_0\\\widehat\beta_1\end{pmatrix}
=\begin{pmatrix}59/4\\143/4\end{pmatrix}.
$$

Multiplying by four gives $14\widehat\beta_0+33\widehat\beta_1=59$ and $33\widehat\beta_0+97\widehat\beta_1=143$. Their [determinant](../../../../../determinant.md) is $269$, giving

$$
\widehat\beta_0=\frac{1004}{269},\qquad \widehat\beta_1=\frac{55}{269}.
$$

Thus, to two significant digits, **$\boxed{\widehat\beta_0=3.7,\quad\widehat\beta_1=0.20}$**, with the slope measured in expression units per hour.

There is a wording convention to make explicit. Because the stated objective squares $w_i$, the choice above gives the final two _squared residuals_ one-quarter of the influence of the others. If “half as much” instead means half the coefficient of each squared residual, use $W=\operatorname{diag}(1,1,1,1/\sqrt2,1/\sqrt2)$. Then the [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md) are

$$
\begin{pmatrix}4&21/2\\21/2&69/2\end{pmatrix}
\begin{pmatrix}\widehat\beta_0\\\widehat\beta_1\end{pmatrix}
=\begin{pmatrix}33/2\\87/2\end{pmatrix},
$$

giving $\widehat\beta_0=150/37\approx\boxed{4.1}$ and $\widehat\beta_1=1/37\approx\boxed{0.027}$. Stating which quantity is halved resolves the ambiguity.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [B3](../../b3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
