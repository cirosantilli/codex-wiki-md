# Paper 64

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper64.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper64.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)

## 1

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write $\rho=\bar\rho(1+\delta)$, take a constant barotropic equation-of-state parameter $w$, and keep first-order terms in $\delta$, $v^i$ and $h_{ij}$. In [synchronous gauge](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology), the inverse metric is $g^{00}=-a^{-2}$, $g^{0i}=0$, $g^{ij}=a^{-2}(\delta^{ij}-h^{ij})$. The normalization $u^\mu u_\mu=-1$ gives $u^0=a^{-1}+O(v^2)$ and $u^i=a^{-1}v^i$. Substitution in the [perfect fluid](../../../general-relativity.md#perfect-fluid) stress tensor gives the [linear perfect-fluid stress tensor in synchronous gauge](../../../linear-cosmological-perturbation-theory.md#linear-perfect-fluid-stress-tensor-in-synchronous-gauge):

$$
\boxed{\begin{aligned}
T^{00}&=a^{-2}\bar\rho(1+\delta),\\
T^{0i}&=a^{-2}\bar\rho(1+w)v^i,\\
T^{ij}&=a^{-2}w\bar\rho[(1+\delta)\delta^{ij}-h^{ij}].
\end{aligned}}
$$

In the first component the pressure contributions cancel; in the last, the velocity product is second order and the inverse-metric perturbation supplies the minus sign.

Use projections of [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation), $\nabla_\mu T^{\mu\nu}=0$, to retain all connection terms efficiently. Let $\mathcal H=a'/a$ be the [conformal Hubble parameter](../../../cosmology.md#conformal-hubble-parameter) and $h=\delta^{ij}h_{ij}$. Since $\sqrt{-g}=a^4(1+h/2)$, the fluid expansion is

$$
\vartheta=\nabla_\mu u^\mu=\frac1{\sqrt{-g}}\partial_\mu(\sqrt{-g}u^\mu)=a^{-1}\left(3\mathcal H+\partial_iv^i+\frac12h'\right).
$$

The energy projection is $u^\mu\partial_\mu\rho+(\rho+P)\vartheta=0$. Its background is $\bar\rho'+3\mathcal H(1+w)\bar\rho=0$. Expanding and subtracting that background leaves the [synchronous perfect-fluid density equation](../../../linear-cosmological-perturbation-theory.md#synchronous-perfect-fluid-density-equation)

$$
\delta'+(1+w)\left(\partial_iv^i+\frac12h'\right)=0.
$$

For momentum, the spatial projection is $(\rho+P)u^\nu\nabla_\nu u_i+(\delta_i{}^\nu+u_i u^\nu)\partial_\nu P=0$. The given connections yield $u^\nu\nabla_\nu u_i=v_i'+\mathcal H v_i$ at first order. The pressure projection contains both $\partial_i\delta P$ and $v_i\bar P'$; retaining the latter is essential. With $\delta P=w\bar\rho\delta$ and $\bar P'=-3w\mathcal H(1+w)\bar\rho$, division by $\bar\rho(1+w)$ gives the [Cosmological Euler equation in synchronous gauge](../../../linear-cosmological-perturbation-theory.md#cosmological-euler-equation-in-synchronous-gauge),

$$
v_i'+(1-3w)\mathcal H v_i+\frac{w}{1+w}\partial_i\delta=0.
$$

For Fourier convention $e^{i\mathbf k\cdot\mathbf x}$, these results are

$$
\boxed{\delta'+(1+w)i\mathbf k\cdot\mathbf v+\frac12(1+w)h'=0,\qquad\mathbf v'+(1-3w)\mathcal H\mathbf v+\frac{w}{1+w}i\mathbf k\delta=0.}
$$

The velocity equation assumes nonzero enthalpy $\bar\rho+\bar P$, so a cosmological constant with $w=-1$ is not a propagating fluid-velocity case. A time-dependent $w$ would also introduce additional terms and is not the constant-barotropic system used here.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Put $\theta=i\mathbf k\cdot\mathbf v$. The [synchronous perfect-fluid density equation](../../../linear-cosmological-perturbation-theory.md#synchronous-perfect-fluid-density-equation) and [Cosmological Euler equation in synchronous gauge](../../../linear-cosmological-perturbation-theory.md#cosmological-euler-equation-in-synchronous-gauge) give

$$
\delta'=-(1+w)(\theta+h'/2),\qquad\theta'+(1-3w)\mathcal H\theta-\frac{w}{1+w}k^2\delta=0.
$$

Differentiate the first equation and use the second and the scalar trace metric equation. Before making a nonrelativistic approximation, the result is

$$
\delta''+\mathcal H\delta'+\left[wk^2-\frac32(1+w)(1+3w)\mathcal H^2\right]\delta=-3w(1+w)\mathcal H\theta.
$$

For $w=w_m=c_s^2\ll1$, discard relative pressure corrections to the background gravitational and damping terms, while retaining $c_s^2k^2$ because a large wavenumber can compensate a small sound speed. Matter domination and the flat [Friedmann equation](../../../cosmology.md#friedmann-equations) give $\tfrac32\mathcal H^2=4\pi G\bar\rho_m a^2$. Thus the leading [nonrelativistic density equation in synchronous gauge](../../../linear-cosmological-density-perturbation.md#nonrelativistic-density-equation-in-synchronous-gauge) is

$$
\boxed{\delta_m''+\mathcal H\delta_m'+(c_s^2k^2-4\pi G\bar\rho_m a^2)\delta_m\simeq0.}
$$

The approximation sign records the small finite-$w$ terms just displayed; the printed Newtonian-form equation is not an exact relativistic equation at nonzero $w$.

The comoving [Jeans wavenumber](../../../linear-cosmological-density-perturbation.md#jeans-wavenumber) balances pressure and gravity: $c_s^2k_J^2=4\pi G\bar\rho_m a^2$. Defining physical wavelength as $2\pi a/k$, the physical [Jeans length](../../../linear-cosmological-density-perturbation.md#jeans-length) is

$$
\boxed{\lambda_J=\frac{2\pi a}{k_J}=c_s\sqrt{\frac\pi{G\bar\rho_m}}.}
$$

For wavelengths longer than this scale, gravity can overcome pressure and density modes grow; shorter modes are pressure-supported acoustic oscillations, with expansion modifying both growth and damping. Before [cosmological recombination](../../../cosmology.md#recombination-cosmology), the tightly coupled [photon-baryon fluid](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-fluid) has substantial photon pressure, $c_{s,\gamma b}^2=1/[3(1+R_b)]$, where $R_b=3\bar\rho_b/(4\bar\rho_\gamma)$. The baryonic Jeans scale is correspondingly large, so baryons oscillate instead of freely collapsing on small scales. [Cold dark matter](../../../cosmology.md#cold-dark-matter) has a much smaller pressure scale and can supply gravitational potential wells. After [photon decoupling](../../../cosmology.md#photon-decoupling), baryons lose photon pressure support and their sound speed falls to its thermal-gas value; the [baryon Jeans length across recombination](../../../linear-cosmological-density-perturbation.md#baryon-jeans-length-across-recombination) drops, allowing baryons to fall into those wells. The earlier photon-coupled fluid is not itself a constant-small-$w$ fluid; its role is a physical comparison of pressure support, not an extension of the preceding approximation through recombination.

Define a normalized smoothing window on physical radius $R$, with comoving radius $r=R/a$. If $\langle\delta_{\mathbf k}\delta_{\mathbf k'}^*\rangle=(2\pi)^3\delta_D(\mathbf k-\mathbf k')P(k,\tau)$, the [smoothed matter density variance](../../../linear-cosmological-density-perturbation.md#smoothed-matter-density-variance) is

$$
\sigma_R^2(\tau)=\langle\delta_R^2\rangle=\frac1{2\pi^2}\int_0^\infty k^2P(k,\tau)|W(kr)|^2dk.
$$

Thus $\sigma_R$ is the root-mean-square amplitude. For a Gaussian window, $W(u)=e^{-u^2/2}$; this choice makes the scale-free integral ultraviolet convergent.

On scales where pressure is negligible, a flat matter-dominated universe has $a\propto\tau^2$, $\mathcal H=2/\tau$, and $4\pi G\bar\rho_m a^2=6/\tau^2$. The density equation has powers satisfying $s(s-1)+2s-6=0$, so

$$
\delta_m=C_+\tau^2+C_-\tau^{-3}.
$$

Select the growing mode and exclude residual synchronous gauge modes. Starting with $P(k,\tau_{\rm eq})=Ak$ gives $P(k,\tau)=Ak(\tau/\tau_{\rm eq})^4$. The [dimensionless cosmological power spectrum](../../../cosmic-inflation.md#dimensionless-cosmological-power-spectrum) is then

$$
\mathcal P_\delta(k,\tau)=\frac{k^3P(k,\tau)}{2\pi^2}=\frac{A}{2\pi^2\tau_{\rm eq}^4}(k\tau)^4.
$$

At [cosmological horizon crossing](../../../linear-cosmological-density-perturbation.md#cosmological-horizon-crossing), $k\sim aH=\mathcal H$, hence $k\tau\sim2$, and

$$
\boxed{\mathcal P_\delta(k,\tau_H)=\frac{8A}{\pi^2\tau_{\rm eq}^4},\qquad\text{independent of }k.}
$$

For the smoothed [variance](../../../variance.md), change variables to $u=kr$:

$$
\sigma_R^2=\frac{A}{2\pi^2r^4}\left(\frac\tau{\tau_{\rm eq}}\right)^4\int_0^\infty u^3|W(u)|^2du.
$$

The Gaussian integral equals $1/2$. At a physical Hubble-radius window, $R=H^{-1}$ and $r=\tau/2$, giving the [Gaussian horizon-crossing variance for a Harrison-Zeldovich spectrum](../../../linear-cosmological-density-perturbation.md#gaussian-horizon-crossing-variance-for-a-harrison-zeldovich-spectrum)

$$
\boxed{\sigma_{H^{-1}}^2=\frac{4A}{\pi^2\tau_{\rm eq}^4},\qquad\text{constant at crossing}.}
$$

The window-dependent numerical constant is secondary; cancellation of the scale dependence is the [Harrison-Zeldovich spectrum](../../../linear-cosmological-density-perturbation.md#harrison-peebles-zeldovich-spectrum) property. This demonstration uses the growing pressureless matter-era idealization and therefore applies to modes crossing in that era. Modes which crossed before equality require radiation-era transfer and cannot be evolved through that period with the matter equation. A pure $P\propto k$ spectrum with a real-space top-hat window also has a logarithmically divergent ultraviolet [variance](../../../variance.md) unless a physical high-$k$ cutoff or transfer function is supplied; the Gaussian choice makes the stated idealized [variance](../../../variance.md) well defined.

## 2

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use the photon phase-space coordinates $(\mathbf x,q,\mathbf n)$, with $q=ap$ and $\mathbf n$ its propagation direction. Divide the [Collisionless Boltzmann equation](../../../galaxy.md#collisionless-boltzmann-equation) by $d\tau/d\lambda$ and apply the chain rule. The homogeneous blackbody distribution is time independent at fixed comoving momentum because its physical temperature scales as $a^{-1}$. Therefore

$$
\partial_\tau f_1+\frac{dx^i}{d\tau}\partial_i f_1+q'\frac{df_0}{dq}+q'\partial_qf_1+(n^i)'\partial_{n^i}f_1=0.
$$

On the unperturbed ray $dx^i/d\tau=n^i$; its correction is first order and multiplies the first-order spatial gradient of $f_1$. Similarly $q'$ and $(n^i)'$ are first order, so their products with derivatives of $f_1$ are second order. The zeroth-order distribution has no directional dependence. Keeping only linear terms and using $q'=-qh'_{ij}n^in^j/2$ gives

$$
\partial_\tau f_1+n^i\partial_i f_1=\frac12qf_0'(q)h'_{ij}n^in^j.
$$

After Fourier transforming with $e^{i\mathbf k\cdot\mathbf x}$ and $\mu=\widehat{\mathbf k}\cdot\mathbf n$, the [Free-streaming photon Boltzmann equation](../../../cosmic-microwave-background-anisotropy.md#free-streaming-photon-boltzmann-equation) in synchronous variables is

$$
\boxed{f_1'+ik\mu f_1=\frac12qf_0'(q)h'_{ij}n^in^j.}
$$

Direction deflection is a real first-order geodesic effect, but its effect on the already perturbed distribution starts at second order here.

Let $I_0=\int_0^\infty q^3f_0(q)dq$, so in the phase-space normalization being used $a^4\bar\rho_\gamma=4\pi I_0$. The [photon brightness perturbation](../../../cosmic-microwave-background-anisotropy.md#photon-brightness-perturbation) is $\Delta=I_0^{-1}\int q^3f_1dq$. This agrees with the stated density normalization, and $I_0$ is independent of [conformal time](../../../cosmology.md#conformal-time). Integrating the distribution equation gives

$$
\Delta'+ik\mu\Delta=\frac{h'_{ij}n^in^j}{2I_0}\int_0^\infty q^4f_0'(q)dq.
$$

For a [Planck distribution](../../../statistical-physics.md#planck-photon-distribution), the endpoint term $[q^4f_0]_0^\infty$ vanishes. Integration by parts yields $\int q^4f_0' dq=-4I_0$. Thus the [synchronous photon brightness equation](../../../cosmic-microwave-background-anisotropy.md#synchronous-photon-brightness-equation) is

$$
\boxed{\Delta'+ik\mu\Delta=-2h'_{ij}n^in^j.}
$$

For a small directional blackbody temperature shift $\Theta=\Delta T/T$, expansion gives $f_1=-qf_0'(q)\Theta$. The same integral then gives $\Delta=4\Theta$, also following from blackbody energy density proportional to $T^4$. This temperature interpretation presumes a perturbed blackbody shape; frequency-integrated brightness can still be defined for more general distributions.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

In the [tight-coupling approximation](../../../cosmic-microwave-background-anisotropy.md#tight-coupling-approximation), repeated [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering) drives the photon distribution toward isotropy in the local baryon rest frame. At linear order a temperature perturbation gives a monopole and a small boost gives only a dipole. A photon propagating along $\mathbf n$ has rest-frame energy $p(1-\mathbf n\cdot\mathbf v)$, so

$$
f_1=-qf_0'(q)\left(\Theta_{\rm rest}+\mathbf n\cdot\mathbf v\right).
$$

Since the rest-frame [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast) is $\delta_\gamma=4\Theta_{\rm rest}$, the initial [photon brightness perturbation](../../../cosmic-microwave-background-anisotropy.md#photon-brightness-perturbation) is

$$
\boxed{\Delta_*=\delta_{\gamma *}+4\mathbf n\cdot\mathbf v_*.}
$$

The quadrupole and higher [photon temperature multipoles](../../../cosmic-microwave-background-anisotropy.md#photon-temperature-multipole) are small when the conformal collision rate $\kappa=a n_e\sigma_T$ greatly exceeds both $k$ and $\mathcal H$. For example the quadrupole is suppressed by a factor of order $k/\kappa$ relative to the dipole. Instantaneous decoupling idealizes this strongly coupled state as the initial data for collisionless propagation; finite mean free path and polarization corrections are omitted from that initial truncation.

Multiply the [synchronous photon brightness equation](../../../cosmic-microwave-background-anisotropy.md#synchronous-photon-brightness-equation) by $e^{ik\mu\tau}$ and integrate from $\tau_*$ to $\tau_0$. The [line-of-sight solution for free-streaming photons](../../../cosmic-microwave-background-anisotropy.md#line-of-sight-solution-for-free-streaming-photons) is

$$
\Delta(\mathbf k,\mathbf n,\tau_0)=e^{-ik\mu(\tau_0-\tau_*)}\Delta_*(\mathbf k,\mathbf n)-2\int_{\tau_*}^{\tau_0}e^{-ik\mu(\tau_0-\tau)}h'_{ij}(\mathbf k,\tau)n^in^j d\tau.
$$

The phase is essential: it specifies the emission point and the points traversed by the ray. In real space define $\mathbf x(\tau)=\mathbf x_0-\mathbf n(\tau_0-\tau)$ and $\mathbf x_*=\mathbf x(\tau_*)$. Dividing by four gives the [synchronous Sachs-Wolfe line-of-sight formula](../../../cosmic-microwave-background-anisotropy.md#synchronous-sachs-wolfe-line-of-sight-formula),

$$
\boxed{\frac{\Delta T}{T}(\mathbf x_0,\mathbf n,\tau_0)=\frac14\delta_\gamma(\mathbf x_*,\tau_*)+\mathbf n\cdot\mathbf v(\mathbf x_*,\tau_*)-\frac12\int_{\tau_*}^{\tau_0}h'_{ij}(\mathbf x(\tau),\tau)n^in^j d\tau.}
$$

The spatial arguments suppressed in a shorthand version must be understood in this retarded sense; evaluating the emission terms at $\mathbf x_0$ instead would discard free streaming. Here $\mathbf n$ is propagation direction. The observer-to-source direction on the sky is $-\mathbf n$, explaining the opposite Doppler sign often used with that convention. The formula describes the synchronous-frame observer; an additional observer peculiar velocity contributes a dipole.

The first term is the intrinsic temperature perturbation at emission, since $\delta_\gamma=4\Theta$. The second is the [Doppler CMB anisotropy](../../../cosmic-microwave-background-anisotropy.md#doppler-cmb-anisotropy) from the plasma bulk velocity. The third is gravitational frequency shifting by the time-dependent spatial metric along the ray, and can include scalar and tensor metric contributions. In scalar [Newtonian gauge](../../../linear-cosmological-perturbation-theory.md#newtonian-gauge), rearranging that metric contribution supplies the emission gravitational potential as well as the [Integrated Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#integrated-sachs-wolfe-effect), up to the observer terms. It should not be identified solely with the integrated Sachs-Wolfe term: a constant Newtonian potential need not give a vanishing synchronous metric integral.

On large angles, modes are outside or comparable to the sound horizon at emission. For the growing [adiabatic mode](../../../linear-cosmological-perturbation-theory.md#adiabatic-mode) during matter domination, the intrinsic and emission-potential contributions give the ordinary [Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-effect), $\Theta_0+\Psi=\Psi/3$ in Newtonian variables. Velocity is a gradient effect, of order $k\tau_*\Psi$ on superhorizon scales, so its Doppler contribution is suppressed there. A scale-invariant primordial curvature spectrum produces approximately the familiar large-angle plateau in $\ell(\ell+1)C_\ell$. Evolving potentials during radiation-to-matter transition or late acceleration can add integrated gravitational anisotropy; constant matter-era scalar potentials do not generate a genuine scalar integrated Sachs-Wolfe source.

On smaller angles, the [photon-baryon fluid](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-fluid) has undergone acoustic oscillations. Its density and velocity are approximately in cosine and sine phases, producing acoustic structure in the intrinsic and Doppler sources and their projection onto angular multipoles. [Silk damping](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-diffusion-damping) suppresses sufficiently short wavelengths before decoupling, while the finite width of last scattering also smooths the real small-angle signal. These corrections refine the instantaneous-decoupling model rather than follow from a collisionless equation alone. The separate intrinsic, velocity and metric pieces depend on gauge convention; the complete observed anisotropy, including the appropriate observer terms and removal of the unobservable mean, is the physical quantity.

## 3

↑ **Parent:** [Paper 64](paper-64.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Write $\gamma_{ij}={}^{(3)}g_{ij}$, $\gamma=\det\gamma_{ij}$ and $D_i$ for the [spatial covariant derivative](../../../numerical-relativity.md#spatial-covariant-derivative). With the negative-shift convention, the [extrinsic curvature of a spatial hypersurface](../../../numerical-relativity.md#extrinsic-curvature-of-a-spatial-hypersurface) is $K_{ij}=-(\dot\gamma_{ij}+D_iN_j+D_jN_i)/(2N)$. Contracting with $\gamma^{ij}$ and using metric compatibility gives

$$
K=-\frac1{2N}\left(\gamma^{ij}\dot\gamma_{ij}+2D_iN^i\right).
$$

The logarithmic [determinant](../../../linear-algebra.md#determinant) identity makes $\gamma^{ij}\dot\gamma_{ij}=\dot\gamma/\gamma$, hence

$$
\boxed{K=-\frac1{2N}\left(\frac{\dot\gamma}{\gamma}+2D_iN^i\right).}
$$

This is also the fractional volume expansion, with a minus sign from the extrinsic-curvature convention.

Define $a=\gamma^{1/6}$ so that $\sqrt\gamma=a^3$. The useful unit-determinant conformal decomposition is $\gamma_{ij}=a^2\widetilde\gamma_{ij}$ with $\det\widetilde\gamma=1$, equivalently $\widetilde\gamma_{ij}=a^{-2}\gamma_{ij}$. Multiplying by $a^2$ instead would be a different conformal rescaling, not this unit-determinant one; no conformal decomposition is needed for the trace identity itself.

With zero [shift vector](../../../numerical-relativity.md#shift-vector), $\dot\gamma/\gamma=6\dot a/a$ and the [local volume Hubble parameter](../../../cosmology.md#local-volume-hubble-parameter) is

$$
\boxed{H=-\frac K3=\frac1{Na}\dot a.}
$$

Along a normal trajectory proper time satisfies $ds=Ndt$, so $H=a^{-1}da/ds$ is the local physical volume-expansion rate. The printed equality with $\dot a/a$ requires the proper-time gauge $N=1$; zero shift alone does not set the lapse to unity. In a homogeneous [Friedmann-Lemaître-Robertson-Walker metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) it reduces to the ordinary [Hubble parameter](../../../cosmology.md#hubble-parameter), while in an inhomogeneous spacetime it can vary from one normal trajectory to another.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The [long-wavelength approximation in cosmology](../../../cosmology.md#long-wavelength-approximation-in-cosmology) organizes equations in powers of $\epsilon\sim k/(aH)\ll1$, while allowing finite perturbation amplitudes. For fields and lapse varying on the same large spatial scale, a spatial derivative is of order $\epsilon$ relative to a temporal expansion scale. Intrinsic spatial curvature, scalar gradient energy, and second spatial derivatives of the lapse are therefore second order and can be neglected at leading order. First-gradient constraints must still be retained: they relate neighboring locally homogeneous patches. During [cosmic inflation](../../../cosmic-inflation.md), physical wavelengths stretch while the Hubble scale changes slowly, improving this expansion. Sharp spatial features or independently large anisotropic expansion require additional care.

Set the shift to zero, let $S^i{}_j=\widetilde K^i{}_j$, $S^2=S^i{}_jS^j{}_i$, and keep the lapse explicit. The normal scalar momentum is $\Pi=\dot\phi/N$, and the [shear-inclusive long-wavelength scalar equations](../../../cosmology.md#shear-inclusive-long-wavelength-scalar-equations) obtained from the given Einstein and scalar equations are

$$
\boxed{\begin{aligned}
\dot a&=NaH,&\dot\phi&=N\Pi,\\
\dot\Pi&=-N(3H\Pi+V_{,\phi}),&3H^2&=8\pi G(\Pi^2/2+V)+\tfrac12S^2,\\
\dot H&=-4\pi GN\Pi^2-\tfrac12NS^2,&\dot S^i{}_j&=-3NH S^i{}_j,\\
D_iH&=-4\pi G\Pi D_i\phi-\tfrac12D_jS^j{}_i.
\end{aligned}}
$$

Terms with two spatial gradients have been omitted in the time equations; the last equation is the retained first-gradient [momentum constraint](../../../numerical-relativity.md#momentum-constraint). The Friedmann-type equation is the [Hamiltonian constraint](../../../numerical-relativity.md#hamiltonian-constraint). To check the Hubble evolution, the trace equation gives $\dot H=-3NH^2+8\pi GNV$; inserting the [Hamiltonian constraint](../../../numerical-relativity.md#hamiltonian-constraint) gives the displayed kinetic and [cosmological shear](../../../cosmology.md#cosmological-shear) terms. Shear energy is not a spatial-gradient correction and cannot be discarded merely because the wavelength is large.

The trace-free evolution integrates immediately:

$$
\frac{d}{dt}(a^3S^i{}_j)=a^3(\dot S^i{}_j+3NH S^i{}_j)=0,\qquad\boxed{\widetilde K^i{}_j=C^i{}_j(\mathbf x)a^{-3}.}
$$

The arbitrary spatial integration tensor is trace free and must obey the initial constraints. This [inflationary shear damping](../../../cosmology.md#inflationary-shear-damping) suppresses anisotropic expansion exponentially during sustained inflation; its contribution $S^2$ falls as $a^{-6}$. It does not force the spatial conformal metric to be exactly flat: a frozen anisotropic shape or tensor perturbation can survive with negligible time-dependent [cosmological shear](../../../cosmology.md#cosmological-shear).

After this decaying [cosmological shear](../../../cosmology.md#cosmological-shear) mode and its first-gradient contribution become negligible, the equations simplify to $3H^2=8\pi G(\Pi^2/2+V)$ and $D_iH=-4\pi G\Pi D_i\phi$. Spatially differentiating the first relation gives

$$
6H D_iH=8\pi G(\Pi D_i\Pi+V_{,\phi}D_i\phi).
$$

Substitute the [momentum constraint](../../../numerical-relativity.md#momentum-constraint) and divide by $\Pi\ne0$ to obtain $D_i\Pi=-(3H+V_{,\phi}/\Pi)D_i\phi$. The time scalar equation, together with $\dot\phi=N\Pi$, similarly becomes $\dot\Pi=-(3H+V_{,\phi}/\Pi)\dot\phi$. Finally $\dot H=-4\pi G\Pi\dot\phi$. Thus the requested single-clock relations are

$$
\boxed{\begin{aligned}
\dot\Pi&=-\left(3H+\frac{V_{,\phi}}\Pi\right)\dot\phi,&D_i\Pi&=-\left(3H+\frac{V_{,\phi}}\Pi\right)D_i\phi,\\
\dot H&=-4\pi G\Pi\dot\phi,&D_iH&=-4\pi G\Pi D_i\phi.
\end{aligned}}
$$

These retain arbitrary lapse and reduce to proper-time expressions when $N=1$. The division assumes the scalar is a valid local clock; turning points with $\Pi=0$ need another regular variable or a limiting treatment. The shear-neglect step, rather than the long-wavelength expansion alone, is what permits these single-clock spatial relations.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Let $\alpha=\log a$, and define $A=3H+V_{,\phi}/\Pi$ on a patch with $\Pi\ne0$. In the shear-negligible [long-wavelength approximation in cosmology](../../../cosmology.md#long-wavelength-approximation-in-cosmology), the relations just derived give

$$
\dot\alpha=NH,\qquad\dot\phi=N\Pi,\qquad\dot\Pi=-NA\Pi,\qquad\dot H=-4\pi GN\Pi^2,
$$

with $\partial_iH=-4\pi G\Pi\partial_i\phi$ and $\partial_i\Pi=-A\partial_i\phi$. For the [nonlinear curvature covector](../../../cosmology.md#nonlinear-curvature-covector),

$$
\zeta_i=-\partial_i\alpha+\frac H\Pi\partial_i\phi,
$$

commuting coordinate derivatives gives

$$
\dot\zeta_i=-\partial_i(NH)+\left(\frac{\dot H}\Pi-\frac{H\dot\Pi}{\Pi^2}\right)\partial_i\phi+\frac H\Pi\partial_i(N\Pi).
$$

The two terms proportional to $\partial_iN$ cancel exactly. The remaining expression is

$$
\dot\zeta_i=-N\partial_iH+N\left(-4\pi G\Pi+\frac{HA}\Pi\right)\partial_i\phi+\frac{NH}\Pi\partial_i\Pi.
$$

Substituting the spatial relations cancels the gravitational terms and then the $A$ terms separately. Therefore

$$
\boxed{\dot\zeta_i\simeq0\qquad\text{on superhorizon scales in the shear-negligible single-clock regime}.}
$$

This is nonlinear in perturbation amplitude; only the spatial-gradient truncation and the decaying-shear approximation have been used. Conservation does not require a spatially homogeneous lapse. On a uniform-field slice, $\zeta_i=-\partial_i\log a$, making its interpretation as a conserved local spatial-curvature perturbation transparent, with the sign convention used here.

For ordinary attractor single-field inflation, conservation means that nonlinear curvature correlations already generated near horizon exit are transported to later superhorizon times without additional local growth. It does not prove that the perturbation is Gaussian: horizon-scale interactions, the nonlinear relation to the field perturbation, and quantum initial conditions can generate a nonzero bispectrum. In canonical slow-roll inflation that [primordial non-Gaussianity](../../../cosmology.md#primordial-non-gaussianity) is usually slow-roll suppressed; the [single-field inflation squeezed-limit consistency relation](../../../cosmology.md#single-field-inflation-squeezed-limit-consistency-relation) describes the effect of a long adiabatic mode on shorter modes under its stated attractor and initial-state assumptions. Strong local superhorizon [primordial non-Gaussianity](../../../cosmology.md#primordial-non-gaussianity) is therefore not generated merely by evolving this conserved variable. Entropy perturbations in multifield models, or non-attractor single-field phases for which the preceding single-clock and shear-neglect assumptions cannot be applied in this form, evade that inference. The result is a conservation theorem under explicit dynamical assumptions, not a blanket assertion that every single-field model has zero or small [primordial non-Gaussianity](../../../cosmology.md#primordial-non-gaussianity).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
