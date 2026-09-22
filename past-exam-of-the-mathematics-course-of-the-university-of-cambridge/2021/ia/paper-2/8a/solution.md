<h1 id="8a/solution">Solution</h1>

↑ **Parent:** [8A](../8a.md)

Termwise differentiation of the [matrix exponential](../../../../../matrix-exponential.md) gives

$$
\begin{aligned}
\frac d{dt}e^{tA}
&=\sum_{m=1}^{\infty}\frac{m t^{m-1}A^m}{m!}\\
&=A\sum_{j=0}^{\infty}\frac{t^jA^j}{j!}
=Ae^{tA}.
\end{aligned}
$$

Thus $y(t)=e^{tA}y_0$ satisfies $y'=Ay$ and $y(0)=y_0$. If two solutions existed, multiplying their difference by $e^{-tA}$ would give a vector with zero derivative and zero initial value, proving uniqueness.

For the inhomogeneous equation, multiply by the integrating factor $e^{-tA}$:

$$
\frac d{dt}(e^{-tA}x)=e^{-tA}f(t).
$$

Integration and multiplication by $e^{tA}$ give the variation-of-constants formula

$$
\boxed{
x(t)=e^{tA}x_0
+\int_0^te^{(t-s)A}f(s)\,ds}.
$$

For the stated matrix,

$$
A^2=
\begin{pmatrix}
12&-4&-4\\
12&-4&-4\\
24&-8&-8
\end{pmatrix},
\qquad
A^3=0,
$$

so

$$
e^{tA}=I+tA+\frac{t^2}{2}A^2.
$$

Writing $f(t)=v\sin t$ with $v=(1,3,0)^T$, one finds

$$
Ax_0=0,\qquad Av=(8,8,16)^T,\qquad A^2v=0.
$$

Therefore

$$
x(t)=x_0+v(1-\cos t)+Av(t-\sin t),
$$

or explicitly

$$
\boxed{
x(t)=
\begin{pmatrix}
8t-8\sin t-\cos t+2\\
8t-8\sin t-3\cos t+4\\
16t-16\sin t+2
\end{pmatrix}}.
$$

## ↑ Ancestors (10)

1. [8A](../8a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
