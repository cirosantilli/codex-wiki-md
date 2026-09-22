# Paper 312

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_312.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_312.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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

## 1

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The operator $\dot\phi^2\phi$ is not invariant under a [scalar-field shift symmetry](../../../quantum-field-theory.md#scalar-field-shift-symmetry) because one field is undifferentiated. An arbitrary large coefficient would therefore radiatively generate equally unsuppressed nonderivative operators, including a mass and a steep [scalar potential](../../../quantum-field-theory.md#scalar-potential), and would spoil the approximate shift symmetry and flat potential needed for [single-field slow-roll inflation](../../../cosmic-inflation.md#single-field-slow-roll-inflation). In a technically natural slow-roll model its coefficient must consequently be small, so it does not produce parametrically large [primordial non-Gaussianity](../../../cosmology.md#primordial-non-gaussianity). Treated merely as an effective spectator-field interaction, it does generate the tree-level [primordial bispectrum](../../../cosmology.md#primordial-bispectrum) computed below, whose size is controlled by the dimensionless interaction strength at the Hubble scale; taking that strength large abandons the controlled slow-roll premise.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Since $dt=a\,d\tau$ and $\dot\phi=a^{-1}\phi'$, the interaction is

$$
S_{\rm int}=\frac\lambda{3!}\int d\tau\,d^3x\,a^2\phi'^2\phi,
\qquad
H_{\rm int}=-\frac\lambda{3!}\int d^3x\,a^2\phi'^2\phi
$$

to first order in $\lambda$. The tree-level [in-in formalism](../../../quantum-field-theory.md#keldysh-formalism) gives

$$
\langle\phi_{\mathbf k_1}\phi_{\mathbf k_2}\phi_{\mathbf k_3}\rangle
=2\operatorname{Im}\int_{-\infty(1-i\epsilon)}^0d\tau\,
\langle0|\phi_{\mathbf k_1}(0)\phi_{\mathbf k_2}(0)
\phi_{\mathbf k_3}(0)H_{\rm int}(\tau)|0\rangle.
$$

There are two [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction) for each choice of the undifferentiated field at the vertex. With $K=k_1+k_2+k_3$, the stated [Bunch-Davies vacuum](../../../cosmic-inflation.md#bunch-davies-vacuum) mode obeys

$$
f_k(0)=\frac{H}{\sqrt{2k^3}},
\qquad
f_k^{*\prime}(\tau)=\frac{Hk^2\tau}{\sqrt{2k^3}}e^{ik\tau}.
$$

The two powers of $\tau$ from the differentiated modes cancel $a^2=1/(H^2\tau^2)$, and the remaining integral is

$$
\int_{-\infty(1-i\epsilon)}^0
(1-ik_i\tau)e^{iK\tau}\,d\tau
=-i\frac{K+k_i}{K^2}.
$$

Removing the momentum-conserving delta function, the [bispectrum from a time-derivative cubic scalar interaction](../../../cosmology.md#bispectrum-from-a-time-derivative-cubic-scalar-interaction) is therefore

$$
\boxed{
B(k_1,k_2,k_3)=
\frac{\lambda H^4}{12k_1^3k_2^3k_3^3K^2}
\left[
k_2^2k_3^2(K+k_1)+k_3^2k_1^2(K+k_2)
+k_1^2k_2^2(K+k_3)
\right]}.
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

With the [Fourier transform](../../../analysis.md#fourier-transform) convention $\phi(\mathbf k)=\int d^3x\,e^{-i\mathbf k\cdot\mathbf x}\phi(\mathbf x)$, scale invariance of the position-space three-point function gives

$$
\langle\phi(\mu\mathbf k_1)\phi(\mu\mathbf k_2)\phi(\mu\mathbf k_3)\rangle
=\mu^{-9}\langle\phi(\mathbf k_1)\phi(\mathbf k_2)\phi(\mathbf k_3)\rangle.
$$

Because $\delta^{(3)}(\mu\sum_i\mathbf k_i)=\mu^{-3}\delta^{(3)}(\sum_i\mathbf k_i)$, the reduced [primordial bispectrum](../../../cosmology.md#primordial-bispectrum) must satisfy

$$
\boxed{B(\mu k_1,\mu k_2,\mu k_3)=\mu^{-6}B(k_1,k_2,k_3)}.
$$

In the result of part b, the bracket has momentum degree five, while $k_1^3k_2^3k_3^3K^2$ has degree eleven. Its total degree is therefore $-6$, exactly as required.

## 2

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The constant [scalar-field shift symmetry](../../../quantum-field-theory.md#scalar-field-shift-symmetry) has momentum-space action

$$
\boxed{\Delta\phi(\mathbf k)=c(2\pi)^3\delta^{(3)}(\mathbf k)}.
$$

For the [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation) $[\phi(\mathbf x),\Pi(\mathbf y)]=i\delta^{(3)}(\mathbf x-\mathbf y)$, its [Noether charge](../../../quantum-field-theory.md#noether-charge) can be written

$$
\boxed{Q=c\int d^3x\,\Pi(\mathbf x)=c\,\Pi(\mathbf k=0)}.
$$

Indeed, $i[Q,\phi(\mathbf x)]=c$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Regulate the zero mode by a soft momentum $\mathbf q$ and write the free modes as

$$
\phi_{\mathbf q}=f_q a_{\mathbf q}+f_q^*a_{-\mathbf q}^\dagger,
\qquad
\Pi_{\mathbf q}=g_q a_{\mathbf q}+g_q^*a_{-\mathbf q}^\dagger.
$$

The [Wronskian normalization](../../../quantum-field-theory.md#wronskian-normalization) $f_qg_q^*-f_q^*g_q=i$ follows from the canonical commutator, while the [power spectrum](../../../probability-and-statistics.md#power-spectrum) is $P(q)=|f_q|^2$. Inserting the creation part of $Q$ on the ket and the annihilation part on the bra, their difference is precisely the Wronskian. For ${\cal O}=\phi(\mathbf k)\phi(\mathbf k')$ this gives, after taking $q\to0$ and setting the irrelevant normalization $c=1$,

$$
\boxed{i\langle[Q,{\cal O}]\rangle
=\frac1{P(0)}
\langle\phi(\mathbf k)\phi(\mathbf k')\phi(\mathbf0)\rangle}.
$$

Equivalently, before removing the regulator, the right-hand side is the soft three-point function divided by $P(q)$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The variation of the product is

$$
\Delta[\phi(\mathbf k)\phi(\mathbf k')]
=c(2\pi)^3\left[
\delta^{(3)}(\mathbf k)\phi(\mathbf k')
+\delta^{(3)}(\mathbf k')\phi(\mathbf k)
\right].
$$

Its expectation value vanishes because the background has $\langle\phi\rangle=0$. The [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity) and part b therefore give the [shift-symmetry soft theorem for a scalar bispectrum](../../../cosmology.md#shift-symmetry-soft-theorem-for-a-scalar-bispectrum)

$$
\boxed{\lim_{q\to0}
\frac{B_\phi(q,k,|\mathbf k+\mathbf q|)}{P_\phi(q)}=0}.
$$

**Thus an exact internal shift creates no leading soft response of the two hard modes.**

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [single-field inflation squeezed-limit consistency relation](../../../cosmology.md#single-field-inflation-squeezed-limit-consistency-relation) for the [comoving curvature perturbation](../../../cosmic-inflation.md#comoving-curvature-perturbation) is

$$
\boxed{\lim_{q\to0}
B_{\mathcal R}(q,k,|\mathbf k+\mathbf q|)
=-(n_s-1)P_{\mathcal R}(q)P_{\mathcal R}(k)}.
$$

Equivalently, $B_{\mathcal R}/P_{\mathcal R}(q)=-(3+k\partial_k)P_{\mathcal R}(k)$. The scalar shift in parts a--c is an internal symmetry and leaves the hard fields unchanged, so its right-hand side vanishes. A long adiabatic curvature mode instead acts as a spatial dilation of the hard coordinates, and its response is the scale dependence measured by the [scalar spectral index](../../../cosmic-inflation.md#scalar-spectral-index).

## 3

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [cosmological continuity equation](../../../cosmology.md#cosmological-continuity-equation) expresses conservation of dark-matter mass: $\delta$ is the [density contrast](../../../linear-cosmological-density-perturbation.md#density-contrast), $\mathbf v$ is the [peculiar velocity](../../../cosmology.md#peculiar-velocity), and a prime denotes a [conformal time](../../../cosmology.md#conformal-time) derivative. The [cosmological Euler equation](../../../linear-cosmological-perturbation-theory.md#cosmological-euler-equation) expresses momentum conservation: $\mathcal H=a'/a$ is the conformal Hubble rate, $\phi$ is the [peculiar gravitational potential](../../../linear-cosmological-density-perturbation.md#peculiar-gravitational-potential), $\rho$ is the density, and $\sigma_{ij}$ is the [velocity-dispersion tensor of collisionless matter](../../../large-scale-structure-of-the-universe.md#velocity-dispersion-tensor-of-collisionless-matter). The terms are respectively Hubble drag, convective acceleration, gravity, and velocity-dispersion stress.

For curl-free flow, introduce the [peculiar-velocity divergence](../../../cosmology.md#peculiar-velocity-divergence) $\theta=\nabla\cdot\mathbf v$ and set $\sigma_{ij}=0$. A [Fourier transform](../../../analysis.md#fourier-transform) of the nonlinear continuity term gives

$$
\delta'(\mathbf k)+\theta(\mathbf k)
=-\int\frac{d^3q}{(2\pi)^3}
\alpha(\mathbf q,\mathbf k-\mathbf q)
\theta(\mathbf q)\delta(\mathbf k-\mathbf q),
$$

with the [alpha mode-coupling kernel](../../../large-scale-structure-of-the-universe.md#alpha-mode-coupling-kernel)

$$
\boxed{\alpha(\mathbf k_1,\mathbf k_2)
=\frac{(\mathbf k_1+\mathbf k_2)\cdot\mathbf k_1}{k_1^2}}.
$$

Taking the divergence of the Euler equation gives the quadratic velocity kernel

$$
\boxed{\beta(\mathbf k_1,\mathbf k_2)
=\frac{|\mathbf k_1+\mathbf k_2|^2
(\mathbf k_1\cdot\mathbf k_2)}{2k_1^2k_2^2}}.
$$

This is the [beta mode-coupling kernel](../../../large-scale-structure-of-the-universe.md#beta-mode-coupling-kernel); its symmetry follows from the two velocity factors.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Expand $\delta=\delta^{(1)}+\delta^{(2)}+\delta^{(3)}+\cdots$, where the [standard perturbation theory density kernel](../../../large-scale-structure-of-the-universe.md#standard-perturbation-theory-density-kernel) $F_n$ convolves $n$ linear fields. Through fourth order in the Gaussian linear field, the only power-spectrum diagrams are the tree contraction $P_{11}$, the loop joining two $F_2$ vertices $P_{22}$, and the two orderings that join an $F_3$ vertex to a linear leg, $P_{13}+P_{31}=2P_{13}$. Their expressions are

$$
P_{11}(k)=P_L(k),
$$



$$
P_{22}(k)=2\int\frac{d^3q}{(2\pi)^3}
F_2(\mathbf q,\mathbf k-\mathbf q)^2
P_L(q)P_L(|\mathbf k-\mathbf q|),
$$



$$
2P_{13}(k)=6P_L(k)\int\frac{d^3q}{(2\pi)^3}
F_3(\mathbf k,\mathbf q,-\mathbf q)P_L(q).
$$

<a id="3/b/image-one-loop-matter-power-spectrum-diagrams-and-schematic-present-day-contributions"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-312-one-loop-matter-power.png)

**[Figure 1](#3/b/image-one-loop-matter-power-spectrum-diagrams-and-schematic-present-day-contributions). One-loop matter-power-spectrum diagrams and schematic present-day contributions**. The three required contraction topologies are P11, P22, and P13 plus P31. At low wavenumber the one-loop sum approaches the linear spectrum; the loop terms become appreciable around 0.1 inverse megaparsecs times h, and fixed-order perturbation theory eventually fails.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [effective field theory of large-scale structure](../../../large-scale-structure-of-the-universe.md#effective-field-theory-of-large-scale-structure) supplements the one-loop prediction by the leading deterministic counterterm and a stochastic term,

$$
P_{\rm EFT}(k)=P_{11}+P_{22}+2P_{13}
-2c_{\rm eff}^2k^2P_{11}(k)+P_{\rm stoch}(k)+\cdots,
$$

where the normalization scale may be absorbed into $c_{\rm eff}^2$ and mass and momentum conservation make $P_{\rm stoch}=O(k^4)$ at small $k$. The ultraviolet part of the [P13 contribution to the one-loop matter power spectrum](../../../large-scale-structure-of-the-universe.md#p13-contribution-to-the-one-loop-matter-power-spectrum) has

$$
P_{13}^{\rm UV}(k)\propto
P_L(k)\int^{\Lambda}\frac{d^3q}{(2\pi)^3}
\frac{k^2}{q^2}P_L(q)
=k^2P_L(k)\frac1{2\pi^2}
\int^{\Lambda}dq\,P_L(q).
$$

Its cutoff dependence has exactly the $k^2P_L(k)$ form of the [effective sound-speed counterterm in large-scale structure](../../../large-scale-structure-of-the-universe.md#effective-sound-speed-counterterm-in-large-scale-structure), so the running of $c_{\rm eff}^2(\Lambda)$ cancels it. The stochastic and higher-derivative counterterms similarly absorb the allowed analytic ultraviolet dependence of $P_{22}$ and higher orders.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Conservation of tracer number under the map from the [Lagrangian coordinate](../../../continuum-mechanics.md#lagrangian-coordinate) $\mathbf q$ to the Eulerian position $\mathbf x$ gives

$$
[1+\delta_g^{(E)}(\mathbf x)]d^3x
=[1+\delta_g^{(L)}(\mathbf q)]d^3q.
$$

Matter conservation gives $[1+\delta^{(E)}(\mathbf x)]d^3x=d^3q$, and hence

$$
1+\delta_g^{(E)}=(1+\delta^{(E)})(1+\delta_g^{(L)}).
$$

At linear order, $\delta_g^{(L)}=b_1^{(L)}\delta$ and therefore

$$
\delta_g^{(E)}=(1+b_1^{(L)})\delta.
$$

The [Lagrangian-to-Eulerian linear bias relation](../../../large-scale-structure-of-the-universe.md#lagrangian-to-eulerian-linear-bias-relation) is

$$
\boxed{b_1^{(E)}=1+b_1^{(L)}}.
$$

## 4

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

In the absence of [scalar anisotropic stress](../../../linear-cosmological-perturbation-theory.md#scalar-anisotropic-stress), the traceless spatial [Einstein field equations](../../../general-relativity.md#einstein-field-equations) give

$$
\boxed{\Phi=\Psi}.
$$

The photon [mass-shell condition](../../../string-theory.md#string-mass-shell-condition) $g_{\mu\nu}P^\mu P^\nu=0$, together with $p^2=g_{ij}P^iP^j$ and $\epsilon=ap$, gives to first order

$$
\boxed{P^\mu=\frac{\epsilon}{a^2}
\left[1-\Psi,(1+\Phi)\widehat p^i\right]}.
$$

Use the time component of the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation), divide it by $d\eta/d\lambda=P^0$, and substitute the stated [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol). Keeping the perturbed ratios $P^i/P^0=(1+\Phi+\Psi)\widehat p^i$ where they multiply the background $\mathcal H$ terms makes those terms cancel. Comparing the result with the total derivative of $P^0=\epsilon a^{-2}(1-\Psi)$ yields

$$
\boxed{\frac{d\ln\epsilon}{d\eta}
=\Phi'-\widehat p^i\partial_i\Psi}.
$$

The first term is the time-dependent gravitational redshift and the second is the gravitational frequency shift along the photon direction.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Write the total derivative of the [phase-space distribution function](../../../statistical-physics.md#phase-space-distribution-function) as

$$
\frac{df}{d\eta}=\frac{\partial f}{\partial\eta}
+\frac{dx^i}{d\eta}\frac{\partial f}{\partial x^i}
+\frac{d\ln\epsilon}{d\eta}\frac{\partial f}{\partial\ln\epsilon}
+\frac{d\widehat p^i}{d\eta}\frac{\partial f}{\partial\widehat p^i}.
$$

Since $a\bar T$ is constant for the background photon gas, expand the [Bose-Einstein distribution](../../../statistical-physics.md#bose-einstein-distribution) as

$$
f=\bar f(\epsilon)-\epsilon\bar f_{,\epsilon}\Theta+O(2).
$$

At first order the four terms are respectively

$$
-\epsilon\bar f_{,\epsilon}\Theta',
\qquad
-\epsilon\bar f_{,\epsilon}\widehat p^i\partial_i\Theta,
\qquad
\epsilon\bar f_{,\epsilon}
(\Phi'-\widehat p^i\partial_i\Psi),
\qquad
0.
$$

The angular-deflection velocity is already first order and multiplies the first-order angular dependence of $f$, so its contribution is second order. Thus the collisionless left-hand side of the [Free-streaming photon Boltzmann equation](../../../cosmic-microwave-background-anisotropy.md#free-streaming-photon-boltzmann-equation) is

$$
\boxed{\frac{df}{d\eta}
=-\epsilon\bar f_{,\epsilon}
\left[\Theta'+\widehat{\mathbf p}\cdot\nabla\Theta
+\widehat{\mathbf p}\cdot\nabla\Psi-\Phi'\right]}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

<a id="4/c/image-schematic-cosmic-microwave-background-temperature-power-spectrum-and-source-contributions"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-312-cmb-temperature-power.png)

**[Figure 2](#4/c/image-schematic-cosmic-microwave-background-temperature-power-spectrum-and-source-contributions). Schematic cosmic microwave background temperature power spectrum and source contributions**. The Sachs-Wolfe contribution controls the low-multipole plateau, acoustic physics produces the peaks, the Doppler contribution is phase shifted, and photon diffusion suppresses the spectrum in the high-multipole damping tail.

The conventional vertical variable is $D_\ell=\ell(\ell+1)C_\ell/(2\pi)$ in $\mu{\rm K}^2$, plotted against the dimensionless angular multipole $\ell$. The [Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-effect) supplies a nearly flat large-angle plateau for $\ell\lesssim30$. The total spectrum has its first acoustic peak near $\ell\simeq220$ with $D_\ell$ of order $5\times10^3\,\mu{\rm K}^2$, followed by further [Cosmic microwave background acoustic peaks](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-acoustic-peak); the [Doppler CMB anisotropy](../../../cosmic-microwave-background-anisotropy.md#doppler-cmb-anisotropy) is phase shifted relative to the photon-density oscillation. At $\ell\gtrsim1000$, [Cosmic microwave background diffusion damping](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-diffusion-damping) lets photons random-walk across perturbations during recombination and produces the rapidly falling damping tail.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
