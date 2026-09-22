<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Work in the rest frame of the hole and neglect stellar velocities compared with $v$. In addition to $v\gg\sigma_*$, assume the galactic encounter speed is nonrelativistic, $v\ll c$. Treat a star as a test particle with specific [angular momentum](../../../../../../angular-momentum.md) $\ell=bv$. At its pericentre $r_{\min}$, its radial velocity vanishes. [Conservation of energy](../../../../../../conservation-of-energy.md) and [conservation of angular momentum](../../../../../../conservation-of-angular-momentum.md) give

$$
\frac{v^2}{2}=\frac{\ell^2}{2r_{\min}^2}-\frac{GM_{\rm BH}}{r_{\min}},
\qquad
b^2=r_{\min}^2+\frac{2GM_{\rm BH}r_{\min}}{v^2}.
$$

The second term is [gravitational focusing](../../../../../../gravitational-focusing.md). For the rough Newtonian estimate in the question, assume capture when the pericentre reaches the [Schwarzschild radius](../../../../../../schwarzschild-radius.md), $r_S=2GM_{\rm BH}/c^2$. It follows that

$$
b_{\rm cap}^2=r_S^2\left(1+\frac{c^2}{v^2}\right),
\qquad
\boxed{b_{\rm cap}\simeq\frac{2GM_{\rm BH}}{cv}.}
$$

The approximation keeps the focusing term because $v\ll c$.

Let $\rho_*=mn_*$ be the stellar mass density. Multiplying the [geometric collision cross-section](../../../../../../geometric-collision-cross-section.md) by the incoming mass flux gives the [collisionless black-hole capture](../../../../../../collisionless-black-hole-capture.md) rate

$$
\dot M_*\simeq\pi b_{\rm cap}^2\rho_*v
=\frac{4\pi G^2M_{\rm BH}^2\rho_*}{c^2v}.
$$

For a supersonic gas with negligible [sound speed](../../../../../../speed-of-sound.md), [Bondi--Hoyle--Lyttleton accretion](../../../../../../bondi-hoyle-accretion.md) has capture radius $r_a=2GM_{\rm BH}/v^2$ and rate

$$
\dot M_{\rm BHL}\simeq\pi r_a^2\rho_gv
=\frac{4\pi G^2M_{\rm BH}^2\rho_g}{v^3}.
$$

Consequently

$$
\boxed{\frac{\dot M_*}{\dot M_{\rm BHL}}
\simeq\frac{\rho_*}{\rho_g}\left(\frac vc\right)^2.}
$$

For comparable densities and $v=200\,\mathrm{km\,s^{-1}}$, the suppression is approximately $4\times10^{-7}$. Gas can collide, dissipate orbital energy, and be captured from a region of size $GM/v^2$; collisionless particles generally leave on an unbound orbit unless their [angular momentum](../../../../../../angular-momentum.md) is small enough for direct capture. [Chandrasekhar dynamical friction](../../../../../../chandrasekhar-dynamical-friction.md) can slow the hole by transferring energy to a stellar wake, but does not mean that the stars producing that wake are swallowed.

There is an important accuracy limitation in the requested numerical coefficient. Newtonian orbital mechanics evaluated at a relativistic [event horizon](../../../../../../event-horizon.md) cannot give the exact capture boundary. In [Schwarzschild spacetime](../../../../../../schwarzschild-spacetime.md), a slowly incoming massive particle has dimensionless energy $\mathcal E\simeq1$ and [timelike geodesic effective potential](../../../../../../timelike-geodesic-effective-potential.md)

$$
V(r)=\left(1-\frac{2r_g}{r}\right)
\left(1+\frac{\ell^2}{c^2r^2}\right),\qquad r_g=\frac{GM_{\rm BH}}{c^2}.
$$

The double turning point satisfying $V=1$ and $dV/dr=0$ occurs at $r=4r_g$ and $\ell=4GM_{\rm BH}/c$. The exact low-speed boundary is therefore $b_{\rm cap}\simeq4GM_{\rm BH}/(cv)$, twice the rough value; it makes the rate ratio $4(\rho_*/\rho_g)(v/c)^2$. The key suppression scaling is unchanged.

Direct capture of ordinary stars or [dark matter](../../../../../../dark-matter.md) is therefore an inefficient route to rapid growth of a [supermassive black hole](../../../../../../supermassive-black-hole.md) under these conditions. [Tidal disruption events](../../../../../../tidal-disruption-event.md) can capture stellar debris without swallowing an intact point-like star, and special dense environments can modify the supply. These qualifications do not make collisionless capture equivalent to dissipative gas accretion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
