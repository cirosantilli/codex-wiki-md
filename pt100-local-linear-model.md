# Pt100 local linear model

↑ **Parent:** [Pt100](pt100.md)

Choose the illustrative local model

$$
R(t)=R_0(1+\alpha t),\qquad
R_0=100\,\Omega,\qquad
\alpha=0.00385\,({}^\circ\mathrm C)^{-1}.
$$

Here $t$ is the Celsius [temperature](temperature-split.md), measured relative to $0\,{}^\circ\mathrm C$, so $\alpha t$ is dimensionless. For this chosen [affine function](affine-function.md), the [derivative](derivative.md) and inverse relation are

$$
\frac{dR}{dt}=R_0\alpha=0.385\,\Omega/{}^\circ\mathrm C,\qquad
t=\frac{R/R_0-1}{\alpha},\qquad
\Delta t=\frac{\Delta R}{0.385\,\Omega/{}^\circ\mathrm C}.
$$

Calculated values are $R(0\,{}^\circ\mathrm C)=100\,\Omega$, $R(20\,{}^\circ\mathrm C)=107.70\,\Omega$, $R(25\,{}^\circ\mathrm C)=109.625\,\Omega$, and $R(50\,{}^\circ\mathrm C)=119.25\,\Omega$. These are model outputs, not measurements or an assertion that any real [Pt100](pt100.md) follows this line exactly. The number $0.00385$ here is the chosen slope parameter; it is not a universal local [derivative](derivative.md) for all [platinum resistance thermometers](platinum-resistance-thermometer.md). Curvature, manufacturing differences, and the fitted calibration interval matter. A wider-range calibration uses a validated response curve rather than extrapolating this line indefinitely.

<a id="platinum-resistance-temperature-calibration"></a>
![](platinum-resistance-temperature-calibration.png)

**[Figure 3](#platinum-resistance-temperature-calibration). Chosen Pt100 line and an illustrative calibration with an independent check**. [Source](platinum-resistance-temperature-calibration.py). The left panel plots the [Pt100 local linear model](pt100-local-linear-model.md). The right panel uses stipulated values for a different illustrative element: two points set a line, while a third point tests it. Every point is synthetic; none is measured calibration data or a tolerance band.

For a separate synthetic [thermometer calibration](thermometer-calibration.md), stipulate $R_a=100.20\,\Omega$ at $t_a=0\,{}^\circ\mathrm C$ and $R_b=119.60\,\Omega$ at $t_b=50\,{}^\circ\mathrm C$. A two-point [affine function](affine-function.md) has slope $0.388\,\Omega/{}^\circ\mathrm C$ and gives

$$
t=\frac{R-100.20\,\Omega}{0.388\,\Omega/{}^\circ\mathrm C}.
$$

Thus $R=109.90\,\Omega$ would indicate $25\,{}^\circ\mathrm C$. If an additional synthetic check at reference $25\,{}^\circ\mathrm C$ instead supplied $110.10\,\Omega$, the line would indicate $25.515\ldots\,{}^\circ\mathrm C$. The $0.20\,\Omega$ residual exposes disagreement that two fitted points cannot reveal. This separate example changes both offset and slope; it is not a replacement specification for the nominal [Pt100 local linear model](pt100-local-linear-model.md).

## ↑ Ancestors (11)

1. [Pt100](pt100.md)
2. [Industrial platinum resistance thermometer](industrial-platinum-resistance-thermometer.md)
3. [Platinum resistance thermometer](platinum-resistance-thermometer.md)
4. [Resistance thermometer](resistance-thermometer.md)
5. [Thermometer](thermometer.md)
6. [Temperature](temperature-split.md)
7. [Thermodynamics](thermodynamics-split.md)
8. [Statistical physics](statistical-physics-split.md)
9. [Branches of physics](branches-of-physics.md)
10. [Physics](physics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Platinum resistance thermometer lead resistance error](platinum-resistance-thermometer-lead-resistance-error.md)
- [Pt100](pt100.md)
- [Pt100 local linear model](pt100-local-linear-model.md)
- [Resistance thermometer self-heating](resistance-thermometer-self-heating.md)
