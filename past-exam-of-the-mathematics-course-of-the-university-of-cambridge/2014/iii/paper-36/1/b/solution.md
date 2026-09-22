<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Among the supplied candidates, **choose [ARMA](../../../../../../autoregressive-moving-average-model.md)(2,1)**. It has the smallest [Akaike information criterion](../../../../../../akaike-information-criterion.md). Relative to [ARMA](../../../../../../autoregressive-moving-average-model.md)(2,2), its AIC improvement is $1.71$; the additional second moving-average estimate is only half a standard error from zero and increases the log [likelihood function](../../../../../../likelihood-function.md) by only about $0.14$. Dropping it is a reasonable parsimony choice, although that AIC gap is small. [ARMA](../../../../../../autoregressive-moving-average-model.md)(1,1) has AIC larger by $17.55$, a much clearer loss of fit. In the chosen model the second autoregressive term is about seven standard errors from zero, so it should not be dropped merely to obtain order one. The first autoregressive term is less precisely estimated; this does not justify automatically deleting it without fitting and comparing the reduced candidate.

Using the usual positive-sign moving-average convention, the fitted [autoregressive moving-average model](../../../../../../autoregressive-moving-average-model.md) is

$$
\boxed{X_t=-0.30X_{t-1}+0.28X_{t-2}+Z_t+0.50Z_{t-1},\qquad Z\sim\operatorname{WN}(0,4).}
$$

These are plug-in values rounded as given, not exact population parameters. The model has zero mean. Its polynomials are $\phi(z)=1+0.30z-0.28z^2=(1-0.4z)(1+0.7z)$ and $\theta(z)=1+0.5z$.

With angular frequency $\omega\in[-\pi,\pi]$, so that the [autocovariance](../../../../../../autocovariance.md) is $\gamma(h)=\int_{-\pi}^{\pi}e^{ih\omega}f_X(\omega)\,d\omega$, the [spectral density of a stationary process](../../../../../../spectral-density-of-a-stationary-process.md) is

$$
\boxed{f_X(\omega)=\frac4{2\pi}\frac{|1+0.5e^{-i\omega}|^2}{|1+0.30e^{-i\omega}-0.28e^{-2i\omega}|^2}
=\frac2\pi\frac{1.25+\cos\omega}{(1.16-0.8\cos\omega)(1.49+1.4\cos\omega)}.}
$$

The frequency convention makes the normalization unambiguous.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
