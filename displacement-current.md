# Displacement current

↑ **Parent:** [Ampère's circuital law](ampere-s-circuital-law.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Displacement_current)

In vacuum, [displacement current](displacement-current.md) is the term $\mathbf J_D=\epsilon_0\partial_t\mathbf E$ in the [Ampère-Maxwell equation](ampere-s-circuital-law.md). It has the units of [current density](current-density.md), but need not describe [electric charge](electric-charge-split.md) crossing the region. In [Maxwell equations in matter](maxwell-equations-in-matter.md), the corresponding term is $\partial_t\mathbf D$, with $\mathbf D$ the [electric displacement field](electric-displacement-field.md).

Consider a slowly charging [parallel-plate capacitor](parallel-plate-capacitor.md) with vacuum gap, plate area $A$, and charge $Q(t)$ on its positive plate. Neglect fringing and assume the charging timescale is long compared with the light-travel time across the apparatus. The nearly uniform gap [electric field](electric-field-split.md) has magnitude $E=Q/(\epsilon_0A)$, so the [displacement current](displacement-current.md) through the gap is

$$
I_D=\epsilon_0 A\frac{dE}{dt}=\frac{dQ}{dt}=I.
$$

For $A=0.010\,\mathrm{m^2}$ and charging [electric current](electric-current.md) $I=1.0\,\mathrm{mA}$, this gives $dE/dt\simeq1.13\times10^{10}\,\mathrm{V\,m^{-1}\,s^{-1}}$ and $J_D=0.10\,\mathrm{A/m^2}$. No conducting [electric current](electric-current.md) crosses the gap. A spanning surface cutting the wire and another passing between the plates nevertheless give the same magnetic circulation when the full [Ampère-Maxwell equation](ampere-s-circuital-law.md) is used. [Feynman lectures, II.18.2: charging a capacitor](https://www.feynmanlectures.caltech.edu/II_18.html#Ch18-S2).

The local consistency check is short. Without [displacement current](displacement-current.md), taking the [divergence](divergence.md) of $\nabla\times\mathbf B=\mu_0\mathbf J$ would force $\nabla\cdot\mathbf J=0$, allowing no local accumulation of [electric charge](electric-charge-split.md). With [displacement current](displacement-current.md), the [divergence of a curl is zero](divergence-of-a-curl-is-zero.md) and [Gauss's law](gauss-s-law.md) give

$$
0=\mu_0\left(\nabla\cdot\mathbf J+\epsilon_0\partial_t\nabla\cdot\mathbf E\right)
=\mu_0\left(\nabla\cdot\mathbf J+\partial_t\rho\right).
$$

This is precisely the [charge continuity equation](charge-continuity-equation.md). [Electric charge conservation](charge-conservation.md) fixes the required [divergence](divergence.md) of the added term; it does not by itself exclude other divergence-free additions. The specific [Maxwell equations](maxwell-equations-split.md) also yield the [electromagnetic wave equation](electromagnetic-wave-equation.md), linking this consistency correction to propagation at the [speed of light](speed-of-light.md).

**Table of contents**

- [Axisymmetric high-frequency capacitor field](axisymmetric-high-frequency-capacitor-field.md)
- [Conduction-to-displacement current ratio](conduction-to-displacement-current-ratio.md)
- [Surface independence of Ampère circulation during capacitor charging](surface-independence-of-ampere-circulation-during-capacitor-charging.md)

## ↑ Ancestors (6)

1. [Ampère's circuital law](ampere-s-circuital-law.md)
2. [Maxwell equations](maxwell-equations-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (33)

- [Charge conservation](charge-conservation.md)
- [Conduction current](conduction-current.md)
- [Displacement current](displacement-current.md)
- [Electromagnetism](electromagnetism-split.md)
- [Electromagnetism by David Tong](electromagnetism-by-david-tong.md)
- [Magnetic diffusivity](magnetic-diffusivity.md)
- [Magnetic field strength](magnetic-field-strength.md)
- [Magnetostatic Ampère law](magnetostatic-ampere-law.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2018/section-a/a1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-36/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-75/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/16b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-64/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/7a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-314/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/17c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2/15d/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1/section-b/b6/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-1/section-a/a2/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2/section-b/b6/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2/section-b/b6/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-2/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2/section-b/b6/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2/section-b/b6/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-1/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2/section-b/b6/c/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/section-e/e15/d/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/section-e/e15/d/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/b8/solution.md)
- [Poynting flux in a centrally discharged parallel-plate capacitor](poynting-flux-in-a-centrally-discharged-parallel-plate-capacitor.md)
- [Quasistatic electromagnetic approximation](quasistatic-electromagnetic-approximation.md)
- [Transverse wave cutoff in a cold unmagnetized plasma](transverse-wave-cutoff-in-a-cold-unmagnetized-plasma.md)
