<h1 id="16c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an axisymmetric separated amplitude $\widehat\phi(r,z)=R(r)Z(z)$, [Laplace equation in cylindrical coordinates](../../../../../../laplace-equation-in-cylindrical-coordinates.md) becomes

$$
\frac1R\frac1r(rR')'
=-\frac{Z''}{Z}
=-k^2.
$$

The radial equation is

$$
R''+\frac1rR'+k^2R=0.
$$

Its solution regular at the axis is the [Bessel function](../../../../../../bessel-function.md) $J_0(kr)$. The vertical equation is $Z''-k^2Z=0$, and the bottom condition $Z'(-h)=0$ selects

$$
\boxed{Z(z)=\cosh(k(z+h))}
$$

up to an irrelevant constant multiplier. Finally, the sidewall condition gives

$$
0=R'(R)=kJ_0'(kR).
$$

Therefore the allowed positive wavenumbers are

$$
\boxed{k_n=\frac{x_n}{R},
\qquad J_0'(x_n)=0},
$$

and

$$
\boxed{\widehat\phi(r,z)
=A J_0(k_nr)\cosh(k_n(z+h))}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16C](../../16c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
