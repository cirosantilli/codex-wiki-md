<h1 id="7b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Substitute $y_2=vy_1$ and use $y_1''+py_1'+qy_1=0$ to cancel the terms proportional to $v$. The remaining [ordinary differential equation](../../../../../../ordinary-differential-equation.md) is

$$
\boxed{y_1v''+(2y_1'+py_1)v'=0.}
$$

On an interval where $y_1\ne0$, divide through and put $w=v'$:

$$
w'+\left(2\frac{y_1'}{y_1}+p\right)w=0,\qquad w=C\frac{e^{-\int p(x)\,dx}}{y_1(x)^2}.
$$

Thus [reduction of order](../../../../../../reduction-of-order.md) gives

$$
\boxed{y_2(x)=y_1(x)\int^x\frac{e^{-\int^s p(r)\,dr}}{y_1(s)^2}\,ds.}
$$

A nonzero multiplicative constant gives an independent solution; adding a constant inside the integral adds a multiple of $y_1$. The [Wronskian](../../../../../../wronskian.md) is proportional to $e^{-\int p}$ and is nonzero on the interval. The undivided equation remains meaningful at a zero of $y_1$, but this integral representation then needs continuation rather than direct division.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7B](../../7b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
