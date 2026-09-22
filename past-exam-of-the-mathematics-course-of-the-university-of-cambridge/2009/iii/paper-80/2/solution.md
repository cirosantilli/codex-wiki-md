<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the steady axisymmetric [top-hat plume model](../../../../../top-hat-plume-model.md), with plume radius $b(z)$, uniform mean upward speed $w(z)>0$ and [reduced gravity](../../../../../reduced-gravity-split.md) $g'(z)=g[\rho_a(z)-\rho_p(z)]/\rho_0$. The [Boussinesq approximation](../../../../../boussinesq-approximation.md) uses constant reference density $\rho_0$ in inertia and retains the small density difference only in [buoyancy](../../../../../buoyancy.md). Assume a quiescent hydrostatic ambient, a slender fully [turbulent plume](../../../../../turbulent-plume-split.md), negligible molecular transport and an [entrainment](../../../../../fluid-entrainment.md) [velocity](../../../../../velocity.md) $\alpha w$, with constant positive [entrainment coefficient](../../../../../entrainment-coefficient.md) $\alpha$. Define the ambient [buoyancy frequency](../../../../../buoyancy-frequency.md) by $N^2=-(g/\rho_0)d\rho_a/dz$; positive $N^2$ is stable stratification.

The integrated volume, momentum and [buoyancy](../../../../../buoyancy.md) balances of a [Boussinesq top-hat plume in a stratified ambient](../../../../../boussinesq-top-hat-plume-in-a-stratified-ambient.md) are

$$
\boxed{\frac d{dz}(b^2w)=2\alpha bw,\qquad
\frac d{dz}(b^2w^2)=b^2g',\qquad
\frac d{dz}(b^2wg')=-N^2b^2w.}
$$

The first follows from side [entrainment](../../../../../fluid-entrainment.md), the second from the integrated [buoyancy](../../../../../buoyancy.md) force, and the third accounts for the changing ambient density. Common factors of $\pi$ are cancelled. Equivalently, the requested radius, speed and reduced-gravity equations are

$$
\boxed{b'=2\alpha-\frac{bg'}{2w^2},\qquad
w'=\frac{g'}w-\frac{2\alpha w}b,\qquad
(g')'=-N^2-\frac{2\alpha g'}b.}
$$

These equations stop describing an upward light plume once $w$ vanishes, and their light-plume interpretation requires $g'>0$.

For nonzero $C$, seek [plume similarity in power-law stratification](../../../../../plume-similarity-in-power-law-stratification.md) in the form $b=\beta z$, $w=Az^n$ and $g'=Gz^m$. The first balance gives $\beta=2\alpha/(n+2)$. Momentum gives $m=2n-1$ and $G=2(n+1)A^2$. The [buoyancy](../../../../../buoyancy.md) balance then requires $3n=2+n+p$, so

$$
n=\frac{p+2}{2},\quad m=p+1,\quad
\beta=\frac{4\alpha}{p+6},\quad G=-\frac{2C}{3p+8},\quad
A^2=-\frac{2C}{(p+4)(3p+8)}.
$$

Choosing $A>0$ gives the exact power-law family, including its normalization:

$$
\boxed{b=\frac{4\alpha}{p+6}z,\qquad
w=\left[\frac{-2C}{(p+4)(3p+8)}\right]^{1/2}z^{(p+2)/2},\qquad
g'=-\frac{2C}{3p+8}z^{p+1}.}
$$

These are the [amplitudes and physical branches of a power-law stratified plume](../../../../../amplitudes-and-physical-branches-of-a-power-law-stratified-plume.md). No source flux was specified, so an arbitrary finite-source solution is not determined by $C,p$ alone; the displayed family is an exact similarity solution, rather than the general solution for arbitrary initial fluxes.

With the specific flux convention $Q=b^2w$, $M=b^2w^2$ and $B=b^2wg'$, their values are

$$
\boxed{Q=\beta^2A z^{3+p/2},\qquad
M=\beta^2A^2z^{4+p},\qquad
B=\beta^2AGz^{4+3p/2}.}
$$

The physical [volume flux](../../../../../volumetric-flow-rate.md) is $\pi Q$, mass flux is $\rho_0\pi Q$, [momentum flux](../../../../../momentum-flux.md) is $\rho_0\pi M$, and kinematic [buoyancy flux](../../../../../buoyancy-flux.md) is $\pi B$. Thus the “specific mass flux” is the mass flux divided by reference density, with or without the explicitly stated factor $\pi$.

The parameter restrictions follow directly from positivity. Positive radius needs $p>-6$. Positive $g'$ and real positive $w$ further require $p>-4$ and $-C/(3p+8)>0$, giving

$$
\boxed{C>0:\ -4<p<-8/3;\qquad C<0:\ p>-8/3.}
$$

For stable $C>0$, [buoyancy flux](../../../../../buoyancy-flux.md) decreases with height, while volume and momentum fluxes increase. However, $B\propto z^{4+3p/2}$ diverges at $z=0$ throughout this interval. Also the ambient density gradient and plume speed are singular there. Thus this stable similarity branch can describe a region away from a virtual source, but cannot represent a finite-buoyancy-flux point source extending all the way to $z=0$. For ordinary regular stable stratifications, including positive $p$, a finite-source rising plume instead loses [buoyancy](../../../../../buoyancy.md) and eventually reaches neutral [buoyancy](../../../../../buoyancy.md) and a finite rise limit; the pure-power ansatz does not supply such a solution.

For unstable $C<0$ and $p>-8/3$, the [buoyancy flux](../../../../../buoyancy-flux.md) grows with height and tends to zero at the origin. The plume draws its increasing [buoyancy](../../../../../buoyancy.md) from an unstable ambient rather than a finite positive source [buoyancy flux](../../../../../buoyancy-flux.md). Such an ambient must be maintained or treated locally, since it is itself convectively unstable. If $p\leq-1$, its density profile is singular at the source, while for $p>-1$ its increasing density contrast eventually violates the [Boussinesq approximation](../../../../../boussinesq-approximation.md) at sufficiently large height. These are formal local similarity solutions with corresponding physical limits. For $C<0$ and $-6<p<-4$, the algebra also gives a real positive speed but negative $g'$: this is a heavy upward flow, not the specified light plume.

At nonzero $C$, the values $p=-6,-4,-8/3$ do not give finite coefficients. Respectively they would require zero entrained volume-flux growth, zero momentum-flux growth despite nonzero [buoyancy](../../../../../buoyancy.md), or constant [buoyancy flux](../../../../../buoyancy-flux.md) despite nonzero ambient stratification. They are not omitted regular endpoints.

When $C=0$, the ambient is unstratified regardless of the nominal value of $p$. The nontrivial positive-buoyancy point-source solution is the [Boussinesq point-source plume](../../../../../boussinesq-point-source-plume.md):

$$
\boxed{b=\frac{6\alpha}{5}z,\qquad
w=A_0z^{-1/3},\qquad
g'=\frac43A_0^2z^{-5/3},\qquad
A_0^3=\frac{25B_0}{48\alpha^2}.}
$$

Here $B_0>0$ is the constant specific [buoyancy flux](../../../../../buoyancy-flux.md) with $\pi$ removed. Its $Q\propto z^{5/3}$ and $M\propto z^{4/3}$ vanish at the point source, while $B=B_0$. Its near-source singularity is the usual ideal point-source limit; a finite vent replaces that limit by finite source data or a virtual origin.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
