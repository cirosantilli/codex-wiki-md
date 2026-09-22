# Respirometer gas balance

↑ **Parent:** [Respirometer](respirometer.md)

For an original idealized [mathematical model](mathematical-model.md), let $n_{\mathrm O_2}(t)$ be the [amount of substance](amount-of-substance.md) of [molecular oxygen](molecular-oxygen.md) consumed since the initial reading and $n_{\mathrm{CO}_2}(t)$ the [carbon dioxide](carbon-dioxide.md) produced. Suppose a fraction $f$ of that [carbon dioxide](carbon-dioxide.md) is removed from the gas, all other gas inventories remain fixed, and [temperature](temperature-split.md) $T$ and gas [pressure](pressure-split.md) $P$ stay constant. The [ideal gas law](ideal-gas-law.md) gives the positive gas contraction

$$
D(t)=V(0)-V(t)=\frac{RT}{P}\left[n_{\mathrm O_2}(t)-(1-f)n_{\mathrm{CO}_2}(t)\right],
$$

where $R$ is the [molar gas constant](molar-gas-constant.md) and $V$ the gas [volume](volume.md). With complete absorption, $f=1$, the contraction reflects [molecular oxygen](molecular-oxygen.md) uptake regardless of the amount of [carbon dioxide](carbon-dioxide.md) made. For a uniform pipette bore of [area](surface-area.md) $A$, an inward boundary displacement $x$ gives $D=Ax$. A graduated pipette can instead supply the displaced [volume](volume.md) directly.

Let $D_s$ denote sample contraction and $D_b$ the matched blank contraction. Define $D_{\mathrm{corr}}=D_s-D_b$ with both taken relative to their own initial readings. Under the preceding assumptions,

$$
n_{\mathrm O_2}(t)\simeq\frac{P D_{\mathrm{corr}}(t)}{RT},\qquad
\overline{r}_{\mathrm O_2}=\frac{P}{RT}\frac{D_{\mathrm{corr}}(t_2)-D_{\mathrm{corr}}(t_1)}{t_2-t_1}.
$$

The [slope](slope.md) of corrected [volume](volume.md) against [time](time-in-physics.md) estimates uptake over the chosen interval. The approximate sign acknowledges that a liquid boundary also responds to hydrostatic and capillary [pressure](pressure-split.md), while the gas can exchange [water](water.md) vapour. A fixed-[volume](volume.md) apparatus would instead show a [pressure](pressure-split.md) decrease; its ideal conversion is $n_{\mathrm O_2}\simeq V\bigl(P(0)-P(t)\bigr)/(RT)$ after complete absorption and appropriate blank correction.

The [ideal gas law](ideal-gas-law.md) also exposes drift without any biology: for fixed gas inventory, $V\propto T/P$. A one-percent rise in absolute [temperature](temperature-split.md) at fixed [pressure](pressure-split.md) produces a one-percent expansion. Matching the initial gas spaces makes such common changes easier to subtract. Subtracting unmatched blanks can leave a physical signal that looks biological.

**Table of contents**

- [Respiratory quotient](respiratory-quotient.md)

## ↑ Ancestors (5)

1. [Respirometer](respirometer.md)
2. [Cellular respiration](cellular-respiration.md)
3. [Metabolism](metabolism.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Pea seed respirometry](pea-seed-respirometry.md)
- [Respiratory quotient](respiratory-quotient.md)
