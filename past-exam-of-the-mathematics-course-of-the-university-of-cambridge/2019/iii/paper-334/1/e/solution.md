<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The wall removes the far-field decay condition and instead imposes $\psi_{1x}(d)=0$, $\psi_{1y}(d)=U_1$. The [force-free](../../../../../../force-free.md) condition eliminates any first-order mean shear; since mean sheet tangential velocity is zero, $U_1=0$. Thus $\psi_1=f_d(y)\sin\theta$, where

$$
(\partial_y^2-1)^2f_d=0,\qquad f_d(0)=1,\quad f_d'(0)=0,\quad f_d(d)=f_d'(d)=0.
$$

Start with the [hyperbolic function](../../../../../../hyperbolic-function.md) form $f_d=(a+by)\cosh y+(c+ey)\sinh y$. The lower conditions give $a=1$, $c=-b$. Defining $\Delta=\sinh^2d-d^2$, the wall conditions give

$$
b=\frac{d+\sinh d\cosh d}{\Delta},\qquad e=-\frac{\sinh^2d}{\Delta}.
$$

Consequently the first-order flow for [Taylor-sheet swimming next to a rigid wall](../../../../../../taylor-sheet-swimming-next-to-a-rigid-wall.md) is

$$
\boxed{\psi_1=\left[\cosh y+\frac{d+\sinh d\cosh d}{\Delta}(y\cosh y-\sinh y)-\frac{\sinh^2d}{\Delta}y\sinh y\right]\sin\theta.}
$$

For $d>0$, $\sinh d>d$ ensures a nonzero denominator; as $d\to\infty$, this reduces to the unbounded first-order field on every fixed height interval.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 334](../../../paper-334-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
