# Biot-Savart law

↑ **Parent:** [Electromagnetism](electromagnetism-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Biot-Savart_law)

For a steady [current density](current-density.md) $J$, the [magnetic field](magnetic-field-split.md) is

$$
B(r)=\frac{\mu_0}{4\pi}\int
\frac{J(r')\times(r-r')}{|r-r'|^3}\,d^3r'.
$$

The [Biot-Savart law](biot-savart-law.md) adds [magnetic field](magnetic-field-split.md) contributions from a specified [electric current](electric-current.md) distribution. The [vectors](vector.md) $\mathbf r'$ and $\mathbf r$ locate source and observer; $\mathbf r-\mathbf r'$ points toward the observer. Here $\mu_0$ is [vacuum permeability](vacuum-permeability.md). For a thin wire carrying [electric current](electric-current.md) $I$, the [volume integral](volume-integral.md) becomes a [line integral](line-integral.md):

$$
\mathbf B(\mathbf r)=\frac{\mu_0 I}{4\pi}
\int_C\frac{d\boldsymbol\ell'\times(\mathbf r-\mathbf r')}
{|\mathbf r-\mathbf r'|^3},\qquad
 d\mathbf B=\frac{\mu_0}{4\pi}\frac{I\,d\boldsymbol\ell'\times\widehat{\mathbf R}}{R^2},
\quad \mathbf R=\mathbf r-\mathbf r'.
$$

Here $d\boldsymbol\ell'$ follows positive [conventional current](conventional-current.md); $\widehat{\mathbf R}$ is the [unit vector](unit-vector.md) toward the observer. With fixed path orientation, reversing the [electric current](electric-current.md) replaces $I$ by $-I$. The [cross product](cross-product.md) and [right-hand rule](right-hand-rule.md) fix the direction. Reversing the source-to-observer displacement would give the wrong sign.[II.14–6, equations (14.37)–(14.38); II.14–7, equations (14.42)–(14.43), including the cross-product order](the-feynman-lectures-on-physics-volume-ii-by-richard-feynman-and-others.md)

The setting is [magnetostatics](magnetostatics.md): time-independent [current density](current-density.md) and [charge density](charge-density.md), in [vacuum](vacuum.md) or with the vacuum approximation for air. [Electric charge conservation](charge-conservation.md) then gives $\nabla\cdot\mathbf J=0$. A finite segment is part of a complete [electrical circuit](electrical-circuit-split.md); its endpoints cannot continuously accumulate [electric charge](electric-charge-split.md) in a steady state. The instantaneous integral above does not describe switching transients or [electromagnetic radiation](electromagnetic-radiation-split.md). In magnetic matter, specify the total [current density](current-density.md), including [magnetization current](magnetization-current.md), rather than automatically replacing $\mu_0$ by an arbitrary [magnetic permeability](permeability-electromagnetism.md).[II.13–4, equations (13.12)–(13.13), steady-current and closed-circuit discussion; II.13–5, internal currents in magnetic matter](the-feynman-lectures-on-physics-volume-ii-by-richard-feynman-and-others.md)

The [superposition principle](superposition-principle.md) makes the [Biot-Savart law](biot-savart-law.md) useful even when the complete [electrical circuit](electrical-circuit-split.md) lacks the [symmetry](symmetry-physics.md) needed to evaluate [Ampère's circuital law](ampere-s-circuital-law.md) directly. Integrate a straight piece, a curved piece, and the return path separately, then add their [magnetic fields](magnetic-field-split.md) as [vectors](vector.md). The beauty is that a local oriented [current element](current-element.md) produces both the circulating [magnetic field of a finite straight wire](magnetic-field-of-a-finite-straight-wire.md) and the reinforcing [on-axis magnetic field of a circular current loop](on-axis-magnetic-field-of-a-circular-current-loop.md).

An actual laboratory procedure is documented in WPI Physics Department's [Magnetic Field Mapping](https://users.wpi.edu/~kwu/Teaching/PH2651/biot-savart-law_MField_2017.pdf), §§1.2–1.2.3 and the single-coil checklist on p. 9. Preparation locates the active area of a [Hall effect](hall-effect.md) sensor using a small magnet. A field meter reads the component normal to that area. The wire apparatus is a wall-mounted square loop selectable between one and five conductors. The coil connects to a power supply and [ammeter](ammeter.md); its diameter and turn count are recorded. Align the sensor and scan distance. The control is a current-off background reading at each position, subtracted from the current-on reading. The inference compares corrected [magnetic field](magnetic-field-split.md) with position and the predicted geometry dependence. Active-area displacement, sensor tilt, background variation, and finite coil width limit that comparison. These are instructions, not reported measurements.[pp. 2–5, §§1.2–1.2.3: preparation, sensor orientation, wire background subtraction and single-coil apparatus; p. 9, single-coil checklist](magnetic-field-mapping-by-wpi-physics-department.md)

A further proposed control is to reverse $I$ at fixed sensor position and orientation. If the background and meter offset stay unchanged, the odd part isolates the [magnetic field](magnetic-field-split.md) from the [electric current](electric-current.md):

$$
\frac{B_{\rm read}(+I)-B_{\rm read}(-I)}2=B_{\rm current}.
$$

This is a deduction from the [superposition principle](superposition-principle.md), not a reported WPI measurement. The measured component, sensor position, and complete return path must still match the model.

**Table of contents**

- [Centre field of a rigidly rotating charged loop](centre-field-of-a-rigidly-rotating-charged-loop.md)
- [Magnetic field of a uniformly conducting strip](magnetic-field-of-a-uniformly-conducting-strip.md)
- [Magnetic-field cancellation of an arc and tangent leads](magnetic-field-cancellation-of-an-arc-and-tangent-leads.md)
- [Current element](current-element.md)
- [Magnetic field of a finite straight wire](magnetic-field-of-a-finite-straight-wire.md)
- [On-axis magnetic field of a circular current loop](on-axis-magnetic-field-of-a-circular-current-loop.md)
- [Magnetic-field cancellation between oppositely driven coaxial loops](magnetic-field-cancellation-between-oppositely-driven-coaxial-loops.md)

## ↑ Ancestors (4)

1. [Electromagnetism](electromagnetism-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (41)

- [Biot-Savart law](biot-savart-law.md)
- [Current element](current-element.md)
- [Geselowitz formula](geselowitz-formula.md)
- [Long-solenoid approximation](long-solenoid-approximation.md)
- [Magnetic-energy lower bound from helicity](magnetic-energy-lower-bound-from-helicity.md)
- [Magnetic-field cancellation of an arc and tangent leads](magnetic-field-cancellation-of-an-arc-and-tangent-leads.md)
- [Magnetic field of a finite straight wire](magnetic-field-of-a-finite-straight-wire.md)
- [Magnetization](magnetization.md)
- [On-axis magnetic field of a circular current loop](on-axis-magnetic-field-of-a-circular-current-loop.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-36/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/18b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/17g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/16b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-76/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2/18d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-3/11c/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-2/6c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/15d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/15d/c/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a/section-a/2/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2b/section-a/2/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-1/section-b/b8/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-1/section-a/a5/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2/section-b/b6/a/solution.md)
- [A1](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1/section-a/a1.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-1/section-b/b8/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-1/section-b/b7/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-1/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2/section-b/b6/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-1/section-c/c9/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-1/section-c/c9/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2/section-b/b7/c/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/section-e/e14/b/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/e15/c/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/section-e/e14/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/section-e/15/c/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/section-b/10/b/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/section-b/10/c/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/section-b/10/a/solution.md)
- [Vortex filament](vortex-filament.md)
- [Vortex ring](vortex-ring.md)
