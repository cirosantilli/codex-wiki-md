<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [circular orbit](../../../../../circular-orbit.md) the origin of [mean anomaly](../../../../../mean-anomaly.md) is arbitrary because there is no distinguished [pericentre](../../../../../periapsis.md). Choose $M=0$ at the [ascending node](../../../../../ascending-node.md), so $M$ is also the argument of latitude. If a different periapsis convention is used, replace $M$ below by $M+\omega$. The [orbital-frame rotation from inclination and node](../../../../../orbital-frame-rotation-from-inclination-and-node.md) gives

$$
\boldsymbol r=R_z(\Omega)R_x(I)\begin{pmatrix}a\cos M\\a\sin M\\0\end{pmatrix},
\qquad
\boxed{\begin{aligned}
x&=a(\cos\Omega\cos M-\sin\Omega\cos I\sin M),\\
y&=a(\sin\Omega\cos M+\cos\Omega\cos I\sin M),\\
z&=a\sin I\sin M.
\end{aligned}}
$$

In particular the crossing at $M=0$ has increasing $z$ for prograde $n>0$ and $0<I<\pi$, confirming the [ascending node](../../../../../ascending-node.md) convention.

Put $\epsilon=a/a_{\rm pl}$ and $c=\cos\psi=\widehat{\boldsymbol r}\cdot\widehat{\boldsymbol r}_\star$. The [binomial series](../../../../../binomial-series.md) expansion of the direct [disturbing function](../../../../../disturbing-function.md) is

$$
\frac{1}{|\boldsymbol r_\star-\boldsymbol r|}
=\frac1{a_{\rm pl}}(1-2\epsilon c+\epsilon^2)^{-1/2}
=\frac1{a_{\rm pl}}\left[1+\epsilon c+\frac{\epsilon^2}{2}(3c^2-1)+O(\epsilon^3)\right].
$$

The [indirect disturbing function](../../../../../indirect-disturbing-function.md) subtracts $GM_\star ac/a_{\rm pl}^2$, cancelling the dipole term. The constant $GM_\star/a_{\rm pl}$ has no spatial derivative and does not perturb the particle. After omitting that constant, the leading [stellar quadrupole disturbing function](../../../../../stellar-quadrupole-disturbing-function.md) is

$$
\boxed{\mathcal R_\star=\frac{GM_\star a^2}{a_{\rm pl}^3}\frac{3\cos^2\psi-1}{2}+O\!\left(\frac{GM_\star a^3}{a_{\rm pl}^4}\right).}
$$

Thus the PDF's equality is understood modulo a dynamically irrelevant additive constant and higher multipoles.

Define $\ell=M+\Omega$ and let $\ell_\star$ be the star's orbital longitude as seen from the planet. Its [orbital plane](../../../../../orbital-plane.md) has $I_{\rm pl},\Omega_{\rm pl}$. The vector from planet to star is the negative of the planet's heliocentric vector: if $\ell_{\rm pl}$ describes that latter vector, use $\ell_\star=\ell_{\rm pl}+\pi$. This sign matters in $\cos\psi$ but drops out of $\cos^2\psi$. Expanding the two rotated [unit vectors](../../../../../unit-vector.md) gives

$$
\boxed{\begin{aligned}
\cos\psi={}&\cos(\ell-\ell_\star)
-\frac{I^2}{2}\sin(\ell-\Omega)\sin(\ell_\star-\Omega)\\
&-\frac{I_{\rm pl}^2}{2}\sin(\ell_\star-\Omega_{\rm pl})\sin(\ell-\Omega_{\rm pl})\\
&+II_{\rm pl}\sin(\ell-\Omega)\sin(\ell_\star-\Omega_{\rm pl})+O((|I|+|I_{\rm pl}|)^4).
\end{aligned}}
$$

For example, the particle's horizontal correction is $-(I^2/2)\sin(\ell-\Omega)(-\sin\Omega,\cos\Omega)$, while its vertical component is $I\sin(\ell-\Omega)$; their [dot products](../../../../../dot-product.md) with the corresponding stellar components produce these terms. No cubic terms occur because simultaneous reversal of both small [orbital inclinations](../../../../../orbital-inclination.md) leaves the [dot product](../../../../../dot-product.md) unchanged.

The two [mean longitudes](../../../../../mean-longitude.md) are uniform for the circular [Kepler orbits](../../../../../kepler-orbit.md), so [orbit averaging](../../../../../orbit-averaging.md) is uniform in both $\ell$ and $\ell_\star$. Set $c_0=\cos(\ell-\ell_\star)$ and $c_2=\cos\psi-c_0$ through quadratic order. The needed averages follow by integrating sine and cosine products over $[0,2\pi]^2$:

$$
\langle c_0^2\rangle=\frac12,\qquad
\langle c_0\sin(\ell-\Omega)\sin(\ell_\star-\Omega)\rangle=\frac14,
$$



$$
\langle c_0\sin(\ell-\Omega)\sin(\ell_\star-\Omega_{\rm pl})\rangle
=\frac14\cos(\Omega_{\rm pl}-\Omega).
$$

For the last identity, expand $c_0=\cos\ell\cos\ell_\star+\sin\ell\sin\ell_\star$ and factor the two integrations, each using $\langle\sin^2\ell\rangle=\langle\cos^2\ell\rangle=1/2$. Squaring $c_0+c_2$ now yields

$$
\langle\cos^2\psi\rangle=\frac12-\frac14(I^2+I_{\rm pl}^2)+\frac12II_{\rm pl}\cos(\Omega_{\rm pl}-\Omega)+O(I^4),
$$

where the error includes all fourth-order combinations of the two [orbital inclinations](../../../../../orbital-inclination.md). Therefore

$$
\boxed{\left\langle\frac{3\cos^2\psi-1}{2}\right\rangle
=\frac14+\frac34II_{\rm pl}\cos(\Omega_{\rm pl}-\Omega)-\frac38(I^2+I_{\rm pl}^2)+O(I^4).}
$$

Multiplying this by $GM_\star a^2/a_{\rm pl}^3$ gives the requested secular [disturbing function](../../../../../disturbing-function.md). Equivalently, the exact angular factor for two circular rings is $(3\cos^2 I_m-1)/8$, where $I_m$ is their [mutual inclination](../../../../../mutual-inclination.md); its small-angle expansion gives the same result. This is the [double-averaged circular tidal potential](../../../../../double-averaged-circular-tidal-potential.md).

For aligned equatorial and planetary [orbital planes](../../../../../orbital-plane.md), set $I_{\rm pl}=0$. The secular [stellar quadrupole disturbing function](../../../../../stellar-quadrupole-disturbing-function.md) then has derivative $\partial_I\overline{\mathcal R}_\star=-3GM_\star a^2I/(4a_{\rm pl}^3)$. The supplied [Lagrange planetary equations](../../../../../lagrange-planetary-equations.md) for [nodal precession](../../../../../nodal-precession.md) gives

$$
\boxed{\dot\Omega_\star=-\frac{3GM_\star}{4na_{\rm pl}^3}.}
$$

The [planetary quadrupole coefficient](../../../../../planetary-quadrupole-coefficient.md) $J_2>0$ contributes $\partial_I\overline{\mathcal R}_{J_2}=-3GM_{\rm pl}J_2R_{\rm pl}^2I/(2a^3)$, hence

$$
\boxed{\dot\Omega_{J_2}=-\frac{3GM_{\rm pl}J_2R_{\rm pl}^2}{2na^5}
=-\frac32nJ_2\left(\frac{R_{\rm pl}}a\right)^2.}
$$

Both are retrograde [nodal precession](../../../../../nodal-precession.md) rates. Equating them cancels $n$ and gives the [Laplace radius](../../../../../laplace-radius.md)

$$
\boxed{a_L=\left[2J_2\frac{M_{\rm pl}}{M_\star}R_{\rm pl}^2a_{\rm pl}^3\right]^{1/5}.}
$$

The planetary quadrupole dominates inside $a_L$ and the stellar tide outside it. These are small-inclination rates for planet-bound [Kepler orbits](../../../../../kepler-orbit.md) in the hierarchical regime $a\ll a_{\rm pl}$. At exactly $I=0$, the node itself is undefined; the rates are the limiting precession frequencies of an infinitesimal tilt.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
