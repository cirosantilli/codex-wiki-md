# Frank-Tamm formula

↑ **Parent:** [Cherenkov radiation](cherenkov-radiation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frank–Tamm_formula)

For constant particle [speed](speed.md) and [electric charge](electric-charge-split.md) $q=ze$, in a transparent, linear, nonmagnetic medium with [isotropy](isotropy.md), the [Frank-Tamm formula](frank-tamm-formula.md) gives the produced [photon](photon.md) density:

$$
\frac{d^2N}{dx\,d\lambda}
=\frac{2\pi\alpha z^2}{\lambda^2}
\left(1-\frac{1}{\beta^2n^2(\lambda)}\right),
\qquad \beta n(\lambda)>1.
$$

Set it to zero below threshold. Here $e$ is the positive [elementary charge](elementary-charge.md), $x$ is track length, $\lambda=2\pi c/\omega$ is [vacuum](vacuum.md) [wavelength](wavelength.md), and $\alpha$ is the [fine-structure constant](fine-structure-constant.md). With [SI](international-system-of-units.md) lengths in metres, the density has units $\mathrm{m}^{-2}$; multiplying by $dx\,d\lambda$ gives a dimensionless expected count. The explicit [SI](international-system-of-units.md) convention is

$$
\alpha=\frac{e^2}{4\pi\epsilon_0\hbar c},\qquad
\frac{d^2N}{dx\,d\omega}=\frac{\alpha z^2}{c}
\left(1-\frac{1}{\beta^2n^2(\omega)}\right).
$$

These conventions agree.[§34.7.1, equations (34.43)–(34.44), p. 34: photon yields](passage-of-particles-through-matter-by-donald-e-groom-and-spencer-klein.md)

To check the convention, start from $E=\hbar\omega=hc/\lambda$ and $d^2N/(dx\,dE)=\alpha z^2\sin^2\theta/(\hbar c)$. Changing variables uses the positive density Jacobian $|dE/d\lambda|=hc/\lambda^2$; since $h/\hbar=2\pi$, the coefficient becomes $2\pi\alpha z^2$. No factor of the material [refractive index](refractive-index.md) belongs in this Jacobian: $\lambda$ is not the in-medium [wavelength](wavelength.md). Multiplication by $\hbar\omega$ gives the corresponding energy loss density in this [SI](international-system-of-units.md) nonmagnetic convention:

$$
\frac{d^2W}{dx\,d\omega}
=\frac{z^2e^2\omega}{4\pi\epsilon_0c^2}
\left(1-\frac{1}{\beta^2n^2(\omega)}\right).
$$

For an original constant-index example, stipulate $n=1.50$, $\beta=0.90$, $z=1$ and $\alpha=1/137.036$. Integration from $400$ to $700\,\mathrm{nm}$ gives

$$
\frac NL=2\pi\alpha\left(1-\frac1{1.35^2}\right)
\left(\frac1{400\times10^{-9}\,\mathrm m}-\frac1{700\times10^{-9}\,\mathrm m}\right)
\simeq2.217\times10^4\,\mathrm m^{-1}.
$$

Thus a stipulated $1\,\mathrm{cm}$ track produces about $222$ [photons](photon.md) in this band in the ideal model. This is an emitted count before [absorption](absorption-electromagnetic-radiation.md), collection losses and detector response, not a brightness measurement or a measured water yield.

**Table of contents**

- [Finite-band Cherenkov yield model](finite-band-cherenkov-yield-model.md)

## ↑ Ancestors (6)

1. [Cherenkov radiation](cherenkov-radiation.md)
2. [Electromagnetic wave](electromagnetic-wave-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Cherenkov cone angle](cherenkov-cone-angle.md)
- [Cherenkov radiation](cherenkov-radiation.md)
- [Finite-band Cherenkov yield model](finite-band-cherenkov-yield-model.md)
- [Frank-Tamm formula](frank-tamm-formula.md)
