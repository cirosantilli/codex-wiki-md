<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonzero solution on a branch where the real power is differentiable, set $v=u^{1-\alpha}$. Multiplying the [Bernoulli differential equation](../../../../../bernoulli-differential-equation.md) by $(1-\alpha)u^{-\alpha}$ gives the linear equation

$$
v'+(1-\alpha)f(x)v=(1-\alpha)g(x).
$$

It can be solved by an [integrating factor](../../../../../integrating-factor.md). For the specified cubic equation take $\alpha=3$, $f=g=x$, so $v=u^{-2}$ satisfies $v'-2xv=-2x$. Its integrating factor is $e^{-x^2}$, giving $(ve^{-x^2})'=-2xe^{-x^2}$ and hence $v=1+Ce^{x^2}$. Thus all nonzero real solutions are

$$
\boxed{u(x)=\pm\frac1{\sqrt{1+Ce^{x^2}}},}
$$

on connected intervals where the denominator is positive, with a fixed sign on each interval. Also **$u\equiv0$** solves the original equation and must be restored because the substitution excluded it. The choices $C=0$ give the constant solutions $u=\pm1$. Smoothness of the original right-hand side gives uniqueness, so a nonzero solution cannot cross through the zero solution at a finite regular point.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
