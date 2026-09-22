<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fit a stimulus-conditioned [linear-nonlinear-Poisson cascade model](../../../../../../linear-nonlinear-poisson-cascade-model.md). Choose a causal stimulus-history window, subtract the stimulus mean, and estimate a temporal filter $k$. A useful initial estimate is the [spike-triggered average](../../../../../../spike-triggered-average.md), $\widehat a(u)=N^{-1}\sum_i[s(t_i-u)-\bar s]$. For white Gaussian stimulation and a one-filter response, this estimates the filter direction. With correlated Gaussian stimulation it estimates a direction proportional to $Ck$, where $C$ is the history [covariance matrix](../../../../../../covariance-matrix.md); use [stimulus-correlated spike-triggered averaging](../../../../../../stimulus-correlated-spike-triggered-averaging.md) to whiten or regularize this correction. An arbitrary stimulus or an even response nonlinearity does not guarantee that this average identifies the correct model.

A general fitting approach is to expand a causal filter in smooth basis functions, compute $a(t)=b+\int_0^U k(u)s(t-u)du$, and take a nonnegative rate $\lambda(t)=f(a(t))$. With $f(a)=e^a$, fit the coefficients by [Poisson spike-train likelihood fitting](../../../../../../poisson-spike-train-likelihood-fitting.md):

$$
\boxed{\ell=\sum_i\log\lambda(t_i)-\int_0^{T_{\rm obs}}\lambda(t)dt}.
$$

The first term rewards rate at observed spikes and the second penalizes overprediction elsewhere. Include a filter-size or smoothness penalty, and choose complexity on held-out data. Another option estimates $f$ by stimulus-projection histograms: divide the density of projection values at spikes by their occupancy density, multiplied by the mean firing rate. Avoid interpreting poorly sampled bins as reliable rates. Temporal train/test splits should avoid leakage through the filter-history window.

Given the fitted rate and the same stimulus, generate an [Inhomogeneous Poisson process](../../../../../../inhomogeneous-poisson-process.md). For small bins of width $\Delta t$, spike with probability $1-e^{-\lambda(t)\Delta t}$, choosing the bins sufficiently short that multiple events are negligible. More exactly, advance integrated intensity until it increases by an independent unit-exponential random variable, then place the next event. Repeating this generates different synthetic [spike trains](../../../../../../spike-train.md) with the same fitted stimulus-dependent rate, not copies of the original event times.

Compare held-out log-likelihood, stimulus-conditioned firing-rate predictions, count distributions, interspike-interval distributions and [autocorrelation](../../../../../../autocorrelation.md). With repeated identical stimulus presentations, compare trial-averaged time courses and trial-to-trial count variance, including the [Fano factor](../../../../../../fano-factor.md). A single recorded train does not by itself supply a reliable repeated-trial average or variance; use held-out temporal data, model-based uncertainty and further recordings instead. [Time-rescaled spike-train diagnostics](../../../../../../time-rescaled-spike-train-diagnostics.md) test whether integrated-intensity intervals look independently exponential, rather than comparing raw intervals to an exponential law under a changing rate.

**A successful model reproduces specified statistical features on new data; identical spike times are not the goal.** The basic Poisson model can miss refractoriness, bursting, adaptation, history dependence or stimulus-unexplained trial variability. If needed, add a spike-history filter to the conditional rate, including an absolute dead time, and fit the resulting history-dependent model. A [complex cell](../../../../../../complex-cell.md) may also require multiple filters or quadratic stimulus features: its spike-triggered mean can vanish despite strong tuning. These failures identify model limitations rather than evidence that a random spike generator should match every observed interval.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
