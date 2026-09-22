<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The central equation must be read as $\ddot{\mathbf r}=-\mu\mathbf r/r^3$; its printed left-hand expression lacks $=0$. Initially $\mu$ is constant. Dotting this equation with the velocity gives

$$
\frac{d}{dt}\left(\frac{v^2}{2}-\frac{\mu}{r}\right)=0.
$$

Taking its cross product with $\mathbf r$ gives $d(\mathbf r\times\mathbf v)/dt=0$. In the fixed orbital plane the magnitude is $h=r^2\dot\theta$. These are conservation of [specific orbital energy](../../../../../specific-orbital-energy.md) and [specific angular momentum](../../../../../specific-angular-momentum.md).

Let $f=\theta-\varpi$. Differentiating the polar equation of the [Kepler orbit](../../../../../kepler-orbit.md), with its elements initially constant, gives

$$
\dot r=\frac{\mu}{h}e\sin f,\qquad r\dot\theta=\frac{\mu}{h}(1+e\cos f).
$$

Substitution into the [specific orbital energy](../../../../../specific-orbital-energy.md) yields

$$
C=\frac{\mu^2}{2h^2}\left[e^2\sin^2f+(1+e\cos f)^2-2(1+e\cos f)\right]
=\boxed{\frac{\mu^2}{2h^2}(e^2-1)}.
$$

For [isotropic stellar mass loss](../../../../../isotropic-stellar-mass-loss.md) with no recoil or drag, the force is still central, so $\mathbf h$ remains exactly constant, although $C$ does not. Now

$$
\dot C=-\frac{\dot\mu}{r}.
$$

The same algebraic relation between $C,h,e$ holds for the instantaneous [osculating orbital elements](../../../../../osculating-orbital-element.md). Differentiating it and using $h^2/(\mu r)=1+e\cos f$ gives

$$
e\dot e=\frac{h^2}{\mu^2}\dot C-\frac{2Ch^2}{\mu^3}\dot\mu
=-\frac{\dot\mu}{\mu}e(e+\cos f),
$$

and, for $e>0$,

$$
\boxed{\dot e=-\frac{\dot\mu}{\mu}(e+\cos f)}.
$$

A particularly useful nonsingular description uses the [eccentricity vector](../../../../../eccentricity-vector.md)

$$
\mathbf e=\frac{\mathbf v\times\mathbf h}{\mu}-\widehat{\mathbf r},\qquad
\boxed{\dot{\mathbf e}=-\frac{\dot\mu}{\mu}(\mathbf e+\widehat{\mathbf r})}.
$$

The vector equation remains meaningful at a circular orbit, where a [longitude of pericentre](../../../../../longitude-of-periapsis.md) is undefined. Its components along and perpendicular to $\mathbf e$ give the scalar formula above and

$$
\boxed{\dot\varpi=-\frac{\dot\mu}{\mu}\frac{\sin f}{e}}.
$$

The osculating [pericentre](../../../../../periapsis.md) is $q=h^2/[\mu(1+e)]$. Therefore

$$
\boxed{\frac{\dot q}{q}=-\frac{\dot\mu}{\mu}\frac{1-\cos f}{1+e}}.
$$

For [mass](../../../../../mass.md) loss, $\dot\mu<0$, this is nonnegative: [pericentre](../../../../../periapsis.md) does not decrease. It is positive except at [pericentre](../../../../../periapsis.md) itself, where $\cos f=1$ and $\dot q=0$. Thus a strictly opposite sign at every instant is not literally true; a [pericentre](../../../../../periapsis.md) passage with nonzero [mass](../../../../../mass.md)-loss rate is a counterexample to the strict wording. The intended monotonicity follows exactly, without requiring slow [mass](../../../../../mass.md) loss.

For [adiabatic orbital expansion under isotropic mass loss](../../../../../adiabatic-orbital-expansion-under-isotropic-mass-loss.md), average over the unperturbed [Kepler orbit](../../../../../kepler-orbit.md) and hold $\dot\mu/\mu$ constant to leading order during that orbit. If $E$ is the [eccentric anomaly](../../../../../eccentric-anomaly.md) and $n=\sqrt{\mu/a^3}$, then

$$
\cos f=\frac{\cos E-e}{1-e\cos E},\qquad dt=\frac{1-e\cos E}{n}\,dE,\qquad P=\frac{2\pi}{n}.
$$

It follows immediately that

$$
\langle\cos f\rangle=\frac1{2\pi}\int_0^{2\pi}(\cos E-e)\,dE=-e,
\qquad \boxed{\langle\dot e\rangle=0}.
$$

Averaging with uniform [true anomaly](../../../../../true-anomaly.md) instead of uniform time would give the wrong result. Since $\mu a(1-e^2)=h^2$, conserved $h$ and constant secular [orbital eccentricity](../../../../../orbital-eccentricity.md) give

$$
\boxed{\mu a=\text{constant},\qquad a\propto\mu^{-1}}.
$$

The [pericentre](../../../../../periapsis.md) and [apocentre](../../../../../apoapsis.md) expand in the same secular proportion. These are leading [adiabatic invariants](../../../../../adiabatic-invariant.md), rather than exact invariants for arbitrary time-dependent $\mu$.

For the instantaneous precession fraction write $\theta=f+\varpi$ and $\dot\theta=h/r^2$. The [adiabatic apsidal condition](../../../../../adiabatic-apsidal-condition.md) is controlled by

$$
\boxed{\frac{\dot\varpi}{\dot\theta}
=-\frac{\dot\mu}{\mu}\frac{r^2}{he}\sin f
=-\frac{\dot\mu}{\mu n}\frac{(1-e^2)^{3/2}\sin f}{e(1+e\cos f)^2}}.
$$

It is a signed fraction: apsidal advance contributes positively on the outward leg during [mass](../../../../../mass.md) loss, and negatively on the inward leg. Let $\tau_\mu=|\mu/\dot\mu|$. Ordinary [orbit averaging](../../../../../orbit-averaging.md) requires $\tau_\mu\gg P$, together with negligible variation of the [mass](../../../../../mass.md)-loss law over one orbit. If the [pericentre](../../../../../periapsis.md) direction is also to vary negligibly relative to the instantaneous azimuthal motion, the maximum absolute fraction must be small. A precise condition for $0<e<1$ is

$$
n\tau_\mu\gg F(e),\qquad F(e)=\frac{(1-e^2)^{3/2}}e\max_f\frac{|\sin f|}{(1+e\cos f)^2}.
$$

The maximizing cosine is $c=(1-\sqrt{1+8e^2})/(2e)$: differentiating the last factor gives $c+2e-ec^2=0$. Thus one can evaluate $F(e)$ explicitly by putting $\sqrt{1-c^2}/(1+ec)^2$ into the formula. Its useful limits are

$$
F(e)\sim e^{-1}\quad(e\to0),\qquad F(e)\to\frac{3\sqrt3}{4}\quad(e\to1).
$$

**For [orbital eccentricity](../../../../../orbital-eccentricity.md) of order unity, [mass](../../../../../mass.md) loss much slower than an [orbital period](../../../../../orbital-period.md) suffices; near a circular orbit, keeping the [pericentre](../../../../../periapsis.md) direction slowly varying additionally requires $n\tau_\mu e\gg1$.** The latter divergence is a singularity of the [pericentre](../../../../../periapsis.md) coordinate, not a divergence of the [eccentricity vector](../../../../../eccentricity-vector.md) dynamics. Indeed, at frozen $\dot\mu/\mu$, integrating the scalar evolution to first order gives $\delta e=-(\dot\mu/\mu)(1-e^2)\sin E/n$ up to an integration constant. Its absolute amplitude stays small for slow [mass](../../../../../mass.md) loss even when the scalar [longitude of pericentre](../../../../../longitude-of-periapsis.md) becomes unsuitable.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
