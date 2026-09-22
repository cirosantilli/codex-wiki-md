# Thermopile radiative measurement

↑ **Parent:** [Thermopile](thermopile.md)

PASCO's documented lamp experiment connects a TD-8553 [thermopile](thermopile.md) sensor to a millivoltmeter and places it level with a lamp filament along a meter stick. Lamp and detector axes are aligned. With the lamp off, readings at several positions establish an average ambient [thermal radiation](thermal-radiation.md) background. With the lamp on at a fixed supply setting, detector readings at different distances are compared after background subtraction. Between readings, a reflective shield prevents the detector warming; its shutter also protects the reference junction when idle. Moving the shutter can move the sensor, so fixed geometry matters. The manual's lamp limits must be followed.[p. 1, Radiation Sensor; pp. 9–11, Experiment 2, Fig. 2.1, procedure and calculations: alignment, lamp-off ambient readings, heat shield and distance comparison](thermal-radiation-system-instruction-manual-and-experiment-guide-td-8553-td-8554a-and-td-8555-by-pasco-scientific.md)

This protocol tests whether the background-corrected [electric potential difference](electric-potential-difference.md) approximately follows the [inverse-square law](inverse-square-law.md) over a suitable distance range. It is a relative [electromagnetic radiation](electromagnetic-radiation-split.md) measurement; those readings alone do not calibrate absorbed [power](power.md) in [watts](watt.md). The manual treats the filament as an approximate [point source](point-source.md).[p. 3, Stefan-Boltzmann Lamp; p. 11, Experiment 2 calculations: point-source approximation and comparison against inverse squared distance](thermal-radiation-system-instruction-manual-and-experiment-guide-td-8553-td-8554a-and-td-8555-by-pasco-scientific.md)

For an absolute calibration, independently known absorbed [power](power.md) and a monitored reference [temperature](temperature-split.md) would be needed. A useful additional control is to repeat a fixed detector position before and after a distance sweep: disagreement reveals possible drift. These additions test the measurement chain rather than assuming that background subtraction fixes every error. A finite source, changing illuminated [area](surface-area.md), reflections, changing reference [temperature](temperature-split.md), and insufficient settling can alter the measured dependence. In particular, the [time constant](time-constant.md) in [thermopile thermal response](thermopile-thermal-response.md) explains why a quick reading and a settled reading may differ. The detector infers its own absorber [temperature](temperature-split.md) difference; inferring the source's [temperature](temperature-split.md) additionally requires its [emissivity](emissivity.md), optical geometry and an appropriate [thermal radiation](thermal-radiation.md) model.

## ↑ Ancestors (8)

1. [Thermopile](thermopile.md)
2. [Thermocouple](thermocouple.md)
3. [Seebeck effect](seebeck-effect.md)
4. [Thermoelectric effect](thermoelectric-effect-split.md)
5. [Electromagnetism](electromagnetism-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
