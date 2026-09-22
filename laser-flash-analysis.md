# Laser flash analysis

↑ **Parent:** [Thermal diffusivity](thermal-diffusivity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laser_flash_analysis)

[Laser flash analysis](laser-flash-analysis.md) measures [thermal diffusivity](thermal-diffusivity.md) by heating one face of a specimen briefly and recording the opposite face's [temperature](temperature-split.md) rise. The original 1961 experiment used a flash tube rather than a [laser](laser-split.md): a blackened thin metal specimen sat in an opaque ceramic holder, with [thermocouple](thermocouple.md) wires pressed against its rear face. An amplifier, oscilloscope and camera recorded the signal. Uniform front illumination and the black coating promoted uniform absorption; the opaque low-[thermal conductivity](thermal-conductivity.md) holder blocked direct rear illumination and reduced edge losses. The delayed rear response reveals internal [thermal conduction](thermal-conduction.md) rather than direct heating of the sensor. [Parker, Jenkins, Butler and Abbott, pp. 1682–1683, Experimental Procedure and figure 3: holder, flash, thermocouple and recording chain](flash-method-of-determining-thermal-diffusivity-heat-capacity-and-thermal-conductivity-by-w-j-parker-and-others.md)

A modern version uses a [laser](laser-split.md) or flash lamp, a specimen of measured thickness $L$, controlled initial [temperature](temperature-split.md), and a rear-facing [infrared](infrared.md) detector with a synchronized recorder. The readout is a [temperature](temperature-split.md) rise versus time, starting from a pre-pulse baseline. [Thermal conductivity](thermal-conductivity.md) additionally requires [mass density](density.md) and [specific heat capacity](specific-heat-capacity.md); it is not obtained from timing alone. [NETZSCH, Principle of the LFA Method: opposite-face infrared readout and conductivity product](light-and-laser-flash-analyzers-by-netzsch-analyzing-and-testing.md)

Under ideal one-dimensional, insulated, constant-property assumptions, instantaneous uniform absorption in a very thin front layer gives the normalized rear rise

$$
R(t)=\frac{T(L,t)-T_0}{T_\infty-T_0}
=1+2\sum_{n=1}^{\infty}(-1)^n
\exp\left(-\frac{n^2\pi^2\alpha t}{L^2}\right),\qquad t>0.
$$

Here $T_0$ is the initial uniform [temperature](temperature-split.md) and $T_\infty$ is the final uniform [temperature](temperature-split.md) in the insulated model. Fitting this curve estimates [thermal diffusivity](thermal-diffusivity.md); each term has the same $\alpha K_n^2$ decay as the insulated-bar [Fourier modes](fourier-mode.md). Equivalently, the half-rise time $t_{1/2}$ solves $R(t_{1/2})=1/2$. Writing $s=\alpha t/L^2$, the series gives $s_{1/2}\approx0.13879$, hence

$$
\alpha\approx0.13879\frac{L^2}{t_{1/2}}.
$$

This coefficient comes from the stated ideal [heat equation](heat-equation.md) solution, not from an empirical sensor calibration. It has been independently checked by solving the series equation. Absolute absorbed pulse [energy](energy-split.md) cancels from the normalized curve; determining [heat capacity](heat-capacity.md) from its absolute height needs additional information. [Carr, section 2, equations (4)–(7): rear-face series, half-rise time and corrected dimensionless constant 1.370](rear-surface-integral-method-for-calculating-thermal-diffusivity-from-laser-flash-experiments-by-elliot-j-carr.md)

Parker and colleagues identify finite flash duration, [heat](heat-split.md) loss, nonuniform illumination, recording bandwidth and electrical interference as practical limits. A specimen too thin responds during the pulse; one too thick allows losses before the rear rise finishes. They shielded the electrical chain and recorded a baseline; their reported tests were preliminary metal measurements near ambient and moderately elevated [temperatures](temperature-split.md). [Parker and colleagues, pp. 1682–1684: signal distortion, shielding, thickness tradeoff and Conclusions](flash-method-of-determining-thermal-diffusivity-heat-capacity-and-thermal-conductivity-by-w-j-parker-and-others.md)

Useful additional controls are to measure thickness at several points, verify the recorder's time scale and detector response independently, record a no-pulse baseline, and repeat at different pulse [energies](energy-split.md) while avoiding [phase transitions](phase-transition.md). Compare different thicknesses of the same homogeneous material: ideal half-rise times scale as $L^2$. Failure of these checks can expose finite-pulse effects, sensor delay, optical transmission, coating storage or edge losses; a thickness error is especially consequential because the inferred [thermal diffusivity](thermal-diffusivity.md) depends on $L^2$. These are proposed diagnostic controls, not invented measurements. When the pulse is not short or the sample exchanges appreciable [heat](heat-split.md) with its surroundings, fit a model that includes those effects instead of applying the ideal half-rise coefficient unchanged.

## ↑ Ancestors (8)

1. [Thermal diffusivity](thermal-diffusivity.md)
2. [Thermal conduction](thermal-conduction.md)
3. [Heat](heat-split.md)
4. [Thermodynamics](thermodynamics-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Ångström periodic heating method](angstrom-periodic-heating-method.md)
- [Laser flash analysis](laser-flash-analysis.md)
