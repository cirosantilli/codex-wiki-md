<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Spatial homogeneity](../../../../spatial-homogeneity.md) makes $\rho$ independent of position and makes the [two-particle number density](../../../../two-particle-number-density.md) depend only on the separation. [Isotropy](../../../../isotropy.md) removes its directional dependence. Consequently

$$
n_2(\mathbf x,\mathbf x_\star,t)=\rho^2g_2(|\mathbf x_\star-\mathbf x|,t).
$$

Here $g_2$ is a [radial distribution function](../../../../radial-distribution-function.md), with the finite-$N$ normalization inherited from [a](../a.md); statistical independence is unnecessary. In particular, the translated pair in [c](../c.md) has separation $\mathbf R$ for every $s$, so its $s$ integral is simply $\rho^2g_2(R,t)$.

[Isotropy](../../../../isotropy.md) of the random [velocity](../../../../velocity.md) $\mathbf c=\mathbf v-\mathbf u$ makes its second [velocity moment](../../../../velocity-moment.md) proportional to the identity. Taking its trace fixes the proportionality constant:

$$
\boxed{\theta=\frac1{3\rho}\int|\mathbf v-\mathbf u|^2f\,d^3v,\qquad P_{ij}=\rho\theta\delta_{ij}.}
$$

Thus $\theta$ is the one-component random [velocity](../../../../velocity.md) variance; for unit [mass](../../../../mass.md) in [thermal equilibrium](../../../../thermal-equilibrium-split.md), $\theta=k_BT$. A [Maxwell-Boltzmann velocity distribution](../../../../maxwell-boltzmann-velocity-distribution.md) is not required for the [pressure tensor](../../../../pressure-tensor.md) to be isotropic.

For the interaction contribution, the angular integral is $\int d\Omega\,\widehat R_i\widehat R_j=(4\pi/3)\delta_{ij}$, by [isotropy](../../../../isotropy.md) and its trace. With $d^3R=R^2\,dR\,d\Omega$, [c](../c.md) becomes

$$
P^\phi_{ij}=-\frac{2\pi}{3}\rho^2\delta_{ij}\int_0^\infty R^3\phi'(R)g_2(R,t)\,dR.
$$

Combining the two [pressure tensors](../../../../pressure-tensor.md) gives the [virial pressure from pair correlations](../../../../virial-pressure-from-pair-correlations.md):

$$
\boxed{\mathbf P+\mathbf P^\phi=p\mathbf I,\qquad p=\rho\theta-\frac{2\pi}{3}\rho^2\int_0^\infty R^3\phi'(R)g_2(R,t)\,dR.}
$$

For a repulsive [pair potential](../../../../pair-potential.md), the outward radial [force](../../../../force-split.md) is $-\phi'(R)\geq0$. Since $g_2\geq0$, the second term in $p$ is **nonnegative**, and positive when occupied separations feel nonzero repulsion. It expresses additional [momentum transfer](../../../../momentum-transfer.md) through interactions. The displayed integral assumes a differentiable [pair potential](../../../../pair-potential.md) and convergence; a hard core requires a contact formula or a limiting argument.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
