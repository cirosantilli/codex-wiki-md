<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose an individual uniformly from the population. The [law of total probability](../../../../../../law-of-total-probability.md) gives **the population density and survivor function** as mixtures:

$$
\boxed{\overline f(t)=\frac1n\sum_{i=1}^n f_i(t),\qquad\overline F(t)=\frac1n\sum_{i=1}^n F_i(t).}
$$

A [hazard function](../../../../../../hazard-function.md) is a ratio of density to survival, so averaging the densities does not average those ratios. Instead,

$$
\boxed{\overline h(t)=\frac{\sum_iF_i(t)h_i(t)}{\sum_iF_i(t)}=\sum_iw_i(t)h_i(t),\qquad w_i(t)=\frac{F_i(t)}{\sum_jF_j(t)}.}
$$

These are the proportions of the original individual types among those still event-free at $t$, rather than their equal starting proportions. For example, a mixture of different [exponential distributions](../../../../../../exponential-distribution.md) progressively favours the lower-rate individuals. This [population hazard of a survival mixture](../../../../../../population-hazard-of-a-survival-mixture.md) generally differs from $n^{-1}\sum_i h_i(t)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
