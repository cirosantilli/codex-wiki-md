# Solubility product and material balance

↑ **Parent:** [Solubility product](solubility-product.md)

A [solubility product](solubility-product.md) constrains a product of [thermodynamic activities](thermodynamic-activity.md); the available inventories determine which combinations of [concentrations](concentration.md) are possible. Their intersection determines the [molar solubility](molar-solubility.md). Consider an original, abstract AB [solid](solid.md), with the preceding one-to-one dissolution [chemical equation](chemical-equation.md). Stipulate $c^\circ=1\,\mathrm M$, $\gamma_{\mathrm A}=\gamma_{\mathrm B}=1$ and $K_{\mathrm{sp},c}=10^{-4}\,\mathrm M^2$ at fixed [temperature](temperature-split.md) and [pressure](pressure-split.md). Thus $K_{\mathrm{sp}}=10^{-4}$ is [dimensionless](dimensionless-quantity.md). These are chosen model parameters, not data for an identified material.

Initially, a completely dissociated soluble XB [salt](salt-chemistry.md) supplies B [anions](anion.md) at [molar concentration](molar-concentration.md) $c_0\geq0$ and X [cations](cation.md) at the same [molar concentration](molar-concentration.md); A is absent. All three [ions](ion.md) have unit [electric charge](electric-charge-split.md) magnitude. X remains a [spectator ion](spectator-ion.md), and only AB can form a [solid](solid.md). Assume constant [volume](volume-thermodynamics.md), no additional [chemical reactions](chemical-reaction-split.md), and negligible contributions from [self-ionization of water](self-ionization-of-water.md). Dissolving AB raises both reacting-ion [concentrations](concentration.md) by the same $s$:

$$
c_{\mathrm A}=s,\qquad c_{\mathrm B}=c_0+s,\qquad c_{\mathrm X}=c_0.
$$

[Charge neutrality](charge-neutrality.md) is satisfied: $c_{\mathrm A}+c_{\mathrm X}-c_{\mathrm B}=s+c_0-(s+c_0)=0$. Adding B alone without its accompanying [cation](cation.md) would omit the initial [electric charge](electric-charge-split.md) balance.

In the plane of the two reacting-ion [concentrations](concentration.md), this inventory constraint is the [line](straight-line.md) $c_{\mathrm B}=c_{\mathrm A}+c_0$. Saturation supplies the [hyperbola](hyperbola.md) $c_{\mathrm B}=K_{\mathrm{sp},c}/c_{\mathrm A}$ for $c_{\mathrm A}>0$. Their positive intersection solves a [quadratic equation](quadratic-equation.md):

$$
s(s+c_0)=K_{\mathrm{sp},c},\qquad
s_* =\frac{\sqrt{c_0^2+4K_{\mathrm{sp},c}}-c_0}{2}
=\frac{2K_{\mathrm{sp},c}}{\sqrt{c_0^2+4K_{\mathrm{sp},c}}+c_0}.
$$

The [quadratic formula](quadratic-formula.md) supplies two [roots of a polynomial](root-of-a-polynomial.md); only the positive one is a physical [concentration](concentration.md). Uniqueness also follows because $s(s+c_0)$ strictly increases for $s\geq0$, starting at zero and growing without bound. The second expression, obtained by multiplying by the conjugate, avoids subtraction of nearly equal numbers at large $c_0$.

<a id="image-solubility-product-and-material-balance-and-the-conditional-solubility-product-select-the-dissolved-concentrations"></a>
![](solubility-product-balance-intersection.png)

**[Figure 2](#image-solubility-product-and-material-balance-and-the-conditional-solubility-product-select-the-dissolved-concentrations). Solubility product and material balance and the conditional solubility product select the dissolved concentrations**. Original stipulated AB model with $K_{\mathrm{sp},c}=10^{-4}\,\mathrm M^2$ and unit [activity coefficients](activity-coefficient.md). Intersections of the saturation [hyperbola](hyperbola.md) with inventory [lines](straight-line.md) give the pure-[water](water.md) and common-ion [chemical equilibrium](chemical-equilibrium.md) compositions. The dashed projections read the $c_0=0.03\,\mathrm M$ intersection; these curves are calculated constraints, not measured data or a time evolution.

For pure [water](water.md), $c_0=0$ gives $s_*=\sqrt{K_{\mathrm{sp},c}}=0.010\,\mathrm M$. For $c_0=0.030\,\mathrm M$,

$$
s_*\approx0.003027756\,\mathrm M,\qquad
c_{\mathrm B}\approx0.033027756\,\mathrm M.
$$

Their product is $10^{-4}\,\mathrm M^2$, although neither [concentration](concentration.md) equals the pure-[water](water.md) value. This is the useful geometrical distinction: an inventory [line](straight-line.md) and an [equilibrium constant](equilibrium-constant.md) specify different constraints.

Check the [solid](solid.md) inventory before imposing saturation. If the initially added AB has [amount of substance](amount-of-substance.md) $n_0$ in [volume](volume-thermodynamics.md) $V$, the saturated branch requires $n_0>Vs_*$ for excess [solid](solid.md) to remain. For example, choose $n_0=0.0020\,\mathrm{mol}$ and $V=0.100\,\mathrm L$. In pure [water](water.md), $0.0010\,\mathrm{mol}$ dissolves and the same [amount of substance](amount-of-substance.md) remains as [solid](solid.md). At $c_0=0.030\,\mathrm M$, approximately $0.0003027756\,\mathrm{mol}$ dissolves, leaving $0.0016972244\,\mathrm{mol}$ as [solid](solid.md). In this model, an insufficient supply instead gives

$$
s=\min\{n_0/V,s_*\}.
$$

If $n_0/V<s_*$, all AB dissolves and the [ion product](ion-product.md) is below the [solubility product](solubility-product.md). At $n_0/V=s_*$, the last [solid](solid.md) disappears exactly at saturation.

## ↑ Ancestors (5)

1. [Solubility product](solubility-product.md)
2. [Precipitation (chemistry)](precipitation-chemistry.md)
3. [Chemical reaction](chemical-reaction-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Common-ion effect](common-ion-effect.md)
- [Solubility product and material balance](solubility-product-and-material-balance.md)
