<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $u_i=\langle v_i\rangle$, $\sigma_{ij}=\langle(v_i-u_i)(v_j-u_j)\rangle$, and $P_{ij}=\rho\sigma_{ij}$. The [Jeans equation](../../../../../jeans-equation.md) obtained by taking the first [velocity](../../../../../velocity.md) moment of the [Collisionless Boltzmann equation](../../../../../collisionless-boltzmann-equation.md) is

$$
\partial_t(\rho u_j)+\partial_k(\rho u_ju_k+P_{jk})=-\rho\partial_j\Phi.
$$

For an equilibrium population multiply by $x_i$ and integrate. [Integration by parts](../../../../../integration-by-parts.md) gives

$$
\oint x_i(\rho u_ju_k+P_{jk})n_k\,dS-\int(\rho u_iu_j+P_{ji})\,d^3x=-\int\rho x_i\partial_j\Phi\,d^3x.
$$

Assume the integrals exist and the boundary flux vanishes, as for an isolated finite system with adequate decay. With the [stellar kinetic-energy tensor](../../../../../stellar-kinetic-energy-tensor.md), [stellar pressure-energy tensor](../../../../../stellar-pressure-energy-tensor.md) and [stellar potential-energy tensor](../../../../../stellar-potential-energy-tensor.md) defined by

$$
T_{ij}=\frac12\int\rho u_iu_j\,d^3x,\qquad \Pi_{ij}=\int\rho\sigma_{ij}\,d^3x,\qquad W_{ij}=-\int\rho x_i\partial_j\Phi\,d^3x,
$$

we obtain the equilibrium [tensor virial theorem](../../../../../tensor-virial-theorem.md)

$$
\boxed{2T_{ij}+\Pi_{ij}+W_{ij}=0.}
$$

The [stellar kinetic-energy tensor](../../../../../stellar-kinetic-energy-tensor.md) describes ordered motion, whereas the [stellar pressure-energy tensor](../../../../../stellar-pressure-energy-tensor.md) describes random motion. In particular, $T_{ij}=0$ does not mean the [stars](../../../../../star.md) have no [kinetic energy](../../../../../kinetic-energy.md). If a surface flux is retained, the right side of the displayed equilibrium identity is that surface tensor; it cannot be discarded for an arbitrary finite aperture. For an isolated self-gravitating population, $W_{ij}$ is symmetric by pairwise interchange in the Newtonian interaction integral, and the time-dependent identity is $\tfrac12\ddot I_{ij}=2T_{ij}+\Pi_{ij}+W_{ij}$ with $I_{ij}=\int\rho x_ix_jd^3x$.

For the spherical [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md), $\partial_j\Phi=\Phi'(r)x_j/r$. In the pressure-supported case the [tensor virial theorem](../../../../../tensor-virial-theorem.md) gives $\Pi_{ii}=\int\rho\Phi'(r)x_i^2/r\,d^3x$. The notation $\Pi_{RR}$ used in this question is the [planar virial trace](../../../../../planar-virial-trace.md) $\Pi_{xx}+\Pi_{yy}$, not just the integral of the local cylindrical radial [velocity dispersion](../../../../../velocity-dispersion.md). In [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md) this trace includes both $v_R^2$ and $v_\phi^2$. Summing the two Cartesian components therefore gives

$$
\boxed{\frac{\Pi_{RR}}{\Pi_{zz}}=\frac{\int\rho\Phi'(r)R^2/r\,d^3x}{\int\rho\Phi'(r)z^2/r\,d^3x}.}
$$

The distinction explains the factor of two in the spherical limit.

Use ordinary [spherical coordinates](../../../../../spherical-coordinate-system.md), $R=r\sin\theta$, $z=r\cos\theta$. The [mass density](../../../../../density.md) separates as $\rho_0r^{-\gamma}h(\theta)$, where

$$
h(\theta)=(\sin^2\theta+q^{-2}\cos^2\theta)^{-\gamma/2}.
$$

Both potential-energy integrals have the same radial factor $2\pi\rho_0\int_0^\infty r^{3-\gamma}\Phi'(r)\,dr$. When this factor is finite and positive it cancels, leaving the [scale-free tracer virial ratio](../../../../../scale-free-tracer-virial-ratio.md)

$$
\boxed{\frac{\Pi_{RR}}{\Pi_{zz}}=\frac{\int_0^\pi\sin^3\theta\,(\sin^2\theta+q^{-2}\cos^2\theta)^{-\gamma/2}\,d\theta}{\int_0^\pi\sin\theta\cos^2\theta\,(\sin^2\theta+q^{-2}\cos^2\theta)^{-\gamma/2}\,d\theta}.}
$$

**The angular factor in the printed intermediate formula has its sine and cosine interchanged.** Keeping its sine/cosine weights while using that printed factor would instead produce the opposite sign in the final small-flattening correction. Merely measuring $\theta$ from the equatorial plane cannot fix this: the measure and both moment weights would have to change as well.

The angular ratio is finite and positive for every fixed $q>0$ and finite real $\gamma$, because $h$ is positive and bounded above and below. However, the claim that the unrestricted global virial integrals are always well-defined needs a hypothesis. In a point-mass [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md), the common radial factor is proportional to $\int_0^\infty r^{1-\gamma}dr$: convergence at zero requires $\gamma<2$, while convergence at infinity requires $\gamma>2$. There is no such $\gamma$. If the global energies diverge, the boxed angular ratio is still the ratio of the two potential-energy integrals with identical spherical inner and outer cutoffs, independent of the cutoffs. It is not a quotient of two finite global [stellar pressure-energy tensors](../../../../../stellar-pressure-energy-tensor.md); applying a finite-aperture [tensor virial theorem](../../../../../tensor-virial-theorem.md) additionally requires its surface terms. These convergence and boundary qualifications are separate from the printed angular typo.

Set $\epsilon=q^{-2}-1$. For modest flattening, the [Taylor expansion](../../../../../taylor-expansion.md) is $h=1-(\gamma/2)\epsilon\cos^2\theta+O(\epsilon^2)$. The required elementary angular [integrals](../../../../../integral.md) are

$$
\int_0^\pi\sin^3\theta\,d\theta=\frac43,\quad \int_0^\pi\sin^3\theta\cos^2\theta\,d\theta=\frac4{15},\quad \int_0^\pi\sin\theta\cos^2\theta\,d\theta=\frac23,\quad \int_0^\pi\sin\theta\cos^4\theta\,d\theta=\frac25.
$$

These follow directly by $t=\cos\theta$, or from the supplied [gamma function](../../../../../gamma-function.md) identity. Hence the numerator is $(4/3)[1-\gamma\epsilon/10+O(\epsilon^2)]$ and the denominator is $(2/3)[1-3\gamma\epsilon/10+O(\epsilon^2)]$. The [flattening–anisotropy virial relation](../../../../../flattening-anisotropy-virial-relation.md) becomes

$$
\boxed{\frac{\Pi_{RR}}{2\Pi_{zz}}=1+\frac\gamma5(q^{-2}-1)+O((q^{-2}-1)^2).}
$$

For a decreasing tracer [mass density](../../../../../density.md) ($\gamma>0$), oblate flattening ($q<1$) requires more random kinetic support per in-plane direction than vertically. In a spherical [Newtonian gravitational field](../../../../../newtonian-gravitational-field.md), directional orbital anisotropy supplies the flattening rather than an anisotropic force law. A steeper radial [mass density](../../../../../density.md) amplifies the required [velocity dispersion](../../../../../velocity-dispersion.md) anisotropy. A prolate tracer reverses the leading inequality. The relation constrains integrated [velocity dispersions](../../../../../velocity-dispersion.md), not a unique local [galactic distribution function](../../../../../galactic-distribution-function.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
