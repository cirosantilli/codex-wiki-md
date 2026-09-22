# Shot noise spectral convention

↑ **Parent:** [Shot noise](shot-noise.md)

Write an ideal point-transfer model using the [Dirac delta function](dirac-delta-function.md):

$$
i(t)=q\sum_k\delta(t-t_k),\qquad \delta i(t)=i(t)-I.
$$

For this arrival stream with [independent increments](independent-increments.md), distinct arrivals contribute the product of the means, which cancels when centering. The same-arrival term leaves the [autocovariance](autocovariance.md)

$$
\mathbb E[\delta i(t)\delta i(t+s)]=q^2\lambda\delta(s)=qI\delta(s).
$$

Its [Fourier transform](fourier-transform-split.md) gives the two-sided [power spectral density](power-spectral-density.md), while folding negative [frequencies](frequency.md) onto positive ones gives the one-sided convention:

$$
S_I^{(2)}(f)=qI\quad(-\infty<f<\infty),\qquad
S_I^{(1)}(f)=2qI\quad(f>0),\qquad
[S_I]=\mathrm{A^2/Hz}.
$$

These spectra describe $\delta i$, excluding the spectral line from the mean [direct current](direct-current.md). The [amplitude spectral density](amplitude-spectral-density.md) is $\sqrt{2qI}$ in $\mathrm A/\sqrt{\mathrm{Hz}}$; it is not a [root mean square](root-mean-square.md) [electric current](electric-current.md) until a measurement [signal bandwidth](signal-bandwidth.md) is specified. Approximate [white noise](white-noise.md) requires [frequencies](frequency.md) low enough that the single-transfer pulse shape and any correlations can be neglected. Neither the ideal impulses nor a flat spectrum extending to infinity describe a real detector at every timescale.

All spectra above are per [hertz](hertz.md), with $f$ in cycles per second. One possible [angular frequency](angular-frequency.md) convention defines a density $\mathcal S_I^{(2)}(\omega)$ integrated using $d\omega$ alone. Since $\omega=2\pi f$, it has

$$
\mathcal S_I^{(2)}(\omega)=\frac{S_I^{(2)}(\omega/(2\pi))}{2\pi},\qquad
\operatorname{Var}(i_{\rm filtered})=\int_{-\infty}^{\infty}\mathcal S_I^{(2)}(\omega)|H(\omega/(2\pi))|^2\,d\omega.
$$

Another common convention keeps the numerical density $qI$ but integrates it with $d\omega/(2\pi)$. State the integration measure as well as whether a spectrum is one-sided: a change of variable and a folding of signs are separate operations.

## ↑ Ancestors (6)

1. [Shot noise](shot-noise.md)
2. [Noise (signal processing)](noise-signal-processing.md)
3. [Signal](signal.md)
4. [Signal processing](signal-processing.md)
5. [Electrical engineering](electrical-engineering-split.md)
6. [Codex Wiki](split.md)
