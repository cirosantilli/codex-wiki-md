<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The three-component [finite Gaussian mixture with a common variance](../../../../../../finite-gaussian-mixture-with-a-common-variance.md) has the largest displayed maximized [log-likelihood](../../../../../../log-likelihood.md), but it also has more fitted parameters. For $k$ components there are $k-1$ free weights, $k$ means and one common variance, making **$d=2k$** residual-distribution parameters. Applying the nominal [Akaike information criterion](../../../../../../akaike-information-criterion.md) and [Bayesian information criterion](../../../../../../bayesian-information-criterion.md) to the three residual fits gives

$$
\begin{array}{c|r|r|r|r}
 k&\ell&d&\mathrm{AIC}=-2\ell+2d&\mathrm{BIC}=-2\ell+d\log500\\\hline
1&-1205.2500&2&2414.500&2422.929\\
2&-1193.8265&4&2395.653&2412.511\\
3&-1192.2715&6&2396.543&2421.831
\end{array}
$$

Both criteria favour **the two-component model**. It improves the likelihood substantially over one normal component; the third component gains only $1.5550$ in log-likelihood at a cost of two further parameters. The [Akaike information criterion](../../../../../../akaike-information-criterion.md) difference between two and three components is small, about $0.89$, so that criterion alone gives only a slight preference; the [Bayesian information criterion](../../../../../../bayesian-information-criterion.md) preference for two is stronger. Their nearly indistinguishable overlaid curves also support retaining the simpler two-component fit.

These calculations are model-selection aids, not an exact test. Ordinary chi-squared calibration of a [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) for the number of mixture components is invalid in general: under a smaller-component null, some weights lie on the boundary and extra-component parameters are unidentified. This is [nonregular mixture model selection](../../../../../../nonregular-mixture-model-selection.md). A parametric bootstrap or predictive [cross-validation](../../../../../../cross-validation.md) is preferable for a formal comparison, and should account for the mean-adjustment stage. The table uses the provided residual likelihoods and their nominal parameter counts; first-stage regression uncertainty and possible local EM maxima remain qualifications. **On the supplied evidence, select two components without claiming that two distinct biological groups have been established.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
