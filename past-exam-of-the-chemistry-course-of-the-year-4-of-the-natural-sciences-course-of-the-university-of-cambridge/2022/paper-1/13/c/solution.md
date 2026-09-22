<h1 id="13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A one-dimensional [probability density](../../../../../probability-density.md) has units $L^{-1}$, while $D$ has units $L^2T^{-1}$. With no other length scale, [dimensional analysis](../../../../../dimensional-analysis.md) requires

$$
\boxed{n(x,t)=\frac1{\sqrt{Dt}}F\left(\frac{x}{\sqrt{Dt}}\right).}
$$

Normalization gives $\int_{-\infty}^{\infty}F(\xi)\,d\xi=1$ and unbiased [diffusion](../../../../../diffusion.md) gives an even $F$. **Dimensional arguments alone do not specify $F$.**

For ordinary Fickian [diffusion](../../../../../diffusion.md), impose $\partial_t n=D\partial_x^2 n$ with $n(x,0)=\delta(x)$. Substitution of the similarity form yields

$$
F''+\tfrac12(\xi F)'=0.
$$

A decaying symmetric solution obeys $F'=-\xi F/2$, so $F=C e^{-\xi^2/4}$. Normalization fixes $C=1/\sqrt{4\pi}$:

$$
\boxed{n(x,t)=\frac1{\sqrt{4\pi Dt}}
\exp\left(-\frac{x^2}{4Dt}\right),\qquad t>0.}
$$

This [heat kernel](../../../../../heat-kernel.md) integrates to one, has [variance](../../../../../variance-split.md) $2Dt$, and tends to the initial [Dirac delta distribution](../../../../../dirac-delta-function.md) as $t\downarrow0$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
