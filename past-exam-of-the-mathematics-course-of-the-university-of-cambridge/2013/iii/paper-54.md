# Paper 54

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_54.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_54.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
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

## 1

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Assume an axisymmetric [thin disc](../../../astrophysics.md#thin-disk) rotating in the fixed potential of a dominant central mass, with $\Omega=(GM_*)^{1/2}r^{-3/2}$ independent of time and height. Neglect vertical mass loss and vertical [angular-momentum flux](../../../classical-mechanics.md#angular-momentum-flux) at the two faces, as well as [self-gravity](../../../classical-mechanics.md#self-gravity) and radial [pressure](../../../thermodynamics.md#pressure) corrections to the rotation law. Define the [surface density](../../../astrophysics.md#surface-density-of-a-disk) and density-weighted [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity) by

$$
\Sigma=\int\rho\,dz,\qquad \bar\nu=\frac1\Sigma\int\rho\nu\,dz,
$$

and let $v_r=\Sigma^{-1}\int\rho u_r\,dz$. These assumptions give the [vertically averaged viscous disk equations](../../../astrophysics.md#vertically-averaged-viscous-disk-equations)

$$
\partial_t\Sigma+\frac1r\partial_r(r\Sigma v_r)=0,\qquad
\partial_t(\Sigma l)+\frac1r\partial_r(r\Sigma v_rl-r^3\bar\nu\Sigma\Omega')=0,
$$

where $l=r^2\Omega$ is [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum). Subtract $l$ times [conservation of mass](../../../continuum-mechanics.md#mass-conservation) from [conservation of angular momentum](../../../classical-mechanics.md#conservation-of-angular-momentum). Since $l$ is fixed in time,

$$
r\Sigma v_r l'=\partial_r(r^3\bar\nu\Sigma\Omega'),\qquad
v_r=-\frac3{\Sigma r^{1/2}}\partial_r(r^{1/2}\bar\nu\Sigma).
$$

Substitution into [conservation of mass](../../../continuum-mechanics.md#mass-conservation) proves the [Keplerian viscous diffusion equation](../../../astrophysics.md#keplerian-viscous-diffusion-equation)

$$
\boxed{\partial_t\Sigma=\frac3r\partial_r\left[r^{1/2}\partial_r(r^{1/2}\bar\nu\Sigma)\right].}
$$

No assumption of height-independent [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity) is needed; its density-weighted average is the one appearing in the integrated stress. A wind or surface magnetic stress would add terms and must not be silently discarded.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $F=\bar\nu\Sigma$. In [steady state](../../../dynamical-systems.md#steady-state), $r^{1/2}\partial_r(r^{1/2}F)$ is constant, so

$$
\boxed{F=A+B r^{-1/2}.}
$$

The inward [mass accretion rate](../../../astrophysics.md#mass-accretion-rate) and outward [viscous torque in an accretion disk](../../../astrophysics.md#viscous-torque-in-an-accretion-disk) are

$$
\dot M=-2\pi r\Sigma v_r=6\pi r^{1/2}\partial_r(r^{1/2}F)=3\pi A,\qquad
\mathcal G=3\pi(GM_*)^{1/2}r^{1/2}F.
$$

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For a [zero-torque inner boundary condition](../../../astrophysics.md#zero-torque-inner-boundary-condition) at finite $r_{\rm in}$,

$$
\boxed{\bar\nu\Sigma=\frac{\dot M}{3\pi}\left(1-\sqrt{\frac{r_{\rm in}}r}\right).}
$$

With positive finite inner [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity), $\Sigma$ tends to zero there. At fixed nonzero inward mass flux, the corresponding $v_r=-\dot M/(2\pi r\Sigma)$ becomes large, signaling the breakdown of the nearly circular [thin disc](../../../astrophysics.md#thin-disk) approximation in the inner transition region.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For no central accretion, $A=0$ and

$$
\boxed{\bar\nu\Sigma=B r^{-1/2},\qquad v_r=0,\qquad\mathcal G=3\pi(GM_*)^{1/2}B.}
$$

This [nonaccreting constant-torque disk](../../../astrophysics.md#nonaccreting-constant-torque-disk) has a finite inner stress and normally a nonzero inner [surface density](../../../astrophysics.md#surface-density-of-a-disk). An external inner [torque](../../../classical-mechanics.md#torque) supplies the [angular momentum](../../../classical-mechanics.md#angular-momentum) transported to an outer sink, although mass does not flow. If both this zero-mass-flux condition and a zero inner [torque](../../../classical-mechanics.md#torque) are imposed, $B=0$; there is no nontrivial positive-viscosity steady disk satisfying both.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The instantaneous [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity) law is $\bar\nu(r,\Sigma)$, with no explicit constitutive memory. Expand its transported quantity at the possibly evolving background:

$$
\bar\nu(r,\Sigma_0+\Sigma_1)(\Sigma_0+\Sigma_1)
=\bar\nu_0\Sigma_0+\left.\partial_\Sigma(\bar\nu\Sigma)\right|_0\Sigma_1+O(\Sigma_1^2).
$$

The [viscous transport response exponent](../../../astrophysics.md#viscous-transport-response-exponent) satisfies $\partial_\Sigma(\bar\nu\Sigma)|_0=q\bar\nu_0$. Subtract the background equation and retain only linear terms to obtain

$$
\boxed{\partial_t\Sigma_1=\frac3r\partial_r\left[r^{1/2}\partial_r(r^{1/2}q\bar\nu_0\Sigma_1)\right].}
$$

This remains a [linear equation](../../../linear-algebra.md#linear-equation) with space- and time-dependent background coefficients; neither a steady background nor constant $q$ is required for this step. The sign of the response coefficient is the [negative-diffusion criterion for viscous disk instability](../../../astrophysics.md#negative-diffusion-criterion-for-viscous-disk-instability).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For $\bar\nu=C r^a\Sigma^b$, the response is $q=b+1$. A nonaccreting background has $\bar\nu_0\Sigma_0\propto r^{-1/2}$, while $\Sigma_0\propto r^{-p}$, so

$$
\boxed{a-(b+1)p=-\tfrac12,\qquad a+\tfrac12=qp.}
$$

Consequently $\bar\nu_0\propto r^{p-1/2}$. On this steady background, introduce the [square-root-radius diffusion transform](../../../astrophysics.md#square-root-radius-diffusion-transform)

$$
x=\sqrt r,\qquad g=\sqrt r\,\bar\nu_0\Sigma_1.
$$

Since $q$ is constant and $\partial_r=(2x)^{-1}\partial_x$, the [linear equation](../../../linear-algebra.md#linear-equation) becomes

$$
\partial_tg=3q\bar\nu_0 r^{-1/2}\partial_r(r^{1/2}\partial_rg)
=\frac{3q\bar\nu_0(r)}{4r}\partial_x^2g.
$$

Thus $A(x)\propto x^{2p-3}$, and the required choice is

$$
\boxed{p=\tfrac32,\qquad a=1+\tfrac32b,\qquad A=\frac{3q}{4}\frac{\bar\nu_0}r=\text{constant}.}
$$

For a [Fourier mode](../../../fourier-analysis.md#fourier-mode) $g\propto e^{\lambda t+ik_xx}$, $\lambda=-Ak_x^2$. Positive [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity) makes $A$ have the sign of $q$, so $q<0$ gives growing modes whose rate increases with $k_x^2$. The formal equation is a [backward heat equation](../../../diffusion-equation.md#backward-heat-equation) and predicts arbitrarily rapid small-scale amplification. Physically the [thin disc](../../../astrophysics.md#thin-disk) diffusion closure applies only to [wavelengths](../../../wave-equation.md#wavelength) sufficiently larger than the thickness and stress-relaxation scales; this formal limit identifies the need for a cutoff, rather than a finite fastest [wavelength](../../../wave-equation.md#wavelength) absent from the model. The boundary case $q=0$ has vanishing linear transport response.

## 2

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a [razor-thin disk](../../../astrophysics.md#razor-thin-disk-approximation), integrate the delta function in height to get

$$
\Phi_\epsilon(\mathbf R)=-G\int\frac{\Sigma(\mathbf R')\,d^2R'}{\sqrt{|\mathbf R-\mathbf R'|^2+\epsilon^2}}.
$$

The corresponding horizontal force kernel is proportional to $(\mathbf R-\mathbf R')/(|\mathbf R-\mathbf R'|^2+\epsilon^2)^{3/2}$. It removes the short-distance point-force singularity and smooths forces on separations of order $\epsilon$. This is [height-evaluation gravitational softening](../../../galaxy.md#height-evaluation-gravitational-softening).

To represent finite vertical thickness, choose $\epsilon$ of order the disc [disk scale height](../../../astrophysics.md#disk-scale-height) $H$. There is no universal exact numerical choice: a true vertical [mass density](../../../fluid-mechanics.md#density) profile produces the Fourier reduction factor $\Sigma^{-1}\int\rho(z)e^{-k|z|}dz$, which is not generally $e^{-k\epsilon}$. Matching the long-wave term gives $\epsilon=\langle|z|\rangle_\rho$, the [vertical-profile softening match](../../../galaxy.md#vertical-profile-softening-match). For an exponential vertical profile this mean is $H$, while its full reduction factor is $(1+kH)^{-1}$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use the horizontal Fourier convention $\widetilde f(\mathbf k)=\int e^{-i\mathbf k\cdot\mathbf R}f(\mathbf R)d^2R$. For each nonzero $k=|\mathbf k|$, the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) becomes

$$
(\partial_z^2-k^2)\widetilde\Phi=4\pi G\widetilde\Sigma\delta(z).
$$

Decay away from the sheet and [continuity](../../../calculus.md#continuous-function) at it give $\widetilde\Phi=C e^{-k|z|}$. Its derivative jump is $-2kC=4\pi G\widetilde\Sigma$, hence the [off-plane razor-thin Poisson kernel](../../../astrophysics.md#off-plane-razor-thin-poisson-kernel) is

$$
\boxed{\widetilde\Phi(\mathbf k,z)=-\frac{2\pi G}{k}\widetilde\Sigma(\mathbf k)e^{-k|z|},\qquad
\widetilde\Phi(\mathbf k,\epsilon)=-\frac{2\pi G}{k}\widetilde\Sigma(\mathbf k)e^{-k\epsilon}.}
$$

The spatially uniform mode has a different vertical solution and an arbitrary additive potential reference; it is not obtained by substituting $k=0$ into this decaying-mode formula.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $k=|k_x|$, $c_s^2=(dP/d\Sigma)_0$ and $\kappa^2=2\Omega(2\Omega-S)$. Linearize the [barotropic closure of a razor-thin disk](../../../astrophysics.md#barotropic-closure-of-a-razor-thin-disk) and [shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-sheet) about the given state. Write the radial and azimuthal [velocity](../../../classical-mechanics.md#velocity) perturbations as $u$ and $v$. [Axisymmetry](../../../calculus.md#axisymmetric-vector-field) removes advection by the background shear, giving

$$
-i\omega\Sigma_1+ik_x\Sigma_0u=0,\qquad
-i\omega u-2\Omega v=-ik_x\left(\Phi_1+\frac{c_s^2\Sigma_1}{\Sigma_0}\right),\qquad
-i\omega v+(2\Omega-S)u=0.
$$

The softened potential is $\Phi_1=-2\pi G\Sigma_1e^{-k\epsilon}/k$. Eliminating the [velocity](../../../classical-mechanics.md#velocity) components for the compressive branch gives the [softened Toomre dispersion relation](../../../gravitational-instability-of-an-astrophysical-disk.md#softened-toomre-dispersion-relation)

$$
\boxed{\omega^2=\kappa^2-2\pi G\Sigma_0k e^{-k\epsilon}+c_s^2k^2.}
$$

The Coriolis/shear combination supplies the radial epicyclic restoring term, [pressure](../../../thermodynamics.md#pressure) supplies the short-wave term, and [self-gravity](../../../classical-mechanics.md#self-gravity) lowers the squared frequency. The full three-variable determinant also has a stationary [axisymmetric geostrophic mode](../../../gravitational-instability-of-an-astrophysical-disk.md#axisymmetric-geostrophic-mode), with $u=0$ and azimuthal flow balancing the pressure-plus-gravity gradient. The displayed relation describes the density-wave pair; eliminating by division by $\omega$ must not silently deny that stationary mode.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Assume $\kappa,c_s,\Sigma_0>0$, and use the positive [Toomre parameter](../../../gravitational-instability-of-an-astrophysical-disk.md#toomre-parameter). The dimensionless dispersion relation is

$$
\frac{\omega^2}{\kappa^2}=1+\frac{s^2-2se^{-\delta s}}{Q^2}.
$$

At fixed dimensionless [gravitational softening](../../../galaxy.md#gravitational-softening) $\delta$, maximum growth corresponds to maximizing $F(s)=2se^{-\delta s}-s^2$. Differentiating gives the [most unstable softened disk wavenumber](../../../gravitational-instability-of-an-astrophysical-disk.md#most-unstable-softened-disk-wavenumber)

$$
\boxed{s_*=e^{-\delta s_*}(1-\delta s_*).}
$$

For $\delta>0$, the right side is strictly decreasing on $0<s<1/\delta$, while the left side increases; there is exactly one positive solution. The equation implies $\delta s_*<1$ and $s_*<1-\delta s_*$, so

$$
\boxed{s_*<\frac1{1+\delta}.}
$$

Instability occurs precisely when $Q^2<F(s_*)$. Thus the [critical Toomre parameter with exponential softening](../../../gravitational-instability-of-an-astrophysical-disk.md#critical-toomre-parameter-with-exponential-softening) is

$$
\boxed{Q_c^2=2s_*e^{-\delta s_*}-s_*^2=s_*^2\frac{1+\delta s_*}{1-\delta s_*},\qquad Q<Q_c\ \text{is unstable}.}
$$

The printed description of a minimum $Q$ for instability reverses the threshold: $Q_c$ is the upper boundary of unstable values and the lower boundary of stable ones. Because $s_*<1/(1+\delta)\le1$ and $2s-s^2$ increases on $[0,1]$,

$$
Q_c^2<2s_*-s_*^2<\frac2{1+\delta}-\frac1{(1+\delta)^2}
=\frac{1+2\delta}{(1+\delta)^2}\le1.
$$

Both strict comparisons become equality in the unsoftened limit $\delta=0$: then $s_*=1$ and $Q_c=1$. [Gravitational softening](../../../galaxy.md#gravitational-softening) suppresses short-wave gravity, shifts the most dangerous mode to a longer [wavelength](../../../wave-equation.md#wavelength) and requires stronger [self-gravity](../../../classical-mechanics.md#self-gravity), or smaller $Q$, for instability.

<a id="2/d/image-exponential-gravitational-softening-narrows-and-can-remove-the-unstable-density-wave-band"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-54-softened-dispersion.png)

**[Figure 1](#2/d/image-exponential-gravitational-softening-narrows-and-can-remove-the-unstable-density-wave-band). Exponential gravitational softening narrows and can remove the unstable density-wave band**.

The plot holds $Q$ fixed and changes [gravitational softening](../../../galaxy.md#gravitational-softening). If $Q$ is varied physically at fixed $\kappa\epsilon/c_s$, remember $\delta=(\kappa\epsilon/c_s)/Q$: the marginal curve must be evaluated at its corresponding $\delta$, rather than treating these two dimensionless parameters as independently fixed along that physical variation.

## 3

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The conventional complete-flyby [impulse approximation](../../../galaxy.md#impulse-approximation) uses a straight incoming path $x=x_0$, $y=-Sx_0t$, with $S>0$. Integrate the satellite's transverse acceleration over the whole encounter. For $x_0>0$,

$$
\Delta v_x=-\frac{GM_s}{x_0^2}\int_{-\infty}^{\infty}(1+S^2t^2)^{-3/2}dt
=-\frac{2GM_s}{Sx_0^2}.
$$

The hint's integral is one over a half encounter, and two over the full encounter. The leading longitudinal impulse vanishes by oddness. In weak elastic scattering, conservation of the relative speed $V=S|x_0|$ gives the next-order change along the original [velocity](../../../classical-mechanics.md#velocity) as $-\Delta v_x^2/(2V)$. With the original outer flow along negative $y$, this means

$$
\boxed{\Delta v_y\simeq\frac{2(GM_s)^2}{S^3x_0^5}.}
$$

The same signed expression holds for inner particles and has the opposite sign there. This is the [complete-flyby gravitational impulse](../../../galaxy.md#complete-flyby-gravitational-impulse). Its weak-deflection requirement is $GM_s/(S^2|x_0|^3)\ll1$. Rotation and tidal dynamics retained throughout the encounter give a more detailed response; this impulse model does not claim to solve the full Hill scattering problem exactly.

The printed coefficient $1/2$ is four times smaller than this complete-flyby value. It is obtained if the single-sided transverse impulse $GM_s/(Sx_0^2)$ is inserted into the same quadratic longitudinal estimate, leaving out the other half. Thus the scaling and sign agree, but that numerical coefficient is not derived by the usual full-encounter prescription. To keep the subsequent requested formulas unambiguous, write the [satellite impulse normalization](../../../galaxy.md#satellite-impulse-normalization)

$$
\Delta v_y=\chi\frac{(GM_s)^2}{S^3x_0^5}:
\qquad\chi=\tfrac12\ \text{for the supplied model},\quad\chi=2\ \text{for the complete-flyby model}.
$$

The following parts are derived for general $\chi$ and specialize to the supplied value. The complete-flyby one-sided [torque](../../../classical-mechanics.md#torque) coefficient $8/27$ is also the normalization used in [the primary coplanar impulse calculation summarized by Chametla and collaborators](https://academic.oup.com/mnras/article/468/4/4610/3098191).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A strip $dx$ at $x>0$ passes the satellite at relative speed $Sx$, so its encounter mass flux is $Sx\Sigma(x)dx$. Each unit mass gains [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum) $r_0\Delta v_y$. Therefore the [one-sided impulse torque on a disk](../../../galaxy.md#one-sided-impulse-torque-on-a-disk) is

$$
\Gamma_{>0}=\chi\frac{r_0(GM_s)^2}{S^2}\int_H^\infty\frac{\Sigma(x)}{x^4}dx.
$$

Putting $\chi=1/2$ gives exactly the requested expression. Inner strips have the opposite signed impulse but the same positive encounter flux. The net disc [torque](../../../classical-mechanics.md#torque) is consequently

$$
\boxed{\Gamma=\chi\frac{r_0(GM_s)^2}{S^2}\int_H^\infty\frac{\Sigma(x)-\Sigma(-x)}{x^4}dx.}
$$

An even [surface density](../../../astrophysics.md#surface-density-of-a-disk) makes the integrand vanish pointwise, so the total [torque](../../../classical-mechanics.md#torque) is zero although each one-sided [torque](../../../classical-mechanics.md#torque) can be nonzero. The cutoff must keep the encounters in the weak-deflection regime; an appropriate physical value is at least of order the thickness or the relevant strong-scattering radius. The infinite-sheet integral also assumes convergence or a specified outer truncation.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The odd [mass density](../../../fluid-mechanics.md#density) difference is $2\Sigma_0\beta x/r_0$. Integrating $x^{-3}$ from $H$ to infinity gives

$$
\Gamma=\chi\frac{\beta\Sigma_0(GM_s)^2}{S^2H^2}.
$$

For [Keplerian shear](../../../planetary-science.md#keplerian-shear), $S=3\Omega/2$ and $GM_s=q\Omega^2r_0^3$. Thus the [density-slope satellite torque](../../../galaxy.md#density-slope-satellite-torque) is

$$
\Gamma=\frac{4\chi}{9}\,\beta\frac{q^2}{(H/r_0)^2}\Sigma_0r_0^4\Omega^2,
\qquad
\boxed{\Gamma=\frac29\,\beta\frac{q^2}{(H/r_0)^2}\Sigma_0r_0^4\Omega^2\quad(\chi=\tfrac12).}
$$

Using the complete-flyby normalization multiplies this supplied-model result by four. The linear [mass density](../../../fluid-mechanics.md#density) law is a local Taylor approximation, not a nonnegative [mass density](../../../fluid-mechanics.md#density) on the entire infinite real line. With an outer local cutoff $L\gg H$, the same calculation replaces $H^{-2}$ by $H^{-2}-L^{-2}$; the extension to infinity is the leading local result. Small $|\beta|H/r_0$ keeps the [mass density](../../../fluid-mechanics.md#density) perturbation small in the dominant encounter region.

Outer particles gain [angular momentum](../../../classical-mechanics.md#angular-momentum) and inner particles lose it. The satellite transmits [angular momentum](../../../classical-mechanics.md#angular-momentum) from inner to outer material. If $\beta>0$, the denser outer side receives the larger [torque](../../../classical-mechanics.md#torque): the disc gains net [angular momentum](../../../classical-mechanics.md#angular-momentum) and the satellite loses it. If $\beta<0$, the net transfer reverses. At zero slope these exchanges cancel in the satellite's total [torque](../../../classical-mechanics.md#torque).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For a fixed satellite mass on an adiabatically changing [circular orbit](../../../classical-mechanics.md#circular-orbit), $L_s=M_s\sqrt{GM_*r_0}=M_sr_0^2\Omega$. The satellite [torque](../../../classical-mechanics.md#torque) is minus the disc [torque](../../../classical-mechanics.md#torque). Hence

$$
\frac12M_sr_0\Omega\frac{dr_0}{dt}=-\Gamma,\qquad
\frac{dr_0}{dt}=-\frac{8\chi}{9}\,\beta q\frac{\Sigma_0r_0^2}{M_*}\frac{r_0\Omega}{(H/r_0)^2}.
$$

The [circular-orbit migration rate from disk torque](../../../planetary-science.md#circular-orbit-migration-rate-from-disk-torque), in the normalization supplied by the question, is

$$
\boxed{\frac{dr_0}{dt}=-\frac49\,\beta q\frac{\Sigma_0r_0^2}{M_*}\frac{r_0\Omega}{(H/r_0)^2}.}
$$

It is inward for a positive [mass density](../../../fluid-mechanics.md#density) slope and outward for a negative one. The complete-flyby normalization makes its magnitude four times larger, with the same direction. This is a local [torque](../../../classical-mechanics.md#torque) estimate; the hypothesis of a nearly circular slowly migrating orbit is needed when using the derivative of the circular [angular momentum](../../../classical-mechanics.md#angular-momentum).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
