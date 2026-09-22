<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Ignoring [gravitational focusing](../../../../../gravitational-focusing.md), a [galaxy](../../../../../galaxy-split.md) sweeps a cylinder of volume $\pi R^2v_{\rm rel}T$. Multiplying this by the number density $N$ of target [galaxies](../../../../../galaxy-split.md) and averaging the relative speed gives the mean encounter count

$$
\boxed{\mu=\pi R^2\langle v_{\rm rel}\rangle NT.}
$$

For independent encounters modeled by a [Poisson process](../../../../../poisson-process.md), the probability of at least one [galaxy merger](../../../../../galaxy-merger.md) is $1-e^{-\mu}$. The printed expression $P=\mu$ is its rare-encounter approximation $\mu\ll1$; it is not an exact probability for arbitrary $T$.

For an illustrative present-day field population take an effective merger [impact parameter](../../../../../impact-parameter.md) $R=20\,\mathrm{kpc}=0.02\,\mathrm{Mpc}$, $N=10^{-2}\,\mathrm{Mpc}^{-3}$, and $\langle v_{\rm rel}\rangle=200\,\mathrm{km\,s^{-1}}$. These are assumed order-of-magnitude inputs, not precise observational measurements. Taking a [Hubble time](../../../../../hubble-time.md) of $T\simeq1.4\times10^{10}\,\mathrm{yr}\simeq4.4\times10^{17}\,\mathrm s$, the given distance conversion yields

$$
\langle v_{\rm rel}\rangle T\simeq
\frac{200(4.4\times10^{17})}{3\times10^{19}}\,\mathrm{Mpc}
\simeq2.9\,\mathrm{Mpc},
$$

and hence

$$
\boxed{P\simeq\mu\simeq\pi(0.02)^2(10^{-2})(2.9)
\simeq3.7\times10^{-5}.}
$$

Thus the geometric field estimate is of order $10^{-5}$ to $10^{-4}$ per [Hubble time](../../../../../hubble-time.md). It scales as $R^2N\langle v_{\rm rel}\rangle T$ and is very sensitive to environment and the adopted effective merger radius. Enhanced density in groups, [gravitational focusing](../../../../../gravitational-focusing.md), and the evolution of the galaxy population are all omitted; this number is not a prediction of the full cosmological merger fraction.

Now use the stipulated rapid, distant encounter. The consistent rectilinear trajectory is

$$
\mathbf R(t)=\mathbf r_p(t)=(p,0,vt),\qquad
R(t)=\sqrt{p^2+v^2t^2}.
$$

With the stated [impact parameter](../../../../../impact-parameter.md) along $x$ and velocity along $z$, this trajectory lies in the $xz$-plane. The original PDF's reference to the $xy$-plane is a typo; the local TeX also corrupts the impact-parameter direction. The original PDF fixes that direction as $x$.

Use the positive potential $Gm_p/|\mathbf R-\mathbf r|$, whose gradient is the attractive acceleration under the question's sign convention. Its [multipole expansion](../../../../../electric-multipole-expansion.md) is

$$
\frac1{|\mathbf R-\mathbf r|}
=\frac1R+\frac{\mathbf r\cdot\mathbf R}{R^3}
+\frac{3(\mathbf r\cdot\mathbf R)^2-R^2r^2}{2R^5}
+O\!\left(\frac{r^3}{R^4}\right).
$$

The first term has no force; the linear term accelerates the entire galaxy and disappears in the frame following its [centre of mass](../../../../../center-of-mass.md). The leading internal tidal potential is therefore

$$
\boxed{\psi(\mathbf r,t)=\frac{Gm_p}{R^3}
\left[-\frac{r^2}{2}+\frac{3(\mathbf r\cdot\mathbf R)^2}{2R^2}\right].}
$$

This is a [quadrupole approximation](../../../../../quadrupole-approximation.md) valid for $r\ll p$, rather than an exact equality for every $r<p$. Its acceleration [tidal tensor](../../../../../tidal-tensor.md) acts on $\mathbf r$ as

$$
\nabla\psi=Gm_p\left[-\frac{\mathbf r}{R^3}
+\frac{3(\mathbf r\cdot\mathbf R)\mathbf R}{R^5}\right].
$$

In the [impulse approximation](../../../../../impulse-approximation.md), each stellar position is held fixed during the flyby and the velocity kick is the integral of this acceleration. Put $s=vt$; terms odd in $s$ integrate to zero, while

$$
\int_{-\infty}^{\infty}\frac{ds}{(p^2+s^2)^{3/2}}=\frac2{p^2},
\qquad
\int_{-\infty}^{\infty}\frac{ds}{(p^2+s^2)^{5/2}}=\frac4{3p^4},
\qquad
\int_{-\infty}^{\infty}\frac{s^2\,ds}{(p^2+s^2)^{5/2}}=\frac2{3p^2}.
$$

The integrated diagonal coefficients of the [tidal tensor](../../../../../tidal-tensor.md) are consequently $(2,-2,0)/(vp^2)$, giving

$$
\boxed{\Delta\mathbf v=\frac{2Gm_p}{vp^2}(x,-y,0).}
$$

The encounter stretches the galaxy along the [impact parameter](../../../../../impact-parameter.md), compresses it along $y$, and gives no net leading kick along the flyby direction.

Denote the pre-encounter stellar velocity by $\mathbf u$, to distinguish it from the relative flyby speed $v$. The instantaneous change of specific [kinetic energy](../../../../../kinetic-energy.md) is

$$
\Delta e=\mathbf u\cdot\Delta\mathbf v+\frac12|\Delta\mathbf v|^2.
$$

Uncorrelated kicks with zero mean cross term imply $\langle\mathbf u\cdot\Delta\mathbf v\rangle=0$, so the phase-averaged heating at a specified position is

$$
\boxed{\langle\Delta e\rangle=\frac{2G^2m_p^2}{v^2p^4}(x^2+y^2).}
$$

For an individual star the cross term need not vanish: the formula is an ensemble or orbital-phase average. Integrating over a spherical [galaxy](../../../../../galaxy-split.md) of mass $m_g$, symmetry gives $\langle x^2\rangle=\langle y^2\rangle=\langle z^2\rangle=\langle r^2\rangle/3$. Therefore the total [tidal heating](../../../../../tidal-heating.md) is

$$
\boxed{\Delta E_g=\frac{4G^2m_p^2m_g}{3v^2p^4}\langle r^2\rangle.}
$$

For two identical galaxies, each receives this heating with $m_p=m_g$. Adding both contributions gives

$$
\boxed{\Delta E_{\rm int}=\frac{8G^2m_g^3}{3v^2p^4}\langle r^2\rangle.}
$$

In the [centre of mass](../../../../../center-of-mass.md) frame, equal masses approach with speeds $v/2$ if $v$ is their relative speed at infinity. The initial orbital energy is

$$
E_{\rm orb}=2\left[\frac12m_g\left(\frac v2\right)^2\right]
=\frac12\left(\frac{m_g}{2}\right)v^2
=\boxed{\frac14m_gv^2},
$$

where $m_g/2$ is the [reduced mass](../../../../../reduced-mass.md). The orbital [potential energy](../../../../../potential-energy.md) vanishes at infinite separation. Within the weak-deflection approximation this asymptotic speed is also the nearly constant speed used in the flyby calculation.

[Conservation of energy](../../../../../conservation-of-energy.md) transfers the positive internal heating out of the relative orbit. [Tidal capture of galaxies](../../../../../tidal-capture-of-galaxies.md) occurs in this model if $E_{\rm orb}-\Delta E_{\rm int}<0$, which gives

$$
\frac{8G^2m_g^3\langle r^2\rangle}{3v^2p^4}>\frac14m_gv^2,
\qquad
\boxed{pv<\left[\frac{32}{3}G^2m_g^2\langle r^2\rangle\right]^{1/4}.}
$$

The equality is marginal capture. A bound pair still needs subsequent evolution to coalesce, so the result is an approximate capture criterion used here as a merger criterion. Its right-hand side has dimensions of length times speed, as required.

The [impulse approximation](../../../../../impulse-approximation.md) requires the flyby duration $\tau\sim p/v$ to be short compared with the stellar dynamical time $\Omega^{-1}$, namely $v/p\gg\Omega$. If $v/p<\Omega$, a star moves substantially during the encounter. Its orbital [adiabatic invariance of an orbital action](../../../../../adiabatic-invariance-of-an-orbital-action.md) suppresses net heating by a slowly varying tidal field: [adiabatic shielding of tidal encounters](../../../../../adiabatic-shielding-of-tidal-encounters.md) replaces the frozen-position calculation. The divergent $v^{-2}$ heating predicted by extrapolating the impulsive formula to slow encounters is therefore spurious. Close passages with $p$ comparable to the galaxy size or strong [gravitational focusing](../../../../../gravitational-focusing.md) also lie outside the derivation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
