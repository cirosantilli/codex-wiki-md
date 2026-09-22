<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a local electric-dipole response of order $n$, write

$$
P_i(\omega_s)=\epsilon_0\sum_{j_1\ldots j_n}\chi^{(n)}_{ij_1\ldots j_n}(\omega_s;\omega_1,\ldots,\omega_n)
E_{j_1}(\omega_1)\cdots E_{j_n}(\omega_n),\qquad
\omega_s=\sum_r\omega_r.
$$

Its susceptibility is a rank-$(n+1)$ [tensor](../../../../../tensor.md). Initially it has $3^{n+1}$ components in three dimensions, before symmetries and [frequency](../../../../../frequency.md) constraints are applied. [nonlinear-susceptibility tensor symmetry](../../../../../nonlinear-susceptibility-tensor-symmetry.md) involves several logically different restrictions.

[Neumann's principle](../../../../../neumann-s-principle.md) requires invariance under the material [point group](../../../../../point-group.md). For an operation $R$,

$$
\chi_{ij_1\ldots j_n}=R_{ia}R_{j_1b_1}\cdots R_{j_nb_n}\chi_{ab_1\ldots b_n}.
$$

For inversion, $R=-I$, so $\chi^{(n)}=(-1)^{n+1}\chi^{(n)}$. Thus **all even orders vanish in a centrosymmetric material's local bulk electric-dipole response**. In particular $\chi^{(2)}=0$ there, while $\chi^{(3)}$ is permitted. Surface symmetry breaking, an applied bias or nonlocal magnetic/quadrupole response lies outside that statement. A noncentrosymmetric crystal permits some second-order components, but other point-group operations can still eliminate a chosen component.

Intrinsic permutation symmetry follows from interchanging commuting input field factors, provided the associated [frequency](../../../../../frequency.md) labels are interchanged too. At second order,

$$
\chi^{(2)}_{ijk}(\omega_s;\omega_1,\omega_2)=\chi^{(2)}_{ikj}(\omega_s;\omega_2,\omega_1).
$$

For equal input [frequencies](../../../../../frequency.md) this makes the last two spatial indices symmetric, reducing 27 components to 18 before material symmetries. At unequal [frequencies](../../../../../frequency.md) it does not identify the two index arrangements with the arguments held fixed. Reality of the time-domain polarization separately gives

$$
\chi^{(n)}(-\omega_s;-\omega_1,\ldots,-\omega_n)=\chi^{(n)}(\omega_s;\omega_1,\ldots,\omega_n)^*.
$$

[causality](../../../../../causality.md) imposes dispersion relations; neither arbitrary real coefficients nor full index symmetry should be inferred merely from the word lossless.

[Kleinman symmetry](../../../../../kleinman-symmetry.md) is a stronger approximation far from relevant resonances when [frequency](../../../../../frequency.md) dispersion can be neglected. A frequency-independent effective interaction [energy](../../../../../energy-split.md) makes its derivatives interchangeable, allowing full permutation of output and input spatial indices. At second order a fully symmetric rank-three [tensor](../../../../../tensor.md) has $\binom{5}{3}=10$ components. Close to resonance or across a dispersive band, that reduction can fail even when [absorption](../../../../../absorption-electromagnetic-radiation.md) at the measured [frequencies](../../../../../frequency.md) is small. The original analysis distinguishes high-resonance electronic response from strongly dispersive lattice mechanisms and identifies additional symmetry constraints on the former.[abstract, mechanism dependence and additional symmetry requirements](../../../../../nonlinear-dielectric-polarization-in-optical-media-by-d-a-kleinman.md)

For an [isotropic fourth-rank susceptibility](../../../../../isotropic-fourth-rank-susceptibility.md),

$$
\chi^{(3)}_{ijkl}=a\delta_{ij}\delta_{kl}+b\delta_{ik}\delta_{jl}+c\delta_{il}\delta_{jk}.
$$

If the relevant input slots are fully interchangeable, the coefficients coincide and **$\chi_{xxxx}^{(3)}=3\chi_{xxyy}^{(3)}$**. With distinct or mixed-sign [frequency](../../../../../frequency.md) slots, [frequency](../../../../../frequency.md) arguments must be followed and isotropy alone leaves the three displayed structures. These distinctions explain why [tensor](../../../../../tensor.md) contractions, pump polarizations and operating [frequencies](../../../../../frequency.md) must be specified before comparing effective self- and cross-phase coefficients.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the nonlinear Optics and Quantum States of Light course of the University of Cambridge](../../../../split.md)
6. [Nonlinear Optics and Quantum States of Light course of the University of Cambridge](../../../../../nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
