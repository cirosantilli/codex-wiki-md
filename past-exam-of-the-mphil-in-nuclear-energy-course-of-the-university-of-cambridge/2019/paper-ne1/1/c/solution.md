<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The idealized external photon estimate is approximately $0.557\ \mathrm{mSv\,h^{-1}}$ at one metre.** First apply [radioactive decay](../../../../../radioactive-decay.md) to the certified [radioactive activity](../../../../../radioactive-activity.md):

$$
A=2.4\times10^9\,2^{-3/5.27}
=1.61751\times10^9\ \mathrm{Bq}.
$$

Treat the source as isotropic and small compared with the observation distance. Neglect photon self-absorption, capsule attenuation and attenuation in air. The metal and capsule stop the primary [beta particles](../../../../../beta-particle.md), so the direct external contribution is taken to be the two [gamma rays](../../../../../gamma-ray.md); secondary [bremsstrahlung](../../../../../bremsstrahlung.md) is neglected. Their total energy per transformation is

$$
E_\gamma=(1.17+1.33)\ \mathrm{MeV}
=4.00544\times10^{-13}\ \mathrm J.
$$

The incident photon energy flow per area at distance $r$ is therefore

$$
\Psi_E(r)=\frac{AE_\gamma}{4\pi r^2}.
$$

Interpret the given $3\ \mathrm{m^{-1}}$ as the [linear energy-absorption coefficient](../../../../../linear-energy-absorption-coefficient.md) $\mu_{\rm en}$, rather than a total photon-removal coefficient. For an absorbing medium of [mass density](../../../../../density.md) $\rho$, a thin volume $S\,dx$ absorbs energy per time $\Psi_E S\mu_{\rm en}\,dx$ and has [mass](../../../../../mass.md) $\rho S\,dx$. Its [absorbed dose](../../../../../absorbed-dose.md) rate is consequently

$$
\dot D=\Psi_E\frac{\mu_{\rm en}}{\rho}.
$$

For the estimate assume a water-like $\rho=10^3\ \mathrm{kg\,m^{-3}}$ and local deposition of the secondary charged-particle energy. At $r=1\ \mathrm m$,

$$
\boxed{
\dot D=
\frac{(1.61751\times10^9)(4.00544\times10^{-13})}{4\pi}
\frac{3}{1000}
=1.54671\times10^{-7}\ \mathrm{Gy\,s^{-1}}
=0.556815\ \mathrm{mGy\,h^{-1}}.
}
$$

For [gamma rays](../../../../../gamma-ray.md), the [radiation weighting factor](../../../../../radiation-weighting-factor.md) is one, giving **$\dot H=0.556815\ \mathrm{mSv\,h^{-1}}$** under these assumptions.[More Details: photon radiation weighting factor one and the distinction between absorbed and equivalent dose](../../../../../absorbed-equivalent-and-effective-dose-by-international-commission-on-radiological-protection.md)

The phrase “equivalent absorbed dose” mixes two quantity names: [absorbed dose](../../../../../absorbed-dose.md) is measured in [gray](../../../../../gray.md), while [equivalent dose](../../../../../equivalent-dose.md) is measured in [sievert](../../../../../sievert.md). Their rates are numerically equal here because the weighting factor is one. The estimate is a physical energy-deposition calculation; the assumed [mass density](../../../../../density.md) is essential, and the stated inverse-length coefficient must not be used as if it already had area-per-mass units.

## ↑ Ancestors (10)

1. [C](../c.md)
2. [1](../../1.md)
3. [Module NE1](../../../paper-ne1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
