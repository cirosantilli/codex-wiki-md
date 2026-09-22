# Electron hole

↑ **Parent:** [Quasiparticle](quasiparticle.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Electron_hole)

An [electron hole](electron-hole.md) is an unoccupied [Electron](electron.md) [quantum state](quantum-state.md) in an otherwise nearly full [energy band](energy-band.md), often the [valence band](valence-band.md). “Filled” refers to occupation of the allowed [quantum states](quantum-state.md), not to filling all space with a continuous fluid of [Electrons](electron.md). Each state, including its [spin](spin.md) label, can hold at most one [Electron](electron.md) by the [Pauli exclusion principle](pauli-exclusion-principle.md). The almost full [energy band](energy-band.md) and its few missing occupants are therefore simpler to describe as a background plus a few [electron holes](electron-hole.md). The [electron hole](electron-hole.md) is a [quasiparticle](quasiparticle.md), not a [Positron](positron.md) inserted into the crystal.

Removing an [Electron](electron.md) of [electric charge](electric-charge.md) $-e$ changes the background's [electric charge](electric-charge.md) by $+e$. Thus an [electron hole](electron-hole.md) carries positive [electric charge](electric-charge.md) relative to that background. Promoting an [Electron](electron.md) into the [conduction band](conduction-band.md) creates an [electron hole](electron-hole.md) without changing the whole crystal's [electric charge](electric-charge.md): $(-e)+(+e)=0$. An unbound pair still consists of two separate [charge carriers](charge-carrier.md); only a [bound state](bound-state.md) of their relative motion is an [exciton](exciton.md).

<a id="image-energy-band-occupation-and-the-motion-and-filling-of-an-electron-hole"></a>
![](electron-hole-band-occupation.png)

**[Figure 2](#image-energy-band-occupation-and-the-motion-and-filling-of-an-electron-hole). Energy band occupation and the motion and filling of an electron hole**. [Source](electron-hole-band-occupation.py). Original occupation schematic. Blue filled circles are occupied spin-resolved states; open circles are empty states. A promotion conserves the displayed [Electron](electron.md) count while changing occupation of the [valence band](valence-band.md) and [conduction band](conduction-band.md). The lower, localized cartoon shows an [Electron](electron.md) filling a neighboring vacancy so that the vacancy moves oppositely, and a [conduction band](conduction-band.md) [Electron](electron.md) filling a [valence band](valence-band.md) [electron hole](electron-hole.md). The [energy](energy.md) axis is qualitative: the row diagrams are neither a [dispersion relation](dispersion-relation.md) nor single-electron levels for an [exciton](exciton.md).

The local cartoon explains why a vacancy can move: when a neighboring [Electron](electron.md) fills it, another vacancy appears where that [Electron](electron.md) was. The vacancy has moved opposite to that particular transfer of an [Electron](electron.md). In an extended [Bloch state](bloch-state.md), use [crystal momentum](crystal-momentum.md) instead of imagining a permanently empty atomic site. For a completely filled [energy band](energy-band.md) the summed [electric current](electric-current.md) vanishes. Omitting one [Electron](electron.md) with [group velocity](group-velocity.md) $\mathbf v_v$ removes its contribution $-e\mathbf v_v$, leaving a contribution $+e\mathbf v_v$. This fixes both the positive [electric charge](electric-charge.md) and the velocity convention of the [electron hole](electron-hole.md).

More precisely, near a parabolic [valence band](valence-band.md) maximum, set its [energy](energy.md) $E_v(0)$ as reference and define the [electron hole](electron-hole.md) [wave vector](wavevector.md) by $\mathbf k_h=-\mathbf k_v$. Then

$$
E_h(\mathbf k_h)=E_v(0)-E_v(-\mathbf k_h),\qquad
\mathbf v_h=\frac{1}{\hbar}\nabla_{\mathbf k_h}E_h=\mathbf v_v(-\mathbf k_h),\qquad
E_h(\mathbf k_h)\simeq\frac{\hbar^2k_h^2}{2m_h^*}.
$$

The occupied [Electron](electron.md) branch has negative curvature there, while the [electron hole](electron-hole.md) branch has positive [effective mass](band-effective-mass.md) $m_h^*$. The velocity equality compares the [electron hole](electron-hole.md) with the missing [Bloch state](bloch-state.md)'s [group velocity](group-velocity.md); it does not contradict the opposite vacancy motion in a local transfer cartoon. The sign conventions are listed in [Phys 460 Lecture 17](phys-460-fall-2006/phys-460-lecture-17.md).

**Table of contents**

- [Electron-hole recombination](electron-hole-recombination.md)
- [Valence band](valence-band.md)
- [Conduction band](conduction-band.md)

## ↑ Ancestors (5)

1. [Quasiparticle](quasiparticle.md)
2. [Quantum mechanics](quantum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Conduction band](conduction-band.md)
- [Drude conductivity and Hall experiment](drude-conductivity-and-hall-experiment.md)
- [Electron hole](electron-hole.md)
- [Electron-hole recombination](electron-hole-recombination.md)
- [Exciton](exciton.md)
- [Exciton absorption experiment in copper(I) oxide](exciton-absorption-experiment-in-copper-i-oxide.md)
- [Exciton binding energy](exciton-binding-energy.md)
- [Seebeck coefficient](seebeck-coefficient.md)
- [Valence band](valence-band.md)
