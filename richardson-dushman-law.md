# Richardson-Dushman law

↑ **Parent:** [Thermionic emission](thermionic-emission-split.md)

The [Richardson-Dushman law](richardson-dushman-law.md) models the magnitude of emitted [electric current density](current-density.md) as

$$
J=A T^2\exp\!\left(-\frac{W}{k_BT}\right).
$$

Here $T$ is absolute [thermodynamic temperature](thermodynamic-temperature.md), $W$ is the [work function](work-function.md), $k_B$ is the [Boltzmann constant](boltzmann-constant.md), and $A$ is the [Thermionic Richardson constant](thermionic-richardson-constant.md). The signed [electric current density](current-density.md) points opposite to the outgoing [electron](electron.md) motion; $J$ here is positive. For uniform emission over area $S$, the emitted [electric current](electric-current.md) magnitude is $I=SJ$.

The [Richardson-Dushman law](richardson-dushman-law.md) assumes an emitter close to [thermal equilibrium](thermal-equilibrium-split.md), a surface with a well-defined and approximately constant [work function](work-function.md) over the fitted [temperature](temperature-split.md) range, and predominantly thermal escape over the barrier. Interpreting a measured collector [electric current](electric-current.md) with this law additionally requires an [emission-limited thermionic current](emission-limited-thermionic-current.md), known emitting area, and negligible return emission from the collector. Strong [electric fields](electric-field-split.md) can lower the surface barrier or enable [quantum tunnelling](quantum-tunnelling.md); then this zero-field expression is insufficient.

For a deliberately chosen teaching model, take $W=2.0\,\mathrm{eV}$ and $A=120\,\mathrm{A\,cm^{-2}\,K^{-2}}$, expressing the barrier in [electronvolts](electronvolt.md). These are illustrative parameters, not measured properties of a named material. Using $k_B=8.617333262\times10^{-5}\,\mathrm{eV\,K^{-1}}$, at $1000\,\mathrm K$ the [Boltzmann factor](boltzmann-factor.md) is about $8.33\times10^{-11}$, yet

$$
J(1000\,\mathrm K)\simeq0.00999\,\mathrm{A\,cm^{-2}},
\qquad
J(1200\,\mathrm K)\simeq0.6885\,\mathrm{A\,cm^{-2}}.
$$

A 20 percent increase in [temperature](temperature-split.md) raises the predicted [electric current density](current-density.md) by about 69 times. For a chosen emitting area $S=0.010\,\mathrm{cm^2}$, these correspond to approximately $0.100\,\mathrm{mA}$ and $6.89\,\mathrm{mA}$ if collection is complete. The small escaping fraction is replenished by the external [electrical circuit](electrical-circuit-split.md).

The sensitivity is especially clear from the [logarithmic derivative](logarithmic-derivative.md) at fixed $A,W$:

$$
\frac{d\ln J}{dT}=\frac{2}{T}+\frac{W}{k_BT^2}.
$$

In the chosen model at $1000\,\mathrm K$, a $1\,\mathrm K$ rise changes $J$ by about 2.5 percent to first order. Accurate [temperature](temperature-split.md) measurement matters even when [electric current](electric-current.md) measurement is easy.

**Table of contents**

- [Thermionic Richardson constant](thermionic-richardson-constant.md)
- [Richardson plot](richardson-plot.md)
- [Thermionic tail-flux derivation](thermionic-tail-flux-derivation.md)

## ↑ Ancestors (5)

1. [Thermionic emission](thermionic-emission-split.md)
2. [Electron](electron.md)
3. [Subatomic particle](subatomic-particle.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Emission-limited thermionic current](emission-limited-thermionic-current.md)
- [Richardson-Dushman law](richardson-dushman-law.md)
- [Richardson plot](richardson-plot.md)
- [Thermionic emission](thermionic-emission-split.md)
