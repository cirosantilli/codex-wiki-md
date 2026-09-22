# Thermal boundary resistance

↑ **Parent:** [Cryogenics](cryogenics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interfacial_thermal_resistance)

[Thermal boundary resistance](thermal-boundary-resistance.md) describes a [temperature](temperature-split.md) drop between the two sides of a material interface carrying [heat flux](heat-flux-density.md). Efficient [thermal conduction](thermal-conduction.md) within each material does not guarantee efficient [heat transfer](heat-transfer.md) between them. The solid–[helium](helium.md) case is [Kapitza resistance](kapitza-resistance.md); the broader concept also includes solid–solid interfaces. [Swartz and Pohl (1989), abstract: helium–solid and solid–solid interfaces](thermal-boundary-resistance-by-e-t-swartz-and-robert-otto-pohl.md)

Let $T_s$ and $T_l$ be the [temperatures](temperature-split.md) extrapolated to the interface from its solid and liquid sides, each treated as internally in [thermal equilibrium](thermal-equilibrium-split.md). For uniform normal [heat flux](heat-flux-density.md) $q>0$ through [area](surface-area.md) $A$, define the finite-drop, area-specific [thermal resistance](thermal-resistance.md) and the resistance of the whole interface by

$$
\Delta T=T_s-T_l,\qquad \dot Q=Aq,\qquad
r_B=\frac{\Delta T}{q}\quad[\mathrm{K\,m^2\,W^{-1}}],\qquad
\mathcal R_B=\frac{\Delta T}{\dot Q}=\frac{r_B}{A}\quad[\mathrm{K\,W^{-1}}].
$$

The macroscopic jump represents an unresolved interfacial region; it is not a claim that one point has two equilibrium [temperatures](temperature-split.md). At nonzero [heat flux](heat-flux-density.md), the two sides are outside mutual [thermal equilibrium](thermal-equilibrium-split.md). A measured difference between distant [thermometers](thermometer.md) also contains bulk [temperature gradients](temperature-gradient.md), which must be measured or bounded before assigning all of it to the interface.

An [energy](energy-split.md) balance explains why a [temperature](temperature-split.md) jump can coexist with continuous [heat flux](heat-flux-density.md). For a stationary interfacial region with no local [work](work.md) or [heat](heat-split.md) source,

$$
\frac{dU_{\rm int}}{dt}=Aq_{\rm in}-Aq_{\rm out}.
$$

The [first law of thermodynamics](first-law-of-thermodynamics-split.md) therefore requires $q_{\rm in}=q_{\rm out}=q$ in a [steady state](steady-state.md). It does not require $T_s=T_l$. For a heated sample with electrical [power](power.md) $P=VI$, an independently determined outward parasitic loss $P_{\rm leak}$ and no other inputs,

$$
\frac{dU_s}{dt}=P-P_{\rm leak}-Aq,\qquad
q=\frac{P-P_{\rm leak}}{A}\quad\text{in a steady state}.
$$

Here $V$ is the heater's [electric potential difference](electric-potential-difference.md) and $I$ its [electric current](electric-current.md). Subtracting a lead loss means subtracting [power](power.md) before dividing by [area](surface-area.md); $q$ is not the total heating [power](power.md). Unknown losses and stored [internal energy](internal-energy-split.md) prevent that simple steady inference.

For a one-dimensional comparison, put an interface between two slabs with the same [area](surface-area.md) $A$, positive constant [thermal conductivities](thermal-conductivity.md) $k_s,k_l$ and [lengths](length.md) $L_s,L_l$. Neglect side losses. Integrating [Fourier's law](fourier-s-law.md) across each slab gives

$$
T_H-T_s=q\frac{L_s}{k_s},\qquad
T_l-T_C=q\frac{L_l}{k_l},\qquad
T_H-T_C=q\left(\frac{L_s}{k_s}+\frac{L_l}{k_l}\right)+(T_s-T_l).
$$

Thus, for a linear interface with constant $r_B$, the series result is

$$
q=\frac{T_H-T_C}{L_s/k_s+r_B+L_l/k_l},\qquad
\mathcal R_{\rm total}=\frac1A\left(\frac{L_s}{k_s}+r_B+\frac{L_l}{k_l}\right).
$$

These slab formulas are a chosen [thermal conduction](thermal-conduction.md) model, not a bulk transport law for moving liquid [helium](helium.md). If the interface law is nonlinear, substitute its own relation between $q$ and $T_s-T_l$ into the preceding balance; a single constant resistance cannot describe every load. Increasing bulk [thermal conductivity](thermal-conductivity.md) has diminishing benefit when the interfacial drop dominates. Increasing usable contact [area](surface-area.md) reduces the whole-interface [thermal resistance](thermal-resistance.md) if the local interface law and the other conditions remain fixed.

**Table of contents**

- [Kapitza resistance](kapitza-resistance.md)
  - [Kapitza thermal boundary experiment](kapitza-thermal-boundary-experiment.md)
  - [Fourth-power thermal boundary model](fourth-power-thermal-boundary-model.md)

## ↑ Ancestors (7)

1. [Cryogenics](cryogenics.md)
2. [Temperature](temperature-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Kapitza resistance](kapitza-resistance.md)
- [Kapitza thermal boundary experiment](kapitza-thermal-boundary-experiment.md)
- [Thermal boundary resistance](thermal-boundary-resistance.md)
