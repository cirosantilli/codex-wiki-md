# Maxwell-Boltzmann velocity distribution

↑ **Parent:** [Maxwell-Boltzmann distribution](maxwell-boltzmann-distribution.md)

In the gas rest frame, the [Maxwell-Boltzmann velocity distribution](maxwell-boltzmann-velocity-distribution.md) is the [probability density function](probability-density-function.md) per unit volume in [velocity](velocity.md) space:

$$
f(\mathbf v)=
\left(\frac{m}{2\pi k_BT}\right)^{3/2}
\exp\left(-\frac{m|\mathbf v|^2}{2k_BT}\right)
=\frac{e^{-|\mathbf v|^2/(2s^2)}}{(2\pi s^2)^{3/2}},
\qquad \int_{\mathbb R^3}f(\mathbf v)\,d^3\mathbf v=1.
$$

Thus $f(\mathbf v)\,d^3\mathbf v$ gives the [probability](probability.md) of a small three-dimensional [velocity](velocity.md) region. For a gas with bulk [mean velocity](mean-velocity-of-a-kinetic-distribution.md) $\mathbf V$, replace $\mathbf v$ by $\mathbf v-\mathbf V$; the [Maxwell speed distribution](maxwell-speed-distribution.md) then describes the magnitude relative to that bulk motion.

For any one Cartesian [velocity](velocity.md) component $v_x$, integrating out the other two gives

$$
q(v_x)=\frac{1}{\sqrt{2\pi}s}e^{-v_x^2/(2s^2)},
\qquad \langle v_x\rangle=0,
\qquad \langle v_x^2\rangle=s^2=\frac{k_BT}{m}.
$$

The factorization $f(\mathbf v)=q(v_x)q(v_y)q(v_z)$ establishes [independence](independent-random-variables.md): all three components are centered [normal random variables](gaussian-random-variable.md), with [variance](variance-split.md) $s^2$. Both the component density $q$ and the vector density $f$ have their largest values at zero. This concerns densities for small equal-sized regions; any single exact [velocity](velocity.md) still has [probability](probability.md) zero. [Fitzpatrick, component distribution and factorization](https://farside.ph.utexas.edu/teaching/sm1/lectures/node72.html)

The [standard deviation](standard-deviation.md) $s$ measures thermal motion even though the [mean velocity](mean-velocity-of-a-kinetic-distribution.md) is zero. Positive and negative components cancel in the [mean](expected-value-split.md), but their squares add. This is why [thermal Doppler broadening](thermal-doppler-broadening.md) measures a nonzero line width in a gas with no bulk motion.

**Table of contents**

- [Maxwell speed distribution](maxwell-speed-distribution.md)
  - [Most probable speed in the Maxwell distribution](most-probable-speed-in-the-maxwell-distribution.md)
- [Doppler broadening](doppler-broadening.md)
  - [Doppler resolution of a Zeeman pattern](doppler-resolution-of-a-zeeman-pattern.md)
  - [Thermal Doppler broadening](thermal-doppler-broadening.md)
    - [Thermal cutoff of Lyman-alpha line widths](thermal-cutoff-of-lyman-alpha-line-widths.md)

## ↑ Ancestors (6)

1. [Maxwell-Boltzmann distribution](maxwell-boltzmann-distribution.md)
2. [Quantum ideal-gas statistics](quantum-ideal-gas-statistics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (28)

- [Astrophysical S factor](astrophysical-s-factor.md)
- [Energy-temperature curve of a two-dimensional self-gravitating rod gas](energy-temperature-curve-of-a-two-dimensional-self-gravitating-rod-gas.md)
- [Gaussian line-of-sight velocity distribution](gaussian-line-of-sight-velocity-distribution.md)
- [Isothermal collisionless tracer](isothermal-collisionless-tracer.md)
- [Kinetic theory](kinetic-theory-split.md)
- [Lowered Maxwellian velocity distribution](lowered-maxwellian-velocity-distribution.md)
- [Lyman-alpha forest](lyman-alpha-forest.md)
- [Maxwell-Boltzmann distribution](maxwell-boltzmann-distribution.md)
- [Maxwell-Boltzmann velocity distribution](maxwell-boltzmann-velocity-distribution.md)
- [Maxwell speed distribution](maxwell-speed-distribution.md)
- [Mode (statistics)](mode-statistics.md)
- [Nuclear S-factor variation across a Gamow window](nuclear-s-factor-variation-across-a-gamow-window.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-67/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-70/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-72/1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-69/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-73/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4/34d/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-62/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-315/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/36a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/36a/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/36a/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-346/1/a/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2015/paper-1/2/b/solution.md)
- [Thermal Doppler broadening](thermal-doppler-broadening.md)
- [Thermionic tail-flux derivation](thermionic-tail-flux-derivation.md)
- [Two-level saturation population model](two-level-saturation-population-model.md)
