<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In a stationary axisymmetric [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md), [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) gives $L_z=R^2\dot\phi$. Eliminating $\dot\phi$ introduces the [effective potential](../../../../../effective-potential.md)

$$
\Phi_{\rm eff}(R,z)=\Phi(R,z)+\frac{L_z^2}{2R^2},\qquad\ddot R=-\partial_R\Phi_{\rm eff},\quad\ddot z=-\partial_z\Phi.
$$

For an equatorial [circular orbit](../../../../../circular-orbit.md), radial balance is $\partial_R\Phi_{\rm eff}(R_c,0)=0$, giving

$$
\boxed{\Phi_{,R}(R_c,0)=\frac{L_z^2}{R_c^3}.}
$$

Vertical balance also requires $\Phi_{,z}(R_c,0)=0$.

For [epicyclic motion](../../../../../epicyclic-motion.md), assume a twice differentiable stationary [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) symmetric under $z\mapsto-z$, small displacements $|x|,|z|\ll R_c$, and a stable [circular orbit](../../../../../circular-orbit.md). Choose the [epicyclic guiding center](../../../../../epicyclic-guiding-center.md) using the conserved $L_z$. Reflection symmetry makes $\Phi_{,Rz}(R_c,0)=0$, eliminating radial-vertical coupling at first order. Expanding the equations about $(R_c,0)$ gives

$$
\boxed{\ddot x=-\kappa^2x,\qquad\ddot z=-\nu^2z,\qquad\kappa^2=\Phi_{,RR}+\frac{3L_z^2}{R_c^4},\quad\nu^2=\Phi_{,zz}.}
$$

The derivatives are evaluated at the guiding centre, and stability requires $\kappa^2,\nu^2>0$. Without midplane symmetry, a mixed Hessian term can couple the two oscillations. The [radial epicyclic frequency](../../../../../radial-epicyclic-frequency.md) and [vertical epicyclic frequency](../../../../../vertical-epicyclic-frequency.md) are the frequencies of these independent linear oscillations.

Set $\Omega=L_z/R_c^2$. Along the family of equatorial [circular orbits](../../../../../circular-orbit.md), $\Phi_{,R}=R\Omega^2$. Differentiating this relation and adding the centrifugal contribution gives

$$
\boxed{\kappa^2=R\frac{d\Omega^2}{dR}+4\Omega^2.}
$$

To interpret the common frequency range, let $q=d\log v_c/d\log R$. Since $v_c=R\Omega$, one has $\kappa^2=2(1+q)\Omega^2$. A [Keplerian disk](../../../../../keplerian-disk.md) has $q=-1/2$ and $\kappa=\Omega$, a [flat galaxy rotation curve](../../../../../flat-galaxy-rotation-curve.md) has $q=0$ and $\kappa=\sqrt2\Omega$, and [solid-body rotation](../../../../../solid-body-rotation.md) has $q=1$ and $\kappa=2\Omega$. Typical galactic [rotation curves](../../../../../galaxy-rotation-curve.md) lie between these slopes. Thus **$\Omega\lesssim\kappa\lesssim2\Omega$ is a useful galactic range**, not a theorem for every possible axisymmetric potential. As a precise sufficient example, [epicyclic frequency bounds for monotone spherical density](../../../../../epicyclic-frequency-bounds-for-monotone-spherical-density.md) follow from $\kappa^2=\Omega^2+4\pi G\rho$ and $0\leq\rho\leq3M/(4\pi R^3)$.

Use a Cartesian frame rotating with the [epicyclic guiding center](../../../../../epicyclic-guiding-center.md), with $x$ pointing radially outwards and $y=R_c(\phi-\Omega t)$ in the direction of rotation. To first order, [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) gives

$$
\dot\phi=\frac{L_z}{(R_c+x)^2}=\Omega\left(1-\frac{2x}{R_c}\right)+O(x^2/R_c^2),\qquad\dot y=-2\Omega x.
$$

The radial [harmonic oscillator](../../../../../simple-harmonic-motion.md) solution and its azimuthal integral are

$$
\boxed{x=X\cos(\kappa t+\chi),\qquad y=-\frac{2\Omega X}{\kappa}\sin(\kappa t+\chi)=-Y\sin(\kappa t+\chi),\qquad\frac XY=\frac\kappa{2\Omega}.}
$$

A constant in $y$ merely changes the azimuthal origin of the guiding centre. The [epicyclic ellipse](../../../../../epicyclic-ellipse.md) obeys $x^2/X^2+y^2/Y^2=1$. In the usual frequency range it is elongated azimuthally, and the star travels clockwise when $x$ points right and $y$ up: its small motion relative to the prograde guiding centre is retrograde.

For the [Oort constants](../../../../../oort-constants.md), subtract the defining expressions to obtain $\Omega=A-B$ and insert $R\Omega'=-2A$ into the [radial epicyclic frequency](../../../../../radial-epicyclic-frequency.md) formula:

$$
\kappa^2=4\Omega(\Omega-A)=-4\Omega B,\qquad\frac XY=\sqrt{\frac{-B}{A-B}}.
$$

The solar-neighbourhood values give $\Omega=26.5\,\mathrm{km\,s^{-1}\,kpc^{-1}}$, $\kappa=\sqrt{1272}\,\mathrm{km\,s^{-1}\,kpc^{-1}}$, and

$$
\boxed{X/Y=\sqrt{24/53}\simeq0.673.}
$$

The solar [epicyclic ellipse](../../../../../epicyclic-ellipse.md) is therefore about $1.49$ times longer azimuthally than radially.

A complete radial oscillation takes $T_r=2\pi/\kappa$. The oscillatory part of $\dot\phi$ has zero average over this interval, so the [epicyclic azimuthal advance](../../../../../epicyclic-azimuthal-advance.md) is

$$
\boxed{\Delta\psi=\Omega T_r=\frac{2\pi\Omega}{\kappa}=2\pi\left(4+\frac{d\log\Omega^2}{d\log R}\right)^{-1/2}.}
$$

This describes the advance between consecutive radial turning points of the same type; it need not be a full $2\pi$ revolution. For the Sun,

$$
\boxed{\Delta\psi=\pi\sqrt{53/24}\simeq4.669\ \mathrm{rad}\simeq267.5^\circ.}
$$

The azimuthal advance estimate uses the same linear [epicyclic motion](../../../../../epicyclic-motion.md) approximation as the axis ratio.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
