# Klein-Gordon packet velocities

↑ **Parent:** [Phase velocity and group velocity](phase-velocity-and-group-velocity.md)

A useful stipulated dispersive medium obeys the [Klein-Gordon equation](klein-gordon-equation.md) $u_{tt}-c^2u_{xx}+\omega_0^2u=0$, with $c>0$ and $\omega_0>0$. Its positive-[angular frequency](angular-frequency.md) [dispersion relation](dispersion-relation.md) is

$$
\omega(k)=\sqrt{\omega_0^2+c^2k^2},\qquad
v_p=\frac{\omega(k)}{k},\qquad
v_g=\omega'(k)=\frac{c^2k}{\omega(k)}.
$$

Here $\omega_0$ is the gap at zero [wavenumber](wavenumber.md), not the central [angular frequency](angular-frequency.md) $\omega_c=\omega(k_0)$ of a [wave packet](wave-packet.md); the parameter in the preceding formula is $A=\omega_0/c$. For $k>0$, the [phase velocity](phase-velocity.md) satisfies $v_p>c$, the [group velocity](group-velocity.md) satisfies $0<v_g<c$, and $v_pv_g=c^2$. In this stipulated medium $c$ is the limiting propagation speed of the model; it need not mean the vacuum [speed of light](speed-of-light.md). The same square-root [dispersion relation](dispersion-relation.md) appears in [waveguide phase and group velocities](waveguide-phase-and-group-velocities.md), with a [waveguide cutoff frequency](waveguide-cutoff-frequency.md) playing the role of $\omega_0$.[equation 9.6 and equations 9.10–9.12: square-root dispersion and local group velocity](pulse-propagation-by-richard-fitzpatrick.md)

For the original dimensionless choice $c=\omega_0=k_0=1$, a [carrier wave](carrier-wave.md) has [phase velocity](phase-velocity.md) $v_p=\sqrt2$, while a narrow [wave packet](wave-packet.md) has leading [group velocity](group-velocity.md) $v_g=1/\sqrt2$. After time $t=8$, the carrier's zero-[wave phase](phase-waves.md) reference has moved to $x=8\sqrt2\simeq11.31$, whereas the leading [wave envelope](envelope-waves.md) centre is at $x=8/\sqrt2\simeq5.66$. A carrier [wave crest](wave-crest.md) therefore moves through the [wave envelope](envelope-waves.md); it does not carry an identifiable piece of the envelope with it.

<a id="image-stipulated-klein-gordon-medium-secant-phase-velocity-tangent-group-velocity-and-front-speed"></a>
![](klein-gordon-dispersion-and-velocity-scales.png)

**[Figure 12](#image-stipulated-klein-gordon-medium-secant-phase-velocity-tangent-group-velocity-and-front-speed). Stipulated Klein-Gordon medium: secant phase velocity, tangent group velocity and front speed**.

The origin-to-curve secant on the [dispersion diagram](dispersion-diagram.md) gives [phase velocity](phase-velocity.md), while its local tangent gives [group velocity](group-velocity.md). As $k\to0^+$, $v_p\to\infty$ and $v_g\to0$; at $k=0$ the [phase velocity](phase-velocity.md) itself is undefined. As $k\to\infty$, both approach $c$, from opposite sides. On the same positive-[angular frequency](angular-frequency.md) branch with $k<0$, both signed velocities are negative and their product remains $c^2$. These conventions distinguish direction from [phase speed](phase-speed.md). Reversing both $k$ and $\omega$ represents the same real [plane wave](plane-wave.md); changing just one sign changes its direction.

For an original finite-bandwidth check, take equal-amplitude [plane waves](plane-wave.md) at $k_1=0.8$ and $k_2=1.2$, still with $c=\omega_0=1$. The exact two-tone [wave envelope](envelope-waves.md) speed is

$$
v_{\rm beat}=\frac{\sqrt{1+1.2^2}-\sqrt{1+0.8^2}}{1.2-0.8}\simeq0.703563,
$$

while its [carrier wave](carrier-wave.md) has [phase velocity](phase-velocity.md) $(\sqrt{1+0.8^2}+\sqrt{1+1.2^2})/2\simeq1.421337$. Their product is exactly $1$: rationalizing the difference gives $v_{\rm beat}=2/(\omega_1+\omega_2)$. Nevertheless $v_{\rm beat}\ne\omega'(1)$; the derivative describes the limit of vanishing separation, not an arbitrary pair of tones. The two-tone [wave envelope](envelope-waves.md) repeats indefinitely, so it has no isolated first arrival and cannot measure [front velocity](front-velocity.md).

## ↑ Ancestors (8)

1. [Phase velocity and group velocity](phase-velocity-and-group-velocity.md)
2. [Dispersion relation](dispersion-relation.md)
3. [Wave equation](wave-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gaussian envelope in a Klein-Gordon medium](gaussian-envelope-in-a-klein-gordon-medium.md)
- [Phase velocity](phase-velocity.md)
