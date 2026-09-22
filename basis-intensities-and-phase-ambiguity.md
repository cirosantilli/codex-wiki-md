# Basis intensities and phase ambiguity

↑ **Parent:** [X-ray crystallographic structure inference](x-ray-crystallographic-structure-inference.md)

Keep the cubic translations above, but attach an [atomic basis](atomic-basis-of-a-crystal.md) with A at [fractional crystal coordinates](fractional-crystal-coordinate.md) $(0,0,0)$ and B at $(u,0,0)$. Stipulate real, angle-independent relative [scattering amplitudes](scattering-amplitude.md) $f_A=1$ and $f_B=0.6$. Neglect [wave absorption](wave-absorption.md), repeated [crystal scattering](crystal-scattering.md) and thermal motion. This is a point-scatterer model under the [Born approximation](born-approximation.md), not a claim about the scattering strengths of named elements. Its [crystal basis structure factor](crystal-basis-structure-factor.md) is

$$
F_{hkl}(u)=1+0.6e^{2\pi ihu},\qquad
J_{hkl}(u)=|F_{hkl}(u)|^2=1.36+1.2\cos(2\pi hu).
$$

Here $J$ is a dimensionless squared motif amplitude. Comparing it with measured integrated [wave intensities](intensity-physics.md) requires the experimental geometry and detector response as well. The algebra follows directly by multiplying $F$ by its [complex conjugate](complex-conjugate.md); the cross term records [wave interference](interference-wave-propagation.md) between the two sites.

With $u=1/2$, reflections with even $h$ have $J=2.56$, whereas odd $h$ gives $J=0.16$, a ratio of $16:1$. With $u=1/4$, the first four $(h00)$ values instead are $1.36,0.16,1.36,2.56$. Their geometrically possible positions are unchanged, although their strengths change. For equal stipulated amplitudes $f_A=f_B=1$ and $u=1/2$, the odd-$h$ amplitude vanishes exactly: an example of a [systematic absence](systematic-absence.md). Different motif weights can thus expose a repeat that equal weights conceal.

<a id="image-x-ray-basis-intensities-and-phase-ambiguity"></a>
![](x-ray-basis-intensities-and-phase-ambiguity.png)

**[Figure 3](#image-x-ray-basis-intensities-and-phase-ambiguity). The motif changes intensities, while inversion can preserve them**. Original point-scatterer simulations with $f_A=1$ and $f_B=0.6$. Top: the same $(h00)$ reflection labels have different squared motif amplitudes for $u=1/2$ and $u=1/4$. Bottom left: moving B from $u=1/4$ to $u=3/4$ inverts its offset modulo a translation. Bottom right: the two $(100)$ [crystal basis structure factors](crystal-basis-structure-factor.md) are [complex conjugates](complex-conjugate.md), $1\pm0.6i$, with the same squared modulus $1.36$. No detector profiles or real-material measurements are plotted.

The same formula also proves an ambiguity: $u=1/4$ and $u=3/4$ give identical $J_{hkl}$ for every [integer](integer-split.md) $h,k,l$, because $\cos(2\pi h(1-u))=\cos(2\pi hu)$. Yet $F_{100}$ changes from $1+0.6i$ to $1-0.6i$, reversing its [wave phase](phase-waves.md). This particular ambiguity is inversion of the motif; it does not prove that these two simple motifs are distinct chemical substances. The conclusion is conditional on the stipulated real [scattering amplitudes](scattering-amplitude.md).

## ↑ Ancestors (6)

1. [X-ray crystallographic structure inference](x-ray-crystallographic-structure-inference.md)
2. [Crystallography](crystallography.md)
3. [Crystal structure](crystal-structure.md)
4. [Physical chemistry](physical-chemistry-split.md)
5. [Chemistry](chemistry-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [X-ray crystallographic structure inference](x-ray-crystallographic-structure-inference.md)
