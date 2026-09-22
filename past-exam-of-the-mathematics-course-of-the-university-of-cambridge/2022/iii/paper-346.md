# Paper 346

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_346.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_346.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 346](paper-346.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For an [adiabatic cosmological perturbation](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions), the baryon and photon fractional density perturbations obey $\delta_b=3\delta_\gamma/4$. Since the pressure of the [photon-baryon fluid](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-fluid) is supplied by the photons,

$$
dP=\frac13d\bar\rho_\gamma,
\qquad
d\bar\rho=d\bar\rho_\gamma+d\bar\rho_b
=\left(1+\frac{3\bar\rho_b}{4\bar\rho_\gamma}\right)d\bar\rho_\gamma.
$$

The [photon-baryon sound speed](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-sound-speed) is therefore

$$
\boxed{c_s=c\sqrt{\frac{dP}{d\bar\rho}}
=\frac c{\sqrt3}\left(1+\frac{3\bar\rho_b}{4\bar\rho_\gamma}\right)^{-1/2}.}
$$

Use $\bar\rho_b\propto a^{-3}$ and $\bar\rho_\gamma\propto a^{-4}$ in the [comoving Jeans length](../../../linear-cosmological-density-perturbation.md#comoving-jeans-length)

$$
\lambda_{J,{\rm com}}=\frac{c_s}{a}\sqrt{\frac\pi{G\bar\rho_b}}.
$$

Well before [matter-radiation equality](../../../cosmology.md#matter-radiation-equality), photon inertia dominates, $c_s\simeq c/\sqrt3$, and

$$
\lambda_{J,{\rm com}}\propto a^{1/2}\propto t^{1/4}.
$$

Once baryon loading dominates while [tight coupling](../../../cosmic-microwave-background-anisotropy.md#tight-coupling-approximation) still holds, $c_s\propto a^{-1/2}$, so $\lambda_{J,{\rm com}}$ is approximately constant. At [cosmological recombination](../../../cosmology.md#recombination-cosmology), photon pressure support disappears and the baryonic Jeans scale drops sharply. For a subsequently adiabatic monatomic gas, $T_b\propto a^{-2}$ and $c_s\propto a^{-1}$, giving

$$
\lambda_{J,{\rm com}}\propto a^{-1/2}\propto t^{-1/3}
$$

in an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe). The requested graph therefore rises as $t^{1/4}$, flattens before recombination, jumps downward there, and then decreases as $t^{-1/3}$.

For collisionless matter, the same instantaneous estimate uses its one-dimensional [velocity dispersion](../../../galaxy.md#velocity-dispersion) $\sigma_v$ instead of $c_s$; more precisely, suppression is described by [collisionless free streaming](../../../linear-cosmological-density-perturbation.md#free-streaming). Thus

$$
\lambda_{J,{\rm com}}\sim\frac{\sigma_v}{a}\sqrt{\frac\pi{G\bar\rho_{\rm cdm}}}.
$$

While the particles are relativistic, $\sigma_v\simeq c$ and $\lambda_{J,{\rm com}}\propto a^{1/2}$. Once nonrelativistic but thermally coupled to radiation, $T_{\rm cdm}\propto a^{-1}$, so $\sigma_v\propto a^{-1/2}$ and the scale is constant. After kinetic decoupling, momentum redshifts as $a^{-1}$, so $\sigma_v\propto a^{-1}$ and $\lambda_{J,{\rm com}}\propto a^{-1/2}$. The second graph joins these three power laws at $t_{\rm NR}$ and $t_{\rm dec}$; unlike the baryonic graph, its final decline begins at dark-matter kinetic decoupling rather than recombination.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The shell feels only radial gravity and the radial force due to the [cosmological constant](../../../cosmology.md#cosmological-constant), so its torque vanishes and its [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum) $L=r^2\dot\theta$ is conserved. Multiplying

$$
\ddot r=\frac{L^2}{r^3}-\frac{GM}{r^2}+\frac\Lambda3r
$$

by $\dot r$ and integrating gives the conserved [specific orbital energy](../../../classical-mechanics.md#specific-orbital-energy)

$$
\boxed{E=\frac12\dot r^2+\frac{L^2}{2r^2}-\frac{GM}{r}-\frac\Lambda6r^2.}
$$

For a uniform sphere, assembling concentric shells gives its gravitational [potential energy](../../../classical-mechanics.md#potential-energy)

$$
W_{G,{\rm ta}}=-\int_0^{r_{\rm ta}}\frac{GM(r)}r\,dM
=-\frac{3GM^2}{5r_{\rm ta}}.
$$

The cosmological-constant potential per unit mass is $-\Lambda r^2/6$. Since $\langle r^2\rangle=3r_{\rm ta}^2/5$ in a uniform sphere,

$$
W_{\Lambda,{\rm ta}}=-\frac\Lambda6M\langle r^2\rangle
=-\frac1{10}\Lambda Mr_{\rm ta}^2.
$$

The scalar [virial theorem](../../../classical-mechanics.md#virial-theorem) weights a potential homogeneous of degree $n$ by $-nW$. Gravity has degree $-1$ and the $\Lambda$ potential degree $2$, so the final state obeys

$$
\boxed{2T_f+W_{G,f}=2W_{\Lambda,f}.}
$$

At turnaround $T=0$, while the virial relation gives $E_f=W_{G,f}/2+2W_{\Lambda,f}$. Conservation of energy, together with $M=4\pi\rho_{\rm ta}r_{\rm ta}^3/3$, then gives, for $x=r_f/r_{\rm ta}$ and $\eta=\Lambda/(4\pi G\rho_{\rm ta})$,

$$
\boxed{2\eta x^3-(2+\eta)x+1=0.}
$$

The root connected continuously to the $\Lambda=0$ solution has $x=1/2-\eta/8+O(\eta^2)$, equivalently

$$
\boxed{\frac{r_f}{r_{\rm ta}}\simeq
\frac{1-\eta/2}{2-\eta/2}}
$$

to first order in $\eta$. With $\Lambda=0$, virialization occurs at half the [turnaround radius](../../../large-scale-structure-of-the-universe.md#turnaround-radius). At fixed turnaround state, positive $\Lambda$ makes this equilibrium root slightly smaller because its repulsive quadratic potential enters both energy conservation and the virial relation; sufficiently strong repulsion instead prevents a bound virialized state. Negative $\Lambda$ shifts the root in the opposite direction.

## 2

↑ **Parent:** [Paper 346](paper-346.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The two halo centres orbit their [centre of mass](../../../classical-mechanics.md#center-of-mass) with separation $R$. Their relative coordinate obeys $\ddot{\mathbf R}=-G(M_1+M_2)\mathbf R/R^3$, hence circular motion requires

$$
\boxed{\omega^2=\frac{G(M_1+M_2)}{R^3}.}
$$

Reflection symmetry about the orbital plane makes the vertical force point back toward $z=0$, while the centrifugal force has no vertical component. An equilibrium away from that plane is therefore impossible.

In the uniformly rotating frame, an equilibrium is a stationary point of the gravitational plus centrifugal [effective potential](../../../physics.md#effective-potential)

$$
E(x,y)=-\frac{\omega^2}{2}|\mathbf r_S|^2
-\frac{GM_1}{|\mathbf r_S-\mathbf r_1|}
-\frac{GM_2}{|\mathbf r_S-\mathbf r_2|}.
$$

Set $R=1$, divide by $G(M_1+M_2)/R$, and write $\alpha=M_2/(M_1+M_2)$. The primary and secondary lie at $x=-\alpha$ and $x=1-\alpha$, so on their line

$$
F(x)=-\frac{x^2}{2}-\frac{1-\alpha}{|x+\alpha|}
-\frac\alpha{|x+\alpha-1|}.
$$

For the two roots near the secondary, put $x=1-\alpha\mp d$ in $F'(x)=0$. Dominant balance gives $3d\simeq\alpha/d^2$, so $d=(\alpha/3)^{1/3}$. Expanding the root beyond the primary directly in powers of $\alpha$ gives

$$
\boxed{L_1=(1-(\alpha/3)^{1/3},0,0),}
$$



$$
\boxed{L_2=(1+(\alpha/3)^{1/3},0,0),}
$$



$$
\boxed{L_3=(-1-5\alpha/12,0,0),}
$$

to the requested orders. The other equilibria are the two [Triangular Lagrange points](../../../classical-mechanics.md#triangular-lagrange-point)

$$
\boxed{L_{4,5}=(1/2-\alpha,\ \pm\sqrt3/2,\ 0).}
$$

The distance from $H_2$ to either nearby collinear point is the [Hill radius](../../../classical-mechanics.md#hill-radius). Since $\alpha\simeq M_2/M_1$,

$$
\boxed{r_t=R\left(\frac{M_2}{3M_1}\right)^{1/3}.}
$$

Inside this [tidal radius](../../../galaxy.md#tidal-radius), the subhalo's gravity dominates the host's differential gravitational field; outside it, material can escape through the neighborhoods of $L_1$ and $L_2$. For an extended spherical host, $M_1$ is replaced by enclosed mass and the coefficient becomes $3-d\log M_1/d\log R$, giving the [Jacobi tidal radius](../../../galaxy.md#jacobi-tidal-radius). An extended subhalo requires the bound mass inside $r_t$ to be found self-consistently. On an eccentric orbit there is no time-independent rotating potential or exact tidal boundary; stripping is strongest near pericentre and the instantaneous radius varies around the orbit.

Because the dark component is more extended, [tidal stripping](../../../galaxy.md#tidal-stripping) first sends dark matter through both $L_1$ and $L_2$, producing leading and trailing dark-matter [tidal tails](../../../galaxy.md#tidal-tail). The compact stellar component is stripped more deeply and also produces a leading and a trailing stellar tail. The two constituents therefore give four tails distinguished by composition, with the dark tails broader and more extended.

## 3

↑ **Parent:** [Paper 346](paper-346.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The definition of the [virial radius of a dark-matter halo](../../../large-scale-structure-of-the-universe.md#virial-radius-of-a-dark-matter-halo) immediately gives the [virial mass of a dark-matter halo](../../../large-scale-structure-of-the-universe.md#virial-mass-of-a-dark-matter-halo)

$$
\boxed{M_v=\frac{4\pi}{3}v\rho_c^0r_v^3.}
$$

In an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), spherical collapse gives $v=18\pi^2\simeq178$, conventionally rounded to about $200$.

For the [Navarro--Frenk--White profile](../../../large-scale-structure-of-the-universe.md#navarro-frenk-white-profile), put $x=r/r_s=cs$. Direct integration gives

$$
M(r)=4\pi\rho_c^0\delta_{\rm char}r_s^3
\left[\log(1+x)-\frac{x}{1+x}\right].
$$

Using $r_s=r_v/c$ and $\delta_{\rm char}=vc^3g(c)/3$ therefore yields

$$
\boxed{\frac{M(s)}{M_v}=g(c)
\left[\log(1+cs)-\frac{cs}{1+cs}\right].}
$$

At small radius the bracket is $(cs)^2/2+O((cs)^3)$, so $M(r)\propto r^2$, consistent with the central $\rho\propto r^{-1}$ cusp. At large radius it is $\log(cs)-1+o(1)$, so the mass diverges logarithmically unless the halo is truncated.

The primordial free streaming of [warm dark matter](../../../cosmology.md#warm-dark-matter) erases small-scale density fluctuations and lowers the central phase-space density, tending to replace the smallest, earliest cold-dark-matter cusps by shallower central profiles or cores.

Since $V_v^2=GM_v/r_v$, the spherical potential that vanishes at infinity is

$$
\Phi(s)=-g(c)V_v^2\frac{\log(1+cs)}s.
$$

Indeed, $r\,d\Phi/dr=GM(r)/r$, and normalization at $s=1$ requires

$$
\boxed{g(c)=\left[\log(1+c)-\frac{c}{1+c}\right]^{-1}.}
$$

The [circular speed](../../../galaxy.md#circular-speed) is consequently

$$
\boxed{V^2(s)=V_v^2\frac{g(c)}s
\left[\log(1+cs)-\frac{cs}{1+cs}\right].}
$$

It rises as $s^{1/2}$ near the centre, peaks at $r\simeq2.16r_s$, and then declines approximately as $\sqrt{\log r/r}$. Increasing the [concentration of a dark-matter halo](../../../large-scale-structure-of-the-universe.md#concentration-of-a-dark-matter-halo) moves the peak inward in units of $r_v$ and raises it relative to $V_v$. Thus an NFW curve can be fairly broad but is not exactly a [flat galaxy rotation curve](../../../galaxy.md#flat-galaxy-rotation-curve); stellar and gas contributions matter when comparing with an observed [galaxy rotation curve](../../../galaxy.md#galaxy-rotation-curve).

Lower-mass haloes typically collapse earlier, when the cosmic background density is larger. Their characteristic inner densities are consequently larger relative to the present virial density, producing the [mass-concentration relation of dark-matter haloes](../../../large-scale-structure-of-the-universe.md#mass-concentration-relation-of-dark-matter-haloes) in which concentration decreases weakly with mass.

For a mass smaller by $1024=2^{10}$,

$$
M_v\simeq9.8\times10^8M_\odot,
\qquad
r_v=200\,1024^{-1/3}\ {\rm kpc}\simeq19.8\ {\rm kpc},
$$

and $c=10\,1024^{0.1}=20$. Hence

$$
\boxed{r_s=r_v/c\simeq0.99\ {\rm kpc}.}
$$

A halo of roughly $10^9M_\odot$ and kiloparsec scale naturally hosts a [dwarf galaxy](../../../galaxy.md#dwarf-galaxy), possibly an extremely faint one if star formation is inefficient.

## 4

↑ **Parent:** [Paper 346](paper-346.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write proper position as $\mathbf r=a(t)\mathbf x$ and proper velocity as

$$
\mathbf u=\dot{\mathbf r}=H\mathbf r+\mathbf v,
\qquad
\mathbf v=a\dot{\mathbf x}.
$$

Substitute this decomposition into the proper-coordinate [Euler equations for an inviscid fluid](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid), use $\nabla_r=a^{-1}\nabla_x$, and subtract the homogeneous-background acceleration. With $\rho=\bar\rho(1+\delta)$, one obtains the comoving [peculiar-velocity equation](../../../cosmology.md#peculiar-velocity-equation)

$$
\boxed{\frac{\partial\mathbf v}{\partial t}+\frac{\dot a}{a}\mathbf v
+\frac1a(\mathbf v\mathbin\cdot\nabla)\mathbf v
=-\frac1a\nabla\Phi
-\frac1{a\bar\rho(1+\delta)}\nabla P.}
$$

The [peculiar gravitational potential](../../../linear-cosmological-density-perturbation.md#peculiar-gravitational-potential) $\Phi$ is the total Newtonian potential with the potential of the exactly homogeneous expanding background subtracted. Its gradient therefore generates only accelerations relative to the [Hubble flow](../../../cosmology.md#hubble-flow).

For a pressureless fluid, [linearization](../../../algebra.md#linearization) discards the quadratic advection term, leaving

$$
\dot{\mathbf v}+H\mathbf v=-\frac1a\nabla\Phi,
\qquad
\boxed{\frac d{dt}(a\mathbf v)=-\nabla\Phi.}
$$

In the early [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), the growing mode has $\Phi(\mathbf x,t)=[D(a)/a]\Phi_i(\mathbf x)$. Integration gives

$$
\boxed{\mathbf v=-\frac{\nabla\Phi_i}{a}\int^t\frac{D(a)}a\,dt.}
$$

The [linear growth factor](../../../linear-cosmological-density-perturbation.md#linear-growth-factor) obeys

$$
\ddot D+2H\dot D=4\pi G\bar\rho D.
$$

Since $\bar\rho=\bar\rho_i/a^3$ after choosing $a_i=1$, this is equivalent to

$$
\boxed{\frac{D(a)}a=\frac1{4\pi G\bar\rho_i}
\frac d{dt}\left(a^2\frac{dD}{dt}\right).}
$$

It follows that $a\mathbf v=-a^2\dot D\nabla\Phi_i/(4\pi G\bar\rho_i)$. Since $\dot{\mathbf x}=\mathbf v/a$, one final integration gives the [Zeldovich approximation](../../../large-scale-structure-of-the-universe.md#zeldovich-approximation)

$$
\boxed{\mathbf x(t)\simeq\mathbf x_i
-\frac{D(a)}{4\pi G\bar\rho_i}\nabla\Phi_i,}
$$

where an additive initial displacement has been absorbed into $\mathbf x_i$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
