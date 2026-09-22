<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For data $D$, parameters $\theta$ and model $M$, [conditional probability](../../../../../conditional-probability.md) gives

$$
\boxed{p(\theta\mid D,M)=\frac{p(D\mid\theta,M)\,p(\theta\mid M)}{p(D\mid M)},\qquad p(D\mid M)=\int p(D\mid\theta,M)p(\theta\mid M)\,d\theta.}
$$

The [likelihood](../../../../../likelihood-function.md) describes the measurement process, the [prior](../../../../../prior-probability.md) encodes parameter information before these data, and the [Bayesian evidence](../../../../../bayesian-model-evidence.md) normalizes the [posterior](../../../../../bayesian-posterior.md). A [prior](../../../../../prior-probability.md) is a [probability density](../../../../../probability-density.md) with respect to a specified measure; a uniform [prior](../../../../../prior-probability.md) in distance is not uniform in parallax. [Bayes' theorem](../../../../../bayes-theorem.md) combines [conditional probabilities](../../../../../conditional-probability.md) and does not itself select an appropriate [likelihood](../../../../../likelihood-function.md) or [prior](../../../../../prior-probability.md).

An astronomical application starts with a forward model. For measured fluxes $d_i$ with predictions $f_i(\theta)$ and known Gaussian covariance $C$, $L\propto|C|^{-1/2}\exp[-(d-f)^{\mathsf T}C^{-1}(d-f)/2]$. Correlated [calibration](../../../../../calibration-differential-geometry.md) errors belong in $C$ or in explicit [calibration](../../../../../calibration-differential-geometry.md) [nuisance parameters](../../../../../nuisance-parameter.md); assuming every filter or epoch is independent can give falsely narrow uncertainties. For a faint photon-counting source, the more appropriate [likelihood](../../../../../likelihood-function.md) can instead be $p(N\mid s,b)=e^{-(s+b)}(s+b)^N/N!$, with nonnegative expected source and background counts. Background measurements constrain $b$, which is then marginalized rather than set to an exact subtracted number. The observed background-subtracted count can be negative even though the physical expected source count is nonnegative.

For a simple flux example with $d\mid F\sim\mathcal N(F,\sigma^2)$ and a Gaussian [calibration](../../../../../calibration-differential-geometry.md) [prior](../../../../../prior-probability.md) $F\sim\mathcal N(F_0,\sigma_0^2)$, completing the square gives

$$
\sigma_p^{-2}=\sigma^{-2}+\sigma_0^{-2},\qquad F_p=\sigma_p^2\left(\frac d{\sigma^2}+\frac{F_0}{\sigma_0^2}\right).
$$

This explicitly shows how independent information combines. A physical nonnegative-flux [prior](../../../../../prior-probability.md) would truncate or replace that illustrative Gaussian [prior](../../../../../prior-probability.md). Photometric-redshift fitting similarly compares predicted [galaxy](../../../../../galaxy-split.md) colours with measured fluxes, then integrates over [luminosity](../../../../../luminosity.md), dust and other [nuisance parameters](../../../../../nuisance-parameter.md) to obtain $p(z\mid D)$. Multimodal [posteriors](../../../../../bayesian-posterior.md) should be retained when different spectral features produce similar colours; a best fit alone hides that ambiguity. The same framework applies to orbit parameters, stellar [temperatures](../../../../../temperature-split.md), cosmological parameters and cluster SZ amplitudes.

[credible intervals](../../../../../credible-interval.md) state [posterior](../../../../../bayesian-posterior.md) [probability](../../../../../probability.md) conditional on the model and [prior](../../../../../prior-probability.md). [posterior predictive checks](../../../../../posterior-predictive-check.md) compare replicated observations with the data and can reveal a deficient noise or source model. Sensitivity to plausible [priors](../../../../../prior-probability.md) is especially important for weak signals and inverse problems. For competing models, [posterior](../../../../../bayesian-posterior.md) odds equal [prior](../../../../../prior-probability.md) odds times the [Bayes factor](../../../../../bayes-factor.md) $Z_1/Z_2$; the evidence averages fit quality over the [prior](../../../../../prior-probability.md) volume and therefore depends on proper, physically justified [prior](../../../../../prior-probability.md) ranges. Detection thresholds and catalogue selection must enter the sampling model when inferring a population, otherwise a carefully calculated [posterior](../../../../../bayesian-posterior.md) can still describe a biased sample. **The practical gain is a joint uncertainty distribution with [nuisance parameters](../../../../../nuisance-parameter.md) propagated, not merely a single fitted number.**

## ↑ Ancestors (14)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the frontiers of Observational Astrophysics course of the University of Cambridge](../../../../split.md)
6. [Frontiers of Observational Astrophysics course of the University of Cambridge](../../../../../frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
