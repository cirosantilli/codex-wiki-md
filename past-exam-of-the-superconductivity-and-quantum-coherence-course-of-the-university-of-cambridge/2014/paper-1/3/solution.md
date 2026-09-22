<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A complex [order parameter](../../../../order-parameter.md) captures both the amplitude and phase rigidity of a [superfluid](../../../../superfluid.md). A local isotropic [Ginzburg-Landau theory](../../../../ginzburg-landau-theory.md) writes its free-energy functional, to fourth order in amplitude and second order in gradients, as

$$
\mathcal F[\Psi]=\int d^3r\left[\alpha|\Psi|^2+\frac\beta2|\Psi|^4+K|\nabla\Psi|^2\right],\qquad \beta,K>0.
$$

The uniform minimum has $\Psi=0$ for $\alpha>0$ and $|\Psi_0|^2=-\alpha/\beta$ for $\alpha<0$. Its phase remains arbitrary under a global $U(1)$ transformation. Minimizing with respect to $\Psi^*$ gives $-K\nabla^2\Psi+\alpha\Psi+\beta|\Psi|^2\Psi=0$. The phenomenological description specifies the allowed structures and coefficients; microscopic input is needed to identify the normalization of $\Psi$ and calculate those coefficients. A static functional by itself does not fix the dynamical equation or mode frequencies.

For a dilute three-dimensional Bose gas with short-range repulsion and particle [mass](../../../../mass.md) $m_B$, the microscopic low-energy Hamiltonian is

$$
\widehat H=\int d^3r\left[
\frac{\hbar^2}{2m_B}\nabla\widehat\psi^\dagger\cdot\nabla\widehat\psi
+V_{\rm ext}\widehat\psi^\dagger\widehat\psi
+\frac{g_B}{2}\widehat\psi^\dagger\widehat\psi^\dagger\widehat\psi\widehat\psi\right],
\qquad g_B=\frac{4\pi\hbar^2a_s}{m_B}>0.
$$

The interaction parameter is expressed through the low-energy [s-wave scattering length](../../../../s-wave-scattering-length.md) $a_s$, rather than an unrenormalized bare delta potential. In a symmetry-selected description, $\Psi=\langle\widehat\psi\rangle$ and $|\Psi|^2=n_0$ is condensate density. Equivalently, fixed-number [off-diagonal long-range order](../../../../off-diagonal-long-range-order.md) identifies the macroscopically occupied natural orbital and its amplitude without a nonzero one-point expectation.

Evaluating $\widehat H-\mu\widehat N$ in a [coherent-field condensate variational state](../../../../coherent-field-condensate-variational-state.md) gives the [Ginzburg-Landau functional of a dilute Bose gas](../../../../ginzburg-landau-functional-of-a-dilute-bose-gas.md), with the mean-field microscopic identifications

$$
\boxed{K=\frac{\hbar^2}{2m_B},\qquad
\alpha=V_{\rm ext}-\mu,\qquad\beta=g_B.}
$$

Its stationary variational equation is the [Gross–Pitaevskii equation](../../../../gross-pitaevskii-equation.md). The time-dependent variational action additionally contains $i\hbar\Psi^*\partial_t\Psi$, giving

$$
i\hbar\partial_t\Psi=\left[-\frac{\hbar^2\nabla^2}{2m_B}+V_{\rm ext}+g_B|\Psi|^2\right]\Psi.
$$

This term expresses [density-phase conjugacy](../../../../density-phase-conjugacy.md). It is the missing microscopic dynamical input; a purely dissipative relaxation law would describe a different approximation.

[Bogoliubov theory](../../../../bogoliubov-theory.md) writes $\widehat\psi=\Psi+\delta\widehat\psi$ and retains quadratic fluctuations. In a uniform condensate, $\mu=g_Bn_0$ and the fluctuation matrix is

$$
\begin{pmatrix}
\epsilon_k+g_Bn_0&g_Bn_0\\
-g_Bn_0&-\epsilon_k-g_Bn_0
\end{pmatrix}.
$$

Its eigenvalues are $\pm\sqrt{\epsilon_k(\epsilon_k+2g_Bn_0)}$. The positive branch is the gapless sound mode, continuously crossing over to particle-like excitations at larger $k$. The same result follows by linearizing the time-dependent [Gross–Pitaevskii equation](../../../../gross-pitaevskii-equation.md) about its uniform solution. Thus the microscopic condensate amplitude, scattering interaction and [mass](../../../../mass.md) determine the mean-field static coefficients and the collective mode. Quadratic quantum fluctuations also produce [quantum depletion of a Bose condensate](../../../../quantum-depletion-of-a-bose-condensate.md), which a pure coherent-state product omits.

These identifications are controlled for a dilute weakly interacting gas away from a fluctuation-dominated critical region. They are not a universal statement that the exact finite-temperature GL coefficient is always $-\mu$ or that its quartic coefficient never receives corrections. Integrating out noncondensed and short-wavelength modes produces effective temperature-dependent coefficients and can change their near-critical behavior. The phase rigidity described by $K$ and the thermodynamic order-parameter expansion remain the shared organizing structure.

For [BCS theory](../../../../bcs-theory.md), the microscopic [order parameter](../../../../order-parameter.md) is instead an anomalous pair amplitude, commonly normalized as an [energy](../../../../energy-split.md) gap $\Delta\propto\langle\widehat\psi_\downarrow\widehat\psi_\uparrow\rangle$. It is not an ordinary single-electron field expectation or automatically the square root of a pair number density. Integrating out [fermions](../../../../fermion.md) and expanding in small $\Delta$ and slow gradients near $T_c$ gives the [microscopic derivation of Ginzburg-Landau theory](../../../../microscopic-derivation-of-ginzburg-landau-theory.md). The [BCS pairing-field effective action](../../../../bcs-pairing-field-effective-action.md) supplies its coefficients through normal-state pair-response functions and thermal [fermion](../../../../fermion.md) sums.

For example, a clean isotropic three-dimensional weak-coupling s-wave model, with $N(0)$ the [density of states](../../../../density-of-states.md) per spin at the [Fermi energy](../../../../fermi-energy.md) and $\Delta$ measured in [energy](../../../../energy-split.md) units, gives

$$
\mathcal F_s-\mathcal F_n=\int d^3r
\left[\alpha_\Delta|\Delta|^2+\frac{\beta_\Delta}{2}|\Delta|^4
+K_\Delta\left|\left(\nabla-\frac{iq\mathbf A}{\hbar}\right)\Delta\right|^2
+\frac{|\mathbf B|^2}{2\mu_0}\right],\qquad q=-2e,
$$

with [microscopic Ginzburg-Landau coefficients from BCS theory](../../../../microscopic-ginzburg-landau-coefficients-from-bcs-theory.md)

$$
\boxed{\alpha_\Delta\simeq N(0)\frac{T-T_c}{T_c},\qquad
\beta_\Delta=\frac{7\zeta(3)N(0)}{8\pi^2(k_BT_c)^2},\qquad
K_\Delta=\frac{7\zeta(3)N(0)\hbar^2v_F^2}{48\pi^2(k_BT_c)^2}.}
$$

The numerical factors arise from fermionic [Matsubara sums](../../../../bosonic-matsubara-sum.md) and the isotropic velocity average; they depend on the stated gap and density-of-states conventions. Rescaling the [order parameter](../../../../order-parameter.md) rescales all three coefficients. The expansion applies near the transition with sufficiently slow spatial variation; disorder, anisotropic pairing and strong coupling alter the coefficients or require additional components. Microscopic derivation also fixes the pair charge in the covariant gradient, producing the superconducting screening current and the [Meissner effect](../../../../meissner-effect.md).[1959, near-transition gap expansion and twice-electron charge](../../../../microscopic-derivation-of-the-ginzburg-landau-equations-in-the-theory-of-superconductivity-by-lev-gor-kov.md)

The neutral Bose and charged Fermi theories therefore share a complex [order parameter](../../../../order-parameter.md) and a phase-stiffness functional, while deriving that field from different microscopic objects. The [Bogoliubov transformation](../../../../bogoliubov-transformation.md) mixes particle and hole fluctuations of the bosonic condensate in one case and paired fermionic excitations in the other. The static GL limit organizes long-distance behavior; the full microscopic theories retain excitation spectra and [temperature](../../../../temperature-split.md) dependence beyond that local near-transition expansion.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the superconductivity and Quantum Coherence course of the University of Cambridge](../../../split.md)
5. [Superconductivity and Quantum Coherence course of the University of Cambridge](../../../../superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
