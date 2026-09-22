<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**An ionic atmosphere.** A negatively charged [molecule](../../../../molecule-split.md) attracts positive [counterions](../../../../counterion.md) and repels negative [co-ions](../../../../co-ion.md); signs reverse for a positive [molecule](../../../../molecule-split.md). The resulting [electric double layer](../../../../electric-double-layer.md) partially screens the bare [electric field](../../../../electric-field-split.md). Far from an isolated molecule, the [electrolyte](../../../../electrolyte.md) recovers its neutral bulk composition. At [thermodynamic equilibrium](../../../../thermodynamic-equilibrium.md), spatial uniformity of each species' [electrochemical potential](../../../../electrochemical-potential.md) requires

$$
\mu_i=\mu_i^0+k_BT\ln n_i(\mathbf r)+z_i e\psi(\mathbf r),\qquad
\boxed{n_i(\mathbf r)=n_i^\infty e^{-z_ie\psi(\mathbf r)/(k_BT)}}.
$$

The logarithm implicitly uses a common reference density. This result for [Boltzmann ion densities in a symmetric electrolyte](../../../../boltzmann-ion-densities-in-a-symmetric-electrolyte.md) neglects ion correlations, finite size and nonideal activities, but shows immediately why equal concentrations of the two signs do not persist close to a charged surface.

**Self-consistent screening.** Insert these densities into [Poisson's equation](../../../../poisson-s-equation.md), with solvent permittivity $\epsilon$ and fixed charge density $\rho_f$:

$$
-\epsilon\nabla^2\psi=\rho_f+\sum_i z_ie n_i^\infty
 e^{-z_ie\psi/(k_BT)}.
$$

This is the [Poisson-Boltzmann equation](../../../../poisson-boltzmann-equation.md). For a symmetric monovalent salt with bulk density $n_s$ of _each_ sign, outside the fixed charge it becomes

$$
\nabla^2\psi=\frac{2en_s}{\epsilon}\sinh\left(\frac{e\psi}{k_BT}\right).
$$

For $|z_i e\psi|\ll k_BT$, linearizing and using bulk neutrality gives the [Debye–Hückel approximation](../../../../debye-huckel-approximation.md)

$$
\nabla^2\psi=\kappa^2\psi,\qquad
\boxed{\kappa^2=\frac{e^2}{\epsilon k_BT}\sum_i z_i^2n_i^\infty,
\quad\lambda_D=\kappa^{-1}}.
$$

Thus added salt shortens the [Debye length](../../../../debye-length.md): [electrostatic screening](../../../../electrostatic-screening.md) becomes stronger over a shorter distance. The factor of two in a $1{:}1$ salt comes from two ionic species, not from double-counting the density of salt pairs.

For example, a charged sphere of radius $a$ and total charge $Q$ has the exterior linearized solution

$$
\psi(r)=\frac{Q}{4\pi\epsilon(1+\kappa a)}\frac{e^{-\kappa(r-a)}}r,
\qquad r\ge a,
$$

assuming fixed uniform surface charge and no ions inside. It follows from the decaying spherical solution and $-\epsilon\psi'(a)=Q/(4\pi a^2)$. At zero salt it reduces to the [Coulomb potential](../../../../coulomb-potential-energy.md); at finite salt it decays exponentially as well as geometrically. The excess mobile charge integrates to $-Q$ in an infinite neutralizing reservoir, although a finite sphere surrounding the molecule generally contains only part of that ionic atmosphere.

**Biophysical scales and limitations.** In [water](../../../../water.md) at room [temperature](../../../../temperature-split.md), the monovalent formula is approximately $\lambda_D=0.304\,\mathrm{nm}/\sqrt{I/(\mathrm{mol\,L^{-1}})}$, with $I$ the [ionic strength](../../../../ionic-strength.md). It gives about $0.79\,\mathrm{nm}$ at $0.15\,\mathrm{mol\,L^{-1}}$ and $9.6\,\mathrm{nm}$ at $1\,\mathrm{mmol\,L^{-1}}$. Consequently the same charged [protein](../../../../protein-split.md) can exert very different long-range interactions mediated by [electrostatics](../../../../electrostatics-split.md) at different salt concentrations. Close to strongly charged [DNA](../../../../deoxyribonucleic-acid.md), the linear approximation fails; nonlinear screening, [counterion condensation](../../../../counterion-condensation.md), ion-specific adsorption and changes of surface ionization through [charge regulation](../../../../charge-regulation.md) may matter. [Mean-field theory](../../../../mean-field-theory.md) also misses strong multivalent-ion correlations and finite-size saturation: the exponential law cannot be extrapolated to arbitrarily large near-surface concentrations.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
