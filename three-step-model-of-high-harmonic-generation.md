# Three-step model of high harmonic generation

↑ **Parent:** [High harmonic generation](high-harmonic-generation.md)

For an original classical calculation of the return step, neglect the residual [ion](ion.md)'s [Coulomb force](coulomb-force.md) after release. Take a spatially uniform driving [electric field](electric-field-split.md) $E(t)=E_0\cos\omega t$, an [electron](electron.md) of [electric charge](electric-charge-split.md) $-e$ and [mass](mass.md) $m$, and zero initial position and [velocity](velocity.md) at $t_i$. With $\alpha=\omega t_i$ and $\beta=\omega t$, integrating [Newton's second law](newton-s-second-law.md) gives

$$
v(t)=-\frac{eE_0}{m\omega}(\sin\beta-\sin\alpha),\qquad
x(t)=\frac{eE_0}{m\omega^2}\left[\cos\beta-\cos\alpha+(\beta-\alpha)\sin\alpha\right].
$$

A return requires $\beta>\alpha$ and $x(t)=0$. Define the cycle-averaged free-electron quiver [kinetic energy](kinetic-energy.md)

$$
U_p=\frac{e^2E_0^2}{4m\omega^2},\qquad
K_{\rm return}=2U_p(\sin\beta-\sin\alpha)^2.
$$

Searching the first-return solutions for release phases $0<\alpha<\pi/2$ gives a maximum near $\alpha=0.3134$ and $\beta=4.3990$, with $K_{\rm return}\simeq3.1731U_p$. For a chosen [ionization energy](ionization-energy.md) $I_p$, recombination into the initial state can therefore emit a [photon](photon.md) with [energy](energy-split.md) up to approximately $I_p+3.17U_p$ in this model. This is an upper return-energy scale, not a prediction of the emitted yield. It omits release probabilities, [quantum interference](quantum-interference.md), propagation, [phase matching](phase-matching.md) and depletion of the neutral [gas](gas.md).

The calculation explains why a long driving [wavelength](wavelength.md) can increase the available return [energy](energy-split.md): at fixed $E_0$, $U_p$ grows as $\omega^{-2}$. It does not say that conversion efficiency improves. The [electron](electron.md) must return with a [probability amplitude](probability-amplitude.md) for emission that survives the microscopic dynamics and adds coherently across the [gas](gas.md).

## ↑ Ancestors (7)

1. [High harmonic generation](high-harmonic-generation.md)
2. [Attosecond physics](attosecond-physics.md)
3. [Laser](laser-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
