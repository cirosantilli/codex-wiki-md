# Paper 62

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper62.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper62.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use [metric signature](../../../topology.md#metric-signature) $(-,+,+,+)$ and units $c=1$. Write $\dot x^\mu=dx^\mu/d\lambda$ in this part. Varying the [worldline einbein](../../../classical-mechanics.md#worldline-einbein), without first fixing it, gives

$$
0=\frac{\partial L}{\partial e}=\frac m2\left(-\frac{g_{\mu\nu}\dot x^\mu\dot x^\nu}{e^2}-1\right),\qquad \boxed{g_{\mu\nu}\dot x^\mu\dot x^\nu=-e^2.}
$$

The canonical four-momentum is $p_\mu=mg_{\mu\nu}\dot x^\nu/e$, so the same [mass shell](../../../special-relativity.md#mass-shell) constraint is the [mass shell](../../../special-relativity.md#mass-shell) $g^{\mu\nu}p_\mu p_\nu=-m^2$.

The [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) for the trajectory is

$$
\frac{d}{d\lambda}\left(\frac{g_{\mu\nu}\dot x^\nu}{e}\right)-\frac1{2e}\partial_\mu g_{\alpha\beta}\dot x^\alpha\dot x^\beta=0.
$$

Multiplying by $e$ and then by the [inverse metric](../../../general-relativity.md#inverse-metric), and collecting the [metric tensor](../../../general-relativity.md#metric-tensor) derivatives into the [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol), gives

$$
\boxed{\ddot x^\mu+\Gamma^\mu_{\alpha\beta}\dot x^\alpha\dot x^\beta=\frac{\dot e}{e}\dot x^\mu.}
$$

This is a [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) in a possibly nonaffine parameter.

Under a change of parameter, $e'(\lambda')=e(\lambda)d\lambda/d\lambda'$, so $e\,d\lambda$ is invariant. On the positive branch, the [mass shell](../../../special-relativity.md#mass-shell) constraint identifies this invariant with the [proper time](../../../special-relativity.md#proper-time) increment $ds=\sqrt{-g_{\mu\nu}dx^\mu dx^\nu}=e\,d\lambda$. Choosing $\lambda'=s$ therefore sets $e'=1$. The trajectory equation is then the affinely parametrized [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) and its tangent has norm minus one. This is [proper-time gauge for a massive worldline einbein](../../../classical-mechanics.md#proper-time-gauge-for-a-massive-worldline-einbein). The [mass shell](../../../special-relativity.md#mass-shell) constraint must still be imposed: fixing $e$ in the action before varying would lose it. A fixed parameter interval can retain a [proper-time modulus](../../../classical-mechanics.md#proper-time-modulus); here changing to the actual proper-time interval is permitted.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In proper-time gauge the particle [Lagrangian](../../../calculus-of-variations.md#lagrangian) is $L=m(-\dot t^2+a^2\dot{\mathbf x}^{\,2}-1)/2$, now with dots referring to [proper time](../../../special-relativity.md#proper-time) $s$. The canonical spatial [momentum](../../../classical-mechanics.md#momentum) is

$$
\boxed{p_i^C=\frac{\partial L}{\partial\dot x^i}=ma^2\delta_{ij}\frac{dx^j}{ds}.}
$$

The [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) is independent of all spatial coordinates. Hence $\partial L/\partial x^i=0$ and the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) gives $dp_i^C/ds=0$. This [conserved quantity](../../../classical-mechanics.md#conserved-quantity) is the [comoving momentum](../../../linear-cosmological-density-perturbation.md#comoving-momentum).

The mass-shell [mass shell](../../../special-relativity.md#mass-shell) constraint gives $(dt/ds)^2-a^2|d\mathbf x/ds|^2=1$. For future-directed motion and proper [peculiar velocity](../../../cosmology.md#peculiar-velocity) $\mathbf v=a\,d\mathbf x/dt$, it follows that $dt/ds=(1-v^2)^{-1/2}=\gamma$. Therefore

$$
\mathbf p^C=ma^2\gamma\frac{d\mathbf x}{dt}=a\gamma m\mathbf v=a\mathbf p^K,
\qquad \boxed{\mathbf p^K=\frac{\mathbf p^C}{a}.}
$$

The kinetic [momentum](../../../classical-mechanics.md#momentum) here is the [physical momentum in an FRW universe](../../../linear-cosmological-density-perturbation.md#physical-momentum-in-an-frw-universe), measured in the [orthonormal frame](../../../general-relativity.md#orthonormal-frame-in-spacetime) of a [comoving observer](../../../cosmology.md#comoving-observer). It [redshifts](../../../optics.md#redshift) as $a^{-1}$ irrespective of whether the particle is relativistic or nonrelativistic.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [mass shell](../../../special-relativity.md#mass-shell) constraint and the conserved [comoving momentum](../../../linear-cosmological-density-perturbation.md#comoving-momentum) give

$$
\frac{dt}{ds}=\sqrt{1+\frac{(p^C)^2}{m^2a^2}},\qquad \frac{d\mathbf x}{ds}=\frac{\mathbf p^C}{ma^2}.
$$

Dividing yields

$$
\boxed{\frac{d\mathbf x}{dt}=\frac{\mathbf p^C}{a\sqrt{(p^C)^2+m^2a^2}}.}
$$

The comoving direction is constant because $\mathbf p^C$ is constant. With $a(t_0)=1$ and physical [momentum](../../../classical-mechanics.md#momentum) magnitude $p_0>0$ at $t_0$, we have $p^C=p_0$. Integrating the speed along that fixed direction gives

$$
\boxed{d=\int_0^{t_0}\frac{dt}{a(t)}\frac1{\sqrt{1+[ma(t)/p_0]^2}}.}
$$

This is a distance travelled, rather than a light-ray distance: the extra factor is the particle's proper peculiar speed $v=p^K/\sqrt{m^2+(p^K)^2}$. For a particle at rest, $p_0=0$, the distance is zero, understood separately or as the limit. The formula assumes collisionless motion over the interval. Its existence at the lower endpoint depends on the early [scale factor](../../../cosmology.md#scale-factor-cosmology); in [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination) the integral is finite.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Let $t_*$ be the observation time and normalize $a(t_*)=1$ temporarily. In pure [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), $a(t)=(t/t_*)^{1/2}$ and $H_*=1/(2t_*)$. With $p(t)=T_r(t)=T_*/a(t)$, the proper speed is $v=[1+(ma/T_*)^2]^{-1/2}$. Put $u=\sqrt{t/t_*}=a(t)$ in the preceding integral. Since $dt=2t_*u\,du$,

$$
d=2t_*\int_0^1\frac{du}{\sqrt{1+(mu/T_*)^2}}=\boxed{H_*^{-1}\frac{T_*}{m}\operatorname{arsinh}\!\left(\frac m{T_*}\right).}
$$

The small-$m/T_*$ limit is $H_*^{-1}$, the radiation-era [particle horizon](../../../cosmology.md#particle-horizon). For $m/T_*\gg1$, the ratio is approximately $(T_*/m)\log(2m/T_*)$, retaining the distance accumulated while the particle was faster.

There is a normalization qualification: in arbitrary fixed [comoving coordinates](../../../cosmology.md#comoving-coordinate) the distance is $\chi=H_*^{-1}\operatorname{arsinh}(y)/(a_*y)$, $y=m/T_*$. The expression just derived is also the physical distance $L_*=a_*\chi$ at observation. Thus it equals a comoving distance only when $a_*=1$ is used, as in the preceding part. To express it in today's convention $a_0=1$, multiply $L_*$ by $1+z_*$. This is the [accumulated free-streaming distance in a radiation-dominated universe](../../../linear-cosmological-density-perturbation.md#accumulated-free-streaming-distance-in-a-radiation-dominated-universe).

Write $\omega_M=\Omega_Mh^2$, where $h$ here is the dimensionless present [Hubble constant](../../../cosmology.md#hubble-constant). The supplied equality [redshift](../../../optics.md#redshift) gives $1+z_{\rm eq}\simeq2.5\times10^4\omega_M$, and $T_{\rm eq}=T_0(1+z_{\rm eq})$. For $m=30\,\mathrm{eV}$ the requested dimensionless ratio is

$$
\boxed{\frac{L_{\rm eq}}{H_{\rm eq}^{-1}}=\frac{\operatorname{arsinh}(y_{\rm eq})}{y_{\rm eq}},\qquad y_{\rm eq}=\frac{30\,\mathrm{eV}}{T_0(1+z_{\rm eq})}.}
$$

The Hubble rate in this formula is the radiation-era extrapolation used in deriving it. A unique numerical ratio cannot be chosen without $\omega_M$.

**The printed [CMB](../../../cosmology.md#cosmic-microwave-background) [temperature](../../../thermodynamics.md#temperature) contains a factor-of-ten error.** Its $2.35\,\mathrm{meV}$ means $2.35\times10^{-3}\,\mathrm{eV}$, whereas the [cosmic microwave background temperature in energy units](../../../cosmology.md#cosmic-microwave-background-temperature-in-energy-units) is about $2.35\times10^{-4}\,\mathrm{eV}=0.235\,\mathrm{meV}$, corresponding to $2.725\,\mathrm K$. The [temperature](../../../thermodynamics.md#temperature) is supported by [NASA's CMB measurements](https://asd.gsfc.nasa.gov/archive/arcade/cmb_temperature.html). Using the printed value gives $y_{\rm eq}\simeq0.5106/\omega_M$; using the corrected value gives $y_{\rm eq}\simeq5.106/\omega_M$. For the illustrative choice $\Omega_M=1,h=0.5$, so $\omega_M=0.25$, these give respectively $T_{\rm eq}\simeq14.7$ and $1.47\,\mathrm{eV}$, and distance-to-Hubble-radius ratios about $0.716$ and $0.182$. This benchmark is an assumption for the estimate, not an extra parameter supplied by the paper.

For the present-day comoving length, use $H_r(z_{\rm eq})=H_0\sqrt{\Omega_M}(1+z_{\rm eq})^{3/2}$, the radiation contribution extrapolated to equality. Restoring $c$ for the conversion and using $c/H_0\simeq2998h^{-1}\,\mathrm{Mpc}$ gives

$$
\chi_0\simeq\frac{c}{H_0\sqrt{\Omega_M}\sqrt{1+z_{\rm eq}}}\frac{\operatorname{arsinh}(y_{\rm eq})}{y_{\rm eq}}\simeq\boxed{\frac{18.96}{\omega_M}\frac{\operatorname{arsinh}(y_{\rm eq})}{y_{\rm eq}}\,\mathrm{Mpc}.}
$$

For the same benchmark, this is about $54\,\mathrm{Mpc}$ using the printed [temperature](../../../thermodynamics.md#temperature) and $14\,\mathrm{Mpc}$ using the corrected [temperature](../../../thermodynamics.md#temperature), in the prescribed representative-momentum radiation-era model.

At equality matter is no longer negligible, so these are transition-era estimates. The actual total $H_{\rm eq}$ is $\sqrt2H_r(z_{\rm eq})$; inserting it in the simple normalization would lower the length by $\sqrt2$, but would not constitute an exact [integration](../../../calculus.md#integral) through equality. An exact matter-plus-radiation treatment instead replaces the radiation integral by

$$
\chi_0=\frac{c}{H_0\sqrt{\Omega_r}}\int_0^{a_{\rm eq}}\frac{da}{\sqrt{1+a/a_{\rm eq}}\sqrt{1+(ma/p_0)^2}},\qquad a_0=1,
$$

with $p_0=T_0$ in the assumed model. This makes the order-one equality correction explicit. Real [neutrino](../../../standard-model.md#neutrino) [physical momenta in an FRW universe](../../../linear-cosmological-density-perturbation.md#physical-momentum-in-an-frw-universe) are distributed and their [temperature](../../../thermodynamics.md#temperature) need not equal the [photon](../../../quantum-mechanics.md#photon) [temperature](../../../thermodynamics.md#temperature); the calculation above follows the specified $p=T_r$ idealization.

## 2

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Vary the [scalar field](../../../quantum-field-theory.md#scalar-field) and integrate by parts, taking the [variation](../../../calculus-of-variations.md#variation) to vanish at the boundary:

$$
\delta S=\int d^4x\sqrt{-g}\left\{\nabla_\mu\nabla^\mu\phi-V_{,\phi}\right\}\delta\phi.
$$

Thus the curved-spacetime [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) is $\Box\phi-V_{,\phi}=0$. In the flat [FRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric), $\sqrt{-g}=a^3$ and $g^{00}=-1$. A spatially homogeneous field therefore has

$$
\Box\phi=\frac1{a^3}\partial_t(-a^3\dot\phi)=-\ddot\phi-3\frac{\dot a}{a}\dot\phi.
$$

Consequently

$$
\boxed{\ddot\phi+3H\dot\phi+V_{,\phi}=0,\qquad H=\frac{\dot a}{a}.}
$$

Dots now denote [cosmic time](../../../cosmology.md#cosmic-time) derivatives. The $3H\dot\phi$ term is [Hubble friction](../../../cosmology.md#hubble-friction) caused by expansion of the [comoving volume](../../../cosmology.md#comoving-volume).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For a [variation](../../../calculus-of-variations.md#variation) of the covariant [metric tensor](../../../general-relativity.md#metric-tensor), $\delta g^{\alpha\beta}=-g^{\alpha\mu}g^{\beta\nu}\delta g_{\mu\nu}$ and $\delta\sqrt{-g}=\tfrac12\sqrt{-g}\,g^{\mu\nu}\delta g_{\mu\nu}$. Writing $\mathcal L=-\tfrac12g^{\alpha\beta}\partial_\alpha\phi\partial_\beta\phi-V$, one obtains

$$
\delta S=\frac12\int d^4x\sqrt{-g}\left\{\partial^\mu\phi\partial^\nu\phi+g^{\mu\nu}\mathcal L\right\}\delta g_{\mu\nu}.
$$

The specified metric-variation convention therefore gives

$$
\boxed{T^{\mu\nu}=\partial^\mu\phi\partial^\nu\phi-g^{\mu\nu}\left(\tfrac12\partial_\alpha\phi\partial^\alpha\phi+V\right).}
$$

For $\phi=\phi(t)$, its invariant gradient square is $-\dot\phi^2$. Hence $T^{00}=\dot\phi^2-(\dot\phi^2/2-V)=\dot\phi^2/2+V$, while $T^{ij}=a^{-2}\delta^{ij}(\dot\phi^2/2-V)$ and $T^{0i}=0$. Lowering one index makes $T^\mu{}_{\nu}=\operatorname{diag}(-\rho,P,P,P)$, with

$$
\boxed{\rho=\frac12\dot\phi^2+V(\phi),\qquad P=\frac12\dot\phi^2-V(\phi).}
$$

[Potential energy](../../../classical-mechanics.md#potential-energy) has negative [pressure](../../../thermodynamics.md#pressure), whereas scalar [kinetic energy](../../../classical-mechanics.md#kinetic-energy) contributes positive [pressure](../../../thermodynamics.md#pressure). This sign distinction is what permits accelerated expansion.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

With spatial flatness, the scalar as the only source, and $M_{\rm Pl}=(8\pi G)^{-1/2}$, the [Friedmann equation](../../../cosmology.md#friedmann-equations) is

$$
\boxed{H^2=\frac{\rho}{3M_{\rm Pl}^2}=\frac{\dot\phi^2/2+V}{3M_{\rm Pl}^2}.}
$$

The scalar equation gives $\dot\rho=\dot\phi(\ddot\phi+V_{,\phi})=-3H\dot\phi^2$, which is the energy-conservation equation $\dot\rho+3H(\rho+P)=0$. Differentiating the [Friedmann equation](../../../cosmology.md#friedmann-equations) on the expanding branch yields $6M_{\rm Pl}^2H\dot H=-3H\dot\phi^2$, so $\dot H=-\dot\phi^2/(2M_{\rm Pl}^2)$. Combining this with $\ddot a/a=H^2+\dot H$ gives the [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation):

$$
\boxed{\frac{\ddot a}{a}=\frac{V-\dot\phi^2}{3M_{\rm Pl}^2}=-\frac{\rho+3P}{6M_{\rm Pl}^2}.}
$$

Thus **[cosmic inflation](../../../cosmic-inflation.md) occurs exactly when $V(\phi)>\dot\phi^2$** in this canonical scalar model. Equivalently $P<-\rho/3$, or the [first Hubble slow-roll parameter](../../../cosmic-inflation.md#first-hubble-slow-roll-parameter) $\epsilon_H=-\dot H/H^2$ is smaller than one.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Assume $V>0$ and that its derivatives do not change substantially over the field interval traversed in the estimate. With initially negligible [kinetic energy](../../../classical-mechanics.md#kinetic-energy), $H^2\simeq V/(3M_{\rm Pl}^2)$. The force $-V_{,\phi}$ changes the field [velocity](../../../classical-mechanics.md#velocity) on the [Hubble friction](../../../cosmology.md#hubble-friction) time. Keeping $H$ and $V_{,\phi}$ approximately constant for that local estimate, and starting at rest, solves the field equation explicitly:

$$
\dot\phi(t)=-\frac{V_{,\phi}}{3H}(1-e^{-3H\Delta t}),\qquad \Delta t=t-t_i.
$$

After one [Hubble time](../../../cosmology.md#hubble-time),

$$
\frac{\dot\phi^2}{V}\simeq\frac{M_{\rm Pl}^2V_{,\phi}^2}{3V^2}(1-e^{-3})^2.
$$

Writing $A=M_{\rm Pl}^2V_{,\phi}^2/V^2$, the condition $A<1$ keeps this kinetic-to-potential ratio below about $0.31$, comfortably inside the inflationary bound. Integrating once more gives the fractional potential change estimate

$$
\frac{|\Delta V|}{V}\simeq A\left[1-\frac{1-e^{-3}}3\right]\simeq0.683A
$$

over the same interval. Thus the characteristic time for an order-one potential change is $H^{-1}/A$, up to constants of order one. The requested local Hubble-timescale criterion is

$$
\boxed{M_{\rm Pl}^2\frac{V_{,\phi}^2}{V^2}\lesssim1.}
$$

Using a strict inequality with one as the order-one threshold is conventional; its coefficient is not an exact universal end-of-inflation bound. Much smaller $A$ gives the controlled slow-roll regime and many [Hubble times](../../../cosmology.md#hubble-time) of [cosmic inflation](../../../cosmic-inflation.md) if the bounds persist.

After the transient in [relaxation to the slow-roll attractor](../../../cosmic-inflation.md#relaxation-to-the-slow-roll-attractor), $3H\dot\phi\simeq-V_{,\phi}$. Differentiating this approximate relation gives

$$
\frac{\ddot\phi}{H\dot\phi}\simeq-\frac{V_{,\phi\phi}}{3H^2}-\frac{\dot H}{H^2}\simeq-\eta_V+\epsilon_V,
\qquad \epsilon_V=\frac{M_{\rm Pl}^2}{2}\left(\frac{V_{,\phi}}V\right)^2,\quad \eta_V=M_{\rm Pl}^2\frac{V_{,\phi\phi}}V.
$$

Therefore the standard sufficient conditions for negligible acceleration throughout slow roll are $\epsilon_V\ll1$ and

$$
\boxed{\left|M_{\rm Pl}^2\frac{V_{,\phi\phi}}V\right|\ll1.}
$$

The [absolute value](../../../real-analysis.md#absolute-value) matters: large negative curvature also drives rapid evolution. The more precise local acceleration criterion is $|\eta_V-\epsilon_V|\ll1$, with the usual separate smallness conditions avoiding a tuned cancellation. If a field starts exactly at rest on a nonzero slope, its initial acceleration is not negligible; the displayed exponential transient describes its approach to the attractor.

These are local timescale and slow-roll conditions, rather than a global duration theorem from derivatives at a single point. A smooth potential can have a narrow flat shoulder followed by a steep drop, ending [cosmic inflation](../../../cosmic-inflation.md) soon despite small starting derivatives. The conditions must hold over the traversed interval. This is the additional smooth-evolution assumption implicit in the estimate.

## 3

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

[Chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) for $p+e^-\leftrightarrow H+\gamma$ implies $\mu_H=\mu_p+\mu_e$, because equilibrium [photons](../../../quantum-mechanics.md#photon) have zero [chemical potential](../../../thermodynamics.md#chemical-potential). Dividing the three nonrelativistic Maxwell-Boltzmann [number densities](../../../statistical-physics.md#number-density) therefore gives

$$
\frac{n_H}{n_pn_e}=\frac{g_H}{g_pg_e}\left(\frac{m_H}{m_pm_e}\right)^{3/2}\left(\frac{2\pi}T\right)^{3/2}\exp\!\left(\frac{m_p+m_e-m_H}T\right).
$$

The [Hydrogen binding energy](../../../cosmology.md#hydrogen-binding-energy) is $I=m_p+m_e-m_H=13.6\,\mathrm{eV}$ in [natural units](../../../physics.md#natural-units). For ground-state [hydrogen](../../../chemistry.md#hydrogen), with hyperfine splittings unresolved, $g_H=4$ and $g_p=g_e=2$, so the degeneracy ratio is one. Equivalently one can omit nuclear-spin degeneracy consistently from both the [proton](../../../physics.md#proton) and atom. Excited [hydrogen](../../../chemistry.md#hydrogen) levels are exponentially suppressed at [recombination temperatures](../../../cosmology.md#recombination-temperature). Also $m_H/m_p=1+O(m_e/m_p)$, so its effect in the prefactor is negligible. Thus

$$
\boxed{\frac{n_H}{n_pn_e}\simeq\left(\frac{2\pi}{m_eT}\right)^{3/2}e^{I/T}.}
$$

The sign of the exponential follows from the smaller [rest mass](../../../special-relativity.md#invariant-mass) of the bound atom: cooling favours neutral [hydrogen](../../../chemistry.md#hydrogen) once translational [entropy](../../../thermodynamics.md#entropy) no longer compensates the binding [energy](../../../classical-mechanics.md#energy).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Ignoring [helium](../../../chemistry.md#helium), [charge neutrality](../../../electromagnetism.md#charge-neutrality) gives $n_e=n_p$, while [baryon](../../../physics.md#baryon) conservation gives $n_B=n_p+n_H$. Defining the [hydrogen ionization fraction](../../../cosmology.md#hydrogen-ionization-fraction) $X_e=n_e/n_B$ yields $n_p=n_e=X_en_B$ and $n_H=(1-X_e)n_B$. Substituting in the abundance relation gives

$$
\frac{1-X_e}{X_e^2}=n_B\left(\frac{2\pi}{m_eT}\right)^{3/2}e^{I/T}.
$$

Use $n_B=\eta n_\gamma$ and $n_\gamma=2\zeta(3)T^3/\pi^2$ to obtain the [Saha equation](../../../cosmology.md#saha-ionization-equation):

$$
\boxed{\frac{1-X_e}{X_e^2}=\frac{2\zeta(3)}{\pi^2}\eta\left(\frac{2\pi T}{m_e}\right)^{3/2}e^{I/T}.}
$$

If the positive right side is denoted by $A(T)$, the physical root is

$$
\boxed{X_e(T)=\frac2{1+\sqrt{1+4A(T)}}.}
$$

This form avoids subtracting nearly equal numbers when $A$ is small, and makes the limits transparent: $X_e\simeq1-A$ for $A\ll1$, whereas $X_e\simeq A^{-1/2}$ for $A\gg1$. It is an equilibrium prediction; a kinetic [cosmological recombination](../../../cosmology.md#recombination-cosmology) treatment is needed after reactions cease to keep up with expansion.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

There are about $\eta^{-1}\sim10^9$ [photons](../../../quantum-mechanics.md#photon) per [baryon](../../../physics.md#baryon). Even when the typical [photon](../../../quantum-mechanics.md#photon) [energy](../../../classical-mechanics.md#energy) is below the [Hydrogen binding energy](../../../cosmology.md#hydrogen-binding-energy), the high-energy tail can provide abundant ionizing [photons](../../../quantum-mechanics.md#photon). The nonrelativistic [Electron](../../../physics.md#electron)'s translational [phase space](../../../classical-mechanics.md#phase-space) also favours the ionized state. Quantitatively, the [Saha equation](../../../cosmology.md#saha-ionization-equation) contains both suppressing factors $\eta$ and $(T/m_e)^{3/2}$. Recombination needs their tiny product to be overcome by $e^{I/T}$, so $I/T$ must be several tens, not of order one.

For an illustrative $\Omega_Bh^2=0.02$, the supplied baryon-to-photon relation gives $\eta=5.36\times10^{-10}$. With $m_e=5.11\times10^5\,\mathrm{eV}$, direct evaluation gives

$$
\begin{array}{c|ccc}
T\ (\mathrm{eV})&0.30&0.28&0.27\\
A(T)&45.1&1.04\times10^3&5.93\times10^3\\
X_e&0.138&0.0306&0.0129
\end{array}
$$

Thus **the equilibrium ionization fraction reaches a few per cent just below $0.3\,\mathrm{eV}$**, while at $13.6\,\mathrm{eV}$ it is essentially unity. The exact [temperature](../../../thermodynamics.md#temperature) depends weakly on the [baryon](../../../physics.md#baryon) abundance and on the fraction used to define [cosmological recombination](../../../cosmology.md#recombination-cosmology). This is [small baryon abundance delays hydrogen recombination](../../../cosmology.md#small-baryon-abundance-delays-hydrogen-recombination). Recombination, [photon decoupling](../../../cosmology.md#photon-decoupling) and [residual electron freeze-out](../../../cosmology.md#residual-electron-freeze-out) are related but distinct: the last two involve rates and cannot be determined by [chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) alone.

<a id="3/c/image-hydrogen-only-saha-ionization-fraction-during-cooling-with-the-three-per-cent-crossing-near-0-28-electronvolts-for-baryon-to-photon-ratio-5-36-times-ten-to-the-minus-ten"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-62-saha-ionization.png)

**[Figure 1](#3/c/image-hydrogen-only-saha-ionization-fraction-during-cooling-with-the-three-per-cent-crossing-near-0-28-electronvolts-for-baryon-to-photon-ratio-5-36-times-ten-to-the-minus-ten). Hydrogen-only Saha ionization fraction during cooling, with the three-per-cent crossing near 0.28 electronvolts for baryon-to-photon ratio 5.36 times ten to the minus ten**.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Use the flat matter-only Einstein-de Sitter approximation for the distance-redshift relation, neglecting radiation corrections at [cosmological recombination](../../../cosmology.md#recombination-cosmology). Let $z_*$ be the [cosmological recombination](../../../cosmology.md#recombination-cosmology) [redshift](../../../optics.md#redshift). Adiabatic [photon](../../../quantum-mechanics.md#photon) cooling gives $1+z_*=T_*/T_0$. The Hubble rate is $H(z)=H_0(1+z)^{3/2}$, so the [comoving radial distance](../../../cosmology.md#comoving-radial-distance) to last scattering is

$$
\chi_* =\int_0^{z_*}\frac{dz}{H(z)}=\frac2{H_0}\left(1-\frac1{\sqrt{1+z_*}}\right).
$$

The [angular diameter distance](../../../cosmology.md#angular-diameter-distance) is $D_A=\chi_* /(1+z_*)$. A proper [Hubble radius](../../../cosmology.md#hubble-radius) $H_*^{-1}=H_0^{-1}(1+z_*)^{-3/2}$ therefore subtends the small angle

$$
\boxed{\theta_H=\frac{H_*^{-1}}{D_A}=\frac1{2(\sqrt{1+z_*}-1)}\quad\text{radians}.}
$$

This is the [angular Hubble-radius scale in an Einstein-de Sitter universe](../../../cosmology.md#angular-hubble-radius-scale-in-an-einstein-de-sitter-universe); the present [Hubble constant](../../../cosmology.md#hubble-constant) cancels.

Taking $T_*=0.3\,\mathrm{eV}$ and the literal printed $T_0=2.35\,\mathrm{meV}$ gives $1+z_*=127.7$ and $\theta_H\simeq0.0486$ radians, or $2.8$ degrees. As noted above, that present [CMB](../../../cosmology.md#cosmic-microwave-background) [energy](../../../classical-mechanics.md#energy) is too large by ten. With the corrected $T_0=0.235\,\mathrm{meV}$, $1+z_*=1277$ and

$$
\boxed{\theta_H\simeq0.0144\ \mathrm{rad}\simeq0.83^\circ,}
$$

which gives the familiar order-one-degree scale within the assumed cosmology. Using $0.28\,\mathrm{eV}$ to mark a few-per-cent ionization fraction changes this only modestly. These numbers refer to the Hubble-radius scale, not its diameter. In a matter-only universe the particle-horizon radius is $2H^{-1}$ and would give twice the angle; the acoustic [sound horizon](../../../cosmic-microwave-background-anisotropy.md#sound-horizon) is a different length again.

## 4

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

At [linear order](../../../algebra.md#linear-order) a coordinate displacement $\xi^\mu$ changes a [metric perturbation](../../../general-relativity.md#linearized-gravity) by $q_{\mu\nu}\mapsto q_{\mu\nu}-\mathcal L_\xi\bar g_{\mu\nu}$. Work in [conformal time](../../../cosmology.md#conformal-time) with $\bar g_{\mu\nu}=a^2\operatorname{diag}(-1,1,1,1)$, write $\xi^0=\alpha$ and lower spatial indices with $\delta_{ij}$. Directly evaluating the [Lie derivative of a covariant tensor field](../../../fiber-bundle.md#lie-derivative-of-a-covariant-tensor-field) gives

$$
q'_{00}=q_{00}+2a^2(\alpha'+\mathcal H\alpha),\qquad q'_{0i}=q_{0i}-a^2(\xi_i'-\partial_i\alpha),\qquad\mathcal H=\frac{a'}a.
$$

Here primes on $\alpha,\xi_i$ mean conformal-time derivatives, while primes on $q'_{0\mu}$ label transformed components. Setting the transformed lapse and shift perturbations to zero requires

$$
\alpha'+\mathcal H\alpha=-\frac{q_{00}}{2a^2},\qquad \xi_i'=\frac{q_{0i}}{a^2}+\partial_i\alpha.
$$

These are first-order time equations. Their explicit local solutions are

$$
\alpha(\tau,x)=\frac1{a(\tau)}\left[C(x)-\int^{\tau}\frac{q_{00}(s,x)}{2a(s)}\,ds\right],\qquad
\xi_i(\tau,x)=D_i(x)+\int^{\tau}\left[\frac{q_{0i}(s,x)}{a(s)^2}+\partial_i\alpha(s,x)\right]ds.
$$

Thus four coordinate functions can impose the four synchronous conditions in any regular perturbative patch. This is [synchronous gauge fixing by coordinate displacement](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-fixing-by-coordinate-displacement). The arbitrary spatial functions $C,D_i$ remain as residual gauge freedom; the conditions alone do not fix the coordinate system completely.

Geometrically, synchronous coordinates follow a congruence of freely falling observers launched normally from a spatial slice, using their [proper time](../../../special-relativity.md#proper-time). This gives unit lapse and zero shift in [cosmic time](../../../cosmology.md#cosmic-time); conversion to background [conformal time](../../../cosmology.md#conformal-time) gives the displayed convention. “Always possible” is local: [geodesic](../../../riemannian-geometry.md#geodesic) caustics or singularities can prevent a global synchronous chart. Such global obstructions do not invalidate local [linear cosmological perturbation theory](../../../linear-cosmological-perturbation-theory.md).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use primes for conformal-time derivatives. The cold-dark-matter [Cosmological Euler equation in synchronous gauge](../../../linear-cosmological-perturbation-theory.md#cosmological-euler-equation-in-synchronous-gauge) is $v_C'+\mathcal Hv_C=0$, so multiplying by $a$ gives $(av_C)'=0$. Therefore

$$
\boxed{v_C(\tau,x)=\frac{a(\tau_i)}{a(\tau)}v_C(\tau_i,x).}
$$

In an expanding universe $a$ increases, damping any initial [peculiar velocity](../../../cosmology.md#peculiar-velocity) as $a^{-1}$. During [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination) $a\propto\tau$, so the [velocity](../../../classical-mechanics.md#velocity) scales as $\tau^{-1}$; during [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination) $a\propto\tau^2$, it scales as $\tau^{-2}$. This is the [nonrelativistic limit](../../../special-relativity.md#nonrelativistic-limit) of the physical-momentum [redshift](../../../optics.md#redshift) derived in Q1. It concerns the bulk [velocity](../../../classical-mechanics.md#velocity) in the synchronous coordinate frame, not a growing [peculiar velocity](../../../cosmology.md#peculiar-velocity) sourced in another gauge. A cold-matter rest-frame choice also removes the residual synchronous time displacement relevant to that component. The decay statement assumes expanding evolution and the pressureless, linear approximation used by the equation.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

With negligible cold-dark-matter [velocity](../../../classical-mechanics.md#velocity), the [synchronous perfect-fluid density equation](../../../linear-cosmological-perturbation-theory.md#synchronous-perfect-fluid-density-equation) gives $\delta_C'=-h'/2$. Differentiate and use the trace [Einstein equation](../../../general-relativity.md#einstein-field-equations), taking the cold matter [sound speed](../../../compressible-flow.md#speed-of-sound) to vanish and its density to dominate:

$$
\delta_C''+\mathcal H\delta_C'=4\pi Ga^2\rho_C\delta_C.
$$

In a spatially flat [matter-dominated universe](../../../linear-cosmological-density-perturbation.md#matter-domination), $a\propto\tau^2$, $\mathcal H=2/\tau$, and the conformal [Friedmann equation](../../../cosmology.md#friedmann-equations) gives $4\pi Ga^2\rho_C=3\mathcal H^2/2=6/\tau^2$. Hence

$$
\delta_C''+\frac2\tau\delta_C'-\frac6{\tau^2}\delta_C=0.
$$

Put $\delta_C\propto\tau^s$. The [indicial equation](../../../differential-equation.md#indicial-equation) is $s(s-1)+2s-6=(s-2)(s+3)=0$. These two independent modes span the solution space, so

$$
\boxed{\delta_C(\tau,x)=A(x)\tau^2+B(x)\tau^{-3}.}
$$

Equivalently the growing mode is proportional to $a$ and the decaying mode to $a^{-3/2}$. The coefficients are set by [initial data](../../../general-relativity.md#initial-data-in-general-relativity). Since [synchronous gauge](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology) has residual coordinate modes, interpreting the [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) physically requires fixing its residual freedom consistently, for example by the cold-matter [rest frame](../../../physics.md#rest-frame) and [metric tensor](../../../general-relativity.md#metric-tensor) [integration](../../../calculus.md#integral) convention; the mode equation alone is not a gauge-invariant observable.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The continuity and [Cosmological Euler equation in synchronous gauge](../../../linear-cosmological-perturbation-theory.md#cosmological-euler-equation-in-synchronous-gauge) combine particularly simply. Differentiate $\delta_C'=-\nabla\cdot v_C-h'/2$ and add $\mathcal H\delta_C'$:

$$
\delta_C''+\mathcal H\delta_C'=-\nabla\cdot(v_C'+\mathcal Hv_C)-\frac12(h''+\mathcal Hh')=4\pi Ga^2\sum_N(1+3c_N^2)\rho_N\delta_N.
$$

The [velocity](../../../classical-mechanics.md#velocity) terms cancel by the [Cosmological Euler equation in synchronous gauge](../../../linear-cosmological-perturbation-theory.md#cosmological-euler-equation-in-synchronous-gauge), so this step does not require setting the initial [velocity](../../../classical-mechanics.md#velocity) exactly to zero.

For subhorizon modes deep in [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), take the rapidly oscillating radiation perturbation to be negligible in the averaged gravitational forcing. Also neglect the subdominant matter self-gravity to leading order in $\rho_C/\rho_r$. With $a\propto\tau$ and $\mathcal H=1/\tau$, the resulting equation is

$$
\delta_C''+\frac1\tau\delta_C'=0,\qquad (\tau\delta_C')'=0.
$$

Integrating twice gives

$$
\boxed{\delta_C(\tau,x)=A(x)\log(\tau/\tau_*)+B(x),}
$$

where the arbitrary reference time $\tau_*$ makes the logarithm dimensionless and can be absorbed into $B$. This is [logarithmic growth of matter perturbations during radiation domination](../../../linear-cosmological-density-perturbation.md#logarithmic-growth-of-matter-perturbations-during-radiation-domination).

The neglect of matter self-gravity is needed for the displayed form to be exact within the leading radiation-background approximation. Uniform radiation alone leaves a nonzero term $4\pi Ga^2\rho_C\delta_C$ if the cold-matter density is retained. Relative to $\mathcal H^2$, its coefficient is $3\Omega_C(a)/2$, small deep in the radiation era but not near equality. The [Mészáros equation](../../../linear-cosmological-density-perturbation.md#meszaros-equation) retains that effect in a matter-plus-radiation background; its solution basis tends to a constant and a logarithm at $a/a_{\rm eq}\ll1$, recovering the present leading result. It connects smoothly to matter-era growth rather than allowing the logarithmic approximation to be extrapolated indefinitely.

Galaxy-scale modes enter the [Hubble radius](../../../cosmology.md#hubble-radius) before [matter-radiation equality](../../../cosmology.md#matter-radiation-equality). The earlier radiation forcing and horizon-entry matching ordinarily generate a nonzero logarithmic coefficient, even though subsequent oscillatory radiation forcing is small. A [Fourier mode](../../../fourier-analysis.md#fourier-mode) with entry time $\tau_h\sim k^{-1}$ accumulates $\log(\tau_{\rm eq}/\tau_h)\sim\log(k\tau_{\rm eq})$ before equality. Across a large scale-factor range this factor need not be small, so treating the [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) as exactly frozen would lose an important part of the galaxy-scale seed amplitude and its scale dependence. Growth is nevertheless much slower than $\delta_C\propto a$ in [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination). This is the [Mészáros effect](../../../linear-cosmological-density-perturbation.md#meszaros-effect), and the logarithmic matching contributes to the small-scale matter [cold-dark-matter transfer function](../../../linear-cosmological-perturbation-theory.md#cold-dark-matter-transfer-function).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
