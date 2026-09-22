<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

**Singular points.** Normalizing the equation gives $p=2/x$ and $q=1-\ell(\ell+1)/x^2$. The only finite singular point is $x=0$, and it is regular because $xp$ and $x^2q$ are analytic there. At infinity put $t=1/x$ and $Y(t)=y(1/t)$; the equation becomes

$$
Y''+\left[\frac1{t^4}-\frac{\ell(\ell+1)}{t^2}\right]Y=0.
$$

The fourth-order pole makes $t=0$ an [irregular singular point](../../../../irregular-singular-point.md), so **infinity is irregular**.

**Exponents and recurrence.** Substitution of a series for a [Frobenius solution](../../../../frobenius-solution.md) gives the [indicial equation](../../../../indicial-equation.md)

$$
\sigma(\sigma+1)-\ell(\ell+1)=0,\qquad\boxed{\sigma=\ell\quad\text{or}\quad\sigma=-\ell-1.}
$$

With negative-index coefficients set to zero, the coefficient equation is

$$
\boxed{[(j+\sigma)(j+\sigma+1)-\ell(\ell+1)]a_j=-a_{j-2}.}
$$

For $\sigma=\ell$, it gives $a_1=0$ and

$$
a_j=-\frac{a_{j-2}}{j(j+2\ell+1)},\qquad j\geq2.
$$

For $\sigma=-\ell-1$, it gives

$$
a_j=-\frac{a_{j-2}}{j(j-2\ell-1)},\qquad j\geq1,\quad j\neq2\ell+1.
$$

For $\ell\geq1$, $a_1=0$. At the exceptional odd index $j=2\ell+1$, the recurrence becomes $a_{2\ell-1}=0$, which is already satisfied. Thus $a_{2\ell+1}$ is free; choosing it to be zero gives an independent pure-even series times $x^{-\ell-1}$. A nonzero choice adds a multiple of the regular solution. For $\ell=0$, this freedom occurs at $j=1$ itself. This [Frobenius resonance in the spherical Bessel equation](../../../../frobenius-resonance-in-the-spherical-bessel-equation.md) is compatible, so no logarithmic term is needed despite the integer separation of exponents.

**Normalized regular solution.** Set $\sigma=\ell$ and $a_0=2^\ell\ell!/(2\ell+1)!$. The proposed even coefficients

$$
a_{2s}=\frac{2^\ell(-1)^s(s+\ell)!}{s!(2s+2\ell+1)!}
$$

satisfy $a_{2s}/a_{2s-2}=-1/[2s(2s+2\ell+1)]$, precisely the recurrence above. Therefore

$$
\boxed{j_\ell(x)=2^\ell x^\ell\sum_{s=0}^\infty\frac{(-1)^s(s+\ell)!}{s!(2s+2\ell+1)!}x^{2s}.}
$$

This is the regular [Spherical Bessel function](../../../../spherical-bessel-function.md). The coefficient ratio tends to zero, so its series converges for every finite $x$; the other even-series factor also has infinite radius, although the prefactor has a pole at zero.

For $\ell=0$, the coefficients reduce to $(-1)^s/(2s+1)!$, giving

$$
\boxed{j_0(x)=\frac{\sin x}{x},\qquad j_0(0)=1.}
$$

Directly, $x^2j_0'=x\cos x-\sin x$, whose [derivative](../../../../derivative.md) is $-x\sin x$. Thus $(x^2j_0')'+x^2j_0=0$, verifying the equation. The independent singular branch at $\ell=0$ can be chosen as $\cos x/x$.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
