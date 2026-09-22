<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the reduced attractive [reduced BCS pairing Hamiltonian](../../../../../reduced-bcs-pairing-hamiltonian.md) with volume V, $\xi_k=\varepsilon_k-\mu$ and attraction $\lambda>0$:

$$
\mathcal H=\sum_{k\sigma}\xi_kc_{k\sigma}^\dagger c_{k\sigma}-\frac\lambda V B^\dagger B,\qquad
B=\sum_kc_{-k\downarrow}c_{k\uparrow}.
$$

A specified pairing shell or an ultraviolet renormalization is part of the model. The trace is grand canonical. Insert [fermionic coherent states](../../../../../fermionic-coherent-state.md) into its time-sliced trace. The resulting [Grassmann variables](../../../../../grassmann-variable.md) are antiperiodic, and with inverse-energy [imaginary time](../../../../../imaginary-time.md) $0\le\tau\le\beta$ the dimensionless action is

$$
\mathcal S=\int_0^\beta d\tau\left[\sum_{k\sigma}\bar\psi_{k\sigma}(\partial_\tau+\xi_k)\psi_{k\sigma}-\frac\lambda V\bar P P\right],\qquad
P=\sum_k\psi_{-k\downarrow}\psi_{k\uparrow}.
$$

This boundary condition is essential for [Fermi-Dirac statistics](../../../../../fermi-dirac-statistics.md); replacing it by a bosonic periodic trace changes the answer. A complex [Hubbard–Stratonovich transformation](../../../../../hubbard-stratonovich-transformation.md) uses the local identity

$$
e^{(\lambda/V)\bar P P}\propto\int d\Delta\,d\Delta^*\,
e^{-V|\Delta|^2/\lambda+\Delta\bar P+\Delta^*P},
$$

with time-slice factors understood. The pairing field renders the fermion action quadratic. For a uniform static field the independent [Nambu spinor](../../../../../nambu-spinor.md) block $(\psi_{k\uparrow},\bar\psi_{-k\downarrow})^T$ has

$$
\mathcal G^{-1}(k,i\omega_n)=
\begin{pmatrix}-i\omega_n+\xi_k&-\Delta\\-\Delta^*&-i\omega_n-\xi_k\end{pmatrix},\qquad
\omega_n=(2n+1)\pi/\beta,\qquad E_k=\sqrt{\xi_k^2+|\Delta|^2}.
$$

Its determinant is $-(\omega_n^2+E_k^2)$. The phase-independent determinant sign cancels under consistent reference normalization. Integrating the fermions gives the [BCS pairing-field effective action](../../../../../bcs-pairing-field-effective-action.md), $\mathcal S_{\rm eff}=\int_0^\beta V|\Delta|^2/\lambda\,d\tau-\operatorname{Tr}\ln\mathcal G^{-1}$, with the normal-ordering/reference term retained. The [fermionic pairing-block determinant normalization](../../../../../fermionic-pairing-block-determinant-normalization.md) uses one independent pairing block for every k; a fully doubled spin-particle-hole trace instead needs one half. The [subtracted grand potential of the reduced BCS model](../../../../../subtracted-grand-potential-of-the-reduced-bcs-model.md) is particularly unambiguous:

$$
\Omega(\Delta)-\Omega(0)=\frac{V|\Delta|^2}{\lambda}
-\frac1\beta\sum_{kn}\ln\frac{\omega_n^2+E_k^2}{\omega_n^2+\xi_k^2}.
$$

Performing the [Matsubara frequency](../../../../../matsubara-frequency.md) sum yields

$$
\Omega(\Delta)=\frac{V|\Delta|^2}{\lambda}
+\sum_k(\xi_k-E_k)-\frac2\beta\sum_k\ln(1+e^{-\beta E_k}),
$$

up to a common constant. At zero gap this reduces exactly to the two-spin free-gas result. The [Matsubara derivation of the BCS saddle](../../../../../matsubara-derivation-of-the-bcs-saddle.md) follows by differentiating with respect to $\Delta^*$ and using $\beta^{-1}\sum_n(\omega_n^2+E^2)^{-1}=\tanh(\beta E/2)/(2E)$ gives

$$
\boxed{1=\frac\lambda V\sum_k\frac{\tanh(\beta E_k/2)}{2E_k},\qquad
N=\sum_k\left[1-\frac{\xi_k}{E_k}\tanh\frac{\beta E_k}2\right].}
$$

The second equation fixes the [chemical potential](../../../../../chemical-potential-split.md) at specified number. This stationary action is BCS [mean-field theory](../../../../../mean-field-theory.md), not an exact integration of pairing-field fluctuations. With constant single-spin [density of states](../../../../../density-of-states.md) $\nu_F$ per volume and a symmetric energy cutoff $\Lambda$, weak coupling gives $\Delta(0)\simeq2\Lambda e^{-1/(\lambda\nu_F)}$ and $k_BT_c\simeq(2e^{\gamma_E}/\pi)\Lambda e^{-1/(\lambda\nu_F)}$. The zero-temperature condensation grand-potential density is $-\nu_F\Delta^2/2$ to leading weak-coupling order; using a spin-summed density would change these displayed factors. The [BCS coherence factors](../../../../../bcs-coherence-factors.md) are $u_k^2=(1+\xi_k/E_k)/2$ and $v_k^2=(1-\xi_k/E_k)/2$, and the associated [BCS ground state](../../../../../bcs-ground-state.md) is the normalized product of empty and occupied pair states. [Chapter11, BCS variational state, coherence factors, gap and thermal occupations](../../../../../lecture-notes-for-quantum-matter-by-steven-h-simon.md)

Allowing a slowly varying complex pairing field generates phase stiffness and, near the transition, the [Ginzburg-Landau theory of superconductivity](../../../../../ginzburg-landau-theory-of-superconductivity.md). A neutral paired system has a gapless phase sound mode; in a charged bulk superconductor electromagnetic coupling produces the [Anderson-Higgs mechanism in a superconductor](../../../../../anderson-higgs-mechanism-in-a-superconductor.md) and the [Meissner effect](../../../../../meissner-effect.md). These collective fluctuations are distinct from the gapped fermionic excitations. A microscopic dynamical calculation is needed to fix collective-mode dispersion and damping; the static saddle alone does not determine them. [§§3.1–3.2, coherent-state construction; §2.3, pair-field integration and charged phase dynamics](../../../../../physics-215c-quantum-field-theory-part-3-by-john-mcgreevy.md)

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
