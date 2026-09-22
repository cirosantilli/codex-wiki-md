<h1 id="17b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the test equation $f(y)=\lambda y$, put $z=h\lambda$. The stage equations of this [implicit Runge-Kutta method](../../../../../../implicit-runge-kutta-method.md) are

$$
\begin{pmatrix}
1-z/4&-z(1/4-a)\\
-z(1/4+a)&1-z/4
\end{pmatrix}
\begin{pmatrix}k_1\\k_2\end{pmatrix}
=\lambda y_n\begin{pmatrix}1\\1\end{pmatrix}.
$$

Substitution into the update gives the [stability function](../../../../../../stability-function.md)

$$
R(z)=\frac{2+z+2a^2z^2}{2-z+2a^2z^2}.
$$

For $z=x+iy$, direct expansion gives

$$
\begin{aligned}
&|2-z+2a^2z^2|^2-|2+z+2a^2z^2|^2\\
&\hspace{35mm}=-8x(1+a^2|z|^2).
\end{aligned}
$$

This is nonnegative whenever $x\leq0$, and hence $|R(z)|\leq1$ throughout the closed left half-plane, provided the denominator has no zero there.

If $a=0$, the denominator vanishes only at $z=2$. If $a\ne0$, its zeros solve

$$
2a^2z^2-z+2=0.
$$

Real roots are positive, while a complex-conjugate pair has positive real part because the sum of the roots is $1/(2a^2)>0$. Thus there are no poles in the closed left half-plane for any real $a$. Therefore

$$
\boxed{a\in\mathbb R}
$$

is the complete set of [A-stable](../../../../../../a-stability.md) parameters, as summarized by the [A-stability of a symmetric two-stage implicit Runge-Kutta family](../../../../../../a-stability-of-a-symmetric-two-stage-implicit-runge-kutta-family.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17B](../../17b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
