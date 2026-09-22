# Electrical substitution heat balance

↑ **Parent:** [Electrical substitution radiometer](electrical-substitution-radiometer.md)

An explicit lumped model makes the cancellation understandable. Treat the receiver as having uniform [temperature](temperature-split.md) $T$, [heat capacity](heat-capacity.md) $C$, heater [power](power.md) $P_h$ deposited in the receiver, net parasitic input $P_{\rm par}$, and outward [heat transfer](heat-transfer.md) $Q_{\rm out}(T,T_b)$ to a reference at [temperature](temperature-split.md) $T_b$. With incident [radiant flux](radiant-flux.md) $P_{\rm in}$ and [radiometric absorptance](radiometric-absorptance.md) $a$, [conservation of energy](conservation-of-energy.md) gives

$$
C\frac{dT}{dt}=P_h+aP_{\rm in}+P_{\rm par}-Q_{\rm out}(T,T_b).
$$

The dark state has no admitted beam. Compare settled dark and light states, denoted $d$ and $l$; each has $dT/dt=0$. Subtracting their balances gives

$$
P_{\rm abs}=aP_{\rm in}=\Delta P_h+\Delta Q_{\rm out}-\Delta P_{\rm par},\qquad
\Delta P_h=P_{h,d}-P_{h,l},
$$

where $\Delta Q_{\rm out}=Q_{{\rm out},l}-Q_{{\rm out},d}$ and $\Delta P_{\rm par}=P_{{\rm par},l}-P_{{\rm par},d}$. At identical $T$ and $T_b$, with unchanged surroundings and parasitic heating, both correction differences vanish. Thus $P_{\rm abs}=\Delta P_h$, and $P_{\rm in}=\Delta P_h/a$. Notice the signs: extra stray [thermal radiation](thermal-radiation.md) admitted with the beam also reduces heater [power](power.md), so it must be subtracted from that reduction before attributing the result to the intended beam.

Measure the heater's own terminal voltage $V_h$ and [electric current](electric-current.md) $I_h$: for steady electrical heating, $P_h=V_hI_h=I_h^2R_h$, where $R_h$ is its [electrical resistance](electrical-resistance.md). A supply voltage that includes wire voltage drops counts [Joule heating](joule-heating.md) in the leads too; only the portion deposited in the receiver belongs in this balance. Changes in that deposited lead [heat](heat-split.md) belong in $\Delta P_{\rm par}$. [Optical-electrical heating non-equivalence](optical-electrical-heating-non-equivalence.md) adds a further instrument-specific correction when the uniform-[temperature](temperature-split.md) model is insufficient.[§5.2, printed p. 30: heater wires, window transmission and optical/electrical non-equivalence](spectroradiometric-detector-measurements-ultraviolet-visible-and-near-infrared-detectors-for-spectral-power-by-thomas-c-larason-and-others.md)

**Table of contents**

- [Radiometer thermal link](radiometer-thermal-link.md)
- [Fixed-temperature electrical substitution example](fixed-temperature-electrical-substitution-example.md)

## ↑ Ancestors (6)

1. [Electrical substitution radiometer](electrical-substitution-radiometer.md)
2. [Radiometry](radiometry-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Optical-electrical heating non-equivalence](optical-electrical-heating-non-equivalence.md)
