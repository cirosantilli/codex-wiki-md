<h1 id="thevenin-measurement-experiment">Thévenin measurement experiment</h1>

↑ **Parent:** [Thévenin's theorem](thevenin-s-theorem.md)

An authored teaching experiment uses an adjustable steady-voltage supply, a digital multimeter, fixed [resistors](resistor.md), and a $10\,\mathrm{k\Omega}$ [potentiometer](potentiometer.md) or resistance decade box. Its original circuit uses a $10\,\mathrm V$ supply and $3.3$, $6.8$, and $4.7\,\mathrm{k\Omega}$ [resistors](resistor.md); the student compares $8.2$ and $2.2\,\mathrm{k\Omega}$ [electrical loads](electrical-load.md). The readout is load voltage, recorded against prediction and deviation. The student then removes the [electrical load](electrical-load.md) to measure the [open-circuit voltage](open-circuit-voltage.md), disconnects the supply and substitutes a wire to measure the [Thévenin resistance](thevenin-resistance.md) with the multimeter's resistance mode, and restores the supply for an independent method: adjust the variable [electrical load](electrical-load.md) until the [voltmeter](voltmeter.md) reads half the unloaded voltage. Finally the student builds the equivalent and repeats both load measurements. Its tables are blank recording forms, not reported observations. [Laboratory Manual for DC Electrical Circuit Analysis by James M. Fiore, version 1.4.3, experiment 11, printed pp. 52–55: Equipment, Procedure 1–10, Tables 11.1–11.3](laboratory-manual-for-dc-electrical-circuit-analysis-by-james-m-fiore.md)

The half-voltage inference assumes negligible [voltmeter loading](voltmeter-loading.md) and positive $R_{\mathrm{th}}$. A finite [voltmeter](voltmeter.md) input [electrical resistance](electrical-resistance.md) $R_m$ actually gives an apparent unloaded reading

$$
V_m=V_{\mathrm{oc}}\frac{R_m}{R_{\mathrm{th}}+R_m}.
$$

When the same [voltmeter](voltmeter.md) remains connected across a variable [electrical load](electrical-load.md) $R_L$, the network sees $R_p=R_LR_m/(R_L+R_m)$. Setting its reading to $V_m/2$, rather than to the true $V_{\mathrm{oc}}/2$, gives

$$
R_L=\frac{R_{\mathrm{th}}R_m}{R_{\mathrm{th}}+R_m}.
$$

Thus the uncorrected half-reading method underestimates positive $R_{\mathrm{th}}$. In the original $12\,\mathrm V$ example, a stipulated $R_m=10\,\mathrm{k\Omega}$ gives $V_m=120/17\,\mathrm V\approx7.059\,\mathrm V$ and half-reading load $R_L=20/17\,\mathrm{k\Omega}\approx1.176\,\mathrm{k\Omega}$, instead of $\tfrac43\,\mathrm{k\Omega}$. These are model predictions for a deliberately loading meter, not the specification or observed readout of the source experiment's instrument.

Finite readings can also estimate the terminal line without a physical short. For two distinct load settings with corrected delivered [electric currents](electric-current.md) $I_1,I_2$ and terminal voltages $V_1,V_2$,

$$
R_{\mathrm{th}}=\frac{V_1-V_2}{I_2-I_1},\qquad
V_{\mathrm{oc}}=V_1+I_1R_{\mathrm{th}}.
$$

If the [voltmeter](voltmeter.md) remains across each [electrical load](electrical-load.md), the delivered [electric current](electric-current.md) is $I_k=V_k(1/R_{L,k}+1/R_m)$, including the meter branch. Omitting it biases the inferred slope.

Useful additional controls are to measure each [resistor](resistor.md) separately before assembly, verify terminal polarity, repeat an earlier load setting to detect supply drift, and compare a third setting with the inferred [Thévenin terminal response](thevenin-terminal-response.md). These are proposed controls, not reported outcomes of the source experiment. Closely spaced [electric currents](electric-current.md) make the slope estimate sensitive to voltage resolution and [measurement error](measurement-error.md); widely separated settings may trigger source current limiting or [Joule heating](joule-heating.md) that changes [electrical resistance](electrical-resistance.md). Lead and contact [electrical resistance](electrical-resistance.md), meter input uncertainty and rounding limit the inference. An [ohmmeter](ohmmeter.md) injects its own test [electric current](electric-current.md); its reading on a powered network is not the suppressed-network ratio. Measurements with independent sources physically removed do not characterize an active [dependent electrical source](dependent-electrical-source.md) whose control or supply has also been disconnected.

## ↑ Ancestors (3)

1. [Thévenin's theorem](thevenin-s-theorem.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Battery voltage measurement experiment](battery-voltage-measurement-experiment.md)
- [Potentiometer](potentiometer.md)
