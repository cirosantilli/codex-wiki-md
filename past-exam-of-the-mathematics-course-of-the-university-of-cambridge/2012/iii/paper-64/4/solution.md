<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

At each fixed [semimajor axis](../../../../../semi-major-axis.md), let $B=b_{3/2}^{2}(\alpha)/b_{3/2}^{1}(\alpha)$ and $Z_f=B e_{\rm pl}$. The [planet](../../../../../planet.md)'s [longitude of pericentre](../../../../../longitude-of-periapsis.md) is the zero of longitude. The [secular perturbation](../../../../../secular-perturbation.md) equation becomes $\dot z=iA(z-Z_f)$. Integrating it with the initial condition $z(0)=0$ gives

$$
\boxed{z(t)=Z_f[1-e^{iAt}]}.
$$

The [forced eccentricity](../../../../../forced-eccentricity.md) vector is the constant real $Z_f$; the [free eccentricity](../../../../../proper-eccentricity.md) vector is $-Z_f e^{iAt}$. Consequently the [complex eccentricity](../../../../../complex-eccentricity.md) follows a circle in the [Argand plane](../../../../../complex-plane.md) centered at $Z_f$, with radius $Z_f$, starting at the origin and moving counterclockwise. Its initial velocity is downward, $\dot z(0)=-iAZ_f$. The secular period is $2\pi/A$, and

$$
e(t)=|z(t)|=2Z_f|\sin(At/2)|,\quad e_{\max}=2Z_f,\quad
\overline e=\frac{4Z_f}{\pi},\quad \sqrt{\overline{e^2}}=\sqrt2Z_f.
$$

The [longitude of pericentre](../../../../../longitude-of-periapsis.md) is undefined at the origin, but the [complex eccentricity](../../../../../complex-eccentricity.md) passes smoothly through it. At $At=\pi$, $z=2Z_f$ and the orbit is maximally eccentric and aligned with the [planet](../../../../../planet.md).

<a id="4/image-forced-and-free-eccentricity-vectors-tracing-a-secular-circle-in-the-argand-plane"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-64-eccentricity-circle.png)

**[Figure 2](#4/image-forced-and-free-eccentricity-vectors-tracing-a-secular-circle-in-the-argand-plane). Forced and free eccentricity vectors tracing a secular circle in the Argand plane**.

Using the small-$\alpha$ [Laplace coefficient](../../../../../laplace-coefficient.md) expansion gives

$$
b_{3/2}^{1}=3\alpha+O(\alpha^3),\qquad
b_{3/2}^{2}=\frac{15}{4}\alpha^2+O(\alpha^4),\qquad
Z_f=\frac54\alpha e_{\rm pl}[1+O(\alpha^2)].
$$

Also $n=n_{\rm pl}\alpha^{-3/2}$ to leading order in the [planet](../../../../../planet.md)-to-[star](../../../../../star.md) [mass](../../../../../mass.md) ratio. The [secular forcing by a distant outer planet](../../../../../secular-forcing-by-a-distant-outer-planet.md) is therefore

$$
A=\frac34n_{\rm pl}\frac{M_{\rm pl}}{M_\star}\alpha^{3/2}[1+O(\alpha^2)],
\qquad
\boxed{z(t)\simeq\frac54\alpha e_{\rm pl}\left[1-\exp\left(i\frac34n_{\rm pl}\frac{M_{\rm pl}}{M_\star}\alpha^{3/2}t\right)\right]}.
$$

A relative $O(\alpha^2)$ correction to $A$ can accumulate a phase error at very long times; the leading-frequency formula is not a uniform-in-time expansion.

If $a_2=a_1(1+\delta)$ with $\delta=\delta a/a_1\ll1$, then $Z_{f,2}/Z_{f,1}=1+\delta+O(\delta^2)$ and $A_2/A_1=1+3\delta/2+O(\delta^2)$. The outer [planetesimal](../../../../../planetesimal.md) therefore has a slightly larger [forced eccentricity circle](../../../../../forced-eccentricity-circle.md) and a shorter secular period. Its accumulated secular phase lead is $\Delta(At)\simeq3A_1t\delta/2$. Initially both circles start at the origin, but their [eccentricity vectors](../../../../../eccentricity-vector.md) progressively lose alignment. Linearizing the exponential in $\delta$ additionally requires $|A_1t\delta|\ll1$.

The [orbit crossing](../../../../../orbit-crossing.md) is caused by this accumulating differential secular phase, even though individual [orbital eccentricities](../../../../../orbital-eccentricity.md) remain small. To first order in [orbital eccentricity](../../../../../orbital-eccentricity.md), the radius of an orbit at fixed inertial longitude $\theta$ is

$$
r(a,\theta,t)=a\left[1-\operatorname{Re}(z(a,t)e^{-i\theta})\right]+O(ae^2).
$$

For an infinitesimally neighboring orbit,

$$
\frac{\delta r}{\delta a}\simeq1-\operatorname{Re}\left[(z+a\partial_a z)e^{-i\theta}\right].
$$

This derivative is evaluated within the first-order orbital-shape model; derivatives of the neglected quadratic terms give relative $O(Z_f)$ corrections near crossing. The least separation over longitude is consequently $\delta a[1-|z+a\partial_a z|]$. The [differential secular orbit-crossing criterion](../../../../../differential-secular-orbit-crossing-criterion.md) is $|z+a\partial_a z|=1$. Since $Z_f\propto a$ and $A\propto a^{3/2}$,

$$
z+a\partial_a z=2Z_f(1-e^{iAt})-\frac32iZ_fAt\,e^{iAt}.
$$

The first term stays bounded by $4Z_f\ll1$, whereas the second grows in proportion to time. To leading order in $Z_f$, crossing begins when $(3/2)Z_fAt=1$. Thus

$$
\boxed{t_{\rm cross}\simeq\frac{2}{3Z_fA}
=\frac{32}{45}n_{\rm pl}^{-1}\frac{M_\star}{M_{\rm pl}}e_{\rm pl}^{-1}\left(\frac{a_1}{a_{\rm pl}}\right)^{-5/2}}.
$$

More precisely, in this first-order orbital-shape approximation the exact first crossing lies within a fractional $O(Z_f)$ window of this value, since the magnitude differs from $(3/2)Z_fAt$ by at most $4Z_f$. Higher-order [Laplace coefficients](../../../../../laplace-coefficient.md) give additional corrections. The local derivation takes the neighboring-orbit limit before the long-time limit; for a finite separation it requires $\delta a/a_1\ll Z_f$ near crossing. A broad continuous disk contains such neighboring orbits. The crossings first appear in directions selected by the phase of $z+a\partial_a z$, not simultaneously at every longitude.

For the [collision](../../../../../collision.md) energy estimate adopt the phase-averaged mean [orbital eccentricity](../../../../../orbital-eccentricity.md) $\overline e=4Z_f/\pi\simeq5\alpha e_{\rm pl}/\pi$. The specified velocity estimate gives

$$
v_{\rm col}\sim\overline e\sqrt{\frac{GM_\star}{a_1}},\qquad
v_{\rm col}^2\sim\frac{25}{\pi^2}\alpha e_{\rm pl}^2\frac{GM_\star}{a_{\rm pl}}.
$$

Using the projectile [kinetic energy](../../../../../kinetic-energy.md) per target [mass](../../../../../mass.md) convention for [specific impact energy](../../../../../specific-impact-energy.md), equal-size and equal-density bodies have equal [masses](../../../../../mass.md) and $Q=\tfrac12v_{\rm col}^2$. A [catastrophic planetesimal collision](../../../../../catastrophic-planetesimal-collision.md) requires $Q\gtrsim Q_D^*$, so

$$
\boxed{\frac{a_1}{a_{\rm pl}}\gtrsim\frac{2\pi^2}{25}\frac{Q_D^*a_{\rm pl}}{GM_\star e_{\rm pl}^2}}.
$$

The numerical coefficient is only illustrative because the [collision](../../../../../collision.md) speed was specified only to order of magnitude. If the disruption threshold is instead defined using the [centre of mass](../../../../../center-of-mass.md) [kinetic energy](../../../../../kinetic-energy.md) per combined [mass](../../../../../mass.md), equal [masses](../../../../../mass.md) give $Q_R=v_{\rm col}^2/8$ and the coefficient becomes $8\pi^2/25$ for a threshold expressed in that convention. The robust result is a lower bound of order $Q_D^*a_{\rm pl}/(GM_\star e_{\rm pl}^2)$.

**Within the inner-disk approximation, catastrophic [collisions](../../../../../collision.md) require sufficiently large $a_1/a_{\rm pl}$, not arbitrarily small radii.** Although the Keplerian speed rises inward, the secularly induced [orbital eccentricity](../../../../../orbital-eccentricity.md) falls faster: $v_{\rm col}^2\propto\alpha$. The lower bound must be much smaller than one to leave a domain compatible with $\alpha\ll1$. A small [planet](../../../../../planet.md) [orbital eccentricity](../../../../../orbital-eccentricity.md), a large disruption threshold, or a distant [planet](../../../../../planet.md) can eliminate that domain. The [planet](../../../../../planet.md) [mass](../../../../../mass.md) controls the time to crossing but cancels from the eventual [forced eccentricity](../../../../../forced-eccentricity.md) amplitude and this [collision](../../../../../collision.md)-energy criterion. The threshold alone does not ensure that crossing has occurred within the disk's available lifetime.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
