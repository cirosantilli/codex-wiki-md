# Photon-recoil lag correlation

↑ **Parent:** [Bothe-Geiger coincidence experiment](bothe-geiger-coincidence-experiment.md)

A [photon-recoil lag correlation](photon-recoil-lag-correlation.md) asks how often a [photon](photon.md) record occurs at a specified time displacement from an [electron](electron.md) record. Let $r_e,r_\gamma$ be observed separate-channel rates, $S$ the rate of detected genuine pairs before a timing cut, and $f(\ell)$ their normalized timing [probability density function](probability-density-function.md). For an original dilute, stationary model with observation time $T$, neglecting end effects and [detector dead time](detector-dead-time.md), the expected pair density is

$$
\frac{d\mathbb E[N]}{d\ell}
=T\bigl[r_er_\gamma+Sf(\ell)\bigr],\qquad
\int_{-\infty}^{\infty} f(\ell)\,d\ell=1.
$$

This counts all pairs of records, rather than at most one [detector trigger](trigger-particle-physics.md) per [electron](electron.md). It uses independent unrelated detections for the flat term and an added same-event contribution. A [normal distribution](normal-distribution.md) for timing spread is a chosen approximation, not a claim about the historical instrument. Intrinsic emission delay, counter response and readout uncertainty can all affect the observed [probability density function](probability-density-function.md).

Define the accepted lag interval by $|\ell|<w/2$: **$w$ is its full width**. Integrating the flat baseline gives the existing [accidental coincidence](accidental-coincidence.md) expectation $Tr_er_\gamma w$. The additional area is $TS\int_{-w/2}^{w/2}f(\ell)\,d\ell$. Moving a window of the same full width away from the peak tests the baseline under the model's stationarity assumption. It does not remove correlated instrumental backgrounds or changing rates automatically.

<a id="image-photon-recoil-joint-lag-correlation"></a>
![](photon-recoil-joint-lag-correlation.png)

**[Figure 4](#image-photon-recoil-joint-lag-correlation). Lag-dependent pairs and a joint probability distribution carry information absent from singles totals**. Original chosen models, not historical counts or fitted data. Left: a normalized [normal distribution](normal-distribution.md) of genuine-pair lags with [standard deviation](standard-deviation.md) $1\,\mathrm{ms}$ is added to an independent-pair baseline. Shaded intervals have full width $2\,\mathrm{ms}$, centered at zero and $5\,\mathrm{ms}$. Right: a separate exact ideal-bin model ignores timing spread; the two populations have identical singles expectations but different joint expectations.

For the lag model, choose $T=1000\,\mathrm s$, $r_e=2\,\mathrm{s^{-1}}$, $r_\gamma=0.5\,\mathrm{s^{-1}}$, $S=0.1\,\mathrm{s^{-1}}$ and timing [standard deviation](standard-deviation.md) $\sigma=1\,\mathrm{ms}$. A full width $w=2\,\mathrm{ms}$ gives $2$ expected [accidental coincidences](accidental-coincidence.md) and $100\operatorname{erf}(1/\sqrt2)\simeq68.27$ accepted genuine pairs, using the [error function](error-function.md). The total is approximately $70.27$, whereas the displaced interval from $4$ to $6\,\mathrm{ms}$ has approximately $2.003$ expected pairs. A finite sample fluctuates around these expectations; these values are not measured counts or a significance calculation.

The right panel isolates the information lost by retaining singles totals alone. In a separate idealized model, stipulate $M=10^6$ independent $1\,\mathrm{ms}$ bins, with [Bernoulli distribution](bernoulli-distribution.md) indicators $X,Y$ for [electron](electron.md) and [photon](photon.md) detection in a bin. Set $p_e=\Pr(X=1)=0.002$ and $p_\gamma=\Pr(Y=1)=0.0005$. [Independence](independent-random-variables.md) predicts $\Pr(X=1,Y=1)=p_ep_\gamma=10^{-6}$, hence one expected double detection. Alternatively choose

$$
\Pr(X=1,Y=1)=0.000101,\quad
\Pr(X=1,Y=0)=0.001899,\quad
\Pr(X=0,Y=1)=0.000399,\quad
\Pr(X=0,Y=0)=0.997601.
$$

These nonnegative [probabilities](probability.md) sum to one and preserve both marginal [probabilities](probability.md), yet predict $101$ double detections in expectation. Their [covariance](covariance.md) is $0.000101-p_ep_\gamma=0.000100$. This is an exact [joint probability distribution](joint-probability-distribution.md) illustrating pairing; it does not model the timing spread in the left panel or reconstruct either historical hypothesis quantitatively. Its lesson is why two singles totals cannot decide whether the observed events share a cause.

## ↑ Ancestors (7)

1. [Bothe-Geiger coincidence experiment](bothe-geiger-coincidence-experiment.md)
2. [X-ray](x-ray.md)
3. [Electromagnetic radiation](electromagnetic-radiation-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Photon-recoil lag correlation](photon-recoil-lag-correlation.md)
