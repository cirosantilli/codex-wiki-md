<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the test equation $y'=\lambda y$, put $z=h\lambda$. The amplification roots satisfy

$$
D(z)\xi^2-\frac45\xi-\frac15(1+z)=0,
\qquad
D(z)=1-z+\frac25z^2.
$$

The quadratic [Schur stability criterion](../../../../../../schur-stability-criterion.md) shows that both roots lie in the closed unit disk when

$$
|1+z|\leq5|D|,
\qquad
4|5\overline D+1+z|
\leq25|D|^2-|1+z|^2.
$$

To check these inequalities on the closed left half-plane, write $z=-u+iv$ with $u\geq0$. The right side of the second inequality is

$$
4(u^4+5u^3+2u^2v^2+11u^2+5uv^2+13u+v^4+v^2+6)>0.
$$

After squaring, the difference between its square and $16|5\overline D+1+z|^2$ is a polynomial in $u$ and $v^2$ with nonnegative coefficients:

$$
\begin{aligned}
16\bigl[{}&u^8+10u^7+4u^6v^2+47u^6+30u^5v^2+136u^5\\
&+6u^4v^4+96u^4v^2+259u^4+30u^3v^4+172u^3v^2+330u^3\\
&+4u^2v^6+51u^2v^4+168u^2v^2+261u^2\\
&+10uv^6+36uv^4+54uv^2+108u+v^8+2v^6+9v^4\bigr]\geq0.
\end{aligned}
$$

The first inequality follows from the same displayed positive expression. The unit-circle cases are semisimple, so the entire closed left half-plane is in the [linear stability domain](../../../../../../linear-stability-domain.md). Hence the method is [A-stable](../../../../../../a-stability.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
