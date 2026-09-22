# Magnetic neutron diffraction

↑ **Parent:** [Magnetic order](magnetic-order.md)

[Magnetic neutron diffraction](magnetic-neutron-diffraction.md) uses scattering of [neutrons](neutron-split.md) by ordered [magnetic moments](magnetic-dipole-moment.md) to infer [magnetic order](magnetic-order.md). [Neutrons](neutron-split.md) also scatter from [atomic nuclei](atomic-nucleus-split.md), so a pattern can contain nuclear and magnetic contributions. A [Bragg scattering](bragg-scattering.md) peak encodes periodicity; it is not a photograph of an individual [spin](spin.md).

A minimal original calculation makes the extra periodicity visible. Consider identical nuclear scatterers at positions $x_n=na$, with equal neighboring separation $a$, and ordered [magnetic moments](magnetic-dipole-moment.md) alternating between $+m_A$ and $-m_B$. A two-site repeating block of [length](length.md) $2a$ has nuclear and magnetic [scattering amplitudes](scattering-amplitude.md), apart from common geometric factors,

$$
F_N(q)=b(1+e^{iqa}),\qquad
F_M(q)=m_A-m_Be^{iqa},\qquad
q=\frac{\pi h}{a},\quad h\in\mathbb Z.
$$

Here $b$ is the common nuclear scattering coefficient and $q$ the component of the scattering [wave vector](wavevector.md) along the row. The magnetic expression assumes equally scattering point [magnetic moments](magnetic-dipole-moment.md) perpendicular to the scattering [wave vector](wavevector.md); real magnetic scattering measures the perpendicular component and has a [momentum](momentum-split.md)-dependent amplitude. This one-dimensional calculation is a periodicity illustration, not a finite-[temperature](temperature-split.md) solution for a chain.

For even $h$, $F_N=2b$ and $F_M=m_A-m_B$. For odd $h$, $F_N=0$ and $F_M=m_A+m_B$. Thus equivalent opposing [magnetic sublattices](magnetic-sublattice.md), $m_A=m_B$, cancel in forward scattering but reinforce at the odd positions of the doubled period. The [intensity](intensity-physics.md) is proportional to the squared magnitude of the [scattering amplitude](scattering-amplitude.md), so changing an amplitude's sign does not make a negative [intensity](intensity-physics.md).

<a id="image-an-alternating-magnetic-moment-pattern-creates-extra-reciprocal-lattice-peaks"></a>
![](magnetic-diffraction-sublattice-selection.png)

**[Figure 21](#image-an-alternating-magnetic-moment-pattern-creates-extra-reciprocal-lattice-peaks). An alternating magnetic moment pattern creates extra reciprocal lattice peaks**. Original exact two-site [crystal basis structure factor](crystal-basis-structure-factor.md) illustration, not historical measurements or a simulation of MnO. Nuclear strengths use $b=1$. Ordered magnetic strengths use $(m_A,m_B)=(1,1)$ or $(2,1)$; each channel is in its own arbitrary units, so their absolute heights cannot be compared. Thin solid nuclear sticks and dashed magnetic sticks coincide at even $h$ in the ferrimagnetic case. The top panel stipulates loss of long-range magnetic order while retaining nuclear periodicity; diffuse magnetic scattering is omitted, rather than asserted absent. Only positive nonzero $q$ is shown.

This calculation also exposes a useful difference between [antiferromagnetism](antiferromagnetism.md) and [ferrimagnetism](ferrimagnetism.md): with $m_A=2$ and $m_B=1$, magnetic squared amplitudes are $1$ at even $h$ and $9$ at odd $h$. Extra magnetic peaks can therefore occur in a [ferrimagnet](ferrimagnetism.md) too. Identifying a real magnetic structure needs the full [crystal basis structure factor](crystal-basis-structure-factor.md), multiple reflections, and the allowed moment orientations, rather than a single extra peak.

**Table of contents**

- [Magnetic form factor](magnetic-form-factor.md)
- [Manganese monoxide neutron diffraction experiment](manganese-monoxide-neutron-diffraction-experiment.md)

## ↑ Ancestors (6)

1. [Magnetic order](magnetic-order.md)
2. [Magnetism](magnetism.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Antiferromagnetism](antiferromagnetism.md)
- [Magnetic neutron diffraction](magnetic-neutron-diffraction.md)
- [Neutron diffraction](neutron-diffraction.md)
- [Neutron scattering](neutron-scattering.md)
- [Nuclear neutron scattering length](nuclear-neutron-scattering-length.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2/section-b/21/c/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2005/section-b/b4/a/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012/2/c/solution.md)
