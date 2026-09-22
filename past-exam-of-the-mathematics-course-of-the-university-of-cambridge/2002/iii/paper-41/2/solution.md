<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In the dominant central [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md), [conservation of energy](../../../../../conservation-of-energy.md) for gas falling from rest at infinity gives $u^2/2=GM_c/R$, hence $u=aR^{-1/2}$ with $a=(2GM_c)^{1/2}$. The characteristic stellar speed has the same radial scaling. For random stellar directions, the cross term in $|\boldsymbol u-\boldsymbol v|^2$ averages to zero, so the typical relative speed is also $V=bR^{-1/2}$. With the stated kinetic-energy estimate, an rms convention gives $V^2\simeq4GM_c/R$; another convention changes only the constant $b$.

In the steady spherical inflow approximation, [mass conservation](../../../../../mass-conservation.md) gives $A=4\pi R^2\rho u$. Thus

$$
\boxed{\rho(R)=\frac{A}{4\pi a}R^{-3/2},\qquad V\propto R^{-1/2}.}
$$

This leading calculation treats the inward gas flux as essentially undepleted over the region used. Substantial distributed removal by stars would make the local flux a function of $R$, an important limitation discussed below.

Insert these scalings in the [Bondi--Hoyle--Lyttleton accretion rate](../../../../../bondi-hoyle-lyttleton-accretion-rate.md). The factors $R^{3/2}$ from $V^{-3}$ and $R^{-3/2}$ from $\rho$ cancel:

$$
\dot M=4\pi G^2M^2b^{-3}R^{3/2}\frac{A}{4\pi a}R^{-3/2}
=\Lambda M^2,\qquad\boxed{\alpha=2,\quad\beta=0,\quad\Lambda=\frac{G^2A}{ab^3}.}
$$

This is [quadratic accretion in a central Keplerian potential](../../../../../quadratic-accretion-in-a-central-keplerian-potential.md). Write its fixed coefficient as $\lambda=\Lambda$. Integrating $d(1/M)/dt=-\lambda$ gives

$$
\boxed{M(t)=\frac{M_0}{1-\lambda M_0t},\qquad\lambda M_0t<1.}
$$

The cancellation of radius means that orbital variation of $R$ alone does not change this coefficient, provided the assumed steady gas profile, central mass and relative-velocity scaling remain fixed.

Conserve the number of stars along these deterministic mass trajectories. Inverting the map and taking its [Jacobian determinant](../../../../../jacobian-determinant.md) gives

$$
M_0=\frac{M}{1+\lambda Mt},\qquad\frac{dM_0}{dM}=\frac1{(1+\lambda Mt)^2}=\left(\frac{M_0}{M}\right)^2.
$$

The [mass-spectrum transport under quadratic accretion](../../../../../mass-spectrum-transport-under-quadratic-accretion.md) is therefore

$$
\boxed{F(M,t)=\left(\frac{M_0}{M}\right)^2F_0\left(\frac{M}{1+\lambda Mt}\right).}
$$

For a narrow but nonzero initial mass interval, the mapping stretches the high end especially strongly. If its endpoints are $m_1<m_2$, their evolved ratio is $(m_2/m_1)(1-\lambda m_1t)/(1-\lambda m_2t)$, which can become large as $t$ approaches $1/(\lambda m_2)$ from below. In an intermediate high-mass range with $\lambda Mt\gg1$, mapped back into a portion of the initial interval where $F_0$ changes little,

$$
F(M,t)\simeq\frac{F_0(M_*)}{(\lambda t)^2}M^{-2},\qquad\boxed{dN\propto M^{-2}\,dM.}
$$

Here $M_*$ is near $1/(\lambda t)$ on the populated side of the initial interval. Finite initial support gives a finite upper mass cutoff at every time before the earliest blow-up; this is an approximate broad-range [power law](../../../../../power-law.md), not a literal infinite tail of a finite pre-blow-up population. A strictly monochromatic initial population remains monochromatic under identical accretion coefficients and does not generate a spectrum.

The limitations of this [accretion](../../../../../accretion.md) model are substantial. The [star cluster](../../../../../star-cluster.md) must remain centrally dominated, and both the central mass and gas supply must remain effectively fixed. Stellar capture depletes the gas flux and eventually invalidates the $R^{-3/2}$ profile. Gas [pressure](../../../../../pressure.md), [angular momentum](../../../../../angular-momentum.md), [shocks](../../../../../shock-wave.md), radiative feedback and winds can reduce capture relative to the cold [Bondi–Hoyle accretion](../../../../../bondi-hoyle-accretion.md) estimate; a broad relative-speed distribution is not faithfully represented by one typical speed, especially because capture scales as $V^{-3}$. A growing star can perturb the surrounding potential, overlap capture regions, change its orbit through momentum loading, or compete with its neighbors for the same gas. Finally, number conservation excludes mergers, new star formation and stellar losses. The formal finite-time mass divergence cannot persist under a finite available gas mass, so the inferred mass-spectrum slope applies only while these approximations remain adequate.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
