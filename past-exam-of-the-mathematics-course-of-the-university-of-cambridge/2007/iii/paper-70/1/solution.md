<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For an equatorial [circular orbit](../../../../../circular-orbit.md) in the [Paczyński-Wiita potential](../../../../../paczynski-wiita-potential.md), radial force balance gives

$$
R\Omega^2=\frac{d\Phi}{dR}=\frac{GM}{(R-R_S)^2},\qquad \Omega^2=\frac{GM}{R(R-R_S)^2}.
$$

Its [specific angular momentum](../../../../../specific-angular-momentum.md) is $j=R^2\Omega=\sqrt{GM}R^{3/2}/(R-R_S)$. Perturbing the circular radius at fixed $j$ gives the [radial epicyclic frequency](../../../../../radial-epicyclic-frequency.md) squared $\kappa^2=R^{-3}d(j^2)/dR$. Therefore

$$
\boxed{\kappa^2(R)=\frac{GM(R-3R_S)}{R(R-R_S)^3}=\Omega^2\frac{R-3R_S}{R-R_S}.}
$$

Circular motion is radially stable for $R>3R_S$, marginal at $3R_S$, and unstable between $R_S$ and $3R_S$. Thus **the inner edge of the nearly circular thin accretion disk is $R_{\mathrm{in}}=3R_S$**, joining a [plunging region of a black-hole accretion disk](../../../../../plunging-region-of-a-black-hole-accretion-disk.md) inside the [innermost stable circular orbit](../../../../../innermost-stable-circular-orbit.md). This conclusion concerns the circular thin-disk model, not an assertion that all gas disappears inside this radius.

Take the inward [mass accretion rate](../../../../../mass-accretion-rate.md) $\dot M$ as positive, and write the positive outward [viscous torque in an accretion disk](../../../../../viscous-torque-in-an-accretion-disk.md) as

$$
\mathcal G=-2\pi\nu\Sigma R^3\Omega'(R).
$$

Steady [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) makes the net inward flux $C=\dot M j-\mathcal G$ independent of radius. Impose a [zero-torque inner boundary condition](../../../../../zero-torque-inner-boundary-condition.md) at $3R_S$, appropriate to an approximately stress-free transition to plunging motion. Then

$$
\boxed{C=\dot Mj_{\mathrm{in}}=\frac{3\sqrt3}{2}\dot M\sqrt{GMR_S},\qquad\mathcal G=\dot M(j-j_{\mathrm{in}}).}
$$

This is the [steady accretion disk with arbitrary rotation law](../../../../../steady-accretion-disk-with-arbitrary-rotation-law.md) angular-momentum balance.

The local [viscous dissipation](../../../../../viscous-dissipation.md) integrated through the full disk thickness is $D=\nu\Sigma(R\Omega')^2=-\mathcal G\Omega'/(2\pi R)$. It is the power per unit planar area summed over both radiating faces. Since

$$
-\Omega'=\frac{\sqrt{GM}(3R-R_S)}{2R^{3/2}(R-R_S)^2},\qquad
\frac{j_{\mathrm{in}}}{j}=\frac{3\sqrt3}{2}\left(\frac{R_S}{R}\right)^{1/2}\frac{R-R_S}{R},
$$

substitution gives the [two-face dissipation of a Paczyński-Wiita disk](../../../../../two-face-dissipation-of-a-paczynski-wiita-disk.md):

$$
\boxed{D(R)=\frac{GM\dot M(3R-R_S)}{4\pi R(R-R_S)^3}\left[1-\frac{3\sqrt3}{2}\left(\frac{R_S}{R}\right)^{1/2}\frac{R-R_S}{R}\right].}
$$

In particular $D$ vanishes at the stress-free inner edge and is nonnegative outside it because $j$ increases there. A one-face radiative flux is $D/2$; the total [accretion luminosity](../../../../../accretion-luminosity.md) is therefore $L=\int_{3R_S}^\infty2\pi R D\,dR$, with no additional factor of two.

For a direct evaluation put $x=R/R_S$. Then

$$
L=\frac{GM\dot M}{2R_S}\left\{\int_3^\infty\frac{3x-1}{(x-1)^3}dx-\frac{3\sqrt3}{2}\int_3^\infty\frac{3x-1}{x^{3/2}(x-1)^2}dx\right\}.
$$

The first integral is $7/4$, using $(3x-1)/(x-1)^3=3/(x-1)^2+2/(x-1)^3$. For the second,

$$
\frac{d}{dx}\frac1{\sqrt x(x-1)}=-\frac{3x-1}{2x^{3/2}(x-1)^2},
$$

so it equals $2/[\sqrt3(3-1)]=1/\sqrt3$. Hence

$$
\boxed{L=\frac{GM\dot M}{8R_S}=\frac1{16}\dot M c^2,\qquad\epsilon=\frac1{16}.}
$$

This is the [radiative efficiency of black-hole accretion](../../../../../radiative-efficiency-of-black-hole-accretion.md) within this pseudo-Newtonian model.

Independently, the [specific orbital energy](../../../../../specific-orbital-energy.md) of a circular particle is

$$
E(R)=\frac12R^2\Omega^2+\Phi(R)=\frac{GM(2R_S-R)}{2(R-R_S)^2}.
$$

Thus $E(\infty)=0$ and $E(3R_S)=-GM/(8R_S)=-c^2/16$. The energy released per unit accreted mass is exactly $c^2/16$, confirming the integrated [accretion luminosity](../../../../../accretion-luminosity.md). The [Paczyński-Wiita circular orbit](../../../../../paczynski-wiita-circular-orbit.md) reproduces the Schwarzschild inner radius but gives an approximate binding energy; the efficiency derived here is for the stated potential.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
