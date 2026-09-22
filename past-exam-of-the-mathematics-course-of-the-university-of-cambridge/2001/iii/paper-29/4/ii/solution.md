<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [posterior mean](../../../../../../posterior-mean.md) is a weighted average of the sample proportion and prior mean:

$$
\frac{9+\alpha}{90+\kappa}
=\frac{90}{207.75}(0.10)+\frac{117.75}{207.75}(0.05).
$$

Thus it is pulled from 10% toward the prior's 5%, giving about 7.17%. This is an [affine shrinkage estimator for a binomial proportion](../../../../../../affine-shrinkage-estimator-for-a-binomial-proportion.md). The prior carries substantial concentration relative to the 90 observations, so the posterior is also more precise under this model: its standard deviation is about $0.01785$, compared with the binomial plug-in standard error $\sqrt{0.1(0.9)/90}=0.03162$. The posterior 95% [credible interval](../../../../../../credible-interval.md) $[0.04076,0.11035]$ is narrower and shifted down compared with the simple Wald interval $[0.03802,0.16198]$ based on $9/90$ alone.

**The point estimate shrinks toward the historical mean, and the interval is narrower under the informative prior.** A [credible interval](../../../../../../credible-interval.md) and a frequentist [confidence interval](../../../../../../confidence-interval.md) have different [probability](../../../../../../probability.md) interpretations; the comparison does not make the prior's relevance automatic.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
