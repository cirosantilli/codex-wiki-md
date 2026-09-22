<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

[Newton's second law](../../../../../newton-s-second-law.md) takes its familiar form $m\mathbf a=\mathbf F$ in an [inertial frame](../../../../../inertial-frame.md). Axes fixed to a turning apparatus or to the [Earth](../../../../../earth.md) form a [rotating reference frame](../../../../../rotating-reference-frame.md). Extra [inertial forces](../../../../../fictitious-force.md) account for the [acceleration](../../../../../acceleration.md) of these coordinates. Their values depend on the chosen [reference frame](../../../../../reference-frame.md); physical interactions such as [gravity](../../../../../gravity.md), [tension](../../../../../tension.md) and contact [forces](../../../../../force-split.md) must still be included separately.

Let the rotating origin have inertial [acceleration](../../../../../acceleration.md) $\mathbf A$, and let its axes have [angular velocity](../../../../../angular-velocity.md) $\boldsymbol\Omega(t)$. For any [vector](../../../../../vector.md) $\mathbf q$, the [rotating-frame derivative formula](../../../../../rotating-frame-derivative-formula.md) is

$$
\left(\frac{d\mathbf q}{dt}\right)_{\rm I}=\left(\frac{d\mathbf q}{dt}\right)_{\rm R}+\boldsymbol\Omega\times\mathbf q.
$$

Each rotating [basis vector](../../../../../basis-vector.md) changes by $\boldsymbol\Omega\times\mathbf e_i$, which proves this rule by expanding $\mathbf q$ in that basis. Apply it twice to the position relative to the moving origin. With $\mathbf v'$ and $\mathbf a'$ measured in the rotating axes,

$$
\mathbf a_{\rm I}=\mathbf A+\mathbf a'+2\boldsymbol\Omega\times\mathbf v'+\dot{\boldsymbol\Omega}\times\mathbf r+\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf r).
$$

Consequently the equation in the [rotating reference frame](../../../../../rotating-reference-frame.md) is

$$
m\mathbf a'=\mathbf F-m\mathbf A-2m\boldsymbol\Omega\times\mathbf v'-m\dot{\boldsymbol\Omega}\times\mathbf r-m\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf r).
$$

The additional terms are the translational [inertial force](../../../../../fictitious-force.md), [Coriolis force](../../../../../coriolis-force.md), [Euler force](../../../../../euler-force.md) and [centrifugal force](../../../../../centrifugal-force.md), respectively. The last two simplify when the [angular velocity](../../../../../angular-velocity.md) is constant: the [Euler force](../../../../../euler-force.md) vanishes, while the other rotation terms remain.

The [centrifugal force](../../../../../centrifugal-force.md) points away from the rotation axis. If $\mathbf r_\perp$ is the perpendicular displacement from that axis, then

$$
\boxed{\mathbf F_{\rm cf}=m\Omega^2\mathbf r_\perp.}
$$

For uniform rotation it has [potential energy](../../../../../potential-energy.md)

$$
\Phi_{\rm cf}=-\frac12m|\boldsymbol\Omega\times\mathbf r|^2,\qquad \mathbf F_{\rm cf}=-\nabla\Phi_{\rm cf}.
$$

A mass at rest relative to a turntable can therefore be described as having an inward [tension](../../../../../tension.md) or [friction](../../../../../friction.md) balancing its outward [centrifugal force](../../../../../centrifugal-force.md). In an [inertial frame](../../../../../inertial-frame.md), the inward physical [force](../../../../../force-split.md) instead produces the required [centripetal acceleration](../../../../../centripetal-acceleration.md). These are two descriptions of the same motion; one must not insert the rotating-frame outward term into the inertial equation as an additional physical interaction.

A rotating liquid gives a useful quantitative example. For a liquid in [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) relative to a vessel rotating uniformly about the vertical axis,

$$
\frac{\partial p}{\partial s}=\rho\Omega^2s,\qquad \frac{\partial p}{\partial z}=-\rho g.
$$

Along the [free surface](../../../../../free-surface.md) the [pressure](../../../../../pressure-split.md) is constant, so $\Omega^2s\,ds-g\,dz=0$ and

$$
z(s)=z(0)+\frac{\Omega^2s^2}{2g}.
$$

The surface is a [elliptic paraboloid](../../../../../elliptic-paraboloid.md). This is the balance of [gravity](../../../../../gravity.md) and the [centrifugal force](../../../../../centrifugal-force.md) in the rotating description. On the [Earth](../../../../../earth.md), the same outward [acceleration](../../../../../acceleration.md) reduces effective [gravity](../../../../../gravity.md), most strongly at the equator, and contributes to the planet's equatorial bulge.

The [Coriolis force](../../../../../coriolis-force.md) depends on relative motion:

$$
\boxed{\mathbf F_{\rm cor}=-2m\boldsymbol\Omega\times\mathbf v'.}
$$

It is perpendicular to both $\boldsymbol\Omega$ and $\mathbf v'$, vanishes for motion along the rotation axis, and reverses when the relative [velocity](../../../../../velocity.md) reverses. The [dot product](../../../../../dot-product.md) gives

$$
\mathbf F_{\rm cor}\cdot\mathbf v'=0.
$$

Thus the [Coriolis force](../../../../../coriolis-force.md) does no [work](../../../../../work.md) in the [rotating reference frame](../../../../../rotating-reference-frame.md): it changes the direction of motion rather than directly changing the rotating-frame [kinetic energy](../../../../../kinetic-energy.md). For example, on a horizontal turntable rotating anticlockwise as viewed from above, an outward-moving slider has a clockwise [Coriolis acceleration](../../../../../coriolis-acceleration.md), whereas an inward-moving slider has an anticlockwise one. The deflection can be observed by comparing a laboratory camera with a camera rotating with the table.

For slow horizontal motion on the [Earth](../../../../../earth.md) at latitude $\lambda$, keep the vertical component $\Omega_E\sin\lambda$ of its [angular velocity](../../../../../angular-velocity.md). In east-north coordinates $(u,v)$ the horizontal [Coriolis acceleration](../../../../../coriolis-acceleration.md) is

$$
(a_E,a_N)=(fv,-fu),\qquad f=2\Omega_E\sin\lambda.
$$

It deflects motion to the right in the northern hemisphere and to the left in the southern hemisphere. In large-scale atmospheric and oceanic motion it can balance a horizontal [pressure gradient](../../../../../pressure-gradient.md), giving [geostrophic balance](../../../../../geostrophic-balance.md). With $\hat{\mathbf z}$ upward, the steady horizontal equation without [friction](../../../../../friction.md) is

$$
f\hat{\mathbf z}\times\mathbf v=-\frac1\rho\nabla_h p.
$$

The resulting [velocity](../../../../../velocity.md) runs along lines of equal [pressure](../../../../../pressure-split.md). This approximation requires rotation to dominate local inertial changes; it is inappropriate close to the equator where $f$ tends to zero.

The [Foucault pendulum](../../../../../foucault-pendulum.md) gives another terrestrial example. In the [small-angle approximation](../../../../../small-angle-approximation.md), its horizontal coordinates satisfy

$$
\ddot x+\omega_0^2x=f\dot y,\qquad \ddot y+\omega_0^2y=-f\dot x,\qquad \omega_0^2=\frac g\ell.
$$

To first order in the small ratio $\Omega_E/\omega_0$, the oscillation plane precesses relative to the ground at angular rate $-\Omega_E\sin\lambda$: clockwise in the northern hemisphere, zero at the equator, and one revolution per sidereal day at a pole. The [Coriolis force](../../../../../coriolis-force.md) explains this changing orientation without requiring [energy](../../../../../energy-split.md) input. Together these examples show why [inertial forces](../../../../../fictitious-force.md) are useful whenever the apparatus or environment supplies naturally rotating coordinates.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
