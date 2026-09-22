# Waveguide phase and group velocities

↑ **Parent:** [Waveguide cutoff frequency](waveguide-cutoff-frequency.md)

For a propagating branch of an ideal [vacuum](vacuum.md)-filled [rectangular electromagnetic waveguide](rectangular-electromagnetic-waveguide.md), the [phase velocity](phase-velocity.md) tracks constant [wave phase](phase-waves.md) along the axis, whereas the [group velocity](group-velocity.md) describes a sufficiently narrow, weakly distorted [wave packet](wave-packet.md). Using $\omega^2=c^2\beta^2+\omega_c^2$ gives

$$
v_{\rm ph}=\frac{\omega}{\beta}=\frac{c}{\sqrt{1-(\omega_c/\omega)^2}},\qquad
v_g=\frac{d\omega}{d\beta}=\frac{c^2\beta}{\omega}=c\sqrt{1-(\omega_c/\omega)^2}.
$$

Thus $v_{\rm ph}>c$, $0<v_g<c$, and $v_{\rm ph}v_g=c^2$. Differentiating the [dispersion relation](dispersion-relation-split.md) proves the second formula; dividing it by $\beta^2$ proves the first. This is the same mathematical structure as [Klein-Gordon packet velocities](klein-gordon-packet-velocities.md). In the stipulated $f=1.25f_c$ example,

$$
v_{\rm ph}=\frac53c,\qquad v_g=\frac35c.
$$

Over $0.30\,\mathrm m$, the corresponding narrow-envelope delay is $(0.50\,\mathrm m)/c$, approximately $1.668\,\mathrm{ns}$. Timing a carrier [wave crest](wave-crest.md) would give $0.6004\,\mathrm{ns}$; it does not time the arrival of a newly introduced message.

There is an independent [energy](energy-split.md) check. For the forward $\mathrm{TE}_{10}$ fields, the average axial [Poynting vector](poynting-vector.md) is $\langle S_z\rangle=\beta|E_y|^2/(2\mu_0\omega)$. Integrating across the guide gives average [power](power.md) $P$ and average [electromagnetic energy](electromagnetic-energy.md) per unit length $U'$:

$$
P=\frac{ab\beta E_0^2}{4\mu_0\omega},\qquad U'=\frac{\epsilon_0abE_0^2}{4},\qquad \frac{P}{U'}=\frac{c^2\beta}{\omega}=v_g.
$$

The transverse [sine](sine.md) and [cosine](cosine.md) squared each integrate to $a/2$; $\beta^2+(\pi/a)^2=\omega^2/c^2$ then makes the integrated electric and magnetic contributions to $U'$ equal. The axial [energy](energy-split.md) transport therefore agrees with the [group velocity](group-velocity.md) in this ideal model.

As $\omega\downarrow\omega_c$, $v_g\to0$ and $v_{\rm ph}\to\infty$; exactly at cutoff $\omega/\beta$ is undefined. Strong [wave dispersion](wave-dispersion.md) close to cutoff also limits the narrow-packet approximation. Neither a large [phase velocity](phase-velocity.md) nor a pulse peak establishes superluminal [information velocity](information-velocity.md); [front velocity](front-velocity.md) asks a separate causal question. In a uniform filling with constant positive [permittivity](permittivity-split.md) $\varepsilon$ and [magnetic permeability](permeability-electromagnetism.md) $\mu$, replace $c$ by $u=1/\sqrt{\varepsilon\mu}$, giving $v_{\rm ph}v_g=u^2$. Frequency-dependent material response or significant loss requires differentiating the actual [dispersion relation](dispersion-relation-split.md), so this product is not universal.

## ↑ Ancestors (7)

1. [Waveguide cutoff frequency](waveguide-cutoff-frequency.md)
2. [Rectangular electromagnetic waveguide](rectangular-electromagnetic-waveguide.md)
3. [Electromagnetic wave](electromagnetic-wave-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Klein-Gordon packet velocities](klein-gordon-packet-velocities.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/17a/solution.md)
