<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Assume a stationary, spherical, nonrotating [collisionless stellar system](../../../../../collisionless-stellar-system.md), a constant [mass-to-light ratio](../../../../../mass-to-light-ratio.md) $\Upsilon$, and vanishing boundary stresses at infinity. Let $\lambda$ be the [luminosity density](../../../../../luminosity-density.md), so $\rho=\Upsilon\lambda$, and set $\gamma=G\Upsilon$. Distinguish spatial radius $r$ from projected radius $R$. The enclosed [luminosity](../../../../../luminosity.md) and radial force are

$$
L(r)=4\pi\int_0^r\lambda(s)s^2\,ds,\qquad \Phi'(r)=\frac{GM(r)}{r^2}=\frac{\gamma L(r)}{r^2}.
$$

Here $\sigma_t^2$ is the [velocity dispersion](../../../../../velocity-dispersion.md) of either one of the two tangential components; thus $\beta=1-\sigma_t^2/\sigma_r^2$. If a combined tangential variance is used instead, its contribution must be divided by two in this definition.

To derive the [Jeans equation](../../../../../jeans-equation.md), start with the steady [Collisionless Boltzmann equation](../../../../../collisionless-boltzmann-equation.md) $v_j\partial_j f-(\partial_j\Phi)\partial_{v_j}f=0$. Multiply by $v_i$ and integrate over all velocities. [Integration by parts](../../../../../integration-by-parts.md) in velocity, with $f$ decaying fast enough to eliminate boundary terms, gives

$$
\partial_j\bigl(\lambda\overline{v_iv_j}\bigr)=-\lambda\partial_i\Phi.
$$

The same equation holds with luminosity weighting because the tracer's luminosity is conserved along its orbit. Spherical symmetry makes the local [stellar velocity moment](../../../../../stellar-velocity-moment.md) tensor diagonal, with entries $q=\lambda\sigma_r^2$, $q_t=\lambda\sigma_t^2$, $q_t$. Its radial [divergence](../../../../../divergence.md) is $q'+(2q-2q_t)/r$: the second term accounts for the changing directions of the radial and tangential unit vectors. Therefore

$$
\boxed{\frac{d(\lambda\sigma_r^2)}{dr}+\frac{2\beta}{r}\lambda\sigma_r^2=-\frac{\gamma\lambda L(r)}{r^2}.}
$$

This is the [Spherical Jeans equation](../../../../../spherical-jeans-equation.md); it follows from a [stellar velocity moment](../../../../../stellar-velocity-moment.md) rather than requiring a particular form of the [galactic distribution function](../../../../../galactic-distribution-function.md).

Integrating the [luminosity density](../../../../../luminosity-density.md) along a line of sight gives its [surface brightness](../../../../../surface-brightness.md):

$$
\mu(R)=2\int_R^\infty\frac{\lambda(r)r\,dr}{\sqrt{r^2-R^2}},\qquad \lambda(r)=-\frac1\pi\int_r^\infty\frac{\mu'(R)\,dR}{\sqrt{R^2-r^2}}.
$$

The second identity is [Spherical Abel deprojection](../../../../../spherical-abel-deprojection.md). For the second [stellar velocity moment](../../../../../stellar-velocity-moment.md), the angle between the radial direction and the line of sight has $\sin^2\theta=R^2/r^2$. The line-of-sight [velocity dispersion](../../../../../velocity-dispersion.md) is therefore $\sigma_r^2\cos^2\theta+\sigma_t^2\sin^2\theta=\sigma_r^2(1-\beta R^2/r^2)$, and

$$
S(R)\equiv\mu(R)\sigma_p^2(R)=2\int_R^\infty\left(1-\beta(r)\frac{R^2}{r^2}\right)\frac{q(r)r\,dr}{\sqrt{r^2-R^2}}.
$$

From the [Spherical Jeans equation](../../../../../spherical-jeans-equation.md), $\beta q=-rq'/2-\gamma\lambda L/(2r)$. Substitution produces

$$
S(R)=2\int_R^\infty\frac{q(r)r\,dr}{\sqrt{r^2-R^2}}+R^2\int_R^\infty\frac{q'(r)\,dr}{\sqrt{r^2-R^2}}+\gamma R^2\int_R^\infty\frac{\lambda(r)L(r)\,dr}{r^2\sqrt{r^2-R^2}}.
$$

The primary PDF has a genuine symbol error in its projected gravity term: it prints a second $\gamma$ multiplying $L$ inside the integral, where $\lambda$ is required. The corrected [projected spherical Jeans residual](../../../../../projected-spherical-jeans-residual.md) is

$$
\boxed{p(R)=S(R)-\gamma R^2\int_R^\infty\frac{\lambda(r)L(r)\,dr}{r^2\sqrt{r^2-R^2}}=2A(R)+RA'(R),\quad A(R)=\int_R^\infty\frac{q(r)r\,dr}{\sqrt{r^2-R^2}}.}
$$

To justify the derivative at the singular-looking lower limit, write $A(R)=\int_0^\infty q(\sqrt{R^2+z^2})\,dz$. Differentiation then gives $A'(R)=R\int_R^\infty q'(r)(r^2-R^2)^{-1/2}dr$. In particular, $Rp=(R^2A)'$. If $R^2A$ tends to zero both at zero and infinity, as for a finite isolated equilibrium with sufficiently decaying stresses,

$$
\int_0^\infty 6\pi R p(R)\,dR=6\pi[R^2A(R)]_0^\infty=0.
$$

If a boundary stress survives, its contribution must be retained; the zero-integral statement is not a finite-aperture identity.

Now identify each integral with a term in the [virial theorem](../../../../../virial-theorem.md). Let $K$ be the total [kinetic energy](../../../../../kinetic-energy.md), including all three random components, and $W$ the [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) energy. Averaging over spatial directions in a spherical system gives one third of the total [stellar velocity moment](../../../../../stellar-velocity-moment.md) along any chosen line of sight, even if the velocities are locally anisotropic. Thus

$$
2\pi\int_0^\infty R S(R)\,dR=\int\lambda\overline{v_{\rm los}^2}\,d^3x=\frac{2K}{3\Upsilon},\qquad K=3\pi\Upsilon\int_0^\infty R S(R)\,dR.
$$

Building the spherical mass shell by shell gives

$$
W=-\int_0^\infty\frac{GM(r)}{r}\,dM(r)=-4\pi G\Upsilon^2\int_0^\infty r\lambda(r)L(r)\,dr=-4\pi\gamma\Upsilon\int_0^\infty r\lambda L\,dr.
$$

Finally, [Fubini theorem](../../../../../fubini-s-theorem.md) and $\int_0^r R^3(r^2-R^2)^{-1/2}dR=2r^3/3$ give the gravitational contribution to the residual integral explicitly:

$$
6\pi\gamma\int_0^\infty R^3dR\int_R^\infty\frac{\lambda(r)L(r)\,dr}{r^2\sqrt{r^2-R^2}}=4\pi\gamma\int_0^\infty r\lambda L\,dr=-\frac{W}{\Upsilon}.
$$

Consequently

$$
\boxed{6\pi\int_0^\infty Rp(R)\,dR=\frac{2K+W}{\Upsilon},\qquad \gamma=\frac{3\int_0^\infty R\sigma_p^2(R)\mu(R)\,dR}{2\int_0^\infty r\lambda(r)L(r)\,dr}.}
$$

The [global projected virial estimate of a mass-to-light ratio](../../../../../global-projected-virial-estimate-of-a-mass-to-light-ratio.md) is independent of the [velocity-anisotropy parameter](../../../../../velocity-anisotropy-parameter.md) under these assumptions. It does not remove the [mass--anisotropy--density degeneracy](../../../../../mass-anisotropy-density-degeneracy.md) for arbitrary radial mass profiles. In particular, if an independent [dark matter halo](../../../../../dark-matter-halo.md) makes mass fail to follow light, a single constant $\Upsilon$ is no longer the physical enclosed mass-to-light ratio at every radius.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
