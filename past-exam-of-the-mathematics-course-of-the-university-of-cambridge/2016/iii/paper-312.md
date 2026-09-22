# Paper 312

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_312.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_312.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Write $h_{ij}$ for the spatial [metric tensor](../../../general-relativity.md#metric-tensor) and lower the [shift vector](../../../numerical-relativity.md#shift-vector) with $h_{ij}$. For the negative-shift convention, the four-dimensional metric and its inverse have components

$$
g_{00}=-N^2+N_iN^i,\quad g_{0i}=-N_i,\quad g_{ij}=h_{ij},\qquad g^{00}=-N^{-2},\quad g^{0i}=-N^iN^{-2}.
$$

The normal has covariant components $n_\mu=(-N,0,0,0)$, so $n_\mu n^\mu=-1$ and it annihilates every tangent vector to the spatial slice. Since $n_i=0$, its [covariant derivative](../../../general-relativity.md#covariant-derivative) gives $n_{i;j}=N\Gamma^0{}_{ij}$ and therefore $K_{ij}=-N\Gamma^0{}_{ij}$.

Compute the required [Christoffel symbol](../../../riemannian-geometry.md#christoffel-symbol) using the symmetric connection formula. Its time-index term and spatial-index term combine to give

$$
\Gamma^0{}_{ij}=\frac{1}{2N^2}\left(\dot h_{ij}+\partial_iN_j+\partial_jN_i-N^k(\partial_i h_{jk}+\partial_jh_{ik}-\partial_kh_{ij})\right).
$$

The spatial expression in parentheses is $\dot h_{ij}+D_iN_j+D_jN_i$, where $D$ is the [covariant derivative](../../../general-relativity.md#covariant-derivative) of $h$. Thus the [extrinsic curvature with a negative shift](../../../numerical-relativity.md#extrinsic-curvature-with-a-negative-shift) is

$$
\boxed{K_{ij}=-\frac{1}{2N}(\dot h_{ij}+D_iN_j+D_jN_i).}
$$

This derivation fixes both signs from the actual [3+1 decomposition of spacetime](../../../numerical-relativity.md#3-plus-1-decomposition-of-spacetime), rather than transferring a formula using the opposite [shift vector](../../../numerical-relativity.md#shift-vector) convention. The connection formula used here has $g_{\lambda\kappa,\nu}$ as its second differentiated term; the printed repeated-index version is a typographical error.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Set $h=\det h_{ij}$. Contract the [extrinsic curvature with a negative shift](../../../numerical-relativity.md#extrinsic-curvature-with-a-negative-shift) with $h^{ij}$. The [Jacobi determinant derivative formula](../../../linear-algebra.md#jacobi-determinant-derivative-formula) and metric compatibility give

$$
h^{ij}\dot h_{ij}=\partial_t\ln h=\frac{\dot h}{h},\qquad h^{ij}D_iN_j=D_iN^i.
$$

Consequently

$$
\boxed{K=-\frac{1}{2N}\left(\frac{\dot h}{h}+2D_iN^i\right).}
$$

The local volume element is $\sqrt h\,d^3x$, so for zero [shift vector](../../../numerical-relativity.md#shift-vector) the proper-time derivative along the normal is $d/ds=N^{-1}\partial_t$ and

$$
\theta=\frac1N\partial_t\ln\sqrt h=-K.
$$

Here $\theta$ is the [expansion scalar](../../../geodesic-congruence.md#expansion-scalar). Writing $a_{\mathrm{loc}}=h^{1/6}$ defines a local linear scale from this volume, whence the [local volume Hubble parameter](../../../cosmology.md#local-volume-hubble-parameter) is

$$
\boxed{H_{\mathrm{loc}}=\frac{1}{a_{\mathrm{loc}}}\frac{da_{\mathrm{loc}}}{ds}=\frac{\dot a_{\mathrm{loc}}}{Na_{\mathrm{loc}}}=-\frac K3.}
$$

The factor of three converts volume expansion into linear expansion, and $N$ converts coordinate time into proper time. This agrees with the usual [Hubble parameter](../../../cosmology.md#hubble-parameter) in a homogeneous [FLRW metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric).

For a volume-shape decomposition the [unimodular spatial metric](../../../numerical-relativity.md#unimodular-spatial-metric) is $\gamma_{ij}=a_{\mathrm{loc}}^{-2}h_{ij}$, with determinant one. If instead the printed positive power $a_{\mathrm{loc}}^2h_{ij}$ is taken literally, its determinant is $a_{\mathrm{loc}}^{12}$; it is a conformal rescaling but not the unimodular shape metric. The trace calculation does not need that rescaling.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Decompose the mixed [extrinsic curvature of a spatial hypersurface](../../../numerical-relativity.md#extrinsic-curvature-of-a-spatial-hypersurface) into $K^i{}_j=\tfrac13K\delta^i{}_j+\widetilde K^i{}_j$. In the [long-wavelength approximation in cosmology](../../../cosmology.md#long-wavelength-approximation-in-cosmology), the [inflationary shear damping](../../../cosmology.md#inflationary-shear-damping) law makes $\widetilde K^i{}_j$ fall as the inverse local volume. During [cosmic inflation](../../../cosmic-inflation.md), many e-folds therefore suppress the anisotropic expansion, while $K$ still measures the local isotropic expansion through the [local volume Hubble parameter](../../../cosmology.md#local-volume-hubble-parameter).

Neglecting spatial gradients at leading order gives approximately independent expanding patches. Restrict also to [scalar cosmological perturbations](../../../linear-cosmological-perturbation-theory.md#scalar-cosmological-perturbation), and neglect the independent frozen [tensor cosmological perturbation](../../../linear-cosmological-perturbation-theory.md#tensor-cosmological-perturbation). The remaining spatial scale can be written as a background scale times a local fluctuation:

$$
a_{\mathrm{loc}}(t,\mathbf x)=a_{\mathrm{bg}}(t)e^{\zeta(t,\mathbf x)},\qquad h_{ij}=a_{\mathrm{bg}}^2 e^{2\zeta}\delta_{ij}.
$$

This is the [nonlinear scalar metric in a cosmological gradient expansion](../../../cosmology.md#nonlinear-scalar-metric-in-a-cosmological-gradient-expansion). The exponential keeps the metric positive and permits finite $\zeta$; no expansion in its amplitude is needed. Scalar lapse and shift perturbations describe the remaining freedom in time slicing and spatial threading. Choose $N=1+\Psi$ and $N_i=-a_{\mathrm{bg}}^2\partial_iB$. The negative [shift vector](../../../numerical-relativity.md#shift-vector) convention then produces the positive mixed term $2a_{\mathrm{bg}}^2\partial_iB\,dt\,dx^i$.

The exact completed-square form has

$$
g_{00}=-(1+\Psi)^2+h^{ij}N_iN_j=-(1+\Psi)^2+a_{\mathrm{bg}}^2e^{-2\zeta}\delta^{ij}\partial_iB\partial_jB.
$$

The quadratic shift expression must be understood as this norm. If the raised derivative in the displayed ansatz is intended as a flat derivative, the corresponding factors of the spatial scale are needed. In either convention the shift-square term is of second gradient order, and the leading [long-wavelength approximation in cosmology](../../../cosmology.md#long-wavelength-approximation-in-cosmology) is unaffected.

**Damping of shear motivates locally isotropic scalar expansion, not the disappearance of every tensor perturbation.** A time-independent anisotropic shape can survive; the conformally flat scalar ansatz additionally neglects that tensor sector.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use a dot for the coordinate-time derivative and let $\bar N$ be the homogeneous background [lapse function](../../../numerical-relativity.md#lapse-function). The passive linear transformation is $\delta\widetilde g_{\mu\nu}=\delta g_{\mu\nu}-\mathcal L_\xi\bar g_{\mu\nu}$. Its time-time and time-space components yield the [scalar gauge transformations with a background lapse](../../../linear-cosmological-perturbation-theory.md#scalar-gauge-transformations-with-a-background-lapse):

$$
\widetilde\Psi=\Psi-\dot\xi^0-\frac{\dot{\bar N}}{\bar N}\xi^0,\qquad \widetilde B=B+\frac{\bar N^2}{a^2}\xi^0-\dot\lambda.
$$

For example, $\bar g_{00}=-\bar N^2$ gives $-(\mathcal L_\xi\bar g)_{00}=2\bar N\dot{\bar N}\xi^0+2\bar N^2\dot\xi^0$; $\bar g_{0i}=0$ gives $-(\mathcal L_\xi\bar g)_{0i}=\bar N^2\partial_i\xi^0-a^2\partial_i\dot\lambda$. These establish the signs directly.

To preserve [synchronous gauge in cosmology](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology), both transformed quantities must remain zero. Hence

$$
\partial_t(\bar N\xi^0)=0,\qquad\dot\lambda=\frac{\bar N^2}{a^2}\xi^0.
$$

Integrating gives the [residual synchronous-gauge freedom](../../../linear-cosmological-perturbation-theory.md#residual-synchronous-gauge-freedom)

$$
\boxed{\xi^0=\frac{C(\mathbf x)}{\bar N(t)},\qquad\lambda=C(\mathbf x)\int^t\frac{\bar N(t')}{a(t')^2}\,dt'+D(\mathbf x).}
$$

The integration lower limit can be absorbed into $D$. Spatially homogeneous additions to $\lambda$ generate no spatial displacement, so they are physically irrelevant to this scalar parametrization.

The spatial transformation also gives $\widetilde\Phi=\Phi+(\dot a/a)\xi^0$ and $\widetilde E=E+\lambda$. Thus fixing the lapse and shift perturbations does not fix the entire coordinate system; the arbitrary functions $C,D$ can still change the remaining [scalar cosmological perturbations](../../../linear-cosmological-perturbation-theory.md#scalar-cosmological-perturbation).

## 2

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Throughout this question dots denote [conformal time](../../../cosmology.md#conformal-time) derivatives, and $\mathcal H=\dot a/a$ is the [conformal Hubble parameter](../../../cosmology.md#conformal-hubble-parameter). The monopole of the [photon Boltzmann hierarchy](../../../cosmic-microwave-background-anisotropy.md#photon-boltzmann-hierarchy) gives $\dot\Theta_0+k\Theta_1/3=\dot\phi$. With the specified velocity convention, the [photon continuity equation](../../../cosmic-microwave-background-anisotropy.md#photon-continuity-equation) is therefore

$$
\boxed{\dot\delta_\gamma-\frac43kv_\gamma=4\dot\phi.}
$$

The dipole equation is $\dot\Theta_1+k(2\Theta_2/5-\Theta_0)=\dot\tau(\Theta_1+v_b)+k\psi$. Thus the [photon Euler equation](../../../cosmic-microwave-background-anisotropy.md#photon-euler-equation) is

$$
\boxed{\dot v_\gamma+\frac{k}{4}\delta_\gamma-\frac{2k}{5}\Theta_2+k\psi=\dot\tau(v_\gamma-v_b).}
$$

In particular, $\dot\tau<0$ makes the scattering term damp the [photon-baryon velocity slip](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-velocity-slip); it does not amplify it.

The linear momentum density of the [photon-baryon fluid](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-fluid) is weighted by enthalpy, not merely energy density:

$$
q_{\mathrm{tot}}=\frac43\bar\rho_\gamma v_\gamma+\bar\rho_bv_b.
$$

Elastic [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering) exchanges momentum internally. Its [photon](../../../quantum-mechanics.md#photon) force density is $(4\bar\rho_\gamma/3)\dot\tau(v_\gamma-v_b)$, so the [baryon](../../../physics.md#baryon) force density is its negative. Dividing by $\bar\rho_b$ gives the [baryon Euler equation with Thomson drag](../../../cosmic-microwave-background-anisotropy.md#baryon-euler-equation-with-thomson-drag)

$$
\boxed{\dot v_b+\mathcal H v_b+k\psi=\frac{\dot\tau}{R}(v_b-v_\gamma),\qquad R=\frac{3\bar\rho_b}{4\bar\rho_\gamma}.}
$$

This $R$ is the [baryon loading parameter](../../../cosmic-microwave-background-anisotropy.md#baryon-loading-parameter), the [baryon](../../../physics.md#baryon)-to-[photon](../../../quantum-mechanics.md#photon) inertia ratio. The two collision terms cancel exactly when the equations are weighted by their enthalpies. Background conservation gives $\bar\rho_b\propto a^{-3}$ and $\bar\rho_\gamma\propto a^{-4}$, so $\dot R=\mathcal H R$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [tight-coupling approximation](../../../cosmic-microwave-background-anisotropy.md#tight-coupling-approximation) requires the positive scattering rate $\kappa=-\dot\tau$ to exceed both $k$ and the [conformal Hubble parameter](../../../cosmology.md#conformal-hubble-parameter). The [photon-baryon velocity slip](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-velocity-slip) and [photon quadrupole](../../../cosmic-microwave-background-anisotropy.md#photon-quadrupole) are then small, and the leading fluid motion has $v_b=v_\gamma=v$. One must combine the equations before setting the slip to zero: a small slip times a large collision rate can exert a finite force.

Add the [photon Euler equation](../../../cosmic-microwave-background-anisotropy.md#photon-euler-equation) to $R$ times the [baryon Euler equation with Thomson drag](../../../cosmic-microwave-background-anisotropy.md#baryon-euler-equation-with-thomson-drag). The collisions cancel and, neglecting $\Theta_2$ at this order, the result is

$$
(1+R)\dot v+\mathcal H Rv+\frac{k}{4}\delta_\gamma+(1+R)k\psi=0.
$$

Since $\dot R=\mathcal H R$, the common velocity obeys

$$
\boxed{\dot v_\gamma+\frac{\dot R}{1+R}v_\gamma+\frac{k}{4(1+R)}\delta_\gamma+k\psi=0.}
$$

The inertia of the [baryons](../../../physics.md#baryon) reduces the [photon-baryon sound speed](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-sound-speed) to $c_s^2=1/[3(1+R)]$.

Differentiate the [photon continuity equation](../../../cosmic-microwave-background-anisotropy.md#photon-continuity-equation) and substitute this velocity equation:

$$
\ddot\delta_\gamma=\frac43k\dot v_\gamma+4\ddot\phi=-\frac{\dot R}{1+R}(\dot\delta_\gamma-4\dot\phi)-\frac{k^2}{3(1+R)}\delta_\gamma-\frac43k^2\psi+4\ddot\phi.
$$

Thus the [photon-baryon acoustic oscillator](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-acoustic-oscillator) is

$$
\boxed{\ddot\delta_\gamma+\frac{\dot R}{1+R}\dot\delta_\gamma+\frac{k^2}{3(1+R)}\delta_\gamma=4\ddot\phi+\frac{4\dot R}{1+R}\dot\phi-\frac43k^2\psi.}
$$

The terms on the right drive the oscillation gravitationally; the first-derivative term comes from changing [baryon](../../../physics.md#baryon) inertia. Diffusion damping enters only beyond this leading [tight-coupling approximation](../../../cosmic-microwave-background-anisotropy.md#tight-coupling-approximation).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Expand the fractional [CMB](../../../cosmology.md#cosmic-microwave-background) temperature fluctuation as $\Theta(\mathbf n)=\sum_{\ell m}a_{\ell m}Y_{\ell m}(\mathbf n)$. Under [statistical isotropy](../../../probability-and-statistics.md#statistical-isotropy), its [CMB angular power spectrum](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-power-spectrum) is defined by

$$
\boxed{\langle a_{\ell m}a_{\ell' m'}^*\rangle=C_\ell\delta_{\ell\ell'}\delta_{mm'},\qquad C_\ell=\frac{1}{2\ell+1}\sum_m\langle|a_{\ell m}|^2\rangle.}
$$

The normalization is for dimensionless temperature, rather than temperature in kelvin. The [spherical harmonics](../../../analysis.md#spherical-harmonic) separate angular scales, with large $\ell$ corresponding to small angles.

For approximately constant $R,\phi,\psi$, a useful solution of the [photon-baryon acoustic oscillator](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-acoustic-oscillator) is

$$
\delta_\gamma=-4(1+R)\psi+A\cos(kr_s)+B\sin(kr_s),\qquad\boxed{r_s(\eta)=\int_0^\eta\frac{d\eta'}{\sqrt{3[1+R(\eta')]}}.}
$$

Here $r_s$ is the comoving [sound horizon](../../../cosmic-microwave-background-anisotropy.md#sound-horizon). With slowly varying $R$, the oscillatory phase is still $kr_s$ and its homogeneous amplitude varies approximately as $(1+R)^{-1/4}$ under the short-period approximation. Evolving potentials add gravitational driving rather than erase this phase coherence.

The regular growing [adiabatic initial conditions](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) produce an initial density displacement and negligible initial acoustic velocity outside the horizon. They therefore select the cosine phase, with $B$ approximately zero, for all modes. At last scattering, extrema of compression and rarefaction occur at $kr_s(\eta_*)\simeq n\pi$. The observed monopole-plus-potential [Sachs-Wolfe combination](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-combination) is $\Theta_0+\psi=\delta_\gamma/4+\psi$, so [baryon](../../../physics.md#baryon) loading shifts its equilibrium and makes alternating peaks unequal. The velocity produces a phase-shifted [Doppler CMB anisotropy](../../../cosmic-microwave-background-anisotropy.md#doppler-cmb-anisotropy).

Projection from the [Cosmic microwave background last-scattering surface](../../../cosmology.md#cosmic-microwave-background-last-scattering-surface) places a mode near $\ell\simeq k\chi_*$, where $\chi_*=\eta_0-\eta_*$ is its [comoving radial distance](../../../cosmology.md#comoving-radial-distance) in a flat universe. The resulting [adiabatic acoustic-peak spacing](../../../cosmic-microwave-background-anisotropy.md#adiabatic-acoustic-peak-spacing) is

$$
\boxed{\ell_n\simeq n\pi\frac{\chi_*}{r_s(\eta_*)},\qquad n=1,2,\ldots.}
$$

**Coherent acoustic phases turn successive compressions and rarefactions into the [CMB](../../../cosmology.md#cosmic-microwave-background) peak series.** Finite-width last scattering, Doppler projection, evolving potentials and diffusion shift or broaden actual peaks, so this is the requested approximate spacing, not an exact prediction for every peak.

## 3

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Let $q^i=e^i-\tfrac12h^i{}_je^j$, so $p^0=\epsilon/a^2$ and $p^i=(\epsilon/a^2)q^i$. The [orthonormal tetrad](../../../general-relativity.md#orthonormal-frame-in-spacetime) gives $\delta_{ij}e^ie^j=1$. To first order,

$$
\delta_{ij}q^iq^j=1-h_{ij}e^ie^j,\qquad h_{ij}q^iq^j=h_{ij}e^ie^j.
$$

Hence the time-index [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) contract to

$$
\Gamma^0{}_{00}+\Gamma^0{}_{ij}q^iq^j=2\mathcal H+\frac12\dot h_{ij}e^ie^j.
$$

The $\mathcal H h_{ij}$ term cancels the perturbation in the coordinate direction norm. This cancellation is why the local tetrad direction must not be mistaken for the coordinate direction.

Along the [photon](../../../quantum-mechanics.md#photon) [null geodesic](../../../special-relativity.md#null-geodesic), $d/d\lambda=p^0d/d\eta$, and

$$
\frac{dp^0}{d\lambda}=\left(\frac\epsilon{a^2}\right)^2\left(\frac1\epsilon\frac{d\epsilon}{d\eta}-2\mathcal H\right).
$$

The time component of the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) now gives the [photon energy redshift from a tensor metric perturbation](../../../linear-cosmological-perturbation-theory.md#photon-energy-redshift-from-a-tensor-metric-perturbation):

$$
\boxed{\frac1\epsilon\frac{d\epsilon}{d\eta}=-\frac12\dot h_{ij}e^ie^j.}
$$

The derivative on the left follows the ray; the dot on $h$ is a partial [conformal time](../../../cosmology.md#conformal-time) derivative. The background redshift has already been removed by using comoving energy. The calculation only needs $\Gamma^0{}_{00}$ and $\Gamma^0{}_{ij}$; the unrelated printed $\Gamma^i{}_{j0}$ should contain $\tfrac12\dot h^i{}_j$, rather than the full derivative.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

To first order, propagate along the unperturbed ray $\mathbf x(\eta)=\mathbf x_0-(\eta_0-\eta)\mathbf e$ and keep its [orthonormal tetrad](../../../general-relativity.md#orthonormal-frame-in-spacetime) direction fixed. Corrections to direction or trajectory multiply an already first-order temperature source and are second order. Define the angular scattering source

$$
S(\eta,\mathbf x,\mathbf e)=\frac{3}{16\pi}\int d\Omega_{\mathbf m}\,\Theta(\eta,\mathbf x,\mathbf m)[1+(\mathbf e\cdot\mathbf m)^2].
$$

Using the [photon energy redshift from a tensor metric perturbation](../../../linear-cosmological-perturbation-theory.md#photon-energy-redshift-from-a-tensor-metric-perturbation), the [Photon Boltzmann equation with Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#photon-boltzmann-equation-with-thomson-scattering) along this ray becomes

$$
\frac{d\Theta}{d\eta}-\dot\tau\Theta=-\frac12\dot h_{ij}e^ie^j-\dot\tau S.
$$

Multiply by the survival probability $e^{-\tau}$. The [cosmological visibility function](../../../cosmic-microwave-background-anisotropy.md#cosmological-visibility-function) is $g(\eta)=-\dot\tau e^{-\tau}$, so integration gives

$$
\Theta_0=e^{-\tau_i}\Theta_i+\int_{\eta_i}^{\eta_0}gS\,d\eta-\frac12\int_{\eta_i}^{\eta_0}e^{-\tau}\dot h_{ij}e^ie^j\,d\eta.
$$

Every source here is evaluated on the same ray, and $\tau(\eta_0)=0$.

The instantaneous-visibility approximation makes $e^{-\tau}$ a step from zero to one at $\eta_*$. It suppresses the early boundary term and localizes the scattering source to $S_*$. To obtain only the requested [tensor CMB line-of-sight source](../../../cosmic-microwave-background-anisotropy.md#tensor-cmb-line-of-sight-source), additionally neglect this last-scattering angular source: in leading [tight coupling](../../../cosmic-microwave-background-anisotropy.md#tight-coupling-approximation), the tensor-induced incident quadrupole is small, and a tensor mode has no scalar monopole or dipole. Ignore later [reionization](../../../cosmology.md#reionization) and its scattering as well. Then

$$
\boxed{\Theta(\eta_0,\mathbf x_0,\mathbf e)\simeq-\frac12\int_{\eta_*}^{\eta_0}\dot h_{ij}(\eta,\mathbf x_0-(\eta_0-\eta)\mathbf e)e^ie^j\,d\eta.}
$$

**Instantaneous visibility alone would leave the term $S_*$; neglect of that term is an additional approximation.** The time derivative on $h$ is essential and is present in the PDF, although it was lost in the extracted TeX.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Choose the arbitrary normalization of the complex [plane wave](../../../quantum-mechanics.md#plane-wave) polarization so that $h_{ij}=u_iu_jh(\eta)e^{ikz}$ with $\mathbf u=(1,i,0)$. For $\mathbf e=(\sin\theta\cos\varphi,\sin\theta\sin\varphi,\cos\theta)$, contraction gives

$$
(u_ie^i)^2=\sin^2\theta\,e^{2i\varphi}.
$$

At the observer origin, write $\mu=\cos\theta$. The [tensor CMB line-of-sight source](../../../cosmic-microwave-background-anisotropy.md#tensor-cmb-line-of-sight-source) is

$$
\Theta(\mathbf e)=-\frac12\sin^2\theta\,e^{2i\varphi}\int_{\eta_*}^{\eta_0}\dot h(\eta)e^{-ik(\eta_0-\eta)\mu}\,d\eta.
$$

The rest of the expression is independent of $\varphi$. Projection onto $Y_{\ell m}^*\propto e^{-im\varphi}$ therefore gives zero unless $m=2$. This is the [helicity selection for tensor CMB multipoles](../../../linear-cosmological-perturbation-theory.md#helicity-selection-for-tensor-cmb-multipoles). It applies to the specified complex helicity mode; taking a physical real field also introduces the conjugate mode and its conjugate azimuthal dependence.

For the very long wavelength solution during matter domination, differentiation gives $\dot h=-h_{\mathrm{prim}}k^2\eta/5+O(k^4\eta^3)$. Expand the [plane wave](../../../quantum-mechanics.md#plane-wave) factor once to obtain

$$
\Theta=\frac{h_{\mathrm{prim}}k^2}{10}\sin^2\theta e^{2i\varphi}[A_0-ik\mu A_1]+O(h_{\mathrm{prim}}k^4\eta_0^4),
$$

where

$$
A_0=\frac{\eta_0^2-\eta_*^2}{2},\qquad A_1=\frac{\eta_0^3}{6}-\frac{\eta_0\eta_*^2}{2}+\frac{\eta_*^3}{3}.
$$

Let $\mathcal N_{22}=\tfrac14\sqrt{15/(2\pi)}$. Then $Y_{22}=\mathcal N_{22}\sin^2\theta e^{2i\varphi}$ and $Y_{32}=\sqrt7\mathcal N_{22}\mu\sin^2\theta e^{2i\varphi}$. Reading off the [long-wavelength tensor CMB quadrupole and octupole](../../../linear-cosmological-perturbation-theory.md#long-wavelength-tensor-cmb-quadrupole-and-octupole) yields

$$
\Theta_{22}=\frac{h_{\mathrm{prim}}k^2A_0}{10\mathcal N_{22}},\qquad\frac{\Theta_{32}}{\Theta_{22}}=-\frac{ik}{\sqrt7}\frac{A_1}{A_0}.
$$

In the limit $\eta_*/\eta_0\to0$,

$$
\boxed{\Theta_{22}=\frac{h_{\mathrm{prim}}}{20\mathcal N_{22}}(k\eta_0)^2+O((k\eta_0)^4),\qquad\Theta_{32}=-\frac{i}{3\sqrt7}(k\eta_0)\Theta_{22}+O((k\eta_0)^5).}
$$

A perfectly frozen tensor produces no redshift; the first contribution comes from its order-$k^2\eta^2$ evolution. The extra spatial phase makes the octupole one power of $k\eta_0$ smaller than the quadrupole.

## 4

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

For a centered [Gaussian random field](../../../stochastic-process.md#gaussian-random-field), [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) takes the classical form of the [Isserlis theorem](../../../probability-theory.md#isserlis-s-theorem): every even correlator is a sum over pairings of two-point correlators, and every odd correlator vanishes. For example, with $G_i=\zeta_G(\mathbf x_i)$,

$$
\langle G_1G_2G_3G_4\rangle=\langle G_1G_2\rangle\langle G_3G_4\rangle+\langle G_1G_3\rangle\langle G_2G_4\rangle+\langle G_1G_4\rangle\langle G_2G_3\rangle.
$$

A $2n$-point correlator has $(2n-1)!!$ pairings. Equivalently, all [connected correlation functions](../../../critical-phenomenon.md#connected-correlation-function) beyond order two vanish. **The [covariance](../../../variance.md#covariance) completely determines the centered Gaussian statistics; higher ordinary correlators can be nonzero, but contain no independent connected information.** For a field with nonzero mean, apply these statements to the centered field and then restore its mean.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Use the [Fourier transform](../../../analysis.md#fourier-transform) convention $\zeta(\mathbf x)=\int d^3k\,e^{i\mathbf k\cdot\mathbf x}\zeta(\mathbf k)/(2\pi)^3$. Statistical homogeneity and isotropy define the [primordial bispectrum](../../../cosmology.md#primordial-bispectrum) by

$$
\boxed{\langle\zeta(\mathbf k_1)\zeta(\mathbf k_2)\zeta(\mathbf k_3)\rangle_c=(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2+\mathbf k_3)B(k_1,k_2,k_3).}
$$

The [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) enforces [momentum conservation](../../../classical-mechanics.md#momentum-conservation); the three magnitudes describe a closed triangle. Set $\alpha=3f_{\mathrm{NL}}/5$. For the [centered quadratic Gaussian transformation](../../../stochastic-process.md#centered-quadratic-gaussian-transformation), its quadratic Fourier term is

$$
\alpha\int\frac{d^3q}{(2\pi)^3}G(\mathbf q)G(\mathbf k-\mathbf q)-\alpha(2\pi)^3\delta^{(3)}(\mathbf k)\langle G^2\rangle.
$$

At first order in $\alpha$, choose the quadratic field at one of the three external positions. For the first position, [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction) pair the two internal fields with the two remaining external fields in two ways. The self-pairing is precisely removed by the subtracted mean. The surviving contribution is $2\alpha P(k_2)P(k_3)$ times the momentum delta. Adding the other positions gives the tree-level [local-type primordial non-Gaussianity](../../../cosmology.md#local-type-primordial-non-gaussianity) result

$$
\boxed{B^{\mathrm{loc}}=\frac65f_{\mathrm{NL}}[P(k_1)P(k_2)+P(k_2)P(k_3)+P(k_3)P(k_1)].}
$$

**This expression is at leading order in $f_{\mathrm{NL}}$.** The exact quadratic map also has a [loop correction to the local primordial bispectrum](../../../cosmology.md#loop-correction-to-the-local-primordial-bispectrum), from three quadratic vertices:

$$
B_{\mathrm{loop}}=8\alpha^3\int\frac{d^3q}{(2\pi)^3}P(q)P(|\mathbf k_1-\mathbf q|)P(|\mathbf k_2+\mathbf q|).
$$

There is no quadratic-in-$\alpha$ bispectrum term, because it would involve five centered Gaussian fields. A regulator may be needed for this higher-order integral. The displayed leading formula uses the Gaussian power $P$, consistently neglecting its order-$f_{\mathrm{NL}}^2$ correction.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

Distinguish the [slow-roll approximation](../../../cosmic-inflation.md#slow-roll-approximation) parameter $\epsilon$ from the infinitesimal positive contour regulator $\varepsilon$. In the [interaction picture](../../../quantum-mechanics.md#interaction-picture), the ordered unequal-time [Wick contraction](../../../perturbative-quantum-field-theory.md#wick-contraction) is

$$
\langle\zeta(\mathbf k,0)\zeta(\mathbf p,\tau)\rangle=(2\pi)^3\delta^{(3)}(\mathbf k+\mathbf p)u_k(0)u_k^*(\tau).
$$

A differentiated vertex field instead supplies $u_k^{*\prime}(\tau)$. These conjugates are fixed by the [annihilation operators](../../../quantum-mechanics.md#annihilation-operator) and [creation operators](../../../quantum-mechanics.md#creation-operator) and cannot be dropped while retaining the same contour.

Convert the interaction time integral to [conformal time](../../../cosmology.md#conformal-time). Since $dt=a\,d\tau$ and each cosmic-time derivative is $a^{-1}\partial_\tau$, the integrated cubic vertex is

$$
\int dt\,H_{\mathrm{int}}=-M_{\mathrm{Pl}}^2\epsilon^2\int d\tau\,a^2\int d^3x\,\zeta\zeta'^2.
$$

The [in-in formalism](../../../quantum-field-theory.md#keldysh-formalism) supplies $-2i$ multiplying the expectation of the Hamiltonian, so its negative sign gives $+2i$ multiplying this vertex. At nonzero external momenta, the connected contractions join each of the three external fields to one vertex field. There are six bijections, not three. Choosing which external field meets the undifferentiated vertex gives three cyclic choices; swapping the two differentiated fields gives a further factor of two. This is the [Wick-pairing multiplicity for a zeta zeta-prime-squared vertex](../../../cosmology.md#wick-pairing-multiplicity-for-a-zeta-zeta-prime-squared-vertex).

For example, before the internal momenta are integrated, one cyclic contribution includes

$$
\int\prod_{r=1}^3\frac{d^3p_r}{(2\pi)^3}\,(2\pi)^3\delta^{(3)}(\mathbf p_1+\mathbf p_2+\mathbf p_3)\prod_{r=1}^3[(2\pi)^3\delta^{(3)}(\mathbf k_r+\mathbf p_r)]\,u_{p_1}^*u_{p_2}^{*\prime}u_{p_3}^{*\prime}.
$$

The factors of $2\pi$ cancel to leave one overall $(2\pi)^3$ and the external momentum delta. Thus the properly normalized reduced expression is

$$
\boxed{\begin{aligned}
\langle\zeta_1\zeta_2\zeta_3\rangle_c&=(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2+\mathbf k_3)\\
&\quad\times\operatorname{Re}\left[4iM_{\mathrm{Pl}}^2\epsilon^2\prod_ru_{k_r}(0)\int_{-\infty(1-i\varepsilon)}^0d\tau\,a^2\sum_{\mathrm{cyc}}u_{k_1}^*u_{k_2}^{*\prime}u_{k_3}^{*\prime}\right].
\end{aligned}}
$$

The [vacuum prescription for inflationary in-in integrals](../../../quantum-field-theory.md#vacuum-prescription-for-inflationary-in-in-integrals) damps the early-time oscillations and selects the [Bunch-Davies vacuum](../../../cosmic-inflation.md#bunch-davies-vacuum). Internal self-contractions correspond to disconnected zero-momentum tadpole terms and are excluded from this connected three-point function.

The printed intermediate expression has unconjugated modes and only three literal cyclic terms with coefficient $-2i$. The conjugate form of the result above would use $-4i$, together with the conjugated contour. A literal $-2i$ with only three terms gives half the final printed answer. The six-contraction expression above is the consistent reduction of the supplied Hamiltonian and leads to that final answer.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

Write $A_k=H/\sqrt{4\epsilon M_{\mathrm{Pl}}^2k^3}$, so $u_k(0)=A_k$. For the cyclic term with the first field undifferentiated, insertion into the [in-in formalism](../../../quantum-field-theory.md#keldysh-formalism) gives

$$
a^2\prod_ru_{k_r}(0)\,u_{k_1}^*u_{k_2}^{*\prime}u_{k_3}^{*\prime}=\frac{H^4}{64\epsilon^3M_{\mathrm{Pl}}^6(k_1k_2k_3)^3}\,k_2^2k_3^2(1-ik_1\tau)e^{iK\tau},
$$

where $K=k_1+k_2+k_3>0$. The two differentiated modes contribute $\tau^2$, cancelling the $\tau^{-2}$ in $a^2$.

Along the vacuum-selected contour, the lower boundary vanishes. The elementary integrals are

$$
\int_{-\infty(1-i\varepsilon)}^0e^{iK\tau}\,d\tau=-\frac{i}{K},\qquad \int_{-\infty(1-i\varepsilon)}^0\tau e^{iK\tau}\,d\tau=\frac{1}{K^2},
$$

and therefore

$$
\int_{-\infty(1-i\varepsilon)}^0(1-ik_1\tau)e^{iK\tau}\,d\tau=-i\left(\frac1K+\frac{k_1}{K^2}\right).
$$

Multiplying by $4iM_{\mathrm{Pl}}^2\epsilon^2$, taking the real part and summing the three cyclic choices gives the [curvature bispectrum from a zeta zeta-prime-squared interaction](../../../cosmology.md#curvature-bispectrum-from-a-zeta-zeta-prime-squared-interaction):

$$
\boxed{\begin{aligned}
\langle\zeta_1\zeta_2\zeta_3\rangle_c&=(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2+\mathbf k_3)B^{\mathrm{sf}},\\
B^{\mathrm{sf}}&=\frac{H^4}{16\epsilon M_{\mathrm{Pl}}^4(k_1k_2k_3)^3}\sum_{\mathrm{cyc}}k_2^2k_3^2\left(\frac1K+\frac{k_1}{K^2}\right).
\end{aligned}}
$$

This matches the final normalization. The coefficient requires all six connected [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction).

The calculation assumes the Gaussian [Bunch-Davies vacuum](../../../cosmic-inflation.md#bunch-davies-vacuum), tree order in the specified cubic interaction, effectively constant $H$ and $\epsilon$ during the integral, the approximate de Sitter [scale factor](../../../cosmology.md#scale-factor-cosmology), and observation after the modes freeze as $\tau\to0^-$. The contour tilt is kept until the early boundary has been eliminated; an undamped real-axis integral cannot simply discard that boundary. The [reduced Planck mass](../../../physics.md#reduced-planck-mass) convention is the one in the supplied [De Sitter curvature mode function](../../../cosmic-inflation.md#de-sitter-curvature-mode-function). Other cubic interactions and nonlinear field redefinitions are outside the specified model, so this is not by itself the complete bispectrum of a general single-field action.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

At late time the Gaussian curvature [power spectrum](../../../probability-and-statistics.md#power-spectrum) is $P(k)=H^2/(4\epsilon M_{\mathrm{Pl}}^2k^3)$. Consider the [squeezed bispectrum configuration](../../../cosmology.md#squeezed-bispectrum-configuration) $k_1=q\ll k_2\simeq k_3=k$. The [local-type primordial non-Gaussianity](../../../cosmology.md#local-type-primordial-non-gaussianity) result is dominated by

$$
B^{\mathrm{loc}}(q,k,k)\simeq\frac{12}{5}f_{\mathrm{NL}}P(q)P(k).
$$

In the [curvature bispectrum from a zeta zeta-prime-squared interaction](../../../cosmology.md#curvature-bispectrum-from-a-zeta-zeta-prime-squared-interaction), the leading cyclic term has the long mode in the undifferentiated slot. Its momentum numerator tends to $k^4/(2k)=k^3/2$, while the other two cyclic terms contain $q^2$. Hence

$$
\boxed{B^{\mathrm{sf}}(q,k,k)\simeq\frac{H^4}{32\epsilon M_{\mathrm{Pl}}^4q^3k^3}=\frac\epsilon2P(q)P(k).}
$$

This is the [slow-roll amplitude of the squeezed zeta zeta-prime-squared bispectrum](../../../cosmology.md#slow-roll-amplitude-of-the-squeezed-zeta-zeta-prime-squared-bispectrum). It retains the local-like $q^{-3}$ enhancement: assigning the soft momentum only to differentiated legs would incorrectly miss the dominant permutation. Comparing squeezed amplitudes gives

$$
\boxed{f_{\mathrm{NL}}^{\mathrm{effective}}=\frac{5\epsilon}{24}\ll1.}
$$

For comparison, in the equilateral configuration $B^{\mathrm{sf}}(k,k,k)=(4\epsilon/3)P(k)^2$, so the signal is slow-roll suppressed away from the squeezed limit as well.

Use the quoted observational bound as the sensitivity benchmark supplied by this problem, rather than as a new current measurement. A local-template sensitivity at the order-ten level is far above this order-$\epsilon$ signal; detection of this interaction with comparable [CMB](../../../cosmology.md#cosmic-microwave-background) measurements is consequently very unlikely. The entire shape is not identical to the local template, so its bound is not an exact constraint on every single-field shape, but the squeezed amplitude already exposes the large suppression. **The obstacle is the slow-roll amplitude, even though this specified interaction has a squeezed enhancement.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
