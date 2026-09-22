<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The likelihood-ratio statistic is

$$
\boxed{G^2=2[-1201.56-(-1202.92)]=2.72.}
$$

The [null hypothesis](../../../../../../null-hypothesis.md) $\pi=0$ is at the boundary of the permitted mixture weights. Assuming the remaining parameters are identifiable and interior, including $\tau>0$, an efficient normalized score for $\pi$ is asymptotically $Z\sim N(0,1)$ under the [null hypothesis](../../../../../../null-hypothesis.md). The locally unconstrained quadratic [log-likelihood](../../../../../../log-likelihood.md) maximizer is proportional to $Z$, while the constrained maximizer truncates it at zero. Thus $G^2\Rightarrow(\max(0,Z))^2$, giving the [one-sided boundary likelihood-ratio limit](../../../../../../single-parameter-boundary-likelihood-ratio-test.md)

$$
\boxed{G^2\ \overset{\rm approx}{\sim}\ \tfrac12\delta_0+\tfrac12\chi^2_1.}
$$

Here $\delta_0$ is a [point mass](../../../../../../point-mass.md) at zero. For a positive observed statistic the upper-tail probability is half the ordinary $\chi^2_1$ upper tail. The 5% critical value is the 90th percentile of $\chi^2_1$, about 2.7055, displayed as 2.71. Hence **the reported likelihoods give a very marginal rejection of $\pi=0$ at 5%**, with $p\simeq0.04955$.

Using the ordinary 95th-percentile cutoff 3.84 would be inappropriate for this one-sided boundary test. The conclusion is close enough to the threshold that likelihood rounding matters: since each [log-likelihood](../../../../../../log-likelihood.md) is printed to two decimals, the unrounded statistic can differ from 2.72 by nearly 0.02. The intended calculation rejects using the reported values, but an exact decision from the fitted data requires unrounded likelihoods. If the nuisance dispersion is also on its boundary or the mixture is not identifiable, the stated half-and-half null distribution needs reconsideration.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
