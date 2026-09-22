<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the target model $p_0=0.20$, the [normal approximation](../../../../../../normal-approximation.md) gives

$$
\widehat p\approx N\left(0.20,\frac{0.20(0.80)}n\right).
$$

The pointwise 95% [binomial funnel control limits](../../../../../../binomial-funnel-control-limits.md) are therefore

$$
\boxed{L(n)=\max\left(0,0.20-1.96\frac{0.40}{\sqrt n}\right),\qquad U(n)=\min\left(1,0.20+1.96\frac{0.40}{\sqrt n}\right).}
$$

Draw these curves around the horizontal 20% target, as in the figure. At $n=100$, the approximate limits are $0.1216$ and $0.2784$, so B and H are outside the nominal bands; that is a signal for investigation, not proof of inferior or superior care. The bands use the target [variance](../../../../../../variance-split.md) rather than each hospital's observed rate. They are [control limits](../../../../../../control-limits.md) for possible observations under the target model, not [confidence intervals](../../../../../../confidence-interval.md) centered on the observed points.

Normal coverage is approximate, especially for the small hospitals; clipping does not repair that approximation. Exact binomial tail limits can be used if exact calibration is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
