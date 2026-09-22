<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

For the [series-fed parallel LC voltage response](../../../../../series-fed-parallel-lc-voltage-response.md), use [phasors](../../../../../phasor.md) with time dependence $e^{i\omega t}$. The parallel branch has impedance $iX$, where $X=\omega L/(1-\omega^2LC)$. Therefore

$$
\boxed{Z=R+iX,\quad|Z|=\sqrt{R^2+X^2},\quad\arg Z=\operatorname{atan2}(X,R).}
$$

At the ideal parallel [resonance](../../../../../resonance.md) $\omega_0=1/\sqrt{LC}$ its input impedance diverges. The input-current phase changes sign on crossing this pole; expressions there are interpreted by limits.

The [capacitor](../../../../../capacitor.md) [voltage](../../../../../voltage.md) equals the parallel-branch [voltage](../../../../../voltage.md). Define $q=R(1-\omega^2LC)/(\omega L)$. Then

$$
\boxed{H(\omega)=\frac{V_C}{V_i}=\frac{iX}{R+iX}=\frac1{1-iq},\quad
|H|=(1+q^2)^{-1/2},\quad\arg H=\arctan q.}
$$

At low [frequency](../../../../../frequency.md) $H\sim i\omega L/R$; at high [frequency](../../../../../frequency.md) $H\sim-i/(\omega RC)$; at [resonance](../../../../../resonance.md) $H=1$. Thus it is a **band-pass [voltage](../../../../../voltage.md) filter or [resonant frequency](../../../../../resonant-frequency.md) selector**. Its phase decreases continuously from $+\pi/2$ through zero to $-\pi/2$. Half-power points satisfy $|q|=1$ and

$$
\omega_\pm=\frac{\sqrt{(RC)^{-2}+4/(LC)}\pm(RC)^{-1}}2,\qquad
\omega_+-\omega_-=\frac1{RC}.
$$

<a id="section-c/c11/image-voltage-response-of-a-parallel-resonator"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1-ia2010-lc-response.png)

**[Figure 3](#section-c/c11/image-voltage-response-of-a-parallel-resonator). Voltage response of a parallel resonator**. Original transfer amplitude and phase for the stated series-fed parallel LC circuit. The example has R sqrt(C/L)=1; resonance and both half-power points are marked, with asymptotic phases shown.

For the supplied component values and $\omega=2\pi(50)\,\mathrm{s^{-1}}$, $X=421.745\,\Omega$ and $V_{C,\rm pk}=99.3046\,\mathrm V$. The element peak currents are

$$
\boxed{I_{R,\rm pk}=\frac{100}{\sqrt{50^2+421.745^2}}=0.23546\,\mathrm A,\quad
I_{L,\rm pk}=\frac{99.3046}{\omega(0.150)}=2.10731\,\mathrm A,\quad
I_{C,\rm pk}=\omega(60\times10^{-6})(99.3046)=1.87185\,\mathrm A.}
$$

[Inductor](../../../../../inductor.md) and [capacitor](../../../../../capacitor.md) currents are opposite [phasors](../../../../../phasor.md); their magnitudes subtract here rather than add. The [resistor](../../../../../resistor.md) carries the input current, with

$$
\boxed{I_{\rm rms}=I_{R,\rm pk}/\sqrt2=0.16650\,\mathrm A.}
$$

These results assume ideal components and sinusoidal [steady state](../../../../../steady-state.md).

## ↑ Ancestors (13)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
