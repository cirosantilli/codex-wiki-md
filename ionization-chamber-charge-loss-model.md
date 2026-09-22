# Ionization-chamber charge-loss model

↑ **Parent:** [Hess cosmic-ray balloon experiment](hess-cosmic-ray-balloon-experiment.md)

An elementary [ionization-chamber charge-loss model](ionization-chamber-charge-loss-model.md) makes the inference explicit. Let a positively charged [electrode](electrode.md) and its [electrometer](electrometer.md) have effective [capacitance](capacitance.md) $C$, [electric potential difference](electric-potential-difference.md) $U$, and enclosed gas volume $\mathcal V$. Assume constant $C$, a short enough interval that collection conditions remain stable, and no multiplication of charge in the gas. If [ionization](ionization.md) produces $q$ [ion pairs](ion-pair.md) per unit volume per unit time and a fraction $\eta$ is collected, then

$$
Q=CU,\qquad s=-\frac{dU}{dt},\qquad Cs=e\eta\mathcal Vq+I_{\rm leak},\qquad q=\frac{Cs-I_{\rm leak}}{e\eta\mathcal V}.
$$

Here $e$ is the [elementary charge](elementary-charge.md) and $I_{\rm leak}$ is the parasitic [electric current](electric-current.md) through imperfect insulation. Each fully collected [ion pair](ion-pair.md) transfers one elementary charge through the measuring circuit; counting its two opposite carriers as two transfers would introduce a factor-of-two error. The relation follows from [charge conservation](charge-conservation.md), rather than from a model of the incoming particle's identity.

For an invented example, take $C=2.00\,\mathrm{pF}$, $\mathcal V=2.00\,\mathrm{L}$, $\eta=1$, a measured fall of $6.00\,\mathrm{V\,h^{-1}}$, and a separately determined leakage-equivalent fall of $0.60\,\mathrm{V\,h^{-1}}$. The leakage-subtracted fall is $5.40\,\mathrm{V\,h^{-1}}$, so

$$
I_{\rm ion}=2.00\times10^{-12}\frac{5.40}{3600}\,\mathrm A=3.00\times10^{-15}\,\mathrm A,\qquad q\approx9.36\,\mathrm{cm^{-3}\,s^{-1}}.
$$

This is about $1.87\times10^4$ collected [ion pairs](ion-pair.md) per second throughout the chamber, not that many [primary cosmic rays](primary-cosmic-ray.md). Unknown collection losses make $\eta<1$ another uncertainty; changes in [capacitance](capacitance.md) would require differentiating $Q=CU$ with both factors variable.

Gas [density](density.md) is a separate issue. Under a fixed radiation field, fixed gas composition and approximately constant energy deposited per unit gas mass, the volume-based [ionization](ionization.md) rate scales as $q\propto\rho$. For a vented [ionization chamber](ionization-chamber.md), the [ideal gas law](ideal-gas-law.md) gives the illustrative correction

$$
q_{\rm ref}=q\frac{\rho_{\rm ref}}{\rho}=q\frac{p_{\rm ref}}p\frac{T}{T_{\rm ref}},
$$

where $T$ is absolute [temperature](temperature-split.md). A pressure-only correction presumes equal [temperature](temperature-split.md). A sealed rigid chamber instead fixes gas [number density](number-density.md) as it rises: its internal [pressure](pressure-split.md) may change with [temperature](temperature-split.md) without losing gas. This does not make its insulation, [electrometer](electrometer.md) calibration or collection efficiency insensitive to [temperature](temperature-split.md). Nor can dividing by gas [density](density.md) correct arbitrary radiation from the vessel walls or changing particle energies. Those are distinct effects, not a universal normalization recipe.

## ↑ Ancestors (9)

1. [Hess cosmic-ray balloon experiment](hess-cosmic-ray-balloon-experiment.md)
2. [Cosmic ray](cosmic-ray.md)
3. [Interstellar medium](interstellar-medium.md)
4. [Milky Way](milky-way.md)
5. [Galaxy](galaxy-split.md)
6. [Astrophysics](astrophysics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Hess cosmic-ray balloon experiment](hess-cosmic-ray-balloon-experiment.md)
- [Ionization-chamber charge-loss model](ionization-chamber-charge-loss-model.md)
