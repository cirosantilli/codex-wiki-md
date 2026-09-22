# Thermocouple reference function

↑ **Parent:** [Thermocouple voltage calibration](thermocouple-voltage-calibration.md)

A [thermocouple reference function](thermocouple-reference-function.md) gives the nominal thermoelectric [electromotive force](electromotive-force.md) versus [temperature](temperature-split.md) for a specified material pair and reference [temperature](temperature-split.md), conventionally $0\,{}^\circ\mathrm C$. Real [Seebeck coefficients](seebeck-coefficient.md) vary with [temperature](temperature-split.md), so

$$
F'(T)=S_A(T)-S_B(T)
$$

is generally nonconstant. A lookup calibration can use [interpolation](interpolation-split.md) between tabulated values; a fitted calibration can use [polynomials](polynomial-split.md) over stated intervals. Use the correct material type, units, reference and validity interval in both the forward and inverse conversions. The FP-TC-120 manual specifically requires the channel's [thermocouple](thermocouple.md) type to be configured and describes its use of NIST-175 reference characteristics.[p. 6, Connecting Thermocouple Input Signals: channel type and NIST-175 linearization](fp-tc-120-and-cfp-tc-120-operating-instructions-by-national-instruments.md) A nominal reference curve is not evidence that an aged or inhomogeneous wire still follows it.

A local error estimate explains why the reference [thermometer](thermometer.md) matters. If $\delta V$ is an additive voltage error and $\delta T_c$ is the error in the supplied reference [temperature](temperature-split.md), [differentiation](differentiation.md) of the compensation equation gives, for $F'(T_h)\ne0$,

$$
\delta T_h\approx\frac{\delta V+F'(T_c)\,\delta T_c}{F'(T_h)}.
$$

A small [slope](slope.md) $F'(T_h)$ magnifies voltage errors. In the stipulated $40\,\mu\mathrm{V/K}$ model, a $40\,\mu\mathrm V$ offset gives a $1\,\mathrm K$ inferred-[temperature](temperature-split.md) error, and a $1\,\mathrm K$ reference error gives a $1\,\mathrm K$ inferred-[temperature](temperature-split.md) error. These are sensitivities of the chosen model, not universal performance figures for real sensors.

## ↑ Ancestors (8)

1. [Thermocouple voltage calibration](thermocouple-voltage-calibration.md)
2. [Thermocouple](thermocouple.md)
3. [Seebeck effect](seebeck-effect.md)
4. [Thermoelectric effect](thermoelectric-effect-split.md)
5. [Electromagnetism](electromagnetism-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Cold-junction compensation](cold-junction-compensation.md)
- [Thermocouple reference function](thermocouple-reference-function.md)
- [Thermocouple voltage calibration](thermocouple-voltage-calibration.md)
