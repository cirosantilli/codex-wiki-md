<h1 id="31d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

After division by $x$, the equation is

$$
y''+\left(\frac1x-1\right)y'-\frac1xy=0.
$$

The [removal of the first derivative from a second-order differential equation](../../../../../../removal-of-the-first-derivative-from-a-second-order-differential-equation.md) uses

$$
y=e^{-\frac12\int(1/x-1)\,dx}v
=e^{x/2}x^{-1/2}v.
$$

With

$$
P=\frac1x-1,\qquad Q=-\frac1x,
$$

the normal-form coefficient is

$$
Q-\frac12P'-\frac14P^2
=-\frac14-\frac1{2x}+\frac1{4x^2}.
$$

Consequently

$$
\boxed{
v''-\frac14\left(1+\frac2x-\frac1{x^2}\right)v=0},
$$

so the constants in the PDF's expression  
$1+Ax^{-1}+Bx^{-2}$ are

$$
\boxed{A=2,\qquad B=-1}.
$$

To classify infinity, put $z=1/x$. Since

$$
\frac{d^2v}{dx^2}=z^4v_{zz}+2z^3v_z,
$$

the coefficient of $v$ in the transformed equation has a pole of order four at $z=0$. This exceeds the order two allowed at a regular singular point. Hence $x=+\infty$ is an [irregular singular point at infinity](../../../../../../irregular-singular-point-at-infinity.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [31D](../../31d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
