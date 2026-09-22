<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a common factor $e^{i(kx-\omega t)}$, with $k=k_0>0$ and $\omega=\omega_0$. For the upward propagating branches with $0<\widehat\omega_2=\omega-kU_2<N_2$, define

$$
\boxed{\sin\theta_1=\frac{\omega}{N_1},\qquad
\sin\theta_2=\frac{\widehat\omega_2}{N_2},\qquad
m_j=-k\cot\theta_j,\quad 0<\theta_j<\frac\pi2.}
$$

These are the inclinations of upward-sloping [constant-phase lines of an internal gravity wave](../../../../../../constant-phase-line-of-an-internal-gravity-wave.md) to the horizontal. Write the incident, reflected and transmitted complex velocity amplitudes as $A_0,A_r,A_t$. [Incompressibility](../../../../../../incompressible-flow.md) gives $(u_i,w_i)=A_0(\cos\theta_1,\sin\theta_1)$, $(u_r,w_r)=A_r(\cos\theta_1,-\sin\theta_1)$, and $(u_t,w_t)=A_t(\cos\theta_2,\sin\theta_2)$.

The [jump conditions for stratified inviscid shear flow](../../../../../../jump-conditions-for-stratified-inviscid-shear-flow.md) require a common interface displacement, not a common vertical velocity: $w=-i\widehat\omega\eta$ on each side. Since the background [mass density](../../../../../../density.md) is continuous, [pressure](../../../../../../pressure.md) is continuous without a hydrostatic jump. The horizontal momentum equation gives $p/\rho_0=(\widehat\omega/k)u$. Hence

$$
\frac{\sin\theta_1}{\omega}(A_0-A_r)
=\frac{\sin\theta_2}{\widehat\omega_2}A_t,\qquad
\omega\cos\theta_1(A_0+A_r)
=\widehat\omega_2\cos\theta_2A_t.
$$

These two matching equations determine [internal-wave transmission across a velocity jump](../../../../../../internal-wave-transmission-across-a-velocity-jump.md):

$$
\boxed{\frac{A_t}{A_0}=
\frac{2}{r\cos\theta_2/\cos\theta_1+r^{-1}\sin\theta_2/\sin\theta_1},\qquad
\frac{A_r}{A_0}=\frac{r\cos\theta_2/\cos\theta_1-r^{-1}\sin\theta_2/\sin\theta_1}{r\cos\theta_2/\cos\theta_1+r^{-1}\sin\theta_2/\sin\theta_1},\quad
r=\frac{\widehat\omega_2}{\omega}.}
$$

The amplitude formula printed in the PDF is inconsistent with these material-interface matching conditions. In particular, identical layers have $A_t/A_0=1$ and $A_r/A_0=0$, whereas its expression labelled “reflected” equals one. The displayed results above distinguish reflection from transmission and retain the intrinsic-frequency factors required by the [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) and pressure balance.

For equal [buoyancy frequencies](../../../../../../buoyancy-frequency.md) and the specified opposing current, $\theta_1=\pi/6$, $\theta_2=\arcsin(3/4)$, and

$$
\boxed{\frac{A_t}{A_0}=\frac8{4+\sqrt{21}},\qquad
\frac{A_r}{A_0}=\frac{\sqrt{21}-4}{\sqrt{21}+4}.}
$$

The incident phase lines have slope $1/\sqrt3$, the reflected lines slope $-1/\sqrt3$, and the transmitted lines slope $3/\sqrt7$: they steepen above the interface. For the other specified current, $\widehat\omega_2=0$. The transmitted vertical [wavenumber](../../../../../../wavenumber.md) then diverges and there is no regular propagating upper-layer wave of that frequency: this is the [critical level of an internal gravity wave](../../../../../../critical-level-of-an-internal-gravity-wave.md) limit. Approaching it from $\widehat\omega_2>0$ gives $A_r/A_0\to-1$ and vanishing transmitted vertical energy flux; setting the intrinsic frequency to zero directly is outside the regular matching calculation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
