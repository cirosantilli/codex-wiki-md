# Spark-excited damped oscillation

↑ **Parent:** [Wireless telegraphy](wireless-telegraphy.md)

A [spark gap](spark-gap.md) can rapidly discharge a charged [capacitor](capacitor.md) through an [inductor](inductor.md). After excitation, the stored [energy](energy-split.md) runs down through [Joule heating](joule-heating.md), radiation and other losses. A key held down can permit repeated discharges: each discharge starts a damped train of rapid [oscillations](oscillation.md). The spark repetition [frequency](frequency.md), the electrical [oscillation](oscillation.md) [frequency](frequency.md) within each train, and the rate of keyed symbols are different quantities. Repetition does not make each train a maintained [sinusoid](sinusoid.md).

An original lumped model replaces the conducting [spark gap](spark-gap.md) and other losses by a constant total [electrical resistance](electrical-resistance.md) $R>0$ in an isolated [series RLC circuit](series-rlc-circuit.md). For [electric charge](electric-charge-split.md) $q$ on the [capacitor](capacitor.md), the [Kirchhoff cycle law](kirchhoff-cycle-law.md) gives

$$
L\ddot q+R\dot q+\frac qC=0,\qquad
\omega_0=\frac1{\sqrt{LC}},\quad
\alpha=\frac R{2L},\quad
Q=\frac{\omega_0L}R.
$$

For $Q>1/2$, its characteristic roots are $-\alpha\pm\mathrm i\omega_d$, with $\omega_d=\sqrt{\omega_0^2-\alpha^2}$, proving the stated damped form. The [electric current](electric-current.md) $\dot q$ has the same exponential decay scale. Its [wave envelope](envelope-waves.md) falls by $\exp(-2\pi\alpha/\omega_d)$ per cycle; the [energy](energy-split.md) envelope falls twice as fast in the exponent. A maintained [sinusoid](sinusoid.md) instead requires continuing input [power](power.md) balancing losses.

With $L=5\,\mathrm{mH}$, $C=2\,\mathrm{nF}$ and $R=100\,\Omega$, the model gives $f_0=\omega_0/(2\pi)=50.329\,\mathrm{kHz}$, [Q factor](q-factor.md) $Q=15.811$, amplitude [time constant](time-constant.md) $1/\alpha=100\,\mathrm{\mu s}$, and damped [frequency](frequency.md) $\omega_d/(2\pi)=50.304\,\mathrm{kHz}$. These are chosen component values. A real [spark gap](spark-gap.md) switches nonlinearly, an [antenna](antenna-radio.md) radiates, and coupling exchanges [energy](energy-split.md) between circuits; one constant-$R$ free decay does not model the complete transmitter. Rapid [damping](damping.md) also broadens the [frequency spectrum](frequency-spectrum.md), which helps explain why short trains make sharp receiver selection difficult.

## ↑ Ancestors (5)

1. [Wireless telegraphy](wireless-telegraphy.md)
2. [Radio communication](radio-communication.md)
3. [Telecommunication](telecommunication.md)
4. [Electrical engineering](electrical-engineering-split.md)
5. [Codex Wiki](split.md)
