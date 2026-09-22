<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use equal allocation and a conventional two-sided 5% comparison of independent proportions. The assumed risks are $p_C=0.005$ and $p_I=0.005(1-0.30)=0.0035$, giving target difference $\delta=0.0015$. Put $\overline p=(p_C+p_I)/2=0.00425$ and let $m$ be the number per arm.

The null critical difference is approximately $z_{0.975}\sqrt{2\overline p(1-\overline p)/m}$. Under the alternative, the difference has standard deviation $\sqrt{[p_C(1-p_C)+p_I(1-p_I)]/m}$. For 80% [statistical power](../../../../../../statistical-power.md), the target difference must exceed the critical difference by $z_{0.8}$ alternative standard deviations. Solving gives the [sample size for comparing two proportions](../../../../../../sample-size-for-comparing-two-proportions.md)

$$
m\simeq\frac{\left[z_{0.975}\sqrt{2\overline p(1-\overline p)}+z_{0.8}\sqrt{p_C(1-p_C)+p_I(1-p_I)}\right]^2}{\delta^2}.
$$

This is about $29{,}500$ per arm, or $59{,}000$ altogether. Rounding for planning:

$$
\boxed{\text{about 60 thousand participants in total, roughly 30 thousand per arm}.}
$$

The rare-event Poisson approximation gives a similar answer. This assumes the stated baseline risk applies, no endpoint loss, and no attenuation by [treatment contamination](../../../../../../treatment-contamination.md). The two-sided convention is explicit: a one-sided 5% test would require fewer participants.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
