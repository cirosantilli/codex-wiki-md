<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [passive disk](../../../../../passive-disk.md) is heated predominantly by intercepted stellar radiation, rather than by its own [viscous dissipation](../../../../../viscous-dissipation.md). A rough luminosity criterion, ignoring geometric factors, is

$$
\boxed{L_{\rm acc}\sim\frac{GM\dot M}{R_*}\ll L_*.}
$$

The intrinsic [accretion disk](../../../../../accretion-disk.md) luminosity is of order $GM\dot M/(2R_*)$, with additional accretion energy potentially released at the stellar surface. The local test is more precise: absorbed irradiation must dominate the viscous flux at the radius being considered. For an ordinary steady [Keplerian accretion disk](../../../../../keplerian-accretion-disk.md), sufficiently far outside its inner edge,

$$
F_{\rm vis}\simeq\frac{3GM\dot M}{8\pi R^3},\qquad
F_{\rm irr}\simeq\frac{L_*\alpha}{4\pi R^2},\qquad
\frac{F_{\rm vis}}{F_{\rm irr}}\simeq\frac{3GM\dot M}{2L_*R\alpha}\ll1,
$$

where $\alpha$ is the [irradiation grazing angle of a disk](../../../../../irradiation-grazing-angle-of-a-disk.md). Reflection, very small incidence angles and shadowing can invalidate a simple total-luminosity comparison. The following calculation assumes an illuminated, absorbing surface.

At a point $(R,z_s)$ on the upper surface, the outward unit normal in the meridional plane is proportional to $(-z_s',1)$, and a light ray from the point source is directed along $(R,z_s)$. Its flux through the upper face is the incident inverse-square flux times minus their scalar product:

$$
F_d=\frac{L_*}{4\pi(R^2+z_s^2)}\frac{Rz_s'-z_s}{\sqrt{R^2+z_s^2}\sqrt{1+(z_s')^2}}.
$$

For a [thin disk](../../../../../thin-disk.md) with small surface slope this becomes

$$
\boxed{F_d\simeq\frac{L_*}{4\pi R^2}\left(z_s'-\frac{z_s}{R}\right)
=\frac{L_*}{4\pi R}\frac{d}{dR}\left(\frac{z_s}{R}\right).}
$$

The tangent slope and ray slope differ by $\alpha\simeq z_s'-z_s/R$. Positive incidence requires [disk flaring](../../../../../disk-flaring.md), $d(z_s/R)/dR>0$, and an unobstructed ray from the star. A negative value of the formula would mean that direct illumination of this face is absent, not that it receives a negative heating flux. The hierarchy $z_s\gg R_*$ makes the finite angular size of the star negligible here.

Let $a=\mathcal R/\mu$, so the [ideal gas](../../../../../ideal-gas.md) [equation of state](../../../../../equation-of-state.md) gives the [isothermal sound speed](../../../../../isothermal-sound-speed.md) $c_s^2=aT_c$. In the stellar vertical [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md), [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) has vertical acceleration $-\Omega_K^2z$, where $\Omega_K^2=GM/R^3$. Integration of $c_s^2\partial_z\rho=-\rho\Omega_K^2z$ gives a Gaussian atmosphere with [disk scale height](../../../../../disk-scale-height.md)

$$
H^2=\frac{aT_cR^3}{GM}.
$$

Consequently $q=z_s/R=fH/R$ satisfies $T_c=GMq^2/(af^2R)$. Substitute this into the stipulated [Stefan–Boltzmann law](../../../../../stefan-boltzmann-law.md) $F_d=\sigma T_c^4$ and the irradiation flux:

$$
\boxed{\frac{dq}{dR}=C\frac{q^8}{R^3},\qquad
C=\frac{4\pi\sigma}{L_*f^8}\left(\frac{GM}{a}\right)^4.}
$$

Here $f$ specifies surface height in units of [disk scale height](../../../../../disk-scale-height.md) and is unrelated to the wind-energy fraction in the preceding solution. This [separable differential equation](../../../../../separable-differential-equation.md) integrates exactly to

$$
q^{-7}=\frac{7C}{2R^2}+B=\frac{R_0^2}{R^2}+B,\qquad
\boxed{R_0^2=\frac{14\pi\sigma}{L_*f^8}\left(\frac{GM}{\mathcal R/\mu}\right)^4.}
$$

If the thin-disc solution is formally matched to $q(R_M)=1$, then $B=1-R_0^2/R_M^2$, giving

$$
q(R)=\left[1+R_0^2\left(\frac1{R^2}-\frac1{R_M^2}\right)\right]^{-1/7}
=\left(\frac R{R_0}\right)^{2/7}\left[1+\frac{R^2}{R_0^2}-\frac{R^2}{R_M^2}\right]^{-1/7}.
$$

It follows that the [flaring passive disk](../../../../../flaring-passive-disk.md) asymptotic is

$$
\boxed{\frac{z_s}{R}\simeq\left(\frac R{R_0}\right)^{2/7},\qquad H\propto R^{9/7},\qquad T_c\propto R^{-3/7}.}
$$

This applies in the thin intermediate region $R\ll\min(R_0,R_M)$, in addition to the point-source and stellar-gravity assumptions. The corrections are of relative order $R^2/R_0^2+R^2/R_M^2$. In particular, the printed hierarchy $R\ll R_M$ must still be accompanied by the initial thin-disc condition $q\ll1$: if $R_M\gg R_0$, radii larger than $R_0$ cannot satisfy that approximation. The matching at $q=1$ is an extrapolation used to set an integration constant; the derivation is not a valid treatment of a thick surface at $R_M$ itself.

Identify the stellar surface [temperature](../../../../../temperature.md) with its effective radiating [temperature](../../../../../temperature.md), so that [luminosity of a spherical blackbody](../../../../../luminosity-of-a-spherical-blackbody.md) gives $L_*=4\pi R_*^2\sigma T_*^4$. The given stellar surface scale height has $H_*^2=aT_*R_*^3/(GM)$, hence $GM/(aT_*R_*)=(R_*/H_*)^2$. Substituting into $R_0$ yields

$$
\boxed{\frac{R_0}{R_*}=\sqrt{\frac72}\left(\frac{R_*}{fH_*}\right)^4\gg1.}
$$

Thus a small stellar surface scale height leaves a wide interval above $R_*$ and below $R_0$ in which the [thin disk](../../../../../thin-disk.md) flaring law can apply. The point-source approximation imposes the stronger lower cutoff obtained from $z_s\gg R_*$:

$$
R\gg R_*^{7/9}R_0^{2/9}.
$$

This cutoff is still much smaller than $R_0$ when $R_0\gg R_*$. The full interval is therefore $R_*^{7/9}R_0^{2/9}\ll R\ll\min(R_0,R_M)$, whenever these bounds overlap. An assumed thickening radius must lie above the lower cutoff for all of the original approximations to hold simultaneously. The stellar luminosity-[temperature](../../../../../temperature.md) relation is essential to the final comparison; independent arbitrary values of $L_*$ and $T_*$ would not imply it.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
