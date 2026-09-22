# Chirped pulse amplification energy budget

↑ **Parent:** [Chirped pulse amplification](chirped-pulse-amplification.md)

Let $P(t)$ be the pulse's [power](power.md) integrated over its transverse section, and $U$ its [energy](energy-split.md). Its [peak power](peak-power.md) is $\max_t P(t)$. For a chosen Gaussian power envelope with [full width at half maximum](full-width-at-half-maximum.md) $\tau$,

$$
P(t)=P_{\rm pk}e^{-4\ln2\,t^2/\tau^2},\qquad
U=P_{\rm pk}\tau\sqrt{\frac{\pi}{4\ln2}},\qquad
P_{\rm pk}=\sqrt{\frac{4\ln2}{\pi}}\frac{U}{\tau}.
$$

The numerical shape factor is approximately $0.9394$. It matters when comparing quoted [peak powers](peak-power.md); the estimate $U/\tau$ assumes a shape and a width convention.

If an otherwise unchanged pulse is stretched by a factor $S$ without loss, its [energy](energy-split.md) stays fixed and its [peak power](peak-power.md) falls by $S$. For energy gain $G$ and compressor energy transmission $\eta$, ideal restoration of the original shape gives

$$
U_{\rm out}=\eta G U_{\rm in},\qquad
\frac{P_{{\rm pk},\,\rm out}}{P_{{\rm pk},\,\rm amplified}}=\eta S.
$$

These relations require a specified shape and preserved spectrum; they do not model amplifier saturation. For the diagram's chosen $1\,\mathrm{nJ}$, $30\,\mathrm{fs}$ seed, $S=9.2959$, $G=1000$ and $\eta=0.8$, the successive [peak powers](peak-power.md) are $31.31\,\mathrm{kW}$, $3.369\,\mathrm{kW}$, $3.369\,\mathrm{MW}$ and $25.05\,\mathrm{MW}$. The last pulse contains $0.8\,\mathrm{\mu J}$: the compressor increases [peak power](peak-power.md) while losing some [energy](energy-split.md).

[Fluence](fluence.md) is time-integrated [light intensity](light-intensity.md), $F(x,y)=\int I(x,y,t)\,dt$, measured in $\mathrm{J\,m^{-2}}$. For a uniform beam of area $\mathcal A$, $F=U/\mathcal A$ and $I_{\rm pk}=P_{\rm pk}/\mathcal A$. At fixed transverse profile, lossless temporal stretching lowers peak [light intensity](light-intensity.md) but leaves [fluence](fluence.md) unchanged. Absorbed [energy](energy-split.md), heat removal, beam size, coatings and pulse duration still constrain optical components. For nonoverlapping identical pulses at repetition [frequency](frequency.md) $f_r$, the average [power](power.md) is $U f_r$; it is a different quantity from [peak power](peak-power.md).

## ↑ Ancestors (6)

1. [Chirped pulse amplification](chirped-pulse-amplification.md)
2. [Laser](laser-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
