<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [natural cubic spline interpolant](../../../../../../natural-cubic-spline-interpolant.md) $s$ satisfies $s(x_i)=y_i$, is twice continuously differentiable, and is a [polynomial](../../../../../../polynomial-split.md) of degree at most three on each interval $[x_i,x_{i+1}]$. Its natural [boundary conditions](../../../../../../boundary-condition.md) are

$$
\boxed{s''(x_1)=s''(x_n)=0.}
$$

If defined outside the data interval, it continues linearly on both exterior intervals. Thus function values and the first two [derivatives](../../../../../../derivative.md) match at the knots, but the third [derivative](../../../../../../derivative.md) may jump.

For an explicit construction, let $h_i=x_{i+1}-x_i>0$ and $M_i=s''(x_i)$. Set $M_1=M_n=0$ and solve

$$
h_{i-1}M_{i-1}+2(h_{i-1}+h_i)M_i+h_iM_{i+1}
=6\left\{\frac{y_{i+1}-y_i}{h_i}-\frac{y_i-y_{i-1}}{h_{i-1}}\right\},\quad2\le i\le n-1.
$$

On $[x_i,x_{i+1}]$, put

$$
\begin{aligned}
s(x)={}&\frac{M_i(x_{i+1}-x)^3+M_{i+1}(x-x_i)^3}{6h_i}\\
&+\left(y_i-\frac{M_ih_i^2}{6}\right)\frac{x_{i+1}-x}{h_i}
+\left(y_{i+1}-\frac{M_{i+1}h_i^2}{6}\right)\frac{x-x_i}{h_i}.
\end{aligned}
$$

This formula interpolates the values and matches second [derivatives](../../../../../../derivative.md); the tridiagonal equations enforce first-derivative matching. The homogeneous system has only the zero solution: in a row with maximal nonzero $|M_i|$, its diagonal coefficient strictly exceeds the sum of its neighbour coefficients, making cancellation impossible. Thus the natural interpolant exists uniquely.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
