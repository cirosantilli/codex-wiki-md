# Reactance phase convention

↑ **Parent:** [Electrical reactance](electrical-reactance.md)

Use [complex amplitudes](complex-amplitude.md) only for signals at one common positive [angular frequency](angular-frequency.md) $\omega$. Define the real terminal voltage and [electric current](electric-current.md) by

$$
v(t)=\operatorname{Re}\left(\widehat V e^{\mathrm i\omega t}\right),\qquad
i(t)=\operatorname{Re}\left(\widehat I e^{\mathrm i\omega t}\right),\qquad
Z=\frac{\widehat V}{\widehat I}.
$$

The [complex amplitudes](complex-amplitude.md) here use peak magnitudes; both can instead use [root mean square](root-mean-square.md) magnitudes without changing their ratio. Choose positive [electric current](electric-current.md) entering the terminal assigned positive voltage, so $p=vi$ is absorbed [power](power.md). For an ideal linear [inductor](inductor.md) and [capacitor](capacitor.md), their terminal laws $v_L=L\,di/dt$ and $i_C=C\,dv_C/dt$ give

$$
\widehat V_L=\mathrm i\omega L\widehat I,\qquad
\widehat I_C=\mathrm i\omega C\widehat V_C,\qquad
Z_L=\mathrm i\omega L,\qquad
Z_C=\frac1{\mathrm i\omega C}=-\frac{\mathrm i}{\omega C}.
$$

The [derivative](derivative.md) multiplies a [complex amplitude](complex-amplitude.md) by $\mathrm i\omega$: this single algebraic step explains both signs. Taking $i(t)=I_0\cos\omega t$ as a reference gives $v_L(t)=-\omega LI_0\sin\omega t$ and $v_C(t)=I_0\sin\omega t/(\omega C)$ for the sinusoidal response. Thus [inductor](inductor.md) voltage leads [electric current](electric-current.md) by $\pi/2$, while [capacitor](capacitor.md) voltage lags [electric current](electric-current.md) by $\pi/2$. A constant offset or a free transient is outside this single-[frequency](frequency.md) representation. [Feynman, Leighton and Sands, II.22.1: complex sinusoidal representation and component impedances](https://www.feynmanlectures.caltech.edu/II_22.html#Ch22-S1).

With the alternative $e^{-\mathrm i\omega t}$ convention, the same real signals use conjugated [complex amplitudes](complex-amplitude.md) and $Z_L=-\mathrm i\omega L$, $Z_C=+\mathrm i/(\omega C)$. Their physical leads and lags stay the same; the sign of $\operatorname{Im}Z$ changes. Also, some textbooks call the positive magnitude $1/(\omega C)$ the capacitive reactance and write the series expression as $X_L-|X_C|$. This article consistently uses signed $X_C=-1/(\omega C)$ and hence $X=X_L+X_C$. [Ling, Moebs and Sanny, University Physics 2, §15.2: positive capacitive-reactance magnitude and quarter-cycle phase relations](https://openstax.org/books/university-physics-volume-2/pages/15-2-simple-ac-circuits).

## ↑ Ancestors (7)

1. [Electrical reactance](electrical-reactance.md)
2. [Electrical impedance](electrical-impedance.md)
3. [Electrical circuit](electrical-circuit.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Electrical reactance bench measurement](electrical-reactance-bench-measurement.md)
