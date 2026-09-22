<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Model deaths in disjoint equal-duration periods as independent observations with [Poisson distributions](../../../../../../poisson-distribution.md) with comparable population exposure and ascertainment. The expected before and after counts are $\mu_0=400$ and $\mu_1=320$. Their difference has

$$
\mathbb E(D_0-D_1)=80,\qquad\operatorname{Var}(D_0-D_1)=400+320=720.
$$

The expected signal relative to its standard deviation is therefore

$$
\boxed{80/\sqrt{720}\simeq2.98.}
$$

Under the null of equal rates, condition on $N=D_0+D_1$: the first-period count has a [binomial distribution](../../../../../../binomial-distribution.md) with parameters $N$ and $1/2$. At a total near 720, the two-sided 5% rejection boundary for $D_0-D_1$ is approximately $1.96\sqrt{720}$. Under the proposed alternative, conditional on that total, its mean is $N/9$ and its variance is $80N/81$. Thus at $N=720$ the [normal approximation](../../../../../../normal-approximation.md) gives power approximately

$$
\boxed{\Phi\left(\frac{80-1.96\sqrt{720}}{\sqrt{720\cdot80/81}}\right)\simeq0.85.}
$$

The lower-tail rejection probability is negligible at this alternative; allowing the Poisson total to fluctuate and using discrete rejection cutoffs changes the approximation slightly: an exact two-sided conditional test has about $83.8\%$ power under these Poisson means. **Two years on each side should have adequate power for a 20% reduction under this model**, though a particular realization can still fail to detect it.

This conclusion needs stable recording of drug-related deaths, comparable exposure denominators and no substantial [overdispersion](../../../../../../overdispersion.md) or temporal dependence. A change in population size, certification practice or other drug use can affect the comparison. Detecting a decline does not establish that [mephedrone](../../../../../../mephedrone.md) caused it: attributing displacement requires a credible comparison of [potential outcomes](../../../../../../potential-outcome.md), using an otherwise expected trend or other controls for changes occurring at the same time.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
