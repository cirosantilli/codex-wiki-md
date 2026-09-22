<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The optimal approximation is the [orthogonal projection](../../../../../orthogonal-projection.md) onto the [linear span](../../../../../linear-span.md) of $p_0,\ldots,p_N$. Their [orthogonality](../../../../../orthogonal-vectors.md) gives

$$
\left\|f-\sum_{n=0}^N a_np_n\right\|_w^2
=\|f\|_w^2-2\sum_{n=0}^N a_n\langle f,p_n\rangle_w
+\sum_{n=0}^N a_n^2\|p_n\|_w^2.
$$

Completing each square proves both optimality and uniqueness:

$$
\boxed{a_n=\frac{\langle f,p_n\rangle_w}{\|p_n\|_w^2}}.
$$

For real $f$, these are real coefficients. If complex-valued $f$ is allowed while the coefficients remain real, replace the numerator by its real part and use the modulus-squared norm. The question's real formulation corresponds to real $f$.

Here the first three squared norms are one. Using $\int_0^\infty x^j e^{-2x}\,dx=j!/2^{j+1}$,

$$
\begin{aligned}
a_0&=\int_0^\infty e^{-2x}(1+x)\,dx=\frac12+\frac14=\frac34,\\
a_1&=\int_0^\infty e^{-2x}(1-x^2)\,dx=\frac12-\frac14=\frac14,\\
a_2&=\int_0^\infty e^{-2x}\left(1-x-\frac32x^2+\frac12x^3\right)dx
=\frac12-\frac14-\frac38+\frac3{16}=\frac1{16}.
\end{aligned}
$$

Thus

$$
\boxed{(a_0,a_1,a_2)=\left(\frac34,\frac14,\frac1{16}\right),\qquad
f_2(x)=\frac{17}{16}-\frac38x+\frac1{32}x^2}.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
