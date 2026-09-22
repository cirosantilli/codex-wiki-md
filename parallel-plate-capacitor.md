# Parallel-plate capacitor

↑ **Parent:** [Capacitor](capacitor.md)

A [parallel-plate capacitor](parallel-plate-capacitor.md) consists of two parallel [electrical conductors](electrical-conductor.md) with overlapping [area](surface-area.md) $A$ and separation $d$. If the gap is small compared with both plate widths and is filled by a uniform material of positive [permittivity](permittivity-split.md) $\epsilon$, its [capacitance](capacitance.md) is approximately

$$
C\simeq\frac{\epsilon A}{d}.
$$

This neglects the [fringing field of a capacitor](fringing-field-of-a-capacitor.md) near the plate edges. The interior [electric field](electric-field-split.md) points from the plate of positive [electric charge](electric-charge-split.md) to the plate of negative [electric charge](electric-charge-split.md), and is approximately uniform. [OpenStax University Physics 2, §8.1: the parallel-plate approximation](https://openstax.org/books/university-physics-volume-2/pages/8-1-capacitors-and-capacitance).

For a worked vacuum example, stipulate $A=0.01\,\mathrm{m^2}$, $d=0.001\,\mathrm m$, and [vacuum permittivity](vacuum-permittivity.md) $\epsilon_0\approx8.854\times10^{-12}\,\mathrm{F/m}$. This rounds the value in [Fundamental Physical Constants — Complete Listing by National Institute of Standards and Technology and others](fundamental-physical-constants-complete-listing-by-national-institute-of-standards-and-technology-and-others.md). Within the approximation,

$$
C\simeq\frac{(8.854\times10^{-12})(0.01)}{0.001}\,\mathrm F
=8.854\times10^{-11}\,\mathrm F=88.54\,\mathrm{pF}.
$$

At terminal [electric potential difference](electric-potential-difference.md) $V=10\,\mathrm V$, the [electric field](electric-field-split.md) magnitude is $E\simeq V/d=10^4\,\mathrm{V/m}$, the plate [electric charge](electric-charge-split.md) magnitude is $Q=CV=0.8854\,\mathrm{nC}$, and the [capacitor energy](capacitor-energy.md) is $U=CV^2/2=4.427\,\mathrm{nJ}$. These numbers use the stipulated rounded [vacuum permittivity](vacuum-permittivity.md); finite plates also have corrections from the [fringing field of a capacitor](fringing-field-of-a-capacitor.md).

<a id="image-uniform-electric-field-in-a-parallel-plate-capacitor"></a>
![](parallel-plate-capacitor-field.png)

**[Figure 1](#image-uniform-electric-field-in-a-parallel-plate-capacitor). Uniform electric field in a parallel-plate capacitor**.

The formula makes design changes easy to predict: doubling the overlapping [area](surface-area.md) doubles the [capacitance](capacitance.md), and halving the gap doubles the [capacitance](capacitance.md), with [permittivity](permittivity-split.md) fixed and the [fringing field of a capacitor](fringing-field-of-a-capacitor.md) neglected. Doubling [permittivity](permittivity-split.md) also doubles [capacitance](capacitance.md) if the material uniformly fills the gap and remains linear. This lets a compact device store more separated [electric charge](electric-charge-split.md) at the same terminal [electric potential difference](electric-potential-difference.md).

The short derivation uses [surface charge density](surface-charge-density.md) $\sigma=Q/A$. In the interior, [Gauss's law](gauss-s-law.md) gives [electric field](electric-field-split.md) magnitude $E\simeq\sigma/\epsilon=Q/(\epsilon A)$. The [electric potential difference](electric-potential-difference.md) is $V\simeq Ed=Qd/(\epsilon A)$, so dividing $Q$ by $V$ gives $C\simeq\epsilon A/d$. A narrow curved [capacitor](capacitor.md) gap has the same leading local approximation when its width is much less than the curvature radius.

**Table of contents**

- [Fringing field of a capacitor](fringing-field-of-a-capacitor.md)
  - [Uniform-charge estimate at a capacitor corner](uniform-charge-estimate-at-a-capacitor-corner.md)
    - [Charge redistribution at a capacitor corner](charge-redistribution-at-a-capacitor-corner.md)
  - [Capacitor gap aspect ratio](capacitor-gap-aspect-ratio.md)
  - [Bounded two-dimensional capacitor field model](bounded-two-dimensional-capacitor-field-model.md)
  - [Mapping a capacitor fringing field](mapping-a-capacitor-fringing-field.md)
  - [Guard electrode of a capacitor](guard-electrode-of-a-capacitor.md)

## ↑ Ancestors (5)

1. [Capacitor](capacitor.md)
2. [Electromagnetism](electromagnetism-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (29)

- [Arithmetic-harmonic bounds for dielectric capacitance](arithmetic-harmonic-bounds-for-dielectric-capacitance.md)
- [Capacitor](capacitor.md)
- [Capacitor energy](capacitor-energy.md)
- [Capacitor gap aspect ratio](capacitor-gap-aspect-ratio.md)
- [Coaxial capacitor with grounded inner and outer cylinders](coaxial-capacitor-with-grounded-inner-and-outer-cylinders.md)
- [Dielectric](dielectric.md)
- [Dielectric capacitance measurement](dielectric-capacitance-measurement.md)
- [Dielectric capacitor response](dielectric-capacitor-response.md)
- [Dielectric strength](dielectric-strength.md)
- [Displacement current](displacement-current.md)
- [Electric potential](electric-potential.md)
- [Electric potential difference](electric-potential-difference.md)
- [Farad](farad.md)
- [Fixed-voltage capacitor energy balance](fixed-voltage-capacitor-energy-balance.md)
- [Fringing field of a capacitor](fringing-field-of-a-capacitor.md)
- [Parallel-plate capacitor](parallel-plate-capacitor.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/17e/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2021/paper-1/7/iii/b/solution.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2021/paper-2/section-b/20/v/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2021/section-a/a3/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2/section-b/b6/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2/section-b/b6/c/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-1/section-a/a4/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2/section-b/b7/b/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/section-a/6/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/section-e/e15/c/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/section-a/a4/solution.md)
- [Permittivity](permittivity-split.md)
- [Vacuum permittivity](vacuum-permittivity.md)
