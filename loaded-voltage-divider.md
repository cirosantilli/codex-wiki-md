# Loaded voltage divider

↑ **Parent:** [Voltage divider](voltage-divider.md)

Connect a passive [electrical load](electrical-load.md) of [electrical resistance](electrical-resistance.md) $R_L>0$ from the junction to the reference. In the steady [direct current](direct-current.md) model, $R_L$ and $R_2$ share the same [electric potential difference](electric-potential-difference.md) and are connected in parallel. Their equivalent [electrical resistance](electrical-resistance.md) is

$$
R_p=R_2\parallel R_L=\frac{R_2R_L}{R_2+R_L},\qquad
V_{\mathrm{out}}=V_{\mathrm{in}}\frac{R_p}{R_1+R_p}
=\frac{V_{\mathrm{in}}R_2R_L}{R_1R_2+(R_1+R_2)R_L}.
$$

This is the replacement required when a [voltmeter](voltmeter.md) is connected across $R_2$. The inspected teaching guide explicitly models the meter this way.[ET 304A, Lab 4: Voltage Measurements and Meter Loading Effects, pp. 1–2, Figure 1 and equations (1)–(3)](lab-4-voltage-measurements-and-meter-loading-effects-southern-illinois-university-et-304a.md)

The [Kirchhoff's current law](kirchhoff-node-law.md) proof makes the changed assumption visible:

$$
\frac{V_{\mathrm{in}}-V_{\mathrm{out}}}{R_1}
=\frac{V_{\mathrm{out}}}{R_2}+\frac{V_{\mathrm{out}}}{R_L}.
$$

The upper [resistor](resistor.md) carries the sum of the lower and load [electric currents](electric-current.md), so the two original [resistors](resistor.md) no longer have equal [electric currents](electric-current.md). In the stipulated $R_L=10\,\mathrm{k\Omega}$ example, $R_p=5\,\mathrm{k\Omega}$, the upper current is $2/3\,\mathrm{mA}$, and each lower branch carries $1/3\,\mathrm{mA}$.

For a digital [multimeter](multimeter.md) used as a [voltmeter](voltmeter.md), let its input [electrical resistance](electrical-resistance.md) on the selected voltage range be $R_m$. With no other load, set $R_L=R_m$; if an intended load is also present, use $R_L\parallel R_m$ in place of $R_L$. Two instruments connected simultaneously add two branches. Their ideal indicated value equals the voltage of this altered circuit; [voltmeter loading](voltmeter-loading.md) can exist even with perfect [measurement calibration](measurement-calibration.md). Real readout additionally has [measurement uncertainty](measurement-uncertainty.md), offsets, and finite resolution. Consult the actual range and input specifications rather than assigning every digital [multimeter](multimeter.md) the same $R_m$.

For an [oscilloscope](oscilloscope.md), the resistance-only model applies to settled [direct current](direct-current.md) with a compatible input coupling setting. The [oscilloscope](oscilloscope.md) input and cable also have [capacitance](capacitance.md); changing [signals](signal.md) can therefore have loading that depends on [frequency](frequency.md). A probe changes the impedance seen at its tip and the relation between tip voltage and displayed voltage; use the probe-and-input combination's specification and attenuation setting. NJIT's guide models the parallel [electrical resistance](electrical-resistance.md) and [capacitance](capacitance.md) and adjusts probe compensation with a square-wave readout.[Lab 7: Input Impedance of an Oscilloscope and the Scope Probe, Introduction, Figure 5 and probe adjustment; Laboratory §1(a)–(c)](lab-7-input-impedance-of-an-oscilloscope-and-the-scope-probe-njit-ece-291.md)

## ↑ Ancestors (3)

1. [Voltage divider](voltage-divider.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Resistor tolerance](resistor-tolerance.md)
- [Voltage divider teaching experiment](voltage-divider-teaching-experiment.md)
- [Voltmeter loading](voltmeter-loading.md)
