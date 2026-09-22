<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

**Distinguishable noninteracting particles.** Interpret $V$ as the same external one-particle potential for each particle; the total potential is $V(\mathbf r_1)+V(\mathbf r_2)$. The [Time-dependent Schrödinger equation](../../../../../time-dependent-schrodinger-equation.md) is

$$
\boxed{i\hbar\frac{\partial\Psi}{\partial t}=
\left[-\frac{\hbar^2}{2m}(\nabla_1^2+\nabla_2^2)
+V(\mathbf r_1)+V(\mathbf r_2)\right]\Psi.}
$$

Let $\widehat h\phi_a=\epsilon_a\phi_a$ and $\widehat h\phi_b=\epsilon_b\phi_b$, where $\widehat h=-\hbar^2\nabla^2/(2m)+V$. Applying $\widehat h_1+\widehat h_2$ to the product multiplies it by $\epsilon_a+\epsilon_b$. The time [derivative](../../../../../derivative.md) of $e^{-iEt/\hbar}$ multiplies it by $E$. Thus the proposed stationary product is a solution provided

$$
\boxed{E=\epsilon_a+\epsilon_b.}
$$

The [tensor product](../../../../../tensor-product.md) separates the two independent one-particle dynamics.

**Identical spin-one-half particles.** Identical [fermions](../../../../../fermion.md) require antisymmetry under exchange of the complete position-and-spin labels. First take $a,b$ to be distinct orthonormal spatial orbitals, and define

$$
\Phi_\pm(1,2)=\frac{\phi_a(\mathbf r_1)\phi_b(\mathbf r_2)
\pm\phi_b(\mathbf r_1)\phi_a(\mathbf r_2)}{\sqrt2}.
$$

The symmetric spatial state must multiply the antisymmetric [spin-one-half singlet state](../../../../../spin-one-half-singlet-state.md); the antisymmetric spatial state must multiply one of the three symmetric [spin-one-half triplet states](../../../../../spin-one-half-triplet-state.md). The four normalized possibilities, each with the common time factor $e^{-iEt/\hbar}$, are

$$
\begin{array}{c|c|c}
\text{spatial factor}&\text{spin factor}&(S,m_S)\\\hline
\Phi_+&\dfrac{|\uparrow\downarrow\rangle-|\downarrow\uparrow\rangle}{\sqrt2}&(0,0)\\[4pt]
\Phi_-&|\uparrow\uparrow\rangle&(1,1)\\
\Phi_-&\dfrac{|\uparrow\downarrow\rangle+|\downarrow\uparrow\rangle}{\sqrt2}&(1,0)\\[4pt]
\Phi_-&|\downarrow\downarrow\rangle&(1,-1)
\end{array}
$$

These are the required product states under [fermionic exchange symmetry](../../../../../fermi-dirac-statistics.md). If $a=b$, the antisymmetric spatial combination vanishes. Only the product $\phi_a(\mathbf r_1)\phi_a(\mathbf r_2)$ times the singlet remains, as required by the [Pauli exclusion principle](../../../../../pauli-exclusion-principle.md). A nonorthogonal pair would require different normalization factors; the displayed $1/\sqrt2$ assumes an orthonormal stationary-state basis.

**Weak repulsive [Coulomb interaction](../../../../../coulomb-interaction.md).** For fixed orbitals $a,b$, first-order [perturbation theory](../../../../../perturbation-theory.md) gives spatial [energy](../../../../../energy-split.md) shifts $J\pm K$. Here $J$ is the direct interaction [energy](../../../../../energy-split.md), while the exchange integral for repulsion strength $g>0$ is

$$
K=g\iint\frac{\phi_a^*(\mathbf r)\phi_b(\mathbf r)
\phi_b^*(\mathbf r')\phi_a(\mathbf r')}{|\mathbf r-\mathbf r'|}\,d^3r\,d^3r'\ge0.
$$

The positivity follows from the positive [Fourier transform](../../../../../fourier-transform-split.md) of the Coulomb kernel. Consequently [Coulomb exchange splitting of two orbitals](../../../../../coulomb-exchange-splitting-of-two-orbitals.md) gives

$$
\boxed{E_{\rm triplet}=\epsilon_a+\epsilon_b+J-K
\le E_{\rm singlet}=\epsilon_a+\epsilon_b+J+K.}
$$

All three triplet [spin](../../../../../spin.md) components remain degenerate for a spin-independent [Coulomb interaction](../../../../../coulomb-interaction.md). Their antisymmetric spatial factor vanishes at coincidence and reduces close encounters. The inequality is strict when $K>0$; for negligible orbital overlap, the splitting may vanish. This comparison fixes one particle in each of the specified orbitals and does not rank singlets with a different orbital occupation.

**Spin-zero bosons.** For one particle in each of the same distinct orthonormal orbitals, the [spin](../../../../../spin.md) factor is symmetric and [bosonic exchange symmetry](../../../../../bosonic-exchange-symmetry.md) requires $\Phi_+$. At coincident positions,

$$
|\Phi_+(\mathbf r,\mathbf r)|^2=2|\phi_a(\mathbf r)|^2|\phi_b(\mathbf r)|^2,
\qquad
|\Psi_D(\mathbf r,\mathbf r)|^2=|\phi_a(\mathbf r)|^2|\phi_b(\mathbf r)|^2.
$$

Thus the [bosonic coincidence enhancement in two orthogonal orbitals](../../../../../bosonic-coincidence-enhancement-in-two-orthogonal-orbitals.md) is

$$
\boxed{\frac{P_B(\mathbf r,\mathbf r)}{P_D(\mathbf r,\mathbf r)}=2.}
$$

These are joint [probability densities](../../../../../probability-density.md), or small-detector-volume limits; an exactly specified point has zero [probability](../../../../../probability.md) in a continuous distribution. If both particles occupy the same orbital, the properly normalized product is already symmetric and the corresponding enhancement relative to distinguishable particles in that same orbital is one. The paper's usual factor-two answer presumes distinct orthogonal input orbitals.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
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
