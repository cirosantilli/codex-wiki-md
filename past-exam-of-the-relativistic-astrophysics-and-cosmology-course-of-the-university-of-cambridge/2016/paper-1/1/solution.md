<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [active galactic nucleus](../../../../active-galactic-nucleus.md) is a compact, exceptionally luminous central source powered chiefly by [black-hole accretion](../../../../black-hole-accretion.md) rather than ordinary stellar fusion. Typical signatures include a broad spectral-energy distribution extending from radio to [X-rays](../../../../x-ray.md), rapid variability implying a small emitting region, strong optical or ultraviolet emission lines and, in some objects, radio [jets](../../../../jet-particle-physics.md) and lobes. Broad permitted lines indicate rapidly moving dense gas; narrower forbidden lines can arise farther out. Obscuration and viewing orientation can hide the broad-line region, and many active nuclei are radio quiet, so no one signature is required in every object.

For the [Schwarzschild circular-ring energy shift](../../../../schwarzschild-circular-ring-energy-shift.md), set $r_g=GM/c^2$ and let $E_0$ be the [photon](../../../../photon.md) energy in the orbiting gas frame. A local static observer in [Schwarzschild spacetime](../../../../schwarzschild-spacetime-split.md) measures $E_{\rm stat}$. For gas receding along the line-of-sight component of its velocity, special-relativistic frequency transformation gives

$$
E_0=\gamma E_{\rm stat}(1+\beta\sin i),\qquad
\beta=v/c,\quad\gamma=(1-\beta^2)^{-1/2}.
$$

Propagation from that static frame to a distant stationary observer contributes $E_\infty=E_{\rm stat}\sqrt{1-2r_g/r}$. Hence

$$
\boxed{1+z=\frac{E_0}{E_\infty}
=(1-2r_g/r)^{-1/2}(1-\beta^2)^{-1/2}
(1+\beta\sin i).}
$$

The factors describe [gravitational redshift](../../../../gravitational-redshift.md), transverse [time dilation](../../../../time-dilation.md) and the longitudinal [Doppler shift](../../../../doppler-effect.md). Here the emitter is on the maximally receding azimuth of a circular disc ring. A general azimuth has a smaller projected velocity, and a fully ray-traced image must use the [photon](../../../../photon.md) direction at emission rather than equating that local direction with the distant inclination. The supplied expression is the direct-projection transfer model, not a complete light-bending calculation.

The [innermost stable circular orbit](../../../../innermost-stable-circular-orbit.md) is the marginal stable timelike circular geodesic separating stable circular motion from radial instability. In [Schwarzschild spacetime](../../../../schwarzschild-spacetime-split.md),

$$
\boxed{r_{\rm ISCO}=6r_g=3r_s,\qquad r_s=2r_g.}
$$

For example, the circular-orbit [specific angular momentum](../../../../specific-angular-momentum.md) satisfies $j_c^2=GMr^2/(r-3r_g)$; its radial stability changes where $\mathrm d j_c^2/\mathrm dr=0$, at $6r_g$. This is outside both the horizon at $2r_g$ and the circular [photon](../../../../photon.md) orbit at $3r_g$.

The printed local orbital-speed relation gives $\beta^2=r_g/(r-2r_g)$. Combining the gravitational and transverse factors,

$$
(1-2r_g/r)^{-1/2}(1-\beta^2)^{-1/2}
=(1-3r_g/r)^{-1/2}.
$$

At the ISCO, $\beta=1/2$, so

$$
\boxed{1+z_{\rm ISCO}(i)=\sqrt2\left(1+\frac12\sin i\right).}
$$

The [Edge-on Schwarzschild ISCO redshift envelope](../../../../edge-on-schwarzschild-isco-redshift-envelope.md) is reached for an edge-on disc on its receding side:

$$
\boxed{1+z_{\max}=\frac3{\sqrt2},\qquad z_{\max}\simeq1.1213.}
$$

The approaching edge has $1+z=\sqrt2(1-\tfrac12\sin i)$. For a fixed inclination below $90$ degrees the maximum is smaller; the quoted number is an upper envelope, not the value for every observer. Within the stated ring model the receding factor increases inward across stable orbits, so the inner edge sets that envelope. Emission from a plunging region, occultation and returning rays are outside this ISCO-emitting model.

<a id="1/image-original-schwarzschild-circular-ring-transfer-calculation-showing-inclination-dependence-and-the-edge-on-isco-redshift-envelope"></a>
![](../../../../past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2016/paper-1-disc-redshift.png)

**[Figure 1](#1/image-original-schwarzschild-circular-ring-transfer-calculation-showing-inclination-dependence-and-the-edge-on-isco-redshift-envelope). Original Schwarzschild circular-ring transfer calculation showing inclination dependence and the edge-on ISCO redshift envelope**.

The [Kerr ISCO efficiency limits](../../../../kerr-isco-efficiency-limits.md) follow from equatorial [circular orbits](../../../../circular-orbit.md) in the [Kerr metric](../../../../kerr-metric.md). Prograde motion has a smaller ISCO than the non-spinning case, while retrograde motion has a larger one. A zero-torque thin disc radiating the orbital [binding energy](../../../../binding-energy.md) before the gas plunges has efficiency $\eta=1-E_{\rm ISCO}$, where $E_{\rm ISCO}$ is energy per unit rest-mass energy at infinity. The ideal limiting values are

$$
\begin{array}{c|c|c}
\text{orbit}&r_{\rm ISCO}/r_g&\eta\\\hline
\text{extremal retrograde}&9&1-\sqrt{25/27}\simeq0.03775\\
\text{Schwarzschild}&6&1-\sqrt{8/9}\simeq0.05719\\
\text{extremal prograde limit}&1&1-1/\sqrt3\simeq0.42265
\end{array}
$$

Thus more orbital [binding energy](../../../../binding-energy.md) is available in the prograde inner disc. The extremal values are formal geodesic limits: [photon](../../../../photon.md) capture, inner stresses, outflows and finite accretion thickness change the efficiency of real flows. An ISCO inside the ergoregion is not a claim that material or [radiation](../../../../radiation.md) escapes from inside the horizon.

For [accretion output relative to galactic binding energy](../../../../accretion-output-relative-to-galactic-binding-energy.md), distinguish accreted rest mass from the mass retained by the [black hole](../../../../black-hole-split.md). At constant radiative efficiency, building a hole from a negligible seed to $M_{\rm BH}=\alpha M$ emits

$$
E_{\rm rad}=\frac{\eta}{1-\eta}\alpha Mc^2.
$$

A non-negligible seed replaces $\alpha M$ by the actual mass increase. Let the first use of $\sigma_v$ mean the total three-dimensional rms random speed. For an approximately virialized [galaxy](../../../../galaxy-split.md) with negligible boundary term, $K=\tfrac12M\sigma_v^2$ and $W=-2K=-M\sigma_v^2$. The ratio to the magnitude of its [gravitational potential energy](../../../../gravitational-energy.md) is therefore

$$
\boxed{\frac{E_{\rm rad}}{|W|}
\simeq\frac{\eta}{1-\eta}\,\alpha\frac{c^2}{\sigma_v^2}.}
$$

If “[binding energy](../../../../binding-energy.md)” means the net energy needed to unbind the virialized system, $|K+W|=M\sigma_v^2/2$, the ratio is twice as large. The widely used order-of-magnitude estimate drops the retained-mass correction and writes $\eta\alpha(c/\sigma_v)^2$; it should not be confused with a precisely fixed structural coefficient.

For the numerical parameters given,

$$
\alpha(c/\sigma_v)^2\simeq998.6,\qquad
\frac{E_{\rm rad}}{|W|}\simeq998.6\,\frac{\eta}{1-\eta}.
$$

No efficiency is specified, so this function is the numerical result. For an explicitly chosen illustration $\eta=0.1$, it is about $111$, or $222$ relative to the net virial [binding energy](../../../../binding-energy.md). The non-spinning zero-torque efficiency gives about $60.6$ relative to $|W|$; the ideal retrograde and prograde limits give about $39.2$ and $731$, respectively. Spin affects the ratio through the adopted efficiency and orbital orientation, not through a universal rule that a larger unsigned spin always means a larger efficiency.

Such large energy ratios make even a modest coupling of the output to galactic gas dynamically important. [Radiation](../../../../radiation.md) and winds can heat or eject gas and reduce [star formation](../../../../star-formation.md) or later black-hole feeding. For the $\eta=0.1$ illustration a percent-level coupling is already comparable to $|W|$. Energy available is not energy necessarily deposited: cooling, escape directions, gas geometry, [photon](../../../../photon.md) opacity and the duration of activity determine the actual feedback. It does not follow that the entire stellar [galaxy](../../../../galaxy-split.md) must be disrupted.

For the swept-shell calculation, the problem now explicitly redefines $\sigma_v$ as a one-dimensional line-of-sight dispersion. The specified isothermal profile has

$$
M_{\rm gal}(R)=\frac{2\sigma_v^2R}{G},\quad
M_{\rm sh}=fM_{\rm gal},\quad
M_{\rm int}=(1-f)M_{\rm gal}.
$$

Neglecting central-hole gravity and the shell's [self-gravity](../../../../self-gravity.md), the inward force due to the remaining interior component is

$$
F_g=\frac{GM_{\rm int}M_{\rm sh}}{R^2}
=\frac{4f(1-f)\sigma_v^4}{G}.
$$

In a single-scattering momentum-driven model with the shell intercepting the central [luminosity](../../../../luminosity.md), $F_{\rm rad}=L/c$. At the [hydrogen](../../../../hydrogen.md) [Eddington luminosity](../../../../eddington-luminosity.md) this becomes $4\pi GM_{\rm BH}m_p/\sigma_T$. Sustained outward acceleration against that weight requires

$$
\frac{4\pi GM_{\rm BH}m_p}{\sigma_T}
>\frac{4f(1-f)\sigma_v^4}{G},
$$

and hence

$$
\boxed{M_{\rm BH}>
\frac{(1-f)f\sigma_v^4\sigma_T}{\pi m_pG^2}.}
$$

The radius cancels because the swept isothermal mass is proportional to $R$. This is the [isothermal-galaxy momentum-balance shell threshold](../../../../isothermal-galaxy-momentum-balance-shell-threshold.md), with its fourth-power dispersion scaling.

The coefficient identifies the approximations. [Self-gravity in a thin spherical shell expansion](../../../../self-gravity-in-a-thin-spherical-shell-expansion.md) adds the shell's inward pressure-equivalent force $GM_{\rm sh}^2/(2R^2)$ and replaces $f(1-f)$ by $f(1-f/2)$. A shell intercepting only a fraction of the [photon](../../../../photon.md) [momentum](../../../../momentum-split.md) needs a larger [luminosity](../../../../luminosity.md); Thomson-thin material does not automatically receive $L/c$. Conversely, [multiple scattering](../../../../multiple-scattering.md) or an energy-driven hot wind changes the force model. A shell already carrying sufficient outward [kinetic energy](../../../../kinetic-energy.md) need not satisfy this instantaneous acceleration condition everywhere to escape. The printed inequality is the stated quasistatic, fully coupled momentum-balance estimate, not an assumption-free lower bound for every possible shell trajectory.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../split.md)
5. [Relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../../relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
