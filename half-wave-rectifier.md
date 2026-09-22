# Half-wave rectifier

↑ **Parent:** [Rectifier](rectifier.md)

A [half-wave rectifier](half-wave-rectifier.md) with one [diode](diode.md) and a [resistor](resistor.md) load passes one half of each input cycle.[The Junction Diode, §1.12.1, printed p. 30: alternate-half-cycle conduction into a resistor load](the-junction-diode-by-w-marshall-leach-jr.md)

For an original ideal example, let an ideal [voltage source](voltage-source.md) supply the [sinusoid](sinusoid.md) $v_S(t)=V_p\sin(\omega t)$, with $V_p=5\,\mathrm V$ and [angular frequency](angular-frequency.md) $\omega>0$. Connect its positive reference terminal to the [diode anode](diode-anode.md), the [diode cathode](diode-cathode.md) to the upper terminal of a load [resistor](resistor.md) with [electrical resistance](electrical-resistance.md) $R_L=1\,\mathrm{k\Omega}$, and the lower terminal to the source return. Let $v_L$ be the upper-minus-lower load [electric potential difference](electric-potential-difference.md), and $i_L$ the downward load [electric current](electric-current.md). Assume the [ideal diode model](ideal-diode-model.md), zero source [electrical resistance](electrical-resistance.md), and no filter [capacitor](capacitor.md), [inductor](inductor.md) or switching delay.

<a id="image-an-ideal-half-wave-rectifier-selects-the-positive-half-cycle"></a>
![](half-wave-rectifier-circuit-and-waveform.png)

**[Figure 2](#image-an-ideal-half-wave-rectifier-selects-the-positive-half-cycle). An ideal half-wave rectifier selects the positive half-cycle**. Original schematic and calculated load [electric potential difference](electric-potential-difference.md) for $v_S=5\sin(\omega t)\,\mathrm V$ and $R_L=1\,\mathrm{k\Omega}$. The [diode cathode](diode-cathode.md) is the bar at $K$; positive load [electric current](electric-current.md) flows downward through the [resistor](resistor.md). Dashed orange: source [sinusoid](sinusoid.md). Blue: load output, zero during the negative half-cycle. Green: its cycle-average [electric potential difference](electric-potential-difference.md) $5/\pi\,\mathrm V$. No smoothing [capacitor](capacitor.md) is present; these are ideal model predictions.

The [Kirchhoff cycle law](kirchhoff-cycle-law.md) gives $v_S=V_D+v_L$, and [Ohm's law](ohm-s-law.md) gives $v_L=R_Li_L$. If $v_S>0$, the blocking assumption would give $V_D=v_S>0$, contradicting the [ideal diode model](ideal-diode-model.md), so the [diode](diode.md) conducts with $V_D=0$. If $v_S<0$, conduction would give $i_L=v_S/R_L<0$, also forbidden, so the [diode](diode.md) blocks. At the crossings both values vanish. Thus

$$
v_L(t)=\max\{0,V_p\sin(\omega t)\},\qquad i_L(t)=\frac{v_L(t)}{R_L}.
$$

The peak load [electric current](electric-current.md) is $5\,\mathrm{mA}$. The output is unidirectional but still varies in [time](time-in-physics.md), reaching zero throughout every negative half-cycle. Over a [period of a function](period-of-a-function.md) $2\pi/\omega$, write the [wave phase](phase-waves.md) as $\theta=\omega t$. Its [average value of a function](average-value-of-a-function.md) and [root mean square](root-mean-square.md) follow from two [integrals](integral-split.md):

$$
\overline v_L=\frac1{2\pi}\int_0^\pi V_p\sin\theta\,d\theta=\frac{V_p}{\pi}=1.59155\,\mathrm V,\qquad
v_{L,\mathrm{rms}}=\left(\frac1{2\pi}\int_0^\pi V_p^2\sin^2\theta\,d\theta\right)^{1/2}=\frac{V_p}{2}=2.500\,\mathrm V.
$$

Consequently the average load [power](power.md) is $v_{L,\mathrm{rms}}^2/R_L=6.25\,\mathrm{mW}$, not $\overline v_L^{\,2}/R_L$. The ideal [diode](diode.md) has zero loss; the [resistor](resistor.md) converts supplied [energy](energy-split.md) into [Joule heating](joule-heating.md). The same switching argument predicts $v_L=\min(0,v_S)$ when the [diode](diode.md) is reversed. Directional selection changes the waveform and its [average value of a function](average-value-of-a-function.md); it does not by itself produce a constant output.

## ↑ Ancestors (7)

1. [Rectifier](rectifier.md)
2. [Diode](diode.md)
3. [Electrical circuit](electrical-circuit-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Half-wave rectifier](half-wave-rectifier.md)
