# Work-energy theorem

↑ **Parent:** [Work](work.md)

For a [point mass](point-mass.md) of constant [mass](mass.md) $m$ observed in an [inertial frame](inertial-frame.md), the net [work](work.md) along its actual path equals its change in [kinetic energy](kinetic-energy.md):

$$
W_{\mathrm{net}}=\int_{t_a}^{t_b}\mathbf F_{\mathrm{net}}(t)\cdot\mathbf v(t)\,dt
=\int_a^b\mathbf F_{\mathrm{net}}\cdot d\mathbf r
=\frac12m|\mathbf v_b|^2-\frac12m|\mathbf v_a|^2.
$$

The middle expression is a [line integral](line-integral.md); the [dot product](dot-product.md) selects the component of [force](force.md) along the [displacement](displacement.md). Positive net [work](work.md) increases [speed](speed.md), negative net [work](work.md) decreases it, and zero net [work](work.md) leaves the endpoint [speeds](speed.md) equal. Equal endpoint [speeds](speed.md) do not imply equal [velocities](velocity.md): a perpendicular [force](force.md) can continually change direction while doing zero [work](work.md). [MIT mechanics, Chapter 13, section 13.11](https://ocw.mit.edu/courses/8-01sc-classical-mechanics-fall-2016/mit8_01scs22_chapter13.pdf)

The bridge to [Newton's second law](newton-s-second-law.md) is short: take the [dot product](dot-product.md) of $m\dot{\mathbf v}=\mathbf F_{\mathrm{net}}$ with [velocity](velocity.md). The [chain rule](chain-rule.md) gives $d(m|\mathbf v|^2/2)/dt=\mathbf F_{\mathrm{net}}\cdot\mathbf v$, equating the rate of change of [kinetic energy](kinetic-energy.md) to instantaneous [power](power.md). Integrating gives the theorem. No [conservative force](conservative-force.md) assumption entered this argument; [friction](friction.md) also contributes to the net [work](work.md).

For the [harmonic oscillator](simple-harmonic-motion.md) with [spring](spring.md) stiffness $k=2\,\mathrm{N/m}$, release a [mass](mass.md) $m=0.5\,\mathrm{kg}$ from rest at $x=0.3\,\mathrm m$. The [spring](spring.md) exerts $F=-kx$. Its [work](work.md) before the first passage through $x=0$ is

$$
W=\int_{0.3\,\mathrm m}^{0}(-kx)\,dx
=\frac12k(0.3\,\mathrm m)^2=0.09\,\mathrm J.
$$

Thus $mv^2/2=0.09\,\mathrm J$ gives [speed](speed.md) $0.6\,\mathrm{m/s}$ there. The [velocity](velocity.md) is negative on this passage because the [position](position.md) is decreasing. The [energy](energy.md) calculation alone determines its magnitude, so the direction still requires information about the motion.

For a time-independent [potential energy](potential-energy.md) $V$, the [conservative force](conservative-force.md) contributes [work](work.md) $-\Delta V$. Separating all other [work](work.md) as $W_{\mathrm{other}}$ gives $\Delta(T+V)=W_{\mathrm{other}}$. Consequently [conservation of mechanical energy](conservation-of-mechanical-energy.md) requires zero net other [work](work.md); the [work-energy theorem](work-energy-theorem.md) itself does not require that conservation. With [damping](damping.md), [mechanical energy](mechanical-energy.md) decreases even though the theorem remains valid. [MIT mechanics, Chapter 14: mechanical energy and nonconservative work](https://ocw.mit.edu/courses/8-01sc-classical-mechanics-fall-2016/mit8_01scs22_chapter14.pdf)

## ↑ Ancestors (6)

1. [Work](work.md)
2. [Energy](energy.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Classical mechanics](classical-mechanics-split.md)
- [Free fall in a constant gravitational field](free-fall-in-a-constant-gravitational-field.md)
- [Kinetic energy](kinetic-energy.md)
- [Kinetic friction](kinetic-friction.md)
- [Lorentz force](lorentz-force.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4/3a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-4/10c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-4/12a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4/3b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-4/9c/solution.md)
- [Radius change at constant angular momentum](radius-change-at-constant-angular-momentum.md)
- [Rotational kinetic energy](rotational-kinetic-energy.md)
- [Work](work.md)
- [Work-energy theorem](work-energy-theorem.md)
