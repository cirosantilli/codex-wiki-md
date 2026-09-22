<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Multiplication by a positive weight puts the [differential equation](../../../../../differential-equation-split.md) into [Sturm-Liouville form](../../../../../sturm-liouville-form.md) if $(xw)'=(1-x)w$. Thus $xw'=-xw$, and the constant factor can be chosen so that

$$
\boxed{w(x)=e^{-x}},\qquad -(xe^{-x}y')'=n e^{-x}y.
$$

This fixes the otherwise arbitrary normalization of the weight consistently with the requested unit norms.

Write the [polynomial](../../../../../polynomial-split.md) as $p_n(x)=\sum_{j=0}^n c_jx^j$. Comparing coefficients gives

$$
(j+1)^2c_{j+1}+(n-j)c_j=0,\qquad c_0=1.
$$

Consequently $c_j=(-1)^j\binom nj/j!$, identifying the solutions as [Laguerre polynomials](../../../../../laguerre-polynomial.md). In particular,

$$
\boxed{p_0=1,\qquad p_1=1-x,\qquad p_2=1-2x+\frac{x^2}{2}}.
$$

Repeated [integration by parts](../../../../../integration-by-parts.md) gives the moments $\int_0^\infty e^{-x}x^j\,dx=j!$. Therefore

$$
\begin{aligned}
\|p_0\|_w^2&=1,\\
\|p_1\|_w^2&=1-2(1!)+2!=1,\\
\|p_2\|_w^2&=1-4(1!)+5(2!)-2(3!)+\tfrac14(4!)=1.
\end{aligned}
$$

For later use, [integration by parts](../../../../../integration-by-parts.md) in the weighted [eigenvalue equations](../../../../../eigenvalue-equation.md) also gives

$$
(n-m)\langle p_n,p_m\rangle_w
=\left[xe^{-x}(p_np_m'-p_n'p_m)\right]_0^\infty=0.
$$

The endpoint expression vanishes because of the factor $x$ at zero and exponential decay at infinity. Hence distinct [Laguerre polynomials](../../../../../laguerre-polynomial.md) are orthogonal, an instance of [orthogonality of Sturm-Liouville eigenfunctions](../../../../../orthogonality-of-sturm-liouville-eigenfunctions.md).

## ↑ Ancestors (13)

1. [B](../b.md)
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
