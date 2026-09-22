# Narrowband frequency modulation

↑ **Parent:** [Frequency modulation](frequency-modulation.md)

When the [FM modulation index](fm-modulation-index.md) satisfies $|\beta|\ll1$, a [Taylor expansion](taylor-expansion.md) gives a useful first-order approximation. With $\omega_c=2\pi f_c$ and $\omega_m=2\pi f_m$,

$$
\frac{s(t)}A
=\cos(\omega_ct)-\beta\sin(\omega_mt)\sin(\omega_ct)+O(\beta^2)
=\cos(\omega_ct)+\frac\beta2\cos((\omega_c+\omega_m)t)-\frac\beta2\cos((\omega_c-\omega_m)t)+O(\beta^2).
$$

The [product-to-sum formula](product-to-sum-formula.md) for [sines](sine.md) exposes a carrier and one pair of sidebands, with opposite signs for this [wave phase](phase-waves.md) convention. Higher sidebands are neglected, not identically absent. For $\beta=0.1$, the predicted normalized first-sideband magnitude $0.05$ is close to the original exact evaluation $J_1(0.1)\approx0.0499375$. The neglected waveform term is bounded in [absolute value](absolute-value.md) by $\beta^2/2=0.005$, using the second-[derivative](derivative.md) bound for the [cosine](cosine.md). Small [frequency deviation](frequency-deviation.md) relative to $f_c$ alone does not justify this approximation: it is $\Delta f/f_m$ that must be small.

## ↑ Ancestors (3)

1. [Frequency modulation](frequency-modulation.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)
