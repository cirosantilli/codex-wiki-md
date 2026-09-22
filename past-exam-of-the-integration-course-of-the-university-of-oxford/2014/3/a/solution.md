<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $(X,\mathcal A,\mu)$ and $(Y,\mathcal B,\nu)$ be [measure spaces](../../../../measure-space.md) with [sigma-finite measures](../../../../sigma-finite-measure.md), and use their [product measure](../../../../product-measure.md).

**[Fubini's theorem](../../../../fubini-s-theorem.md):** if $u$ is a measurable absolutely integrable [function](../../../../function-split.md) on $X\times Y$, then its sections are integrable for [almost every](../../../../almost-everywhere.md) fixed value of the other coordinate, the resulting section-integral [functions](../../../../function-split.md) are integrable, and

$$
\boxed{\int_{X\times Y}u\,d(\mu\times\nu)
=\int_X\left(\int_Yu(x,y)\,d\nu(y)\right)d\mu(x)
=\int_Y\left(\int_Xu(x,y)\,d\mu(x)\right)d\nu(y).}
$$

All three [integrals](../../../../integral-split.md) are finite. Values of an inner [integral](../../../../integral-split.md) on an exceptional [null set](../../../../null-set.md) can be assigned arbitrarily.

**[Tonelli's theorem](../../../../tonelli-theorem.md):** if $u:X\times Y\to[0,\infty]$ is measurable and nonnegative, the same equality holds for its nonnegative product and iterated [integrals](../../../../integral-split.md), allowing the common value $+\infty$. No advance [absolute integrability](../../../../integrability.md) assumption is needed. On a completed [Lebesgue measure](../../../../lebesgue-measure.md) product, the section and measurability assertions are interpreted [almost everywhere](../../../../almost-everywhere.md).

Thus [Tonelli's theorem](../../../../tonelli-theorem.md) can first establish that $\int|u|<\infty$; after this, [Fubini's theorem](../../../../fubini-s-theorem.md) permits signed integration in either order.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
