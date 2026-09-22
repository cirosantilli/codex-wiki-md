<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Preserve the original row order and set $G_i=0$ for the first eight fixed-route providers and $G_i=1$ for the twelve on-demand providers. A suitable group comparison builds on a selected small predictor set $z_i$:

$$
\boxed{\log\mu_i=\beta_0+\gamma G_i+z_i^T\beta+G_i z_i^T\delta.}
$$

The model with $\gamma=0,\delta=0$ pools service types; adding $\gamma$ changes the baseline; adding selected components of $\delta$ allows different predictor dependence. Center $z$ at meaningful values so that $e^\gamma$ compares groups at those values. The predictor-specific [rate ratio](../../../../../../rate-ratio.md) is $e^{\beta_j}$ in the fixed-route group and $e^{\beta_j+\delta_j}$ in the on-demand group; the group ratio at predictor value $z$ is $e^{\gamma+z^T\delta}$.

Fit common-slope and selected-interaction models, respecting model hierarchy by retaining corresponding main effects. Test the added interaction block jointly with a [likelihood-ratio test](../../../../../../likelihood-ratio-test.md), or an appropriate quasi-likelihood comparison under estimated dispersion, and check group-specific residual patterns and leave-one-provider sensitivity. Seven interactions plus all main effects would use 16 parameters for just twenty providers and leave only four residual degrees of freedom; an indiscriminate full interaction model is consequently a poor basis for stable inference.

**The excerpt contains only $G=0$, so neither the service-type effect nor any interaction is estimable from it.** Full-data estimates could distinguish a baseline difference from genuinely different slopes, but the printed records cannot establish either conclusion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
