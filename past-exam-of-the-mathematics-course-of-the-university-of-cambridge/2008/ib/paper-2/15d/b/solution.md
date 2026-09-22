<h1 id="15d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The axis-regular [separation of variables](../../../../../../separation-of-variables.md) expansion for an axisymmetric harmonic potential is

$$
\Phi(r,x)=\sum_{n=0}^\infty(A_nr^n+B_nr^{-n-1})P_n(x).
$$

The radial powers solve $r^2R''+2rR'-n(n+1)R=0$, while the regular angular solutions are [Legendre polynomials](../../../../../../legendre-polynomial.md). For an exterior solution tending to zero at infinity, retain only the negative radial powers. The boundary polynomial decomposes as $1+x^2=\tfrac43P_0(x)+\tfrac23P_2(x)$. Therefore

$$
\boxed{\Phi(r,x)=\frac{4a}{3r}+\frac{2a^3}{3r^3}P_2(x)
=\frac{4a}{3r}+\frac{a^3}{3r^3}(3x^2-1),\quad r\ge a.}
$$

It has the required boundary value and decay. Uniqueness follows from the [maximum principle for harmonic functions](../../../../../../maximum-principle-for-harmonic-functions.md) for a harmonic difference, using its zero boundary values and vanishing limit at infinity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15D](../../15d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
