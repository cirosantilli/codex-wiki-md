# Thermal noise spectral convention

↑ **Parent:** [Thermal electrical noise](thermal-electrical-noise.md)

Model an ideal [resistor](resistor.md) of constant [electrical resistance](electrical-resistance.md) $R>0$ at uniform absolute [temperature](temperature-split.md) $T$ by its [Thévenin equivalent](thevenin-equivalent.md): a zero-mean random [voltage source](voltage-source.md) in series with a noiseless $R$. In the classical range its one-sided, [open-circuit voltage](open-circuit-voltage.md) [power spectral density](power-spectral-density.md), per [hertz](hertz.md), is

$$
S_v^{(1)}(f)=4k_{\rm B}TR\quad(f\geq0),\qquad [S_v^{(1)}]=\mathrm{V^2/Hz},
$$

where $k_{\rm B}$ is the [Boltzmann constant](boltzmann-constant.md). Thus a positive-[frequency](frequency.md) interval of width $df$ contributes $4k_{\rm B}TR\,df$ to the mean square voltage. This is approximately [white noise](white-noise.md) only where the [electrical resistance](electrical-resistance.md) is effectively constant and $hf\ll k_{\rm B}T$, with $h$ the [Planck constant](planck-constant.md). The ideal constant spectrum cannot describe arbitrarily high [frequencies](frequency.md).[Nyquist (1928), p. 113, equations (4)–(8): classical spectrum and high-frequency thermal correction](https://123.physics.ucdavis.edu/johnson_files/nyquist_1928.pdf)

For a real voltage, an equivalent two-sided [power spectral density](power-spectral-density.md) is $S_v^{(2)}(f)=2k_{\rm B}TR$ over signed [frequencies](frequency.md). With a real [linear time-invariant system](linear-time-invariant-system.md) of [frequency response](frequency-response.md) $H(f)$, the same output mean square is

$$
\langle v_o^2\rangle=\int_0^\infty S_v^{(1)}(f)|H(f)|^2\,df
=\int_{-\infty}^{\infty}S_v^{(2)}(f)|H(f)|^2\,df.
$$

Angle brackets denote an [expected value](expected-value-split.md); for this zero-mean [noise](noise-signal-processing.md) the mean square is its [variance](variance-split.md). Do not integrate $4k_{\rm B}TR$ over both signs of [frequency](frequency.md): that counts the same fluctuations twice. All integrals here use [frequency](frequency.md) $f$ in [hertz](hertz.md), not [angular frequency](angular-frequency.md) $\omega=2\pi f$. The [amplitude spectral density](amplitude-spectral-density.md) is $\sqrt{4k_{\rm B}TR}$ in $\mathrm V/\sqrt{\mathrm{Hz}}$, whereas the [root mean square](root-mean-square.md) voltage requires a specified measurement [signal bandwidth](signal-bandwidth.md).

## ↑ Ancestors (6)

1. [Thermal electrical noise](thermal-electrical-noise.md)
2. [Noise (signal processing)](noise-signal-processing.md)
3. [Signal](signal.md)
4. [Signal processing](signal-processing.md)
5. [Electrical engineering](electrical-engineering-split.md)
6. [Codex Wiki](split.md)
