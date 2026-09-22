# Filtered shot noise

↑ **Parent:** [Shot noise](shot-noise.md)

Let $K(f)$ be the complete current-to-voltage [frequency response](frequency-response.md) from detector input to readout, in $\mathrm{V/A}$. For a real stable [linear time-invariant system](linear-time-invariant-system.md), the shot contribution to the output voltage [variance](variance-split.md) is

$$
\sigma_{v,\rm shot}^2=\int_0^\infty 2qI|K(f)|^2\,df
=\int_{-\infty}^{\infty}qI|K(f)|^2\,df.
$$

If $K(f)=R_FG H(f)$ with feedback [electrical resistance](electrical-resistance.md) $R_F$, a reference [voltage gain](voltage-gain.md) $G$, and dimensionless normalized [frequency response](frequency-response.md) $H$, then

$$
B_{\rm n}=\int_0^\infty |H(f)|^2\,df,\qquad
\sigma_{v,\rm shot}^2=2qI R_F^2G^2B_{\rm n}.
$$

This is the [effective noise bandwidth](effective-noise-bandwidth.md) for unit reference magnitude. The [transimpedance amplifier](transimpedance-amplifier.md) factor $R_F$ converts [electric current](electric-current.md) to voltage; $G$ multiplies voltage. Neither is an additional [noise](noise-signal-processing.md) source merely because it amplifies an existing fluctuation. In contrast, a real [amplifier](amplifier.md) adds input voltage [noise](noise-signal-processing.md) and input current [noise](noise-signal-processing.md), and its feedback [resistor](resistor.md) contributes [thermal electrical noise](thermal-electrical-noise.md). Those terms need their own transfers to the output. In particular, input voltage [noise](noise-signal-processing.md) generally has a different transfer from an injected detector [electric current](electric-current.md). Simply multiplying every input specification by $R_FG$ is incorrect.

For a unit-gain exponential [low-pass filter](low-pass-filter.md), with [time constant](time-constant.md) $\tau>0$,

$$
h(t)=\frac1\tau e^{-t/\tau}\quad(t\geq0),\qquad
H(f)=\frac1{1+2\pi\mathrm i f\tau},\qquad
B_{\rm n}=\frac1{4\tau}=\frac\pi2 f_c,\qquad f_c=\frac1{2\pi\tau}.
$$

The [cutoff frequency](cutoff-frequency.md) $f_c$ is not $B_{\rm n}$. An independent time-domain derivation sums independent event contributions to give

$$
\operatorname{Var}(i_{\rm filtered})
=\lambda q^2\int_0^\infty h(t)^2\,dt
=\frac{qI}{2\tau}.
$$

The same reasoning for a rectangular averaging gate has $h=1/T$ on $[0,T]$ and zero elsewhere, hence [effective noise bandwidth](effective-noise-bandwidth.md) $1/(2T)$ and [variance](variance-split.md) $qI/T$, agreeing with the [shot noise counting model](shot-noise-counting-model.md). Equal numerical durations $T=\tau$ do not make these two different [linear filters](linear-filter.md) equivalent.

## ↑ Ancestors (6)

1. [Shot noise](shot-noise.md)
2. [Noise (signal processing)](noise-signal-processing.md)
3. [Signal](signal.md)
4. [Signal processing](signal-processing.md)
5. [Electrical engineering](electrical-engineering-split.md)
6. [Codex Wiki](split.md)
