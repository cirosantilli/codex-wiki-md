<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If equally informative independent draws have variance $s_m^2$, an ordinary mean of $K_{\mathrm{eff}}$ draws has variance $s_m^2/K_{\mathrm{eff}}$. The weighted mean has the corresponding variance $s_m^2\sum_iw_i^2$. Equating them gives the [effective sample size of importance sampling](../../../../../../effective-sample-size-of-importance-sampling.md)

$$
K_{\mathrm{eff}}=\frac1{\sum_{i=1}^Kw_i^2}
=\frac{\left(\sum_i p(d\mid x_i)\right)^2}
{\sum_i p(d\mid x_i)^2}\leq K,
$$

where the inequality follows from [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
