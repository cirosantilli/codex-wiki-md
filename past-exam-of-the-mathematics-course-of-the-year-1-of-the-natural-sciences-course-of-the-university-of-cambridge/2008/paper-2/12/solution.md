<h1 id="12/solution">Solution</h1>

↑ **Parent:** [12](../12.md)

The integrand is even and decays at both infinity and zero, since $a,b>0$. On $x>0$ set $u=\sqrt a\,x-\sqrt b/x$, a strictly increasing bijection onto the whole real line. Then

$$
ax^2+b/x^2=u^2+2\sqrt{ab},\qquad
x=\frac{u+\sqrt{u^2+4\sqrt{ab}}}{2\sqrt a},\qquad
\frac{dx}{du}=\frac1{2\sqrt a}\left(1+\frac u{\sqrt{u^2+4\sqrt{ab}}}\right).
$$

Using evenness for the negative half-axis gives

$$
I(a,b)=\frac{e^{-\sqrt{ab}}}{\sqrt a}\int_{-\infty}^{\infty}e^{-u^2/2}\left(1+\frac u{\sqrt{u^2+4\sqrt{ab}}}\right)du.
$$

The second summand is an integrable [odd function](../../../../odd-function.md), so its integral vanishes. The remaining [Gaussian integral](../../../../gaussian-integral.md) gives

$$
\boxed{I(a,b)=\sqrt{\frac{2\pi}a}\,e^{-\sqrt{ab}}.}
$$

For the second integral use $x=1/t$ separately on each half-axis. The factor $x^{-2}dx$ becomes $-dt$, and reversing the transformed limits yields $J(a,b)=I(b,a)$. Thus

$$
\boxed{J(a,b)=\sqrt{\frac{2\pi}b}\,e^{-\sqrt{ab}}.}
$$

These identities are instances of the [Gaussian integral with an inverse-square term](../../../../gaussian-integral-with-an-inverse-square-term.md). Splitting at zero before either [change of variables](../../../../change-of-variables-formula.md) avoids treating a discontinuous transformation as a single bijection.

## ↑ Ancestors (12)

1. [12](../12.md)
2. [Paper 2](../../paper-2-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
