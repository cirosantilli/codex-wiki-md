<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work in an inertial frame centred on the [centre of mass](../../../../../../center-of-mass.md), and follow a fixed material mass, with no [stellar wind](../../../../../../stellar-wind.md) or accretion through its boundary. Assume nonrelativistic motion, Newtonian self-gravity, no external gravitational field, and sufficiently regular integrable fields. Define

$$
I=\int r^2\,dm,\qquad \mathcal T=\frac12\int |\mathbf v|^2\,dm,\qquad
\Omega=-\frac G2\iint\frac{dm\,dm'}{|\mathbf r-\mathbf r'|}=\frac12\int\rho\Phi\,dV.
$$

Here $I$ is the [scalar second mass moment](../../../../../../scalar-second-mass-moment.md), rather than a moment of inertia about one axis. The [kinetic energy](../../../../../../kinetic-energy.md) $\mathcal T$ measures resolved internal motions relative to the [centre of mass](../../../../../../center-of-mass.md); random microscopic motion contributes to [pressure](../../../../../../pressure.md) and [internal energy](../../../../../../internal-energy.md), and must not be counted again in $\mathcal T$.

The paper's symmetric compressive tensor $\mathbb P$ is minus the tensile [stress](../../../../../../stress.md) tensor, so its force per unit volume is $-\partial_jP_{ij}$. Differentiating the material integral twice and substituting the equation of motion gives

$$
\frac12\ddot I=2\mathcal T-\int r_i\partial_jP_{ij}\,dV-\int\mathbf r\cdot\nabla\Phi\,dm.
$$

[Integration by parts](../../../../../../integration-by-parts.md) and the [divergence theorem](../../../../../../divergence-theorem.md) turn the stress contribution into

$$
-\int r_i\partial_jP_{ij}\,dV=\int\operatorname{tr}\mathbb P\,dV-\oint r_iP_{ij}n_j\,dS.
$$

For the requested scalar [stellar virial theorem](../../../../../../stellar-virial-theorem.md), assume isotropic [pressure](../../../../../../pressure.md), $P_{ij}=P\delta_{ij}$, with uniform surface pressure $P_S$. Then $\operatorname{tr}\mathbb P=3P$ and the surface integral is $P_S\oint\mathbf r\cdot\mathbf n\,dS=3P_SV$. No spherical shape is needed for this step.

Finally, symmetrizing the pair integral for the [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md) gives

$$
-\int\mathbf r\cdot\nabla\Phi\,dm
=-\frac G2\iint\frac{(\mathbf r-\mathbf r')\cdot(\mathbf r-\mathbf r')}{|\mathbf r-\mathbf r'|^3}\,dm\,dm'=\Omega.
$$

Therefore

$$
\boxed{\frac12\ddot I=2\mathcal T+3\int P\,dV-3P_SV+\Omega.}
$$

Anisotropic magnetic or viscous stresses retain their full trace and boundary terms; a changing integration mass adds transport terms.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
