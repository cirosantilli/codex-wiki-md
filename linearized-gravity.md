# Linearized gravity

↑ **Parent:** [General relativity](general-relativity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linearized_gravity)

Linearized gravity writes $g_{\mu\nu}=\eta_{\mu\nu}+h_{\mu\nu}$ with $|h_{\mu\nu}|\ll1$ and discards terms quadratic in $h$ and its derivatives.

**Table of contents**

- [Gauge-invariant scalar-vector-tensor perturbations of Minkowski spacetime](#gauge-invariant-scalar-vector-tensor-perturbations-of-minkowski-spacetime)
  - [Vacuum constraints for gauge-invariant Minkowski perturbations](#vacuum-constraints-for-gauge-invariant-minkowski-perturbations)
- [Static scalar perturbation of Minkowski spacetime](#static-scalar-perturbation-of-minkowski-spacetime)
- [Linearized Schwarzschild metric](#linearized-schwarzschild-metric)
  - [Weak-field photon-orbit validity](#weak-field-photon-orbit-validity)
  - [Isotropic-to-areal weak-field radius change](#isotropic-to-areal-weak-field-radius-change)
- [Quadratic gravitational effective stress-energy tensor](#quadratic-gravitational-effective-stress-energy-tensor)
- [Massless Fierz-Pauli action](#massless-fierz-pauli-action)
- [Linearized coordinate gauge transformation](#linearized-coordinate-gauge-transformation)
  - [Affine transverse trace in a diagonal linearized plane wave is pure gauge](#affine-transverse-trace-in-a-diagonal-linearized-plane-wave-is-pure-gauge)
- [Weak-field approximation](#weak-field-approximation)
- [Linearized Einstein equations](#linearized-einstein-equations)
  - [Parallel photon beams in linearized gravity](#parallel-photon-beams-in-linearized-gravity)
  - [Radiation boundary condition for linearized gravity](#radiation-boundary-condition-for-linearized-gravity)
  - [Retarded quadrupole field](#retarded-quadrupole-field)
    - [Long-wavelength source approximation](#long-wavelength-source-approximation)
- [Linearized inverse metric](#linearized-inverse-metric)
- [Linearized Levi-Civita connection](#linearized-levi-civita-connection)
- [Linearized Riemann curvature operator](#linearized-riemann-curvature-operator)
  - [Gauge invariance of the linearized Riemann tensor](#gauge-invariance-of-the-linearized-riemann-tensor)
    - [Flat linearized metric perturbations are locally pure gauge](#flat-linearized-metric-perturbations-are-locally-pure-gauge)
- [Trace-reversed metric perturbation](#trace-reversed-metric-perturbation)
  - [Lorenz gauge in linearized gravity](#lorenz-gauge-in-linearized-gravity)
    - [Residual gauge symmetry of linearized gravity](#residual-gauge-symmetry-of-linearized-gravity)
      - [Pure-gauge plane wave in linearized gravity](#pure-gauge-plane-wave-in-linearized-gravity)
    - [Plane gravitational wave in linearized gravity](#plane-gravitational-wave-in-linearized-gravity)
      - [Transverse-traceless gauge](#transverse-traceless-gauge)
        - [Explicit plane-wave reduction to transverse-traceless gauge](#explicit-plane-wave-reduction-to-transverse-traceless-gauge)
        - [TT coordinate separation and measured separation](#tt-coordinate-separation-and-measured-separation)
          - [Angular response of a gravitational-wave separation](#angular-response-of-a-gravitational-wave-separation)
          - [Sliding-bead gravitational wave detector](#sliding-bead-gravitational-wave-detector)
        - [Gravitational wave polarization](#gravitational-wave-polarization)
          - [Plus-polarized gravitational wave](#plus-polarized-gravitational-wave)
          - [Transverse-traceless tensor](#transverse-traceless-tensor)
          - [Plus polarization](#plus-polarization)
          - [Cross polarization](#cross-polarization)
          - [Transverse-traceless projector](#transverse-traceless-projector)
            - [Polarization completeness relation](#polarization-completeness-relation)
- [Linearized Ricci tensor and scalar](#linearized-ricci-tensor-and-scalar)
- [Newtonian limit](#newtonian-limit)
  - [Newtonian connection from an exponential lapse](#newtonian-connection-from-an-exponential-lapse)
  - [Static radius](#static-radius)
  - [Linearized point-mass metric in radial Cartesian form](#linearized-point-mass-metric-in-radial-cartesian-form)
- [Slowly rotating weak-field metric](#slowly-rotating-weak-field-metric)

## Gauge-invariant scalar-vector-tensor perturbations of Minkowski spacetime

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

For signature $(+---)$, decompose a [metric perturbation](linearized-gravity.md) into $h_{00}=2A$, $h_{0i}=\partial_iB+B_i$ and $h_{ij}=2C\delta_{ij}+2(\partial_i\partial_j-\delta_{ij}\Delta/3)E+\partial_iE_j+\partial_jE_i+h_{ij}^{\rm TT}$, where the spatial vectors are divergence-free and $h^{\rm TT}$ is a [transverse-traceless tensor](#transverse-traceless-tensor). Under a passive coordinate shift $\xi^0=\tau$, $\xi^i=\partial_iL+L_i$, with $\partial_iL_i=0$, the changes are $\delta A=-\dot\tau$, $\delta B=\dot L-\tau$, $\delta C=\Delta L/3$, $\delta E=L$, $\delta B_i=\dot L_i$, and $\delta E_i=L_i$. The displayed combinations and $h^{\rm TT}$ are therefore gauge invariant. The decomposition is unique after appropriate spatial decay or mode restrictions; homogeneous and boundary modes require separate conventions.

### Vacuum constraints for gauge-invariant Minkowski perturbations

↑ **Parent:** [Gauge-invariant scalar-vector-tensor perturbations of Minkowski spacetime](#gauge-invariant-scalar-vector-tensor-perturbations-of-minkowski-spacetime)

With the reversed convention in [curvature-sign convention in Killing derivative identities](killing-vector-field.md#curvature-sign-convention-in-killing-derivative-identities), choose the representative $h_{00}=2\Phi$, $h_{0i}=V_i$, $h_{ij}=2\Psi\delta_{ij}+h_{ij}^{\rm TT}$. The linearized Einstein components are $G_{00}^{(1)}=-2\Delta\Psi$, $G_{0i}^{(1)}=-2\partial_i\dot\Psi-\Delta V_i/2$ and $G_{ij}^{(1)}=(\partial_i\partial_j-\delta_{ij}\Delta)(\Phi-\Psi)-2\delta_{ij}\ddot\Psi-(\partial_i\dot V_j+\partial_j\dot V_i)/2+\Box h_{ij}^{\rm TT}/2$. On all space with regular decaying fields, or for nonzero spatial Fourier modes, the vacuum constraints remove the scalar and vector parts, leaving two radiative [gravitational wave polarizations](#gravitational-wave-polarization). Singular Coulomb fields, spatial boundaries and homogeneous modes are not covered by that removal argument.

## Static scalar perturbation of Minkowski spacetime

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

For static scalar perturbations with no mixed time-space or spatial shear terms, the displayed [metric tensor](general-relativity.md#metric-tensor) uses signature $(+---)$. With the reversed convention in [curvature-sign convention in Killing derivative identities](killing-vector-field.md#curvature-sign-convention-in-killing-derivative-identities), its first-order [Einstein tensor](riemann-curvature-tensor.md#einstein-tensor) is $\delta G_{00}=2\Delta C$, $\delta G_{0i}=0$, and $\delta G_{ij}=\partial_i\partial_j(A+C)-\delta_{ij}\Delta(A+C)$. These follow by substituting the metric into the first-order [Christoffel symbols](riemannian-geometry.md#christoffel-symbol) and [Ricci tensor](riemann-curvature-tensor.md#ricci-tensor), discarding products of perturbations. A static source with the [dust stress-energy tensor](stress-energy-tensor.md#dust-stress-energy-tensor) obeys $\Delta C=-4\pi G\rho$ and the decaying spatial equation makes $A=-C$. For a point mass the [Newtonian potential of a point mass](newton-s-law-of-universal-gravitation.md#newtonian-potential-of-a-point-mass) gives $A=-GM/r$, $C=GM/r$. The spatial potential is necessary to determine light propagation; a time potential alone is insufficient.

## Linearized Schwarzschild metric

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

For a static spherical point source, the weak-field solution in isotropic radius $\rho$ has $g_{tt}=1-2GM/\rho$ and spatial metric $-(1+2GM/\rho)(d\rho^2+\rho^2d\Omega^2)$. The [isotropic-to-areal weak-field radius change](#isotropic-to-areal-weak-field-radius-change) gives the displayed metric with $r_S=2GM$. Its validity requires $r_S/r\ll1$. Treating it as an exact metric near $r\sim r_S$ can turn omitted terms into large corrections; it does not establish horizons or strong-field photon dynamics.

### Weak-field photon-orbit validity

↑ **Parent:** [Linearized Schwarzschild metric](#linearized-schwarzschild-metric)

The first-order null-orbit equation $(u')^2=r_S^2E^2/h^2-u^2(1-u)$ formally has a circular solution at $u=2/3$, with $|h/E|=3\sqrt3r_S/2$. Its second-order equation gives a perturbation $\delta u''=\delta u$, hence instability. However, $u=2/3$ is outside the weak-field expansion. The exact [Schwarzschild spacetime](schwarzschild-spacetime.md) has a corresponding unstable [photon sphere](schwarzschild-spacetime.md#photon-sphere), but that physical result needs the exact geometry; extrapolating the linearized metric is not a controlled proof.

### Isotropic-to-areal weak-field radius change

↑ **Parent:** [Linearized Schwarzschild metric](#linearized-schwarzschild-metric)

The area of a symmetry sphere in the weak-field isotropic metric is $4\pi\rho^2(1+2GM/\rho)$. Equating it to $4\pi r^2$ defines the [areal radius](general-relativity.md#areal-radius) and gives the displayed change. To first order $dr=d\rho$, and replacing $1/\rho$ by $1/r$ changes the perturbation only at second order. This explains why the isotropic angular correction disappears in the [linearized Schwarzschild metric](#linearized-schwarzschild-metric) without discarding spatial curvature.

## Quadratic gravitational effective stress-energy tensor

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

Expand the [Einstein tensor](riemann-curvature-tensor.md#einstein-tensor) about the [Minkowski metric](special-relativity.md#minkowski-metric). The quadratic term in the [metric perturbation](linearized-gravity.md) defines $t_{\mu\nu}=-G^{(2)}_{\mu\nu}[h,h]/(8\pi)$, a symmetric tensor relative to the background. For a first-order vacuum solution, the expanded [contracted Bianchi identity](riemann-curvature-tensor.md#contracted-bianchi-identity) gives $\partial^\mu t_{\mu\nu}=0$. Equivalently, a second-order correction $j$ obeys $G^{(1)}[j]=8\pi t$, whose flat divergence vanishes identically. This conservation is an on-shell statement. The local $t$ depends on perturbative gauge and the background split; conservation alone does not make it a gauge-independent local gravitational [stress-energy tensor](stress-energy-tensor.md).

## Massless Fierz-Pauli action

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

A [massless Fierz-Pauli action](#massless-fierz-pauli-action) is the quadratic flat-background action for a symmetric metric perturbation that yields the vacuum [Linearized Einstein equations](#linearized-einstein-equations). One normalization, up to a total derivative, is

$$
\mathcal L=-\frac14\partial_\mu h^{\rho\sigma}\partial^\mu h_{\rho\sigma}
+\frac12A_\mu A^\mu-\frac12A^\mu\partial_\mu h
+\frac14\partial_\mu h\partial^\mu h,\qquad A_\mu=\partial_\nu h^\nu{}_\mu.
$$

Varying the symmetric field with compact support gives the displayed linearized [Einstein tensor](riemann-curvature-tensor.md#einstein-tensor) coefficient. Its linearized coordinate-gauge symmetry is consistent with the contracted [Bianchi identity](fiber-bundle.md#bianchi-identity). It is the massless gravitational action, distinct from imposing the massive [Fierz-Pauli equations](relativistic-quantum-field.md#fierz-pauli-equations) with five polarizations.

## Linearized coordinate gauge transformation

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

An infinitesimal coordinate change generated by $\xi$ changes a metric perturbation about [Minkowski spacetime](special-relativity.md#minkowski-spacetime) by $h_{\mu\nu}\mapsto h_{\mu\nu}-\partial_\mu\xi_\nu-\partial_\nu\xi_\mu$, in the passive sign convention. For a passive coordinate change $x^\mu\mapsto x^\mu+\xi^\mu$, the first-order change is minus the [Lie derivative of a tensor field](vector-bundle.md#lie-derivative-of-a-tensor-field) of the background metric, equivalently the pullback by the inverse flow. The [gauge invariance of the linearized Riemann tensor](#gauge-invariance-of-the-linearized-riemann-tensor) follows because the added terms have commuting third derivatives, which cancel in the curvature antisymmetrizations. Gauge choices alter the metric components while preserving linearized tidal effects.

### Affine transverse trace in a diagonal linearized plane wave is pure gauge

↑ **Parent:** [Linearized coordinate gauge transformation](#linearized-coordinate-gauge-transformation)

For a perturbation $h_{xx}=2a(t-z)$, $h_{yy}=2b(t-z)$ with all other components zero, the linearized [Vacuum Einstein equations](einstein-field-equations.md#vacuum-einstein-equations) give $(a+b)''=0$. Put $s=a+b$ and choose $\xi_x=sx/2$, $\xi_y=sy/2$, $\xi_t=-s'(x^2+y^2)/4$, $\xi_z=s'(x^2+y^2)/4$. Under the [linearized coordinate gauge transformation](#linearized-coordinate-gauge-transformation), the mixed time/transverse and longitudinal/transverse components cancel, while the other time/longitudinal changes are proportional to $s''=0$. The remaining components are $h_{xx}=a-b$, $h_{yy}=-(a-b)$, $h_{xy}=0$, a [transverse-traceless gauge](#transverse-traceless-gauge) perturbation of [plus polarization](#plus-polarization). This explicitly removes a nonzero affine trace without assuming it vanishes by boundary conditions. If $(a-b)''=0$ too, all linearized curvature vanishes.

## Weak-field approximation

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

The weak-field approximation requires every dimensionless component of the [metric perturbation](linearized-gravity.md) to have magnitude much smaller than one, so terms quadratic in the perturbation may be neglected.

## Linearized Einstein equations

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

In terms of the [trace-reversed metric perturbation](#trace-reversed-metric-perturbation) and in the [Lorenz gauge in linearized gravity](#lorenz-gauge-in-linearized-gravity), the linearized Einstein equations on Minkowski spacetime are

$$
\Box\bar h_{\mu\nu}=-16\pi T_{\mu\nu}.
$$

### Parallel photon beams in linearized gravity

↑ **Parent:** [Linearized Einstein equations](#linearized-einstein-equations)

For signature $(+---)$ and the curvature convention giving $\Box\bar h_{ik}=-16\pi G\epsilon^{-1}T_{ik}$, take $u=t-x$, $\ell_i=(1,-1,0,0)$ and $T_{ik}=\epsilon\rho(u)\ell_i\ell_k$. A trace-free Lorenz-gauge particular solution has the displayed form. The vector $\ell^i=(1,1,0,0)$ is null, and $\Gamma^i{}_{jk}\ell^j\ell^k=0$, so co-propagating test photons are undeflected by this beam field. For a transversely uniform source, $H=4\pi G\rho(u)(y^2+z^2)$ is one particular solution. A function of $u$ alone has vanishing wave operator and cannot source nonzero $\rho$; homogeneous gravitational perturbations and boundary conditions remain separate data.

### Radiation boundary condition for linearized gravity

↑ **Parent:** [Linearized Einstein equations](#linearized-einstein-equations)

The retarded source solution of the [Linearized Einstein equations](#linearized-einstein-equations) is selected by excluding added incoming or freely specified homogeneous [gravitational waves](gravitational-wave.md). A homogeneous wave can satisfy [Lorenz gauge in linearized gravity](#lorenz-gauge-in-linearized-gravity) while having no source [mass quadrupole moment](gravitational-wave.md#mass-quadrupole-moment). Thus a formula for the retarded source field is not an identity for every solution of the sourced wave equation.

### Retarded quadrupole field

↑ **Parent:** [Linearized Einstein equations](#linearized-einstein-equations)

For a compact slowly moving source in the [weak-field approximation](#weak-field-approximation), with no incoming homogeneous wave and $G=c=1$, the retarded [Linearized Einstein equations](#linearized-einstein-equations) give this leading far-zone [trace-reversed metric perturbation](#trace-reversed-metric-perturbation). The key consequence of [stress-energy conservation](stress-energy-tensor.md#stress-energy-conservation) is $\ddot I_{ij}=2\int T_{ij}\,d^3x$. The physical [gravitational wave](gravitational-wave.md) is obtained by the [transverse-traceless projector](#transverse-traceless-projector).

#### Long-wavelength source approximation

↑ **Parent:** [Retarded quadrupole field](#retarded-quadrupole-field)

Dropping the position-dependent source delay in the leading far-zone retarded field requires source size $d$ to be small compared with its variation time $\tau$, in units $c=1$. The [retarded quadrupole field](#retarded-quadrupole-field) also requires $d/r\ll1$. For a typical nonrelativistic bound source, $\tau\sim d/v$ implies this long-wavelength condition; an arbitrarily rapidly oscillating small displacement is not controlled merely by its instantaneous speed.

## Linearized inverse metric

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

If $g_{\mu\nu}=\eta_{\mu\nu}+h_{\mu\nu}$, then $g^{\mu\nu}=\eta^{\mu\nu}-h^{\mu\nu}+O(h^2)$, with indices on $h$ raised using the background metric.

## Linearized Levi-Civita connection

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

About a Cartesian flat background,

$$
\Gamma^\alpha_{\beta\gamma}
=\frac12\eta^{\alpha\rho}
(\partial_\beta h_{\gamma\rho}+\partial_\gamma h_{\beta\rho}-\partial_\rho h_{\beta\gamma})+O(h^2).
$$

## Linearized Riemann curvature operator

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

The linearized Riemann tensor defines an operator on two-forms by

$$
(\mathcal R\omega)_{ab}=\frac12R^{(1)}_{ab}{}^{cd}\omega_{cd}.
$$

Unlike the metric perturbation itself, this operator is invariant under linearized gauge transformations.

### Gauge invariance of the linearized Riemann tensor

↑ **Parent:** [Linearized Riemann curvature operator](#linearized-riemann-curvature-operator)

Under $h_{\mu\nu}\mapsto h_{\mu\nu}+\partial_\mu\xi_\nu+\partial_\nu\xi_\mu$, every contribution to the linearized Riemann tensor contains three commuting derivatives of $\xi$ and cancels pairwise. Linearized curvature is therefore gauge invariant about flat spacetime.

#### Flat linearized metric perturbations are locally pure gauge

↑ **Parent:** [Gauge invariance of the linearized Riemann tensor](#gauge-invariance-of-the-linearized-riemann-tensor)

On a [contractible](homotopy.md#contractible-space) Cartesian patch of a flat background, zero [linearized Riemann curvature operator](#linearized-riemann-curvature-operator) says that the [connection 1-forms](connection-1-form.md) $\Gamma^{(1)a}{}_{bc}\,dx^c$ are closed. The [Poincaré lemma](differential-form.md#poincare-lemma) writes them as [derivatives](calculus.md#derivative) of a matrix-valued potential. Symmetry of the two lower [affine connection](vector-bundle.md#affine-connection) indices then supplies a second potential, giving $\Gamma^{(1)a}{}_{bc}=\partial_b\partial_c\xi^a$. Linearized [metric compatibility](vector-bundle.md#metric-compatibility) implies that $h_{ab}-2\partial_{(a}\xi_{b)}$ is constant. Its symmetric constant part is absorbed by an affine [vector field](multivariable-calculus.md#vector-field). Thus the [metric perturbation](linearized-gravity.md) is locally a coordinate change. Global [topology](topology.md) and imposed [boundary conditions](differential-equation.md#boundary-condition) can obstruct the corresponding global gauge choice.

## Trace-reversed metric perturbation

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

In four dimensions, the trace-reversed perturbation is

$$
\bar h_{\mu\nu}=h_{\mu\nu}-\frac12\eta_{\mu\nu}h,
\qquad h=\eta^{\rho\sigma}h_{\rho\sigma}.
$$

Trace reversal simplifies the linearized Einstein equations.

### Lorenz gauge in linearized gravity

↑ **Parent:** [Trace-reversed metric perturbation](#trace-reversed-metric-perturbation)

The Lorenz condition $\partial^\mu\bar h_{\mu\nu}=0$ reduces the vacuum field equation to $\Box\bar h_{\mu\nu}=0$. A plane-wave amplitude therefore satisfies $k^\mu H_{\mu\nu}=0$ and $k^\mu k_\mu=0$.

#### Residual gauge symmetry of linearized gravity

↑ **Parent:** [Lorenz gauge in linearized gravity](#lorenz-gauge-in-linearized-gravity)

An infinitesimal coordinate change generated by $\xi_\mu$ changes

$$
\bar h_{\mu\nu}\mapsto
\bar h_{\mu\nu}-\partial_\mu\xi_\nu-\partial_\nu\xi_\mu
+\eta_{\mu\nu}\partial_\rho\xi^\rho.
$$

It preserves Lorenz gauge exactly when $\Box\xi_\mu=0$.

##### Pure-gauge plane wave in linearized gravity

↑ **Parent:** [Residual gauge symmetry of linearized gravity](#residual-gauge-symmetry-of-linearized-gravity)

Under the convention $\delta h_{\mu\nu}=\partial_\mu\xi_\nu+\partial_\nu\xi_\mu$, choose $\xi^\mu=b^\mu\sin(k\cdot x)$ with constant $b^\mu$ and null $k^\mu$. The [trace-reversed metric perturbation](#trace-reversed-metric-perturbation) has amplitude

$$
\epsilon_{\rm gauge}^{\mu\nu}=k^\mu b^\nu+k^\nu b^\mu-\eta^{\mu\nu}(k\cdot b).
$$

It satisfies $k_\mu\epsilon_{\rm gauge}^{\mu\nu}=0$ and $\Box\xi^\mu=0$, so it is an allowed [residual gauge symmetry of linearized gravity](#residual-gauge-symmetry-of-linearized-gravity). Its [linearized Riemann curvature operator](#linearized-riemann-curvature-operator) is zero: the four wavevector factors in each second-derivative term cancel in the antisymmetric curvature combinations. Nonzero transverse-traceless curvature distinguishes the two physical [gravitational wave polarizations](#gravitational-wave-polarization) from these coordinate modes.[Section 5.3.1, equations 5.232–5.234: residual plane-wave gauge transformation and transverse-traceless reduction](https://www.damtp.cam.ac.uk/user/tong/gr/grhtml/S5.html)

#### Plane gravitational wave in linearized gravity

↑ **Parent:** [Lorenz gauge in linearized gravity](#lorenz-gauge-in-linearized-gravity)

A vacuum mode $\bar h_{\mu\nu}=H_{\mu\nu}e^{ik\cdot x}$ has a null wavevector and a transverse symmetric amplitude. Residual gauge freedom can further reduce it to two physical transverse-traceless polarizations.

##### Transverse-traceless gauge

↑ **Parent:** [Plane gravitational wave in linearized gravity](#plane-gravitational-wave-in-linearized-gravity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transverse-traceless_gauge)

Transverse-traceless gauge sets the time and longitudinal components and the spatial trace of a vacuum gravitational-wave perturbation to zero.

###### Explicit plane-wave reduction to transverse-traceless gauge

↑ **Parent:** [Transverse-traceless gauge](#transverse-traceless-gauge)

For a [plane gravitational wave in linearized gravity](#plane-gravitational-wave-in-linearized-gravity) with $k_\mu=(-\omega,0,0,\omega)$, [Lorenz gauge in linearized gravity](#lorenz-gauge-in-linearized-gravity) gives $H_{3\nu}=-H_{0\nu}$. Under $\delta H_{\mu\nu}=i(k_\mu X_\nu+k_\nu X_\mu-\eta_{\mu\nu}k^\rho X_\rho)$, choose $X_i=H_{0i}/(i\omega)$ for $i=1,2$, $X_3-X_0=iH_{00}/\omega$, and $X_0+X_3=(H_{11}+H_{22})/(2i\omega)$. This [residual gauge symmetry of linearized gravity](#residual-gauge-symmetry-of-linearized-gravity) removes all time and longitudinal entries and the transverse trace. The remaining amplitudes $H_+,H_\times$ are the two [gravitational wave polarizations](#gravitational-wave-polarization). The formula uses the plus-sign convention for $\delta h=2\partial_{(\mu}\xi_{\nu)}$; reversing the definition of $\xi$ reverses the gauge change.

###### TT coordinate separation and measured separation

↑ **Parent:** [Transverse-traceless gauge](#transverse-traceless-gauge)

In [transverse-traceless gauge](#transverse-traceless-gauge), particles initially at rest have fixed spatial coordinates because $\Gamma^\mu{}_{00}=0$. Their separation measured in a [parallel-propagated orthonormal frame](general-relativity.md#parallel-propagated-orthonormal-frame) changes: to first order $S^{\hat A}=S^A+h_{AB}S^B/2$. Hence the physical [geodesic deviation](riemann-curvature-tensor.md#geodesic-deviation) is $\ddot\xi^{\hat A}=\ddot h_{AB}L^B/2$, whereas the coordinate displacement obeys $\ddot\xi^A_{\rm coord}=0$. The extra $\partial_0\Gamma^A{}_{0B}L^B$ term in the coordinate expansion of the second [covariant derivative](general-relativity.md#covariant-derivative) reconciles the two results. This applies to infinitesimal separations and linear [metric perturbations](linearized-gravity.md).

###### Angular response of a gravitational-wave separation

↑ **Parent:** [TT coordinate separation and measured separation](#tt-coordinate-separation-and-measured-separation)

For a short pair of stationary test particles in [transverse-traceless gauge](#transverse-traceless-gauge), spatial coordinates stay fixed while the measured [proper length](special-relativity.md#proper-length) changes. In background signature $+---$, let $h_{xx}=-h_{yy}=H_+$ and $h_{xy}=H_\times$. A coordinate separation of length $\Delta$ at angle $\theta$ has

$$
\ell^2=\Delta^2[1-H_+\cos(2\theta)-H_\times\sin(2\theta)],\qquad
\frac{\delta\ell}{\Delta}=-\frac12[H_+\cos(2\theta)+H_\times\sin(2\theta)]+O(H^2).
$$

The [plus polarization](#plus-polarization) and [cross polarization](#cross-polarization) differ by a $45$-degree rotation of their principal axes. With background signature $-+++$ and the same numerical spatial perturbation, the sign reverses because the positive spatial metric is then $\delta_{ij}+h_{ij}$ rather than $\delta_{ij}-h_{ij}$. Consistently redefining the signed strain leaves the physical effect unchanged.

###### Sliding-bead gravitational wave detector

↑ **Parent:** [TT coordinate separation and measured separation](#tt-coordinate-separation-and-measured-separation)

A short rigid nonrotating guide constrains two freely sliding beads to one axis $n$. In its [parallel-propagated orthonormal frame](general-relativity.md#parallel-propagated-orthonormal-frame), the axial [geodesic deviation](riemann-curvature-tensor.md#geodesic-deviation) is $\ddot L=-R_{n0n0}L$. For a transverse [gravitational wave](gravitational-wave.md), $R_{n0n0}=-\epsilon\ddot h_{nn}/2$, so a wave incident after the beads are at rest changes the measured separation by $\epsilon h_{nn}L_0/2$ to first order. Transverse reaction forces do not supply an axial restoring force. Alignment with the propagation direction gives no first-order length change.

###### Gravitational wave polarization

↑ **Parent:** [Transverse-traceless gauge](#transverse-traceless-gauge)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gravitational_wave_polarization)

A gravitational wave in four-dimensional general relativity has two independent linear polarizations, conventionally called plus and cross. A rotation by angle $\vartheta$ in the transverse plane rotates their pair by $2\vartheta$.

###### Plus-polarized gravitational wave

↑ **Parent:** [Gravitational wave polarization](#gravitational-wave-polarization)

A [gravitational wave](gravitational-wave.md) carrying the plus component relative to a chosen pair of transverse axes.

###### Transverse-traceless tensor

↑ **Parent:** [Gravitational wave polarization](#gravitational-wave-polarization)

A transverse-traceless spatial tensor is orthogonal to its [Fourier mode](fourier-analysis.md#fourier-mode) wavevector in each index and has zero trace. The [transverse-traceless projector](#transverse-traceless-projector) extracts this part. Trace terms and symmetrized coordinate-displacement gradients have no such part, explaining the linear gauge invariance of [tensor cosmological perturbations](linear-cosmological-perturbation-theory.md#tensor-cosmological-perturbation).

###### Plus polarization

↑ **Parent:** [Gravitational wave polarization](#gravitational-wave-polarization)

A [gravitational wave](gravitational-wave.md) of plus polarization has opposite transverse strain or [geodesic deviation](riemann-curvature-tensor.md#geodesic-deviation) [eigenvalues](linear-operator-theory.md#eigenvalue) along two fixed perpendicular axes. For a sinusoidal [periodic function](function.md#periodic-function) profile, the stretching and compressing roles alternate every half-period.

###### Cross polarization

↑ **Parent:** [Gravitational wave polarization](#gravitational-wave-polarization)

The cross polarization is the plus pattern rotated through $45$ degrees in the transverse plane.

###### Transverse-traceless projector

↑ **Parent:** [Gravitational wave polarization](#gravitational-wave-polarization)

The transverse-traceless projector maps a symmetric tensor to the part orthogonal to a chosen wavevector and with zero trace. It is the identity on physical gravitational-wave polarizations.

###### Polarization completeness relation

↑ **Parent:** [Transverse-traceless projector](#transverse-traceless-projector)

A polarization completeness relation expresses a projector as a sum of outer products of an orthonormal polarization basis. For transverse-traceless tensors, $\sum_s\epsilon_{ij}^s\epsilon_{mn}^{s*}$ is the transverse-traceless projector up to the chosen normalization.

## Linearized Ricci tensor and scalar

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

To first order around flat spacetime,

$$
R_{\mu\nu}
=\frac12\left(
\partial_\rho\partial_\mu h^\rho{}_{\nu}
+\partial_\rho\partial_\nu h^\rho{}_{\mu}
-\mathop{\Box}h_{\mu\nu}
-\partial_\mu\partial_\nu h
\right),
$$

and

$$
R=\partial_\mu\partial_\nu h^{\mu\nu}-\mathop{\Box}h,
\qquad h=\eta^{\mu\nu}h_{\mu\nu}.
$$

## Newtonian limit

↑ **Parent:** [Linearized gravity](linearized-gravity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Newtonian_limit)

For a weak, static field produced by nonrelativistic matter, $T_{00}=\rho$ is the dominant stress-energy component. The field equations and the slow-particle [geodesic equation](riemannian-geometry.md#geodesic-equation) imply

$$
h_{00}=-2\Phi,
\qquad
\kappa=8\pi G,
$$

where the [Poisson equation](partial-differential-equation.md#poisson-s-equation) is $\nabla^2\Phi=4\pi G\rho$.

### Newtonian connection from an exponential lapse

↑ **Parent:** [Newtonian limit](#newtonian-limit)

For smooth spatial $\phi$ and $g(c)=-c^2e^{2\phi/c^2}dt^2+\delta_{ij}dx^idx^j$, the only nonzero [Christoffel symbols](riemannian-geometry.md#christoffel-symbol) are $\Gamma^t{}_{ti}=\Gamma^t{}_{it}=c^{-2}\partial_i\phi$ and $\Gamma^i{}_{tt}=e^{2\phi/c^2}\partial_i\phi$. Consequently the [Levi-Civita connection](general-relativity.md#levi-civita-connection) converges smoothly on compact sets as $c\to\infty$ although the metric itself diverges in these coordinates. The limiting [torsion-free connection](vector-bundle.md#torsion-free-connection) has only $\Gamma^i{}_{tt}=\partial_i\phi$ and gives $d^2x^i/dt^2=-\partial_i\phi$ when $t$ is an [affine parameter](riemannian-geometry.md#affine-parameter). With $R^a{}_{bcd}=\partial_c\Gamma^a{}_{db}-\partial_d\Gamma^a{}_{cb}+\cdots$, its [Ricci tensor](riemann-curvature-tensor.md#ricci-tensor) is $(\Delta\phi)dt\otimes dt$: quadratic connection terms vanish and $R^i{}_{tjt}=\partial_j\partial_i\phi$. Thus zero Ricci tensor is the [Laplace equation](partial-differential-equation.md#laplace-equation), while full flatness would require the entire Hessian to vanish.

### Static radius

↑ **Parent:** [Newtonian limit](#newtonian-limit)

For a point mass in a positive [cosmological constant](cosmology.md#cosmological-constant), the inward Newtonian acceleration $GM/r^2$ balances the outward cosmological acceleration $\Lambda r/3$ at the static radius $r_{\rm s}=(3GM/\Lambda)^{1/3}$.

### Linearized point-mass metric in radial Cartesian form

↑ **Parent:** [Newtonian limit](#newtonian-limit)

For a point mass and $r>0$, write

$$
h_{00}=\frac{2GM}{r},
\qquad
h_{ij}=f(r)x_i x_j.
$$

The vacuum scalar-curvature equation gives $rf'+3f=0$, so $f=C/r^3$. The remaining vacuum equations fix $C=2GM$ in the corresponding Schwarzschild gauge.

## Slowly rotating weak-field metric

↑ **Parent:** [Linearized gravity](linearized-gravity.md)

Far from a slowly rotating isolated body of mass $m$ and angular momentum $\mathbf J$, the scalar part of the metric is the linearized point-mass field while $g_{0i}$ is the dipole field of $\mathbf J$. For rotation about the z-axis, the cross term is $4Jr^{-3}(y\,dx-x\,dy)dt$ in a common convention.

## ↑ Ancestors (4)

1. [General relativity](general-relativity.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Far-zone quadrupole strain](gravitational-wave.md#far-zone-quadrupole-strain)
- [Frame dragging inside a slowly rotating spherical shell](black-hole.md#frame-dragging-inside-a-slowly-rotating-spherical-shell)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#3/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#37d/i/solution)
