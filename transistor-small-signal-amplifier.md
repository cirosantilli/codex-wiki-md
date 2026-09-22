# Transistor small-signal amplifier

↑ **Parent:** [Transistor](transistor.md)

An original teaching model exposes the roles of input loading, output loading and the supply. Choose a [small-signal model](small-signal-model.md) with positive input [electrical resistance](electrical-resistance.md) $r_i$, [transconductance](transconductance.md) $g_m>0$, and output [electrical resistance](electrical-resistance.md) $r_o>0$. Its controlled output [current source](current-source.md) draws $g_mv_i$ from the output node toward the reference node. This chosen sign gives an inverting [voltage gain](voltage-gain.md); it is not the historical contact circuit's sign convention.

Assume a fixed [operating point](operating-point.md), negligible reverse coupling, a [frequency](frequency.md) range where coupling [capacitors](capacitor.md) pass the [signal](signal.md), and negligible other [capacitances](capacitance.md) and transit delays. A collector [resistor](resistor.md) $R_D$ connects the output to a steady ideal supply $V_{DD}$; an external [electrical load](electrical-load.md) $R_L$ is coupled through a [capacitor](capacitor.md), so it draws no [direct current](direct-current.md). The input source has series [electrical resistance](electrical-resistance.md) $R_s$. All voltages below are small departures from the [operating point](operating-point.md). An ideal fixed supply has zero incremental voltage and therefore becomes the reference node in the [small-signal model](small-signal-model.md).

Define $R_O=R_D\parallel r_o$ and $R_P=R_O\parallel R_L$, where $a\parallel b=ab/(a+b)$. Input voltage division and output [Kirchhoff's current law](kirchhoff-node-law.md) give

$$
v_i=\frac{r_i}{R_s+r_i}v_s,\qquad
\frac{v_o}{R_D}+\frac{v_o}{r_o}+\frac{v_o}{R_L}+g_mv_i=0.
$$

Consequently the port [voltage gain](voltage-gain.md), overall source-to-output [voltage gain](voltage-gain.md), and load [current gain](current-gain.md) magnitudes are

$$
A_v=\frac{v_o}{v_i}=-g_mR_P,\qquad
\frac{v_o}{v_s}=-g_mR_P\frac{r_i}{R_s+r_i},\qquad
|A_i|=\frac{|v_o|/R_L}{|v_i|/r_i}=g_mr_i\frac{R_O}{R_O+R_L}.
$$

This [current gain](current-gain.md) uses load [electric current](electric-current.md), not all the controlled-source [electric current](electric-current.md). It is also a different port definition from the historical emitter-to-collector [current gain](current-gain.md). Larger $R_s$ attenuates the input; smaller $R_L$ attenuates the output.

For a [sinusoid](sinusoid.md) input [signal](signal.md), use [root mean square](root-mean-square.md) voltages. The [power gain](power-gain.md) from accepted input [signal](signal.md) [power](power.md) $P_i=v_i^2/r_i$ to useful load [power](power.md) $P_L=v_o^2/R_L$ is

$$
G_P=\frac{P_L}{P_i}
=g_m^2r_i\frac{R_O^2R_L}{(R_O+R_L)^2}.
$$

Unlike $|A_i|$, this tends to zero as either $R_L\to0$ or $R_L\to\infty$. Differentiation gives

$$
\frac{dG_P}{dR_L}=g_m^2r_iR_O^2\frac{R_O-R_L}{(R_O+R_L)^3},\qquad
G_{P,\max}=\frac{g_m^2r_iR_O}{4}\quad\text{at }R_L=R_O.
$$

Thus matching the output [electrical load](electrical-load.md) maximizes delivered [power](power.md) in this unilateral resistive model. For fixed source voltage, input loading multiplies $P_L$ by $[r_i/(R_s+r_i)]^2$; the accepted-input [power gain](power-gain.md) above excludes the loss in $R_s$.

Choose $r_i=R_s=1\,\mathrm{k\Omega}$, $g_m=2\,\mathrm{mS}$, $r_o=20\,\mathrm{k\Omega}$, and $R_D=2\,\mathrm{k\Omega}$. Then $R_O=20/11\,\mathrm{k\Omega}$. With $R_L=2\,\mathrm{k\Omega}$ and $v_s=20\,\mathrm{mV}$ [root mean square](root-mean-square.md), the input is $10\,\mathrm{mV}$ and the inverted output has magnitude $19.0476\,\mathrm{mV}$ [root mean square](root-mean-square.md). Hence $P_i=0.100\,\mathrm{\mu W}$ and $P_L=0.181406\,\mathrm{\mu W}$: $G_P=1.81406$. These are calculated values of the chosen model, not historical measurements.

With the same parameters but $R_L=100\,\Omega$, $|A_i|=1.89573$ while $G_P=0.359381<1$. At $R_L=10\,\mathrm{k\Omega}$, $|A_v|=3.07692$ while $G_P=0.946746<1$. Neither [current gain](current-gain.md) nor [voltage gain](voltage-gain.md) alone establishes [power gain](power-gain.md).

<a id="image-chosen-transistor-model-transconductance-load-and-supply"></a>
![](transistor-controlled-source-load-and-gain.png)

**[Figure 4](#image-chosen-transistor-model-transconductance-load-and-supply). Chosen transistor model: transconductance, load and supply**. [Source](transistor-controlled-source-load-and-gain.py). Original calculated illustration. Top: incremental [electrical circuit](electrical-circuit-split.md). Lower left: the no-external-load [direct current](direct-current.md) load line intersects three chosen local device curves. Lower right: port [voltage gain](voltage-gain.md), load [current gain](current-gain.md) and [power gain](power-gain.md) as $R_L$ changes. All parameters are stipulated teaching values.

For the [direct current](direct-current.md) load line in the figure, choose $V_{DD}=6\,\mathrm V$, $I_Q=1\,\mathrm{mA}$ and $V_Q=4\,\mathrm V$, consistent with $V_Q=V_{DD}-R_DI_Q$. Locally extend the model as $I=I_Q+g_mv_i+(V-V_Q)/r_o$. With the external [electrical load](electrical-load.md) isolated at [direct current](direct-current.md), its intersection with $I=(V_{DD}-V)/R_D$ is $V=V_Q-g_mR_Ov_i$. Keeping $|v_o|$ small compared with the available voltage headroom is essential; extrapolation to arbitrarily large [signals](signal.md) would be unphysical.

At the chosen [operating point](operating-point.md) the collector supply delivers $V_{DD}I_Q=6\,\mathrm{mW}$: $2\,\mathrm{mW}$ is dissipated in $R_D$ and $4\,\mathrm{mW}$ in the output device. Under a small [signal](signal.md), that [energy](energy-split.md) flow is redistributed to provide load [power](power.md). The incremental controlled [current source](current-source.md) hides the supply's steady [energy](energy-split.md) flow; it does not create [energy](energy-split.md). A real complete [amplifier](amplifier.md) also needs its input [biasing](biasing.md) network and has further losses. This calculation establishes neither its total efficiency nor a universal law for [point-contact transistors](point-contact-transistor.md).

## ↑ Ancestors (4)

1. [Transistor](transistor.md)
2. [Semiconductor](semiconductor-split.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)
