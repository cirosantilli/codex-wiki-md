<h1 id="section-b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mathcal I$ be the sphere's mechanical [moment of inertia](../../../../../moment-of-inertia.md) about its rotation axis, and let $\omega_i=\omega(0)$. For an undriven rigid sphere the rotational [energy](../../../../../energy-split.md) is $E_{\rm rot}=\mathcal I\omega^2/2$. In the weak-radiation-loss approximation, [conservation of energy](../../../../../conservation-of-energy.md) gives

$$
\mathcal I\omega\dot\omega=-\overline P=-K\omega^4,\qquad
\dot\omega=-\frac K{\mathcal I}\omega^3.
$$

Integrating $d(\omega^{-2})/dt=2K/\mathcal I$ gives

$$
\boxed{\omega(t)=\frac{\omega_i}{\sqrt{1+(2K\omega_i^2/\mathcal I)t}}
=\omega_i\left[1+\frac{\mu_0p_0^2\omega_i^2}{3\pi c\mathcal I}t\right]^{-1/2}.}
$$

Equivalently, the characteristic spin-down time is

$$
\boxed{\tau=\frac{\mathcal I}{2K\omega_i^2}
=\frac{27c\mathcal I}{16\pi\mu_0\sigma_0^2R^6\omega_i^2}.}
$$

The [radiative spin-down of a rotating electric dipole](../../../../../radiative-spin-down-of-a-rotating-electric-dipole.md) therefore has [angular frequency](../../../../../angular-frequency.md) that decays as $t^{-1/2}$ at late times within this model, rather than exponentially. The original paper gives no mass or mass-density profile, so $\mathcal I$ cannot be determined from $R$ and the [relative permittivity](../../../../../relative-permittivity.md). If a homogeneous solid sphere of mass $M$ is additionally assumed, insert $\mathcal I=2MR^2/5$; uniform dielectric response alone does not imply this mechanical mass distribution.

The approximation is important. If the dipole angle is $\phi(t)$ with $\dot\phi=\omega(t)$, direct [differentiation](../../../../../differentiation.md) gives $|\ddot{\mathbf p}|^2=p_0^2(\omega^4+\dot\omega^2)$. Using the constant-frequency radiation law instantaneously neglects the second term and assumes $|\dot\omega|\ll\omega^2$. This gives the standard leading slow spin-down solution above. An exact nonadiabatic [radiation reaction](../../../../../radiation-reaction.md) evolution would require the mechanical and near-field dynamics beyond the information supplied, rather than treating this leading law as exact at arbitrarily rapid damping.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
