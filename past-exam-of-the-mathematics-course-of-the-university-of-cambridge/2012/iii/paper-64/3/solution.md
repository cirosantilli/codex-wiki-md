<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use rotating barycentric coordinates $\mathbf R=(x,y,z)$, rotating velocity $\mathbf w$, and $\boldsymbol\Omega=\widehat{\mathbf z}$. Multiplying the three equations by the corresponding velocity components and adding cancels the [Coriolis force](../../../../../coriolis-force.md) terms:

$$
\frac{d}{dt}\frac{|\mathbf w|^2}{2}=\nabla U\cdot\mathbf w=\frac{dU}{dt}.
$$

Thus the [Jacobi constant](../../../../../jacobi-constant.md) is $C=2U-|\mathbf w|^2$. The inertial barycentric velocity is $\mathbf V=\mathbf w+\boldsymbol\Omega\times\mathbf R$. If $H_z=(\mathbf R\times\mathbf V)_z$ and $E_b=|\mathbf V|^2/2-\mu_1/r_1-\mu_2/r_2$, then

$$
|\mathbf w|^2=|\mathbf V|^2+x^2+y^2-2H_z,
\qquad \boxed{C=-2E_b+2H_z}.
$$

The inertial energy $E_b$ and inertial [angular momentum](../../../../../angular-momentum.md) $H_z$ need not separately be constant. Their combination is constant because the two gravitational sources rotate steadily at unit [angular speed](../../../../../angular-speed.md).

For the [Tisserand parameter](../../../../../tisserand-parameter.md) take $\mu_2\ll\mu_1\simeq1$, and compare the [osculating orbital elements](../../../../../osculating-orbital-element.md) well outside a close encounter, where $\mu_2/r_2$ and barycentre-to-primary corrections are negligible. Then

$$
C=\frac{\mu_1}{a}+2\sqrt{\mu_1a(1-e^2)}\cos I+\text{small corrections}
\simeq\boxed{T=\frac1a+2\sqrt{a(1-e^2)}\cos I}.
$$

This requires a circular secondary orbit, the [restricted three-body problem](../../../../../restricted-three-body-problem.md) approximation, and no dissipative force or other perturber. $T$ is conserved to leading order between encounter episodes; the osculating $T$ during a close encounter need not be constant. The exact invariant is $C$.

For clarity the exact two-body energy relation is $a=\mu_1/(2\mu_1/r_1-v_1^2)$, rather than the printed formula without the numerator $\mu_1$. At the leading order $\mu_1=1$ used for $T$, the two agree; retaining finite $\mu_1$ in just part of that formula is inconsistent.

At a close encounter put the secondary radius and speed equal to one at leading order, and denote the particle's incoming relative speed outside the secondary's strong-deflection region by $u$. Conservation of relative speed in the short gravitational encounter gives

$$
|\Delta\mathbf v_1|\le2u.
$$

An incoming orbit with $a=1$ has $|\mathbf v_1|=1$ at $r_1=1$ by the [vis-viva equation](../../../../../vis-viva-equation.md); escape there requires an outgoing speed exceeding $\sqrt2$. The triangle inequality therefore gives the necessary [single-encounter escape velocity bound](../../../../../single-encounter-escape-velocity-bound.md)

$$
\sqrt2<|\mathbf v_{1,\rm out}|\le1+2u,
\qquad \boxed{u>\frac{\sqrt2-1}{2}}.
$$

Equality only gives a marginal parabolic limit. This argument deliberately gives a weak necessary bound, not a sufficient scattering criterion.

The [planet-encounter relative velocity](../../../../../planet-encounter-relative-velocity.md) is related to the [Tisserand parameter](../../../../../tisserand-parameter.md) by

$$
u^2=v_1^2+1-2v_{1,\rm tangential}=3-T.
$$

Here $v_{1,\rm tangential}=h_z$ at the encounter radius, and the formula also applies to inclined passages at the [planet](../../../../../planet.md)'s orbital plane. For the intended prograde coplanar incoming orbit, $I=0$ and $a=1$, so $u^2=2-2\sqrt{1-e^2}$. Applying the preceding necessary bound gives

$$
\sqrt{1-e^2}<1-\frac{3-2\sqrt2}{8}=\frac{5+2\sqrt2}{8},
\qquad \boxed{e>\frac18\sqrt{31-20\sqrt2}}.
$$

Coplanar alone also allows $I=\pi$. For that retrograde case $u^2=2+2\sqrt{1-e^2}$, and even a circular incoming orbit can be scattered onto an escaping orbit; the [orbital eccentricity](../../../../../orbital-eccentricity.md) restriction therefore presumes prograde motion. Also, retaining the outgoing relative-velocity geometry gives the sharper necessary condition $|\mathbf v_{1,\rm out}|\le1+u$, hence $u>\sqrt2-1$ and $e>\sqrt{4\sqrt2-5}/2$ for the same prograde incoming orbit. This stronger bound is consistent with, and implies, the weaker bound above.

For the [Tisserand periapsis bound](../../../../../tisserand-periapsis-bound.md), first write

$$
a=\frac{q+Q}{2},\qquad a(1-e^2)=\frac{2qQ}{q+Q},\qquad
\boxed{T=\frac2{q+Q}+2\sqrt{\frac{2qQ}{q+Q}}\cos I}.
$$

A bound orbit capable of another close encounter must intersect the secondary's circular radius, so $q\le1\le Q$. For fixed $q<1$, the largest possible $T$ occurs at $I=0$. The remaining expression decreases with $Q\ge1$, since

$$
\frac{\partial T(q,Q,0)}{\partial Q}
=\frac2{(q+Q)^2}\left[-1+\frac{q^2}{\sqrt{2qQ/(q+Q)}}\right]<0.
$$

Thus every such orbit obeys

$$
T\le g(q)=\frac2{1+q}+2\sqrt{\frac{2q}{1+q}}.
$$

On $0<q<1$, $g(q)$ increases monotonically from $2$ to $3$. For $2<T<3$ the least accessible [pericentre](../../../../../periapsis.md) is the unique root of $T=g(q)$: the limiting orbit is prograde and coplanar, with [apocentre](../../../../../apoapsis.md) just at the [planet](../../../../../planet.md). Introduce $s=\sqrt{3-T}$. Its tangential speed at this [apocentre](../../../../../apoapsis.md) is $1-s$, and its [vis-viva equation](../../../../../vis-viva-equation.md) gives the particularly well-behaved answer

$$
\boxed{q_{\min}=\frac{(1-\sqrt{3-T})^2}{1+2\sqrt{3-T}-(3-T)}}\qquad(2<T<3).
$$

Equivalently, setting $w=\sqrt{2q/(1+q)}$ gives $T=2-w^2+2w$ and $w=1-s$, with $q=w^2/(2-w^2)$. Rationalizing the previous result yields

$$
\boxed{q_{\min}=\frac{4+2T-T^2-4\sqrt{3-T}}{T^2-8}}.
$$

The apparent singularity at $T=\sqrt8$ is removable; the first form gives $q_{\min}=(\sqrt2-1)/2$ there. The limits are $q_{\min}\to0$ as $T\downarrow2$ and $q_{\min}\to1$ as $T\uparrow3$. The same lower envelope also excludes a smaller [pericentre](../../../../../periapsis.md) on an escaping trajectory when $2<T<3$. To see this without introducing an [apocentre](../../../../../apoapsis.md), use the [planet](../../../../../planet.md)-frame velocity sphere: $u=\sqrt{3-T}<1$ forces the tangential component at an encounter to be at least $w=1-u>0$, so total [specific angular momentum](../../../../../specific-angular-momentum.md) obeys $h\ge w$. At [pericentre](../../../../../periapsis.md) the stellar energy obeys $h^2=2q+2E q^2$, while $E=h_z-T/2\le h-T/2$. Thus

$$
h^2-2hq^2\le2q-Tq^2.
$$

If $q<q_{\min}=w^2/(2-w^2)$, then $q^2<w\le h$, and the left side is increasing with $h$. Hence $w^2\le2q+(2w-T)q^2$. But $2w-T=w^2-2$, and the right side is smaller than $w^2$ for $0\le q<q_{\min}$, a contradiction. This establishes the barrier for all Kepler trajectories that reach the encounter radius, including unbound ones.

For $0<T\le2$, bound encounter-crossing orbits can approach $q=0$ (take $Q\to2/T$), so the positive root extrapolated from the displayed expression is not a universal barrier. For $T>3$ there is no trajectory reaching a close encounter in this approximation, since $u^2=3-T$ would be negative. Multiple encounters can approach the derived lower envelope by changing energy, [angular momentum](../../../../../angular-momentum.md) and inclination while preserving the [Tisserand parameter](../../../../../tisserand-parameter.md); the invariant alone does not guarantee a particular encounter history reaches it.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
