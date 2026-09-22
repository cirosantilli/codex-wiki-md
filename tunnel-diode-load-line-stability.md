# Tunnel-diode load-line stability

↑ **Parent:** [Tunnel diode](tunnel-diode.md)

A [current-voltage characteristic](current-voltage-characteristic.md) determines possible steady [operating points](operating-point.md); it does not alone determine their [linear stability](linear-stability.md). Consider an ideal [voltage source](voltage-source.md) $V_s$ feeding a [tunnel diode](tunnel-diode.md) through a [resistor](resistor.md) $R>0$, with a positive constant [capacitance](capacitance.md) $C$ across the junction. Assume a quasistatic device relation $I(V)$ and neglect [inductance](inductance.md), transit delays, [noise](noise-signal-processing.md) and heating. [Kirchhoff's current law](kirchhoff-node-law.md) gives the original one-state model

$$
C\dot V=\frac{V_s-V}{R}-I(V).
$$

A steady [operating point](operating-point.md) $V_*$ satisfies $I(V_*)=(V_s-V_*)/R$: the device curve intersects the descending supply line. This is the source-side counterpart of a [resistive load line](resistive-load-line.md). A small perturbation $V=V_*+\delta V$ obeys

$$
C\,\delta\dot V=-\left(\frac1R+I'(V_*)\right)\delta V,\qquad
\lambda=-\frac{1/R+I'(V_*)}{C}.
$$

Thus the [equilibrium point](equilibrium-point-of-a-dynamical-system.md) is locally attracting if $1/R+I'(V_*)>0$ and unstable if the inequality reverses. Equality requires higher-order analysis. Even on a [negative differential resistance](negative-differential-resistance.md) segment, a sufficiently small supply [electrical resistance](electrical-resistance.md) can stabilize this model. The assumption about the [electrical circuit](electrical-circuit-split.md) matters: an inductive or delayed circuit has additional state variables and may behave differently.

Choose an original toy forward characteristic, with no fitted device parameters:

$$
x=\frac{V}{V_0},\qquad
I(V)=I_0\,i(x),\qquad
i(x)=x^3-6x^2+10x=x\bigl((x-3)^2+1\bigr),
$$

where $V_0=0.10\,\mathrm V$, $I_0=1.0\,\mathrm{mA}$ and $0\le x\le3.6$. For every $x>0$, $i(x)>0$, so this entire forward curve absorbs positive total [power](power.md). Nevertheless

$$
I'(V)=\frac{I_0}{V_0}(3x^2-12x+10)<0
\quad\Longleftrightarrow\quad
2-\frac{\sqrt6}{3}<x<2+\frac{\sqrt6}{3}.
$$

The model therefore separates [negative differential resistance](negative-differential-resistance.md) from negative total $V/I$. The corresponding peak and valley are at approximately $0.1184\,\mathrm V$ and $0.2816\,\mathrm V$; these voltages deliberately differ from the historical peak.

With $R=100\,\Omega$ and $V_s=0.60\,\mathrm V$, the supply line is $I/I_0=6-x$. The intersection equation factors exactly:

$$
i(x)+x-6=(x-1)(x-2)(x-3)=0.
$$

The three [operating points](operating-point.md) are $(0.10\,\mathrm V,5\,\mathrm{mA})$, $(0.20\,\mathrm V,4\,\mathrm{mA})$ and $(0.30\,\mathrm V,3\,\mathrm{mA})$. Their values of $1/R+I'(V_*)$ are respectively $20$, $-10$ and $20\,\mathrm{mS}$. The outer two attract nearby trajectories; the middle one repels them. This is [bistability](bistability.md) in the specified one-state [electrical circuit](electrical-circuit-split.md).

<a id="image-chosen-tunnel-diode-curve-and-supply-line-linear-stability"></a>
![](tunnel-diode-toy-load-line-stability.png)

**[Figure 2](#image-chosen-tunnel-diode-curve-and-supply-line-linear-stability). Chosen tunnel diode curve and supply-line linear stability**. [Source](tunnel-diode-toy-load-line-stability.py). Original calculated [current-voltage characteristics](current-voltage-characteristic.md) and trajectories of the stated quasistatic model. Filled green points attract nearby trajectories; the open red point repels them. The same negative-slope point becomes attracting when the supply [electrical resistance](electrical-resistance.md) is reduced and the source voltage adjusted. All values are chosen, not measured data or a fit to a historical device. Both panels use $C=10\,\mathrm{nF}$ and the same toy device curve.

For the second panel, choose $R=25\,\Omega$ and $V_s=0.30\,\mathrm V$. Now $I/I_0=12-4x$ and

$$
i(x)+4x-12=(x-2)\bigl((x-2)^2+2\bigr)=0.
$$

There is exactly one real [operating point](operating-point.md), again $(0.20\,\mathrm V,4\,\mathrm{mA})$. Here $1/R+I'(V_*)=20\,\mathrm{mS}>0$, despite the device's own slope $I'(V_*)=-20\,\mathrm{mS}$. With $C=10\,\mathrm{nF}$, the perturbation decays with time constant $C/(20\,\mathrm{mS})=0.50\,\mathrm{\mu s}$; the unstable middle point of the first panel has growth time $1.0\,\mathrm{\mu s}$.

The one-state autonomous model supports switching between attracting [operating points](operating-point.md) after a perturbation or parameter change; it cannot produce a nonconstant periodic orbit. A proposed [oscillator](oscillator.md) needs additional dynamics. This limitation is useful: a load-line intersection establishes a possible steady reading, the slope test establishes local attraction in a specified model, and neither calculation alone predicts an oscillation frequency for a real [tunnel diode](tunnel-diode.md).

## ↑ Ancestors (5)

1. [Tunnel diode](tunnel-diode.md)
2. [P-n junction](p-n-junction.md)
3. [Semiconductor](semiconductor-split.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Esaki tunnel-diode experiment](esaki-tunnel-diode-experiment.md)
