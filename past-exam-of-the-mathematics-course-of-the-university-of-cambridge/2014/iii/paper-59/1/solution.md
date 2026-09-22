<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Synchronous radius and its limits.** [Kepler's third law](../../../../../kepler-s-third-law.md) for a [circumplanetary orbit](../../../../../circumplanetary-orbit.md) gives

$$
a_s=\left(\frac{GMP^2}{4\pi^2}\right)^{1/3}.
$$

Here $G$ is the [gravitational constant](../../../../../gravitational-constant.md). A [planet-synchronous orbit](../../../../../planet-synchronous-orbit.md) repeats after one spin period. A [planet-stationary orbit](../../../../../planet-stationary-orbit.md) additionally requires a [circular orbit](../../../../../circular-orbit.md), zero [orbital inclination](../../../../../orbital-inclination.md) to the equator and prograde motion. Then an antenna fixed on the ground points continuously at the same satellite; merely matching the [orbital period](../../../../../orbital-period.md) does not give this property.

Write the planetary radius as $R_p=(3M/(4\pi\rho))^{1/3}$. Requiring the [semi-major axis](../../../../../semi-major-axis.md) to exceed $R_p$ gives $P^2>3\pi/(G\rho)$. The stellar [tidal force](../../../../../tidal-force.md) restricts the [circumplanetary orbit](../../../../../circumplanetary-orbit.md) to the [Hill sphere](../../../../../hill-sphere.md), of radius $r_H=a(M/(3M_\star))^{1/3}$. Thus

$$
\boxed{\sqrt{\frac{3\pi}{G\rho}}<P<\sqrt{\frac{4\pi^2a^3}{3GM_\star}}.}
$$

These are the surface and Hill-radius constraints in the idealized spherical, small-$M/M_\star$ model. Long-term prograde stability generally requires a radius appreciably inside the [Hill sphere](../../../../../hill-sphere.md); for nonzero [orbital eccentricity](../../../../../orbital-eccentricity.md), the surface constraint applies to the [periapsis](../../../../../periapsis.md), not just to the [semi-major axis](../../../../../semi-major-axis.md).

**Collision time and the launch population.** A phase-mixed isotropic swarm occupies a shell of radial scale $ea_s$. Its [number density](../../../../../number-density.md) scales as $N_s/(ea_s^3)$, its relative [speed](../../../../../speed.md) as $a_s/P$, and its [geometric collision cross-section](../../../../../geometric-collision-cross-section.md) as $r^2$. Consequently the total [collision](../../../../../collision.md) rate scales as $N_s^2r^2/(Pea_s^2)$. To give the numerical normalization used here, adopt an effective shell volume $V=4\pi ea_s^3$. At a fixed position the [velocity](../../../../../velocity.md) directions are uniformly distributed in the tangent plane, so their mean relative [speed](../../../../../speed.md) is $4v_K/\pi=8a_s/P$. For an unordered pair, the [collision cross-section](../../../../../collision-cross-section.md) is $4\pi r^2$, giving

$$
K_{ss}=\frac{4\pi r^2(8a_s/P)}{4\pi ea_s^3}=\frac8{Pe}\left(\frac r{a_s}\right)^2,\qquad
\Gamma_{ss}=\frac12 K_{ss}N_s(N_s-1)\simeq\frac{N_s^2}{A},\qquad
\boxed{A=\frac{Pe}{4}\left(\frac{a_s}{r}\right)^2.}
$$

Thus the mean interval between [collisions](../../../../../collision.md) is $A/N_s^2$ in this large-population kinetic model. The effective shell width fixes an order-one coefficient: small [orbital eccentricity](../../../../../orbital-eccentricity.md) and random planes alone do not specify a unique radial [probability density](../../../../../probability-density.md). Phase mixing, negligible [gravitational focusing](../../../../../gravitational-focusing.md), $r\ll ea_s$, and uncorrelated encounters are implicit in this estimate. Exactly identical [orbital periods](../../../../../orbital-period.md) with perfectly fixed phases do not themselves produce a memoryless [collision](../../../../../collision.md) process.

For nearly [planet-stationary orbits](../../../../../planet-stationary-orbit.md) with $e\ll I\ll1$, the swarm volume is smaller by a factor of order $I$, while the relative [speed](../../../../../speed.md) is smaller by the same factor, since vertical motion of scale $Iv_K$ dominates the eccentric motion. The two changes cancel in the rate $n\sigma v$: **there is no parametric factor $I$ in the collision time** within the same phase-mixed kinetic approximation. Numerical factors and phase correlations can differ. This is not an argument that bringing all satellites into one nearly circular plane makes their phases random.

With $N_s=Rt$, an [Inhomogeneous Poisson process](../../../../../inhomogeneous-poisson-process.md) has [cumulative hazard function](../../../../../cumulative-hazard-function.md)

$$
H(t)=\int_0^t\frac{R^2u^2}{A}\,du=\frac{R^2t^3}{3A}=\frac{N_s^3}{3AR}.
$$

The [survival function](../../../../../survival-function.md) of the first [collision](../../../../../collision.md) is $\exp[-H(t)]$. Setting the expected number of [collisions](../../../../../collision.md) to one gives

$$
\boxed{N_{s0}=(3AR)^{1/3}.}
$$

This is a characteristic first-event population, with probability $1-e^{-1}$ of an earlier event. It is not a median: the median has an additional factor $(\log2)^{1/3}$.

**Which population collides next?** Immediately after the first disruption let $S=N_{s0}-2$ and $F=2x^{-3}$. The latter follows from [mass conservation](../../../../../mass-conservation.md) for equal-density spherical pieces. Using the same unordered-pair counting and [geometric collision cross-sections](../../../../../geometric-collision-cross-section.md) as above, define $b=(1+x)^2/2$; then

$$
\Gamma_{ss}=\frac{S^2}{A},\qquad
\Gamma_{sf}=\frac{bSF}{A},\qquad
\Gamma_{ff}=\frac{x^2F^2}{A}.
$$

Here $S^2,F^2$ stand for the usual large-population approximations to $S(S-1),F(F-1)$. The factor two distinguishing identical and different species is essential. The probability that the next [collision](../../../../../collision.md) is fragment–fragment is

$$
\boxed{p_{ff}=\frac{4x^{-4}}{4x^{-4}+(1+x)^2Sx^{-3}+S^2}.}
$$

It is the most likely type if $S<4/[x(1+x)^2]$ and $S<2/x^2$. It has probability greater than one half if

$$
4>(1+x)^2Sx+x^4S^2.
$$

For $x\ll1$, a strongly fragment-dominated next event therefore requires $Sx\ll4$; the fragment–satellite comparison is more restrictive than the satellite–satellite comparison. If $S=0$, the next event must be fragment–fragment, provided fragments remain.

**Population equations and the normalization discrepancy.** Every satellite–satellite event produces $2x^{-3}$ fragments and destroys two satellites. Every satellite–fragment event produces a net $x^{-3}-1$ fragments and destroys one satellite; every fragment–fragment event destroys two fragments. Consistent [collision](../../../../../collision.md) counting therefore gives

$$
\boxed{\begin{aligned}
A\dot N_f&=2x^{-3}N_s^2+b(x^{-3}-1)N_fN_s-2x^2N_f^2,\\
A\dot N_s&=-2N_s^2-bN_fN_s.
\end{aligned}}
$$

For $x\ll1$, $b\simeq1/2$ and $x^{-3}-1\simeq x^{-3}$. The last two terms in $A\dot N_f$ are then twice those in the printed equation. This is a genuine factor-of-two inconsistency: equal-size fragment pairs have a [collision cross-section](../../../../../collision-cross-section.md) smaller by $x^2$, so their event rate must be $x^2N_f^2/A$ if the satellite event rate is $N_s^2/A$; destroying both fragments necessarily gives the sink $-2x^2N_f^2/A$.

If the printed equation is taken as a prescribed approximate rate model instead, its implicit event rates are $N_s^2/A$, $N_fN_s/(4A)$ and $x^2N_f^2/(2A)$. Under precisely that mixed normalization, its corresponding satellite equation is

$$
\boxed{\dot N_s=-A^{-1}\left(2N_s^2+\frac14N_fN_s\right).}
$$

The printed source term also neglects the consumed fragment in a satellite–fragment event, a legitimate relative $O(x^3)$ approximation. That approximation does not repair the pair-counting discrepancy.

**The ensuing cascade.** This is a [two-size fragmentation cascade](../../../../../two-size-fragmentation-cascade.md). First use the printed approximate model, dropping satellite–satellite events as requested. Put $S=N_s$, $F=N_f$, $k=4x^2$ and take $x<1/2$. Then

$$
\dot S=-\frac{FS}{4A},\qquad
\dot F=\frac{F}{A}\left(\frac{S}{4x^3}-x^2F\right),\qquad
\frac{dF}{dS}-\frac{kF}{S}=-x^{-3}.
$$

Integrating this [linear differential equation](../../../../../linear-differential-equation.md), with $F_0=2x^{-3}$ and $S_0=N_{s0}-2>0$, gives

$$
\boxed{F(S)=C S^k-\frac{x^{-3}S}{1-k},\qquad
C=\frac{F_0+x^{-3}S_0/(1-k)}{S_0^k}.}
$$

Initially the [collisional cascade](../../../../../collisional-cascade.md) grows if $S_0>8x^2$, with approximate early exponential growth time $4Ax^3/S_0$ when the satellite population is nearly fixed. The fragment population reaches its maximum at

$$
F_* =\frac{S_*}{4x^5},\qquad
S_*^{1-k}=4x^5(1-k)C.
$$

Afterwards satellites are depleted and fragment–fragment losses dominate. For $S_0>0$ the continuum solution has $S\to0$, $F\to0$, with

$$
\boxed{F(t)\sim\frac{A}{x^2t},\qquad S(t)\propto t^{-1/(4x^2)}.}
$$

When no satellites remain initially, $F(t)=F_0/[1+x^2F_0t/A]$ directly. Small integer populations eventually invalidate these deterministic [differential equations](../../../../../differential-equation-split.md).

The consistently counted model has, to leading order in $x$, exactly the same curve $F(S)$ and peak, but both retained time derivatives are twice as large. Its growth time is $2Ax^3/S_0$, and $F(t)\sim A/(2x^2t)$. Keeping $(1+x)^2$ and the consumed fragment replaces $k$ by $4x^2/(1+x)^2$ and $x^{-3}$ in the curve by $x^{-3}-1$. This explicitly separates the physical [collision](../../../../../collision.md) bookkeeping from the printed normalization while giving the evolution under both conventions.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
