# Paper 66

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper66.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper66.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
    - [1](#4/i/1)
      - [Solution](#4/i/1/solution)
    - [2](#4/i/2)
      - [Solution](#4/i/2/solution)
    - [3](#4/i/3)
      - [Solution](#4/i/3/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

**The separated disk modes.** Away from the plane of a [razor-thin disk](../../../astrophysics.md#razor-thin-disk-approximation), there is no volume source, so the [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential) obeys the [Laplace equation in cylindrical coordinates](../../../partial-differential-equation.md#laplace-equation-in-cylindrical-coordinates). [Separation of variables](../../../partial-differential-equation.md#separation-of-variables) gives

$$
\frac{(RJ')'}{RJ}=-\frac{Z''}{Z}=-k^2,\qquad J''+\frac1RJ'+k^2J=0,\qquad Z''-k^2Z=0.
$$

Here $k>0$ is a radial [wavenumber](../../../wave-equation.md#wavenumber), with units of inverse length. Regularity on the axis selects the [Bessel function of the first kind](../../../analysis.md#bessel-function-of-the-first-kind) $J_0(kR)$ rather than the singular second solution. Decay away from the disk, continuity across it and reflection symmetry select $Z=e^{-k|z|}$. These conditions apply to each nonzero-wavenumber mode; a uniform sheet is a separate zero-mode problem.

Integrate the [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity) across the disk to obtain the jump condition

$$
\Phi_z(R,0^+)-\Phi_z(R,0^-)=4\pi G\Sigma(R).
$$

For the unit-amplitude separated mode, the jump is $-2kJ_0(kR)$. Thus

$$
\boxed{\Phi_k=e^{-k|z|}J_0(kR),\qquad \Sigma_k=-\frac{k}{2\pi G}J_0(kR).}
$$

An individual basis density is signed; positive physical [surface densities](../../../astrophysics.md#surface-density-of-a-disk) are built by superposition.

**An arbitrary axisymmetric surface density.** Define its order-zero [Hankel transform](../../../analysis.md#hankel-transform) by

$$
\widehat\Sigma(k)=\int_0^\infty\Sigma(R')J_0(kR')R'\,dR',\qquad \Sigma(R)=\int_0^\infty\widehat\Sigma(k)J_0(kR)k\,dk.
$$

Matching the coefficients of the mode densities gives the [Hankel representation of thin-disk gravity](../../../astrophysics.md#hankel-representation-of-thin-disk-gravity),

$$
\boxed{\Phi(R,z)=-2\pi G\int_0^\infty\widehat\Sigma(k)J_0(kR)e^{-k|z|}\,dk.}
$$

The [boundary conditions](../../../differential-equation.md#boundary-condition) exclude added external fields. For sufficiently decaying [surface density](../../../astrophysics.md#surface-density-of-a-disk), this is the isolated-disk potential; for infinite scale-free disks, only potential differences or regularized forces need be finite.

**The Mestel disk.** Put $C=\Sigma_0R_0$. The [Bessel function](../../../analysis.md#bessel-function) integral $\int_0^\infty J_0(kR')\,dR'=1/k$, understood with a decaying regulator, gives $\widehat\Sigma=C/k$. Differentiate the potential before removing the regulator and use $J_0'=-J_1$:

$$
\Phi_R(R,0)=2\pi GC\int_0^\infty J_1(kR)\,dk=\frac{2\pi GC}{R}.
$$

The last integral is $1/R$, since $\int_0^\infty J_1(u)\,du=[-J_0(u)]_0^\infty=1$. Therefore the [circular speed](../../../galaxy.md#circular-speed) and enclosed [mass](../../../classical-mechanics.md#mass) are

$$
\boxed{v_c^2=R\Phi_R=2\pi G\Sigma_0R_0=:v_0^2,\qquad M(R)=2\pi\int_0^R\Sigma(R')R'\,dR'=2\pi\Sigma_0R_0R.}
$$

Consequently $v_c^2=GM(R)/R$. This equality follows from the specific [Mestel disk](../../../astrophysics.md#mestel-disk) calculation; the spherical shell theorem cannot be applied to general disks. Its total [mass](../../../classical-mechanics.md#mass) and absolute potential referenced to infinity diverge. A convenient finite midplane reference is $\Phi(R,0)=v_0^2\log(R/R_0)$.

**The rotating distribution function.** Use specific [energy](../../../classical-mechanics.md#energy) $E=(v_R^2+v_\phi^2)/2+\Phi$ and $L_z=Rv_\phi$. For the printed positive exponential, take $\varepsilon=-E$ and $s:=\sigma>0$; $s$ has units of squared velocity. If instead $\varepsilon$ means ordinary total energy and $\sigma>0$, the velocity integral diverges, so that literal convention cannot define the requested [galactic distribution function](../../../galaxy.md#galactic-distribution-function). Equivalently one can retain ordinary energy and choose the printed $\sigma$ negative.

With the binding-energy convention, write the amplitude as $A$ to distinguish it from the function:

$$
f=A(Rv_\phi)^q\exp\!\left[-\frac{v_R^2+v_\phi^2}{2s}\right](R/R_0)^{-v_0^2/s},\qquad v_\phi>0.
$$

Integration over both radial velocities and positive azimuthal velocities gives

$$
\begin{aligned}
\Sigma(R)&=A R^q(R/R_0)^{-v_0^2/s}\sqrt{2\pi s}\,\frac{(2s)^{(q+1)/2}}{2}\Gamma\!\left(\frac{q+1}{2}\right)\\
&=A R^q(R/R_0)^{-v_0^2/s}\sqrt\pi\,2^{q/2}s^{(q+2)/2}\Gamma\!\left(\frac{q+1}{2}\right).
\end{aligned}
$$

The half-line integral follows by setting $u=v_\phi^2/(2s)$ in the defining [Gamma function](../../../complex-analysis.md#gamma-function) integral and requires $q>-1$. Matching its radial power and normalization to the [Mestel disk](../../../astrophysics.md#mestel-disk) yields the [rotating Mestel disk distribution function](../../../astrophysics.md#rotating-mestel-disk-distribution-function) parameters

$$
\boxed{q=\frac{v_0^2}{s}-1,\qquad F=A=\frac{\Sigma_0R_0^{-q}}{\sqrt\pi\,2^{q/2}s^{(q+2)/2}\Gamma((q+1)/2)}.}
$$

Since $v_0^2,s>0$, the required integrability condition is automatic. The amplitude uses the stated potential reference; changing the additive potential constant changes $A$ without changing the physical distribution.

## 2

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

**First velocity moment.** Assume a stationary, spherical, nonstreaming [collisionless stellar system](../../../galaxy.md#collisionless-stellar-system) with constant [mass-to-light ratio](../../../galaxy.md#mass-to-light-ratio) $\Upsilon$. Use a luminosity-weighted [galactic distribution function](../../../galaxy.md#galactic-distribution-function), with [luminosity density](../../../astrophysics.md#luminosity-density) $\lambda$. Multiplying the [Collisionless Boltzmann equation](../../../galaxy.md#collisionless-boltzmann-equation) by $v_i$ and integrating over velocities, with its velocity-space boundary terms vanishing, gives

$$
\partial_j\big(\lambda\langle v_i v_j\rangle\big)=-\lambda\partial_i\Phi.
$$

Spherical symmetry makes the stress tensor

$$
T_{ij}=q_t\delta_{ij}+(q-q_t)\frac{x_ix_j}{r^2},\qquad q=\lambda\sigma_r^2,\qquad q_t=\lambda\sigma_t^2.
$$

Here $\sigma_t^2$ is one tangential component, as in the paper; the total tangential [variance](../../../variance.md) is $2\sigma_t^2$. Its radial divergence is $q'+2(q-q_t)/r$, since the divergence of the radial unit vector is $2/r$. With the [velocity-anisotropy parameter](../../../galaxy.md#velocity-anisotropy-parameter) $\beta=1-\sigma_t^2/\sigma_r^2$, and enclosed [mass](../../../classical-mechanics.md#mass) $M(r)=\Upsilon L(r)$, this gives the [Spherical Jeans equation](../../../galaxy.md#spherical-jeans-equation)

$$
\boxed{q'+\frac{2\beta q}{r}=-\lambda\Phi'(r)=-\gamma\frac{\lambda L(r)}{r^2},\qquad\gamma=G\Upsilon.}
$$

This uses a constant ratio of total gravitating mass to luminosity, rather than an arbitrary independent dark halo.

**Projection and elimination of anisotropy.** Write $R$ for projected radius and $r$ for spherical radius. The [Abel transform](../../../functional-analysis.md#abel-transform) of the [luminosity density](../../../astrophysics.md#luminosity-density) gives

$$
\mu(R)=2\int_R^\infty\frac{\lambda(r)r\,dr}{\sqrt{r^2-R^2}},
$$

whose inverse is the displayed density inversion in the paper. At a point on this [line of sight](../../../astrophysics.md#line-of-sight), $\sin^2\theta=R^2/r^2$. The line-of-sight second [stellar velocity moment](../../../galaxy.md#stellar-velocity-moment) is $\sigma_r^2\cos^2\theta+\sigma_t^2\sin^2\theta=\sigma_r^2(1-\beta R^2/r^2)$. Therefore the measured quantity $J(R)=\mu(R)\sigma_p^2(R)$ satisfies

$$
J(R)=2\int_R^\infty\left(1-\beta(r)\frac{R^2}{r^2}\right)\frac{q(r)r\,dr}{\sqrt{r^2-R^2}}.
$$

The [Spherical Jeans equation](../../../galaxy.md#spherical-jeans-equation) gives $\beta q=-rq'/2-\gamma\lambda L/(2r)$. Substitution yields

$$
J(R)=2\int_R^\infty\frac{q(r)r\,dr}{\sqrt{r^2-R^2}}+R^2\int_R^\infty\frac{q'(r)\,dr}{\sqrt{r^2-R^2}}+\gamma R^2\int_R^\infty\frac{\lambda(r)L(r)\,dr}{r^2\sqrt{r^2-R^2}}.
$$

The inner $\gamma L$ printed in the PDF's definition of $p$ must therefore be $\lambda L$: the literal expression has an extra gravitational factor and lacks the density. Both this derivation and dimensional consistency require the correction. Define the [projected spherical Jeans residual](../../../galaxy.md#projected-spherical-jeans-residual) by

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

Thus the integrated residual is exactly $(2K+W)/\Upsilon$, and its vanishing is the [virial theorem](../../../classical-mechanics.md#virial-theorem). Solving for $\gamma$ gives the [global projected virial estimate of a mass-to-light ratio](../../../galaxy.md#global-projected-virial-estimate-of-a-mass-to-light-ratio),

$$
\boxed{\gamma=\frac{3\int_0^\infty R\mu(R)\sigma_p^2(R)\,dR}{2\int_0^\infty r\lambda(r)L(r)\,dr}.}
$$

It is independent of the radial anisotropy profile when the full aperture and the stated boundary conditions are used. A finite aperture retains a boundary term.

## 3

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The factor called $N$ in the formula must be the stellar [number density](../../../statistical-physics.md#number-density) $n$, not a dimensionless count. Indeed $\sigma^3/(G^2m^2)$ has dimensions time per volume, so a density in the denominator is essential. If $N_*$ is the population in a representative volume $V$, then $n=N_*/V$.

For a weak encounter between equal-mass [stars](../../../stellar-astrophysics.md#star), let $u$ be the asymptotic relative [speed](../../../classical-mechanics.md#speed) and $b$ the [impact parameter](../../../classical-mechanics.md#impact-parameter). In the straight-line impulse approximation, one star's transverse kick is

$$
\Delta v_\perp=\int_{-\infty}^{\infty}\frac{Gmb\,dt}{(b^2+u^2t^2)^{3/2}}=\frac{2Gm}{bu}.
$$

The other receives the opposite kick, so the relative-velocity change is $\Delta u_\perp=4Gm/(bu)$. Encounters in $(b,b+db)$ occur at rate $2\pi b\,db\,nu$. Independent random kicks add in squared magnitude, giving

$$
D_v:=\frac{d\langle|\Delta\mathbf v|^2\rangle}{dt}=\frac{8\pi nG^2m^2}{u}\int_{b_{\min}}^{b_{\max}}\frac{db}{b}=\frac{8\pi nG^2m^2\ln\Lambda}{u},\qquad D_u=4D_v.
$$

This is the [random-walk derivation of stellar relaxation](../../../galaxy.md#random-walk-derivation-of-stellar-relaxation). The [Coulomb logarithm in stellar dynamics](../../../galaxy.md#coulomb-logarithm-in-stellar-dynamics) is $\ln\Lambda=\ln(b_{\max}/b_{\min})$. The upper cutoff is the size or inhomogeneity scale beyond which independent local encounters are inappropriate. The lower cutoff is of order the strong-deflection scale $G(2m)/u^2$, or a larger stellar-size/softening scale if applicable. A self-gravitating system commonly has $\Lambda$ of order its total number of stars; that population count is distinct from $n$ in the diffusion rate.

To state the numerical convention explicitly, use representative encounter speed $u=\sqrt2\sigma$ and define the relaxation estimate from the relative-velocity diffusion rate with reference squared velocity $3\sigma^2$. This gives

$$
\boxed{T_R:=\frac{3\sigma^2}{D_u}=\frac{3}{16\pi\sqrt2}\frac{\sigma^3}{nG^2m^2\ln\Lambda}.}
$$

This recovers the printed coefficient under a specified convention. There is no convention-independent exact numerical prefactor determined by a representative one-dimensional velocity alone. Using the single-star diffusion rate with the same $3\sigma^2$ reference instead gives four times this time; averaging over a full velocity distribution also changes the prefactor. The [relaxation time conventions in stellar dynamics](../../../galaxy.md#relaxation-time-conventions-in-stellar-dynamics) must therefore distinguish single-star and relative kicks. **The physical scaling is $T_R\propto\sigma^3/(nG^2m^2\ln\Lambda)$, and the printed $N$ must be interpreted as number density.**

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Use $\mu=\gamma m$ for the gravitational parameter, to distinguish it from the Delaunay action called $G$. The displayed actions are per unit reduced mass. Accordingly use specific canonical momenta; with physical relative momenta, all three actions acquire a common reduced-mass factor, which leaves the eccentricity fraction below unchanged.

**The canonical transformation.** In spherical coordinates, separation of the Kepler [Hamilton-Jacobi equation](../../../classical-mechanics.md#hamilton-jacobi-equation) gives

$$
p_\phi=H,\qquad p_\theta^2=G^2-\frac{H^2}{\sin^2\theta},\qquad p_r^2=2E+\frac{2\mu}{r}-\frac{G^2}{r^2},\qquad E=-\frac{\mu^2}{2L^2}.
$$

A local type-two generating function, continued across turning points with the appropriate momentum branches, is

$$
W=H\phi+\int^\theta\sqrt{G^2-H^2/\sin^2\theta'}\,d\theta'+\int^r\sqrt{-\mu^2/L^2+2\mu/r'-G^2/r'^2}\,dr'.
$$

The old momenta are $\partial W/\partial(r,\theta,\phi)$ and the new angles are $l=\partial_LW$, $g=\partial_GW$, $h=\partial_HW$. This defines a [canonical transformation](../../../classical-mechanics.md#canonical-transformation), since its generating differential is $dW=p_rdr+p_\theta d\theta+p_\phi d\phi+l\,dL+g\,dG+h\,dH$. With standard choices of angle origins, the resulting [Delaunay variables](../../../classical-mechanics.md#delaunay-variables) are

$$
L=\sqrt{\mu a},\qquad G=L\sqrt{1-e^2},\qquad H=G\cos i,
$$

with $l$ the [mean anomaly](../../../classical-mechanics.md#mean-anomaly), $g$ the [argument of periapsis](../../../classical-mechanics.md#argument-of-periapsis), and $h$ the [longitude of ascending node](../../../classical-mechanics.md#longitude-of-ascending-node). In particular, the signed $H$ includes retrograde orbits; the squared equation in the PDF must not be read as $H\geq0$.

For bound noncollision [Kepler orbits](../../../classical-mechanics.md#kepler-orbit), the independent ranges are

$$
\boxed{0<L<\infty,\quad0<G<L,\quad-G<H<G,\quad0\leq l,g,h<2\pi.}
$$

The limiting circular, radial and coplanar cases sit on boundaries where some angle charts degenerate. They have zero measure in the generic phase-volume calculation. The ranges are constrained as above, rather than a Cartesian box with three unconstrained actions.

**The eccentricity count.** A [canonical transformation](../../../classical-mechanics.md#canonical-transformation) preserves [phase space](../../../classical-mechanics.md#phase-space) volume, so

$$
dN=F(E(L))\,dL\,dG\,dH\,dl\,dg\,dh.
$$

Integrating the three angles contributes $(2\pi)^3$, and integrating $H$ gives $2G$. At fixed $L$, the condition that the [orbital eccentricity](../../../classical-mechanics.md#orbital-eccentricity) be less than $e_0$ is $G>L\sqrt{1-e_0^2}$. Thus

$$
\int_{L\sqrt{1-e_0^2}}^L2G\,dG=L^2e_0^2,\qquad \int_0^L2G\,dG=L^2.
$$

Any energy weight cancels between these integrals. If the total population is finite, or an explicit finite action band is used,

$$
\boxed{N(e<e_0)=e_0^2N_{\rm tot},\qquad P(e<e_0)=e_0^2,\qquad f_e(e)=2e.}
$$

This is the [Delaunay phase-volume proof of the thermal eccentricity distribution](../../../classical-mechanics.md#delaunay-phase-volume-proof-of-the-thermal-eccentricity-distribution). The source's $e^2$ law is a cumulative count, not a differential eccentricity density. Also, pointwise finite $F(E)$ does not alone imply finite $N_{\rm tot}$: $F=1$ gives $\int_0^\infty L^2dL=\infty$. The [finite normalization of an energy-only Kepler distribution](../../../classical-mechanics.md#finite-normalization-of-an-energy-only-kepler-distribution) is the additional condition needed for a global probability statement; the fraction at every fixed energy is unaffected.

**Why the observation does not imply relaxation or equilibrium.** No [Boltzmann distribution](../../../thermodynamics.md#boltzmann-distribution) was used: every normalizable energy-only [phase-space distribution function](../../../statistical-physics.md#phase-space-distribution-function) has the same eccentricity marginal, irrespective of collisional thermalization. An even stronger counterexample is a genuinely time-dependent collisionless distribution

$$
f(L,G,H,l,g,h,t)=F(E(L))[1+\eta\cos(l-\nu(L)t)],\qquad0<|\eta|<1,\qquad\nu(L)=\frac{\mu^2}{L^3}.
$$

Kepler motion has $\dot l=\nu(L)$ and constant actions and other angles, so $\partial_tf+\nu\partial_lf=0$: this is an exact nonstationary solution of the [Collisionless Boltzmann equation](../../../galaxy.md#collisionless-boltzmann-equation). Integrating $l$ removes the cosine and leaves precisely the same $e^2$ cumulative count at every time. **An eccentricity marginal alone cannot establish thermal relaxation, a relaxed age, or even a stationary distribution.**

## 4

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

An [isolating integral](../../../classical-mechanics.md#isolating-integral) is a single-valued [integral of motion](../../../classical-mechanics.md#integral-of-motion) $I(\mathbf x,\mathbf v)$ whose fixed value confines an orbit to a lower-dimensional level set of [phase space](../../../classical-mechanics.md#phase-space). Along the flow, $dI/dt=0$; for an autonomous [Hamiltonian](../../../classical-mechanics.md#hamiltonian), this means $\{I,H\}=0$. Several [isolating integrals](../../../classical-mechanics.md#isolating-integral) are independent when their gradients are linearly independent on the regular region considered. Counting them requires a specified domain: merely local orbit labels in a flow box do not establish global single-valued integrals. The following cases concern regular globally meaningful orbit constraints.

<h4 id="4/i/1">1</h4>

↑ **Parent:** [I](#4/i)

<h5 id="4/i/1/solution">Solution</h5>

↑ **Parent:** [1](#4/i/1)

**One integral can occur in an autonomous system with a fully chaotic region and no additional continuous orbit constraints.** The [specific orbital energy](../../../classical-mechanics.md#specific-orbital-energy) is conserved in a time-independent [gravitational potential](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass). If a [chaotic stellar orbit](../../../galaxy.md#chaotic-stellar-orbit) is dense in a connected region of its energy hypersurface, every continuous [integral of motion](../../../classical-mechanics.md#integral-of-motion) is constant on that region. Thus it cannot supply a new independent constraint there, and energy is the only independent [isolating integral](../../../classical-mechanics.md#isolating-integral). A generic nonaxisymmetric potential can contain such regions; not every orbit in such a potential is necessarily chaotic.

<h4 id="4/i/2">2</h4>

↑ **Parent:** [I](#4/i)

<h5 id="4/i/2/solution">Solution</h5>

↑ **Parent:** [2](#4/i/2)

**No global isolating integral is possible in a sufficiently general time-dependent system without surviving symmetries or other invariants.** For

$$
E=\tfrac12v^2+\Phi(\mathbf x,t),\qquad \frac{dE}{dt}=\frac{\partial\Phi}{\partial t},
$$

even energy is then not conserved, and nonsymmetric forcing can destroy all global constraints on the orbit. Time dependence alone does not imply this result: a central time-dependent force still conserves [angular momentum](../../../classical-mechanics.md#angular-momentum), and a rigidly rotating potential can conserve a [Jacobi integral of a rigidly rotating potential](../../../classical-mechanics.md#jacobi-integral-of-a-rigidly-rotating-potential). The case of no integrals requires absence of such additional structure. A fixed point or locally defined flow labels are not the global orbit family considered here.

<h4 id="4/i/3">3</h4>

↑ **Parent:** [I](#4/i)

<h5 id="4/i/3/solution">Solution</h5>

↑ **Parent:** [3](#4/i/3)

**More than three integrals occur when additional symmetry or degeneracy restricts motion beyond a generic three-frequency invariant torus.** In a time-independent central [gravitational potential](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass), energy and the three components of [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum) are four generically independent [isolating integrals](../../../classical-mechanics.md#isolating-integral). They fix the orbital plane as well as the radial-motion parameters. A nonclosed planar rosette typically has two-dimensional orbit closure, rather than a three-dimensional [invariant torus](../../../classical-mechanics.md#invariant-torus).

The [Kepler orbit](../../../classical-mechanics.md#kepler-orbit) is a stronger example. In addition to $E$ and $\mathbf L$, the conserved [Laplace-Runge-Lenz vector](../../../classical-mechanics.md#laplace-runge-lenz-vector)

$$
\mathbf A=\mathbf v\times\mathbf L-\mu\frac{\mathbf r}{r},\qquad \mu=GM,
$$

fixes the apsidal direction. Its constraints $\mathbf A\cdot\mathbf L=0$ and $A^2=\mu^2+2EL^2$ leave five independent integrals among $E,\mathbf L,\mathbf A$. It is a maximally [superintegrable Hamiltonian system](../../../classical-mechanics.md#superintegrable-hamiltonian-system), with closed nondegenerate bound orbits.

More than three integrals need not form a set of [Poisson-commuting functions](../../../classical-mechanics.md#poisson-commuting-functions); the three-integral limit applies to an independent commuting set, rather than to every conserved orbit constraint. At a nonstationary point in six-dimensional [phase space](../../../classical-mechanics.md#phase-space), integral gradients annihilate the nonzero flow vector, so at most five are independent. This explains the [isolating integrals and orbital closure dimension](../../../classical-mechanics.md#isolating-integrals-and-orbital-closure-dimension) count. A resonance on one isolated orbit does not by itself prove an additional smooth global integral on a neighborhood.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Use $M$ for the mass parameter throughout; the PDF uses $m$ in its formulas and $M$ in the subsequent prose for the same quantity. Set $a=r_j>0$. The [Jaffe model](../../../galaxy.md#jaffe-model) density simplifies to

$$
\rho(r)=\frac{Ma}{4\pi r^2(r+a)^2}.
$$

Its enclosed [mass](../../../classical-mechanics.md#mass) is

$$
M(r)=4\pi\int_0^r\rho(s)s^2\,ds=Ma\int_0^r\frac{ds}{(s+a)^2}=\boxed{\frac{Mr}{r+a}}.
$$

It tends to $M$ as $r\to\infty$, verifying the total mass. It tends to zero at the center, so the cusp carries no extra point mass.

Spherical symmetry gives $\Phi'(r)=GM(r)/r^2=GM/[r(r+a)]$. Integrating with $\Phi(\infty)=0$ gives

$$
\Phi(r)=-GM\int_r^\infty\frac{ds}{s(s+a)}=\boxed{\frac{GM}{a}\log\frac{r}{r+a}}.
$$

This also directly satisfies the [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity): differentiating $r^2\Phi'=GMr/(r+a)$ gives $4\pi Gr^2\rho(r)$. The [circular speed](../../../galaxy.md#circular-speed) is

$$
\boxed{v_c^2(r)=r\Phi'(r)=\frac{GM}{r+a}.}
$$

For $r\ll a$, $v_c=\sqrt{GM/a}[1-r/(2a)+O((r/a)^2)]$ is approximately constant. For $r\gg a$, $v_c=\sqrt{GM/r}[1-a/(2r)+O((a/r)^2)]\propto r^{-1/2}$. Thus the finite-mass model has an inner nearly flat [galaxy rotation curve](../../../galaxy.md#galaxy-rotation-curve) and an outer Keplerian decline.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
