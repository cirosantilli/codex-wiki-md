<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Itô formula](../../../../../ito-s-lemma.md) for $B_t^2$ yields $\int_0^tB_u\,dB_u=(B_t^2-t)/2$. Substituting into the expression for $Z_t$ gives the pathwise identity

$$
Z_t=\exp\!\left[-\frac\beta2B_t^2+\frac{\beta t}{2}
-\frac{\beta^2}{2}\int_0^tB_u^2\,du\right].
$$

Consequently

$$
Z_t\exp\!\left[\left(\frac\beta2-\alpha\right)B_t^2-\frac{\beta t}{2}\right]
=\exp\!\left[-\alpha B_t^2-\frac{\beta^2}{2}\int_0^tB_u^2\,du\right].
$$

Taking [expected values](../../../../../expected-value-split.md) proves

$$
\boxed{L(t,\alpha,\beta)
=\mathbb E\!\left[Z_t\exp\!\left(\left(\frac\beta2-\alpha\right)B_t^2-\frac{\beta t}{2}\right)\right].}
$$

The random variable on the preceding line is bounded by one for $\alpha\geq0$, so its integrability is immediate.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
