# Einstein solid

↑ **Parent:** [Dulong-Petit law](dulong-petit-law.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Einstein_solid)

The [Einstein model of a solid](einstein-solid.md) represents the vibrations of $N$ [chemical atoms](atom-physics.md) by $3N$ independent one-dimensional [quantum harmonic oscillators](quantum-harmonic-oscillator-split.md), all with the same positive [angular frequency](angular-frequency.md) $\omega$. Equivalently, each [chemical atom](atom-physics.md) has three independent oscillator directions. The common [angular frequency](angular-frequency.md) is a simplifying model assumption, not a claim about every vibration of a real [solid](solid.md). Hold the [volume](volume-thermodynamics.md), $N$ and $\omega$ fixed. Define the characteristic [temperature](temperature-split.md) $\theta_E=\hbar\omega/k_B$ and the dimensionless ratio $x=\theta_E/T$. The vibrational [internal energy](internal-energy-split.md) is

$$
U=3N\hbar\omega\left[\frac12+\frac{1}{e^x-1}\right],\qquad
x=\frac{\hbar\omega}{k_BT}=\frac{\theta_E}{T}.
$$

The first term is the [zero-point energy](zero-point-energy.md) $3N\hbar\omega/2$. It is constant at fixed $\omega$, so it contributes no [heat capacity at constant volume](heat-capacity-at-constant-volume.md). The [temperature](temperature-split.md)-dependent term gives

$$
\frac{C_V}{3Nk_B}=\frac{x^2e^x}{(e^x-1)^2}
=\frac{x^2e^{-x}}{(1-e^{-x})^2}.
$$

This is the vibrational [heat capacity at constant volume](heat-capacity-at-constant-volume.md) of the model, with no expansion or other contributions included. [MIT 3.012, Lecture 22, pages 9–13: Einstein-solid partition function, energy and heat capacity](https://ocw.mit.edu/courses/3-012-fundamentals-of-materials-science-fall-2005/d3fa883afa8df7cf7aa0432fcaadde8f_lec22t.pdf)

For a worked comparison, choose the model parameter $\theta_E=300\,\mathrm K$. The normalized [heat capacity at constant volume](heat-capacity-at-constant-volume.md) depends only on $T/\theta_E$:

| $T/\theta_E$ | [Temperature](temperature-split.md) $T$ in $\mathrm K$ | $C_V/(3Nk_B)$ |
| --- | --- | --- |
| $0.1$ | $30$ | $0.00454$ |
| $0.5$ | $150$ | $0.72406$ |
| $1$ | $300$ | $0.92067$ |
| $2$ | $600$ | $0.97942$ |

At $T=\theta_E$, one [mole](mole-unit.md) of [chemical atoms](atom-physics.md) therefore has vibrational [heat capacity at constant volume](heat-capacity-at-constant-volume.md) $3R(0.92067)\simeq22.965\,\mathrm{J\,mol^{-1}\,K^{-1}}$, using the unrounded model value. Even at twice the characteristic [temperature](temperature-split.md), the model remains about $2.06\%$ below the [Dulong-Petit law](dulong-petit-law.md) limit. These are calculations for the ideal [Einstein solid](einstein-solid.md), not material measurements.

<a id="image-einstein-solid-vibrational-heat-capacity-approaches-the-dulong-petit-law-limit"></a>
![](einstein-solid-heat-capacity.png)

**[Figure 15](#image-einstein-solid-vibrational-heat-capacity-approaches-the-dulong-petit-law-limit). Einstein solid vibrational heat capacity approaches the Dulong-Petit law limit**. The model ratio $C_V/(3Nk_B)$ over $0.02\leq T/\theta_E\leq3$, with the four computed cases marked. The dashed classical line is $1$; quantum freeze-out suppresses the low-[temperature](temperature-split.md) response. All [quantum harmonic oscillators](quantum-harmonic-oscillator-split.md) have the same stipulated [angular frequency](angular-frequency.md).

A short derivation uses the [thermal partition function of a quantum harmonic oscillator](thermal-partition-function-of-a-quantum-harmonic-oscillator.md). The [energy eigenvalues](energy-eigenvalue-split.md) $E_n=\hbar\omega(n+1/2)$ and their [Boltzmann factors](boltzmann-factor.md) form a [geometric series](geometric-series.md), giving the one-oscillator [canonical partition function](canonical-partition-function.md) $z=e^{-x/2}/(1-e^{-x})$. The mean occupation is $1/(e^x-1)$, hence the displayed $U$ after summing over $3N$ independent [quantum harmonic oscillators](quantum-harmonic-oscillator-split.md). Taking its [derivative](derivative.md) with $dx/dT=-x/T$ gives the displayed [heat capacity at constant volume](heat-capacity-at-constant-volume.md). [David Tong, Statistical Physics, Example Sheet 1 (January 2012), problem 5: oscillator energy, the Einstein model and its limits](https://davidtong.org/pdfs/teaching/statistical-physics/omg1.pdf)

The two limits explain the shape. At high [temperature](temperature-split.md), a [Taylor series](taylor-series.md) in small $x$ gives

$$
\frac{C_V}{3Nk_B}=1-\frac{x^2}{12}+O(x^4)\longrightarrow1
\qquad(T\gg\theta_E).
$$

At low [temperature](temperature-split.md), $1-e^{-x}\to1$, so

$$
\frac{C_V}{3Nk_B}\sim x^2e^{-x}\longrightarrow0
\qquad(T\ll\theta_E).
$$

The [zero-point energy](zero-point-energy.md) remains even when the thermal response is tiny: freeze-out means that changing [temperature](temperature-split.md) scarcely changes the occupations, not that the [chemical atoms](atom-physics.md) have zero [energy](energy-split.md). This is the useful lesson of the [Einstein model of a solid](einstein-solid.md): the classical counting rule reappears when many levels are accessible, while discrete excitation spacings explain its failure upon cooling.

The exponential low-[temperature](temperature-split.md) decay is also the model's limitation. Real three-dimensional crystalline [solids](solid.md) have [acoustic phonon branches](acoustic-phonon-branch.md) with arbitrarily small [angular frequencies](angular-frequency.md) in the bulk limit. The [Debye model](debye-model.md) includes these collective [normal modes](normal-mode.md) and predicts a low-[temperature](temperature-split.md) vibrational contribution $C_V\propto T^3$, which the single-frequency [Einstein solid](einstein-solid.md) cannot reproduce. This qualification concerns the vibrational contribution; additional excitations can change a material's total [heat capacity](heat-capacity.md). [David Tong, Statistical Physics, section 3.3: acoustic phonons and the Debye low-temperature law](https://davidtong.org/teaching/statistical-physics/statmechhtml/S3#S3.SS3)

Einstein introduced the quantum treatment of [solid](solid.md) vibrations in his 1907 paper _Die Plancksche Theorie der Strahlung und die Theorie der spezifischen Wärme_. Its historical importance is that quantum excitation energies explained why the classical [Dulong-Petit law](dulong-petit-law.md) could fail; the modern [quantum harmonic oscillator](quantum-harmonic-oscillator-split.md) formulation above includes the [zero-point energy](zero-point-energy.md) explicitly. [A. Einstein, Annalen der Physik 327, 180–190 (1907), original-paper publication metadata](https://onlinelibrary.wiley.com/doi/10.1002/andp.19063270110)

## ↑ Ancestors (9)

1. [Dulong-Petit law](dulong-petit-law.md)
2. [Heat capacity at constant volume](heat-capacity-at-constant-volume.md)
3. [Heat capacity](heat-capacity.md)
4. [Heat](heat-split.md)
5. [Thermodynamics](thermodynamics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Einstein solid](einstein-solid.md)
- [Lamb-Mössbauer factor](lamb-mossbauer-factor.md)
- [Rattling mode](rattling-mode.md)
