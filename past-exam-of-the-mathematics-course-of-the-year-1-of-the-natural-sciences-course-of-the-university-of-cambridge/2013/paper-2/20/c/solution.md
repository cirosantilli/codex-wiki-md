<h1 id="20/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md), justified by the integrable bound $|x\sin(tx)e^{-x^2/2}|\leq xe^{-x^2/2}$. This gives

$$
F'(t)=-\int_0^\infty x\sin(tx)e^{-x^2/2}\,dx
=\int_0^\infty\sin(tx)\,d(e^{-x^2/2}).
$$

[Integration by parts](../../../../../integration-by-parts.md) makes the [boundary](../../../../../boundary-of-a-set.md) term vanish: [sine](../../../../../sine.md) vanishes at zero and the Gaussian tends to zero at infinity. Therefore

$$
\boxed{F'(t)=-t\int_0^\infty\cos(tx)e^{-x^2/2}\,dx=-tF(t)}.
$$

The [integrating factor](../../../../../integrating-factor.md) $e^{t^2/2}$ makes $(e^{t^2/2}F)'=0$, so $F(t)=Ce^{-t^2/2}$. At $t=0$, the given half-line [Gaussian integral](../../../../../gaussian-integral.md) fixes $C=\sqrt{\pi/2}$. Thus

$$
\boxed{F(t)=\sqrt{\frac\pi2}\,e^{-t^2/2}}.
$$

This is the even cosine-transform form of the [Fourier transform of a Gaussian](../../../../../fourier-transform-of-a-gaussian.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
