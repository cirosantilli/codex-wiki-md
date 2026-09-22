<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume the [infectivity profile](../../../../../../../infectivity-profile.md) is separable:

$$
\beta_{t,\tau}=R_tg_\tau,
\qquad g_\tau\geq0,
\qquad \sum_{\tau\geq1}g_\tau=1.
$$

Then $g_\tau$ is the discretized [generation-interval distribution](../../../../../../../generation-interval-distribution.md), $R_t$ is the [instantaneous reproduction number](../../../../../../../instantaneous-reproduction-number.md), and the [infectious disease renewal equation](../../../../../../../infectious-disease-renewal-equation.md) becomes

$$
\Delta_t=R_t\Lambda_t,
\qquad
\Lambda_t=\sum_{\tau=1}^{t}g_\tau\Delta_{t-\tau}.
$$

**Hence $R_t=\Delta_t/\Lambda_t$ whenever the total infectiousness $\Lambda_t$ is positive.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
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
