<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Substitute the [Laplace contour-integral method for a linear differential equation](../../../../../laplace-contour-integral-method-for-a-linear-differential-equation.md) into the [differential equation](../../../../../differential-equation-split.md) and use $z e^{zt}=\partial_t e^{zt}$. [Integration by parts](../../../../../integration-by-parts.md) around a closed contour avoiding singularities gives

$$
0=\int_C e^{zt}\{-[(1+t^2)f(t)]'-2tf(t)\}\,dt.
$$

It suffices to solve $(1+t^2)f'+4tf=0$, giving

$$
\boxed{f(t)=\frac{C_0}{(1+t^2)^2}.}
$$

Nonzero contour integrals arise by enclosing one or both double poles $t=\pm i$. At $t=i$, the [residue](../../../../../residue.md) is

$$
\operatorname{Res}_{t=i}\frac{e^{zt}}{(1+t^2)^2}=-\frac14(z+i)e^{iz}.
$$

The conjugate pole gives the conjugate expression for real $z$. Taking real and imaginary linear combinations yields the real solutions

$$
\boxed{y_1(z)=\sin z-z\cos z,\qquad y_2(z)=\cos z+z\sin z.}
$$

Their [derivatives](../../../../../derivative.md) are $y_1'=z\sin z$, $y_2'=z\cos z$, and their [Wronskian](../../../../../wronskian.md) is $-z^2$, so they are [linearly independent](../../../../../linear-independence.md) on every interval avoiding zero. Both extend analytically across zero and remain independent as functions; the vanishing [Wronskian](../../../../../wronskian.md) at zero reflects the singular leading coefficient of the printed [differential equation](../../../../../differential-equation-split.md) there.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
