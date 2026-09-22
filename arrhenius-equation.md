# Arrhenius equation

↑ **Parent:** [Activation energy](activation-energy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arrhenius_equation)

The [Arrhenius equation](arrhenius-equation.md) models the [temperature](temperature.md) dependence of a [rate constant](rate-constant.md) by

$$
k(T)=A\exp\left(-\frac{E_a}{RT}\right),\qquad A>0,\quad T>0.
$$

Here $A$ is the [pre-exponential factor](pre-exponential-factor.md), $E_a$ the [activation energy](activation-energy.md), $R$ the [molar gas constant](molar-gas-constant.md), and $T$ the absolute [thermodynamic temperature](thermodynamic-temperature.md). In its original form, $A$ and $E_a$ are held constant over the range being modeled. It is an empirical relationship, not a universal rule for every [reaction mechanism](reaction-mechanism.md). See the [Arrhenius equation](iupac-compendium-of-chemical-terminology-gold-book-by-international-union-of-pure-and-applied-chemistry/arrhenius-equation.md).

Eliminating $A$ between two positive [temperatures](temperature.md) gives the useful prediction

$$
\ln\frac{k(T_2)}{k(T_1)}
=\frac{E_a}{R}\left(\frac1{T_1}-\frac1{T_2}\right).
$$

For $E_a>0$, warming increases $k$. The logarithmic sensitivity is $d\ln(k/k_{\mathrm{ref}})/dT=E_a/(RT^2)$, so there is no universal doubling per ten degrees. The same $10\,\mathrm K$ rise from $300$ to $310\,\mathrm K$ gives a factor $1.67749$ for $E_a=40\,\mathrm{kJ\,mol^{-1}}$, versus $2.81398$ for $80\,\mathrm{kJ\,mol^{-1}}$.

<a id="image-temperature-sensitivity-and-straight-line-arrhenius-plots-for-two-illustrative-activation-energies"></a>
![](arrhenius-temperature-sensitivity.png)

**[Figure 54](#image-temperature-sensitivity-and-straight-line-arrhenius-plots-for-two-illustrative-activation-energies). Temperature sensitivity and straight-line Arrhenius plots for two illustrative activation energies**. Both models are anchored at $k(300\,\mathrm K)=0.100\,\mathrm{s^{-1}}$, so they have different [pre-exponential factors](pre-exponential-factor.md). Left: the higher [activation energy](activation-energy.md) produces a larger relative change with [temperature](temperature.md). Right: the [natural logarithm](natural-logarithm.md) of the dimensionless ratio $k(T)/k(300\,\mathrm K)$ is linear in inverse [temperature](temperature.md). These exact model curves are not experimental data.

The useful simplification is that a strong change in [reaction rate](reaction-rate.md) becomes a straight-line relation after changing variables. Measurements at several [temperatures](temperature.md) can estimate the slope and test whether one pair of constants describes the chosen range. Curvature can indicate a failure of that approximation; fitting a line does not uniquely establish a microscopic [reaction mechanism](reaction-mechanism.md).

Svante Arrhenius's 1889 paper on [sucrose](sucrose.md) conversion through [catalysis](catalysis.md) by a [chemical acid](acid-chemistry.md) compared the strong observed [temperature](temperature.md) dependence with the much smaller increase in collision frequency. He discussed van't Hoff's earlier [temperature](temperature.md) relations and proposed a small population of hypothetical active [sucrose](sucrose.md), replenished from ordinary [sucrose](sucrose.md), to interpret the dependence. The inspected translated excerpt derives an inverse-[temperature](temperature.md) relation in its equations (6)–(7) and then applies it to the [reaction rate](reaction-rate.md). That historical hypothesis is distinct from a modern [transition state](transition-state.md) description. See the [On the Reaction Velocity of the Inversion of Cane Sugar by Acids](on-the-reaction-velocity-of-the-inversion-of-cane-sugar-by-acids.md). The excerpt omits parts of the original paper; it does not provide a complete original apparatus description or dataset.

The [pre-exponential factor](pre-exponential-factor.md) must have the same units as the [rate constant](rate-constant.md), since the [exponential function](exponential-function.md) supplies a [dimensionless quantity](dimensionless-quantity.md). For a [rate law](rate-law.md) $v=k[\mathrm A]^m$, both $A$ and $k$ have units $(\mathrm{mol\,L^{-1}})^{1-m}\,\mathrm{s^{-1}}$. Thus a [first-order reaction](first-order-reaction.md) uses $\mathrm{s^{-1}}$, whereas a [second-order reaction](second-order-reaction.md) uses $\mathrm{L\,mol^{-1}\,s^{-1}}$. Calling $A$ a frequency factor does not give it frequency units for every [order of reaction](order-of-reaction.md). Its value includes the physical and geometrical factors allowed by the chosen [reaction mechanism](reaction-mechanism.md); equal [activation energies](activation-energy.md) need not mean equal [reaction rates](reaction-rate.md).

<a id="image-arrhenius-apparent-energy-and-prefactor"></a>
![](arrhenius-apparent-energy-and-prefactor.png)

**[Figure 55](#image-arrhenius-apparent-energy-and-prefactor). Synthetic Arrhenius plots: a constant pre-exponential factor and a temperature-dependent pre-exponential factor**. Both chosen [first-order reaction](first-order-reaction.md) models have $k(300\,\mathrm K)=0.100\,\mathrm{s^{-1}}$ and the same exponent parameter $E_0=60\,\mathrm{kJ\,mol^{-1}}$. Blue uses a constant [pre-exponential factor](pre-exponential-factor.md); orange multiplies it by $(T/300\,\mathrm K)^2$. All markers are synthetic evaluations, not observations. Left: [natural logarithm](natural-logarithm.md) of $k/k(300\,\mathrm K)$ against $1000\,\mathrm K/T$. Right: the corresponding [apparent activation energies](apparent-activation-energy.md), $60$ and $60+2RT/1000$ in $\mathrm{kJ\,mol^{-1}}$. The dashed orange tangent at $300\,\mathrm K$ has numerical slope $-7.81634$ on the displayed horizontal scale.

To read the blue [Arrhenius plot](arrhenius-plot.md), define the [dimensionless quantity](dimensionless-quantity.md) $X=1000\,\mathrm K/T$ and $y=\ln[k/k(300\,\mathrm K)]$. Its numerical slope is $m_X=-60\,000/(1000R)\approx-7.21634$, giving $E_a=-(1000\,\mathrm K)Rm_X=60\,\mathrm{kJ\,mol^{-1}}$. The slope against $1/T$, by contrast, is $-7216.34\,\mathrm K$. The orange tangent at $300\,\mathrm K$ gives $E_{a,\mathrm{app}}\approx64.9887\,\mathrm{kJ\,mol^{-1}}$; its finite-interval slope between $280$ and $340\,\mathrm K$ gives about $65.1227\,\mathrm{kJ\,mol^{-1}}$. The distinction between a local [derivative](derivative.md) and a fitted interval matters even with perfectly noise-free synthetic evaluations.

Two measured positive [rate constants](rate-constant.md) give a two-point estimate

$$
E_{a,\mathrm{fit}}=R\frac{\ln[k(T_2)/k(T_1)]}{1/T_1-1/T_2}.
$$

Several [temperatures](temperature.md) let [linear regression](linear-regression-split.md) test the constant-parameter approximation: inspect the [regression residuals](regression-residual.md), keep the same [rate law](rate-law.md) and composition convention, and account for uncertainty in both $k$ and $T$. A straight line over a short range supports a useful local approximation; it does not uniquely identify a [reaction mechanism](reaction-mechanism.md). A fixed change of units or of $k_{\mathrm{ref}}$ shifts the intercept without changing the inferred [activation energy](activation-energy.md).[§12.5, Example 12.13 and alternate two-point approach: estimating activation energy from a slope](chemistry-2e-by-paul-flowers-and-others/12-5-collision-theory.md)

**Table of contents**

- [Pre-exponential factor](pre-exponential-factor.md)
- [Arrhenius plot](arrhenius-plot.md)
- [Modified Arrhenius equation](modified-arrhenius-equation.md)
- [Conductometric determination of activation energy](conductometric-determination-of-activation-energy.md)

## ↑ Ancestors (5)

1. [Activation energy](activation-energy.md)
2. [Chemical kinetics](chemical-kinetics.md)
3. [Chemical reaction](chemical-reaction.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Activation energy](activation-energy.md)
- [Arrhenius equation](arrhenius-equation.md)
- [Arrhenius plot](arrhenius-plot.md)
- [Catalyst](catalyst.md)
- [Pre-exponential factor](pre-exponential-factor.md)
