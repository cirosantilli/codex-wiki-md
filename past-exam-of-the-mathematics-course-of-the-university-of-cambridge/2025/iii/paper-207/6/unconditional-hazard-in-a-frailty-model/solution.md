<h1 id="6/unconditional-hazard-in-a-frailty-model/solution">Solution</h1>

↑ **Parent:** [Unconditional hazard in a frailty model](../unconditional-hazard-in-a-frailty-model.md)

A [frailty model](../../../../../../frailty-model.md) introduces an unobserved positive random effect $U$ that multiplies an individual's hazard. With $H_0(t)=\int_0^th_0(s)ds$, marginal survival is

$$
\bar S(t)=\int_0^\infty e^{-uH_0(t)}g(u)du.
$$

Differentiation gives

$$
\bar h(t)=h_0(t)
\frac{\int_0^\infty u e^{-uH_0(t)}g(u)du}
{\int_0^\infty e^{-uH_0(t)}g(u)du}
=h_0(t)\mathbb E[U\mid T\geq t].
$$

**Consequently $\bar h(0)=h_0(0)$ exactly when $\mathbb EU=1$.**

## ↑ Ancestors (11)

1. [Unconditional hazard in a frailty model](../unconditional-hazard-in-a-frailty-model.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
