<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Measure [pressure](../../../../../pressure.md) relative to its hydrostatic value and let $\Delta P$ be the lower-side excess [pressure](../../../../../pressure.md) minus the upper-side excess [pressure](../../../../../pressure.md). The long unobstructed parts of the tube act as Poiseuille resistances in series. Their lengths add to $L$ at leading order because $l\ll L$; entrance and exterior resistances are smaller for $L\gg a$. Consequently

$$
\boxed{Q=\frac{\pi a^4\Delta P}{8\mu L}.}
$$

Here $Q$ is downward laboratory-frame [volume flux](../../../../../volumetric-flow-rate.md).

Take $z$ upwards in the particle frame and let $s$ measure distance from the particle surface to the tube wall. In this frame the particle is stationary and the wall moves upwards at speed $U$. In the thin, slowly varying gap, [pressure](../../../../../pressure.md) is uniform across $s$ and the leading axial [Stokes equation](../../../../../stokes-equation.md) is $\mu w_{ss}=p_z$. No slip gives

$$
w(s)=\frac{p_z}{2\mu}s(s-h)+\frac{Us}{h},\qquad q=\int_0^h w(s)ds=-\frac{h^3p_z}{12\mu}+\frac{Uh}{2}.
$$

The gap's upward relative flux is constant, while conservation of displaced volume gives $2\pi aq=\pi a^2U-Q$. Thus $p_z=6\mu U/h^2-12\mu q/h^3$, and integration from bottom to top yields

$$
\boxed{\frac{\Delta P}{6\mu}=2qI_3-UI_2,\qquad q=\frac{\pi a^2U-Q}{2\pi a}.}
$$

[Curvature](../../../../../curvature.md) corrections to the gap circumference are relative order $h/a$. Rapid end regions do not contribute to the leading singular neck resistance.

For the [force](../../../../../force.md) use a cylindrical fluid [control volume](../../../../../control-volume.md) containing the particle, with full-area end caps just beyond it and the particle surface as an inner boundary. The upward [pressure](../../../../../pressure.md) [force](../../../../../force.md) on the caps is $\pi a^2\Delta P$. The outer wall exerts axial [traction](../../../../../traction.md) $\mu w_s(h)$ on the fluid, whereas the particle's [traction](../../../../../traction.md) on the fluid integrates to minus its upward hydrodynamic resistance $F$. The zero-inertia momentum balance is therefore

$$
F=\pi a^2\Delta P+2\pi a\int\mu w_s(h)dz.
$$

The [velocity](../../../../../velocity.md) profile gives $w_s(h)=4U/h-6q/h^2$, proving

$$
\boxed{F=\pi a^2\Delta P+2\pi a\mu(4UI_1-6qI_2).}
$$

Using the outer-wall [traction](../../../../../traction.md) is essential; directly using the particle-side shear and a flat-end [pressure](../../../../../pressure.md) [force](../../../../../force.md) would omit the [pressure](../../../../../pressure.md) on the sloping particle surface. This is [control-volume drag formula for a sphere in a tube](../../../../../control-volume-drag-formula-for-a-sphere-in-a-tube.md).

The four dimensionless relations are

$$
Q^*=\delta\Delta P^*,\quad\Delta P^*=4q^*I_3^*-I_2^*,\quad4q^*=1-Q^*,\quad F^*=\Delta P^*+\frac43I_1^*-4q^*I_2^*.
$$

Solving them gives

$$
\boxed{\Delta P^*=\frac{I_3^*-I_2^*}{1+\delta I_3^*},\quad Q^*=\frac{\delta(I_3^*-I_2^*)}{1+\delta I_3^*},\quad q^*=\frac{1+\delta I_2^*}{4(1+\delta I_3^*)}.}
$$

Within the preceding lubrication and tube-resistance approximations, the [force](../../../../../force.md) is

$$
F^*=\frac{I_3^*-2I_2^*+\tfrac43I_1^*+\delta(\tfrac43I_1^*I_3^*-(I_2^*)^2)}{1+\delta I_3^*}.
$$

Since $h/a\ll1$, $I_3^*\gg I_2^*\gg I_1^*$. Dropping the smaller additive $-2I_2^*+4I_1^*/3$ terms in the numerator yields the requested leading formula

$$
\boxed{F^*\sim\frac{I_3^*+\delta(\tfrac43I_1^*I_3^*-(I_2^*)^2)}{1+\delta I_3^*}.}
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $(I_2^*)^2\le I_1^*I_3^*$, so the retained $\delta$ term is positive. The term multiplied by $\delta$ must be retained: it can compete with $I_3^*$ even though the unmultiplied lower [integrals](../../../../../integral.md) cannot.

For a [sphere](../../../../../sphere.md) of radius $a(1-\epsilon)$, the neck has $h=a\epsilon+z^2/(2a)$ at leading order. With $z=a\sqrt{2\epsilon}\,t$, the [integrals](../../../../../integral.md) reduce to $\sqrt2\epsilon^{1/2-n}\int_{-\infty}^\infty(1+t^2)^{-n}dt$. For $n=1,2,3$ these last [integrals](../../../../../integral.md) are $\pi,\pi/2,3\pi/8$, giving the full two-sided [integrals](../../../../../integral.md). Put

$$
c_1=\pi\sqrt2,\quad c_2=\frac\pi{\sqrt2},\quad c_3=\frac{3\pi}{4\sqrt2};\qquad \frac43c_1c_3-c_2^2=\frac{\pi^2}{2}.
$$

**The printed [sphere](../../../../../sphere.md) [integrals](../../../../../integral.md) are half these values:** they correspond to integrating over one side of the neck rather than the stated interval spanning both sides. The substitution above establishes the [radius-deficit normalization of sphere-tube lubrication integrals](../../../../../radius-deficit-normalization-of-sphere-tube-lubrication-integrals.md). Using the two-sided values, the [force](../../../../../force.md) becomes

$$
F^*\sim\frac{c_3\epsilon^{-5/2}+\delta(\pi^2/2)\epsilon^{-3}}{1+\delta c_3\epsilon^{-5/2}},
$$

so the three answers are

$$
\boxed{F^*\sim\begin{cases}\dfrac{3\pi}{4\sqrt2}\epsilon^{-5/2}&\delta\ll\epsilon^{5/2},\\[3pt]\delta^{-1}&\epsilon^{5/2}\ll\delta\ll\epsilon^{1/2},\\[3pt]\dfrac{2\pi\sqrt2}{3}\epsilon^{-1/2}&\epsilon^{1/2}\ll\delta.\end{cases}}
$$

These are the corrected [sphere-tube drag regimes with a radius-deficit gap](../../../../../sphere-tube-drag-regimes-with-a-radius-deficit-gap.md). If the supplied half-integrals are treated as stipulated data instead, the same algebra gives $3\pi\epsilon^{-5/2}/(8\sqrt2)$, $1/\delta$ and $\pi\sqrt2\epsilon^{-1/2}/3$ in the three regimes. Thus the first and third numerical drag coefficients double when the geometrically correct [integrals](../../../../../integral.md) are used; the regime boundaries and dominant flow patterns are unchanged.

In the first regime, $Q^*\sim\delta c_3\epsilon^{-5/2}\ll1$, $q^*\sim1/4$, and $\Delta P^*\sim c_3\epsilon^{-5/2}\sim F^*$. Almost no displaced fluid escapes through the long tube; it bypasses upwards through the thin annulus. The large pressure-driven bypass resistance sets the drag, with shear smaller.

In the second regime, $Q^*\sim1$, $\Delta P^*\sim F^*\sim1/\delta$, and

$$
q^*\sim\frac{\sqrt2}{3\pi}\frac{\epsilon^{5/2}}\delta+\frac\epsilon3\ll1.
$$

Almost all displaced volume travels through the unobstructed tube, whose [pressure](../../../../../pressure.md) resistance dominates the [force](../../../../../force.md). Both terms in this small gap flux are worth displaying: their crossover at $\delta\sim\epsilon^{3/2}$ changes the balance between pressure-driven and wall-driven gap transport but does not create a fourth leading [force](../../../../../force.md) regime.

In the third regime, $1-Q^*\sim4\epsilon/3$, $q^*\sim\epsilon/3$, and $\Delta P^*\sim1/\delta\ll F^*$. Tube throughflow still carries almost all the displaced volume, but the dominant resistance is local annular lubrication rather than the net tube [pressure](../../../../../pressure.md) drop. The relative gap flux is now of order $Uh$, so wall-driven and pressure-driven components both matter locally. The formulas describe hydrodynamic resistance after subtracting hydrostatic buoyancy; terminal settling would balance it against the particle's excess weight.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
