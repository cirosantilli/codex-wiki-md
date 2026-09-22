<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [logit link](../../../../../../logit.md) $g(\pi)=\log\{\pi/(1-\pi)\}$ and independent counts $R_{ij}\sim\operatorname{Bin}(n_{ij},\pi_{ij})$. This gives a [grouped-binomial logistic regression](../../../../../../grouped-binomial-logistic-regression.md) with 24 cells and 13 free coefficients: an intercept, 11 centre contrasts, and one period contrast. Reference [treatment coding](../../../../../../treatment-coding.md) makes the intercept the log odds for Centre 1 in the earlier of the two included periods. The two [factors](../../../../../../regression-factor.md) are assumed to have been coded as specified in the question.

The binomial [log-likelihood](../../../../../../log-likelihood.md), apart from known constants, is

$$
\ell=\sum_{i,j}\{r_{ij}\eta_{ij}-n_{ij}\log(1+e^{\eta_{ij}})\},\qquad
\eta_{ij}=\mu+\alpha_i+\beta_j.
$$

Maximize by [Fisher scoring](../../../../../../scoring-algorithm.md) or [iteratively reweighted least squares](../../../../../../iteratively-reweighted-least-squares.md). Using response proportions $r_{ij}/n_{ij}$ with binomial trial weights $n_{ij}$ is equivalent to using the count response $(r_{ij},n_{ij}-r_{ij})$; omitting those weights would give the wrong [likelihood](../../../../../../likelihood-function.md) and [standard errors](../../../../../../standard-error.md). The coefficient [covariance matrix](../../../../../../covariance-matrix.md) is approximately the inverse of $X^T\operatorname{diag}\{n_{ij}\widehat\pi_{ij}(1-\widehat\pi_{ij})\}X$.

The fitted reference log odds are $-0.809585$, and the period change is $-0.426758$, giving

$$
\boxed{\widehat\pi_{1,2}=0.30798,\qquad \widehat\pi_{1,3}=0.22507.}
$$

These are fitted probabilities under a common period effect, so they need not equal the separate empirical proportions at Centre 1. The estimated period [odds ratio](../../../../../../odds-ratio.md) is

$$
\boxed{e^{-0.426758}=0.6526,\qquad 95\%\text{ CI}=e^{-0.426758\pm1.96(0.078807)}=(0.5592,0.7616).}
$$

Thus the later-period death odds are estimated to be about 35% lower at each centre, with strong evidence of a period effect: the normal [Wald statistic](../../../../../../wald-test.md) is $-5.415$. The displayed “t value” is a coefficient divided by its [standard error](../../../../../../standard-error.md); with fixed binomial dispersion its usual large-sample calibration is standard normal, not a Student distribution with an estimated Gaussian-error [variance](../../../../../../variance-split.md). The [odds ratio](../../../../../../odds-ratio.md) is not a mortality [probability](../../../../../../probability.md) ratio.

Each centre coefficient is a log [odds ratio](../../../../../../odds-ratio.md) relative to Centre 1, adjusted for period. All its point estimates are negative, so all other centres have lower fitted mortality probabilities in either period. For example, Centre 11's [odds ratio](../../../../../../odds-ratio.md) is $e^{-1.079474}=0.3398$, or about $2.94$ times greater odds at Centre 1 than at Centre 11. Individual unadjusted two-sided [Wald tests](../../../../../../wald-test.md) find significant differences at the 5% level for centres 2, 4, 6, 7, 8, 9, 11 and 12; the coefficients for 3, 5 and 10 do not individually reach that threshold. These separate tests are correlated comparisons against a common reference and should not be presented as 11 independent discoveries without considering [multiple testing](../../../../../../multiple-hypothesis-testing.md). They adjust only for time period, not for differing patient case mix.

For fit assessment, the residual [binomial deviance](../../../../../../binomial-deviance.md) is $15.73891$ on $24-13=11$ [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md). Its $\chi^2_{11}$ upper tail is approximately $0.151$, so there is no appreciable evidence of lack of fit to these binomial cell counts. In particular, comparing with a saturated centre-by-period model gives this same deviance and 11 additional parameters; the data do not strongly require a centre-period [interaction](../../../../../../interaction-statistics.md). The moderate deviance residuals are consistent with that assessment, although a residual plot by centre and period would be more informative than the five-number summary alone.

The reduction from null to fitted deviance is

$$
119.0659-15.73891=103.32699.
$$

It tests the 12 centre-and-period coefficients jointly against an intercept-only model, with reference $\chi^2_{12}$ and $p\approx1.24\times10^{-16}$. It is not a centre-only test adjusted for period. For that test, fit the period-only model and compare its deviance with the full fit: the pooled binomial probabilities in each period give deviance $90.34578$, so

$$
\boxed{D_{\text{period only}}-D_{\text{centre+period}}=74.60687,\quad 11\text{ df},\quad p\approx1.61\times10^{-11}.}
$$

Thus centre heterogeneity persists after allowing for period. Dispersion one is the stipulated binomial [variance](../../../../../../variance-split.md), and the five scoring iterations describe numerical convergence rather than statistical evidence. The fitted associations alone do not establish a causal difference in surgical quality.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
