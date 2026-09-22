# Linear rigid rotor

↑ **Parent:** [Rigid rotor](rigid-rotor.md)

For a [diatomic molecule](diatomic-molecule.md), let $m_1,m_2$ be the two [masses](mass.md) and $r$ their fixed separation. The distances from the [centre of mass](center-of-mass.md) are $r_1=m_2r/(m_1+m_2)$ and $r_2=m_1r/(m_1+m_2)$. A perpendicular axis through the [centre of mass](center-of-mass.md) therefore has [moment of inertia](moment-of-inertia.md)

$$
I=m_1r_1^2+m_2r_2^2=\mu r^2,\qquad \mu=\frac{m_1m_2}{m_1+m_2}.
$$

The [reduced mass](reduced-mass.md) $\mu$ here is not the [electric dipole moment](electric-dipole-moment.md), for which we use $\mathbf d$. For a longer [linear molecule](linear-molecule.md), replace $\mu r^2$ by $\sum_i m_i\rho_i^2$, where $\rho_i$ is each distance along the axis from the [centre of mass](center-of-mass.md). In the point-mass idealization, the axial [moment of inertia](moment-of-inertia.md) is zero; turning about that axis changes no nuclear positions, so no independent axial rotational degree of freedom is included.

For the field-free [linear rigid rotor](linear-rigid-rotor.md), assume a fixed internal [quantum state](quantum-state.md) with no electronic [angular momentum](angular-momentum.md) or electronic [spin](spin.md), and omit couplings to nuclear [spin](spin.md). The rotational [Hamiltonian](hamiltonian.md) is $\widehat H_{\rm rot}=\widehat{\mathbf L}^{\,2}/(2I)$. Its orientation [wavefunctions](wave-function-split.md) are [spherical harmonics](spherical-harmonic.md) $Y_{JM}$, and its [angular momentum eigenstates](angular-momentum-eigenstate.md) satisfy

$$
\widehat{\mathbf L}^{\,2}Y_{JM}=\hbar^2J(J+1)Y_{JM},\qquad
\widehat L_zY_{JM}=\hbar M Y_{JM},\qquad
E_J=\frac{\hbar^2}{2I}J(J+1)=hB J(J+1),
$$

where $J=0,1,2,\ldots$ and $M=-J,-J+1,\ldots,J$. Each $E_J$ belongs to $2J+1$ [angular momentum eigenstates](angular-momentum-eigenstate.md) distinguished by the [magnetic quantum number](magnetic-quantum-number.md) $M$, an instance of [degenerate energy levels](degenerate-energy-levels.md). The [Planck constant](planck-constant.md) is $h=2\pi\hbar$; $B$ is the frequency-valued [rotational constant](rotational-constant.md). Notice that the [energy eigenvalues](energy-eigenvalue-split.md) scale as $J(J+1)$, not $J^2$.

<a id="image-linear-rigid-rotor-levels-and-transitions"></a>
![](linear-rigid-rotor-levels-and-transitions.png)

**[Figure 3](#image-linear-rigid-rotor-levels-and-transitions). Linear rigid rotor: increasing gaps between energy eigenvalues and equally spaced transition frequencies**. Original dimensionless model: $E_J/(hB)=J(J+1)$. Upward arrows show [photon absorption](photon-absorption.md) with $\Delta J=1$; the sticks show positions only, not measured or predicted intensities. The $2J+1$ states at each [energy eigenvalue](energy-eigenvalue-split.md) are represented by one horizontal line.

Subtracting consecutive [energy eigenvalues](energy-eigenvalue-split.md) gives

$$
\nu_{J\to J+1}=\frac{E_{J+1}-E_J}{h}=2B(J+1).
$$

Thus increasing level gaps produce a regularly spaced series of lines at $2B,4B,6B,\ldots$, with spacing $2B$. Allowed positions do not guarantee that every line is visible: [electric-dipole selection rules](electric-dipole-selection-rule.md), occupation of the initial [quantum state](quantum-state.md), and instrument response also matter.

**Table of contents**

- [Rotational temperature](rotational-temperature.md)
- [Rotational constant](rotational-constant.md)
- [Pure rotational electric-dipole selection rules](pure-rotational-electric-dipole-selection-rules.md)
- [Isotope shift of a linear rotor](isotope-shift-of-a-linear-rotor.md)

## ↑ Ancestors (5)

1. [Rigid rotor](rigid-rotor.md)
2. [Molecular rotation](molecular-rotation.md)
3. [Molecule](molecule-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (34)

- [Carbon monosulfide](carbon-monosulfide.md)
- [Diatomic molecule](diatomic-molecule.md)
- [Hydrogen rotational heat capacity](hydrogen-rotational-heat-capacity.md)
- [Linear molecule](linear-molecule.md)
- [Linear rigid rotor](linear-rigid-rotor.md)
- [Most populated rotational level](most-populated-rotational-level.md)
- [Ortho-para conversion heat](ortho-para-conversion-heat.md)
- [Parahydrogen](parahydrogen.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2012/paper-1/1/b/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1/a3/a/i/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1/a3/a/iii/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-1/a3/b/i/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2/a7/c/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2/a7/d/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2/a8/b/ii/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2024/paper-1/a3/a/i/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-2b/section-b/35/c/i/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1/section-b/b9/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-a/2/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-2/section-c/c9/c/solution.md)
- [Planar rigid rotor](planar-rigid-rotor.md)
- [Pure rotational electric-dipole selection rules](pure-rotational-electric-dipole-selection-rules.md)
- [Rigid rotor](rigid-rotor.md)
- [Rotational energy](rotational-energy.md)
- [Rotational monitoring of deuterium exchange](rotational-monitoring-of-deuterium-exchange.md)
- [Rotational partition functions of hydrogen](rotational-partition-functions-of-hydrogen.md)
- [Rotational Raman spectroscopy](rotational-raman-spectroscopy.md)
- [Rotational spectral line assignment](rotational-spectral-line-assignment.md)
- [Rotational spectroscopy](rotational-spectroscopy.md)
- [Rotational spectrum](rotational-spectrum.md)
- [Rotational state populations](rotational-state-populations.md)
- [Rotational temperature](rotational-temperature.md)
- [Spin isomers of hydrogen](spin-isomers-of-hydrogen.md)
- [University of Florida HCl and DCl FTIR experiment](university-of-florida-hcl-and-dcl-ftir-experiment.md)
