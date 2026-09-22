<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Treat the diagnosis counts as the observed [incidence](../../../../../../../incidence-epidemiology.md) series and define their total infectiousness by

$$
s_t=\sum_{\tau=1}^{t}g_\tau I_{t-\tau}.
$$

A conditionally independent [Poisson observation model](../../../../../../../poisson-observation-model.md) for the renewal process is

$$
I_t\mid R_t,g,I_0,\ldots,I_{t-1}\sim\operatorname{Poisson}(R_ts_t),
\qquad
p(I_1,\ldots,I_T\mid R,g)=\prod_{t=1}^{T}
\frac{e^{-R_ts_t}(R_ts_t)^{I_t}}{I_t!}.
$$

Initial infections before the observation window can be included in the definition of $s_t$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
