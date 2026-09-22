<h1 id="forster-distance">Förster distance</h1>

↑ **Parent:** [FRET efficiency](fret-efficiency.md)

The [Förster distance](forster-distance.md) is the separation giving [FRET efficiency](fret-efficiency.md) $E=1/2$ for the specified pair and conditions. It is a property of the optical pair and its environment, rather than a universal length. In the usual pair model,

$$
R_0^6\propto \kappa^2 Q_D J n^{-4},
$$

where $\kappa^2$ is the [FRET dipole orientation factor](fret-dipole-orientation-factor.md), $Q_D$ the [FRET donor quantum yield](fret-donor-quantum-yield.md), $J$ the [FRET spectral overlap](fret-spectral-overlap.md) [integral](integral-split.md), and $n$ the medium's [refractive index](refractive-index.md). The omitted proportionality constant depends on the unit convention for $J$.[§3.1, equations 16–18: factors controlling Förster distance](advanced-fluorescence-microscopy-techniques-frap-flip-flap-fret-and-flim-by-hellen-c-ishikawa-ankerhold-and-others.md)

If [FRET efficiency](fret-efficiency.md) is known and those assumptions hold, inversion gives

$$
r=R_0\left(E^{-1}-1\right)^{1/6},\qquad \frac{d\log r}{dE}=-\frac{1}{6E(1-E)}.
$$

The [derivative](derivative.md) explains why errors become troublesome near $E=0$ or $E=1$. An illustrative pair with $R_0=4$ nanometres and another with $R_0=6$ nanometres both give $E=1/2$ at their different [Förster distances](forster-distance.md): knowing [FRET efficiency](fret-efficiency.md) alone does not determine $r$.

A heterogeneous population adds another ambiguity. In a synthetic example with equal weights per [FRET donor](fret-donor.md) excitation, efficiencies $0.1$ and $0.9$ average to $0.5$, but their separations are $9^{1/6}R_0$ and $9^{-1/6}R_0$. Their average separation is approximately $1.068R_0$, whereas inverting the average [FRET efficiency](fret-efficiency.md) gives $R_0$. A measured emission [ratio](ratio.md) has additional detection weights; it need not equal even this excitation-weighted average. The transferable lesson is that an average readout does not uniquely specify a distribution of molecular separations.

**Table of contents**

- [FRET spectral overlap](fret-spectral-overlap.md)
- [FRET dipole orientation factor](fret-dipole-orientation-factor.md)
- [FRET donor quantum yield](fret-donor-quantum-yield.md)

## ↑ Ancestors (5)

1. [FRET efficiency](fret-efficiency.md)
2. [Förster resonance energy transfer](forster-resonance-energy-transfer.md)
3. [Biophysical measurement](biophysical-measurement.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Förster distance](forster-distance.md)
- [Förster resonance energy transfer](forster-resonance-energy-transfer.md)
- [FRET donor quantum yield](fret-donor-quantum-yield.md)
- [Solution](past-exam-of-the-biochemistry-course-of-the-university-of-cambridge/2025/paper-1/section-i/2/solution.md)
