<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a [bootstrap-t confidence interval](../../../../../../../bootstrap-t-confidence-interval.md), estimate the original [standard error](../../../../../../../standard-error.md) $\widehat s$ of $\widehat r$, for example by the standard deviation of the outer [paired bootstrap](../../../../../../../paired-bootstrap.md) correlations. For each outer resample $b$, estimate its own [standard error](../../../../../../../standard-error.md) $s_b^*$ by drawing many inner paired resamples from that outer sample and taking the standard deviation of their correlations. The resulting studentized statistics are

$$
T_b^*=\frac{r_b^*-\widehat r}{s_b^*}.
$$

Let $t_p^*$ be their empirical quantiles. Approximating the distribution of $(\widehat r-r)/\widehat s$ by that of $T^*$ and solving the two inequalities for $r$ gives

$$
\boxed{[\widehat r-t_{0.975}^*\widehat s,\ \widehat r-t_{0.025}^*\widehat s].}
$$

The reversal of quantiles is essential. The pivot requires positive [standard errors](../../../../../../../standard-error.md) and nondegenerate correlations; its claimed 95% coverage is an approximation under [bootstrap](../../../../../../../bootstrapping-statistics.md) regularity, not an exact finite-sample guarantee. One may intersect the final interval with the parameter space $[-1,1]$.

The same percentile and studentized procedures can be applied to the [sample mean](../../../../../../../sample-mean.md) of $X$, and then only the $X$ observations need be resampled. They are useful when a normal approximation is doubtful. However the mean already has the simple standard-error estimate $S_X/10$ here. For normal observations, the classical exact interval is

$$
\boxed{\overline X\pm t_{99,0.975}\frac{S_X}{10},}
$$

and the same form is an asymptotic approximation for independent finite-variance observations under appropriate large-sample conditions. Thus [bootstrap](../../../../../../../bootstrapping-statistics.md) intervals are valid alternatives, but are often unnecessary for a mean with a reliable classical pivot; the correlation has no corresponding distribution-free elementary pivot. An infinite-variance distribution would require other theory rather than this ordinary standard-error argument.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
