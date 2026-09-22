<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

**Distributed line parameters.** The geometry is the wide [parallel-plate transmission line](../../../../../parallel-plate-transmission-line.md) described in the question, with absolute [permittivity](../../../../../permittivity-split.md) $\varepsilon=\epsilon\varepsilon_0$. A length $dx$ has charge $C V\,dx$ and field $E=V/d$, giving

$$
\boxed{C=\frac{\varepsilon a}{d}.}
$$

The opposed plate currents have sheet density $I/a$ and confine the leading magnetic field $H=I/a$ between the plates. The magnetic [energy](../../../../../energy-split.md) per unit length is $\mu_0H^2ad/2=LI^2/2$, so

$$
\boxed{L=\frac{\mu_0d}{a}.}
$$

Here $C$ and $L$ are per unit length, in $\mathrm{F\,m^{-1}}$ and $\mathrm{H\,m^{-1}}$, not lumped component values. Internal conductor fields and edge corrections are neglected.

**Voltage and current evolution.** The current entering a short length minus that leaving it is the rate of increase of its plate charge:

$$
I(x)-I(x+dx)=C\,dx\,\partial_tV.
$$

The voltage drop across that length is its inductive drop, $V(x)-V(x+dx)=L\,dx\,\partial_tI$. Dividing by $dx$ gives the lossless [Telegrapher's equations](../../../../../telegrapher-s-equations.md),

$$
\boxed{\partial_xI+C\partial_tV=0,\qquad
\partial_xV+L\partial_tI=0.}
$$

**Propagation speed.** Differentiate these equations once more and eliminate the other variable:

$$
\partial_x^2V=LC\,\partial_t^2V,\qquad
\partial_x^2I=LC\,\partial_t^2I.
$$

The [wave equation](../../../../../wave-equation-split.md) speed is

$$
\boxed{v=\frac1{\sqrt{LC}}
=\frac1{\sqrt{\mu_0\varepsilon_0\epsilon}}
=\frac c{\sqrt\epsilon}.}
$$

**Travelling-wave impedance.** For a forward wave $V=F(t-x/v)$, take $I=V/Z_0$. Substitution into $\partial_xI+C\partial_tV=0$ gives $1/(vZ_0)=C$, hence the [characteristic impedance](../../../../../characteristic-impedance.md)

$$
\boxed{Z_0=\sqrt{\frac LC}
=\frac da\sqrt{\frac{\mu_0}{\epsilon\varepsilon_0}}.}
$$

The backward-wave current has the opposite sign relative to its voltage; the fixed ratio above applies to one travelling direction.

**Matching the antenna.** The voltage [reflection coefficient](../../../../../reflection-coefficient.md) is $\Gamma=(Z_{\rm load}-Z_0)/(Z_{\rm load}+Z_0)$. No reflection requires $Z_0=5\ \Omega$. With $a=0.020\ \mathrm m$, $\epsilon=1.5$, and $\sqrt{\mu_0/\varepsilon_0}\simeq376.7\ \Omega$,

$$
\boxed{d=a\frac{Z_0\sqrt\epsilon}{376.7\ \Omega}
\simeq3.25\times10^{-4}\ \mathrm m=0.325\ \mathrm{mm}.}
$$

The resulting $d/a\simeq0.016$ is consistent with the wide-plate approximation.

**Both transverse forces.** The matched [transverse electromagnetic mode](../../../../../transverse-electromagnetic-mode.md) has electric attraction and magnetic repulsion. For time-averaged power $P=100\ \mathrm{kW}$,

$$
V_{\rm rms}=\sqrt{PZ_0}\simeq707\ \mathrm V,\qquad
I_{\rm rms}=\sqrt{P/Z_0}\simeq141\ \mathrm A.
$$

The force on one plate excludes its own field. Thus the average electric attraction and magnetic repulsion per unit length are respectively

$$
f_E=\frac{\varepsilon aV_{\rm rms}^2}{2d^2},\qquad
f_B=\frac{\mu_0I_{\rm rms}^2}{2a}.
$$

The [electric and magnetic pressure cancellation in a matched TEM line](../../../../../electric-and-magnetic-pressure-cancellation-in-a-matched-tem-line.md) follows directly from $V_{\rm rms}=Z_0I_{\rm rms}$:

$$
\boxed{f_E=f_B\simeq0.628\ \mathrm{N\,m^{-1}},\qquad
f_{\rm net}=0.}
$$

The equality also holds instantaneously for a single travelling wave. Quoting either $0.628\ \mathrm{N\,m^{-1}}$ alone would omit the opposing contribution. This is the ideal electromagnetic force in the stated lossless uniform-dielectric model; a standing wave would not generally have the same cancellation.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
