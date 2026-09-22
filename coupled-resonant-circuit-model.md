# Coupled resonant circuit model

↑ **Parent:** [Coupled resonant circuit demonstration](coupled-resonant-circuit-demonstration.md)

Let two series loops have [inductances](inductance.md) $L_1,L_2>0$, [capacitances](capacitance.md) $C_1,C_2>0$, total [electrical resistances](electrical-resistance.md) $R_1,R_2>0$, and reciprocal [mutual inductance](mutual-inductance.md) $M=k\sqrt{L_1L_2}$ with $0\leq k<1$. For a steady [sinusoid](sinusoid.md) of [angular frequency](angular-frequency.md) $\omega>0$, choose complex peak [amplitudes](wave-amplitude.md) with time convention $e^{\mathrm i\omega t}$. An ideal source of peak [electric potential difference](electric-potential-difference.md) $V$ drives loop 1; loop 2 has no independent source. Then

$$
Z_j=R_j+\mathrm i\left(\omega L_j-\frac1{\omega C_j}\right),\qquad
\begin{pmatrix}Z_1&\mathrm i\omega M\\\mathrm i\omega M&Z_2\end{pmatrix}
\begin{pmatrix}I_1\\I_2\end{pmatrix}
=\begin{pmatrix}V\\0\end{pmatrix},\qquad
\frac{I_2}{V}=\frac{-\mathrm i\omega M}{Z_1Z_2+\omega^2M^2}.
$$

Eliminating $I_1$ proves the response formula. Reversing one coil changes the sign of $M$ and the relative [wave phase](phase-waves.md), but leaves this [amplitude](wave-amplitude.md) response unchanged. The measured sense ratio is $|R_sI_2/V|$, with $R_s$ included in $R_2$, not added a second time.

<a id="image-calculated-coupled-resonance-and-the-distinction-between-a-damped-train-and-a-maintained-sine"></a>
![](wireless-telegraphy-coupled-resonance-model.png)

**[Figure 25](#image-calculated-coupled-resonance-and-the-distinction-between-a-damped-train-and-a-maintained-sine). Calculated coupled resonance and the distinction between a damped train and a maintained sine**. Original predictions for two identical linear series loops with $L=5\,\mathrm{mH}$, $C=2\,\mathrm{nF}$ and total $R=100\,\Omega$ per loop; the secondary includes $R_s=50\,\Omega$. Top: steady sense-voltage ratios at three coupling coefficients. Bottom: one isolated loop's free damped train, exponential bounds and a maintained sine reference. Neither panel contains historical or laboratory measurements.

For identical loops at their uncoupled [resonant frequency](resonant-frequency.md) $\omega_0=1/\sqrt{LC}$,

$$
\left|\frac{I_2}{V}\right|_{\omega_0}
=\frac{\omega_0M}{R^2+\omega_0^2M^2}.
$$

Writing $x=\omega_0M/R$ makes this $x/[R(1+x^2)]$. Its [derivative](derivative.md) has the sign of $1-x^2$, so response at this fixed [frequency](frequency.md) is largest when $x=1$, equivalently $k=1/Q$. Too little coupling transfers little excitation; excessive coupling reduces the response at the original centre [frequency](frequency.md). This is a fixed-[frequency](frequency.md) optimum, not a universal optimum over every possible receiver and drive [frequency](frequency.md).

For the chosen values, $k=1/Q=0.063246$ gives $M=0.31623\,\mathrm{mH}$. At source peak $V=0.100\,\mathrm V$, the secondary peak [electric current](electric-current.md) is $0.500\,\mathrm{mA}$ and the sense peak [electric potential difference](electric-potential-difference.md) is $25.0\,\mathrm{mV}$. The primary peak [electric current](electric-current.md) is also $0.500\,\mathrm{mA}$, so source mean [power](power.md) is $25.0\,\mathrm{\mu W}$: each loop dissipates $12.5\,\mathrm{\mu W}$, checking [conservation of energy](conservation-of-energy.md). Here $V$ is the equivalent ideal source behind $R_1$; a generator's terminal reading must be converted using its measured [Thévenin resistance](thevenin-resistance.md).

In the lossless identical-loop limit, the [normal modes](normal-mode.md) have equal or opposite [electric currents](electric-current.md), making their effective [inductances](inductance.md) $L+M$ or $L-M$. Thus

$$
f_{\rm low}=\frac{f_0}{\sqrt{1+k}},\qquad
f_{\rm high}=\frac{f_0}{\sqrt{1-k}}.
$$

At $k=0.20$ these are $45.944$ and $56.270\,\mathrm{kHz}$. Finite [electrical resistance](electrical-resistance.md) broadens and shifts the driven peaks, so the exact response formula, rather than these lossless values, generates the plot. Changing a [capacitor](capacitor.md) moves the uncoupled tuning through $f_0\propto C^{-1/2}$: increasing it by $21\%$ lowers $f_0$ by the factor $1/1.1$. The model explains why tuning and coupling must be adjusted together; it supplies no transatlantic propagation or detector-threshold prediction.

## ↑ Ancestors (6)

1. [Coupled resonant circuit demonstration](coupled-resonant-circuit-demonstration.md)
2. [Wireless telegraphy](wireless-telegraphy.md)
3. [Radio communication](radio-communication.md)
4. [Telecommunication](telecommunication.md)
5. [Electrical engineering](electrical-engineering-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Coupled resonant circuit demonstration](coupled-resonant-circuit-demonstration.md)
- [Tuned spark wireless apparatus](tuned-spark-wireless-apparatus.md)
