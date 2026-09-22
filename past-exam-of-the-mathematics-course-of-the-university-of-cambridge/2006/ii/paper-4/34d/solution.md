<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

Statistical [temperature](../../../../../temperature.md) is defined by $1/T=(\partial S/\partial U)_{V,N}$, with [entropy](../../../../../entropy.md) $S=k_B\log\Omega$. Maximizing total [entropy](../../../../../entropy.md) when two systems exchange energy makes their derivatives equal, explaining why equal [temperature](../../../../../temperature.md) characterizes [thermal equilibrium](../../../../../thermal-equilibrium.md) and why a thermometer can measure another system.

For a dilute monatomic [ideal gas](../../../../../ideal-gas.md), Gaussian integration of momenta gives the classical [partition function](../../../../../canonical-partition-function.md) $Z_N=V^N/(N!\lambda_T^{3N})$, with $\lambda_T=h/\sqrt{2\pi mk_BT}$. Differentiating its logarithm gives

$$
\boxed{PV=Nk_BT,\qquad U=\frac32Nk_BT}.
$$

At fixed volume, gas pressure is proportional to absolute [temperature](../../../../../temperature.md); at fixed pressure its volume is proportional to [temperature](../../../../../temperature.md). A low-density gas thermometer therefore supplies an absolute calibration independent of the gas species in the ideal limit. A liquid-in-glass column responds to the difference between liquid and glass thermal expansion, which need not be exactly linear. Calibration against gas temperatures and correction for expansion nonlinearities improve a simple two-point column scale; an ideal-gas law is not a law of the liquid itself.

For [blackbody radiation](../../../../../black-body-radiation.md), the electromagnetic mode density is $8\pi\nu^2/c^3$ per volume and frequency interval, including two polarizations. For one [photon](../../../../../photon.md) mode, summing its occupation numbers gives $Z_\nu=\sum_{j\ge0}e^{-j h\nu/(k_BT)}=(1-e^{-h\nu/(k_BT)})^{-1}$. Differentiation of $\log Z_\nu$ gives mean energy $h\nu/(e^{h\nu/k_BT}-1)$, so the [Planck distribution](../../../../../planck-photon-distribution.md) follows. Converting to wavelength gives spectral radiance

$$
B_\lambda(T)=\frac{2hc^2}{\lambda^5}\frac1{e^{hc/(\lambda k_BT)}-1}.
$$

At its maximum, $z=hc/(\lambda k_BT)$ satisfies $5(1-e^{-z})=z$, whose positive root is $4.9651\ldots$. Thus the [Wien displacement law](../../../../../wien-s-displacement-law.md) is

$$
\boxed{\lambda_{\max}T=\frac{hc}{4.9651\ldots k_B}\simeq2.898\times10^{-3}\ \mathrm{m\,K}}.
$$

This calibrates a wavelength-based radiation thermometer and avoids identifying a subjective colour with a universal [temperature](../../../../../temperature.md). A peak per frequency interval has a different numerical location, so the spectral convention must be stated. Real objects require emissivity and atmospheric corrections; fitting a measured spectrum is more informative than choosing its visually brightest colour. Integrating the [Planck distribution](../../../../../planck-photon-distribution.md) also gives energy density proportional to $T^4$ and radiative flux proportional to $T^4$, supplying the complementary [Stefan–Boltzmann law](../../../../../stefan-boltzmann-law.md) calibration.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
