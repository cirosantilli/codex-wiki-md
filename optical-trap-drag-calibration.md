# Optical trap drag calibration

↑ **Parent:** [Harmonic optical trap](harmonic-optical-trap.md)

Translate the liquid past a bead held in a stationary [harmonic optical trap](harmonic-optical-trap.md). At steady mean position, take $u$ as the local fluid [velocity](velocity.md) relative to the fixed trap and $x$ positive downstream. Averaging the overdamped [force balance](force-balance.md) gives

$$
0=-k\langle x\rangle+\zeta u,\qquad
\langle x\rangle=\frac{\zeta}{k}u,\qquad
k=\frac{\zeta}{d\langle x\rangle/du}.
$$

For the invented [optical trap Langevin calibration](optical-trap-langevin-calibration.md) example, $u=50.0\,\mathrm{\mu m/s}$ predicts $\langle x\rangle=23.562\,\mathrm{nm}$, $V-V_0=0.23562\,\mathrm V$, and $\zeta u=k\langle x\rangle=0.47124\,\mathrm{pN}$. Reversing $u$ reverses the mean shift but leaves the ideal thermal [variance](variance-split.md) unchanged. A symmetric speed sweep tests the offset and the linear [force](force-split.md) range; the slope determines $\zeta/k$ if position is calibrated.

Near a wall, $\zeta=6\pi\eta a$ is not the appropriate drag without a boundary correction; record bead height and direction of motion. Stage [velocity](velocity.md) must correspond to the local fluid [velocity](velocity.md) after transients have settled. Escape under increasing flow estimates a maximum holding [force](force-split.md) in that geometry, whereas small-displacement drag calibration estimates the local [spring constant](spring-constant.md). They are different quantities. The [atomic force microscopy](atomic-force-microscopy.md) similarly needs a calibrated [spring constant](spring-constant.md) to convert a measured deflection to [force](force-split.md), but its cantilever is a physical spring rather than this optical field.

## ↑ Ancestors (6)

1. [Harmonic optical trap](harmonic-optical-trap.md)
2. [Optical tweezers](optical-tweezers.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Optical trap Langevin calibration](optical-trap-langevin-calibration.md)
- [Optical trap position readout](optical-trap-position-readout.md)
- [Solution](past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2012/paper-1/3/a/solution.md)
