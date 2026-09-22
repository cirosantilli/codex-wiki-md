# Cold-junction compensation

↑ **Parent:** [Thermocouple reference junction](thermocouple-reference-junction.md)

[Cold-junction compensation](cold-junction-compensation.md) converts a reading with reference [temperature](temperature-split.md) $T_c$ into the equivalent reading for a chosen standard reference. Define the [thermocouple reference function](thermocouple-reference-function.md) $F(T)=E(T,0)$, where $0$ means $0\,{}^\circ\mathrm C$, not absolute zero. Additivity of the [definite integral](definite-integral.md) gives

$$
E(T_h,T_c)=F(T_h)-F(T_c),\qquad
F(T_h)=V_{\rm raw}+F(T_c),\qquad
T_h=F^{-1}\!\bigl(V_{\rm raw}+F(T_c)\bigr).
$$

The final [inverse function](inverse-function.md) requires a suitable one-to-one calibration interval. A terminal [thermometer](thermometer.md) supplies $T_c$ independently; the raw [thermocouple](thermocouple.md) [electric potential difference](electric-potential-difference.md) supplies only the difference of the two reference-function values. In general, first converting $V_{\rm raw}$ to a [temperature](temperature-split.md) and then adding $T_c$ is wrong, because the [thermocouple reference function](thermocouple-reference-function.md) need not be linear. The SCC-TC manual explicitly adds the reference-equivalent voltage before its final voltage-to-[temperature](temperature-split.md) conversion.[pp. 5–6, Scaling Voltage Measurements, steps 1–5](scc-tc-series-thermocouple-input-modules-user-guide-by-national-instruments.md)

For a stipulated model only, take $S_A-S_B=40\,\mu\mathrm{V/K}$ throughout the interval. No actual material pair is assigned this constant. Because [degree Celsius](degree-celsius.md) differences have the same numerical size as [kelvin](kelvin.md) differences,

$$
T_h=80\,{}^\circ\mathrm C,\quad T_c=20\,{}^\circ\mathrm C
\quad\Longrightarrow\quad
V_{\rm raw}=(40\,\mu\mathrm{V/K})(60\,\mathrm K)=2.4\,\mathrm{mV}.
$$

In this model $F(20)=0.8\,\mathrm{mV}$ and $F(80)=3.2\,\mathrm{mV}$. Adding the $0.8\,\mathrm{mV}$ correction produces $3.2\,\mathrm{mV}$, whose inverse calibration gives $80\,{}^\circ\mathrm C$. Applying the zero-reference calibration directly to $2.4\,\mathrm{mV}$ would instead display $60\,{}^\circ\mathrm C$.

Now physically change only the reference [temperature](temperature-split.md) to $30\,{}^\circ\mathrm C$, leaving the measuring junction at $80\,{}^\circ\mathrm C$. The raw reading becomes $2.0\,\mathrm{mV}$; the correction becomes $F(30)=1.2\,\mathrm{mV}$, so the corrected total stays $3.2\,\mathrm{mV}$. Physically changing the reference changes the measured [electric potential difference](electric-potential-difference.md). Adding a software correction changes its interpretation and leaves the raw reading intact. If the actual reference is $30\,{}^\circ\mathrm C$ but the software still assumes $20\,{}^\circ\mathrm C$, this model displays $70\,{}^\circ\mathrm C$.

<a id="image-adding-the-reference-equivalent-voltage-before-inverting-the-thermocouple-reference-function"></a>
![](thermocouple-reference-compensation-calibration.png)

**[Figure 6](#image-adding-the-reference-equivalent-voltage-before-inverting-the-thermocouple-reference-function). Adding the reference-equivalent voltage before inverting the thermocouple reference function**. Calculated constant-[Seebeck coefficient](seebeck-coefficient.md)-difference example only. The zero-reference line $F(T)=E(T,0)$ and the $20\,{}^\circ\mathrm C$ raw-reading line differ by $F(20)=0.8\,\mathrm{mV}$. At $T_h=80\,{}^\circ\mathrm C$, adding that correction takes $2.4$ to $3.2\,\mathrm{mV}$. Changing the reference to $30\,{}^\circ\mathrm C$ changes the raw reading and the correction in opposite directions. Real calibration curves need not be straight.

An actual implementation in [FP-TC-120 and cFP-TC-120 Operating Instructions by National Instruments](fp-tc-120-and-cfp-tc-120-operating-instructions-by-national-instruments.md) (p. 7, Cold-Junction Compensation) uses terminal-mounted [temperature](temperature-split.md) sensors, reports their reading as “CJ Temperature”, and enables compensation in [temperature](temperature-split.md) mode but not voltage mode. This makes the distinction between a raw voltage readout and a compensated [temperature](temperature-split.md) readout observable. The specified reference-sensor range also produces an out-of-range indication: a calculated number outside a supported range is not a validated measurement.[p. 7, Cold-Junction Compensation: mode selection, CJ Temperature and out-of-range reporting](fp-tc-120-and-cfp-tc-120-operating-instructions-by-national-instruments.md)

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

- [Cold-junction compensation](cold-junction-compensation.md)
- [Thermocouple reference junction](thermocouple-reference-junction.md)
- [Thermocouple voltage calibration](thermocouple-voltage-calibration.md)
