<h1 id="20/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the first [definite integral](../../../../../definite-integral.md), use [integration by substitution](../../../../../integration-by-substitution.md) $t=\tan x$, with $dx=dt/(1+t^2)$, $\cos^2x=1/(1+t^2)$ and $\sin^2x=t^2/(1+t^2)$. This gives

$$
I=\int_0^\infty\frac{dt}{p+qt^2}
=\frac1{\sqrt{pq}}\left[\arctan\left(t\sqrt{\frac qp}\right)\right]_0^\infty
=\boxed{\frac\pi{2\sqrt{pq}}.}
$$

For the second calculation, let $D=p\cos^2x+q\sin^2x$. Since $p,q>0$, this denominator is bounded away from zero; on compact positive parameter ranges the differentiated integrands have uniform bounds. Thus [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) is justified and gives

$$
I_p=-\int_0^{\pi/2}\frac{\cos^2x}{D^2}\,dx=-\frac\pi{4p^{3/2}q^{1/2}},\qquad
I_q=-\int_0^{\pi/2}\frac{\sin^2x}{D^2}\,dx=-\frac\pi{4p^{1/2}q^{3/2}}.
$$

Adding the two equations and using the [Pythagorean trigonometric identity](../../../../../pythagorean-trigonometric-identity.md) in the numerators yields $J=-I_p-I_q$, hence

$$
\boxed{J=\frac{\pi(p+q)}{4(pq)^{3/2}}.}
$$

For $p=q$, this becomes $\pi/(2p^2)$, agreeing with direct integration of the constant integrand.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
