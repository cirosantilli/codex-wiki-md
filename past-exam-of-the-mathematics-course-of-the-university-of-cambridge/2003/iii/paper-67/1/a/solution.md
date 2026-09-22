<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce one stage $k=f(t_n+h/2,Y)$ with $Y=y_n+hk/2$, and update $y_{n+1}=y_n+hk$. This is the [implicit midpoint rule](../../../../../../implicit-midpoint-rule.md) as a one-stage [Runge-Kutta method](../../../../../../runge-kutta-method.md), with [Butcher tableau](../../../../../../butcher-tableau.md)

$$
\begin{array}{c|c}1/2&1/2\\\hline&1\end{array}.
$$

For a smooth vector field, write $\Delta=y_{n+1}-y_n$. Expanding its stage equation gives

$$
\Delta=hf(t_n,y_n)+\frac{h^2}{2}\bigl(f_t+f_yf\bigr)(t_n,y_n)+O(h^3),
$$

which matches the exact [Taylor expansion](../../../../../../taylor-expansion.md) through degree two. The method therefore has order at least two. On the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md) $y'=\lambda y$, its [stability function](../../../../../../stability-function.md) is

$$
R(z)=\frac{1+z/2}{1-z/2}=1+z+\frac{z^2}{2}+\frac{z^3}{4}+O(z^4),\qquad z=h\lambda.
$$

The third coefficient differs from the exponential's $1/6$, so the order is exactly two.

There is no pole in $\operatorname{Re}z\leq0$, and

$$
|1-z/2|^2-|1+z/2|^2=-2\operatorname{Re}z\geq0.
$$

Thus $|R(z)|\leq1$ throughout the closed left half-plane:

$$
\boxed{\text{one-stage implicit Runge-Kutta; order }2;\quad\text{A-stable}.}
$$

This conclusion is [A-stability](../../../../../../a-stability.md), not strong damping of arbitrarily stiff modes: $R(z)\to-1$ along the negative real axis.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
