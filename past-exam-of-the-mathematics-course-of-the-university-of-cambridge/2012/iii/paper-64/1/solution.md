<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $k=p+1$, $\mu=GM_\star$ and $n_{\rm pl}=\sqrt{\mu/a_{\rm pl}^3}$. To leading order the [mean-motion resonance](../../../../../mean-motion-resonance.md) fixes $a=a_{\rm pl}k^{-2/3}$. The [specific angular momentum](../../../../../specific-angular-momentum.md) is

$$
h^2=\mu q(1+e)\simeq2\mu q.
$$

The [asteroid](../../../../../asteroid.md)'s instantaneous [angular speed](../../../../../angular-speed.md) is $h/r^2$. Thus the [high-eccentricity angular-speed crossover](../../../../../high-eccentricity-angular-speed-crossover.md) satisfies $h/r_x^2=n_{\rm pl}$, giving

$$
\boxed{r_x=a_{\rm pl}\left(\frac{2q}{a_{\rm pl}}\right)^{1/4}},\qquad \dot\theta<n_{\rm pl}\quad\hbox{for }r>r_x.
$$

Here $q\ll r_x\ll a$, so a [parabolic Kepler orbit](../../../../../parabolic-trajectory.md) gives the local motion accurately. Its polar equation is $r=2q/(1+\cos f)$. Write $f_x=\pi-\epsilon_x$. Since $1+\cos f_x\simeq\epsilon_x^2/2$,

$$
\boxed{f_x\simeq\pi-2\sqrt{q/r_x}=\pi-2^{7/8}(q/a_{\rm pl})^{3/8}}.
$$

This is the outward crossing; the inward crossing has [true anomaly](../../../../../true-anomaly.md) $-f_x$ modulo $2\pi$.

For the [pericentre-to-crossover flight time](../../../../../pericentre-to-crossover-flight-time.md) use $D=\tan(f/2)$. The [parabolic Kepler orbit](../../../../../parabolic-trajectory.md) has $r=q(1+D^2)$ and $dt=r^2\,df/h$, whence direct integration gives the [Barker equation](../../../../../barker-equation.md)

$$
t(f)-t(0)=\sqrt{\frac{2q^3}{\mu}}\left(D+\frac{D^3}{3}\right).
$$

At the crossover $D_x\simeq\sqrt{r_x/q}\gg1$. Consequently the [planet](../../../../../planet.md)'s angular displacement is

$$
n_{\rm pl}t_x\simeq\frac{\sqrt2}{3}\left(\frac{r_x}{a_{\rm pl}}\right)^{3/2}
=\boxed{\frac{2^{7/8}}3\left(\frac{q}{a_{\rm pl}}\right)^{3/8}}.
$$

The error tends to zero as $q/a_{\rm pl}\to0$ at fixed $k$; it includes the finite binding energy of the elliptic [Kepler orbit](../../../../../kepler-orbit.md) as well as the subleading term in the [Barker equation](../../../../../barker-equation.md).

At the $j$th [pericentre](../../../../../periapsis.md) passage the [asteroid](../../../../../asteroid.md)'s unwrapped [mean longitude](../../../../../mean-longitude.md) is $\lambda=\varpi+2\pi j$. The [resonant argument](../../../../../resonant-argument.md) therefore gives

$$
\lambda_{\rm pl}-\varpi=\frac{\phi+2\pi j}{k}\pmod {2\pi}.
$$

Thus $\phi/k$ specifies the [planet](../../../../../planet.md)'s direction relative to the [asteroid](../../../../../asteroid.md)'s [longitude of pericentre](../../../../../longitude-of-periapsis.md) when the [asteroid](../../../../../asteroid.md) passes [pericentre](../../../../../periapsis.md), with $k$ branches separated by $2\pi/k$. It is not the instantaneous true-longitude separation throughout the orbit. At high [orbital eccentricity](../../../../../orbital-eccentricity.md) the [asteroid](../../../../../asteroid.md) quickly sweeps to a direction nearly opposite [pericentre](../../../../../periapsis.md), while the [planet](../../../../../planet.md) scarcely moves. During the long outer excursion the [asteroid](../../../../../asteroid.md)'s direction changes slowly and the [planet](../../../../../planet.md) advances substantially. This makes an [astronomical conjunction](../../../../../conjunction-astronomy.md) during the outer excursion much more dangerous than an [astronomical conjunction](../../../../../conjunction-astronomy.md) close to [pericentre](../../../../../periapsis.md).

At the following [apocentre](../../../../../apoapsis.md), the [planet](../../../../../planet.md) has advanced $\pi/k$. The [asteroid](../../../../../asteroid.md)'s direction in the [rotating reference frame](../../../../../rotating-reference-frame.md) is consequently

$$
\psi_{{\rm apo},j}=\pi-\frac{\phi+(2j+1)\pi}{k}.
$$

These $k$ [apocentre](../../../../../apoapsis.md) directions are equally spaced. [Phase protection of interior integer resonances](../../../../../phase-protection-of-interior-integer-resonances.md) places the [planet](../../../../../planet.md) in the largest gap between them, rather than at an [apocentre](../../../../../apoapsis.md) direction. For $k=2$, $\phi=\pi$ puts an [apocentre](../../../../../apoapsis.md) toward the [planet](../../../../../planet.md), whereas $\phi=0$ puts the [apocentres](../../../../../apoapsis.md) at $\pm\pi/2$. For $k=3$, $\phi=0$ puts an [apocentre](../../../../../apoapsis.md) toward the [planet](../../../../../planet.md), whereas $\phi=\pi$ puts the [apocentres](../../../../../apoapsis.md) at $\pi/3,\pi,5\pi/3$. Hence the geometrically favored [resonant-argument libration](../../../../../resonant-argument-libration.md) centres in this regime of high [orbital eccentricity](../../../../../orbital-eccentricity.md) are

$$
\boxed{\phi\simeq0\quad(2:1),\qquad \phi\simeq\pi\quad(3:1)}\pmod {2\pi}.
$$

This is an encounter-avoidance argument for likely stability, not a calculation of a resonant [Hamiltonian](../../../../../hamiltonian.md) or a claim that every orbit near either centre is stable at arbitrary [orbital eccentricity](../../../../../orbital-eccentricity.md).

The following rotating-frame drawing uses $a_{\rm pl}=1$, $a=3^{-2/3}$, $q=0.002$ and $\phi=\pi$. It follows three successive [Kepler orbits](../../../../../kepler-orbit.md), which fill one [planet](../../../../../planet.md) [orbital period](../../../../../orbital-period.md) and close the pattern. The blue segment is just the first outward half-orbit. The marked crossover is a maximum of its rotating-frame polar angle, since $d\psi/dt=h/r^2-n_{\rm pl}$ changes from positive to negative there. The [planet](../../../../../planet.md) stays at $(1,0)$; the three [apocentres](../../../../../apoapsis.md) avoid that direction.

<a id="1/image-phase-protected-high-eccentricity-3-1-orbit-in-the-planet-s-rotating-frame"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-64-resonant-orbit.png)

**[Figure 1](#1/image-phase-protected-high-eccentricity-3-1-orbit-in-the-planet-s-rotating-frame). Phase-protected high-eccentricity 3:1 orbit in the planet's rotating frame**.

To estimate [angular-momentum kicks to nearly radial orbits](../../../../../angular-momentum-kicks-to-nearly-radial-orbits.md), note that $q\simeq h^2/(2\mu)$, so an order-one fractional change in $q$ requires $|\Delta h|$ of order $h$. A characteristic distant encounter at radii of order $a_{\rm pl}$ has tangential acceleration of order $GM_{\rm pl}/a_{\rm pl}^2$ and duration of order $n_{\rm pl}^{-1}$. Its [torque](../../../../../torque.md) per unit [asteroid](../../../../../asteroid.md) [mass](../../../../../mass.md) therefore produces

$$
|\delta h|\sim\frac{GM_{\rm pl}}{a_{\rm pl}n_{\rm pl}}
=\frac{M_{\rm pl}}{M_\star}\sqrt{GM_\star a_{\rm pl}}.
$$

With the most favorable coherent signs, the crude encounter count is

$$
\boxed{N_{\rm coherent}\sim\max\left[1,\frac{M_\star}{M_{\rm pl}}\sqrt{\frac{q}{a_{\rm pl}}}\right]}.
$$

Order-one factors depend on $p$ and encounter geometry. Uncorrelated signs instead give a [random walk](../../../../../random-walk.md) count of order $(M_\star/M_{\rm pl})^2q/a_{\rm pl}$ when this is large. A librating phase-protected orbit can suppress the kicks even further.

There is an important limit to calling this a minimum. The question does not specify an encounter [impact parameter](../../../../../impact-parameter.md). For a weak close encounter with [impact parameter](../../../../../impact-parameter.md) $b$ and relative speed $u\sim\sqrt{GM_\star/a_{\rm pl}}$, the [impulse](../../../../../impulse.md) estimate gives $|\delta h|\sim GM_{\rm pl}a_{\rm pl}/(bu)$ and hence $N\sim(M_\star/M_{\rm pl})(b/a_{\rm pl})\sqrt{q/a_{\rm pl}}$, capped below by one. In the 2:1 case the [Kepler orbit](../../../../../kepler-orbit.md) can cross the [planet](../../../../../planet.md)'s orbit, so one suitably close encounter can suffice: there is no impact-parameter-independent large lower bound. For $k\ge3$, $Q\simeq2a_{\rm pl}k^{-2/3}<a_{\rm pl}$ bounds the separation below by $a_{\rm pl}-Q$, and supplies a geometric factor at fixed $k$. The boxed count is the usual orbital-scale, maximally coherent estimate; the assumptions are essential.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
