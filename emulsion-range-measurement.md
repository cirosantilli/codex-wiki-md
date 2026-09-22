# Emulsion range measurement

↑ **Parent:** [Nuclear emulsion track experiment](nuclear-emulsion-track-experiment.md)

An [emulsion range measurement](emulsion-range-measurement.md) follows a stopping [charged particle](charged-particle.md) through the coating to estimate its complete [particle range](particle-range.md). A projected length on one image can underestimate the distance travelled. In an original geometry example, a straight segment with projected length $L_{xy}=240\,\mathrm{\mu m}$ and corrected depth change $\Delta z=180\,\mathrm{\mu m}$ has length

$$
L=\sqrt{L_{xy}^2+(\Delta z)^2}=300\,\mathrm{\mu m}.
$$

Using the projection alone would underestimate this length by $20\%$. A bent track requires a sum over reconstructed segments. These are stipulated coordinates, not measurements of a historical track.

Suppose [photographic processing](photographic-processing.md) contracts the coating only in depth, with shrinkage ratio $s=t_{\rm developed}/t_{\rm exposed}$. Then an observed depth difference $\Delta z_{\rm developed}$ corresponds to $\Delta z=\Delta z_{\rm developed}/s$. For $s=0.60$, an observed $108\,\mathrm{\mu m}$ becomes the $180\,\mathrm{\mu m}$ used above. This correction assumes uniform contraction and unchanged lateral dimensions; it cannot repair a track that leaves the coating before stopping.

A simple continuous-loss model connects [particle range](particle-range.md) to [kinetic energy](kinetic-energy.md) $T_0$ through [stopping power](stopping-power.md) $S(T)=-\mathrm dT/\mathrm dx>0$:

$$
R(T_0)=\int_0^{T_0}\frac{\mathrm dT}{S(T)}.
$$

This describes the mean trend for a specified particle and material. Fluctuating energy loss produces a spread of stopping distances, called [range straggling](range-straggling.md). An exit point supplies only a lower bound on [particle range](particle-range.md). Consequently, a narrow distribution from fully contained tracks and one assembled by treating exits as stops answer different questions.

**Table of contents**

- [Range straggling](range-straggling.md)

## ↑ Ancestors (5)

1. [Nuclear emulsion track experiment](nuclear-emulsion-track-experiment.md)
2. [Nuclear emulsion](nuclear-emulsion.md)
3. [Photographic emulsion](photographic-emulsion.md)
4. [Photography](photography-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Emulsion range measurement](emulsion-range-measurement.md)
