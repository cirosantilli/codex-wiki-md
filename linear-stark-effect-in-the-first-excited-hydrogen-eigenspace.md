# Linear Stark effect in the first excited hydrogen eigenspace

↑ **Parent:** [Stark effect](stark-effect.md)

Consider a fixed [proton](proton.md) and one [electron](electron.md), omitting [spin](spin.md), [fine structure](fine-structure.md) and the [Lamb shift](lamb-shift.md). Let $e>0$ be the [elementary charge](elementary-charge.md), $a_0$ the [Bohr radius](bohr-radius.md) in this fixed-nucleus model, and $\mathbf E=\mathcal E\widehat{\mathbf z}$. Because the [electron](electron.md)'s [electric dipole moment](electric-dipole-moment.md) is $\mathbf d=-e\mathbf r$, its [electric-dipole interaction](electric-dipole-interaction.md) is

$$
H'= -\mathbf d\cdot\mathbf E=e\mathcal E z.
$$

The [first excited hydrogen eigenspace](first-excited-hydrogen-eigenspace.md) has a common unperturbed [energy eigenvalue](energy-eigenvalue-split.md) $E_2$. Write $|s\rangle=|2,0,0\rangle$ and $|p_m\rangle=|2,1,m\rangle$ in the [hydrogen energy eigenbasis](hydrogen-energy-eigenbasis.md). The [electric-dipole selection rules for hydrogen](electric-dipole-selection-rules-for-hydrogen.md) leave only the $s,p_0$ coupling within this [eigenspace](eigenspace.md). Each diagonal [matrix element](matrix-element.md) vanishes by [parity](parity.md), but that does not make the entire perturbation vanish. [Degenerate perturbation theory](degenerate-perturbation-theory.md) requires its [eigenvalues](eigenvalue.md) in the whole [eigenspace](eigenspace.md). With the usual real [wavefunction](wave-function-split.md) phases the off-diagonal position [matrix element](matrix-element.md) is $\langle s|z|p_0\rangle=-3a_0$.[Quantum Mechanics by Richard Fitzpatrick; Fitzpatrick, Linear Stark Effect, equations (7.82)–(7.86)](quantum-mechanics-by-richard-fitzpatrick/linear-stark-effect.md)

The factor three can be checked directly. Set $\rho=r/a_0$ and use normalized radial [wavefunctions](wave-function-split.md) and [spherical harmonics](spherical-harmonic.md):

$$
R_{20}=\frac{(2-\rho)e^{-\rho/2}}{2\sqrt2\,a_0^{3/2}},
\qquad
R_{21}=\frac{\rho e^{-\rho/2}}{2\sqrt6\,a_0^{3/2}},
\qquad
Y_{00}=\frac1{\sqrt{4\pi}},
\qquad
Y_{10}=\sqrt{\frac3{4\pi}}\cos\theta.
$$

The angular [integral](integral-split.md) is $\int Y_{00}^*\cos\theta Y_{10}\,d\Omega=1/\sqrt3$. Including $z=r\cos\theta$ and the radial volume factor $r^2$ then gives

$$
\langle s|z|p_0\rangle
=\frac{a_0}{24}\int_0^\infty\rho^4(2-\rho)e^{-\rho}\,d\rho
=\frac{a_0}{24}(2\cdot4!-5!)=-3a_0.
$$

Reversing the [quantum phase](quantum-phase.md) of $|p_0\rangle$ reverses this sign, with no change to the predicted [energy eigenvalues](energy-eigenvalue-split.md).

Thus the nontrivial two-dimensional block and its [determinant](determinant.md) equation are

$$
H'_{s,p_0}=e a_0\mathcal E
\begin{pmatrix}0&-3\\-3&0\end{pmatrix},
\qquad
\det(H'_{s,p_0}-\Delta E I)
=(\Delta E)^2-9e^2a_0^2\mathcal E^2=0.
$$

Consequently, for the displayed sign convention,

$$
|\psi_-\rangle=\frac{|s\rangle+|p_0\rangle}{\sqrt2},
\quad \Delta E_-=-3ea_0\mathcal E,
\qquad
|\psi_+\rangle=\frac{|s\rangle-|p_0\rangle}{\sqrt2},
\quad \Delta E_+=+3ea_0\mathcal E.
$$

The two remaining [energy eigenstates](energy-eigenstate.md) $|p_{+1}\rangle,|p_{-1}\rangle$ have zero first-order shifts. The slopes correspond to opposite [electric dipole moments](electric-dipole-moment.md), $\langle d_z\rangle=+3ea_0$ and $-3ea_0$. The [electric field](electric-field-split.md) selects combinations of opposite [parity](parity.md) that already have these dipole expectations at leading order. This is why applying [first-order nondegenerate perturbation theory](first-order-nondegenerate-perturbation-theory.md) separately to $2s$ and $2p_0$, and obtaining two zero diagonal entries, misses the splitting.

The approximation requires $ea_0|\mathcal E|$ small compared with the separation to other [principal quantum numbers](principal-quantum-number.md). For real [hydrogen atoms](hydrogen-atom.md), it also requires the relevant [electric-dipole interaction](electric-dipole-interaction.md) to dominate the small splittings omitted here, including the [Lamb shift](lamb-shift.md). At sufficiently small [electric fields](electric-field-split.md) a pre-existing nonzero $2s$–$2p$ separation must be retained before taking the limit. A simple two-state illustration with unperturbed separation $\delta>0$ has shifts relative to its mean

$$
E_\pm-\overline E=\pm\sqrt{(\delta/2)^2+(3ea_0\mathcal E)^2}.
$$

For $3ea_0|\mathcal E|\ll\delta$, the lower branch moves by $-(3ea_0\mathcal E)^2/\delta+O(\mathcal E^4)$ relative to its zero-field value. At $\delta=0$ the splitting is linear. This interpolation explains the importance of the [hydrogen energy-level degeneracy](hydrogen-energy-level-degeneracy.md); it is not a complete model of the [fine structure](fine-structure.md) multiplet.

**Table of contents**

- [Spectral components of the linear hydrogen Stark effect](spectral-components-of-the-linear-hydrogen-stark-effect.md)

## ↑ Ancestors (4)

1. [Stark effect](stark-effect.md)
2. [Mathematical physics](mathematical-physics-split.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2013/paper-1/2/c/solution.md)
