# RL low-pass filter

↑ **Parent:** [Low-pass filter](low-pass-filter.md)

An [RL circuit](rl-circuit.md) with the output measured across its [resistor](resistor.md) is a first-order [low-pass filter](low-pass-filter.md). For an ideal [inductor](inductor.md), an ideal voltage source and a high-resistance output instrument, the [electrical impedances](electrical-impedance.md) $i\omega L$ and $R$ give

$$
H(\omega)=\frac{R}{R+i\omega L},\qquad |H|=\frac{1}{\sqrt{1+(\omega L/R)^2}},\qquad \omega_c=\frac RL.
$$

The gain approaches one at low [angular frequency](angular-frequency.md) and $R/(\omega L)$ at high [angular frequency](angular-frequency.md); at $\omega_c$ it is $1/\sqrt2$. The time-domain equation is $L\dot I+RI=V_{\rm in}$ and $V_{\rm out}=RI$, so the [time constant](time-constant.md) is $L/R$. Instrument loading, source resistance and nonideal [inductance](inductance.md) can change the response.

## ↑ Ancestors (5)

1. [Low-pass filter](low-pass-filter.md)
2. [Linear filter](linear-filter.md)
3. [Signal processing](signal-processing.md)
4. [Electrical engineering](electrical-engineering-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/section-a/2/solution.md)
