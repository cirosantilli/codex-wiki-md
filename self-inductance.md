# Self-inductance

↑ **Parent:** [Inductance](inductance.md)

[Self-inductance](self-inductance.md) is [inductance](inductance.md) associated with a coil's own [electric current](electric-current.md), rather than [magnetic flux](magnetic-flux.md) supplied by another coil. In the linear model, fixed geometry and magnetic response give constant $L$ in $\Lambda=LI$. With the turn orientations defined in [magnetic flux linkage](magnetic-flux-linkage.md), [Faraday's law of induction](faraday-s-law-of-induction.md) gives the self-induced [electromotive force](electromotive-force.md)

$$
\mathcal E_{\rm ind}=-\frac{d\Lambda}{dt}=-L\frac{dI}{dt}.
$$

The final equality requires constant $L$; if the geometry changes, use $-d\Lambda/dt$. The minus sign expresses [Lenz's law](lenz-s-law.md): the induced [electromotive force](electromotive-force.md) opposes the change in [electric current](electric-current.md). It does not always oppose the [electric current](electric-current.md) itself. When positive [electric current](electric-current.md) decreases, the induced [electromotive force](electromotive-force.md) acts in its direction. [OpenStax University Physics 2, §14.2: self-induced emf and its direction](https://openstax.org/books/university-physics-volume-2/pages/14-2-self-inductance-and-inductors).

For terminal sign bookkeeping, label the ideal [inductor](inductor.md)'s terminals $a,b$, choose positive [electric current](electric-current.md) entering $a$ and leaving $b$, and define $v_L$ as the terminal [electric potential difference](electric-potential-difference.md) drop from $a$ to $b$ in the lumped [electrical circuit](electrical-circuit-split.md) model. This passive convention gives

$$
v_L=+L\frac{dI}{dt}=-\mathcal E_{\rm ind}.
$$

Thus a coil with [self-inductance](self-inductance.md) $0.5\,\mathrm H$ and increasing [electric current](electric-current.md) $dI/dt=12\,\mathrm{A/s}$ has terminal drop $v_L=6\,\mathrm V$ and induced [electromotive force](electromotive-force.md) $\mathcal E_{\rm ind}=-6\,\mathrm V$. These signs describe the same process with different reference conventions. The [RL circuit](rl-circuit.md) uses the terminal-drop convention throughout.

A finite terminal [electric potential difference](electric-potential-difference.md) cannot make the [electric current](electric-current.md) of an ideal [inductor](inductor.md) with constant $L>0$ jump. Integrating its [differential equation](differential-equation-split.md) gives

$$
I(t_2)-I(t_1)=\frac1L\int_{t_1}^{t_2}v_L(t)\,dt.
$$

If $v_L$ stays bounded, the [integral](integral-split.md) tends to zero as the interval shrinks, ensuring [continuity](continuous-function.md) of [electric current](electric-current.md). A step in terminal [electric potential difference](electric-potential-difference.md) changes $dI/dt$ immediately, while [electric current](electric-current.md) remains continuous. At constant [electric current](electric-current.md), the self-induced [electromotive force](electromotive-force.md) is zero, although the [inductor](inductor.md)'s [magnetic energy](magnetic-energy.md) can remain nonzero.

**Table of contents**

- [Inductor](inductor.md)
  - [Energy stored in a nonlinear inductor](energy-stored-in-a-nonlinear-inductor.md)

## ↑ Ancestors (5)

1. [Inductance](inductance.md)
2. [Electromagnetism](electromagnetism-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (43)

- [Alternating-current induction levitation](alternating-current-induction-levitation.md)
- [Coupled inductors](coupled-inductors.md)
- [Coupled RL induction model](coupled-rl-induction-model.md)
- [Electromotive force](electromotive-force.md)
- [Faraday's law of induction](faraday-s-law-of-induction.md)
- [Force on a resistive coil beside an alternating wire](force-on-a-resistive-coil-beside-an-alternating-wire.md)
- [Henry (unit)](henry-unit.md)
- [Induced current in a tilted resistive loop](induced-current-in-a-tilted-resistive-loop.md)
- [Inductance](inductance.md)
- [Inductance correction to a rotating-loop radiation estimate](inductance-correction-to-a-rotating-loop-radiation-estimate.md)
- [Inductance of a rectangular-section toroid](inductance-of-a-rectangular-section-toroid.md)
- [Inductance of a toroid with an oblique narrow air gap](inductance-of-a-toroid-with-an-oblique-narrow-air-gap.md)
- [Inductor](inductor.md)
- [Lenz's law](lenz-s-law.md)
- [Loop crossing a magnetic field boundary](loop-crossing-a-magnetic-field-boundary.md)
- [Lossless limit of magnetic loop braking](lossless-limit-of-magnetic-loop-braking.md)
- [Motional electromotive force](motional-electromotive-force.md)
- [Mutual inductance](mutual-inductance.md)
- [Orientation torque on a flux-conserving loop](orientation-torque-on-a-flux-conserving-loop.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2/17h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/7e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/7a/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2013/paper-1/4/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1/section-a/1/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-2/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-1/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1/section-a/a4/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-1/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/section-e/e14/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/section-e/15/c/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/section-b/10/d/solution.md)
- [Solution](past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2012/paper-1/1/d/solution.md)
- [Persistent current (superconductivity)](persistent-current-superconductivity.md)
- [Resistance upper bound from persistent-current decay](resistance-upper-bound-from-persistent-current-decay.md)
- [Resistive magnetic entry of a falling loop](resistive-magnetic-entry-of-a-falling-loop.md)
- [RL circuit](rl-circuit.md)
- [Rotational damping of a resistive loop in an oscillating field](rotational-damping-of-a-resistive-loop-in-an-oscillating-field.md)
- [Self-inductance](self-inductance.md)
- [Solenoid inductance](solenoid-inductance.md)
- [Stored energy of a solenoid](stored-energy-of-a-solenoid.md)
