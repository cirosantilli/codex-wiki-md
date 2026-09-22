# Light-emitting diode efficiency

↑ **Parent:** [Light-emitting diode](light-emitting-diode.md)

Efficiency has several denominators. Specify a steady [electric current](electric-current.md) $I>0$, positive terminal [electric potential difference](electric-potential-difference.md) $V_f$, and a simplified narrow emission [spectrum](spectrum-functional-analysis.md) with [photon](photon.md) [energy](energy-split.md) $E_\gamma$. Assume at most one radiative [photon](photon.md) per injected [electron](electron.md) and [electron hole](electron-hole.md) pair. Let $\eta_{\rm inj}$ be the fraction of the electrical pair-supply rate $I/q$ reaching the active layer, $\eta_{\rm rad}$ the fraction of those pairs recombining radiatively, and $\eta_{\rm ext}$ the fraction of internally emitted [photons](photon.md) that escape. Then counting the successive events gives

$$
\dot N_{\rm active}=\eta_{\rm inj}\frac Iq,\qquad
\dot N_{\rm internal}=\eta_{\rm rad}\dot N_{\rm active},\qquad
\dot N_{\rm out}=\eta_{\rm ext}\dot N_{\rm internal}.
$$

Define [internal quantum efficiency](internal-quantum-efficiency.md) here conditionally on pairs reaching the active layer: $\eta_{\rm IQE}=\eta_{\rm rad}$. The internal [photon](photon.md) yield per electrical pair is instead $\eta_{\rm inj}\eta_{\rm IQE}$. Stating this convention matters when another definition folds injection into [internal quantum efficiency](internal-quantum-efficiency.md). The [external quantum efficiency](external-quantum-efficiency.md) and [wall-plug efficiency](wall-plug-efficiency.md) are

$$
\eta_{\rm EQE}=\frac{\dot N_{\rm out}}{I/q}
=\eta_{\rm inj}\eta_{\rm IQE}\eta_{\rm ext},\qquad
\eta_{\rm WPE}=\frac{P_{\rm opt}}{IV_f}
=\eta_{\rm EQE}\frac{E_\gamma}{qV_f},\qquad
P_{\rm opt}=\dot N_{\rm out}E_\gamma.
$$

These are [photon](photon.md)-count and [energy](energy-split.md)-flow identities for the declared model. For a broad [spectrum](spectrum-functional-analysis.md), replace $E_\gamma$ by the mean escaping [photon](photon.md) [energy](energy-split.md), weighted by photon number, when computing optical [power](power.md).

A stipulated example chooses $I=20\,\mathrm{mA}$, $V_f=3.20\,\mathrm V$, $\lambda=450\,\mathrm{nm}$, $\eta_{\rm inj}=0.90$, $\eta_{\rm IQE}=0.80$ and $\eta_{\rm ext}=0.50$. For every 100 electrical pairs, 90 reach the active layer, 72 emit internally, and 36 [photons](photon.md) escape. Thus $\eta_{\rm EQE}=0.36$, not $0.80$. Using $q=1.602176634\times10^{-19}\,\mathrm C$ gives

$$
\begin{aligned}
I/q&=1.24830\times10^{17}\,\mathrm{s}^{-1},\\
\dot N_{\rm out}&=4.49389\times10^{16}\,\mathrm{s}^{-1},\\
P_{\rm opt}&=19.8375\,\mathrm{mW},\qquad IV_f=64.0\,\mathrm{mW},\\
\eta_{\rm WPE}&=0.309960.
\end{aligned}
$$

The [dimensional analysis](dimensional-analysis.md) is transparent: $\mathrm{A/C}=\mathrm{s}^{-1}$, $\mathrm{J/s}=\mathrm W$, and $\mathrm{CV}=\mathrm J$. The optical and electrical efficiencies differ because $E_\gamma/q=2.75520\,\mathrm V$ differs from the chosen $V_f$.

<a id="image-photon-energy-wavelength-and-a-chosen-light-emitting-diode-efficiency-budget"></a>
![](blue-led-photon-energy-and-efficiency.png)

**[Figure 4](#image-photon-energy-wavelength-and-a-chosen-light-emitting-diode-efficiency-budget). Photon energy, wavelength and a chosen light-emitting diode efficiency budget**. [Source](blue-led-photon-energy-and-efficiency.py). Original calculations, not measurements or specifications of the historical devices. Left: $E_\gamma=hc/\lambda$, with chosen blue and converted-light [wavelengths](wavelength.md). Right: successive [photon](photon.md) counts per 100 electrical pairs for $\eta_{\rm inj}=0.90$, $\eta_{\rm IQE}=0.80$, $\eta_{\rm ext}=0.50$. The optional converter calculation uses the separately stipulated absorption fraction and [fluorescence quantum yield](fluorescence-quantum-yield.md) below.

The factors suggest different improvements. Better confinement can reduce injection leakage; suppressing [nonradiative recombination](nonradiative-recombination.md) raises the radiative fraction; improving [light extraction efficiency](light-extraction-efficiency.md) helps already-emitted [photons](photon.md) escape. A [photon](photon.md) trapped by [total internal reflection](total-internal-reflection.md) has already passed the radiative step and can still be lost through absorption. Improving extraction therefore need not change the internal radiative fraction. 

[Shuji Nakamura](shuji-nakamura.md)'s lecture cautions that why [indium gallium nitride](indium-gallium-nitride.md) emits efficiently despite many defects was not completely settled in that account.[§IV.B, pp. 1144–1145: high defect density, localization hypothesis and stated uncertainty](https://journals.aps.org/rmp/pdf/10.1103/RevModPhys.87.1139)

As an independent consistency check on the 1994 reported values, treating its broad [spectrum](spectrum-functional-analysis.md) as monochromatic at the $450\,\mathrm{nm}$ peak gives

$$
\eta_{\rm EQE}\approx\frac{(1.5\times10^{-3}\,\mathrm W)q}{(0.020\,\mathrm A)(hc/(450\,\mathrm{nm}))}=0.02722.
$$

This agrees at the quoted precision with the reported $2.7\%$. Its optical/electrical [power](power.md) ratio is instead $1.5\,\mathrm{mW}/(20\,\mathrm{mA}\times3.6\,\mathrm V)=2.0833\%$. The first estimate uses a peak in place of a photon-number-weighted mean, so agreement is a consistency check rather than an exact reanalysis of the measured [spectrum](spectrum-functional-analysis.md).

**Table of contents**

- [Internal quantum efficiency](internal-quantum-efficiency.md)
- [External quantum efficiency](external-quantum-efficiency.md)
- [Light extraction efficiency](light-extraction-efficiency.md)
- [Wall-plug efficiency](wall-plug-efficiency.md)

## ↑ Ancestors (7)

1. [Light-emitting diode](light-emitting-diode.md)
2. [Diode](diode.md)
3. [Electrical circuit](electrical-circuit-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Internal quantum efficiency](internal-quantum-efficiency.md)
- [Light-emitting diode](light-emitting-diode.md)
- [Light-emitting diode efficiency](light-emitting-diode-efficiency.md)
- [Wall-plug efficiency](wall-plug-efficiency.md)
