# Voltage divider

↑ **Parent:** [Electrical engineering](electrical-engineering-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Voltage_divider)

A voltage divider uses two [resistors](resistor.md) connected in series to obtain a fraction of an applied [electric potential difference](electric-potential-difference.md). Let the upper [electrical resistance](electrical-resistance.md) be $R_1>0$, the lower one $R_2>0$, and the input be $V_{\mathrm{in}}=V_s$ relative to a common [electrical reference potential](electrical-reference-potential.md). The output is the junction's [electric potential difference](electric-potential-difference.md) relative to that same reference, across $R_2$. The familiar ratio assumes zero output [electric current](electric-current.md): no external [electrical load](electrical-load.md) draws from the junction. In a steady [direct current](direct-current.md) model with fixed [resistors](resistor.md) obeying [Ohm's law](ohm-s-law.md) and an ideal [voltage source](voltage-source.md),

$$
I=\frac{V_{\mathrm{in}}}{R_1+R_2},\qquad
V_0=IR_2=V_{\mathrm{in}}\frac{R_2}{R_1+R_2}.
$$

Here $V_0$ is the [open-circuit voltage](open-circuit-voltage.md); $R_1,R_2$ correspond to $R_a,R_b$ in the header formula. With no junction branch, [Kirchhoff's current law](kirchhoff-node-law.md) makes the same [electric current](electric-current.md) pass through both [resistors](resistor.md), and [Ohm's law](ohm-s-law.md) gives the two voltage drops. For $V_s\ne0$, division gives $V_0/V_s=R_2/(R_1+R_2)$; if $V_s=0$, the predicted output is zero but this ratio is undefined.

An original stipulated example has $R_1=R_2=10\,\mathrm{k\Omega}$ and $V_{\mathrm{in}}=10\,\mathrm V$. With zero output [electric current](electric-current.md), $I=0.5\,\mathrm{mA}$ and $V_0=5\,\mathrm V$. An attached $10\,\mathrm{k\Omega}$ [electrical load](electrical-load.md) instead gives $V_{\mathrm{out}}=10/3\,\mathrm V$; a $1\,\mathrm{M\Omega}$ load gives $V_{\mathrm{out}}=1000/201\,\mathrm V=4.975124378\ldots\,\mathrm V$. These are exact model predictions, not measured readings or specifications of a particular [multimeter](multimeter.md) or [oscilloscope](oscilloscope.md).

<a id="image-the-same-voltage-divider-has-three-different-predicted-outputs-as-the-attached-load-changes"></a>
![](voltage-divider-load-and-readout-comparison.png)

**[Figure 12](#image-the-same-voltage-divider-has-three-different-predicted-outputs-as-the-attached-load-changes). The same voltage divider has three different predicted outputs as the attached load changes**. [Source](voltage-divider-load-and-readout-comparison.py). Original circuit and readout comparison for ideal $10\,\mathrm V$ input and two $10\,\mathrm{k\Omega}$ resistors. Each finite $R_L$ connects across $R_2$; the displayed numbers are model predictions with ideal readout, not experimental data.

The divider is useful for scaling a voltage or converting a change in a sensor's [electrical resistance](electrical-resistance.md) into an [electric potential difference](electric-potential-difference.md). Its beauty is also its trap: multiplying both [electrical resistances](electrical-resistance.md) by the same positive factor preserves the unloaded ratio, but changes the effect of any fixed [electrical load](electrical-load.md). A divider therefore supplies a predictable ratio under specified loading conditions; it is not a source that maintains that voltage for arbitrary output [electric currents](electric-current.md). A [Wheatstone bridge](wheatstone-bridge.md) compares two divider junctions, while [Thévenin's theorem](thevenin-s-theorem.md) describes the divider's response to many different loads.

**Table of contents**

- [Loaded voltage divider](loaded-voltage-divider.md)
- [Voltage divider loading error](voltage-divider-loading-error.md)
- [Voltage divider teaching experiment](voltage-divider-teaching-experiment.md)

## ↑ Ancestors (2)

1. [Electrical engineering](electrical-engineering-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Direct current](direct-current.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/section-a/a3/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/section-c/11/solution.md)
- [RC low-pass frequency response](rc-low-pass-frequency-response.md)
- [RC low-pass laboratory](rc-low-pass-laboratory.md)
- [Resistor tolerance](resistor-tolerance.md)
- [Thermal noise loading](thermal-noise-loading.md)
- [Thermopile series voltage](thermopile-series-voltage.md)
- [Thévenin divider example](thevenin-divider-example.md)
- [Thévenin load response](thevenin-load-response.md)
- [Thévenin's theorem](thevenin-s-theorem.md)
- [Vibrating-sample magnetometer](vibrating-sample-magnetometer.md)
- [Voltage divider teaching experiment](voltage-divider-teaching-experiment.md)
- [Wheatstone bridge balance](wheatstone-bridge-balance.md)
- [Wheatstone bridge detector loading](wheatstone-bridge-detector-loading.md)
- [Wien bridge](wien-bridge.md)
