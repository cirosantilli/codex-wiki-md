# Thermal noise worked example

↑ **Parent:** [Thermal electrical noise](thermal-electrical-noise.md)

For an original hypothetical calculation, stipulate $T=300\,\mathrm K$, $R=10\,\mathrm{k}\Omega$, and an ideal rectangular measurement [signal bandwidth](signal-bandwidth.md) $B=20\,\mathrm{kHz}$. Using $k_{\rm B}=1.380649\times10^{-23}\,\mathrm{J/K}$ gives

$$
S_v^{(1)}=1.6567788\times10^{-16}\,\mathrm{V^2/Hz},\qquad
\sqrt{S_v^{(1)}}\approx12.872\,\mathrm{nV}/\sqrt{\mathrm{Hz}},
$$



$$
\langle v_{\rm oc}^2\rangle=3.3135576\times10^{-12}\,\mathrm{V^2},\qquad
v_{\rm oc,rms}\approx1.8203\,\mu\mathrm V.
$$

A matched $10\,\mathrm{k}\Omega$ [electrical load](electrical-load.md) receives $0.91016\,\mu\mathrm V$ [root mean square](root-mean-square.md) from the source [resistor](resistor.md), giving $P_{\rm av}=8.283894\times10^{-17}\,\mathrm W$. These are stipulated model predictions, not laboratory measurements. Increasing $R$ raises the [open-circuit voltage](open-circuit-voltage.md) [noise](noise-signal-processing.md) but does not increase the matched available [power](power.md). Restricting the measurement [signal bandwidth](signal-bandwidth.md) reduces [root mean square](root-mean-square.md) [noise](noise-signal-processing.md) as its square root; it improves [signal-to-noise ratio](signal-to-noise-ratio.md) only if the desired [signal](signal.md) is preserved.

## ↑ Ancestors (6)

1. [Thermal electrical noise](thermal-electrical-noise.md)
2. [Noise (signal processing)](noise-signal-processing.md)
3. [Signal](signal.md)
4. [Signal processing](signal-processing.md)
5. [Electrical engineering](electrical-engineering-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Thermal noise measurement](thermal-noise-measurement.md)
