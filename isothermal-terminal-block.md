# Isothermal terminal block

↑ **Parent:** [Thermocouple reference junction](thermocouple-reference-junction.md)

An [isothermal terminal block](isothermal-terminal-block.md) keeps the two reference transitions and the reference [thermometer](thermometer.md) at approximately the same [temperature](temperature-split.md), while maintaining electrical insulation between the terminals. Thermal contact is required; an electrical short between A and B would bypass the signal. Merely using [copper](copper.md) does not eliminate the [Seebeck effect](seebeck-effect.md) in the meter leads. If both homogeneous [copper](copper.md) leads start at $T_c$ and end at a common meter-input [temperature](temperature-split.md) $T_m$, their contributions have equal magnitude and opposite sign around the measurement path:

$$
\int_{T_c}^{T_m}S_{\rm Cu}(T)\,dT-\int_{T_c}^{T_m}S_{\rm Cu}(T)\,dT=0.
$$

This cancellation uses matched endpoint [temperatures](temperature-split.md) and homogeneous lead material, rather than $S_{\rm Cu}=0$. A [temperature gradient](temperature-gradient.md) along each lead is allowed under these assumptions. If the two transitions are at different [temperatures](temperature-split.md), one measured $T_c$ cannot generally correct both; unmatched connectors or wire inhomogeneity can introduce additional [electromotive forces](electromotive-force.md). The FP-TC-120 documentation explicitly locates the reference sensing in the terminal base or connector block and specifies isothermal versions of these assemblies.[p. 7, Cold-Junction Compensation: terminal sensors and isothermal terminal assemblies](fp-tc-120-and-cfp-tc-120-operating-instructions-by-national-instruments.md)

## ↑ Ancestors (8)

1. [Thermocouple reference junction](thermocouple-reference-junction.md)
2. [Thermocouple](thermocouple.md)
3. [Seebeck effect](seebeck-effect.md)
4. [Thermoelectric effect](thermoelectric-effect-split.md)
5. [Electromagnetism](electromagnetism-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Isothermal terminal block](isothermal-terminal-block.md)
- [Thermocouple](thermocouple.md)
- [Thermopile series voltage](thermopile-series-voltage.md)
