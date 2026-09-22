# Diode characteristic measurement

↑ **Parent:** [Diode](diode.md)

The New Jersey Institute of Technology laboratory uses a [silicon](silicon.md) 1N4148 [diode](diode.md). For its forward [current-voltage characteristic](current-voltage-characteristic.md), the supply operates in current-source mode; a benchtop [voltmeter](voltmeter.md) independently reads the [diode](diode.md) [electric potential difference](electric-potential-difference.md). Small [electric current](electric-current.md) steps resolve the steep branch. For reverse measurements, a sensitive [ammeter](ammeter.md) sits in series; the handout suggests a $10$–$100\,\mathrm{k\Omega}$ series [resistor](resistor.md). Reversing the applied polarity supplies the comparison. Meter placement must avoid counting the [voltmeter](voltmeter.md)'s own [electric current](electric-current.md), and the zero reading may have an offset. The same [diode](diode.md) is then measured with an Agilent U2722A source measure unit for graphical comparison.[Part B, Experiments with Semiconductor Diodes, items 1 and 2(a): preparation, current control, independent voltage readout, reverse series resistor and same-device comparison](part-b-semiconductor-devices-diodes-1-by-new-jersey-institute-of-technology.md)

The prescribed analysis uses a [logarithmic scale](logarithmic-scale.md) for forward [electric current](electric-current.md) to infer $I_S$ and $n$ from the straight region. Large-[electric current](electric-current.md) departures can indicate series [electrical resistance](electrical-resistance.md). The handout cautions that the accessible range may not determine it precisely; meter loading also matters. This is a measurement procedure, without a published set of device readings.[Experiments with Semiconductor Diodes, item 1, parameter extraction and high-current trend-line limitations; Report and Analysis](part-b-semiconductor-devices-diodes-1-by-new-jersey-institute-of-technology.md)

The reason for the [logarithmic scale](logarithmic-scale.md) follows directly from the [Shockley diode equation](shockley-diode-equation.md). If $I_D\gg I_S$ and series [electrical resistance](electrical-resistance.md) is negligible,

$$
\ln\left(\frac{I_D}{I_0}\right)\approx\ln\left(\frac{I_S}{I_0}\right)+\frac{V_D}{nV_T},
$$

where $I_0>0$ is a fixed reference [electric current](electric-current.md) making the [logarithm](logarithm.md) dimensionless. The slope is $1/(nV_T)$, so extracting $n$ needs the junction [temperature](temperature-split.md). Fitting only an appropriate [interval](interval-mathematics.md) matters: a straight-looking subset cannot establish the model at all [electric currents](electric-current.md).

## ↑ Ancestors (6)

1. [Diode](diode.md)
2. [Electrical circuit](electrical-circuit-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
