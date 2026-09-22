<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A [random-effects meta-analysis](../../../../../../random-effects-meta-analysis.md) allows differences in true treatment effects across countries and eligibility criteria. For trial $i=1,\ldots,6$, let $y_i$ be its estimated [log odds ratio](../../../../../../log-odds-ratio.md) and $v_i$ its estimated within-trial [variance](../../../../../../variance-split.md). A usual approximate [statistical model](../../../../../../statistical-model-split.md) is

$$
y_i\mid\delta_i\sim N(\delta_i,v_i),\qquad \delta_i=\mu+b_i,\qquad b_i\sim N(0,\tau^2),
$$

independently across trials, with $b_i$ [independent](../../../../../../independent-random-variables.md) of sampling errors. Here $\mu$ is the mean true [log odds ratio](../../../../../../log-odds-ratio.md) in the population of comparable trials, and $\tau^2\geq0$ is between-trial heterogeneity, not additional sampling error. Therefore $y_i\sim N(\mu,v_i+\tau^2)$, and for a fitted heterogeneity value,

$$
\boxed{\widehat\mu=\frac{\sum_iw_i y_i}{\sum_iw_i},\qquad w_i=(v_i+\widehat\tau^2)^{-1}.}
$$

One can estimate $\tau^2$ by [restricted maximum likelihood](../../../../../../restricted-maximum-likelihood.md) or another justified method; $(\sum_iw_i)^{-1}$ is a plug-in conditional [variance](../../../../../../variance-split.md) and does not fully account for estimating heterogeneity. With only six studies that uncertainty matters. Different eligibility rules motivate this [random effect](../../../../../../random-effect.md) but do not by themselves establish exchangeability or remove [bias](../../../../../../bias-of-an-estimator.md); known [effect modifiers](../../../../../../effect-modifier.md) may warrant stratification or regression.

Use [leave-one-study-out influence analysis](../../../../../../leave-one-study-out-influence-analysis.md): fit all six trials, then omit Cohen 1989 and refit both $\mu$ and $\tau^2$. Report $\widehat\mu-\widehat\mu_{(-C)}$, the corresponding change in the [odds ratio](../../../../../../odds-ratio.md), and changes in the [confidence interval](../../../../../../confidence-interval.md) and heterogeneity. As a diagnostic with heterogeneity held fixed, writing $W=\sum_iw_i$ gives

$$
\widehat\mu-\widehat\mu_{(-C)}=\frac{w_C}{W-w_C}(y_C-\widehat\mu).
$$

The fitted Cohen weight would be $(0.15+\widehat\tau^2)^{-1}$ and $y_C=-1.95$. A precise but discordant trial can have large influence; refitting assesses additional influence through heterogeneity. The other five trials' data are absent, so a numerical six-trial influence assessment is not identifiable from the displayed table.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
