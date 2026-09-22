# Rotational inertia measurement with a falling mass

↑ **Parent:** [Inertia tensor](inertia-tensor.md)

PASCO's [PASPORT Rotary Motion Sensor Experiment Guide](pasport-rotary-motion-sensor-experiment-guide.md), Experiment 1, specifies a PS-2120A sensor, a rod carrying two equal-radius weights, a three-step drive wheel, a thread and hanging [mass](mass.md), a clamp-on guide wheel, a support, a balance and calipers. The thread leaves the drive wheel tangentially. The sensor records [angular velocity](angular-velocity.md) against [time](time-in-physics.md); a [linear regression](linear-regression-split.md) over the accelerating interval supplies [angular acceleration](angular-acceleration.md) $\alpha$. The guide measures the drive radius with calipers and repeats the run with the weights removed to subtract the apparatus's own [moment of inertia](moment-of-inertia.md). Its tables are blank: it prescribes a measurement and does not report an observed numerical agreement. [PASPORT Rotary Motion Sensor Experiment Guide](pasport-rotary-motion-sensor-experiment-guide.md)

With hanging [mass](mass.md) $m_h$ including its hanger, effective drive radius $b$, no thread slip and negligible guide-wheel inertia, [Newton's second law](newton-s-second-law.md) gives thread [tension](tension.md) $F=m_h(g-b\alpha)$. The axial [torque](torque.md) is $bF$. Under negligible [friction](friction.md), the inference is therefore

$$
I_{\mathrm{loaded}}=\frac{m_hgb}{\alpha}-m_hb^2.
$$

Repeat the inference for the unloaded assembly and subtract: $I_{\mathrm{weights}}=I_{\mathrm{loaded}}-I_{\mathrm{empty}}$. Omitting the $m_hb^2$ term incorrectly treats thread [tension](tension.md) as the hanging weight. Comparing with $(M_1+M_2)R^2$ tests the [point mass](point-mass.md) approximation; finite-sized weights also have their own [moments of inertia](moment-of-inertia.md) about their [centres of mass](center-of-mass.md). [PASPORT Rotary Motion Sensor Experiment Guide](pasport-rotary-motion-sensor-experiment-guide.md)

Useful proposed checks go beyond that ideal inference. Verify the [rotary encoder](rotary-encoder.md)'s angle scale by turning the shaft through a marked full revolution; check the recorded [time](time-in-physics.md) against an independent clock and the balance against a known [mass](mass.md). Measure $b$ at the thread's running surface, including thread thickness; avoid overlapping wraps that change $b$. Release without a push, inspect the [angular velocity](angular-velocity.md) record for a straight interval, and stop before the hanger lands or the thread runs out. Repeat with several hanging [masses](mass.md), weight radii and rotation directions. A consistent inferred [moment of inertia](moment-of-inertia.md) across drive [torques](torque.md) supports the model; curvature, direction dependence or drift indicates a limitation rather than a new [principal moment of inertia](principal-moment-of-inertia.md).

For approximately constant resisting [torque](torque.md) $\tau_f\geq0$ in one rotation direction, an original calibration model is

$$
m_hgb-m_hb^2\alpha=I\alpha+\tau_f.
$$

Fit the left-hand quantity against $\alpha$ across several drives: the slope estimates the axial [moment of inertia](moment-of-inertia.md) and the intercept estimates $\tau_f$. This calibration is conditional on [friction](friction.md) remaining constant over the fitted [angular speeds](angular-speed.md); a freely slowing run can expose speed dependence. Sensor differentiation noise, guide-wheel [moment of inertia](moment-of-inertia.md), thread slip, flexing connectors and uncertain weight radii limit the inference. Removing weights can also change bearing loads, so empty-apparatus subtraction does not automatically cancel [friction](friction.md). These are proposed controls and a model extension, not results claimed by PASCO.

A fixed-axis readout measures $\mathbf n^T\mathbf I_O\mathbf n$, not the full [inertia tensor](inertia-tensor.md). In a proposed generalization, repeat about $x$, $y$, $z$ and the three diagonal directions $(\mathbf e_x+\mathbf e_y)/\sqrt2$, $(\mathbf e_x+\mathbf e_z)/\sqrt2$, $(\mathbf e_y+\mathbf e_z)/\sqrt2$, all through the same $O$. For example,

$$
I_{xy}=I_{O,(\mathbf e_x+\mathbf e_y)/\sqrt2}-\frac{I_{xx}+I_{yy}}2.
$$

Six independent scalar readings then determine the six entries of a [symmetric matrix](symmetric-matrix.md). Each mounting needs its own apparatus correction, and different reference points require the [tensor parallel-axis theorem](tensor-parallel-axis-theorem.md) before the readings can be combined.

**Table of contents**

- [Rotary encoder](rotary-encoder.md)

## ↑ Ancestors (7)

1. [Inertia tensor](inertia-tensor.md)
2. [Moment of inertia](moment-of-inertia.md)
3. [Rigid body dynamics](rigid-body-dynamics-split.md)
4. [Classical mechanics](classical-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
