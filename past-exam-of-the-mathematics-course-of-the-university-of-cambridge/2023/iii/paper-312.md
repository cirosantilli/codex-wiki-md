# Paper 312

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_312.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_312.pdf)

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
  - [v](#1/v)
    - [Solution](#1/v/solution)
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
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Under [spatial reflection](../../../quantum-mechanics.md#spatial-reflection), a [scalar field](../../../quantum-field-theory.md#scalar-field) obeys $P\phi(\mathbf x)P=\phi(-\mathbf x)$, and hence each [spatial derivative](../../../calculus.md#spatial-derivative) changes sign. The interaction contains three such derivatives, so changing the integration variable from $\mathbf x$ to $-\mathbf x$ gives

$$
PH_{\rm int}P=-H_{\rm int}.
$$

Thus this is a [parity-odd scalar interaction](../../../quantum-field-theory.md#parity-odd-scalar-interaction).

Put $O(\mathbf k_a)=\prod_{a=1}^n\phi_a(\mathbf k_a)$ and $A(\mathbf k_a)=\langle H_{\rm int}O(\mathbf k_a)\rangle$. [Hermitian conjugation](../../../hilbert-space.md#hermitian-conjugation) and commutativity of equal-time scalar fields give

$$
\langle O(\mathbf k_a)H_{\rm int}\rangle
=A(-\mathbf k_a)^*.
$$

The [parity-invariant vacuum](../../../quantum-field-theory.md#parity-invariant-vacuum) and the odd parity of $H_{\rm int}$ imply $A(-\mathbf k_a)=-A(\mathbf k_a)$. Therefore

$$
\boxed{\langle[H_{\rm int},O]\rangle
=A-A(-\mathbf k_a)^*=A+A^*=2\operatorname{Re}A}.
$$

There is no conflict with the usual $2i\operatorname{Im}A$ rule for two [Hermitian operators](../../../hilbert-space.md#hermitian-operator): a momentum-space product at fixed $\mathbf k_a$ is generally not itself Hermitian, since its adjoint carries momenta $-\mathbf k_a$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The first-order [in-in formalism](../../../quantum-field-theory.md#keldysh-formalism) formula at observation time $\tau_0$ is

$$
\langle O(\tau_0)\rangle_{\lambda}
=i\int_{-\infty(1-i\epsilon)}^{\tau_0}d\tau\,
\langle[H_{\rm int}(\tau),O_I(\tau_0)]\rangle.
$$

Fourier transforming the three derivatives gives

$$
H_{\rm int}(\tau)
=-i\lambda a^4
\int_{\mathbf p_1\cdots\mathbf p_4}
(2\pi)^3\delta^{(3)}(\mathbf p_1+\cdots+\mathbf p_4)
\,[\mathbf p_2\mathbin\cdot(\mathbf p_3\mathbin\times\mathbf p_4)]
\prod_{a=1}^4\phi_a(\mathbf p_a,\tau),
$$

where $\int_{\mathbf p}=\int d^3p/(2\pi)^3$. Because the four species are distinct, [Wick contraction](../../../perturbative-quantum-field-theory.md#wick-contraction) pairs each vertex field with the external field of the same species and introduces no permutation factor. If

$$
\mathcal E=\mathbf k_2\mathbin\cdot(\mathbf k_3\mathbin\times\mathbf k_4),
\qquad k_T=k_1+k_2+k_3+k_4,
$$

then

$$
\langle H_{\rm int}(\tau)O(\tau_0)\rangle
=i\lambda a^4(\tau)(2\pi)^3\delta^{(3)}\!\left(\sum_a\mathbf k_a\right)
\mathcal E\prod_{a=1}^4f(k_a,\tau)f^*(k_a,\tau_0).
$$

Combining this with part i gives the requested [time integral](../../../calculus.md#time-integral):

$$
\boxed{
\langle O(\tau_0)\rangle_{\lambda}
=2i\lambda(2\pi)^3\delta^{(3)}\!\left(\sum_a\mathbf k_a\right)\mathcal E
\int_{-\infty(1-i\epsilon)}^{\tau_0}d\tau\,a^4(\tau)
\operatorname{Re}\left[i\prod_{a=1}^4f(k_a,\tau)f^*(k_a,\tau_0)\right]}.
$$

The factor $\mathcal E$ is a [pseudoscalar](../../../quantum-mechanics.md#pseudoscalar), so the resulting [primordial trispectrum](../../../cosmology.md#primordial-trispectrum) is parity odd and purely imaginary in this momentum-space convention.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

The intended oscillatory factor is $e^{-ik\tau}$. Give the early-time endpoint the usual [i-epsilon prescription](../../../quantum-field-theory.md#feynman-i-epsilon-prescription) and set $x=-k\tau$. For an integer $p\geq0$,

$$
\begin{aligned}
I_p&=\int_{-\infty(1-i\epsilon)}^0e^{-ik\tau}(i\tau)^p\,d\tau\\
&=\frac{(-i)^p}{k^{p+1}}
\lim_{\epsilon\downarrow0}\int_0^\infty x^pe^{-(\epsilon-i)x}\,dx\\
&=\frac{(-i)^p\Gamma(p+1)}{k^{p+1}}
\lim_{\epsilon\downarrow0}(\epsilon-i)^{-(p+1)}
=\boxed{\frac{i\,p!}{k^{p+1}}}.
\end{aligned}
$$

It is therefore purely imaginary. Equivalently, rotating the contour to the negative imaginary $\tau$ axis turns the remaining integral into a real [Gamma integral](../../../complex-analysis.md#gamma-integral) and leaves one overall factor of $i$.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

At late time $f(k,\tau_0)\to H/\sqrt{2k^3}$ and $a=-1/(H\tau)$. Define the [elementary symmetric polynomials](../../../polynomial.md#elementary-symmetric-polynomial)

$$
e_2=\sum_{a<b}k_ak_b,
\qquad e_3=\sum_{a<b<c}k_ak_bk_c,
\qquad e_4=k_1k_2k_3k_4.
$$

Then part ii reduces to

$$
\langle O\rangle'_\lambda
=-\frac{i\lambda H^4\mathcal E}{8\prod_a k_a^3}\operatorname{Im}J(\tau_0),
$$

where a prime removes the momentum-conserving [Dirac delta distribution](../../../distribution-theory.md#dirac-delta-function) and

$$
J(\tau_0)=\int_{-\infty(1-i\epsilon)}^{\tau_0}
\frac{d\tau}{\tau^4}e^{-ik_T\tau}
\prod_{a=1}^4(1+ik_a\tau).
$$

Expanding the product gives

$$
\frac1{\tau^4}\prod_a(1+ik_a\tau)
=\frac1{\tau^4}+\frac{ik_T}{\tau^3}-\frac{e_2}{\tau^2}
-\frac{ie_3}{\tau}+e_4.
$$

Repeated [integration by parts](../../../calculus.md#integration-by-parts) reduces every negative power to the supplied logarithmic integral. The power divergences are real and disappear when the imaginary part is taken. Writing

$$
L_T=\gamma_E+\log|k_T\tau_0|,
$$

one obtains

$$
\operatorname{Im}J
=\left(-\frac{k_T^3}{3}+k_Te_2-e_3\right)L_T
+\frac{4k_T^3}{9}-k_Te_2+\frac{e_4}{k_T}+o(1).
$$

Consequently the late-time [parity-odd primordial trispectrum](../../../cosmology.md#parity-odd-primordial-trispectrum) is

$$
\boxed{
\langle\phi_1(\mathbf k_1)\phi_2(\mathbf k_2)
\phi_3(\mathbf k_3)\phi_4(\mathbf k_4)\rangle'
=-\frac{i\lambda H^4}{8\prod_a k_a^3}
[\mathbf k_2\mathbin\cdot(\mathbf k_3\mathbin\times\mathbf k_4)]
\left[
\left(-\frac{k_T^3}{3}+k_Te_2-e_3\right)L_T
+\frac{4k_T^3}{9}-k_Te_2+\frac{e_4}{k_T}
\right]}.
$$

Its factor of $i$ is required by [reality of a momentum-space scalar correlator](../../../cosmology.md#reality-of-a-momentum-space-scalar-correlator): reversing all momenta complex-conjugates the correlator, while the [scalar triple product](../../../linear-algebra.md#scalar-triple-product) changes sign.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

[Statistical homogeneity](../../../probability-and-statistics.md#statistical-homogeneity) forces a scalar two-point function to have momenta $(\mathbf k,-\mathbf k)$. [Statistical isotropy](../../../probability-and-statistics.md#statistical-isotropy) then makes it a function only of $|\mathbf k|$, so it is parity even without using perturbation theory.

For a scalar three-point function, momentum conservation gives $\mathbf k_1+\mathbf k_2+\mathbf k_3=0$, so all three vectors lie in one plane. A rotation by $\pi$ around the normal to that plane sends every $\mathbf k_a$ to $-\mathbf k_a$. Rotational invariance therefore identifies a triangle with its parity reverse, proving nonperturbatively that the scalar [primordial bispectrum](../../../cosmology.md#primordial-bispectrum) is parity even.

A rotationally invariant local parity-odd three-scalar vertex must contain a [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) contracted with three spatial momenta. Its momentum-space factor is proportional to

$$
\epsilon_{ijk}k_1^ik_2^jk_3^k
=\mathbf k_1\mathbin\cdot(\mathbf k_2\mathbin\times\mathbf k_3)=0,
$$

because momentum conservation makes the momenta linearly dependent. The equivalent position-space expression is a [total divergence](../../../calculus.md#total-divergence); its spatial integral vanishes under the stated [vanishing boundary condition](../../../differential-equation.md#vanishing-boundary-condition). Thus a parity-odd interaction of three scalar fields contributes nothing to the action.

## 2

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The background spatial metric is $g_{ij}=a^2\delta_{ij}$. For the [large spatial diffeomorphism](../../../geometry-and-topology.md#large-spatial-diffeomorphism)

$$
\epsilon^0=0,
\qquad \epsilon^i=\omega^i{}_jx^j,
\qquad \omega_{ij}=\omega_{ji},
\qquad \omega_i{}^i=0,
$$

homogeneity and isotropy imply that the purely spatial background [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) vanish. Hence

$$
\nabla_i\epsilon_j=a^2\omega_{ji},
\qquad
\boxed{\Delta\gamma_{ij}=-2\omega_{ij}}.
$$

The shift is constant, transverse and traceless, and is therefore the zero-momentum [adiabatic tensor mode](../../../cosmic-inflation.md#adiabatic-tensor-mode).

A scalar transforms by its [Lie derivative](../../../differential-form.md#lie-derivative-of-a-differential-form):

$$
\Delta\varphi(\mathbf x)
=-\omega_{ij}x^j\partial_i\varphi(\mathbf x).
$$

Fourier transformation and [integration by parts](../../../calculus.md#integration-by-parts) in momentum space give

$$
\boxed{\Delta\varphi(\mathbf k)
=\omega_{ij}k_i\frac{\partial}{\partial k_j}\varphi(\mathbf k)}.
$$

The term proportional to $\omega_i{}^i$ vanishes because the deformation is traceless.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The equal-time [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation) for the transverse-traceless graviton and its [canonical momentum](../../../classical-mechanics.md#canonical-momentum) is the [transverse-traceless projector](../../../general-relativity.md#transverse-traceless-projector). At zero momentum the supplied [polarization completeness relation](../../../general-relativity.md#polarization-completeness-relation) gives

$$
i[Q_S,\gamma_{mn}]
=-2\omega_{ij}\sum_s2\epsilon_{ij}^s(\mathbf0)
\epsilon_{mn}^s(-\mathbf0)
=-2\omega_{mn},
$$

where symmetry and tracelessness of $\omega_{ij}$ remove the trace term. Thus the charge generates precisely the transformation in part i:

$$
\boxed{i[Q_S,\gamma_{mn}]=\Delta\gamma_{mn}}.
$$

This is the soft, field-independent part of the [Noether charge](../../../quantum-field-theory.md#noether-charge) associated with the large diffeomorphism.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Let $O=\varphi(\mathbf k_1)\varphi(\mathbf k_2)$. Since $Q_S=-2\omega_{ij}\Pi_{ij}(\mathbf0)$,

$$
i\langle[Q_S,O]\rangle
=4\omega_{ij}\operatorname{Im}\langle\Pi_{ij}(\mathbf0)O\rangle.
$$

For a soft mode $\gamma^s=f_q a_s+f_q^*a_s^\dagger$ and $\Pi^s=g_q a_s+g_q^*a_s^\dagger$, the vacuum obeys

$$
\langle0|\Pi^s(\mathbf q)
=\frac{g_q}{f_q}\langle0|\gamma^s(\mathbf q).
$$

The mode-function [Wronskian normalization](../../../quantum-field-theory.md#wronskian-normalization)

$$
f_qg_q^*-f_q^*g_q=i
$$

implies

$$
\operatorname{Im}\frac{g_q}{f_q}
=-\frac1{2|f_q|^2}=-\frac1{2P_\gamma(q)},
$$

where $P_\gamma(q)$ is the [graviton power spectrum](../../../cosmic-inflation.md#graviton-power-spectrum) per polarization. The equal-time bispectrum is real in this parity-even configuration, and therefore

$$
\boxed{
i\langle[Q_S,O]\rangle'
=-2\omega_{ij}\lim_{\mathbf q\to0}
\frac{\langle\gamma_{ij}(\mathbf q)
\varphi(\mathbf k_1)\varphi(\mathbf k_2)\rangle'}{P_\gamma(q)}}.
$$

This turns the charge insertion into the soft-graviton insertion used in the [Soft graviton theorem](../../../quantum-field-theory.md#soft-graviton-theorem).

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Applying the scalar transformation from part i to both fields gives

$$
\langle\Delta O\rangle
=\omega_{ij}\sum_{a=1}^2k_{a i}\frac{\partial}{\partial k_{a j}}
\left[(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2)P_\varphi(k_1)\right].
$$

The derivative of the [Dirac delta distribution](../../../distribution-theory.md#dirac-delta-function) is proportional to $\delta_{ij}$ and vanishes after contraction with traceless $\omega_{ij}$. Removing that delta function leaves

$$
\langle\Delta O\rangle'
=\omega_{ij}k_i\frac{\partial}{\partial k_j}P_\varphi(k).
$$

Equating the two sides of the [Ward-Takahashi identity](../../../perturbative-quantum-field-theory.md#ward-identity) and resolving the soft graviton into a polarization $s$ yields the [cosmological soft-graviton consistency relation](../../../cosmic-inflation.md#cosmological-soft-graviton-consistency-relation)

$$
\boxed{
\lim_{q\to0}
\frac{\langle\gamma^s(\mathbf q)
\varphi(\mathbf k)\varphi(-\mathbf k-\mathbf q)\rangle'}{P_\gamma(q)}
=-\frac12\epsilon_{ij}^s(\mathbf q)
k_i\frac{\partial}{\partial k_j}P_\varphi(k)}.
$$

For an isotropic power spectrum this is equivalently

$$
-\epsilon_{ij}^s k_i k_j\frac{\partial P_\varphi}{\partial k^2}.
$$

The long-wavelength [adiabatic tensor mode](../../../cosmic-inflation.md#adiabatic-tensor-mode) acts on the short two-point function as an anisotropic rescaling of its momentum.

## 3

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Let the photon [phase-space distribution](../../../statistical-physics.md#phase-space-distribution-function) be a Planck distribution whose local temperature is $T(\eta)[1+\Theta(\eta,\mathbf x,\widehat{\mathbf p})]$. In the absence of collisions, [Liouville theorem](../../../complex-analysis.md#liouville-theorem) says that the distribution is constant along a photon [null geodesic](../../../special-relativity.md#null-geodesic). Linearizing $df/d\eta=0$ about the homogeneous distribution and using $d\mathbf x/d\eta=\widehat{\mathbf p}$ gives

$$
\left(\partial_\eta+\widehat{\mathbf p}\mathbin\cdot\nabla\right)\Theta
-\frac{d\log\epsilon}{d\eta}=0.
$$

A spatial [Fourier transform](../../../analysis.md#fourier-transform) sends $\widehat{\mathbf p}\mathbin\cdot\nabla$ to $i\widehat{\mathbf p}\mathbin\cdot\mathbf k$, so

$$
\boxed{
\frac{\partial\Theta}{\partial\eta}
+i(\widehat{\mathbf p}\mathbin\cdot\mathbf k)\Theta
-\frac{d\log\epsilon}{d\eta}=0}.
$$

This is the [Free-streaming photon Boltzmann equation](../../../cosmic-microwave-background-anisotropy.md#free-streaming-photon-boltzmann-equation): the second term transports angular structure, while the last term is the gravitational redshift source.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Write $\mu=\widehat{\mathbf k}\mathbin\cdot\widehat{\mathbf p}$ and use the [Legendre polynomial recurrence relation](../../../differential-equation.md#legendre-polynomial-recurrence-relation). The definition in the question is inverted by

$$
\Theta(\mu)=\sum_{\ell\geq0}(2\ell+1)(-i)^\ell
\Theta_\ell P_\ell(\mu).
$$

For Newtonian-gauge potentials the scanned geodesic equation is the standard identity

$$
\frac{d\log\epsilon}{d\eta}
=-\frac{d\Psi}{d\eta}+\Phi'+\Psi'
=\Phi'-\widehat{\mathbf p}\mathbin\cdot\nabla\Psi.
$$

Its monopole and dipole are $S_0=\Phi'$ and $S_1=k\Psi/3$. Projecting the [photon Boltzmann hierarchy](../../../cosmic-microwave-background-anisotropy.md#photon-boltzmann-hierarchy) onto $P_0$ and $P_1$ therefore gives

$$
\boxed{\Theta_0'+k\Theta_1=\Phi'},
$$



$$
\boxed{\Theta_1'=\frac{k}{3}
(\Theta_0+\Psi-2\Theta_2)}.
$$

The first is the photon [continuity equation](../../../physics.md#continuity-equation); the second is the [photon Euler equation](../../../cosmic-microwave-background-anisotropy.md#photon-euler-equation), with the [photon quadrupole](../../../cosmic-microwave-background-anisotropy.md#photon-quadrupole) providing the anisotropic-stress term. Indeed, with photon density contrast $\delta_\gamma=4\Theta_0$ and velocity divergence $\theta_\gamma=3k\Theta_1$,

$$
\boxed{\delta_\gamma'=-\frac43\theta_\gamma+4\Phi',
\qquad
\theta_\gamma'=k^2(\delta_\gamma/4+\Psi-2\Theta_2).}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The [line-of-sight solution for free-streaming photons](../../../cosmic-microwave-background-anisotropy.md#line-of-sight-solution-for-free-streaming-photons) follows the unperturbed ray $\mathbf x(\eta)=\mathbf x_0-\widehat{\mathbf p}(\eta_f-\eta)$. If $\Phi=\Psi$ is spatially homogeneous, its gradient vanishes and $d\log\epsilon/d\eta=\Phi'$. Integration along the ray gives

$$
\boxed{
\Theta(\eta_f,\mathbf x_0,\widehat{\mathbf p})
=\Theta(\eta_i,
\mathbf x_0-\widehat{\mathbf p}(\eta_f-\eta_i),
\widehat{\mathbf p})
+\Phi(\eta_f)-\Phi(\eta_i)}.
$$

The needed initial condition is the temperature pattern on the initial hypersurface; for a superhorizon adiabatic mode during matter domination one may use $\Theta_0(\eta_i)=-2\Psi(\eta_i)/3$.

This calculation contains free streaming of the initial pattern and the gravitational temperature shift caused by the evolving potential, the homogeneous limit of the [Integrated Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#integrated-sachs-wolfe-effect). A perfectly homogeneous potential changes only the unobservable sky monopole and therefore contributes no [CMB angular power spectrum](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-power-spectrum) for $\ell\geq1$. Direction-dependent [Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-effect), Doppler, acoustic, polarization, lensing, and rescattering contributions require spatially varying perturbations or collision terms and are outside this special calculation.

## 4

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Linearizing the [cosmological Euler equation](../../../linear-cosmological-perturbation-theory.md#cosmological-euler-equation) gives

$$
\mathbf v'+\mathcal H\mathbf v=-\nabla\phi.
$$

Taking the [curl](../../../calculus.md#curl) removes the gradient force, so the [vorticity](../../../fluid-mechanics.md#vorticity) $\mathbf w=\nabla\mathbin\times\mathbf v$ obeys

$$
\boxed{\mathbf w'+\mathcal H\mathbf w=0}.
$$

Since $\mathcal H=a'/a$, its solution is

$$
\boxed{\mathbf w\propto a^{-1}}.
$$

**Thus expansion dilutes linear vorticity; in an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), $a\propto\tau^2$ and $\mathbf w\propto\tau^{-2}$.**

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The linearized [cosmological continuity equation](../../../cosmology.md#cosmological-continuity-equation), the divergence of the [cosmological Euler equation](../../../linear-cosmological-perturbation-theory.md#cosmological-euler-equation), and the [cosmological Poisson equation](../../../linear-cosmological-perturbation-theory.md#cosmological-poisson-equation) give

$$
\boxed{\delta'+\theta=0},
\qquad
\boxed{\theta'+\mathcal H\theta
+\frac32\mathcal H^2\Omega_m\delta=0}.
$$

Eliminating $\theta=-\delta'$ yields the equation for a [linear cosmological density perturbation](../../../linear-cosmological-density-perturbation.md):

$$
\boxed{\delta''+\mathcal H\delta'
-\frac32\mathcal H^2\Omega_m\delta=0}.
$$

In an [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), $\Omega_m=1$ and $\mathcal H=2/\tau$, so

$$
\delta''+\frac2\tau\delta'-\frac6{\tau^2}\delta=0.
$$

Substitution of the [power-law ansatz](../../../differential-equation.md#power-law-ansatz) $\delta\propto\tau^p$ gives $(p-2)(p+3)=0$. Hence

$$
\delta=C_+\tau^2+C_-\tau^{-3}
=D_+a+D_-a^{-3/2}.
$$

The leading one of the [matter-era growing and decaying density modes](../../../linear-cosmological-density-perturbation.md#matter-era-growing-and-decaying-density-modes) is $\delta\propto a\propto\tau^2$, as direct substitution confirms, and its velocity divergence is

$$
\boxed{\theta=-\delta'=-\mathcal H\delta\propto-\tau}.
$$

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

In [standard perturbation theory in cosmology](../../../large-scale-structure-of-the-universe.md#standard-perturbation-theory-in-cosmology), $\delta^{(n)}$ is an $n$-leg vertex carrying the symmetrized [standard perturbation theory density kernel](../../../large-scale-structure-of-the-universe.md#standard-perturbation-theory-density-kernel) $F_n$. For [Gaussian random fields](../../../stochastic-process.md#gaussian-random-field), a connected four-point diagram with $L$ loops contains $3+L$ linear [power spectra](../../../probability-and-statistics.md#power-spectrum), hence $6+2L$ linear fields.

At tree level the required perturbative-order partitions are

$$
3+1+1+1,
\qquad
2+2+1+1.
$$

The first is a star with one $F_3$ vertex and three linear external legs. The second has two $F_2$ vertices joined by one internal power-spectrum line, with one linear external leg attached to each vertex. At one loop all five partitions of eight into four positive parts are required:

$$
5+1+1+1,
\quad4+2+1+1,
\quad3+3+1+1,
\quad3+2+2+1,
\quad2+2+2+2.
$$

These are conventionally denoted $T_{5111}$, $T_{4211}$, $T_{3311}$, $T_{3221}$, and $T_{2222}$; all inequivalent placements of external legs and all [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction) are understood. This list is the complete set of [one-loop matter trispectrum](../../../large-scale-structure-of-the-universe.md#one-loop-matter-trispectrum) topologies.

Let $P_a=P_L(k_a)$ and $\mathbf k_{ab}=\mathbf k_a+\mathbf k_b$. With $\sum_a\mathbf k_a=0$, the star contribution is

$$
\boxed{
T_{3111}=6\sum_{d=1}^4
F_3(-\mathbf k_a,-\mathbf k_b,-\mathbf k_c)
P_aP_bP_c},
$$

where $\{a,b,c\}=\{1,2,3,4\}\setminus\{d\}$. For the exchange contribution, sum over the six unordered choices $\{a,b\}$ of linear external legs and let $\{c,d\}$ be the complementary pair:

$$
\boxed{
T_{2211}=4\sum_{\{a,b\}}
P_aP_b\left[
P_L(k_{ac})F_2(-\mathbf k_a,\mathbf k_{ac})
F_2(-\mathbf k_b,-\mathbf k_{ac})
+P_L(k_{ad})F_2(-\mathbf k_a,\mathbf k_{ad})
F_2(-\mathbf k_b,-\mathbf k_{ad})
\right]}.
$$

Thus the connected tree trispectrum is $T_{\rm tree}=T_{3111}+T_{2211}$.

The pressureless single-stream equations cease to be a complete one-loop prediction because loop momenta probe short nonlinear scales and produce ultraviolet-sensitive terms. A consistent result must include the [effective field theory of large-scale structure](../../../large-scale-structure-of-the-universe.md#effective-field-theory-of-large-scale-structure): effective-stress counterterms, including their insertions into the tree topologies, and stochastic terms at the order allowed by [mass conservation](../../../continuum-mechanics.md#mass-conservation) and [momentum conservation](../../../classical-mechanics.md#momentum-conservation). Their coefficients absorb short-scale dependence and must be fitted or matched. If the observable is a biased tracer rather than matter itself, the corresponding renormalized [bias expansion](../../../large-scale-structure-of-the-universe.md#bias-expansion) is also required.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
