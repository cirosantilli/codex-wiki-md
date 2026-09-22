<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The minimum-volume aspect ratio is $H/R\simeq1.847$.** Keep the material parameter $B_m^2=(\eta-1)\Sigma_a/D$ fixed and positive. Write $a=2.405$ and $x=H/R$. The constraint from part (c) gives

$$
\frac{a^2}{R^2}+\frac{\pi^2}{H^2}=B_m^2,
\qquad
R^2=\frac{a^2+\pi^2/x^2}{B_m^2}.
$$

The [cylinder](../../../../../cylinder-geometry.md) [volume](../../../../../volume.md) is consequently

$$
V(x)=\frac{\pi x}{B_m^3}
\left(a^2+\frac{\pi^2}{x^2}\right)^{3/2},
\qquad x>0.
$$

Its logarithmic derivative is

$$
\frac{d\ln V}{dx}
=\frac1x-\frac{3\pi^2}{x(a^2x^2+\pi^2)}
=\frac{a^2x^2-2\pi^2}{x(a^2x^2+\pi^2)}.
$$

The denominator is positive. The derivative changes from negative to positive exactly once, and $V$ diverges as $x\to0$ or $x\to\infty$. Hence this stationary point is the global minimum:

$$
\boxed{\frac HR=x_*=\frac{\sqrt2\,\pi}{2.405}=1.84735.}
$$

Equivalently $H/(2R)\simeq0.924$. This is an aspect ratio in the supplied idealized [boundary value problem](../../../../../boundary-value-problem-split.md); it does not determine an absolute size without a specified material parameter.

## ↑ Ancestors (10)

1. [D](../d.md)
2. [2](../../2.md)
3. [Module NE1](../../../paper-ne1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
