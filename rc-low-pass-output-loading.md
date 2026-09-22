# RC low-pass output loading

↑ **Parent:** [RC low-pass filter](rc-low-pass-filter.md)

A real [electrical load](electrical-load.md) can draw [electric current](electric-current.md) from the [output](output-computing.md). For a load [resistor](resistor.md) $R_L>0$ across the [capacitor](capacitor.md), [Kirchhoff's current law](kirchhoff-node-law.md) instead gives

$$
\frac{v_{\rm in}-v_{\rm out}}R=C\frac{dv_{\rm out}}{dt}+\frac{v_{\rm out}}{R_L}.
$$

Therefore the loaded [continuous-time frequency response](continuous-time-frequency-response.md) is

$$
H_L(\omega)=\frac{K_L}{1+\mathrm i\omega\tau_L},\qquad
K_L=\frac{R_L}{R+R_L},\qquad
\tau_L=\frac{RR_L}{R+R_L}C.
$$

Loading reduces the eventual gain and shortens the [time constant](time-constant.md). With the constructed values and $R_L=10\,\mathrm{k}\Omega$, $K_L\approx0.81967$, $\tau_L\approx84.754\,\mu\mathrm{s}$, and the corner relative to the loaded low-[frequency](frequency.md) gain moves to $1.8778\,\mathrm{kHz}$. A $3\,\mathrm V$ step now approaches $2.4590\,\mathrm V$. A quicker rise alone would conceal the error in the final voltage.

With the ideal input [voltage source](voltage-source.md) set to zero, the [output impedance](output-impedance.md) seen by the [electrical load](electrical-load.md) is

$$
Z_{\rm out}(\omega)=\frac{R}{1+\mathrm i\omega RC}.
$$

This follows from [Thévenin's theorem](thevenin-s-theorem.md): the [resistor](resistor.md) and [capacitor](capacitor.md) are then in parallel. A sufficient small-loading condition is $|Z_L(\omega)|\gg|Z_{\rm out}(\omega)|$ over the [frequencies](frequency.md) of interest. An [oscilloscope](oscilloscope.md) is itself an [electrical load](electrical-load.md): its input [electrical resistance](electrical-resistance.md) and cable or probe [capacitance](capacitance.md) can both change the response. Pure extra parallel [capacitance](capacitance.md) increases $C$ and lowers the corner, whereas a finite parallel [electrical resistance](electrical-resistance.md) gives the different gain-and-corner changes above.

The definition of [input](input-computer-science.md) also matters. If voltage is prescribed inside a source with series [electrical resistance](electrical-resistance.md) $R_s$, the unloaded response to that internal source uses $R+R_s$. If the actual voltage at the filter input terminal is measured, the ratio of output to that measured input still uses $R$. Measuring both terminals avoids mistaking a source setting for the voltage delivered to the filter.

## ↑ Ancestors (6)

1. [RC low-pass filter](rc-low-pass-filter.md)
2. [Low-pass filter](low-pass-filter.md)
3. [Linear filter](linear-filter.md)
4. [Signal processing](signal-processing.md)
5. [Electrical engineering](electrical-engineering-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [RC low-pass filter](rc-low-pass-filter.md)
