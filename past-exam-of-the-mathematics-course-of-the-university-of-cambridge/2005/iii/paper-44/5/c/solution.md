<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the original PDF's value $\widehat p=0.386$; the TeX aid misreads its last digit. In the fitted conditional mixture, $\widehat\theta=0.575$ means that about **57.5% are assigned to the structural-zero, or modelled cured, component**. Its asymptotic 95% [confidence interval](../../../../../../confidence-interval.md) of $(0.30,0.81)$ shows substantial uncertainty about that fraction. An observed post-treatment zero alone is not proof of cure, since the non-cured [Poisson distribution](../../../../../../poisson-distribution.md) can also produce zero.

The parameter $p$ is a conditional allocation probability, not the ratio of post-treatment to pre-treatment means. That ratio among non-cured patients is $\beta=p/(1-p)$. Hence

$$
\widehat\beta=\frac{0.386}{1-0.386}\simeq0.629,
\qquad
\boxed{\text{estimated mean-count reduction among non-cured patients}\simeq37.1\%.}
$$

The map $p\mapsto p/(1-p)$ is strictly increasing, so transform the endpoints of the supplied 95% [confidence interval](../../../../../../confidence-interval.md):

$$
\boxed{\beta\in\left(\frac{0.27}{0.73},\frac{0.52}{0.48}\right)
\simeq(0.370,1.083).}
$$

No change in the non-cured mean is $\beta=1$, equivalently $p=1/2$, which lies in this interval. Thus the point estimate suggests a reduction, but this interval does not firmly establish one among the non-cured patients at the corresponding two-sided 5% level. It is not correct to describe $p=0.386$ itself as a 61.4% reduction in their mean count.

Under a full pre-conditioning mixture with cure independent of the baseline rate, the population mean ratio would be $(1-\theta)\beta$, whose plug-in value is about $0.425(0.629)=0.267$. This combines disappearance of counts in one component with a change of rate in the other; it is distinct from the conditional estimate's direct interpretation. The two marginal [confidence intervals](../../../../../../confidence-interval.md) cannot simply be multiplied to obtain a calibrated joint 95% interval for this derived quantity.

Only 12 patients were observed, so the asymptotic intervals, particularly for a mixture parameter near a boundary, should be interpreted cautiously. The data describe one-minute counts and do not establish permanent cure. Nor does an uncontrolled before-and-after comparison alone prove a [causal effect](../../../../../../causal-effect.md) of the drug: natural count variability, secular changes and [regression to the mean](../../../../../../regression-to-the-mean.md) remain possible. The structural-zero interpretation and the reduction among non-cured patients are conclusions within the specified statistical model.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
