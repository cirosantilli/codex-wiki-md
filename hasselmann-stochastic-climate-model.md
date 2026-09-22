# Hasselmann stochastic climate model

↑ **Parent:** [Climate model](climate-model.md)

The [Hasselmann stochastic climate model](hasselmann-stochastic-climate-model.md) represents slowly responding climate variables driven by fast weather fluctuations as well as external forcing. [Klaus Hasselmann](klaus-hasselmann.md)'s 1976 paper separates fast and slow variables, retains fluctuations lost by simple averaging, and explains why stabilizing [climate feedbacks](climate-feedback.md) are needed to prevent indefinitely growing variability. Its general framework is broader than a single-temperature equation.[Hasselmann, Stochastic climate models. Part I. Theory, 1976, Section 2; Section 7, summary points 1–4](stochastic-climate-models-part-i-theory-by-klaus-hasselmann.md)

Consider an original scalar specialization for a spatially averaged [temperature](temperature-split.md) anomaly $T$, with an effective [ocean mixed layer](ocean-mixed-layer.md) [heat capacity](heat-capacity.md) per unit [area](surface-area.md) $C$:

$$
C\frac{dT}{dt}=F(t)-\lambda T+\eta(t),\qquad C>0,\quad\lambda>0.
$$

Here $F$ is imposed [radiative forcing](radiative-forcing.md), $\lambda$ is the net restoring coefficient after the chosen [climate feedbacks](climate-feedback.md), and $\eta$ represents random net [heat flux](heat-flux-density.md) from unresolved weather. The anomaly [energy](energy-split.md) per unit [area](surface-area.md) is $CT$, so its tendency equals the net input. The weather term represents exchange with omitted degrees of freedom; it does not assert that an isolated ocean creates [energy](energy-split.md). $F$ and $\eta$ have units $\mathrm{W\,m^{-2}}$, and $\lambda$ has units $\mathrm{W\,m^{-2}\,K^{-1}}$.

First set $\eta=0$, start from $T(0)=0$, and switch to constant $F_0>0$. The [integrating factor](integrating-factor.md) $e^{\lambda t/C}$ gives

$$
T(t)=\frac{F_0}{\lambda}(1-e^{-t/\tau}),\qquad \tau=\frac C\lambda.
$$

For $C=2.0\times10^8\,\mathrm{J\,m^{-2}\,K^{-1}}$, $\lambda=2.0\,\mathrm{W\,m^{-2}\,K^{-1}}$ and $F_0=4.0\,\mathrm{W\,m^{-2}}$, the [relaxation time](relaxation-time.md) is $10^8\,\mathrm s$, about $3.17$ years using 365.25 days per year. At $t=\tau$, $T=2(1-e^{-1})\,\mathrm K\simeq1.264\,\mathrm K$, with eventual warming $2\,\mathrm K$. Doubling $C$ doubles the response time but leaves this equilibrium unchanged. This separates thermal inertia from [climate sensitivity](climate-sensitivity.md).

Now set $F=0$ and idealize the weather forcing as [Gaussian white noise](gaussian-white-noise.md) with

$$
\mathbb E\eta(t)=0,\qquad
\mathbb E[\eta(t)\eta(t')]=2D\delta(t-t'),\qquad D>0.
$$

The [Dirac delta function](dirac-delta-function.md) has inverse-time units, so $D$ has units $(\mathrm{W\,m^{-2}})^2\mathrm s$. The rigorous [stochastic differential equation](stochastic-differential-equation.md) is

$$
dT=-\frac{\lambda}{C}T\,dt+\frac{\sqrt{2D}}{C}\,dW_t,
$$

where $W_t$ is [Brownian motion](brownian-motion-split.md). This is an [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md). In stationary initialization its [variance](variance-split.md) and [autocovariance function](autocovariance.md) are

$$
v_\infty=\frac{D}{C\lambda},\qquad R_T(u)=v_\infty e^{-|u|/\tau}.
$$

Define the two-sided angular-frequency [power spectral density](power-spectral-density.md) by $R_T(u)=(2\pi)^{-1}\int_{-\infty}^{\infty}S_T(\omega)e^{i\omega u}\,d\omega$. The [Fourier transform](fourier-transform-split.md) of the exponential [autocovariance function](autocovariance.md), or the squared response to a sinusoidal input, gives

$$
S_T(\omega)=\frac{2D}{\lambda^2+C^2\omega^2},\qquad
\frac{S_T(\omega)}{S_T(0)}=\frac{1}{1+(\omega\tau)^2}.
$$

Thus fast fluctuations are suppressed; the climate output is red over the frequency range above the corner $|\omega|=1/\tau$, with a low-frequency plateau. This is a [colored noise](colored-noise.md) spectrum without a periodic driver. The corner is $f_c=1/(2\pi\tau)$ in cycles per second, not $1/\tau$. The continuous white input is only an approximation on times longer than weather's [correlation time](correlation-time.md).

<a id="image-thermal-inertia-delays-forced-warming-and-filters-random-weather-forcing"></a>
![](stochastic-climate-response-and-spectrum.png)

**[Figure 4](#image-thermal-inertia-delays-forced-warming-and-filters-random-weather-forcing). Thermal inertia delays forced warming and filters random weather forcing**. Original one-box model: the step-forced mean approaches two kelvins, with one-standard-deviation spread from a fixed initial temperature and chosen white-noise strength. The right panel shows the analytic normalized two-sided spectrum, not measured climate data.

For the same $C,\lambda$ and $D=10^8\,(\mathrm{W\,m^{-2}})^2\mathrm s$, $v_\infty=0.25\,\mathrm{K^2}$ and the stationary [standard deviation](standard-deviation.md) is $0.50\,\mathrm K$. From fixed $T(0)=0$, the [variance](variance-split.md) grows as $v_\infty(1-e^{-2t/\tau})$, even when the forced [expected value](expected-value-split.md) is predictable. Integrating $S_T/(2\pi)$ over all angular [frequencies](frequency.md) returns $D/(C\lambda)$, checking the normalization independently. If $\lambda=0$ the unforced [variance](variance-split.md) instead grows as $2Dt/C^2$; if $\lambda<0$, deviations amplify. Neither case has the stationary spectrum above.

A red spectrum alone cannot establish [attribution of recent climate change](attribution-of-recent-climate-change.md): internal variability, changing forcing and measurement effects must be distinguished. This scalar model supplies a calculable baseline for variability and persistence, not a universal spectrum for all climate timescales or a full attribution analysis.

## ↑ Ancestors (6)

1. [Climate model](climate-model.md)
2. [Climate change](climate-change.md)
3. [Geophysics](geophysics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Climate change](climate-change.md)
- [Climate model](climate-model.md)
- [Hasselmann stochastic climate model](hasselmann-stochastic-climate-model.md)
