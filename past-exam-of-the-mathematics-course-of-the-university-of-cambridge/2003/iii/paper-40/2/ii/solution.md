<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Collect distinct observed failure times as $a_m$, with $d_m$ failures and $r_m$ individuals in the [risk set](../../../../../../risk-set.md) just before $a_m$. The grouped [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) is

$$
\boxed{\widehat H_{\rm NA}(t)=\sum_{a_m\le t}\frac{d_m}{r_m}.}
$$

All failures recorded at one time use the same pre-event [risk set](../../../../../../risk-set.md). When failures and [censoring](../../../../../../censoring-statistics.md) share a recorded time, the usual convention includes those censored at that time in the [risk set](../../../../../../risk-set.md) and processes failures before removing censored individuals. A known different ordering should instead be honored. If ties arise solely through rounding of a continuous-time process, an alternative is to resolve the unobserved ordering: $d_m$ successive failures without intervening [censoring](../../../../../../censoring-statistics.md) would contribute $\sum_{s=0}^{d_m-1}(r_m-s)^{-1}$. That is not the grouped jump $d_m/r_m$; the difference represents a choice about what the recorded ties mean.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
