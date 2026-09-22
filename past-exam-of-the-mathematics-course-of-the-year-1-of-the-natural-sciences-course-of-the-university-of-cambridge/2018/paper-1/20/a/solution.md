<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\alpha\ne0$, [integration by substitution](../../../../../integration-by-substitution.md) $t=\alpha x$ gives

$$
I(\alpha)=\int_0^1\frac{dx}{1+\alpha^2x^2}=\boxed{\frac{\arctan\alpha}{\alpha}.}
$$

At $\alpha=0$ the integrand is one, so $I(0)=1$, also the continuous [limit](../../../../../limit-of-a-function.md) of this expression. For nonzero $\alpha$, [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) is valid on the finite interval and yields

$$
I'(\alpha)=-2\alpha\int_0^1\frac{x^2}{(1+\alpha^2x^2)^2}\,dx
=\frac{\alpha/(1+\alpha^2)-\arctan\alpha}{\alpha^2}.
$$

Set $\alpha=\sqrt3$ and use $\arctan\sqrt3=\pi/3$. The requested value is

$$
\boxed{\int_0^1\frac{x^2}{(1+3x^2)^2}\,dx=-\frac{I'(\sqrt3)}{2\sqrt3}
=\frac{\pi}{18\sqrt3}-\frac1{24}=\frac{\pi\sqrt3}{54}-\frac1{24}.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
