# Thermocouple voltage calibration

↑ **Parent:** [Thermocouple](thermocouple.md)

[Thermocouple voltage calibration](thermocouple-voltage-calibration.md) relates an actual assembled sensor's [electromotive force](electromotive-force.md) to independently established junction [temperatures](temperature-split.md). It must be distinguished from selecting a nominal letter-type conversion curve. In [Thermocouples Calibrations Services by National Institute of Standards and Technology](thermocouples-calibrations-services-by-national-institute-of-standards-and-technology.md) (opening method description and bath-calibration table), NIST describes comparison with a maintained reference [thermocouple](thermocouple.md), comparison with a standard platinum [resistance thermometer](resistance-thermometer.md) in controlled [heat baths](heat-bath.md), and fixed-point calibration at the freezing points of zinc, aluminum, silver and gold on the [International Temperature Scale of 1990](international-temperature-scale-of-1990.md). These are independent thermal references, unlike a test that checks only a voltage-input circuit.[method description; table for base-metal thermocouples compared with an SPRT in a temperature-controlled bath](thermocouples-calibrations-services-by-national-institute-of-standards-and-technology.md)

For a concrete electrical check, the SCC-TC guide describes shorting the input after 30 minutes of powered operation and adjusting its offset to a zero-voltage readout. Its separate calibrator procedure requires equal connection [temperatures](temperature-split.md) at the calibrator and module, measures the supplied voltage, converts it to [temperature](temperature-split.md), and compares with the calibrator setting. Such an injected-signal test checks the readout chain; it does not expose a real measuring junction to an independently known bath [temperature](temperature-split.md).[p. 9, Calibrating System Offsets; Calibrating the SCC-TC0X Using a Thermocouple Calibrator](scc-tc-series-thermocouple-input-modules-user-guide-by-national-instruments.md)

Useful additional checks follow from the model: log the raw voltage, the reference [temperature](temperature-split.md), and the final inferred [temperature](temperature-split.md) separately; hold $T_h$ stable while changing $T_c$ and test whether [cold-junction compensation](cold-junction-compensation.md) preserves the inferred $T_h$; compare against an independent [thermometer](thermometer.md) at several stable [heat bath](heat-bath.md) settings. Check immersion and repeatability instead of assuming a steady display establishes [thermal equilibrium](thermal-equilibrium-split.md). These are proposed diagnostic checks, not new experimental results. The equal-[temperature](temperature-split.md) and polarity controls are already described under [Seebeck effect](seebeck-effect.md).

Limits arise separately from the [thermocouple reference function](thermocouple-reference-function.md), sensor-wire changes, thermal contact, terminal [temperature](temperature-split.md) differences, and the voltage-input circuit. In particular, the SCC-TC guide warns of connector-to-module [temperature gradients](temperature-gradient.md) and voltage drops caused by the fault-detection [electric current](electric-current.md) flowing through lead [electrical resistance](electrical-resistance.md).[p. 6, Uncompensated Connectors and Accuracy; p. 7, Errors Due to Open-Thermocouple Detection Circuitry](scc-tc-series-thermocouple-input-modules-user-guide-by-national-instruments.md) A fitted curve or compensation algorithm cannot make all these errors vanish. No single accuracy is assigned to every [thermocouple](thermocouple.md).

**Table of contents**

- [Thermocouple reference function](thermocouple-reference-function.md)

## ↑ Ancestors (7)

1. [Thermocouple](thermocouple.md)
2. [Seebeck effect](seebeck-effect.md)
3. [Thermoelectric effect](thermoelectric-effect-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Thermocouple voltage calibration](thermocouple-voltage-calibration.md)
