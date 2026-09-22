<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $\mu=\gamma m$ for the gravitational parameter, to distinguish it from the Delaunay action called $G$. The displayed actions are per unit reduced mass. Accordingly use specific canonical momenta; with physical relative momenta, all three actions acquire a common reduced-mass factor, which leaves the eccentricity fraction below unchanged.

**The canonical transformation.** In spherical coordinates, separation of the Kepler [Hamilton-Jacobi equation](../../../../../../hamilton-jacobi-equation.md) gives

$$
p_\phi=H,\qquad p_\theta^2=G^2-\frac{H^2}{\sin^2\theta},\qquad p_r^2=2E+\frac{2\mu}{r}-\frac{G^2}{r^2},\qquad E=-\frac{\mu^2}{2L^2}.
$$

A local type-two generating function, continued across turning points with the appropriate momentum branches, is

$$
W=H\phi+\int^\theta\sqrt{G^2-H^2/\sin^2\theta'}\,d\theta'+\int^r\sqrt{-\mu^2/L^2+2\mu/r'-G^2/r'^2}\,dr'.
$$

The old momenta are $\partial W/\partial(r,\theta,\phi)$ and the new angles are $l=\partial_LW$, $g=\partial_GW$, $h=\partial_HW$. This defines a [canonical transformation](../../../../../../canonical-transformation.md), since its generating differential is $dW=p_rdr+p_\theta d\theta+p_\phi d\phi+l\,dL+g\,dG+h\,dH$. With standard choices of angle origins, the resulting [Delaunay variables](../../../../../../delaunay-variables.md) are

$$
L=\sqrt{\mu a},\qquad G=L\sqrt{1-e^2},\qquad H=G\cos i,
$$

with $l$ the [mean anomaly](../../../../../../mean-anomaly.md), $g$ the [argument of periapsis](../../../../../../argument-of-periapsis.md), and $h$ the [longitude of ascending node](../../../../../../longitude-of-ascending-node.md). In particular, the signed $H$ includes retrograde orbits; the squared equation in the PDF must not be read as $H\geq0$.

For bound noncollision [Kepler orbits](../../../../../../kepler-orbit.md), the independent ranges are

$$
\boxed{0<L<\infty,\quad0<G<L,\quad-G<H<G,\quad0\leq l,g,h<2\pi.}
$$

The limiting circular, radial and coplanar cases sit on boundaries where some angle charts degenerate. They have zero measure in the generic phase-volume calculation. The ranges are constrained as above, rather than a Cartesian box with three unconstrained actions.

**The eccentricity count.** A [canonical transformation](../../../../../../canonical-transformation.md) preserves [phase space](../../../../../../phase-space.md) volume, so

$$
dN=F(E(L))\,dL\,dG\,dH\,dl\,dg\,dh.
$$

Integrating the three angles contributes $(2\pi)^3$, and integrating $H$ gives $2G$. At fixed $L$, the condition that the [orbital eccentricity](../../../../../../orbital-eccentricity.md) be less than $e_0$ is $G>L\sqrt{1-e_0^2}$. Thus

$$
\int_{L\sqrt{1-e_0^2}}^L2G\,dG=L^2e_0^2,\qquad \int_0^L2G\,dG=L^2.
$$

Any energy weight cancels between these integrals. If the total population is finite, or an explicit finite action band is used,

$$
\boxed{N(e<e_0)=e_0^2N_{\rm tot},\qquad P(e<e_0)=e_0^2,\qquad f_e(e)=2e.}
$$

This is the [Delaunay phase-volume proof of the thermal eccentricity distribution](../../../../../../delaunay-phase-volume-proof-of-the-thermal-eccentricity-distribution.md). The source's $e^2$ law is a cumulative count, not a differential eccentricity density. Also, pointwise finite $F(E)$ does not alone imply finite $N_{\rm tot}$: $F=1$ gives $\int_0^\infty L^2dL=\infty$. The [finite normalization of an energy-only Kepler distribution](../../../../../../finite-normalization-of-an-energy-only-kepler-distribution.md) is the additional condition needed for a global probability statement; the fraction at every fixed energy is unaffected.

**Why the observation does not imply relaxation or equilibrium.** No [Boltzmann distribution](../../../../../../boltzmann-distribution.md) was used: every normalizable energy-only [phase-space distribution function](../../../../../../phase-space-distribution-function.md) has the same eccentricity marginal, irrespective of collisional thermalization. An even stronger counterexample is a genuinely time-dependent collisionless distribution

$$
f(L,G,H,l,g,h,t)=F(E(L))[1+\eta\cos(l-\nu(L)t)],\qquad0<|\eta|<1,\qquad\nu(L)=\frac{\mu^2}{L^3}.
$$

Kepler motion has $\dot l=\nu(L)$ and constant actions and other angles, so $\partial_tf+\nu\partial_lf=0$: this is an exact nonstationary solution of the [Collisionless Boltzmann equation](../../../../../../collisionless-boltzmann-equation.md). Integrating $l$ removes the cosine and leaves precisely the same $e^2$ cumulative count at every time. **An eccentricity marginal alone cannot establish thermal relaxation, a relaxed age, or even a stationary distribution.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
