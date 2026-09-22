# Paper 57

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_57.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_57.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
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
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Use signature $(-,+,+,+)$ and write $h_{ij}$ for the spatial [induced metric](../../../riemannian-geometry.md#induced-metric), $D_i$ for its [spatial covariant derivative](../../../numerical-relativity.md#spatial-covariant-derivative), and $q^2=h^{ij}D_i\phi D_j\phi$. The negative [shift vector](../../../numerical-relativity.md#shift-vector) convention gives $n^\mu=N^{-1}(1,N^i)$ and $\Pi=n^\mu\partial_\mu\phi$. Decomposing the [scalar field](../../../quantum-field-theory.md#scalar-field) derivative gives

$$
\partial_\mu\phi=-n_\mu\Pi+D_\mu\phi,\qquad g^{\mu\nu}\partial_\mu\phi\partial_\nu\phi=-\Pi^2+q^2.
$$

Varying the [scalar field](../../../quantum-field-theory.md#scalar-field) matter [action](../../../classical-mechanics.md#action) with respect to the inverse [metric tensor](../../../general-relativity.md#metric-tensor), including the variation of $\sqrt{-g}$, gives the [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor)

$$
\boxed{T_{\mu\nu}=\partial_\mu\phi\partial_\nu\phi-g_{\mu\nu}\left[\tfrac12g^{\alpha\beta}\partial_\alpha\phi\partial_\beta\phi+V\right].}
$$

Raising both indices gives the requested $T^{\mu\nu}$. Contracting with the [unit normal](../../../differential-geometry.md#unit-normal) twice, or once with the [spatial projection tensor](../../../numerical-relativity.md#spatial-projection-tensor), gives

$$
\boxed{\rho=\tfrac12\Pi^2+\tfrac12q^2+V=N^2T^{00},\qquad \mathcal J_i=-\Pi D_i\phi.}
$$

Projecting both indices of the [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) onto the spatial hypersurface gives

$$
S_{ij}=D_i\phi D_j\phi+h_{ij}\left(\tfrac12\Pi^2-\tfrac12q^2-V\right),\qquad
\boxed{S=\tfrac32\Pi^2-\tfrac12q^2-3V,\quad \widetilde S_{ij}=D_i\phi D_j\phi-\tfrac13h_{ij}q^2.}
$$

**Two printed identifications require correction.** The [canonical momentum](../../../classical-mechanics.md#canonical-momentum) of the displayed density is $\pi_\phi=\sqrt h\,\Pi$, not $\Pi$: explicitly $\mathcal L_m=N\sqrt h[\Pi^2/2-q^2/2-V]$ and differentiation with respect to $\dot\phi$ supplies $\sqrt h$. Thus $\Pi$ is the [normal scalar-field momentum](../../../numerical-relativity.md#normal-scalar-field-momentum). Also, the printed trace-free stress has an extra factor $1/2$ and uses $\delta_{ij}$ where the general spatial [induced metric](../../../riemannian-geometry.md#induced-metric) requires $h_{ij}$. In an orthonormal spatial frame the latter becomes $\delta_{ij}$, but the coefficient is still one. For a gradient $(q,0,0)$ in that frame, direct projection gives $\widetilde S_{11}=2q^2/3$, rather than the printed $q^2/3$. The PDF's energy-density gradient is spatial $\partial_i\phi\partial^i\phi$; the TeX aid's spacetime index there is an OCR defect.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [unimodular spatial metric](../../../numerical-relativity.md#unimodular-spatial-metric) separates volume from shape: writing $h_{ij}=a^2\widetilde h_{ij}$ and $a^6=h=\det h_{ij}$ gives $\det\widetilde h=1$. Contract the [extrinsic curvature with a negative shift](../../../numerical-relativity.md#extrinsic-curvature-with-a-negative-shift) with $h^{ij}$. [Metric compatibility](../../../fiber-bundle.md#metric-compatibility) and the [Jacobi determinant derivative formula](../../../linear-algebra.md#jacobi-determinant-derivative-formula) give

$$
h^{ij}\dot h_{ij}=\partial_t\log h,\qquad h^{ij}(D_iN_j+D_jN_i)=2D_iN^i.
$$

Consequently

$$
\boxed{K=-\frac1{2N}\left(\frac{\dot h}{h}+2D_iN^i\right).}
$$

For zero [shift vector](../../../numerical-relativity.md#shift-vector), $\dot h/h=6\dot a/a$, so

$$
\boxed{H=-K/3=\dot a/(Na).}
$$

The infinitesimal spatial volume is $\sqrt h\,d^3x=a^3d^3x$; its logarithmic change per unit normal [proper time](../../../special-relativity.md#proper-time) is $3H$. Thus this $H$ is the [local volume Hubble parameter](../../../cosmology.md#local-volume-hubble-parameter), reducing to the usual [Hubble parameter](../../../cosmology.md#hubble-parameter) in a homogeneous universe. The determinant-defined $a$ refers to fixed spatial coordinates, while this normal volume expansion has a geometric interpretation.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Retain zeroth and first spatial-gradient orders in the [long-wavelength approximation in cosmology](../../../cosmology.md#long-wavelength-approximation-in-cosmology). Spatial [Ricci curvature](../../../second-fundamental-form.md#ricci-curvature), $D_iD_jN$, $q^2$ and scalar [anisotropic stress](../../../general-relativity.md#anisotropic-stress) are of second gradient order. Put $A^i{}_j=\widetilde K^i{}_j$ and $A^2=A^i{}_jA^j{}_i$. The supplied [Einstein field equations](../../../general-relativity.md#einstein-field-equations) then reduce to

$$
\boxed{6H^2-A^2\simeq8\pi G(\Pi^2+2V),\qquad D_jA^j{}_i+2D_iH\simeq-8\pi G\Pi D_i\phi,}
$$



$$
\boxed{\dot H\simeq N(-3H^2+8\pi GV)=-4\pi GN\Pi^2-\tfrac12NA^2,\qquad \dot A^i{}_j+3NH A^i{}_j\simeq0.}
$$

The [scalar-field stress projections](../../../numerical-relativity.md#scalar-field-stress-projections) show that the [momentum constraint](../../../numerical-relativity.md#momentum-constraint) is a first-gradient equation and must be retained. The square $A^2$ is not a spatial derivative and cannot yet be dropped merely by invoking the [long-wavelength approximation in cosmology](../../../cosmology.md#long-wavelength-approximation-in-cosmology). The time-derivative dot on the trace-free evolution equation is visible in the PDF and missing from the TeX aid.

Using $NH=\dot a/a$, the last equation becomes $\partial_t(a^3A^i{}_j)\simeq0$. Hence

$$
\boxed{\widetilde K^i{}_j\simeq C^i{}_j(\mathbf x)a^{-3},\qquad C^i{}_i=0.}
$$

The time-independent spatial tensor must also satisfy the [momentum constraint](../../../numerical-relativity.md#momentum-constraint) and the symmetry inherited from $K_{ij}$. This is [inflationary shear damping](../../../cosmology.md#inflationary-shear-damping): expanding regions lose anisotropic expansion, without requiring the frozen spatial metric shape to vanish. The matter evolution, useful below, is $\dot\phi=N\Pi$ and $\dot\Pi\simeq-N(3H\Pi+V_{,\phi})$, the leading [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) in each local region.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Now impose the stipulated negligible shear and work where $\Pi\ne0$. The [Hamiltonian constraint](../../../numerical-relativity.md#hamiltonian-constraint), [momentum constraint](../../../numerical-relativity.md#momentum-constraint) and local expansion evolution give

$$
H^2=\frac{8\pi G}{3}(\tfrac12\Pi^2+V),\qquad \partial_iH=-4\pi G\Pi\partial_i\phi,\qquad \dot H=-4\pi GN\Pi^2.
$$

Time differentiation of the first equation, followed by $\dot\phi=N\Pi$, gives $\dot\Pi=-N(3H\Pi+V_{,\phi})$. Spatial differentiation of the same equation and use of the [momentum constraint](../../../numerical-relativity.md#momentum-constraint) gives

$$
\Pi\partial_i\Pi+V_{,\phi}\partial_i\phi=-3H\Pi\partial_i\phi,\qquad
\partial_i\Pi=-(3H+V_{,\phi}/\Pi)\partial_i\phi.
$$

These are the temporal and spatial identities needed for the [nonlinear curvature covector](../../../cosmology.md#nonlinear-curvature-covector). Differentiate its definition, keeping the spatially varying [lapse function](../../../numerical-relativity.md#lapse-function):

$$
\dot\zeta_i=-\partial_i(NH)+\left[-4\pi GN\Pi+\frac{NH(3H\Pi+V_{,\phi})}{\Pi^2}\right]\partial_i\phi+\frac H\Pi\partial_i(N\Pi).
$$

The terms proportional to $\partial_iN$ cancel. The terms $-N\partial_iH$ and $-4\pi GN\Pi\partial_i\phi$ cancel by the [momentum constraint](../../../numerical-relativity.md#momentum-constraint), and the remaining two terms cancel by the spatial momentum identity. Therefore

$$
\boxed{\dot\zeta_i\simeq0}
$$

to the retained gradient order. No homogeneous-lapse assumption was needed.

For linear [adiabatic cosmological perturbations](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions), expansion of the local scale and [scalar field](../../../quantum-field-theory.md#scalar-field) gives $\zeta_i=\partial_i[\Psi+\bar H\delta\phi/\bar\Pi]$. For nonzero spatial modes, linearizing the [Hamiltonian constraint](../../../numerical-relativity.md#hamiltonian-constraint) and the [momentum constraint](../../../numerical-relativity.md#momentum-constraint) gives

$$
\delta\rho=\frac{3\bar H}{4\pi G}\delta H=-3\bar H\bar\Pi\delta\phi,\qquad \bar\rho+\bar P=\bar\Pi^2.
$$

Thus

$$
\boxed{\zeta_i\simeq\partial_i\left[\Psi-\frac{\delta\rho}{3(\bar\rho+\bar P)}\right]=\partial_i\zeta.}
$$

This uses the paper's overall sign for the [uniform-density curvature perturbation](../../../linear-cosmological-perturbation-theory.md#uniform-density-curvature-perturbation); the opposite overall sign is also common. For an adiabatic single-field attractor, [superhorizon conservation of single-field comoving curvature](../../../cosmic-inflation.md#superhorizon-conservation-of-single-field-comoving-curvature) allows the primordial amplitude to be transported through later epochs without following every short-scale process. This proof specifically discarded the shear contribution to the [momentum constraint](../../../numerical-relativity.md#momentum-constraint) and assumed a usable field clock. It is not a claim that every single-field background conserves every curvature mode: [growing curvature perturbation in ultra-slow-roll inflation](../../../cosmic-inflation.md#growing-curvature-perturbation-in-ultra-slow-roll-inflation) is a non-attractor counterexample, and $\Pi=0$ makes this particular covector undefined.

## 2

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Take $w$ constant and $w\ne-1$, with a barotropic perturbation $\delta P=w\delta\rho$. Define the [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) $\delta=\delta\rho/\bar\rho$ and use the scalar [velocity potential](../../../fluid-mechanics.md#velocity-potential) convention $v_i(\mathbf k)=ik_i\theta(\mathbf k)$, so $\partial_iv^i=-k^2\theta$. This $\theta$ is a potential, not the sometimes-used velocity-divergence variable. In [synchronous gauge in cosmology](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology), the inverse metric is $g^{00}=-a^{-2}$ and $g^{ij}=a^{-2}(\delta^{ij}-h^{ij})$ to first order. Discarding products of perturbations in the [perfect fluid in general relativity](../../../general-relativity.md#perfect-fluid-in-general-relativity) gives

$$
\boxed{T^{00}=a^{-2}\bar\rho(1+\delta),\quad T^{0i}=a^{-2}(1+w)\bar\rho\,ik_i\theta,\quad T^{ij}=a^{-2}w\bar\rho[(1+\delta)\delta^{ij}-h^{ij}].}
$$

For the linearization, each $h_{ij}$ must be small: the PDF's determinant condition alone is insufficient, since $h=\operatorname{diag}(L,0,0)$ has zero determinant even for large $L$.

Write $\mathcal H=a'/a$. The time component of [covariant conservation of stress-energy](../../../general-relativity.md#stress-energy-conservation) is

$$
\partial_\mu T^{0\mu}+\Gamma^0_{\mu\nu}T^{\mu\nu}+\Gamma^\mu_{\mu\nu}T^{0\nu}=0.
$$

Here $\Gamma^\mu_{\mu0}=4\mathcal H+h'/2$. To first order, $\Gamma^0_{ij}T^{ij}=a^{-2}w\bar\rho[3\mathcal H(1+\delta)+h'/2]$: the two metric-$h$ contributions cancel. Multiplying the conservation equation by $a^2$, including $\Gamma^0_{00}T^{00}$, gives

$$
\bar\rho'(1+\delta)+\bar\rho\delta'+3\mathcal H(1+w)\bar\rho(1+\delta)-(1+w)\bar\rho k^2\theta+\tfrac12(1+w)\bar\rho h'=0.
$$

The background [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation), $\bar\rho'=-3\mathcal H(1+w)\bar\rho$, cancels the first and third terms. Thus

$$
\boxed{\delta'-(1+w)k^2\theta+\tfrac12(1+w)h'=0.}
$$

The $h'$ term accounts for perturbation of the spatial volume expansion in [synchronous gauge in cosmology](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology). The PDF's correct connection $\Gamma^i_{0j}=\mathcal H\delta^i_j+h'^i{}_j/2$ is garbled in the TeX aid.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

In the decoupled [perfect fluid in general relativity](../../../general-relativity.md#perfect-fluid-in-general-relativity) limit, photons have $w=1/3$ and no [anisotropic stress](../../../general-relativity.md#anisotropic-stress), while cold baryons have $w\simeq0$ with a small pressure correction $c_b^2\delta_b$. The density equations express particle and energy conservation; [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering) transfers momentum rather than leading-order rest-frame energy. The photon Euler equation consequently gains a drag toward the baryon [velocity potential](../../../fluid-mechanics.md#velocity-potential), and the baryon Euler equation gains the equal-and-opposite drag weighted by their inertias.

Let $\Gamma_T=an_e\sigma_T>0$. With the [velocity potential](../../../fluid-mechanics.md#velocity-potential) used in part (i), these forces are $-\Gamma_T(\theta_\gamma-\theta_b)$ and $-R\Gamma_T(\theta_b-\theta_\gamma)$, with $R=4\bar\rho_\gamma/(3\bar\rho_b)$. Multiplication by the photon and baryon enthalpies, $4\bar\rho_\gamma/3$ and $\bar\rho_b$, makes their sum zero. Note that this paper's $R$ is the reciprocal of the usual [baryon loading parameter](../../../cosmic-microwave-background-anisotropy.md#baryon-loading-parameter). [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering) also relaxes the photon quadrupole, giving the $-\Gamma_T\sigma_\gamma$ term in the stipulated simplified hierarchy. This quadrupole is an [anisotropic stress](../../../general-relativity.md#anisotropic-stress), omitted by a perfect-fluid model; finite relaxation creates [Silk damping](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-diffusion-damping).

**The printed baryon density sign and collision normalization are inconsistent with part (i).** The density equation must be $\delta_b'-k^2\theta_b=-h'/2$. As a direct check, with $h'=0$, nonzero common velocity, and initially $\delta_\gamma=4\delta_b/3$, the printed plus sign gives $(\delta_\gamma-4\delta_b/3)'=8k^2\theta/3$, violating the tight-coupling adiabatic condition immediately. Likewise division of the collision forces by $k^2$ belongs to neither this potential convention nor the usual common velocity-divergence convention; the physical relaxation rate is $\Gamma_T$, independent of $k$. Both printed drag terms still cancel in the weighted sum used below, so that particular algebraic combination is unaffected by this normalization error.

For a nonrelativistic distribution, $T^{ij}=\int d^3p\,p^ip^j f/E$ is down by $v^2$ relative to the rest-mass energy density, and the corresponding [anisotropic stress](../../../general-relativity.md#anisotropic-stress) is also suppressed. The streaming terms coupling successive angular moments are proportional to $kv$, and stresses from the velocity distribution disappear in the cold limit. Thus, on scales where velocity dispersion is negligible, density and bulk velocity suffice; the photon [Boltzmann hierarchy](../../../statistical-physics.md#boltzmann-hierarchy) has no analogous small-speed suppression. This argument needs a cold distribution or a controlled small-dispersion approximation. Collisionless nonrelativistic matter with appreciable dispersion or multistreaming need not be an exact perfect fluid, and near photon decoupling the higher photon moments cannot all remain negligible.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Use the corrected baryon density equation from part (ii). Subtracting $4\delta_b'/3$ from the photon equation gives $(\delta_\gamma-4\delta_b/3)'=(4/3)k^2(\theta_\gamma-\theta_b)$. [Tight coupling](../../../cosmic-microwave-background-anisotropy.md#tight-coupling-approximation) therefore preserves [adiabatic initial conditions](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) to leading order: $\theta_b=\theta_\gamma=\theta$ and $\delta_b=3\delta_\gamma/4$.

Multiply the photon Euler equation by the paper's inertia ratio $R$ and add the baryon Euler equation before setting the velocities equal. The [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering) terms cancel exactly. With $\mathcal H=a'/a$ and $c_b^2$ denoting the baryon sound speed, this yields

$$
(1+R)\theta'=-R(\delta_\gamma/4-\sigma_\gamma)-\mathcal H\theta-\tfrac34c_b^2\delta_\gamma.
$$

No derivative of $R$ occurs in this instantaneous weighted addition; writing a derivative of total momentum instead would also differentiate the background inertia. Define the [photon-baryon sound speed](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-sound-speed)

$$
\boxed{\widetilde c_s^2=\frac R{3(1+R)}=\frac1{3[1+3\bar\rho_b/(4\bar\rho_\gamma)]}.}
$$

Then the coupled equations are

$$
\boxed{\delta_\gamma'=\tfrac43k^2\theta-\tfrac23h',\qquad \theta'=-3\widetilde c_s^2(\delta_\gamma/4-\sigma_\gamma)-\frac{3\widetilde c_s^2}{R}(\mathcal H\theta+\tfrac34c_b^2\delta_\gamma).}
$$

The sound speed is radiation pressure divided by the total photon-baryon inertia. Baryons add inertia with little pressure, reducing it below $1/\sqrt3$. The combined formula is meaningful despite the printed collision-factor error because the same erroneous factor cancels; maintenance of the assumed adiabatic relation does require correcting the baryon continuity sign.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

For $R\gg1$, $3\widetilde c_s^2\simeq1$, and the baryon-inertia corrections to the common Euler equation vanish. Differentiating the photon continuity equation gives

$$
\delta_\gamma''=\tfrac43k^2(-\delta_\gamma/4+\sigma_\gamma)-\tfrac23h'',\qquad
\boxed{\delta_\gamma''-\tfrac43k^2\sigma_\gamma+\tfrac13k^2\delta_\gamma=-\tfrac23h''.}
$$

Set aside the gravitational driving terms and balance the quadrupole streaming source against [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering). With $\tau_c=\Gamma_T^{-1}$ and $\sigma_\gamma'\simeq0$,

$$
\sigma_\gamma\simeq-\tfrac4{15}\tau_ck^2\theta_\gamma=-\tfrac15\tau_c\delta_\gamma',\qquad
\boxed{\delta_\gamma''+\tfrac4{15}\tau_ck^2\delta_\gamma'+\tfrac13k^2\delta_\gamma=0.}
$$

The positive friction is [Silk damping](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-diffusion-damping); this particular truncation gives [shear-only photon diffusion damping](../../../cosmic-microwave-background-anisotropy.md#shear-only-photon-diffusion-damping). Its coefficient follows the supplied simplified quadrupole equation; adding polarization and the full velocity-slip correction changes that coefficient, as in the general [photon-baryon diffusion damping equation](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-diffusion-damping-equation).

For completeness, put $\omega_0=k/\sqrt3$, $b=4k^2\tau_c/15$ and $D=\tfrac12\int_{\tau_0}^\tau b(s)ds$. Substitution $\delta_\gamma=e^{-D}y$ gives the exact transformed equation

$$
y''+\left(\omega_0^2-\tfrac12b'-\tfrac14b^2\right)y=0.
$$

For constant $\tau_c$ the two independent solutions are $e^{-b(\tau-\tau_0)/2}\cos[\sqrt{\omega_0^2-b^2/4}(\tau-\tau_0)]$ and the corresponding sine. Their frequency correction begins at second order in $\tau_c$. For variable $\tau_c$, retaining first order alone does not automatically remove $b'/2$: a general first-order representation is

$$
y(\tau)=y_0(\tau)+\frac1{2\omega_0}\int_{\tau_0}^{\tau}\sin[\omega_0(\tau-s)]b'(s)y_0(s)ds+O(\tau_c^2),\quad y_0=A\cos[\omega_0(\tau-\tau_0)]+B\sin[\omega_0(\tau-\tau_0)].
$$

The intended cosmological approximation additionally uses slow variation on an acoustic period, $\mathcal H/k\ll1$, with tight coupling $k\tau_c\ll1$. Then the $b'$ correction to the frequency is subleading and the two independent [photon-baryon acoustic oscillator](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-acoustic-oscillator) solutions take the resummed damping form

$$
\boxed{\delta_\gamma(\mathbf k,\tau)\simeq[A(\mathbf k)\cos(k\tau/\sqrt3)+B(\mathbf k)\sin(k\tau/\sqrt3)]e^{-k^2/k_D^2(\tau)},\qquad k_D^{-2}(\tau)=\frac2{15}\int_{\tau_0}^{\tau}\tau_c(s)ds.}
$$

A shift of the time origin is absorbed in $A,B$. If the ionization fraction is constant, $n_e\propto a^{-3}$ gives $\tau_c\propto a^2\propto\tau^4$ during matter domination, and an initial origin at zero gives $k_D^{-2}=2\tau\tau_c/75$. Across recombination the ionization fraction varies, so the integral is the general answer. The PDF prints $O(\tau_c^{-2})$, while the TeX aid prints $O(\tau_c^2)$; the small-mean-free-time expansion requires the latter interpretation.

The intrinsic photon temperature fluctuation is $\delta T/T=\delta_\gamma/4$. The cosine and sine produce the [Cosmic microwave background acoustic peaks](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-acoustic-peak); the envelope suppresses their small-scale amplitudes. The corresponding contribution to the [Cosmic microwave background power spectrum](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-power-spectrum) contains $e^{-2k^2/k_D^2}$, before angular projection and the other temperature sources are included. Thus [Silk damping](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-diffusion-damping) erases the high-multipole acoustic structure progressively rather than shifting every peak to a new frequency.

## 3

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $X=\partial^{-2}\zeta$, with an inverse spatial [Laplacian](../../../calculus.md#laplacian) defined by a boundary or zero-mode prescription. It depends on $\zeta$, not on its time derivative. Differentiation gives the [canonical momentum](../../../classical-mechanics.md#canonical-momentum)

$$
\boxed{\pi=\dot\zeta+3\alpha\dot\zeta^2+2\gamma X\dot\zeta.}
$$

Count $\zeta,\pi,X$ as first order. Inverting perturbatively gives

$$
\dot\zeta=\pi-3\alpha\pi^2-2\gamma X\pi+O(\zeta^3).
$$

For the [Legendre transform in mechanics](../../../classical-mechanics.md#legendre-transform-in-mechanics), write $v=\dot\zeta=\pi+\Delta$ with $\Delta$ second order. The quadratic kinetic contribution is $\pi v-v^2/2=\pi^2/2-\Delta^2/2$, whose correction is fourth order; in the cubic terms one may consequently replace $v$ by $\pi$. The [Hamiltonian](../../../classical-mechanics.md#hamiltonian) density is therefore

$$
\boxed{\mathcal H=\tfrac12\pi^2+\tfrac12(\partial\zeta)^2-\alpha\pi^3-\beta\zeta(\partial\zeta)^2-\gamma(\partial^{-2}\zeta)\pi^2+O(\zeta^4).}
$$

The cubic [interaction Hamiltonian](../../../quantum-field-theory.md#interaction-hamiltonian) density is

$$
\boxed{\mathcal H_{\rm int}=-\alpha\pi^3-\beta\zeta(\partial\zeta)^2-\gamma(\partial^{-2}\zeta)\pi^2.}
$$

In the free [interaction picture](../../../quantum-mechanics.md#interaction-picture), $\pi_I=\dot\zeta_I$. Thus here $\mathcal H_{\rm int}=-\mathcal L_3$ with the time derivatives interpreted as free fields. This equality follows from the [cubic Legendre transform for scalar derivative interactions](../../../quantum-field-theory.md#cubic-legendre-transform-for-scalar-derivative-interactions); at higher orders additional terms can appear.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a statistically homogeneous isotropic dimensionless field, write its two-point [autocorrelation function of a random field](../../../stochastic-process.md#autocorrelation-function-of-a-random-field) as $C(r)$ and

$$
C(r)=\int\frac{d^3k}{(2\pi)^3}P(k)e^{i\mathbf k\cdot\mathbf r}.
$$

The formal real-space [scale invariance](../../../mathematics.md#scale-invariance) condition is $C(\lambda\mathbf r)=C(\mathbf r)$ for all $\lambda>0$. Changing variable $\mathbf q=\lambda\mathbf k$ in the first expression and equating the nonzero-mode [Fourier transforms](../../../analysis.md#fourier-transform) gives $\lambda^{-3}P(q/\lambda)=P(q)$, equivalently $P(\lambda k)=\lambda^{-3}P(k)$. Taking $\lambda=k/k_0$ yields

$$
\boxed{P(k)=A/k^3,\qquad \Delta^2(k)=k^3P(k)/(2\pi^2)=A/(2\pi^2).}
$$

Thus a [scale-invariant inflationary power spectrum](../../../cosmic-inflation.md#scale-invariant-inflationary-power-spectrum) has equal [variance](../../../variance.md) per logarithmic [wavenumber](../../../wave-equation.md#wavenumber) interval, rather than equal power per Fourier volume.

There is an important mathematical qualification to the literal [covariance](../../../variance.md#covariance) condition. A nonzero $k^{-3}$ [power spectrum](../../../probability-and-statistics.md#power-spectrum) over all scales has $C(0)=A\int dk/k/(2\pi^2)$, divergent at both endpoints; it is not the [covariance](../../../variance.md#covariance) of a finite-variance ordinary field. Moreover, exact dilation invariance of a continuous isotropic $C(r)$ makes it constant for $r>0$ and, by continuity, at zero: its spectrum can then consist only of a zero-mode delta measure. The nontrivial cosmological statement consequently concerns nonzero modes, with cutoffs or subtraction of an unobservable constant. For example the finite subtracted [covariance](../../../variance.md#covariance)

$$
C(r)-C(r_0)=\frac A{2\pi^2}\int_0^\infty\frac{dk}{k}\left[\frac{\sin kr}{kr}-\frac{\sin kr_0}{kr_0}\right]= -\frac A{2\pi^2}\log(r/r_0)
$$

is invariant under simultaneous rescaling of $r,r_0$. This is the precise [infrared qualification of a scale-invariant covariance](../../../cosmic-inflation.md#infrared-qualification-of-a-scale-invariant-covariance); a regulated unsubtracted $C(r)$ generally shifts by an additive constant under dilation. The formal derivation above gives the intended nonzero-mode scaling, with this qualification rather than an impossible finite-variance premise.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Put $k_1=q\ll k$ and $k_2,k_3\to k$ in the [squeezed bispectrum configuration](../../../cosmology.md#squeezed-bispectrum-configuration). Then $K\to2k$ and the three symmetric combinations in the supplied expression have limits

$$
\sum_i k_i^3\to2k^3,\qquad\sum_{i\ne j}k_i k_j^2\to2k^3,\qquad\sum_{i>j}k_i^2k_j^2\to k^4.
$$

The first two terms inside the $\epsilon$ bracket cancel, leaving $4k^3$. The full bracket is therefore $(\eta+2\epsilon)k^3/4$, and

$$
\boxed{F(q,k,k)\simeq(2\pi)^3\frac{H^4}{16\epsilon^2M_p^4}\frac{\eta+2\epsilon}{q^3k^3}.}
$$

The $(2\pi)^3$ is kept in the normalization of $F$ used by the paper; it should not be introduced a second time by changing the [primordial bispectrum](../../../cosmology.md#primordial-bispectrum) convention.

[Momentum conservation](../../../classical-mechanics.md#momentum-conservation) makes the three vectors close into a triangle. As $q/k\to0$, the two short-wavelength vectors approach equal magnitude and opposite direction, producing a thin, nearly collapsed triangle. In real space the $q$ mode varies slowly over a region containing many short wavelengths, so it modulates their local statistics. For a single adiabatic inflationary clock this is a local spatial dilation, the basis of the [single-field inflation squeezed-limit consistency relation](../../../cosmology.md#single-field-inflation-squeezed-limit-consistency-relation). If $\eta$ is the Hubble-flow convention $\dot\epsilon/(H\epsilon)$, the [scalar spectral index in Hubble slow-roll parameters](../../../cosmic-inflation.md#scalar-spectral-index-in-hubble-slow-roll-parameters) gives $\eta+2\epsilon=1-n_s$ to first order. This identification must not be made with the potential slow-roll $\eta$ without converting conventions.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $G=\Phi_G$ and $f=f_{NL}^{\rm local}$. The [Gaussian random field](../../../stochastic-process.md#gaussian-random-field) [covariance](../../../variance.md#covariance) in Fourier space is

$$
\langle G(\mathbf k)G(\mathbf p)\rangle=(2\pi)^3\delta^3(\mathbf k+\mathbf p)P(k).
$$

The [Fourier transform](../../../analysis.md#fourier-transform) of the centered quadratic term is

$$
Q(\mathbf k)=\int\frac{d^3q}{(2\pi)^3}G(\mathbf q)G(\mathbf k-\mathbf q)-(2\pi)^3\delta^3(\mathbf k)\langle G^2\rangle.
$$

The Gaussian three-point function vanishes. At first order in $f$, the only terms are $f\langle Q_1G_2G_3\rangle$ and its two cyclic placements. For the first, [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) pairs four Gaussian factors in three ways. Pairing the two factors inside $Q_1$ together is canceled by the mean subtraction. Pairing one of those factors with $G_2$ and the other with $G_3$ gives $P(k_2)P(k_3)$ and the overall momentum delta; exchanging the two factors gives the same contribution. Thus

$$
\langle Q_1G_2G_3\rangle=2(2\pi)^3\delta^3(\mathbf k_1+\mathbf k_2+\mathbf k_3)P(k_2)P(k_3).
$$

Adding the three placements gives

$$
\boxed{\langle\Phi_1\Phi_2\Phi_3\rangle_c=2f_{NL}^{\rm local}(2\pi)^3\delta^3(\mathbf k_1+\mathbf k_2+\mathbf k_3)[P(k_1)P(k_2)+P(k_2)P(k_3)+P(k_3)P(k_1)]+O(f^3).}
$$

There is no second-order term because it would contain five centered Gaussian factors. The two-point function receives its first correction at $f^2$, whereas the displayed [local-type primordial non-Gaussianity](../../../cosmology.md#local-type-primordial-non-gaussianity) gives a three-point correlation already at $f$. For $P\propto k^{-3}$ the squeezed limit is $B_\Phi(q,k,k)\simeq4fP(q)P(k)$; this explains the strong correlation between a long potential and short-scale power. A finite [variance](../../../variance.md) or regulator is needed to define the subtracted $\langle G^2\rangle$, as noted in part (b).

## 4

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Use the paper's mode normalization, effectively $M_p=1$, and set $C=\epsilon+1-c_s^2$, $K=k_1+k_2+k_3$, $s_2=k_1k_2+k_1k_3+k_2k_3$, $s_3=k_1k_2k_3$. Write $\langle\zeta_1\zeta_2\zeta_3\rangle_c=(2\pi)^3\delta^3(\sum\mathbf k_i)B$. There are two source consistency issues: the supplied [interaction picture](../../../quantum-mechanics.md#interaction-picture) expansion makes an external-before-vertex [Wick contraction](../../../perturbative-quantum-field-theory.md#wick-contraction) contain $u_k(\tau')$, with positive exponential $e^{ikc_s\tau'}$; it converges at $-\infty(1-i0)$, whereas the PDF prints $-\infty(1+i\varepsilon)$. Also the stated positive interaction has the opposite overall bispectrum sign from the printed target. The following calculation identifies both issues directly.

For the stated mode expansion, the ordered contraction is

$$
\langle\zeta_I(\mathbf k,0)\zeta_I(\mathbf p,\tau')\rangle=(2\pi)^3\delta^3(\mathbf k+\mathbf p)\frac{H^2}{4\epsilon c_s k^3}(1-ikc_s\tau')e^{ikc_s\tau'}.
$$

A spatial derivative at the vertex supplies $ip_j$; the two differentiated legs consequently give $-\mathbf k_i\cdot\mathbf k_j$. There are two [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction) for each choice of the undifferentiated external leg. The extra $a(\tau')$ in the stipulated [in-in formalism](../../../quantum-field-theory.md#keldysh-formalism) integral makes the vertex coefficient $a^2\epsilon C/c_s^2$, using $a^2=1/(H^2\tau'^2)$. This is consistent if the named $H_{\rm int}$ is the cosmic-time generator expressed as a function of $\tau$, since $dt=a\,d\tau$; if it were already the conformal-time generator, that extra $a$ would have to be removed.

For the [spatial-gradient cubic curvature bispectrum](../../../cosmology.md#spatial-gradient-cubic-curvature-bispectrum), define the [late-time scalar gradient vertex integral](../../../quantum-field-theory.md#late-time-scalar-gradient-vertex-integral)

$$
I=\int_{-\infty(1-i0)}^{\tau_f}\frac{d\tau'}{\tau'^2}(1-ic_sk_1\tau')(1-ic_sk_2\tau')(1-ic_sk_3\tau')e^{ic_sK\tau'},\qquad \tau_f\to0^-.
$$

With $\omega=c_sK$, the first two terms of the product obey $(\tau'^{-2}-i\omega\tau'^{-1})e^{i\omega\tau'}=-\partial_{\tau'}(e^{i\omega\tau'}/\tau')$. The other two use $\int_{-\infty}^0e^{i\omega\tau'}d\tau'=-i/\omega$ and $\int_{-\infty}^0\tau'e^{i\omega\tau'}d\tau'=1/\omega^2$, with the same vacuum prescription. The endpoint divergence $-1/\tau_f$ is real, while

$$
\operatorname{Im}I=c_s\left(-K+\frac{s_2}{K}+\frac{s_3}{K^2}\right)=c_s Q.
$$

In particular the finite $-K$ term comes from the endpoint of the total derivative and must not be discarded along with the real divergence.

Let $S=\mathbf k_1\cdot\mathbf k_2+\mathbf k_1\cdot\mathbf k_3+\mathbf k_2\cdot\mathbf k_3$. The ordered vertex expectation, after stripping the momentum delta, is $Z=-2SH^4C I/(64\epsilon^2c_s^5k_1^3k_2^3k_3^3)$. Since $\operatorname{Re}(-2iZ)=2\operatorname{Im}Z$, the literal positive Hamiltonian gives

$$
\boxed{B_{\rm literal}=-\frac{H^4C}{16\epsilon^2c_s^4k_1^3k_2^3k_3^3}\,S\left(-K+\frac{s_2}{K}+\frac{s_3}{K^2}\right).}
$$

**The printed positive-sign target is obtained by replacing the displayed interaction Hamiltonian by its negative**, with the convergent contour above. This is also the expected sign if a positive cubic $\zeta(\partial\zeta)^2$ coefficient was intended as a Lagrangian term, by the [interaction Hamiltonian](../../../quantum-field-theory.md#interaction-hamiltonian) relation proved in question 3(a). Under that explicit repair,

$$
\boxed{B_{\rm intended}=+\frac{H^4C}{16\epsilon^2c_s^4k_1^3k_2^3k_3^3}\,S\left(-K+\frac{s_2}{K}+\frac{s_3}{K^2}\right).}
$$

Restoring the overall $(2\pi)^3\delta^3(\sum\mathbf k_i)$ reproduces all three cyclic terms in the requested expression. An [equilateral bispectrum configuration](../../../cosmology.md#equilateral-bispectrum-configuration) is a concrete sign check: for $k_i=k$, $S=-3k^2/2$, $Q=-17k/9$, so $SQ=17k^3/6>0$. The literal interaction gives $B=-17H^4C/(96\epsilon^2c_s^4k^6)$, while the printed target is positive. This cannot be repaired by merely changing the overall definition of $\zeta$, because its field expansion and interaction were specified together. The contour typo and Hamiltonian sign are therefore documented source repairs, rather than silently altered contractions.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Factor the momentum dependence into

$$
\mathcal G=(2\pi)^3\delta^3(\sum\mathbf k_i)\frac{S}{k_1^3k_2^3k_3^3}\left(-K+\frac{s_2}{K}+\frac{s_3}{K^2}\right).
$$

Write $s=+1$ for the intended target, obtained with the Hamiltonian sign repair in part (i), and $s=-1$ for the literal stated Hamiltonian. The same sign choice applies to both limits and cancels in their amplitude ratio. The [primordial bispectrum](../../../cosmology.md#primordial-bispectrum) contribution is $sH^4(\epsilon+1-c_s^2)\mathcal G/(16\epsilon^2c_s^4)$. Hence

$$
\boxed{c_s^2\to1:\quad\langle\zeta^3\rangle_c\simeq s\frac{H^4}{16\epsilon}\mathcal G,\qquad c_s^2\ll1:\quad\langle\zeta^3\rangle_c\simeq s\frac{H^4(1+\epsilon)}{16\epsilon^2c_s^4}\mathcal G.}
$$

At fixed $H,\epsilon$ and momentum triangle, the ratio to the unit-sound-speed amplitude is

$$
\boxed{\frac{|B(c_s)|}{|B(1)|}=\frac{\epsilon+1-c_s^2}{\epsilon c_s^4}\simeq\frac{101}{c_s^4}\quad(\epsilon=0.01,\ c_s^2\ll1).}
$$

Keeping only the leading slow-roll order makes this $100/c_s^4$. To compare the two pieces of this same interaction at a fixed $c_s$, their ratio is instead $(1-c_s^2)/\epsilon\simeq100(1-c_s^2)$. Thus the noncanonical piece overtakes the slow-roll piece once $1-c_s^2\gg0.01$, while both have the common raw $c_s^{-4}$ enhancement from the interaction and its external mode normalization. For instance $c_s^2=0.1$ gives an exact ratio $9100$ to the canonical limit with these fixed parameters.

A raw [primordial bispectrum](../../../cosmology.md#primordial-bispectrum) amplitude is not the same as normalized [primordial non-Gaussianity](../../../cosmology.md#primordial-non-gaussianity): here $P_\zeta(k)=H^2/(4\epsilon c_sk^3)$, so the ratio $B/P_\zeta^2$ scales as $(\epsilon+1-c_s^2)/c_s^2$ at fixed shape. The small-sound-speed enhancement in normalized non-Gaussianity is therefore $c_s^{-2}$. These are tree-level weak-interaction predictions; approaching arbitrarily small $c_s$ eventually requires checking the perturbative regime.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
