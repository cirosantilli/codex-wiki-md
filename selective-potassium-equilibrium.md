# Selective potassium equilibrium

↑ **Parent:** [Membrane potential](membrane-potential-split.md)

For an ideal dilute [chemical solution](solution-chemistry.md), moving one [mole](mole-unit.md) of a species with signed [ion](ion.md) charge number $z$ from outside to inside changes its [electrochemical potential](electrochemical-potential.md) by

$$
\Delta\widetilde\mu=RT\ln\!\left(\frac{c_{\mathrm{in}}}{c_{\mathrm{out}}}\right)+zFV_m.
$$

Here $R$ is the [molar gas constant](molar-gas-constant.md), $T$ the uniform absolute [temperature](temperature-split.md), $F$ the [Faraday constant](faraday-constant.md), and $c$ the [concentration](concentration.md). This assumes the same reference [chemical potential](chemical-potential-split.md) on both sides. At [thermodynamic equilibrium](thermodynamic-equilibrium.md), $\Delta\widetilde\mu=0$, hence

$$
E_{\mathrm{ion}}=\frac{RT}{zF}\ln\!\left(\frac{c_{\mathrm{out}}}{c_{\mathrm{in}}}\right).
$$

The [Nernst equilibrium potential](nernst-equilibrium-potential.md) uses [thermodynamic activities](thermodynamic-activity.md) in the general case; replacing them by [concentrations](concentration.md) is an ideal-solution approximation.

Choose an original passive model: only $\mathrm K^+$ permeates ($z=+1$), other [ions](ion.md) cannot cross, there are no pumps or imposed [electric currents](electric-current.md), and there is no net [water](water.md) transfer. Stipulate reservoir [concentrations](concentration.md) $c_{\mathrm{in}}=140\,\mathrm{mM}$ and $c_{\mathrm{out}}=5\,\mathrm{mM}$, with $T=310\,\mathrm K$, $R=8.314\,\mathrm{J\,mol^{-1}\,K^{-1}}$ and $F=96485\,\mathrm{C\,mol^{-1}}$. Treat reservoir [concentrations](concentration.md) as effectively unchanged by charging. Then

$$
E_{\mathrm K}=\frac{8.314\times310}{96485}\ln\!\left(\frac5{140}\right)\,\mathrm V
\approx-0.08901\,\mathrm V=-89.01\,\mathrm{mV}.
$$

The [concentration](concentration.md) ratio is dimensionless; $\mathrm{J/C}=\mathrm V$ supplies the voltage unit. At $V_m=0$, $\Delta\widetilde\mu>0$ for inward transport, so outward transport is favored. At $V_m=E_{\mathrm K}$ it vanishes. A more negative $V_m$ favors inward transport. These sign checks explain the result physically.

Keeping the other chosen inputs fixed, doubling $c_{\mathrm{out}}$ to $10\,\mathrm{mM}$ raises $E_{\mathrm K}$ by $(RT/F)\ln2\approx18.52\,\mathrm{mV}$. Equal inside and outside [concentrations](concentration.md) give $E_{\mathrm K}=0$; reversing their ratio reverses its sign. In finite reservoirs, transport changes both [concentrations](concentration.md); the exact final [thermodynamic equilibrium](thermodynamic-equilibrium.md) must also satisfy material conservation. The fixed-reservoir calculation is useful when only a small fraction of the available [ions](ion.md) moves.

## ↑ Ancestors (4)

1. [Membrane potential](membrane-potential-split.md)
2. [Biological cell](biological-cell-split.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)
