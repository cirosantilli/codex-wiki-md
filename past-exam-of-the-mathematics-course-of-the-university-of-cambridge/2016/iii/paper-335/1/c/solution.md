<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At each point the [Gaussian process](../../../../../../gaussian-process.md) has a standard normal [marginal distribution](../../../../../../marginal-distribution.md). Its [characteristic function](../../../../../../characteristic-function.md) gives the coherent screen field

$$
m=\langle e^{i\beta W(z)}\rangle=e^{-\beta^2/2}.
$$

It is constant in $z$, so its [Fourier transform](../../../../../../fourier-transform.md) is $m\delta(\nu)$. Applying the [Fresnel propagator](../../../../../../fresnel-propagator.md) to this zero-transverse-[wavenumber](../../../../../../wavenumber.md) component gives **the ensemble-averaged reduced spectrum**

$$
\boxed{\langle\widehat E(x,\nu)\rangle
=e^{-i\nu^2x/(2k)}e^{-\beta^2/2}\delta(\nu)
=e^{-\beta^2/2}\delta(\nu).}
$$

Thus the reduced mean is independent of $x$. The physical mean $\langle\psi(x,z)\rangle=e^{ikx}e^{-\beta^2/2}$ still has its carrier phase. The [coherent attenuation by a Gaussian phase screen](../../../../../../coherent-attenuation-by-a-gaussian-phase-screen.md) takes place at the screen, with no further coherent attenuation in homogeneous space.

The full [spectral acoustic flux](../../../../../../spectral-acoustic-flux.md) depends on the second moment, not the square of this mean. For a [stationary process](../../../../../../stationary-process.md), the generalized cross-spectral correlation is

$$
\langle\widehat E(x,\nu)\overline{\widehat E(x,\nu')}\rangle
=\delta(\nu-\nu')S_E(\nu).
$$

Indeed its propagation factors cancel on $\nu=\nu'$. This explains why the ensemble-averaged [spectral acoustic flux](../../../../../../spectral-acoustic-flux.md) in (b) is also independent of $x$, even for nonzero transverse [wavenumbers](../../../../../../wavenumber.md) whose individual complex amplitudes change phase. The coherent atom has weight $|m|^2=e^{-\beta^2}$; the full [stationary phase-screen power spectrum](../../../../../../stationary-phase-screen-power-spectrum.md) also contains fluctuations. Under the decay assumptions in (b), their integrated weight is $1-e^{-\beta^2}$. One must use these weights in a [spectral measure of a stationary random field](../../../../../../spectral-measure-of-a-stationary-random-field.md), rather than square a [Dirac delta distribution](../../../../../../dirac-delta-function.md). A phase-only screen preserves the leading-order total [acoustic energy flux](../../../../../../acoustic-energy-flux.md), although it reduces its coherent part.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
