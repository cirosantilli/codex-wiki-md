# Electron hole

↑ **Parent:** [Quasiparticle](quasiparticle.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Electron_hole)

An [electron hole](electron-hole.md) is an unoccupied [electron](electron.md) [quantum state](quantum-state.md) in an otherwise nearly full [energy band](energy-band.md), often the [valence band](valence-band.md). “Filled” refers to occupation of the allowed [quantum states](quantum-state.md), not to filling all space with a continuous fluid of [electrons](electron.md). Each state, including its [spin](spin.md) label, can hold at most one [electron](electron.md) by the [Pauli exclusion principle](pauli-exclusion-principle.md). The almost full [energy band](energy-band.md) and its few missing occupants are therefore simpler to describe as a background plus a few [electron holes](electron-hole.md). The [electron hole](electron-hole.md) is a [quasiparticle](quasiparticle.md), not a [Positron](positron.md) inserted into the crystal.

Removing an [electron](electron.md) of [electric charge](electric-charge-split.md) $-e$ changes the background's [electric charge](electric-charge-split.md) by $+e$. Thus an [electron hole](electron-hole.md) carries positive [electric charge](electric-charge-split.md) relative to that background. Promoting an [electron](electron.md) into the [conduction band](conduction-band.md) creates an [electron hole](electron-hole.md) without changing the whole crystal's [electric charge](electric-charge-split.md): $(-e)+(+e)=0$. An unbound pair still consists of two separate [charge carriers](charge-carrier.md); only a [bound state](bound-state.md) of their relative motion is an [exciton](exciton.md).

<a id="image-energy-band-occupation-and-the-motion-and-filling-of-an-electron-hole"></a>
![](electron-hole-band-occupation.png)

**[Figure 4](#image-energy-band-occupation-and-the-motion-and-filling-of-an-electron-hole). Energy band occupation and the motion and filling of an electron hole**. [Source](electron-hole-band-occupation.py). Original occupation schematic. Blue filled circles are occupied spin-resolved states; open circles are empty states. A promotion conserves the displayed [electron](electron.md) count while changing occupation of the [valence band](valence-band.md) and [conduction band](conduction-band.md). The lower, localized cartoon shows an [electron](electron.md) filling a neighboring vacancy so that the vacancy moves oppositely, and a [conduction band](conduction-band.md) [electron](electron.md) filling a [valence band](valence-band.md) [electron hole](electron-hole.md). The [energy](energy-split.md) axis is qualitative: the row diagrams are neither a [dispersion relation](dispersion-relation-split.md) nor single-electron levels for an [exciton](exciton.md).

The local cartoon explains why a vacancy can move: when a neighboring [electron](electron.md) fills it, another vacancy appears where that [electron](electron.md) was. The vacancy has moved opposite to that particular transfer of an [electron](electron.md). In an extended [Bloch state](bloch-state.md), use [crystal momentum](crystal-momentum.md) instead of imagining a permanently empty atomic site. For a completely filled [energy band](energy-band.md) the summed [electric current](electric-current.md) vanishes. Omitting one [electron](electron.md) with [group velocity](group-velocity.md) $\mathbf v_v$ removes its contribution $-e\mathbf v_v$, leaving a contribution $+e\mathbf v_v$. This fixes both the positive [electric charge](electric-charge-split.md) and the velocity convention of the [electron hole](electron-hole.md).

More precisely, near a parabolic [valence band](valence-band.md) maximum, set its [energy](energy-split.md) $E_v(0)$ as reference and define the [electron hole](electron-hole.md) [wave vector](wavevector.md) by $\mathbf k_h=-\mathbf k_v$. Then

$$
E_h(\mathbf k_h)=E_v(0)-E_v(-\mathbf k_h),\qquad
\mathbf v_h=\frac{1}{\hbar}\nabla_{\mathbf k_h}E_h=\mathbf v_v(-\mathbf k_h),\qquad
E_h(\mathbf k_h)\simeq\frac{\hbar^2k_h^2}{2m_h^*}.
$$

The occupied [electron](electron.md) branch has negative curvature there, while the [electron hole](electron-hole.md) branch has positive [effective mass](band-effective-mass.md) $m_h^*$. The velocity equality compares the [electron hole](electron-hole.md) with the missing [Bloch state](bloch-state.md)'s [group velocity](group-velocity.md); it does not contradict the opposite vacancy motion in a local transfer cartoon. The sign conventions are listed in [Phys 460 Lecture 17](phys-460-fall-2006/phys-460-lecture-17.md).

**Table of contents**

- [Light hole](light-hole.md)
- [Heavy hole](heavy-hole.md)
- [Electron-hole pair](electron-hole-pair.md)
- [Electron-hole recombination](electron-hole-recombination.md)
  - [Minority carrier lifetime](minority-carrier-lifetime.md)
  - [Radiative electron-hole recombination](radiative-electron-hole-recombination.md)
  - [Auger recombination](auger-recombination.md)
- [Valence band](valence-band.md)
  - [Split-off valence band](split-off-valence-band.md)
  - [Heavy-hole and light-hole bands](heavy-hole-and-light-hole-bands.md)
- [Conduction band](conduction-band.md)
  - [Conduction electron](conduction-electron.md)

## ↑ Ancestors (5)

1. [Quasiparticle](quasiparticle.md)
2. [Quantum mechanics](quantum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (89)

- [Bardeen-Brattain point-contact transistor experiment](bardeen-brattain-point-contact-transistor-experiment.md)
- [Biexciton](biexciton.md)
- [Carrier density in a graphene cone](carrier-density-in-a-graphene-cone.md)
- [Charge and carrier density of an abrupt p-n junction](charge-and-carrier-density-of-an-abrupt-p-n-junction.md)
- [Compensated two-carrier magnetoresistance](compensated-two-carrier-magnetoresistance.md)
- [Conduction band](conduction-band.md)
- [Double heterostructure laser](double-heterostructure-laser.md)
- [Drude conductivity and Hall experiment](drude-conductivity-and-hall-experiment.md)
- [Electron hole](electron-hole.md)
- [Electron-hole Coulomb interaction](electron-hole-coulomb-interaction.md)
- [Electron-hole pair](electron-hole-pair.md)
- [Electron-hole recombination](electron-hole-recombination.md)
- [Esaki tunnel-diode experiment](esaki-tunnel-diode-experiment.md)
- [Exciton](exciton.md)
- [Exciton absorption experiment in copper(I) oxide](exciton-absorption-experiment-in-copper-i-oxide.md)
- [Exciton binding energy](exciton-binding-energy.md)
- [GaN blue LED development](gan-blue-led-development.md)
- [Gate control of graphene carrier density](gate-control-of-graphene-carrier-density.md)
- [Graphene](graphene.md)
- [Heavy-hole and light-hole bands](heavy-hole-and-light-hole-bands.md)
- [Hole mobility](hole-mobility.md)
- [Hydrogen passivation of magnesium acceptors in gallium nitride](hydrogen-passivation-of-magnesium-acceptors-in-gallium-nitride.md)
- [Hydrogenic acceptor state](hydrogenic-acceptor-state.md)
- [Indium arsenide](indium-arsenide.md)
- [Internal quantum efficiency](internal-quantum-efficiency.md)
- [Intrinsic semiconductor](intrinsic-semiconductor.md)
- [Light-emitting diode](light-emitting-diode.md)
- [Light-emitting diode efficiency](light-emitting-diode-efficiency.md)
- [Minority carrier](minority-carrier.md)
- [N-type semiconductor](n-type-semiconductor.md)
- [P-n junction](p-n-junction.md)
- [P-type semiconductor](p-type-semiconductor.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2/a10/a/i/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2/a10/b/iii/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2022/paper-2/a10/c/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-2/a10/a/ii/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-2/a10/a/iii/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2024/paper-2/a10/b/ii/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/6/b/ii/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2018/paper-1/section-b/10/i/a/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2019/paper-1/section-b/9/i/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-2/section-d/d12/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-2/section-a/5/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-2/section-d/d13/a/solution.md)
- [Semiconductor bands and efficient light emission](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2/section-c/c11/semiconductor-bands-and-efficient-light-emission.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2/section-d/d13/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2/section-c/c11/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2/section-d/d12/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2/section-a/4/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2/section-d/d13/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-2/section-c/c8/d/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-2/section-a/4/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004/section-a/3/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004/section-b/b9/a/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004/section-b/b9/c/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012/1/a/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012/2/a/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2013/3/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2014/4/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2016/3/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2016/4/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2017/1/b/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2018/section-a/1/b/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2018/section-b/b2/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2019/section-b/4/c/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2021/section-b/4/d/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2021/section-b/6/a/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2021/section-b/6/b/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2022/section-a/1/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2022/section-b/6/b/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2022/section-b/6/e/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2018/section-b/b2/solution.md)
- [Photocurrent](photocurrent.md)
- [Photodiode](photodiode.md)
- [Photovoltaic effect](photovoltaic-effect.md)
- [Quantum dot](quantum-dot.md)
- [Seebeck coefficient](seebeck-coefficient.md)
- [Self-assembled InAs quantum-dot single-photon source](self-assembled-inas-quantum-dot-single-photon-source.md)
- [Semiconductor](semiconductor-split.md)
- [Semiconductor carrier freeze-out](semiconductor-carrier-freeze-out.md)
- [Semiconductor inversion layer](semiconductor-inversion-layer.md)
- [Semiconductor mass-action law](semiconductor-mass-action-law.md)
- [Shockley-Queisser limit](shockley-queisser-limit.md)
- [Solar cell](solar-cell.md)
- [Split-off valence band](split-off-valence-band.md)
- [Trap-assisted electron-hole recombination](trap-assisted-electron-hole-recombination.md)
- [Two-carrier Hall coefficient](two-carrier-hall-coefficient.md)
- [Type-I band alignment](type-i-band-alignment.md)
- [Valence band](valence-band.md)
