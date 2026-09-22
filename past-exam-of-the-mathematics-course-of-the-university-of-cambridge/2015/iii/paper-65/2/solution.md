<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In the [center of mass](../../../../../center-of-mass.md) frame, the velocities are $\mathbf v_1=(M_2/M)\mathbf v$ and $\mathbf v_2=-(M_1/M)\mathbf v$. Hence the [kinetic energy](../../../../../kinetic-energy.md) is $T=\frac12\mu v^2$, while the [Newtonian gravitational potential energy](../../../../../newtonian-gravitational-potential-energy.md) is $U=-GM_1M_2/r=-GM\mu/r$. The [two-body orbital energy](../../../../../two-body-orbital-energy.md) is therefore

$$
\boxed{E=\mu\varepsilon=\mu\left(\frac12v^2-\frac{GM}{r}\right),}\qquad\mu=\frac{M_1M_2}{M}.
$$

The relative equation of [Newtonian gravity](../../../../../gravitational-acceleration.md) is $\ddot{\mathbf r}=-GM\mathbf r/r^3$. It is a [central force](../../../../../central-force.md), so [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) confines the motion to a plane and preserves the [specific angular momentum](../../../../../specific-angular-momentum.md) $h=|\mathbf r\times\mathbf v|=r^2\dot\theta$.

For completeness, derive the [polar equation of a Kepler orbit](../../../../../polar-equation-of-a-kepler-orbit.md). Let $w=1/r$ and use primes for $\theta$ derivatives. Then $\dot r=-hw'$ and $\ddot r-r\dot\theta^2=-h^2w^2(w''+w)$. The radial equation gives the [Binet equation](../../../../../binet-equation.md)

$$
w''+w=\frac{GM}{h^2}.
$$

Choose the angular origin at closest approach. Its solution is $w=(GM/h^2)(1+e\cos\theta)$, so

$$
\boxed{r=\frac{l}{1+e\cos\theta},\qquad l=\frac{h^2}{GM}.}
$$

For the [ellipse](../../../../../ellipse.md), the [orbital eccentricity](../../../../../orbital-eccentricity.md) satisfies $0\le e<1$. Its extreme separations are $r_p=l/(1+e)$ and $r_a=l/(1-e)$. The [semi-major axis](../../../../../semi-major-axis.md) is half their sum, giving $a=l/(1-e^2)$ and thus $l=a(1-e^2)$. The [true anomaly](../../../../../true-anomaly.md) $\theta$ runs through a full $2\pi$; the endpoints are the same position, and for a [circular Kepler orbit](../../../../../circular-kepler-orbit.md) the angular origin is arbitrary.

The radial and transverse relative speeds are $\dot r=(GM/h)e\sin\theta$ and $r\dot\theta=h/r$. Substituting these into the [specific orbital energy](../../../../../specific-orbital-energy.md) gives

$$
\varepsilon=\frac{GM}{2l}\left[e^2\sin^2\theta+(1+e\cos\theta)^2-2(1+e\cos\theta)\right]
=\frac{GM}{2l}(e^2-1).
$$

Therefore **the conserved orbital energy is**

$$
\boxed{E=-\frac{GM\mu}{2a}.}
$$

The negative [specific orbital energy](../../../../../specific-orbital-energy.md) and fixed [angular momentum](../../../../../angular-momentum.md) characterize the bound [Kepler orbit](../../../../../kepler-orbit.md); neither should be assumed unchanged through a mass-ejecting explosion.

Initially the [circular Kepler orbit](../../../../../circular-kepler-orbit.md) has $r=a$ and $v^2=GM/a$. Treat the [supernova kick in a binary star](../../../../../supernova-kick-in-a-binary-star.md) as impulsive: the relative position does not change, the companion's velocity is unchanged during the impulse, and the new [neutron star](../../../../../neutron-star.md) receives $\mathbf u$ with $|\mathbf u|=\alpha v$. Thus $\mathbf v'=\mathbf v+\mathbf u$, and with $\psi$ the angle between these vectors before the kick,

$$
|\mathbf v'|^2=v^2S,\qquad S=1+2\alpha\cos\psi+\alpha^2.
$$

Write $M'=M_1'+M_2$, $\beta=M'/M$ and $\mu'=M_1'M_2/M'$. The post-explosion [specific orbital energy](../../../../../specific-orbital-energy.md) is

$$
\varepsilon'=\frac12v^2S-\frac{GM'}a=\frac{GM}{2a}(S-2\beta).
$$

Using $\varepsilon'=-GM'/(2a')$ gives

$$
\boxed{\frac{M'}{a'}=\frac{2M'}a-\frac Ma(1+2\alpha\cos\psi+\alpha^2).}
$$

Here $a'>0$ for a bound [Kepler orbit](../../../../../kepler-orbit.md). For a [hyperbolic Kepler orbit](../../../../../hyperbolic-kepler-orbit.md), this formula uses the signed energy parameter $a'<0$, rather than the positive geometric magnitude of the hyperbola's [semi-major axis](../../../../../semi-major-axis.md). At the [parabolic Kepler orbit](../../../../../parabolic-trajectory.md) boundary, $1/a'=0$.

The [kick-direction binary survival criterion](../../../../../kick-direction-binary-survival-criterion.md) is **bound if $S<2\beta$ and unbound with positive asymptotic speed if $S>2\beta$**. To prove the printed sufficient disruption condition, choose a perpendicular kick, $\cos\psi=0$: then $S=1+\alpha^2$, so $M'<\frac12(1+\alpha^2)M$ produces positive [specific orbital energy](../../../../../specific-orbital-energy.md). This is sufficient, not the sharp existence threshold. Since

$$
(1-\alpha)^2\le S\le(1+\alpha)^2,
$$

the complete [kick-direction binary survival criterion](../../../../../kick-direction-binary-survival-criterion.md) is

$$
\boxed{\begin{aligned}
\text{some direction gives }\varepsilon'>0&\iff\beta<\tfrac12(1+\alpha)^2,\\
\text{some direction remains bound}&\iff\beta>\tfrac12(1-\alpha)^2.
\end{aligned}}
$$

The second inequality follows by taking a kick directly opposite to $\mathbf v$. All directions remain bound if $2\beta>(1+\alpha)^2$, while every direction has positive escape energy if $2\beta<(1-\alpha)^2$. For $\alpha>0$, the marginal direction obeys $\cos\psi=(2\beta-1-\alpha^2)/(2\alpha)$ when the right-hand side lies in $[-1,1]$. Equalities give marginal [parabolic Kepler orbits](../../../../../parabolic-trajectory.md) for the relevant extreme direction. With zero kick, losing more than half the original total mass unbinds the [circular Kepler orbit](../../../../../circular-kepler-orbit.md).

For an escaping pair, the [Newtonian gravitational potential energy](../../../../../newtonian-gravitational-potential-energy.md) approaches zero at infinite separation. Conservation of the post-explosion [two-body orbital energy](../../../../../two-body-orbital-energy.md) then gives $\frac12\mu'V^2=\mu'\varepsilon'$, or the [asymptotic relative speed of a disrupted binary](../../../../../asymptotic-relative-speed-of-a-disrupted-binary.md)

$$
\boxed{V=v\sqrt{1+2\alpha\cos\psi+\alpha^2-\frac{2M'}M}.}
$$

This is the relative recession speed, not the velocity of the new [center of mass](../../../../../center-of-mass.md) or either star's individual velocity in the original [inertial frame](../../../../../inertial-frame.md). A marginal [parabolic Kepler orbit](../../../../../parabolic-trajectory.md) separates with $V=0$ at infinity.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
