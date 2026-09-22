<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interpret $\dot m$ as the rest-mass supply rate through a coherent disc; the hole's gravitating mass grows more slowly because radiation carries away binding energy. Initially the hole is a [Schwarzschild black hole](../../../../../../schwarzschild-spacetime.md), whose [innermost stable circular orbit](../../../../../../innermost-stable-circular-orbit.md) is at $R_*=6GM_0/c^2$. The relativistic orbital constants there are

$$
E_{\rm ISCO}=\sqrt{\frac89},\qquad
\ell_{\rm ISCO}=2\sqrt3\frac{GM_0}{c}.
$$

They follow by extremizing the [timelike geodesic effective potential](../../../../../../timelike-geodesic-effective-potential.md) for a circular orbit and imposing marginal stability. Assume negligible torque inside the inner edge, so the gas carries this [specific angular momentum](../../../../../../specific-angular-momentum.md) into the hole. Its initial spin-up torque is

$$
\boxed{\dot J_0=\dot m\,\ell_{\rm ISCO}
=2\sqrt3\frac{GM_0\dot m}{c}
\simeq9.7\times10^{48}\,\mathrm{g\,cm^2\,s^{-2}}}
$$

for $M_0=10^8M_\odot$ and $\dot m=0.1M_\odot\,\mathrm{yr^{-1}}$. In SI units this is $9.7\times10^{41}\,\mathrm{kg\,m^2\,s^{-2}}$. A purely Newtonian estimate $\ell\sim\sqrt{GM_0R_*}$ gives a similar order of magnitude, but the relativistic value is appropriate at the [innermost stable circular orbit](../../../../../../innermost-stable-circular-orbit.md).

The maximal [Kerr black hole](../../../../../../kerr-black-hole.md) angular momentum at the initial mass is $J_{\max,0}=GM_0^2/c\simeq8.8\times10^{64}\,\mathrm{g\,cm^2\,s^{-1}}$. Holding both that mass and the initial torque fixed would give

$$
\boxed{t_{\rm spin,rough}\sim\frac{J_{\max,0}}{\dot J_0}
=\frac{M_0}{2\sqrt3\dot m}\simeq2.9\times10^8\,\mathrm{yr},
\qquad\Delta m_{\rm rest,rough}\sim2.9\times10^7M_\odot.}
$$

Initially $\dot M_{\rm BH}=E_{\rm ISCO}\dot m\simeq0.094M_\odot\,\mathrm{yr^{-1}}$, so the corresponding frozen-coefficient estimate of gravitating mass gain is about $2.7\times10^7M_\odot$. These are useful initial spin-growth scales, not a self-consistent time and mass increase for reaching extremality: the target angular momentum itself grows as $M^2$, and the inner orbit changes as the spin increases.

A consistent endpoint estimate is obtained from [black-hole spin-up by coherent accretion](../../../../../../black-hole-spin-up-by-coherent-accretion.md). Let $a_*=cJ/(GM^2)$ and $r=R_{\rm ISCO}c^2/(GM)$, where $M$ is the current mass. On the prograde [Kerr black hole](../../../../../../kerr-black-hole.md) inner-orbit branch, $1\leq r\leq6$, the orbital constants may be written

$$
a_*(r)=\frac{\sqrt r}{3}\left(4-\sqrt{3r-2}\right),
\qquad
E(r)=\sqrt{1-\frac{2}{3r}},
\qquad
\frac{c\ell(r)}{GM}=\frac{2}{3\sqrt3}\left(1+2\sqrt{3r-2}\right).
$$

Ignoring photon capture, an accreted rest mass $dm_0$ changes the hole by $dM=E\,dm_0$ and $dJ=\ell\,dm_0$. Differentiating the spin definition gives

$$
\frac{da_*}{d\log M}=\frac{c\ell}{GME}-2a_*.
$$

Substitution of the orbital constants gives $dr/d\log M=-2r$, hence

$$
M\sqrt r=M_0\sqrt6.
$$

At the formal extremal limit $r=1$, the result is

$$
\boxed{M_f=\sqrt6\,M_0\simeq2.45\times10^8M_\odot,
\qquad\Delta M_{\rm BH}=(\sqrt6-1)M_0\simeq1.45\times10^8M_\odot.}
$$

For constant rest-mass supply, use $r=6(M_0/M)^2$ to integrate the elapsed time:

$$
\Delta m_0=\int_{M_0}^{\sqrt6M_0}\frac{dM}{E(M)}
=\int_{M_0}^{\sqrt6M_0}\frac{dM}{\sqrt{1-M^2/(9M_0^2)}}
=3M_0\left[\arcsin\sqrt{\frac23}-\arcsin\frac13\right]
\simeq1.8464M_0.
$$

Thus the idealized coherent-disc endpoint is

$$
\boxed{t_{\rm extremal,ideal}=\frac{\Delta m_0}{\dot m}
\simeq1.85\times10^9\,\mathrm{yr}.}
$$

If the quoted $0.1M_\odot\,\mathrm{yr^{-1}}$ were instead the actual gravitating mass-growth rate, the corresponding endpoint time would be $\Delta M_{\rm BH}/\dot M_{\rm BH}\simeq1.45\times10^9\,\mathrm{yr}$. The two rate conventions cannot be interchanged.

The exact extremal endpoint is an idealization. Capture of disc photons exerts a counteracting torque and gives the [Thorne spin limit](../../../../../../thorne-spin-limit.md), $a_*\simeq0.998$, for the standard radiatively efficient thin-disc model. Therefore physical disc accretion approaches a large spin below unity rather than producing an exactly extremal hole. [Thorne's original spin-evolution calculation](https://articles.adsabs.harvard.edu/pdf/1974ApJ...191..507T) describes that correction. The independently integrated expressions above explain why the frozen-mass estimate is too short for the ideal endpoint.

The qualitative conclusion is robust: a hole that gains most of its mass through a persistent, coherently corotating [Shakura--Sunyaev thin disk](../../../../../../shakura-sunyaev-thin-disk.md) is expected to have substantial [black-hole spin](../../../../../../black-hole-spin.md). Very low spins require a different angular-momentum history, such as short episodes with changing orientations, counterrotating accretion, or mergers. Coherent feeding, not merely the existence of a disc during each episode, is the decisive assumption.

The [Soltan argument](../../../../../../soltan-argument.md) offers a population-level observational test. From the bolometric [luminosity function](../../../../../../luminosity-function-astronomy.md) of [active galactic nuclei](../../../../../../active-galactic-nucleus.md), infer the total energy radiated per comoving volume over cosmic history,

$$
U_{\rm AGN}=\int dt\int L\,\Phi(L,t)\,dL.
$$

Compare it with the increase $\Delta\rho_{\rm BH}$ in [supermassive black hole](../../../../../../supermassive-black-hole.md) mass density attributed to radiative accretion. For an effective [radiative efficiency of black-hole accretion](../../../../../../radiative-efficiency-of-black-hole-accretion.md) $\eta_{\rm eff}$,

$$
\Delta\rho_{\rm BH}=\frac{1-\eta_{\rm eff}}{\eta_{\rm eff}}
\frac{U_{\rm AGN}}{c^2},\qquad
\boxed{\eta_{\rm eff}=\frac{U_{\rm AGN}}
{U_{\rm AGN}+\Delta\rho_{\rm BH}c^2}.}
$$

In a zero-torque relativistic thin disc, $\eta=1-E_{\rm ISCO}$ rises from about $0.057$ at zero spin to $0.423$ in the photon-free prograde extremal limit. The measured effective efficiency therefore constrains population spin models under the thin-disc assumption. [Soltan's original population argument](https://academic.oup.com/mnras/article/200/1/115/2893514) explains how integrated quasar light constrains accumulated black-hole mass.

This is an accreted-rest-mass-weighted efficiency constraint, not a direct measurement of the arithmetic mean spin of every black hole. Obscured emission, bolometric corrections, seed masses, nonradiative growth, and disc orientation introduce uncertainty, and the efficiency-spin relation is nonlinear. These qualifications are essential when interpreting an inferred average spin for the whole population.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
