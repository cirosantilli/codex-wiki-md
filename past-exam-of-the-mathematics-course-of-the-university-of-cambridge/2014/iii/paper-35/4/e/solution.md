<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The overall mean $\mu$ and the [between-study heterogeneity](../../../../../../between-study-heterogeneity.md) $\tau$ encode different information. A proper broad [normal distribution](../../../../../../normal-distribution.md) prior such as $\mu\sim N(0,2^2)$ is one possible weak prior for the mean [log odds ratio](../../../../../../log-odds-ratio.md); information about the spread of trials alone does not determine its center.

A concrete [prior calibration for normal random-effect range](../../../../../../prior-calibration-for-normal-random-effect-range.md) can make the factor-of-50 statement simultaneous across all six trials. Conditional on $\tau$, each pair difference has [normal distribution](../../../../../../normal-distribution.md) $\beta_j-\beta_k\sim N(0,2\tau^2)$. Set $R=\log50$, $m=\binom62=15$, $z=\Phi^{-1}(1-0.05/(2m))$ and

$$
\boxed{\tau\sim\operatorname{Uniform}(0,A),\qquad A=\frac{R}{\sqrt2\,z}\simeq0.9424.}
$$

For every $\tau\le A$, each pair exceeds $R$ in absolute value with probability at most $0.05/m$. The [union bound](../../../../../../boole-s-inequality.md) therefore gives $\mathbb P(\max_j\beta_j-\min_j\beta_j>R)\le0.05$, and integrating over the [uniform prior](../../../../../../uniform-prior.md) preserves that bound. This is one explicit interpretation of “very unlikely”; a different elicited probability would change the bound. A smoother proper scale prior could be calibrated similarly.

The proposed $1/\tau$ [improper prior](../../../../../../improper-prior.md) is unsuitable. The observed-data [likelihood function](../../../../../../likelihood-function.md) approaches the positive common-effect likelihood as $\tau\downarrow0$. After restricting $\mu$ and the intercepts to a compact interior region, it is bounded below there by a positive constant. Hence

$$
\int_0^\varepsilon L(\mu,\tau)\frac{d\tau}{\tau}=\infty.
$$

This is an [improper posterior from a log-uniform random-effect scale prior](../../../../../../improper-posterior-from-a-log-uniform-random-effect-scale-prior.md). **Proper conditional sampling distributions do not repair the improper joint posterior**, and an arbitrary tiny cutoff would make inference depend on that cutoff.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
