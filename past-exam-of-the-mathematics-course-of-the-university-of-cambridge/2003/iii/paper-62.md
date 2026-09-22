# Paper 62

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper62.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper62.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For an [ideal gas](../../../thermodynamics.md#ideal-gas) with constant [adiabatic index](../../../thermodynamics.md#heat-capacity-ratio) $\gamma>1$, let $c_v$ and $c_p$ be specific heat capacities and $\mathcal R=c_p-c_v$. The [ideal gas law](../../../thermodynamics.md#ideal-gas-law) and the [internal energy of an ideal gas](../../../thermodynamics.md#internal-energy-of-an-ideal-gas) give $P=\rho\mathcal RT$ and specific internal energy $e=c_vT$. Since $\gamma=c_p/c_v$, the [internal energy](../../../thermodynamics.md#internal-energy) per unit volume is $\rho e=P/(\gamma-1)$. Consequently a star with [spherical symmetry](../../../geometry-and-topology.md#spherical-symmetry) has

$$
\boxed{U=\frac1{\gamma-1}\int P\,dV=\frac{4\pi}{\gamma-1}\int_0^R P(r)r^2\,dr.}
$$

The radial integral requires the volume measure $dV=4\pi r^2dr$: the first printed expression omits this factor if its differential is read literally as $dr$. The mass-coordinate expression confirms the required volume interpretation.

Define the enclosed mass $M(r)$, total mass $M_{\rm tot}$ and dimensionless shell label $m=M(r)/M_{\rm tot}$. [Mass conservation](../../../continuum-mechanics.md#mass-conservation) gives $M_{\rm tot}\,dm=dM=\rho\,dV$, so the [change of variables](../../../calculus.md#change-of-variables-formula) gives

$$
\boxed{U=\frac{M_{\rm tot}}{\gamma-1}\int_0^1\frac{P(m)}{\rho(m)}\,dm.}
$$

Here $m$ labels a fixed material shell rather than its radial position. In a mass-preserving [stellar homology](../../../stellar-structure.md#stellar-homology), $r(m)=xr_0(m)$ with $x=R/R_0$. Both a shell's radius and thickness gain a factor $x$, so its volume gains $x^3$ and its [mass density](../../../fluid-mechanics.md#density) becomes $\rho(m)=x^{-3}\rho_0(m)$. An [adiabatic process](../../../thermodynamics.md#adiabatic-process) keeps $P/\rho^\gamma$ fixed separately in each shell, even if that constant differs between shells. Thus $P=x^{-3\gamma}P_0$ and $P/\rho=x^{-3(\gamma-1)}P_0/\rho_0$. Integration at fixed mass labels proves

$$
\boxed{U(x)=U_0x^{-3(\gamma-1)}.}
$$

The [spherical shell theorem](../../../physics.md#spherical-shell-theorem) gives the [Newtonian gravitational potential energy](../../../classical-mechanics.md#newtonian-gravitational-potential-energy) by assembling shells against the mass already inside them:

$$
W=-\int_0^{M_{\rm tot}}\frac{GM}{r(M)}\,dM.
$$

Every radius gains the same factor $x$, while $M$ and $dM$ remain fixed. Hence

$$
\boxed{W(x)=W_0x^{-1},\qquad E(x)=U_0x^{-a}+W_0x^{-1},\quad a=3(\gamma-1).}
$$

This is the [homologous adiabatic stellar stability](../../../stellar-structure.md#homologous-adiabatic-stellar-stability) test. The derivative with respect to the physical stellar radius is $\partial_R=R_0^{-1}\partial_x$. Stationarity at $x=1$ therefore requires $-aU_0-W_0=0$, or

$$
\boxed{|W_0|=3(\gamma-1)U_0.}
$$

After imposing this equilibrium relation, $E/U_0=x^{-a}-a/x$ and

$$
\frac{dE}{dx}=aU_0\left(x^{-2}-x^{-a-1}\right),\qquad
\left.\frac{\partial^2E}{\partial R^2}\right|_{R_0}=\frac{a(a-1)U_0}{R_0^2}.
$$

Since $a>0$, a strict energy minimum under this homologous displacement requires

$$
\boxed{\gamma>\frac43.}
$$

For $a>1$, contraction sends $E$ to $+\infty$, expansion sends it to $0$ from below, and $x=1$ is the unique minimum, with $E(1)=(1-a)U_0<0$. For $0<a<1$, contraction sends $E$ to $-\infty$, expansion sends it to $0$ from above, and $x=1$ is the unique maximum. When $a=1$, the equilibrium relation makes $E(x)=0$ for every $x$: the scale direction is marginal, not strictly stable. The plotted curves display these three possibilities. This checks homologous radial stability; stability against every stellar displacement needs a fuller perturbation analysis.

<a id="1/image-stellar-energy-under-homologous-adiabatic-expansion-stable-minimum-unstable-maximum-and-marginal-scaling"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-62-energy.png)

**[Figure 1](#1/image-stellar-energy-under-homologous-adiabatic-expansion-stable-minimum-unstable-maximum-and-marginal-scaling). Stellar energy under homologous adiabatic expansion: stable minimum, unstable maximum and marginal scaling**.

## 2

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write $\sigma_0^2=\langle v_z^2\rangle=v_{\rm rms}^2/3$ for the one-dimensional thermal [velocity dispersion](../../../galaxy.md#velocity-dispersion) of an isotropic monatomic [ideal gas](../../../thermodynamics.md#ideal-gas). An [isothermal process](../../../thermodynamics.md#isothermal-process) keeps $\sigma_0$ fixed, and the vertical [pressure](../../../thermodynamics.md#pressure) is $P=\rho\sigma_0^2$. [Hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) in the [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential) $\Phi(z)$ gives

$$
\sigma_0^2\frac{d\log\rho}{dz}=-\frac{d\Phi}{dz}.
$$

Planar symmetry reduces the [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity) to $\Phi''=4\pi G\rho$. Combining the two equations yields

$$
\boxed{\sigma_0^2\frac{d^2\log\rho}{dz^2}=-4\pi G\rho.}
$$

The velocity factor here is a velocity second moment, not the square of a particular particle's instantaneous vertical velocity.

Set $H^2=\sigma_0^2/(2\pi G\rho_0)$ and try the symmetric [self-gravitating isothermal slab](../../../galaxy.md#self-gravitating-isothermal-slab) profile $\rho=\rho_0\operatorname{sech}^2(z/H)$. Its logarithmic derivatives are

$$
\frac{d\log\rho}{dz}=-\frac2H\tanh(z/H),\qquad
\frac{d^2\log\rho}{dz^2}=-\frac2{H^2}\operatorname{sech}^2(z/H).
$$

The chosen $H$ makes the second expression satisfy the required equation. The central conditions $\rho(0)=\rho_0$ and $\rho'(0)=0$ fix the smooth even solution uniquely. In the scale-height convention used here,

$$
\boxed{\rho(z)=\rho_0\operatorname{sech}^2\!\left(\frac z{2z_0}\right),\qquad z_0=\frac{\sigma_0}{\sqrt{8\pi G\rho_0}},\qquad H=2z_0.}
$$

The undefined constant printed as $a$ in the scale-height denominator must be $G$; this follows both from substitution and dimensions.

Integrating [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium), with the additive potential constant chosen so that $\Phi(0)=0$, gives

$$
\boxed{\Phi(z)=2\sigma_0^2\log\cosh(z/H),\qquad \ddot z=-\frac{2\sigma_0^2}{H}\tanh(z/H).}
$$

The [orbits in a self-gravitating isothermal slab](../../../galaxy.md#orbits-in-a-self-gravitating-isothermal-slab) separate into horizontal and vertical motions. There is no horizontal force, so $x=x_i+v_xt$ and $y=y_i+v_yt$, with constant horizontal velocities. For collisionless test particles, or between gas collisions, [conservation of energy](../../../physics.md#conservation-of-energy) fixes the vertical energy

$$
E_z=\frac12\dot z^2+\Phi(z).
$$

Every finite $E_z>0$ has two turning points $\pm A$, where

$$
A=H\operatorname{arcosh}\!\left(e^{E_z/(2\sigma_0^2)}\right),\qquad
T_z=4\int_0^A\frac{dz}{\sqrt{2[E_z-\Phi(z)]}}.
$$

Thus the general orbit drifts uniformly in the plane while oscillating periodically across it. A particle with $E_z=0$ stays in the midplane; an orbit with nonzero horizontal velocity is generally not closed.

Near the plane, $\Phi(z)=\sigma_0^2z^2/H^2+O(z^4)$, so the vertical motion is a [harmonic oscillator](../../../classical-mechanics.md#simple-harmonic-motion) with $\nu^2=2\sigma_0^2/H^2=4\pi G\rho_0$. Far from the plane, $\Phi\sim2\sigma_0^2|z|/H$ and the force tends to a constant magnitude. Indeed the [surface density](../../../astrophysics.md#surface-density-of-a-disk) is $\Sigma=\int\rho\,dz=2\rho_0H$, and that magnitude is $2\pi G\Sigma$. Large-amplitude vertical motion is therefore approximately uniformly accelerated on each side, rather than sinusoidal. Because this ideal slab extends infinitely in the horizontal directions and its potential grows without bound as $|z|\to\infty$, no finite-energy particle escapes vertically.

## 3

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For an isolated smooth mass distribution with [spherical symmetry](../../../geometry-and-topology.md#spherical-symmetry), assemble each shell $dM$ at radius $r$ against the [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential) of its interior mass. The [spherical shell theorem](../../../physics.md#spherical-shell-theorem) gives

$$
W=-G\int_0^\infty\frac{M(r)}r\,dM(r)=-\frac G2\int_0^\infty\frac1r\,d[M(r)^2].
$$

Assume finite total mass, finite binding energy and no central point-mass self-energy, so $M(r)^2/r$ vanishes at both endpoints. [Integration by parts](../../../calculus.md#integration-by-parts) then gives

$$
\boxed{W=-\frac G2\int_0^\infty\frac{M(r)^2}{r^2}\,dr.}
$$

For example, $M(r)\propto r^3$ near a regular center guarantees the central boundary condition, while finite total mass guarantees the one at infinity. A divergent central binding energy would fall outside this formula's finite-energy hypotheses.

For the discrete system use the [centre of mass](../../../classical-mechanics.md#center-of-mass) frame, let $N$ be the particle number, and write $M_{\rm tot}=Nm$. The printed $M$ in the particle-count factor and the subsequent $n$ must be understood consistently as $N$. Define

$$
K=\frac12\sum_i m|\dot{\mathbf r}_i|^2,\qquad
W=-Gm^2\sum_{i<j}\frac1{r_{ij}},\qquad
I=\sum_i m|\mathbf r_i|^2.
$$

By [Newton's second law](../../../classical-mechanics.md#newton-s-second-law), differentiation gives

$$
\frac12\ddot I=2K+\sum_i\mathbf r_i\cdot\mathbf F_i.
$$

Each pair contributes

$$
\mathbf r_i\cdot\mathbf F_{ij}+\mathbf r_j\cdot\mathbf F_{ji}
=(\mathbf r_i-\mathbf r_j)\cdot\left[-Gm^2\frac{\mathbf r_i-\mathbf r_j}{r_{ij}^3}\right]
=-\frac{Gm^2}{r_{ij}}.
$$

Therefore the exact dynamical [virial theorem](../../../classical-mechanics.md#virial-theorem) is $\ddot I/2=2K+W$. In a stationary statistical state, or on a bounded-motion time average for which the mean $\ddot I$ vanishes, it becomes

$$
\boxed{2\langle K\rangle+\langle W\rangle=0.}
$$

There is no external pressure, tidal field or boundary work in this isolated point-particle derivation. For a time-averaged system, the following $W$ and [gravitational radius](../../../classical-mechanics.md#gravitational-radius) refer to that same averaged binding energy.

Using $W=-G(Nm)^2/R_g$ and $2K=Nm\langle v_{\rm eq}^2\rangle$, [virial equilibrium](../../../classical-mechanics.md#virial-equilibrium) gives

$$
\boxed{\langle v_{\rm eq}^2\rangle=\frac{GNm}{R_g},\qquad v_{{\rm eq},{\rm rms}}=\sqrt{\frac{GNm}{R_g}}.}
$$

This is the three-dimensional mean squared speed about the [centre of mass](../../../classical-mechanics.md#center-of-mass). For an isotropic system each one-dimensional [velocity dispersion](../../../galaxy.md#velocity-dispersion) squared is one third of it.

Set the [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential) to zero at infinity and exclude each particle's own field. The local [escape velocity](../../../classical-mechanics.md#escape-velocity) in the instantaneous frozen potential obeys $v_{{\rm esc},i}^2=-2\Phi_i$, where $\Phi_i=-Gm\sum_{j\ne i}r_{ij}^{-1}$. Since every pair occurs twice, $\sum_i m\Phi_i=2W$. Averaging over the identical particles proves the [gravitational rms escape and collapse speeds](../../../classical-mechanics.md#gravitational-rms-escape-and-collapse-speeds) relation

$$
\boxed{\langle v_{\rm esc}^2\rangle=-\frac{4W}{Nm}=\frac{4GNm}{R_g}=4\langle v_{\rm eq}^2\rangle,\qquad v_{{\rm esc},{\rm rms}}=2v_{{\rm eq},{\rm rms}}.}
$$

An actual encounter in a changing potential can exchange energy, so this is the usual local escape-speed definition, not a claim about every many-body trajectory.

Finally, dissipation-free collapse from rest at infinite separation has total energy zero. [Conservation of energy](../../../physics.md#conservation-of-energy) at the specified binding energy therefore gives $K_{\rm coll}=-W$, twice the equilibrium kinetic energy at the same $W$. Hence

$$
\boxed{\langle v_{\rm coll}^2\rangle=\frac{2GNm}{R_g}=2\langle v_{\rm eq}^2\rangle,\qquad v_{{\rm coll},{\rm rms}}=\sqrt2\,v_{{\rm eq},{\rm rms}}.}
$$

This mean squared speed includes coherent infall; a local random [velocity dispersion](../../../galaxy.md#velocity-dispersion) after subtracting the infall velocity need not obey that ratio.

## 4

↑ **Parent:** [Paper 62](paper-62.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

There is a genuine inconsistency in this part. For any nonnegative [metallicity distribution function](../../../galaxy.md#metallicity-distribution-function), its maximum is at least its mean. A population of positive mean solar [metallicity](../../../stellar-astrophysics.md#metallicity) cannot have a maximum equal to half that mean. For example, a uniform abundance distribution on $[0,2Z_\odot]$ has mean $Z_\odot$ and maximum $2Z_\odot$. Thus the printed maximum-to-mean ratio cannot be proved. The following calculation explains the supplied function, gives the consistent distribution, and also treats the literal birth-metallicity interpretation separately.

Let $f(\mu)$ denote the supplied abundance function. Algebraically it is

$$
f(\mu)=\frac{Y-(Y+1)\mu+\mu^{Y+1}}{(Y+1)(1-\mu)}.
$$

With $\delta=1-\mu$, a [Taylor series](../../../calculus.md#taylor-series) of $(1-\delta)^{Y+1}$ gives

$$
f(1-\delta)=\frac{Y\delta}{2}+\frac{Y(1-Y)\delta^2}{6}+O(\delta^3).
$$

Consequently

$$
\boxed{f(1-\delta)\simeq\frac{Y\delta}{2}.}
$$

This is an early-consumption expansion: its fractional correction is $(1-Y)\delta/3+O(\delta^2)$. Small yield alone does not make the expression linear throughout most of the gas-consumption history. At fixed $0<\mu<1$, the small-$Y$ expansion instead is

$$
f(\mu)=Y\left[1+\frac{\mu\log\mu}{1-\mu}\right]+O(Y^2).
$$

In a well-mixed [closed-box model of galactic chemical evolution](../../../galaxy.md#closed-box-model-of-galactic-chemical-evolution), the [gas fraction of a galaxy](../../../galaxy.md#gas-fraction-of-a-galaxy) also labels the permanently locked stellar mass: $dM_s=-M_{g,\rm init}\,d\mu$. Newly formed stars inherit the current [gas-phase metallicity](../../../galaxy.md#gas-phase-metallicity) $Z_g(\mu)$. Therefore the mass-weighted mean [stellar metallicity](../../../galaxy.md#stellar-metallicity) satisfies the [cumulative and birth stellar metallicities](../../../galaxy.md#cumulative-and-birth-stellar-metallicities) relation

$$
\overline Z_*(\mu)=\frac1{1-\mu}\int_\mu^1 Z_g(u)\,du,\qquad
Z_g(\mu)=-\frac{d}{d\mu}[(1-\mu)\overline Z_*(\mu)].
$$

Applying the derivative to $f$ gives

$$
\boxed{\overline Z_*(\mu)=f(\mu)\quad\Longleftrightarrow\quad Z_{\rm birth}(\mu)=Z_g(\mu)=1-\mu^Y.}
$$

Thus the supplied function has the natural interpretation of a cumulative mean, not an individual star's birth abundance. Direct integration of $1-u^Y$ verifies that it gives exactly $f$. This is the [saturating closed-box enrichment law](../../../galaxy.md#saturating-closed-box-enrichment-law): it corresponds to effective [stellar yield](../../../galaxy.md#stellar-yield) $Y(1-Z_g)$, with $Z_g$ measured as a fraction. The usual constant-yield trace-metal model instead gives $Z_g=-Y\log\mu$. Both agree to first order when $Y|\log\mu|\ll1$; their exact formulae should not be identified outside that regime.

Let the final gas fraction be $\mu_f>0$ and $\delta_f=1-\mu_f$. In the consistent mean-metallicity interpretation, $\overline Z_*(\mu_f)=Z_\odot$ while the most recently formed stars have the maximum $z_f=1-\mu_f^Y$. At early consumption,

$$
\overline Z_*\simeq\frac{Y\delta_f}{2},\qquad z_f\simeq Y\delta_f,
$$

so the corrected result is

$$
\boxed{Z_{*,\max}\simeq2Z_\odot.}
$$

The assumption here includes $\delta_f\ll1$, equivalently $2Z_\odot/Y\ll1$ in this approximation. Exactly, $z_f=1-\mu_f^Y$ and $Z_\odot=f(\mu_f)$ determine the maximum implicitly; it remains larger than the mean, but its ratio to the mean need not equal two after substantial consumption.

For the mass-weighted [metallicity distribution function](../../../galaxy.md#metallicity-distribution-function), stars formed while the gas fraction falls by $-d\mu$ have probability $dP=-d\mu/\delta_f$. Writing their individual abundance as $z=1-\mu^Y$ gives $\mu=(1-z)^{1/Y}$ and the [change of variables](../../../calculus.md#change-of-variables-formula)

$$
\boxed{dP=F(z)\,dz,\qquad F(z)=\frac{(1-z)^{1/Y-1}}{Y(1-\mu_f)},\quad 0<z<1-\mu_f^Y.}
$$

The density is zero outside this interval. Its cumulative probability is $[1-(1-z)^{1/Y}]/(1-\mu_f)$, so it integrates to one; integrating $zF(z)$ reproduces $f(\mu_f)$. A star-count distribution has the same form if the [initial mass function](../../../stellar-astrophysics.md#initial-mass-function) and survival selection give a fixed number of observed stars per unit locked mass. Luminosity-weighted samples require different weights.

For trace abundances, $(1-z)^{1/Y-1}\simeq e^{-z/Y}$ to leading order at fixed $z/Y$. The corresponding ordinary [closed-box metallicity distribution](../../../galaxy.md#closed-box-metallicity-distribution) is

$$
F_{\rm trace}(z)=\frac{e^{-z/Y}}{Y(1-\mu_f)},\qquad 0<z<-Y\log\mu_f.
$$

In the early-consumption regime $z_f\ll Y$, this becomes approximately uniform, $F\simeq1/(Y\delta_f)$ on $[0,Y\delta_f]$. Its mean is half its upper endpoint, again producing the corrected maximum $2Z_\odot$.

If the supplied $f(\mu)$ is instead retained literally as the individual birth abundance, set $q=f(\mu)$ rather than $z=1-\mu^Y$. The observation-time population mean is then $\delta_f^{-1}\int_{\mu_f}^1 f(u)\,du$, not $f(\mu_f)$. Its exact distribution can be specified parametrically using

$$
\frac{df}{d\delta}=\frac{1-\mu^Y-f(\mu)}{1-\mu}>0,\qquad
\boxed{F_{\rm literal}(f(\mu))=\frac{1-\mu}{(1-\mu_f)[1-\mu^Y-f(\mu)]},\quad \mu_f<\mu<1.}
$$

Positivity follows because $f$ is the average of the increasing function $1-(1-\delta)^Y$. Its support is $0<q<f(\mu_f)$, and normalization follows directly from $dP=d\delta/\delta_f$. At early consumption it is uniform with $F_{\rm literal}\simeq2/(Y\delta_f)$, maximum $Y\delta_f/2$ and mean $Y\delta_f/4$. Even this literal alternative gives maximum twice the population mean, never half. **The distinction between birth abundance and cumulative mean resolves the calculation; the printed inverse maximum-to-mean ratio is false under either interpretation.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
