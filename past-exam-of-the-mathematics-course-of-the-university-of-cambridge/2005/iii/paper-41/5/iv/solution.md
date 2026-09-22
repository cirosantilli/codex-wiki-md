<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

One presentation is the [cost-effectiveness plane](../../../../../../cost-effectiveness-plane.md), with $\Delta E$ horizontally and $\Delta C$ vertically. Plot the point estimate $(45,1800)$ with a joint [confidence region](../../../../../../confidence-region.md) or paired [bootstrap](../../../../../../bootstrapping-statistics.md) cloud. Its position shows the tradeoff quadrant, while the cloud shows uncertainty, dependence and possible dominance. A willingness-to-pay threshold $\lambda$ is the line $\Delta C=\lambda\Delta E$ through the origin. Points below that line have positive [incremental net monetary benefit](../../../../../../incremental-net-monetary-benefit.md), including points in quadrants where a ratio rule would fail. The point-estimated switch occurs at $\lambda=40$ pounds per day.

A second presentation is a [cost-effectiveness acceptability curve](../../../../../../cost-effectiveness-acceptability-curve.md), giving an uncertainty-based measure of cost-effectiveness for a range of thresholds. For paired [bootstrap](../../../../../../bootstrapping-statistics.md) increments $(\Delta E^{*(b)},\Delta C^{*(b)})$, plot

$$
\widehat p(\lambda)=\frac1B\sum_{b=1}^B
\mathbf1\{\lambda\Delta E^{*(b)}-\Delta C^{*(b)}>0\}.
$$

This counts positive net benefits, not merely ratios below the threshold, so it handles all quadrants. Using [Bayesian inference](../../../../../../bayesian-statistics.md) the curve is the [posterior probability](../../../../../../posterior-probability.md) that [incremental net monetary benefit](../../../../../../incremental-net-monetary-benefit.md) is positive; a frequentist bootstrap curve is a resampling summary, not literally a probability that a fixed parameter is positive.

Here the estimated [incremental net monetary benefit](../../../../../../incremental-net-monetary-benefit.md) and its [standard error](../../../../../../standard-error.md) are

$$
\widehat{\operatorname{INMB}}(\lambda)=45\lambda-1800,\qquad
s_{\mathrm{INMB}}(\lambda)=\sqrt{225\lambda^2-4500\lambda+90000}.
$$

Thus a [normal approximation](../../../../../../normal-approximation.md) uncertainty curve is

$$
\widehat p(\lambda)\approx
\Phi\!\left(\frac{45\lambda-1800}{\sqrt{225\lambda^2-4500\lambda+90000}}\right).
$$

It passes through one half at £40 per day. Alternatively display the [incremental net monetary benefit](../../../../../../incremental-net-monetary-benefit.md) curve itself with approximate pointwise $95\%$ bands $45\lambda-1800\pm1.96s_{\mathrm{INMB}}(\lambda)$. **The plane preserves the joint uncertainty; the acceptability curve shows how the threshold changes the cost-effectiveness assessment.** Neither presentation chooses society's willingness-to-pay threshold.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
