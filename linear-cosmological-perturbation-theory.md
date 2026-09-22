# Linear cosmological perturbation theory

↑ **Parent:** [Cosmology](cosmology.md)

This is the first-order sector of [cosmological perturbation theory](cosmology.md#cosmological-perturbation-theory).

Linear cosmological perturbation theory expands the metric and matter fields to first order about a homogeneous and isotropic [Friedmann-Lemaître-Robertson-Walker metric](cosmology.md#friedmann-lemaitre-robertson-walker-metric).

**Table of contents**

- [Longitudinal displacement in linear dust perturbations](#longitudinal-displacement-in-linear-dust-perturbations)
- [Small determinant does not imply a small metric perturbation](#small-determinant-does-not-imply-a-small-metric-perturbation)
- [Gauge transformation in cosmological perturbation theory](#gauge-transformation-in-cosmological-perturbation-theory)
  - [Synchronous-to-Newtonian scalar Fourier transformation](#synchronous-to-newtonian-scalar-fourier-transformation)
  - [Scalar gauge transformation with trace-free spatial shear](#scalar-gauge-transformation-with-trace-free-spatial-shear)
  - [Density perturbation gauge transformation](#density-perturbation-gauge-transformation)
  - [Linear metric gauge-transformation law](#linear-metric-gauge-transformation-law)
- [Vector cosmological perturbation](#vector-cosmological-perturbation)
  - [Photon energy redshift from a vector metric perturbation](#photon-energy-redshift-from-a-vector-metric-perturbation)
- [Adiabatic mode](#adiabatic-mode)
  - [Superhorizon growing density mode of adiabatic matter and radiation](#superhorizon-growing-density-mode-of-adiabatic-matter-and-radiation)
- [Tensor cosmological perturbation](#tensor-cosmological-perturbation)
  - [Tensor normalization with unit-norm polarization tensors](#tensor-normalization-with-unit-norm-polarization-tensors)
  - [Helicity selection for tensor CMB multipoles](#helicity-selection-for-tensor-cmb-multipoles)
    - [Long-wavelength tensor CMB quadrupole and octupole](#long-wavelength-tensor-cmb-quadrupole-and-octupole)
  - [Photon energy redshift from a tensor metric perturbation](#photon-energy-redshift-from-a-tensor-metric-perturbation)
  - [Neutrino tensor anisotropic stress](#neutrino-tensor-anisotropic-stress)
    - [Neutrino tensor free-streaming kernel](#neutrino-tensor-free-streaming-kernel)
    - [Gravitational-wave damping by free-streaming neutrinos](#gravitational-wave-damping-by-free-streaming-neutrinos)
- [Scalar cosmological perturbation](#scalar-cosmological-perturbation)
  - [Weyl lensing potential](#weyl-lensing-potential)
  - [Scalar photon energy redshift](#scalar-photon-energy-redshift)
  - [Perturbed Klein-Gordon equation with background lapse](#perturbed-klein-gordon-equation-with-background-lapse)
  - [Comoving gauge in cosmology](#comoving-gauge-in-cosmology)
  - [Uniform-density curvature perturbation](#uniform-density-curvature-perturbation)
    - [Uniform-density curvature sign test](#uniform-density-curvature-sign-test)
    - [Superhorizon conservation of uniform-density curvature](#superhorizon-conservation-of-uniform-density-curvature)
  - [Scalar gauge transformations with a background lapse](#scalar-gauge-transformations-with-a-background-lapse)
    - [Synchronous-to-Newtonian density transformation with a lapse](#synchronous-to-newtonian-density-transformation-with-a-lapse)
  - [Scalar shear potential](#scalar-shear-potential)
  - [Scalar expansion perturbation](#scalar-expansion-perturbation)
    - [Positive-shift scalar shear convention](#positive-shift-scalar-shear-convention)
  - [Synchronous gauge in cosmology](#synchronous-gauge-in-cosmology)
    - [Synchronous-to-Newtonian transformation with positive spatial perturbations](#synchronous-to-newtonian-transformation-with-positive-spatial-perturbations)
      - [Photon redshift identity with positive spatial perturbations](#photon-redshift-identity-with-positive-spatial-perturbations)
    - [Synchronous gauge fixing by coordinate displacement](#synchronous-gauge-fixing-by-coordinate-displacement)
    - [Linear perfect-fluid stress tensor in synchronous gauge](#linear-perfect-fluid-stress-tensor-in-synchronous-gauge)
    - [Synchronous perfect-fluid density equation](#synchronous-perfect-fluid-density-equation)
    - [Residual synchronous-gauge freedom](#residual-synchronous-gauge-freedom)
      - [Synchronous density gauge mode](#synchronous-density-gauge-mode)
    - [Cosmological Euler equation in synchronous gauge](#cosmological-euler-equation-in-synchronous-gauge)
  - [Newtonian gauge](#newtonian-gauge)
    - [Cosmological Newtonian potential](#cosmological-newtonian-potential)
    - [Conformal optical metric for scalar perturbations](#conformal-optical-metric-for-scalar-perturbations)
      - [First-order photon trajectory in scalar perturbations](#first-order-photon-trajectory-in-scalar-perturbations)
    - [Gravitational potential evolution of a barotropic fluid](#gravitational-potential-evolution-of-a-barotropic-fluid)
    - [Cosmological Euler equation](#cosmological-euler-equation)
      - [Linear matter density equation in Newtonian gauge](#linear-matter-density-equation-in-newtonian-gauge)
    - [Cosmological Poisson equation](#cosmological-poisson-equation)
  - [Scalar velocity potential](#scalar-velocity-potential)
  - [Scalar anisotropic stress](#scalar-anisotropic-stress)
    - [Scalar neutrino anisotropic stress](#scalar-neutrino-anisotropic-stress)
      - [Radiation-era adiabatic potentials with free-streaming neutrinos](#radiation-era-adiabatic-potentials-with-free-streaming-neutrinos)
  - [Flat gauge in cosmology](#flat-gauge-in-cosmology)
- [Cosmological transfer function](#cosmological-transfer-function)
  - [Radiation acoustic transfer function](#radiation-acoustic-transfer-function)
    - [Subhorizon radiation acoustic oscillations](#subhorizon-radiation-acoustic-oscillations)
      - [Matter-era forced radiation response](#matter-era-forced-radiation-response)
      - [Suppressed cold-matter forcing by rapid radiation oscillations](#suppressed-cold-matter-forcing-by-rapid-radiation-oscillations)
  - [Cold-dark-matter transfer function](#cold-dark-matter-transfer-function)
    - [Frozen-radiation approximation to the matter transfer function](#frozen-radiation-approximation-to-the-matter-transfer-function)
    - [Scale-independent matter suppression by a coasting fluid](#scale-independent-matter-suppression-by-a-coasting-fluid)
    - [Sharp-equality cold-dark-matter transfer approximation](#sharp-equality-cold-dark-matter-transfer-approximation)
    - [Matter-era density transfer from primordial curvature](#matter-era-density-transfer-from-primordial-curvature)
    - [Asymptotic cold-dark-matter power spectrum](#asymptotic-cold-dark-matter-power-spectrum)
    - [Logarithmic small-scale matter transfer](#logarithmic-small-scale-matter-transfer)
      - [Logarithmic high-wavenumber density-spectrum transfer](#logarithmic-high-wavenumber-density-spectrum-transfer)
  - [Baryon transfer function](#baryon-transfer-function)
    - [Baryon--cold-dark-matter relative density mode](#baryon-cold-dark-matter-relative-density-mode)

## Longitudinal displacement in linear dust perturbations

↑ **Parent:** [Linear cosmological perturbation theory](linear-cosmological-perturbation-theory.md)

Mass conservation in a Lagrangian dust displacement gives $1+\delta=\det(I+\nabla_q\psi)^{-1}$, hence $\delta=-\nabla_q\cdot\psi$ to first order. The perturbing [gravitational potential](classical-mechanics.md#newtonian-potential-of-a-point-mass) determines the longitudinal part of the force, so the displayed equation holds for the curl-free displacement under the usual homogeneous boundary convention. A divergence-free transverse displacement instead satisfies $\ddot\psi_T+2H\dot\psi_T=0$. Taking the divergence gives $\ddot\delta+2H\dot\delta-4\pi G\bar\rho\delta=0$ without assuming the full displacement is longitudinal. The background Poisson equation with positive source requires $\nabla\Phi_0=+4\pi G\bar\rho r/3$.

## Small determinant does not imply a small metric perturbation

↑ **Parent:** [Linear cosmological perturbation theory](linear-cosmological-perturbation-theory.md)

For $h_{ij}=\operatorname{diag}(L,0,0)$, the determinant is zero for every $L$, even when one perturbation component is arbitrarily large. Linearized metric theory instead requires the eigenvalues of $h$ relative to the background spatial metric to be small, equivalently all its components in a background orthonormal frame to be small. The determinant of $1+h$ then expands as $1+\operatorname{tr}h+O(h^2)$, and the volume element as $1+\operatorname{tr}h/2+O(h^2)$.

## Gauge transformation in cosmological perturbation theory

↑ **Parent:** [Linear cosmological perturbation theory](linear-cosmological-perturbation-theory.md)

A cosmological gauge transformation changes the identification of a perturbed spacetime with its homogeneous background. Individual field perturbations can change without changing physical observables. At first order the metric change is the [linear metric gauge-transformation law](#linear-metric-gauge-transformation-law); matter scalars obey the corresponding background-shift rule.

### Synchronous-to-Newtonian scalar Fourier transformation

↑ **Parent:** [Gauge transformation in cosmological perturbation theory](#gauge-transformation-in-cosmological-perturbation-theory)

For a nonzero [Fourier mode](fourier-analysis.md#fourier-mode) in [synchronous gauge](#synchronous-gauge-in-cosmology), write $h_{ij}=h\delta_{ij}/3+h_s(\widehat k_i\widehat k_j-\delta_{ij}/3)$. Under the passive displacement $\xi^\mu=(T,i\widehat k_iL)e^{i\mathbf k\cdot\mathbf x}$, cancellation of spatial scalar shear requires $h_s+2kL=0$, and cancellation of the shift requires $kT-L'=0$. The resulting [cosmological Newtonian potential](#cosmological-newtonian-potential) is $\Phi=(h_s''+\mathcal Hh_s')/(2k^2)$ and the spatial potential is $\Psi=-(h-h_s)/6-\mathcal Hh_s'/(2k^2)$. Both remain unchanged under [residual synchronous-gauge freedom](#residual-synchronous-gauge-freedom), for which $T'+\mathcal HT=0$ and $L'=kT$.

### Scalar gauge transformation with trace-free spatial shear

↑ **Parent:** [Gauge transformation in cosmological perturbation theory](#gauge-transformation-in-cosmological-perturbation-theory)

For the conformal metric with $g_{0i}=-a^2\partial_iB$ and trace-free scalar spatial shear $E_{ij}=(\partial_i\partial_j-\delta_{ij}\nabla^2/3)E$, the passive coordinate change $\widetilde\eta=\eta+T$, $\widetilde x^i=x^i+\partial^iL$ gives the displayed rules and $\widetilde\phi=\phi+\mathcal HT+\nabla^2L/3$. The combination $C=\phi+\nabla^2E/3$ changes by $\mathcal HT$, while $B+v$ changes by $T$. Hence $\mathcal R=-C+\mathcal H(B+v)$ is the [comoving curvature perturbation](cosmic-inflation.md#comoving-curvature-perturbation) in this sign convention.

### Density perturbation gauge transformation

↑ **Parent:** [Gauge transformation in cosmological perturbation theory](#gauge-transformation-in-cosmological-perturbation-theory)

Density is a [scalar field](quantum-field-theory.md#scalar-field). Under a first-order time shift $\widetilde\tau=\tau+T$, its background changes by $\bar\rho'T$, so its perturbation changes by the negative of that amount. Spatial shifts act only at second order on a homogeneous background density.

### Linear metric gauge-transformation law

↑ **Parent:** [Gauge transformation in cosmological perturbation theory](#gauge-transformation-in-cosmological-perturbation-theory)

For the passive convention $\widetilde x=x+\xi$, expanding the tensor coordinate-transformation law around a fixed background gives this [Lie derivative](differential-form.md#lie-derivative-of-a-differential-form) formula. The background time shift and Jacobian terms must both be retained. On an [FLRW metric](cosmology.md#friedmann-lemaitre-robertson-walker-metric), the scalar lapse, shift and spatial potentials transform under two scalar coordinate functions.

## Vector cosmological perturbation

↑ **Parent:** [Linear cosmological perturbation theory](linear-cosmological-perturbation-theory.md)

A vector cosmological perturbation is the transverse-vector sector of linear metric and matter perturbations. For a [Fourier mode](fourier-analysis.md#fourier-mode) with nonzero wavevector $\mathbf k$, transversality removes the component parallel to $\mathbf k$, leaving two [helicity](special-relativity.md#helicity) components. In a gauge with $ds^2=a^2[-d\eta^2+2B_i d\eta dx^i+\delta_{ij}dx^i dx^j]$, $\partial_iB_i=0$ describes the vector metric perturbation.

### Photon energy redshift from a vector metric perturbation

↑ **Parent:** [Vector cosmological perturbation](#vector-cosmological-perturbation)

For the metric in [vector cosmological perturbation](#vector-cosmological-perturbation), an [orthonormal tetrad](general-relativity.md#orthonormal-frame-in-spacetime) is $E_0=a^{-1}\partial_\eta$, $E_i=a^{-1}(B_i\partial_\eta+\partial_i)$ to first order. A [photon](quantum-mechanics.md#photon) has $p^0=(\epsilon/a^2)(1+B_ie^i)$ and $p^i=(\epsilon/a^2)e^i$, so the covariant component is $p_0=-\epsilon+O(B^2)$. The covariant [geodesic equation](riemannian-geometry.md#geodesic-equation) gives $dp_0/d\eta=(2p^0)^{-1}\partial_\eta g_{\alpha\beta}p^\alpha p^\beta=\epsilon e^i\dot B_i$. The [derivative](calculus.md#derivative) of the [scale factor](cosmology.md#scale-factor-cosmology) cancels by the [null vector](special-relativity.md#null-vector) condition, proving the redshift formula.

## Adiabatic mode

↑ **Parent:** [Linear cosmological perturbation theory](linear-cosmological-perturbation-theory.md)

An adiabatic mode is a long-wavelength physical perturbation whose leading local field configuration is generated by a residual gauge transformation. Its action on shorter modes produces a cosmological soft theorem or consistency relation.

### Superhorizon growing density mode of adiabatic matter and radiation

↑ **Parent:** [Adiabatic mode](#adiabatic-mode)

An adiabatic perturbation obeys $\Delta_r=(4/3)\Delta_c$. In a radiation background this makes the cold-matter density equation $\Delta_c''+\Delta_c'/\tau=4\Delta_c/\tau^2$, whose growing solution is $\tau^2$. In a matter background it instead becomes $\Delta_c''+2\Delta_c'/\tau=6\Delta_c/\tau^2$, with the same growing conformal-time exponent and a different scale-factor dependence.

## Tensor cosmological perturbation

↑ **Parent:** [Linear cosmological perturbation theory](linear-cosmological-perturbation-theory.md)

A tensor cosmological perturbation is the transverse, trace-free part of a metric perturbation about a [Friedmann-Lemaître-Robertson-Walker metric](cosmology.md#friedmann-lemaitre-robertson-walker-metric). In conformal coordinates, its spatial metric has the form $g_{ij}=a^2(\delta_{ij}+h_{ij})$, with $\partial_i h_{ij}=0$ and $h_{ii}=0$. Its two independent polarizations describe a [gravitational wave](general-relativity.md#gravitational-wave). [Neutrino tensor anisotropic stress](#neutrino-tensor-anisotropic-stress) can damp its evolution through [neutrino free streaming](linear-cosmological-density-perturbation.md#neutrino-free-streaming).

### Tensor normalization with unit-norm polarization tensors

↑ **Parent:** [Tensor cosmological perturbation](#tensor-cosmological-perturbation)

If the tensor metric perturbation is $h_{ij}=2E_{ij}$ and the polarization tensors have contraction $M^{(p)}_{ij}M^{(q)*ij}=\delta_{pq}$, the quadratic action for each Fourier amplitude is $(M_{\rm Pl}^2/2)\int a^2(|\psi_{(p)}'|^2-k^2|\psi_{(p)}|^2)$. Thus each helicity is normalized like a real massless scalar by the displayed rescaling. Its power per polarization is $(H_k/(2\pi M_{\rm Pl}))^2$. Factors of two in other tensor spectra depend on the definitions of the metric amplitude, the polarization norm and whether both helicities are summed.

### Helicity selection for tensor CMB multipoles

↑ **Parent:** [Tensor cosmological perturbation](#tensor-cosmological-perturbation)

A complex helicity-$+2$ plane wave along the $z$ axis has polarization contraction $\sin^2\theta e^{2i\varphi}$. Its remaining [tensor CMB line-of-sight source](cosmic-microwave-background-anisotropy.md#tensor-cmb-line-of-sight-source) depends only on $\cos\theta$. Orthogonality of the azimuthal factors of [spherical harmonics](analysis.md#spherical-harmonic) therefore restricts its temperature coefficients to $m=2$. A real perturbation also includes the conjugate mode.

#### Long-wavelength tensor CMB quadrupole and octupole

↑ **Parent:** [Helicity selection for tensor CMB multipoles](#helicity-selection-for-tensor-cmb-multipoles)

For a matter-era superhorizon tensor with $h=h_{\mathrm{prim}}[1-(k\eta)^2/10+\cdots]$, the [tensor CMB line-of-sight source](cosmic-microwave-background-anisotropy.md#tensor-cmb-line-of-sight-source) gives $\Theta_{22}\propto h_{\mathrm{prim}}(k\eta_0)^2$ and $\Theta_{32}/\Theta_{22}=-ik\eta_0/(3\sqrt7)$ when $\eta_*\ll\eta_0$. The extra spatial phase makes the octupole one order smaller.

### Photon energy redshift from a tensor metric perturbation

↑ **Parent:** [Tensor cosmological perturbation](#tensor-cosmological-perturbation)

For a [tensor cosmological perturbation](#tensor-cosmological-perturbation) $h_{ij}$, the time [geodesic equation](riemannian-geometry.md#geodesic-equation) in a local [orthonormal tetrad](general-relativity.md#orthonormal-frame-in-spacetime) gives $d\log\epsilon/d\eta=-\dot h_{ij}e^ie^j/2$. The photon comoving energy removes the background redshift; the dot is a partial time derivative, whereas the energy derivative follows the ray.

### Neutrino tensor anisotropic stress

↑ **Parent:** [Tensor cosmological perturbation](#tensor-cosmological-perturbation)

For massless [neutrinos](standard-model.md#neutrino) with a temperature perturbation $\Theta$ and background [energy density](statistical-physics.md#energy-density) $\bar\rho_\nu$, the physical trace-free spatial [stress-energy tensor](general-relativity.md#stress-energy-tensor) is

$$
\pi_\nu^{ij}=4\bar\rho_\nu\int\frac{d\Omega_e}{4\pi}
\Theta\left(e^ie^j-\frac13\delta^{ij}\right).
$$

Some conventions define $\Pi^{ij}=-\pi_\nu^{ij}$ and correspondingly reverse the sign of the stress source in the gravitational-wave equation.

#### Neutrino tensor free-streaming kernel

↑ **Parent:** [Neutrino tensor anisotropic stress](#neutrino-tensor-anisotropic-stress)

Projecting free-streaming [neutrinos](standard-model.md#neutrino) onto the tensor [spherical harmonic](analysis.md#spherical-harmonic) gives

$$
K(x)=\frac1{16}\int_{-1}^{1}(1-\mu^2)^2e^{-ix\mu}\,d\mu
=\frac{j_2(x)}{x^2},\qquad K(0)=\frac1{15}.
$$

Here $j_2$ is a [Spherical Bessel function](analysis.md#spherical-bessel-function). The continuous value at zero follows by integrating $(1-\mu^2)^2$, whose integral is $16/15$.

#### Gravitational-wave damping by free-streaming neutrinos

↑ **Parent:** [Neutrino tensor anisotropic stress](#neutrino-tensor-anisotropic-stress)

For either tensor [helicity](special-relativity.md#helicity), [neutrino free streaming](linear-cosmological-density-perturbation.md#neutrino-free-streaming) produces the memory equation

$$
\ddot h+2\mathcal H\dot h+k^2h
=-24\mathcal H^2f_\nu\int_0^\eta
K(k(\eta-\eta'))\dot h(\eta')\,d\eta',
\qquad
f_\nu=\frac{\bar\rho_\nu}{\bar\rho_{\rm tot}}.
$$

The [neutrino tensor free-streaming kernel](#neutrino-tensor-free-streaming-kernel) encodes the angular propagation of the perturbation. Energy transferred to neutrino directional anisotropy damps the oscillation amplitude of a [gravitational wave](general-relativity.md#gravitational-wave) after horizon entry. This effect was calculated by [Weinberg](https://arxiv.org/abs/astro-ph/0306304).

## Scalar cosmological perturbation

↑ **Parent:** [Linear cosmological perturbation theory](linear-cosmological-perturbation-theory.md)

A scalar cosmological perturbation transforms as a scalar under spatial rotations and can be represented using scalar metric potentials, density and pressure perturbations, and the longitudinal part of the fluid velocity.

### Weyl lensing potential

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)

The average of the two [conformal Newtonian gauge](#newtonian-gauge) potentials controls scalar [gravitational lensing](general-relativity.md#gravitational-lensing). A conformal rescaling makes the spatial optical metric flat and its time component $1+4\Psi$ to first order. Vanishing [scalar anisotropic stress](#scalar-anisotropic-stress) makes $\phi=\psi$ in general relativity, but lensing depends on their sum even when they differ.

### Scalar photon energy redshift

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)

For the [Newtonian gauge in cosmology](#newtonian-gauge) with potentials $\psi,\phi$, photon comoving momentum $\epsilon$ obeys $d\ln\epsilon/d\eta=\phi'-\mathbf e\cdot\nabla\psi=-d\psi/d\eta+\phi'+\psi'$. The homogeneous physical-energy redshift is separated by $E=\epsilon/a$. The total derivative follows the unperturbed photon path at linear order.

### Perturbed Klein-Gordon equation with background lapse

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)

Let $\mathcal D=\bar N^{-1}\partial_t$ and $\bar\Pi=\mathcal D\bar\phi$. For negative-expansion [extrinsic curvature of a spatial hypersurface](numerical-relativity.md#extrinsic-curvature-of-a-spatial-hypersurface), its trace perturbation is $\kappa$. With $\delta\Pi=\mathcal D\delta\phi-\bar\Pi\Psi$, scalar evolution is $\mathcal D\delta\Pi-\Psi\mathcal D\bar\Pi+3H\delta\Pi-\kappa\bar\Pi-\Delta\delta\phi+V_{,\phi\phi}\delta\phi=0$. Combining background acceleration terms produces the standard lapse source $-\bar\Pi(\kappa+\mathcal D\Psi-3H\Psi)+2\Psi V_{,\phi}$.

### Comoving gauge in cosmology

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)

A [comoving gauge in cosmology](#comoving-gauge-in-cosmology) chooses hypersurfaces with zero scalar momentum density for the specified fluid or total system. For cold [pressureless matter](cosmology.md#pressureless-matter) it can be implemented by taking the matter velocity potential to vanish. The choice of component must be stated in a multi-fluid system; [density contrasts](linear-cosmological-density-perturbation.md#density-contrast) on this slicing can differ from those in a Newtonian or spatially flat gauge.

### Uniform-density curvature perturbation

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)

The uniform-density curvature perturbation is the spatial scalar curvature measured on density-defined hypersurfaces, with an explicitly chosen sign convention. If the spatial scalar potentials are $C,E$, one convention is $\zeta=-C+\nabla^2E/3+\mathcal H\delta\rho/\bar\rho'$. Its two time-shift terms cancel under a [cosmological gauge transformation](#gauge-transformation-in-cosmological-perturbation-theory). The density derivative must be nonzero. This is a different slicing from the [comoving curvature perturbation](cosmic-inflation.md#comoving-curvature-perturbation), although the variables are related for regular adiabatic long-wavelength modes, with signs depending on convention.

#### Uniform-density curvature sign test

↑ **Parent:** [Uniform-density curvature perturbation](#uniform-density-curvature-perturbation)

For spatial metric $a^2(1-2\Phi)\delta_{ij}$, the combination $\zeta=-\Phi+\delta\rho/[3(\bar\rho+\bar P)]$ is invariant under a time displacement: $\Phi$ shifts by $\bar NH T$ and $\delta\rho$ by $3\bar NH(\bar\rho+\bar P)T$. The opposite overall sign is also valid. The sum $\Phi+\delta\rho/[3(\bar\rho+\bar P)]$ is not invariant. This is a useful convention check before applying [superhorizon conservation of uniform-density curvature](#superhorizon-conservation-of-uniform-density-curvature).

#### Superhorizon conservation of uniform-density curvature

↑ **Parent:** [Uniform-density curvature perturbation](#uniform-density-curvature-perturbation)

With the convention $\zeta=\Phi-\delta\rho/[3(\bar\rho+\bar P)]$, energy conservation gives $\zeta'=\mathcal H\delta P_{\rm nad}/(\bar\rho+\bar P)+(\nabla\cdot\mathbf v)/3$. The [non-adiabatic pressure perturbation](cosmic-inflation.md#non-adiabatic-pressure-perturbation) vanishes for [adiabatic cosmological perturbations](cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions), and regular velocity gradients are suppressed on [superhorizon scales](cosmic-inflation.md#superhorizon-scale). Curvature is then conserved to leading gradient order, allowing primordial initial conditions to be propagated between cosmological eras.

### Scalar gauge transformations with a background lapse

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)

For $N=\bar N(1+\Psi)$, $g_{0i}=a^2\partial_iB$ and spatial scalar convention $h_{ij}=a^2[(1-2\Phi)\delta_{ij}-2\partial_i\partial_jE]$, a passive displacement $(\xi^0,\partial^i\lambda)$ gives $\widetilde\Psi=\Psi-\dot\xi^0-(\dot{\bar N}/\bar N)\xi^0$, $\widetilde B=B+\bar N^2\xi^0/a^2-\dot\lambda$, $\widetilde\Phi=\Phi+(\dot a/a)\xi^0$ and $\widetilde E=E+\lambda$. These follow from subtracting the background metric Lie derivative.

#### Synchronous-to-Newtonian density transformation with a lapse

↑ **Parent:** [Scalar gauge transformations with a background lapse](#scalar-gauge-transformations-with-a-background-lapse)

For spatial scalar convention $g_{ij}=a^2[(1-2\Psi)\delta_{ij}-2E_{,ij}]$ and $g_{0i}=a^2B_{,i}$, a passive gauge displacement gives $\widetilde E=E+\lambda$ and $\widetilde B=B-\dot\lambda+\bar N^2\xi^0/a^2$. Moving from [synchronous gauge](#synchronous-gauge-in-cosmology) to [Newtonian gauge](#newtonian-gauge) therefore requires $\lambda=-E_S$ and $\xi^0=-a^2\dot E_S/\bar N^2$. A scalar density transforms by $\delta\widetilde\rho=\delta\rho-\dot{\bar\rho}\xi^0$, giving the displayed [density contrast](linear-cosmological-density-perturbation.md#density-contrast) relation. Keeping the background [lapse function](numerical-relativity.md#lapse-function) explicit prevents cosmic-time and conformal-time factors from being confused.

### Scalar shear potential

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)

For the negative [extrinsic curvature](differential-geometry.md#extrinsic-curvature) convention and a [shift vector](numerical-relativity.md#shift-vector) entering the line element as $dx^i-N^i dt$, the trace-free scalar curvature perturbation is $\delta K^i{}_j{}_{\rm TF}=-(\partial^i\partial_j-\delta^i_j\Delta/3)\chi$. Here spatial raised derivatives use $a^{-2}\delta^{ij}$, so $\Delta=a^{-2}\nabla^2$. Changing the sign of the metric [shift vector](numerical-relativity.md#shift-vector) changes the corresponding definition of $\chi$.

### Scalar expansion perturbation

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)

With negative [extrinsic curvature](differential-geometry.md#extrinsic-curvature) convention, the background [trace](linear-algebra.md#matrix-trace) is $\bar K=-3H$. The scalar expansion perturbation is $\kappa=K+3H$. For [lapse function](numerical-relativity.md#lapse-function) $N=\bar N(1+\Psi)$, [induced metric](riemannian-geometry.md#induced-metric) $h_{ij}=a^2[(1-2\Phi)\delta_{ij}+2E_{,ij}]$ and [shift vector](numerical-relativity.md#shift-vector) $N_i=-a^2B_{,i}$, it is $\kappa=3(\dot\Phi/\bar N+H\Psi)-\Delta\chi$, where $\chi$ is the [scalar shear potential](#scalar-shear-potential). The expansion of the future normal congruence is $-K$, so its perturbation has the opposite sign.

#### Positive-shift scalar shear convention

↑ **Parent:** [Scalar expansion perturbation](#scalar-expansion-perturbation)

For $N_i=a^2B_{,i}$, $\gamma_{ij}=a^2[(1-2\Phi)\delta_{ij}+2E_{,ij}]$ and $K_{ij}=-(\dot\gamma_{ij}-D_iN_j-D_jN_i)/(2N)$, put $\chi_+=a^2(B-\dot E)/\bar N$. Then $K^i{}_j=-H\delta^i{}_j+(\dot\Phi/\bar N+H\Psi)\delta^i{}_j+\partial^i\partial_j\chi_+$ and $\kappa=3(\dot\Phi/\bar N+H\Psi)+\Delta\chi_+$. Defining $\chi=-\chi_+$ instead makes the trace-free tensor coefficient negative and the trace gradient term $-\Delta\chi$. A sign change must affect both pieces.

### Synchronous gauge in cosmology

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)

Synchronous gauge sets the lapse and shift perturbations to zero, $h_{0\mu}=0$. Its coordinates follow freely falling observers, but residual coordinate freedom produces gauge modes that must be distinguished from physical perturbations.

#### Synchronous-to-Newtonian transformation with positive spatial perturbations

↑ **Parent:** [Synchronous gauge in cosmology](#synchronous-gauge-in-cosmology)

Define $\delta g_{ij}=a^2h_{ij}$ and $h_{ij}=h\delta_{ij}/3+(\hat k_i\hat k_j-\delta_{ij}/3)h_S$. Under the passive coordinate shift $\tilde\tau=\tau+T e^{i\mathbf k\cdot\mathbf x}$ and $\tilde x^i=x^i+i\hat k^iL e^{i\mathbf k\cdot\mathbf x}$, removing the traceless spatial perturbation gives $L=h_S/(2k)$. Removing the mixed time-space metric gives $T=L'/k=h_S'/(2k^2)$. The remaining diagonal metric components are the displayed Newtonian potentials. This sign convention is opposite to defining the synchronous perturbation by $g_{ij}=-a^2(\delta_{ij}+h_{ij})$.

##### Photon redshift identity with positive spatial perturbations

↑ **Parent:** [Synchronous-to-Newtonian transformation with positive spatial perturbations](#synchronous-to-newtonian-transformation-with-positive-spatial-perturbations)

Let $q=\mathbf k\cdot\mathbf n$, $E=e^{iq(\tau-\tau_0)}$ and $T=h_S'/(2k^2)$. The [synchronous-to-Newtonian transformation with positive spatial perturbations](#synchronous-to-newtonian-transformation-with-positive-spatial-perturbations) gives $(h'-h_S')/6=\Phi'+\Psi'+T''$. Since $[E(T'-iqT)]'=E(T''+q^2T)$, the displayed identity follows by integration. The emission endpoint combines intrinsic and velocity shifts into the ordinary [Sachs-Wolfe effect](cosmic-microwave-background-anisotropy.md#sachs-wolfe-effect); the local observer endpoint is a monopole plus a dipole. Without [anisotropic stress](general-relativity.md#anisotropic-stress) the remaining integral is the [Integrated Sachs-Wolfe effect](cosmic-microwave-background-anisotropy.md#integrated-sachs-wolfe-effect), $2\int E\Phi' d\tau$. The angular term in the synchronous contraction is positive for this metric convention.

#### Synchronous gauge fixing by coordinate displacement

↑ **Parent:** [Synchronous gauge in cosmology](#synchronous-gauge-in-cosmology)

For the [FRW metric](cosmology.md#friedmann-lemaitre-robertson-walker-metric) in [conformal time](cosmology.md#conformal-time), a displacement $\xi^\mu=(\alpha,\xi^i)$ changes a raw [metric perturbation](general-relativity.md#linearized-gravity) by $q_{\mu\nu}\mapsto q_{\mu\nu}-\mathcal L_\xi\bar g_{\mu\nu}$. The displayed first-order time equations set the lapse and shift perturbations to zero. They can be integrated locally for smooth perturbations, demonstrating accessibility of [synchronous gauge in cosmology](#synchronous-gauge-in-cosmology). Their [homogeneous solutions](differential-equation.md#homogeneous-solution) leave residual spatial functions, so the gauge is not fully fixed. A globally regular synchronous chart need not survive caustics of its freely falling congruence.

#### Linear perfect-fluid stress tensor in synchronous gauge

↑ **Parent:** [Synchronous gauge in cosmology](#synchronous-gauge-in-cosmology)

For constant $P=w\rho$, the [perfect fluid](general-relativity.md#perfect-fluid) stress tensor and inverse perturbed spatial metric give $T^{ij}=a^{-2}w\bar\rho[(1+\delta)\delta^{ij}-h^{ij}]$ at first order. Normalizing the velocity makes $u^0=a^{-1}$ at this order. [Stress-energy conservation](general-relativity.md#stress-energy-conservation) yields the [synchronous perfect-fluid density equation](#synchronous-perfect-fluid-density-equation) and [Cosmological Euler equation in synchronous gauge](#cosmological-euler-equation-in-synchronous-gauge); the pressure projection includes $v_i\bar P'$, which changes the velocity damping from $\mathcal H$ to $(1-3w)\mathcal H$.

// Target: cosmology.bigb

#### Synchronous perfect-fluid density equation

↑ **Parent:** [Synchronous gauge in cosmology](#synchronous-gauge-in-cosmology)

For constant $P=w\rho$ and [velocity potential](fluid-mechanics.md#velocity-potential) $v_i=ik_i\theta$, [stress-energy conservation](general-relativity.md#stress-energy-conservation) gives the displayed density equation in [synchronous gauge in cosmology](#synchronous-gauge-in-cosmology). Here $h$ is the trace of the spatial metric perturbation, and primes denote [conformal time](cosmology.md#conformal-time). In particular cold baryons obey $\delta_b'=k^2\theta_b-h'/2$. A positive sign in front of $k^2\theta_b$ on the left contradicts this potential convention.

#### Residual synchronous-gauge freedom

↑ **Parent:** [Synchronous gauge in cosmology](#synchronous-gauge-in-cosmology)

Preserving $\Psi=B=0$ under the [scalar gauge transformations with a background lapse](#scalar-gauge-transformations-with-a-background-lapse) requires $\bar N\xi^0=C(\mathbf x)$ and $\dot\lambda=C(\mathbf x)\bar N/a^2$. Thus arbitrary spatial functions $C,D$ remain after imposing [synchronous gauge in cosmology](#synchronous-gauge-in-cosmology). This freedom can generate changes in the remaining scalar metric perturbations.

##### Synchronous density gauge mode

↑ **Parent:** [Residual synchronous-gauge freedom](#residual-synchronous-gauge-freedom)

A residual synchronous time displacement $\xi^0=C(\mathbf x)/a$ changes a fluid [density contrast](linear-cosmological-density-perturbation.md#density-contrast) by $-\bar\rho'\xi^0/\bar\rho$. For constant equation of state this gives the displayed mode: it scales as $\tau^{-2}$ during [radiation domination](linear-cosmological-density-perturbation.md#radiation-domination) and as $\tau^{-3}$ during [matter domination](linear-cosmological-density-perturbation.md#matter-domination). Such density changes alone do not indicate physical structure growth. Choosing the cold-matter rest frame fixes the residual time displacement, while a spatial relabeling fixes the remaining integration convention for the metric trace.

#### Cosmological Euler equation in synchronous gauge

↑ **Parent:** [Synchronous gauge in cosmology](#synchronous-gauge-in-cosmology)

For scalar perturbations of a generic fluid in cosmic time, momentum conservation in [synchronous gauge in cosmology](#synchronous-gauge-in-cosmology) gives

$$
\delta P+\nabla^2\pi^S
+\partial_t[(\bar\rho+\bar P)\delta u]
+3H(\bar\rho+\bar P)\delta u=0.
$$

### Newtonian gauge

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Newtonian_gauge)

Newtonian gauge removes scalar shear and writes scalar metric perturbations in terms of gravitational potentials. The fluid Euler equation then contains an explicit gradient of the Newtonian potential.

#### Cosmological Newtonian potential

↑ **Parent:** [Newtonian gauge](#newtonian-gauge)

The potential $\Phi$ describes the lapse perturbation in [conformal Newtonian gauge](#newtonian-gauge). The spatial curvature perturbation is conventionally denoted $\Psi$; the two are equal when the linear scalar anisotropic stress vanishes. On scales where the Newtonian limit applies, $\Phi$ agrees with the peculiar gravitational potential. Its Fourier-mode variance and the power spectrum of a comoving curvature perturbation are different observables.

#### Conformal optical metric for scalar perturbations

↑ **Parent:** [Newtonian gauge](#newtonian-gauge)

Rescale the perturbed cosmological metric by $a^{-2}(1+2\phi)$. To first order, its spatial part is Euclidean and only its lapse is perturbed. The unparameterized [null geodesics](special-relativity.md#null-geodesic) are unchanged. The nonzero linear connection coefficients are $\widehat\Gamma^0_{00}=2\partial_\eta\Psi$, $\widehat\Gamma^0_{0i}=2\partial_i\Psi$ and $\widehat\Gamma^i_{00}=2\partial^i\Psi$. The affine parameter is that of the rescaled metric, not necessarily that of the original spacetime.

##### First-order photon trajectory in scalar perturbations

↑ **Parent:** [Conformal optical metric for scalar perturbations](#conformal-optical-metric-for-scalar-perturbations)

For reception at the origin with unit propagation direction $e$, the [null geodesic](special-relativity.md#null-geodesic) condition fixes $v(\eta_0)=(1+2\Psi_0)e$. The perturbative spatial acceleration is $x^{i\prime\prime}=2e^i d\Psi/d\eta-2(\delta^{ij}-e^ie^j)\partial_j\Psi$. Its integrated trajectory is $x^i=e^i(\eta-\eta_0)+2e^i\int_{\eta_0}^{\eta}\Psi\,d\eta^{\prime}-2\int_{\eta_0}^{\eta}(\eta-\eta^{\prime})(\delta^{ij}-e^ie^j)\partial_j\Psi\,d\eta^{\prime}$. Potentials in these already first-order integrals can be evaluated on the straight background ray.

#### Gravitational potential evolution of a barotropic fluid

↑ **Parent:** [Newtonian gauge](#newtonian-gauge)

For a flat background dominated by one constant-$w$ [barotropic equation of state](cosmology.md#barotropic-equation-of-state), assume $\delta P=w\delta\rho$ and no [scalar anisotropic stress](#scalar-anisotropic-stress). The [Einstein field equations](general-relativity.md#einstein-field-equations) then reduce the common Newtonian-gauge potential to the stated [Fourier transform](analysis.md#fourier-transform) equation, with $\mathcal H=2/[(1+3w)\tau]$. For radiation the regular solution is $3\Phi_0(\sin x-x\cos x)/x^3$, $x=k\tau/\sqrt3$, and oscillates with a decaying envelope after sound-horizon entry. For pressureless matter the two solutions are a constant and $\tau^{-5}$. A non-adiabatic pressure perturbation would supply an additional source, so constant background $w$ alone does not justify the homogeneous equation.

#### Cosmological Euler equation

↑ **Parent:** [Newtonian gauge](#newtonian-gauge)

For pressureless matter in conformal time and Newtonian gauge,

$$
\mathbf v'+\mathcal H\mathbf v+(\mathbf v\mathbin\cdot\nabla)\mathbf v
=-\nabla\phi.
$$

Its linear curl implies that vorticity decays as $a^{-1}$.

##### Linear matter density equation in Newtonian gauge

↑ **Parent:** [Cosmological Euler equation](#cosmological-euler-equation)

For [pressureless matter](cosmology.md#pressureless-matter) in [Newtonian gauge in cosmology](#newtonian-gauge) with a common metric potential $\Phi$, let $\theta=\nabla\cdot\mathbf v$. The linear equations $\delta_m'=-\theta+3\Phi'$ and $\theta'=-\mathcal H\theta-\nabla^2\Phi$, where primes denote [conformal time](cosmology.md#conformal-time), yield

$$
\delta_m''+\mathcal H\delta_m'=\nabla^2\Phi+3(\Phi''+\mathcal H\Phi').
$$

This follows by differentiating the first equation and eliminating $\theta$. On deeply subhorizon scales with a slowly varying matter potential, the metric time derivatives are small compared with its spatial [Laplacian](calculus.md#laplacian).

#### Cosmological Poisson equation

↑ **Parent:** [Newtonian gauge](#newtonian-gauge)

On subhorizon scales, the Newtonian potential sourced by the matter density contrast obeys

$$
\nabla^2\phi=\frac32\mathcal H^2\Omega_m\delta.
$$

### Scalar velocity potential

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)

The longitudinal velocity perturbation of a cosmological fluid can be represented by a scalar velocity potential through $\delta T^0{}_i=(\bar\rho+\bar P)\partial_i\delta u$.

### Scalar anisotropic stress

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)

Scalar anisotropic stress is the trace-free scalar part of the spatial stress perturbation. Under a common convention it enters as $\delta T^i{}_j=\delta P\,\delta^i_j+\partial^i\partial_j\pi^S$.

#### Scalar neutrino anisotropic stress

↑ **Parent:** [Scalar anisotropic stress](#scalar-anisotropic-stress)

Using the unweighted [neutrino Boltzmann hierarchy](linear-cosmological-density-perturbation.md#neutrino-boltzmann-hierarchy) convention and $\Pi_{ij}=-(4\bar\rho_\nu/3)\Pi_\nu(\hat k_i\hat k_j-\delta_{ij}/3)$, the scalar [scalar anisotropic stress](#scalar-anisotropic-stress) is $\Pi_\nu=-3\Theta_2/5$. Only the quadrupole contributes, since the trace-free tensor $e_ie_j-\delta_{ij}/3$ has angular degree two. Different stress and multipole sign conventions change this displayed coefficient.

##### Radiation-era adiabatic potentials with free-streaming neutrinos

↑ **Parent:** [Scalar neutrino anisotropic stress](#scalar-neutrino-anisotropic-stress)

For regular [adiabatic initial conditions](cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) on [superhorizon scales](cosmic-inflation.md#superhorizon-scale) during [radiation domination](linear-cosmological-density-perturbation.md#radiation-domination), the unweighted [neutrino Boltzmann hierarchy](linear-cosmological-density-perturbation.md#neutrino-boltzmann-hierarchy) gives $\Theta_1=\psi k\eta/2$ and $\Theta_2=\psi(k\eta)^2/6$. With $f_\nu=\bar\rho_\nu/(\bar\rho_\nu+\bar\rho_\gamma)$ and neutrinos the only source of [scalar anisotropic stress](#scalar-anisotropic-stress), the trace-free [Einstein field equations](general-relativity.md#einstein-field-equations) gives $\phi=(1+2f_\nu/5)\psi$. For the sign convention $\mathcal R=-\phi-\psi/2$,

$$
\psi=-\frac{10}{15+4f_\nu}\mathcal R,\qquad\phi=-\frac{10+4f_\nu}{15+4f_\nu}\mathcal R.
$$

### Flat gauge in cosmology

↑ **Parent:** [Scalar cosmological perturbation](#scalar-cosmological-perturbation)

Flat gauge sets the scalar perturbation of the spatial metric to zero. Scalar fluctuations then reside in the lapse, shift, and matter fields, making the field fluctuation directly visible while the lapse and shift remain constrained variables.

## Cosmological transfer function

↑ **Parent:** [Linear cosmological perturbation theory](linear-cosmological-perturbation-theory.md)

A cosmological transfer function relates a late perturbation to a specified primordial perturbation mode by mode. It records the scale-dependent evolution caused by horizon entry, pressure, free streaming, and changes in the dominant cosmic component.

### Radiation acoustic transfer function

↑ **Parent:** [Cosmological transfer function](#cosmological-transfer-function)

During matter domination with nearly constant gravitational potential, a radiation density perturbation obeys a forced acoustic equation. The observable [Sachs-Wolfe combination](cosmic-microwave-background-anisotropy.md#sachs-wolfe-combination) is the homogeneous oscillatory part.

#### Subhorizon radiation acoustic oscillations

↑ **Parent:** [Radiation acoustic transfer function](#radiation-acoustic-transfer-function)

Pressure-supported radiation perturbations well inside the horizon oscillate rather than exhibit secular gravitational growth. In the ideal relativistic fluid, $c_s^2=1/3$ and the leading conformal frequency is $k/\sqrt3$. Their rapidly changing source has a small late-time response in the slowly varying cold-matter density mode.

##### Matter-era forced radiation response

↑ **Parent:** [Subhorizon radiation acoustic oscillations](#subhorizon-radiation-acoustic-oscillations)

Let $\delta_c=C_g\tau^2+C_d\tau^{-3}$ be the [matter-era growing and decaying density modes](linear-cosmological-density-perturbation.md#matter-era-growing-and-decaying-density-modes), with radiation neglected in the background gravity. The radiation [density contrast](linear-cosmological-density-perturbation.md#density-contrast) is

$$
\delta_r=C_1\cos(\omega\tau)+C_2\sin(\omega\tau)+\frac{8C_g}{3\omega^2}
+\frac{16C_d}{\omega}\int_{\tau_*}^{\tau}s^{-5}\sin[\omega(\tau-s)]\,ds.
$$

The formula follows by the [Green's function](analysis.md#green-s-function) of the forced [harmonic oscillator](classical-mechanics.md#simple-harmonic-motion). For $k\tau\gg1$, the slowly varying particular response to the decaying mode begins at $16C_d\tau^{-5}/\omega^2$; lower-endpoint oscillations are absorbed into $C_1,C_2$. The growing mode drives a constant radiation offset, while [cold dark matter](cosmology.md#cold-dark-matter) continues growing as $\tau^2$.

##### Suppressed cold-matter forcing by rapid radiation oscillations

↑ **Parent:** [Subhorizon radiation acoustic oscillations](#subhorizon-radiation-acoustic-oscillations)

In deep [radiation domination](linear-cosmological-density-perturbation.md#radiation-domination), an oscillatory radiation density source in the matter equation has order $\Delta_r/\tau^2$ and frequency of order $k$. Its rapidly varying particular response is therefore of order $\Delta_r/(k\tau)^2$. For $k\tau\gg1$ it does not control the secular matter growth, though forcing near horizon entry sets the constant and logarithmic homogeneous amplitudes.

### Cold-dark-matter transfer function

↑ **Parent:** [Cosmological transfer function](#cosmological-transfer-function)

At fixed time after equality, the comoving cold-dark-matter density contrast per unit primordial curvature grows as $k^2$ for $k\ll k_{\rm eq}$ and only logarithmically for $k\gg k_{\rm eq}$. Small-scale modes entered during radiation domination and could grow only logarithmically until equality.

#### Frozen-radiation approximation to the matter transfer function

↑ **Parent:** [Cold-dark-matter transfer function](#cold-dark-matter-transfer-function)

Assume all relevant modes begin outside the horizon at common [conformal time](cosmology.md#conformal-time) $\tau_i$, grow as $\tau^2$ until radiation-era horizon entry, then freeze until [matter-radiation equality](cosmology.md#matter-radiation-equality), and again grow as $\tau^2$ in matter domination. With horizon entry $\tau_h=2\pi/k$, $k_{\rm eq}=2\pi/\tau_{\rm eq}$ and final time $\tau_0$, direct multiplication of the growth factors gives the displayed transfer with $G=(\tau_0/\tau_i)^2$. A primordial density [power spectrum](probability-and-statistics.md#power-spectrum) $P_i=Ak$ becomes $P_0=AG^2k$ below equality wavenumber and $AG^2k_{\rm eq}^4k^{-3}$ above it. This approximation neglects the true logarithmic radiation-era matter growth, baryonic acoustic structure and late acceleration; a conventionally normalized transfer divides out $G$.

#### Scale-independent matter suppression by a coasting fluid

↑ **Parent:** [Cold-dark-matter transfer function](#cold-dark-matter-transfer-function)

The matter equation in the barotropic matter-string model contains no wavenumber. Growing initial data therefore evolve as $\delta_c(k,\eta)=A_kD(\eta)$ with the same $D$ for every mode. For regular adiabatic modes initially outside the horizon during [matter domination](linear-cosmological-density-perturbation.md#matter-domination), $A_k$ is proportional to $k^2$ times the primordial curvature amplitude. The density-per-curvature transfer is consequently proportional to $k^2D(\eta)$ for modes entering after equality. Factoring out both $k^2$ and $D$ gives a constant shape transfer on those scales. Comparing with continued matter-era growth instead introduces the common suppression $D(\eta)/\eta$, not a new wavenumber dependence.

#### Sharp-equality cold-dark-matter transfer approximation

↑ **Parent:** [Cold-dark-matter transfer function](#cold-dark-matter-transfer-function)

In the idealization that subhorizon cold matter freezes during [radiation domination](linear-cosmological-density-perturbation.md#radiation-domination), early-entering modes have an entry density of order the primordial curvature, retain it until equality, and then share the same matter-era growth factor. Their density-per-curvature transfer becomes approximately independent of $k$. Matching this plateau to the matter-era $k^2$ transfer gives the displayed sharp-transition model, with its high-$k$ coefficient dependent on the matching convention. A scale-invariant curvature spectrum then gives density power proportional to $k$ below equality and $k^{-3}$ above it. Actual cold matter grows logarithmically in the radiation era, adding the familiar high-$k$ logarithms of the [Mészáros effect](linear-cosmological-density-perturbation.md#meszaros-effect).

#### Matter-era density transfer from primordial curvature

↑ **Parent:** [Cold-dark-matter transfer function](#cold-dark-matter-transfer-function)

For the regular growing mode in a purely matter-dominated flat background, $h=-2\delta_c$ and $\delta_c=C\tau^2$. The synchronous Einstein constraint $\mathcal Hh'+k^2h^-/3=3\mathcal H^2\delta_c$ with $\mathcal H=2/\tau$ gives $h^-=60C/k^2$. Hence $\zeta=h^-/6+\delta_c/3=10C/k^2+C\tau^2/3$, conserved to leading order on [superhorizon scales](cosmic-inflation.md#superhorizon-scale). Identifying its early constant value gives the displayed density transfer; it includes a $k^2$ factor that is factored out of the conventionally normalized matter transfer function.

#### Asymptotic cold-dark-matter power spectrum

↑ **Parent:** [Cold-dark-matter transfer function](#cold-dark-matter-transfer-function)

The dimensional [matter power spectrum](linear-cosmological-density-perturbation.md#matter-power-spectrum) contains a factor $k^{n_s}$, rather than $k^{n_s+3}$. The [cosmological transfer function](#cosmological-transfer-function) tends to one below the [matter-radiation equality scale](cosmology.md#matter-radiation-equality-scale) and to $\ln(k/k_{\rm eq})/(k/k_{\rm eq})^2$ above it. The smooth spectrum therefore scales as $k^{n_s}$ at small wavenumber and $k^{n_s-4}\ln^2(k/k_{\rm eq})$ at large wavenumber. The logarithmic factor records slow cold-matter growth during [radiation domination](linear-cosmological-density-perturbation.md#radiation-domination). Multiplying by $k^3$ instead produces dimensionless matter power.

#### Logarithmic small-scale matter transfer

↑ **Parent:** [Cold-dark-matter transfer function](#cold-dark-matter-transfer-function)

Modes with $k\gg k_{\rm eq}$ enter the horizon during [radiation domination](linear-cosmological-density-perturbation.md#radiation-domination). Their matter perturbations grow only logarithmically until [matter-radiation equality](cosmology.md#matter-radiation-equality), rather than as $a$. Matching the radiation-era logarithmic growth onto the matter-era growing mode gives the large-$k$ [cosmological transfer function](#cosmological-transfer-function) scaling shown, up to constants and the matching scale inside the logarithm. For a primordial [scalar spectral index](cosmic-inflation.md#scalar-spectral-index) $n_s$, the late-time linear [cosmological density power spectrum](linear-cosmological-density-perturbation.md#matter-power-spectrum) consequently changes from $P(k)\propto k^{n_s}$ at small $k$ to $P(k)\propto k^{n_s-4}\log^2(k/k_{\rm eq})$ at large $k$. These scalings omit baryonic acoustic structure and nonlinear evolution.

Here the [cold-dark-matter transfer function](#cold-dark-matter-transfer-function) is normalized so that $\delta_m(k,a)=A(a)k^2T(k)\mathcal R(k)$, where $\mathcal R$ is the primordial [comoving curvature perturbation](cosmic-inflation.md#comoving-curvature-perturbation) and $A(a)$ is independent of $k$. During [radiation domination](linear-cosmological-density-perturbation.md#radiation-domination), horizon entry occurs at $a_{\rm ent}\propto k^{-1}$. An adiabatic entry amplitude of order $\mathcal R$ then acquires a factor $\log(a_{\rm eq}/a_{\rm ent})\sim\log(k/k_{\rm eq})$ by [matter-radiation equality](cosmology.md#matter-radiation-equality). Subsequent [matter domination](linear-cosmological-density-perturbation.md#matter-domination) supplies a common growth factor; division by the conventional $k^2$ prefactor therefore gives $T(k)\propto k^{-2}\log(k/k_{\rm eq})$.

##### Logarithmic high-wavenumber density-spectrum transfer

↑ **Parent:** [Logarithmic small-scale matter transfer](#logarithmic-small-scale-matter-transfer)

A scale-invariant curvature seed gives wavenumber-independent dimensionless matter power at radiation-era horizon entry. Horizon entry at $\tau_h\sim1/k$, followed by logarithmic growth to equality, gives a density transfer proportional to $\ln(k\tau_{\rm eq})$. Subsequent matter-era growth is proportional to $\tau^2$, so the dimensionless density power is proportional to $(\tau/\tau_{\rm eq})^4\ln^2(k\tau_{\rm eq})$. This is a high-wavenumber asymptote, not an expression at the transition point.

### Baryon transfer function

↑ **Parent:** [Cosmological transfer function](#cosmological-transfer-function)

The baryon transfer function retains acoustic oscillations generated while baryons belonged to the [photon-baryon fluid](cosmic-microwave-background-anisotropy.md#photon-baryon-fluid). After recombination, baryons fall into cold-dark-matter potential wells, reducing the relative perturbation while leaving a small oscillatory imprint.

<h4 id="baryon-cold-dark-matter-relative-density-mode">Baryon--cold-dark-matter relative density mode</h4>

↑ **Parent:** [Baryon transfer function](#baryon-transfer-function)

After recombination and when pressure is negligible, cold dark matter and baryons feel the same gravitational acceleration. Their density-contrast difference therefore obeys

$$
\ddot D+2H\dot D=0.
$$

During matter domination $D=D_0+D_1a^{-1/2}$, whereas the growing total-matter mode is proportional to $a$, so $\delta_c/\delta_b\to1$.

## ↑ Ancestors (4)

1. [Cosmology](cosmology.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Anisotropic stress](general-relativity.md#anisotropic-stress)
- [Cosmological perturbation theory](cosmology.md#cosmological-perturbation-theory)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-62.md#4/a/solution)
