<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $x$ eastward, $y$ northward and $z$ upward, and let $u$ be the eastward [geostrophic wind](../../../../geostrophic-wind.md). With [Coriolis parameter](../../../../coriolis-parameter.md) $f$ independent of $z$, [geostrophic balance](../../../../geostrophic-balance.md), [hydrostatic balance](../../../../hydrostatic-balance.md), and the [ideal gas law](../../../../ideal-gas-law.md) give

$$
fu=-\frac{p_y}{\rho},\qquad p_z=-\rho g,\qquad p=\rho R_dT.
$$

Here $R_d$ is the specific gas constant for dry air. Taking a vertical [derivative](../../../../derivative.md) of the first equation and interchanging mixed [partial derivatives](../../../../partial-derivative.md) gives

$$
f u_z=g\frac{\rho_y}{\rho}-fu\frac{\rho_z}{\rho}.
$$

It matters that $\rho$ is not constant in the [pressure gradient force](../../../../pressure-gradient-force.md). Substituting

$$
\frac{\rho_y}{\rho}=-\frac{fu}{R_dT}-\frac{T_y}{T},\qquad
\frac{\rho_z}{\rho}=-\frac g{R_dT}-\frac{T_z}{T}
$$

cancels the two terms proportional to $gfu/(R_dT)$ and yields the height-coordinate [thermal wind](../../../../thermal-wind.md) relation

$$
f u_z=-\frac gT T_y+\frac{fu}{T}T_z.
$$

If $|uT_z|\ll|Tu_z|$, this reduces to

$$
\boxed{f\frac{\partial u}{\partial z}\simeq-\frac gT\frac{\partial T}{\partial y}.}
$$

The discarded term has relative scale $H|T_z|/T$ when $u_z\sim u/H$. Taking $H=10\ \mathrm{km}$, $T=250\ \mathrm K$ and a [atmospheric lapse rate](../../../../lapse-rate-atmosphere.md) of $6.5\ \mathrm{K\,km^{-1}}$ gives about $0.26$. Thus this height-coordinate formula is a useful estimate, with potentially tens-of-percent compressibility-related correction through the vertical [temperature gradient](../../../../temperature-gradient.md); it is not an exact consequence of the two balances. If the [temperature gradient](../../../../temperature-gradient.md) vanishes vertically, the displayed approximation is exact within those balances.

The [hydrostatic approximation](../../../../hydrostatic-approximation.md) is very good on the broad, shallow atmospheric scales considered. The [geostrophic balance](../../../../geostrophic-balance.md) is normally justified by a small [Rossby number](../../../../rossby-number.md) and fails as a general approximation near the equator. At $30^\circ\mathrm N$, $f=7.292\times10^{-5}\ \mathrm{s^{-1}}$. With the ideal $134\ \mathrm{m\,s^{-1}}$ wind and a $1000$--$2000\ \mathrm{km}$ horizontal scale, $\mathrm{Ro}=U/(fL)\simeq0.9$--$1.8$: quantitative accuracy is limited for this especially strong ideal jet. Small vertical aspect ratio alone does not ensure [geostrophic balance](../../../../geostrophic-balance.md), although a straight, steady zonal flow can satisfy it even when this scale estimate of the [Rossby number](../../../../rossby-number.md) is not small.

For the requested estimate, suppose the upper [jet stream](../../../../jet-stream.md) is $H=10\ \mathrm{km}$ above a weak surface wind, has [temperature](../../../../temperature-split.md) $T\simeq250\ \mathrm K$, and spans a meridional width $L$. Integrating the approximate [thermal wind](../../../../thermal-wind.md) relation in scale form gives

$$
\boxed{T_{\rm south}-T_{\rm north}\simeq\frac{fTUL}{gH}
\simeq25\ \mathrm K\left(\frac{L}{1000\ \mathrm{km}}\right)
\left(\frac{10\ \mathrm{km}}H\right)
\left(\frac{T}{250\ \mathrm K}\right).}
$$

The northward [temperature gradient](../../../../temperature-gradient.md) is negative because the eastward wind strengthens upward. A $1000$--$2000\ \mathrm{km}$ jet width gives roughly $25$--$50\ \mathrm K$. No unique numerical difference follows without specifying the jet width, height and representative [temperature](../../../../temperature-split.md); these are explicitly estimated quantities.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the geophysical fluid dynamics course of the University of Oxford](../../../split.md)
5. [Geophysical fluid dynamics course of the University of Oxford](../../../../geophysical-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
