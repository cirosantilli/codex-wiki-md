<h1 id="11/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The positive lamp [power](../../../../power.md) comes from extra [work](../../../../work.md) by the primary current source. The secondary [electric current](../../../../electric-current.md) creates a changing [magnetic flux](../../../../magnetic-flux.md) through the primary, so maintaining the same prescribed primary [electric current](../../../../electric-current.md) requires an additional terminal [voltage](../../../../voltage.md). With the preceding winding convention,

$$
v_p=L\frac{dI_p}{dt}+M\frac{dI_s}{dt}.
$$

Using [phasors](../../../../phasor.md), $\widetilde I_s=-i\omega M\widetilde I_p/(R+i\omega L_s)$, hence the primary sees the [complex impedance](../../../../electrical-impedance.md)

$$
Z_{\rm in}=i\omega L+\frac{\omega^2M^2}{R+i\omega L_s},\qquad
\operatorname{Re}Z_{\rm in}=\frac{\omega^2M^2R}{R^2+(\omega L_s)^2}>0.
$$

It follows directly that

$$
\boxed{\langle P_{\rm source}\rangle=\tfrac12I_0^2\operatorname{Re}Z_{\rm in}=\langle P_R\rangle.}
$$

This is the [reflected impedance](../../../../reflected-impedance.md) of the secondary load. The [self-inductance](../../../../self-inductance.md) and [mutual inductance](../../../../mutual-inductance.md) terms exchange stored [magnetic energy](../../../../magnetic-energy.md), while the lamp dissipates it. Multiplying the two coupled equations from [Kirchhoff's voltage law](../../../../kirchhoff-cycle-law.md) by their respective [electric currents](../../../../electric-current.md) also gives the instantaneous [conservation of energy](../../../../conservation-of-energy.md) identity

$$
v_pI_p=RI_s^2+\frac{d}{dt}\left(\frac12LI_p^2+MI_pI_s+\frac12L_sI_s^2\right).
$$

The derivative averages to zero in periodic steady state. A fixed primary [current source](../../../../current-source.md) supplies the required extra [voltage](../../../../voltage.md); a fixed [voltage source](../../../../voltage-source.md) would generally change its primary [electric current](../../../../electric-current.md) when the lamp is connected.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [11](../../11.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
