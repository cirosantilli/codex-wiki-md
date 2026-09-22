# Wet-ice bias in fusion calorimetry

↑ **Parent:** [Ice-melting calorimetry](ice-melting-calorimetry.md)

Surface [water](water.md) counted as [ice](ice.md) needs warming but has already undergone [melting](melting.md). Its presence therefore biases a dry-ice estimate of [latent heat of fusion](latent-heat-of-fusion.md) downward. This is why drying the added [ice](ice.md) is a quantitative control in [ice-melting calorimetry](ice-melting-calorimetry.md), rather than cosmetic preparation. Let $m_a$ be the total added [mass](mass.md) at $T_m$, of which a fraction $r$ is already [liquid](liquid.md) and $(1-r)$ remains [solid](solid.md). The correct constant-property balance is

$$
(m_wc_w+C_{\rm cal})(T_i-T_f)+Q_{\rm env}=(1-r)m_aL+m_ac_w(T_f-T_m).
$$

If an analysis incorrectly treats all $m_a$ as [solid](solid.md) and sets $Q_{\rm env}=0$, it obtains

$$
L_{\rm app}=\frac{(m_wc_w+C_{\rm cal})(T_i-T_f)}{m_a}-c_w(T_f-T_m)=(1-r)L-\frac{Q_{\rm env}}{m_a}.
$$

Thus $r=0.10$ gives a $10\%$ low estimate with no heat leak. Unaccounted incoming [heat](heat.md) also lowers the estimate; outgoing [heat](heat.md) raises it. These signs follow directly from the displayed [energy](energy.md) balance. Conversely, dry [ice](ice.md) initially below $T_m$ absorbs additional [sensible heat](sensible-heat.md); neglecting that term overestimates $L$. These are different biases and may partially cancel, so agreement with a reference value alone does not validate the controls.

<a id="image-count-only-the-solid-addition-as-fusion-mass-and-account-for-environmental-heat"></a>
![](fusion-latent-heat-calorimetry-bias.png)

**[Figure 4](#image-count-only-the-solid-addition-as-fusion-mass-and-account-for-environmental-heat). Count only the solid addition as fusion mass, and account for environmental heat**. Original mixing schematic and analytic bias curves, not measured data. Stipulated model: $m_w=0.200\,\mathrm{kg}$, $m_a=0.050\,\mathrm{kg}$, $T_i-T_m=30\,\mathrm K$, $C_{\rm cal}=40\,\mathrm{J\,K^{-1}}$, $c_w=4180\,\mathrm{J\,kg^{-1}\,K^{-1}}$ and $L=334000\,\mathrm{J\,kg^{-1}}$. The leak curves use fixed total $Q_{\rm env}=+1000,0,-1000\,\mathrm J$ as separate hypothetical cases, not a fitted heat-transfer law.

For this model with $r=0$ and $Q_{\rm env}=0$, the balance predicts $T_f-T_m\simeq8.829\,\mathrm K$, with $16.700\,\mathrm{kJ}$ consumed by fusion and $1.845\,\mathrm{kJ}$ by warming the melted [water](water.md). At $r=0.10$ with the same zero leak, it predicts $T_f-T_m\simeq10.369\,\mathrm K$ and $L_{\rm app}=300.6\,\mathrm{kJ\,kg^{-1}}$. A net incoming $1\,\mathrm{kJ}$ shifts $L_{\rm app}$ downward by a further $20\,\mathrm{kJ\,kg^{-1}}$ because $m_a=0.050\,\mathrm{kg}$. The warmer final [water](water.md) in the wet case is evidence of a smaller fusion budget, not a larger true $L$.

## ↑ Ancestors (6)

1. [Ice-melting calorimetry](ice-melting-calorimetry.md)
2. [Latent heat of fusion](latent-heat-of-fusion.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
