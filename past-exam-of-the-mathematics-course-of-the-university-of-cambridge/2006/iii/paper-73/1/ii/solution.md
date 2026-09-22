<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\mu_g=\gamma m$ for the gravitational parameter of the relative [Kepler orbit](../../../../../../kepler-orbit.md), and use [specific orbital energy](../../../../../../specific-orbital-energy.md) and momenta per unit reduced mass. The [Hamiltonian](../../../../../../hamiltonian.md) is

$$
E=\frac12\left(p_r^2+\frac{p_\theta^2}{r^2}+\frac{p_\phi^2}{r^2\sin^2\theta}\right)-\frac{\mu_g}{r}=-\frac{\mu_g}{2a}.
$$

If physical momenta rather than these specific momenta are used, multiply the actions by the reduced mass. This only introduces a constant factor into the [phase space](../../../../../../phase-space.md) measure and leaves the eccentricity fractions unchanged. The formulas in the question adopt the specific-action convention.

Here is an explicit local [canonical transformation](../../../../../../canonical-transformation.md). A separated complete integral of the [Hamilton-Jacobi equation](../../../../../../hamilton-jacobi-equation.md) is

$$
S(r,\theta,\phi;L,G,H)=H\phi+\int^{\theta}\sqrt{G^2-\frac{H^2}{\sin^2\vartheta}}\,d\vartheta+\int^r\sqrt{2E(L)+\frac{2\mu_g}{s}-\frac{G^2}{s^2}}\,ds,\qquad E(L)=-\frac{\mu_g^2}{2L^2}.
$$

Choose branches along an orbit and take $p_j=\partial S/\partial q_j$, $l=\partial S/\partial L$, $g=\partial S/\partial G$, $h=\partial S/\partial H$. Then

$$
dS=\sum_jp_j\,dq_j+l\,dL+g\,dG+h\,dH,
$$

whose exterior derivative proves preservation of the canonical [symplectic form](../../../../../../symplectic-form.md). Thus these variables are canonical, and the absolute [Jacobian determinant](../../../../../../jacobian-determinant.md) is one. The angular separation gives $G=|\mathbf r\times\mathbf v|$ and $H=G\cos i$, including the sign of the [angular momentum](../../../../../../angular-momentum.md) along the reference axis.

For clarity, the radial action can be evaluated rather than assumed. Let $r=a(1-e\cos u)$, with $u$ the [eccentric anomaly](../../../../../../eccentric-anomaly.md). Then $p_r=\sqrt{\mu_g/a}\,e\sin u/(1-e\cos u)$, and

$$
J_r=\frac1{2\pi}\oint p_r\,dr=\frac{\sqrt{\mu_g a}}{2\pi}\int_0^{2\pi}\frac{e^2\sin^2u}{1-e\cos u}\,du=\sqrt{\mu_g a}\bigl(1-\sqrt{1-e^2}\bigr)=L-G.
$$

In the integral, use $e^2\sin^2u/(1-e\cos u)=1+e\cos u-(1-e^2)/(1-e\cos u)$ and $\int_0^{2\pi}(1-e\cos u)^{-1}du=2\pi/\sqrt{1-e^2}$. The polar action is $J_\theta=G-|H|$, while the signed azimuthal action is $J_\phi=H$. The separated angular coordinates have the usual [Delaunay variables](../../../../../../delaunay-variables.md) interpretation: $g$ is the [argument of periapsis](../../../../../../argument-of-periapsis.md), and $h$ is the [longitude of ascending node](../../../../../../longitude-of-ascending-node.md). In particular,

$$
l=\frac{dE}{dL}\int\frac{dr}{p_r}=\frac{\mu_g^2}{L^3}\frac{a^{3/2}}{\sqrt{\mu_g}}\int(1-e\cos u)\,du=u-e\sin u
$$

with a suitable origin at [periapsis](../../../../../../periapsis.md), so $l$ is the [mean anomaly](../../../../../../mean-anomaly.md). We have therefore recovered

$$
L=\sqrt{\mu_g a},\qquad G=L\sqrt{1-e^2},\qquad H=G\cos i,
$$

not merely assigned names to the new coordinates.

For nondegenerate bound [Kepler orbits](../../../../../../kepler-orbit.md), the ranges are

$$
\boxed{0<L<\infty,\quad 0<G<L,\quad -G<H<G,\quad l,g,h\in\mathbb R/(2\pi\mathbb Z).}
$$

The boundaries describe circular, coplanar or radial degeneracies, where some angles cease to be defined; they have zero measure in the present calculation. The actions are canonical coordinates with nested bounds, rather than three independently unrestricted Cartesian coordinates. The square of $H$ alone would miss the distinction between prograde and retrograde inclinations.

By the [canonical transformation](../../../../../../canonical-transformation.md), the population measure becomes

$$
dN=F\!\left(-\frac{\mu_g^2}{2L^2}\right)dL\,dG\,dH\,dl\,dg\,dh.
$$

At fixed $L$, the condition $e'<e$ is $L\sqrt{1-e^2}<G<L$. Integrating all three angles and then $H$ gives

$$
N(e'<e)=(2\pi)^3\int_0^\infty F(E(L))\,dL\int_{L\sqrt{1-e^2}}^L2G\,dG=(2\pi)^3e^2\int_0^\infty F(E(L))L^2\,dL.
$$

Consequently the [Delaunay phase-volume proof of the thermal eccentricity distribution](../../../../../../delaunay-phase-volume-proof-of-the-thermal-eccentricity-distribution.md) yields

$$
\boxed{\frac{N(e'<e)}{N_{\rm bound}}=e^2,\qquad \frac{1}{N_{\rm bound}}\frac{dN}{de}=2e\quad(0\le e<1).}
$$

The PDF's $e^2$ dependence must be interpreted as a [cumulative distribution function](../../../../../../cumulative-distribution-function.md), not an eccentricity [probability density function](../../../../../../probability-density-function.md) or the value of the original six-dimensional [phase-space distribution function](../../../../../../phase-space-distribution-function.md). A finite value of $F(E)$ at every energy also does not suffice to make the total population finite: $F=1$ on all bound energies gives the divergent integral $\int_0^\infty L^2dL$. The fractions are well defined at each fixed energy, over a finite allowed energy range, or for an energy distribution with a finite total integral.

A [Boltzmann distribution](../../../../../../boltzmann-distribution.md) is therefore unnecessary. Any normalizable energy-only distribution has the same eccentricity marginal, although such a distribution is a collisionless steady state by [Jeans theorem](../../../../../../jeans-theorem.md). The marginal alone does not even prove stationarity: for $0<|\eta|<1$,

$$
f_t=F(E(L))\bigl[1+\eta\cos(l-n(L)t)\bigr],\qquad n(L)=\frac{\mu_g^2}{L^3},
$$

is a positive time-dependent solution of the [Collisionless Boltzmann equation](../../../../../../collisionless-boltzmann-equation.md) and has exactly the same eccentricity marginal after integration over $l$. **An observed $e^2$ cumulative law establishes neither thermal relaxation nor the age of the system or Universe.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
