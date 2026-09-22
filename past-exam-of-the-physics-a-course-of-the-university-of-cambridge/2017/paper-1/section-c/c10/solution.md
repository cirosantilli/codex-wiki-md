<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

**Operators, quantization and rotations.** [Angular momentum](../../../../../angular-momentum.md) is the generator of spatial rotations. In [quantum mechanics](../../../../../quantum-mechanics-split.md), its components are [Hermitian operators](../../../../../hermitian-operator.md) on their appropriate domains and obey

$$
[\widehat J_i,\widehat J_j]=i\hbar\epsilon_{ijk}\widehat J_k,
\qquad [\widehat J^2,\widehat J_i]=0.
$$

These [angular momentum commutation relations](../../../../../angular-momentum-commutation-relations.md) prevent all three components from having simultaneous sharp values. For example, the [Robertson uncertainty principle](../../../../../robertson-uncertainty-principle.md) gives $\Delta J_x\Delta J_y\ge\hbar|\langle J_z\rangle|/2$. One conventionally diagonalizes $\widehat J^2$ and a selected component $\widehat J_z$:

$$
\boxed{\widehat J^2|j,m\rangle=\hbar^2j(j+1)|j,m\rangle,
\qquad\widehat J_z|j,m\rangle=\hbar m|j,m\rangle.}
$$

The allowed labels are $j=0,\tfrac12,1,\tfrac32,\ldots$ and $m=-j,-j+1,\ldots,j$. An angular-momentum multiplet has $2j+1$ states. The magnitude $\hbar\sqrt{j(j+1)}$ differs from the largest possible component $\hbar j$; the remaining components fluctuate even in a state with maximal $m$.

The [angular momentum lowering operator](../../../../../angular-momentum-lowering-operator.md) and its raising counterpart, $\widehat J_\pm=\widehat J_x\pm i\widehat J_y$, satisfy

$$
\widehat J_\pm|j,m\rangle
=\hbar\sqrt{j(j+1)-m(m\pm1)}\,|j,m\pm1\rangle.
$$

The ladder terminates at $m=\pm j$. A rotation through angle $\theta$ about unit vector $\widehat{\mathbf n}$ acts through the [unitary operator](../../../../../unitary-operator.md) $\exp[-i\theta\widehat{\mathbf n}\cdot\widehat{\mathbf J}/\hbar]$. Thus quantized components and the continuous rotation of a state are compatible.

**[Orbital angular momentum](../../../../../orbital-angular-momentum.md).** The orbital contribution is associated with motion in space:

$$
\widehat{\mathbf L}=\widehat{\mathbf r}\times\widehat{\mathbf p}
=-i\hbar\,\mathbf r\times\boldsymbol\nabla.
$$

For a spinless spatial [wavefunction](../../../../../wave-function-split.md), the simultaneous angular eigenfunctions are the [spherical harmonics](../../../../../spherical-harmonic.md) $Y_{\ell m}(\theta,\phi)$, with $\ell=0,1,2,\ldots$ and $m=-\ell,\ldots,\ell$. Single-valued ordinary scalar spatial [wavefunctions](../../../../../wave-function-split.md) give integer orbital labels. In a central [potential energy](../../../../../potential-energy.md), $[\widehat H,\widehat L^2]=[\widehat H,\widehat L_z]=0$, so stationary states may be labelled by these angular [quantum numbers](../../../../../quantum-number.md). The angular kinetic contribution appears in the radial equation as $\ell(\ell+1)\hbar^2/(2mr^2)$, the [centrifugal potential](../../../../../centrifugal-potential.md). Noncentral interactions need not conserve these orbital labels.

**Intrinsic [spin](../../../../../spin.md) and addition.** [Spin angular momentum](../../../../../spin.md) is an intrinsic internal degree of freedom with the same commutation algebra. It is not the [angular momentum](../../../../../angular-momentum.md) of a small classical charged sphere literally rotating about its centre. For an [electron](../../../../../electron.md), $s=1/2$ and $m_s=\pm1/2$, so $\widehat S_i=(\hbar/2)\sigma_i$ in terms of the [Pauli matrices](../../../../../pauli-matrices.md). Its squared [spin](../../../../../spin.md) is $3\hbar^2/4$. Other particles can have integer or half-integer [spin](../../../../../spin.md), including [spin](../../../../../spin.md) zero.

For one particle with orbital and [spin](../../../../../spin.md) degrees of freedom, $\widehat{\mathbf J}=\widehat{\mathbf L}+\widehat{\mathbf S}$; the two component sets commute with each other. [Addition of angular momentum](../../../../../addition-of-angular-momentum.md) permits $j=|\ell-s|,|\ell-s|+1,\ldots,\ell+s$. The coupled states $|j,m_j\rangle$ are linear combinations of the uncoupled $|\ell,m_\ell\rangle|s,m_s\rangle$ with $m_j=m_\ell+m_s$, determined by [Clebsch-Gordan coefficients](../../../../../clebsch-gordan-coefficients.md). A rotationally invariant [spin-orbit interaction](../../../../../spin-orbit-interaction.md) can conserve $J^2,J_z$ while mixing the separate component labels.

[Angular momentum](../../../../../angular-momentum.md) also carries a [magnetic moment](../../../../../magnetic-dipole-moment.md). For an electron's orbital motion and intrinsic [spin](../../../../../spin.md),

$$
\boldsymbol\mu_L=-\frac e{2m_e}\mathbf L,\qquad
\boldsymbol\mu_S=-g_s\frac e{2m_e}\mathbf S,\qquad g_s\simeq2.
$$

The minus signs reflect negative [electric charge](../../../../../electric-charge-split.md). With the [Bohr magneton](../../../../../bohr-magneton.md) $\mu_B=e\hbar/(2m_e)$, a [spin](../../../../../spin.md) projection $m_s$ has $\mu_z=-g_s\mu_Bm_s$. A [magnetic field](../../../../../magnetic-field-split.md) can therefore distinguish angular-momentum states through their interaction [energy](../../../../../energy-split.md) $-\boldsymbol\mu\cdot\mathbf B$.

**Stern–Gerlach measurement.** In the [Stern-Gerlach experiment](../../../../../stern-gerlach-experiment.md), atoms emerge from a heated source, pass through collimating apertures, traverse a strongly inhomogeneous [magnetic field](../../../../../magnetic-field-split.md), and strike a position-sensitive screen. The beam is neutral, so its separation is interpreted through the atomic [magnetic moment](../../../../../magnetic-dipole-moment.md) rather than the ordinary charged-particle [Lorentz force](../../../../../lorentz-force.md). Near a chosen quantization direction, the interaction gives

$$
U=-\mu_zB_z,\qquad F_z\simeq\mu_z\frac{\partial B_z}{\partial z}.
$$

A uniform field can exert a [torque](../../../../../torque.md) but would not separate the beam by this translational force; the gradient is essential. Different allowed magnetic-moment components become correlated with different trajectories. A classical ensemble with continuously varying orientations would yield a continuous spread, whereas discrete quantum components yield separated channels.

In the modern electronic description of ground-state [silver](../../../../../silver.md), filled shells cancel their electronic angular momenta and the unpaired $5s$ electron has $L=0$, $S=1/2$, $J=1/2$. The effective electronic measurement therefore has two components, approximately $\mu_z=\pm\mu_B$, rather than an orbital $\ell=1/2$, which is not allowed. For positive field gradient the electronic $m_J=+1/2$ component has negative $\mu_z$ and deflects downward in this coordinate convention. Nuclear [spin](../../../../../spin.md) and [hyperfine structure](../../../../../hyperfine-structure.md) are neglected in this simplified two-channel account. Historically the original splitting preceded the electron-spin interpretation, so the modern explanation should not be confused with the original investigators' interpretation.

<a id="section-c/c10/image-a-neutral-atomic-beam-separates-into-two-electronic-magnetic-moment-channels-in-a-field-gradient"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1-c10-spin-analyser.png)

**[Figure 4](#section-c/c10/image-a-neutral-atomic-beam-separates-into-two-electronic-magnetic-moment-channels-in-a-field-gradient). A neutral atomic beam separates into two electronic magnetic-moment channels in a field gradient**.

More generally a prepared [spin](../../../../../spin.md) state $a|+z\rangle+b|-z\rangle$ gives the two outcomes with probabilities $|a|^2,|b|^2$. Selecting one channel prepares a state for further measurements. An ideal second analyser along the same axis then gives a definite result, whereas one along a perpendicular axis gives two equally likely outcomes for a spin-one-half [eigenstate](../../../../../eigenstate.md). This connects the apparatus directly to incompatible [spin](../../../../../spin.md) components and the [Born rule](../../../../../born-rule.md). **[Angular momentum](../../../../../angular-momentum.md) is quantized through its operator algebra; the Stern–Gerlach gradient turns that discrete internal information into spatially distinguishable outcomes.**

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
