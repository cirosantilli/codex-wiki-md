<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [log-transformed location-scale model](../../../../../../log-transformed-location-scale-model.md), let $F_W$ denote the distribution function associated with $f$. The [change-of-variables formula for a probability density](../../../../../../change-of-variables-formula-for-a-probability-density.md) gives the untruncated density and distribution function

$$
p(t;\alpha,\sigma,q)=\frac{1}{\sigma t}f\left(\frac{\log t-\alpha}{\sigma};q\right),
\qquad F(t;\alpha,\sigma,q)=F_W\left(\frac{\log t-\alpha}{\sigma};q\right).
$$

Consequently its upper-truncated [likelihood](../../../../../../likelihood-function.md) is $\prod_i p(t_i)/F(M)^n$ on the observed support, and the [profile likelihood](../../../../../../profile-likelihood.md) maximizes this over $\alpha,\sigma,q$. Restricting to the corresponding subfamilies gives the [gamma distribution](../../../../../../gamma-distribution.md) and [lognormal distribution](../../../../../../log-normal-distribution.md) profiles. Write the plotted [likelihood ratio](../../../../../../likelihood-ratio.md) as

$$
R(M)=\frac{L_p(M)}{\sup_uL_p(u)}.
$$

It measures how well each endpoint fits relative to that model's own best endpoint, after nuisance refitting. It is not a [probability density function](../../../../../../probability-density-function.md) for $M$ and need not integrate to one. Endpoints whose ratios are near one are relatively compatible with the observations; a rapidly falling profile indicates more information favoring endpoints near the maximum.

**All three profiles favor the smallest admissible endpoint, approximately 14 days; their information about larger endpoints differs substantially.** Reading the actual PDF legend and curves, the dotted [gamma distribution](../../../../../../gamma-distribution.md) profile falls initially but is nearly flat around $0.60$ from about 18 days onward. The solid generalized log-gamma profile declines much further, to roughly $0.20$ at 19 days and $0.18$ at 21 days. The dashed [lognormal distribution](../../../../../../log-normal-distribution.md) profile falls most strongly, to roughly $0.14$ at 18 days and $0.08$ at 21 days. These are graphical readings, not recomputed fits.

Thus the [gamma distribution](../../../../../../gamma-distribution.md) fit gives weak discrimination between moderate and very large endpoints: much of its untruncated mass can already be below these endpoints, making further changes to the truncation have little effect. Over the displayed range, the [lognormal distribution](../../../../../../log-normal-distribution.md) fit gives stronger relative evidence against large endpoints, and the more flexible generalized log-gamma fit is intermediate. The solid curve remains close to the dashed curve near the maximum but has appreciably more relative support farther out. The plot shows slowing declines rather than a sharply determined finite upper endpoint; it cannot establish a biological maximum.

Normalization is essential to this comparison. Although the generalized family includes the two special families and therefore has at least as large a raw maximized [likelihood](../../../../../../likelihood-function.md) at any fixed $M$, its normalization constant can also be larger. Its normalized profile need not lie above the normalized profiles of its submodels. Their individual maxima have all been replaced by one, so this plot alone cannot compare overall goodness of fit or select a family while accounting for extra fitted parameters.

A set $\{M:R(M)\geq c\}$ is a relative-likelihood support set once $c$ is chosen. Turning it into a calibrated [confidence interval](../../../../../../confidence-interval.md) requires an appropriate sampling argument, simulation or other justified method. In particular, a usual [Wilks theorem](../../../../../../wilks-theorem.md) chi-squared cutoff cannot simply be assumed for this changing-support endpoint problem. The original incubation observations are not supplied here, so numerical refitting or calibrated limits cannot be recovered from the graph alone.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
