<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**First velocity moment.** Assume a stationary, spherical, nonstreaming [collisionless stellar system](../../../../../collisionless-stellar-system.md) with constant [mass-to-light ratio](../../../../../mass-to-light-ratio.md) $\Upsilon$. Use a luminosity-weighted [galactic distribution function](../../../../../galactic-distribution-function.md), with [luminosity density](../../../../../luminosity-density.md) $\lambda$. Multiplying the [Collisionless Boltzmann equation](../../../../../collisionless-boltzmann-equation.md) by $v_i$ and integrating over velocities, with its velocity-space boundary terms vanishing, gives

$$
\partial_j\big(\lambda\langle v_i v_j\rangle\big)=-\lambda\partial_i\Phi.
$$

Spherical symmetry makes the stress tensor

$$
T_{ij}=q_t\delta_{ij}+(q-q_t)\frac{x_ix_j}{r^2},\qquad q=\lambda\sigma_r^2,\qquad q_t=\lambda\sigma_t^2.
$$

Here $\sigma_t^2$ is one tangential component, as in the paper; the total tangential [variance](../../../../../variance-split.md) is $2\sigma_t^2$. Its radial divergence is $q'+2(q-q_t)/r$, since the divergence of the radial unit vector is $2/r$. With the [velocity-anisotropy parameter](../../../../../velocity-anisotropy-parameter.md) $\beta=1-\sigma_t^2/\sigma_r^2$, and enclosed [mass](../../../../../mass.md) $M(r)=\Upsilon L(r)$, this gives the [Spherical Jeans equation](../../../../../spherical-jeans-equation.md)

$$
\boxed{q'+\frac{2\beta q}{r}=-\lambda\Phi'(r)=-\gamma\frac{\lambda L(r)}{r^2},\qquad\gamma=G\Upsilon.}
$$

This uses a constant ratio of total gravitating mass to luminosity, rather than an arbitrary independent dark halo.

**Projection and elimination of anisotropy.** Write $R$ for projected radius and $r$ for spherical radius. The [Abel transform](../../../../../abel-transform.md) of the [luminosity density](../../../../../luminosity-density.md) gives

$$
\mu(R)=2\int_R^\infty\frac{\lambda(r)r\,dr}{\sqrt{r^2-R^2}},
$$

whose inverse is the displayed density inversion in the paper. At a point on this [line of sight](../../../../../line-of-sight.md), $\sin^2\theta=R^2/r^2$. The line-of-sight second [stellar velocity moment](../../../../../stellar-velocity-moment.md) is $\sigma_r^2\cos^2\theta+\sigma_t^2\sin^2\theta=\sigma_r^2(1-\beta R^2/r^2)$. Therefore the measured quantity $J(R)=\mu(R)\sigma_p^2(R)$ satisfies

$$
J(R)=2\int_R^\infty\left(1-\beta(r)\frac{R^2}{r^2}\right)\frac{q(r)r\,dr}{\sqrt{r^2-R^2}}.
$$

The [Spherical Jeans equation](../../../../../spherical-jeans-equation.md) gives $\beta q=-rq'/2-\gamma\lambda L/(2r)$. Substitution yields

$$
J(R)=2\int_R^\infty\frac{q(r)r\,dr}{\sqrt{r^2-R^2}}+R^2\int_R^\infty\frac{q'(r)\,dr}{\sqrt{r^2-R^2}}+\gamma R^2\int_R^\infty\frac{\lambda(r)L(r)\,dr}{r^2\sqrt{r^2-R^2}}.
$$

The inner $\gamma L$ printed in the PDF's definition of $p$ must therefore be $\lambda L$: the literal expression has an extra gravitational factor and lacks the density. Both this derivation and dimensional consistency require the correction. Define the [projected spherical Jeans residual](../../../../../projected-spherical-jeans-residual.md) by

$$
p(R)=J(R)-\gamma R^2\int_R^\infty\frac{\lambda(r)L(r)\,dr}{r^2\sqrt{r^2-R^2}}.
$$

To express it entirely in terms of the radial stress, put

$$
A(R)=\int_R^\infty\frac{q(r)r\,dr}{\sqrt{r^2-R^2}}=\int_0^\infty q\!\left(\sqrt{R^2+z^2}\right)dz.
$$

Differentiating the nonsingular $z$ representation gives $A'(R)=R\int_R^\infty q'(r)/\sqrt{r^2-R^2}\,dr$. Hence

$$
\boxed{p(R)=2A(R)+RA'(R)=\frac1R\frac{d}{dR}[R^2A(R)].}
$$

If $R^2A$ vanishes at zero and infinity, then $\int_0^\infty6\pi Rp(R)\,dR=6\pi[R^2A]_0^\infty=0$. These are the absence-of-boundary-stress conditions needed for the global result.

**The virial relation, term by term.** Interchange the order in the residual integral and use

$$
\int_0^r\frac{R^3\,dR}{\sqrt{r^2-R^2}}=r^3\int_0^{\pi/2}\sin^3\theta\,d\theta=\frac23r^3.
$$

It follows that

$$
\int_0^\infty6\pi Rp(R)\,dR=6\pi\int_0^\infty RJ(R)\,dR-4\pi\gamma\int_0^\infty r\lambda(r)L(r)\,dr.
$$

The first term is $2K/\Upsilon$: spherical averaging assigns one third of the integrated velocity-square to any fixed viewing direction, giving $K=3\pi\Upsilon\int RJ\,dR$. The gravitational potential energy is

$$
W=-\int_0^\infty\frac{GM(r)}r\,dM(r)=-4\pi G\Upsilon^2\int_0^\infty r\lambda(r)L(r)\,dr.
$$

Thus the integrated residual is exactly $(2K+W)/\Upsilon$, and its vanishing is the [virial theorem](../../../../../virial-theorem.md). Solving for $\gamma$ gives the [global projected virial estimate of a mass-to-light ratio](../../../../../global-projected-virial-estimate-of-a-mass-to-light-ratio.md),

$$
\boxed{\gamma=\frac{3\int_0^\infty R\mu(R)\sigma_p^2(R)\,dR}{2\int_0^\infty r\lambda(r)L(r)\,dr}.}
$$

It is independent of the radial anisotropy profile when the full aperture and the stated boundary conditions are used. A finite aperture retains a boundary term.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
