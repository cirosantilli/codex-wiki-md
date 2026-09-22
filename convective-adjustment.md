# Convective adjustment

↑ **Parent:** [Radiative-convective climate column](radiative-convective-climate-column.md)

[Convective adjustment](convective-adjustment.md) replaces an excessively steep vertical [temperature gradient](temperature-gradient.md) by an allowed profile while respecting the selected [energy](energy-split.md) budget. It is a closure for unresolved [convection](convection-split.md), not a direct simulation of individual rising parcels. A prescribed critical [atmospheric lapse rate](lapse-rate-atmosphere.md) is a modeling assumption; it need not equal the [dry adiabatic lapse rate](dry-adiabatic-lapse-rate.md).

For an original dry two-slab example, take fixed equal [heat capacities](heat-capacity.md) and slab centers separated by $\Delta z=2\,\mathrm{km}$. Initially $T_1=300\,\mathrm K$ below and $T_2=280\,\mathrm K$ above. Stipulate a permitted [atmospheric lapse rate](lapse-rate-atmosphere.md) $\Gamma_c=6\,\mathrm{K\,km^{-1}}$. The initial difference $20\,\mathrm K$ exceeds the allowed $12\,\mathrm K$. Conservation of the sum of the two sensible [energies](energy-split.md) requires $T_1'+T_2'=580\,\mathrm K$, while the adjusted gradient requires $T_1'-T_2'=12\,\mathrm K$. Hence $T_1'=296\,\mathrm K$ and $T_2'=284\,\mathrm K$. Heat removed below equals heat added above. Simply holding the lower slab fixed and raising the upper slab to $288\,\mathrm K$ would introduce external [energy](energy-split.md).

For unequal constant [heat capacities](heat-capacity.md) $C_1,C_2$, the same two constraints instead give

$$
T_1'=\frac{C_1T_1+C_2T_2+C_2\Gamma_c\Delta z}{C_1+C_2},
\qquad T_2'=T_1'-\Gamma_c\Delta z.
$$

Apply this adjustment only when the original gradient exceeds the threshold. A moist adjustment also has to account for [latent heat](latent-heat.md) and changing composition; conservation of this dry sensible-[energy](energy-split.md) expression alone is then insufficient.

## ↑ Ancestors (7)

1. [Radiative-convective climate column](radiative-convective-climate-column.md)
2. [Climate model](climate-model.md)
3. [Climate change](climate-change.md)
4. [Geophysics](geophysics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Convective adjustment](convective-adjustment.md)
- [Radiative-convective climate column](radiative-convective-climate-column.md)
