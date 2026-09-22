# Paper 312

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_312.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_312.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)

## 1

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) is

$$
\ddot\varphi+3H\dot\varphi-\frac{c^2}{a^2}\nabla^2\varphi+2H^2\varphi=0.
$$

After a spatial [Fourier transform](../../../analysis.md#fourier-transform) and the change to [conformal time](../../../cosmology.md#conformal-time), $\partial_t=a^{-1}\partial_\tau$, this becomes

$$
\varphi_{\mathbf k}''+2\mathcal H\varphi_{\mathbf k}'
+(c^2k^2+2a^2H^2)\varphi_{\mathbf k}=0.
$$

For the exact [de Sitter spacetime](../../../general-relativity.md#de-sitter-spacetime) scale factor $a=-1/(H\tau)$, one has $a''/a=2a^2H^2$. Setting $u_{\mathbf k}=a\varphi_{\mathbf k}$ therefore cancels both the friction term and the effective mass term, leaving

$$
\boxed{(\partial_\tau^2+c^2k^2)(a\varphi_{\mathbf k})=0}.
$$

This is the special cancellation for a [conformally coupled scalar field](../../../quantum-field-theory.md#conformally-coupled-scalar-field).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The positive-frequency solution for $u_k=af_k$ is proportional to $e^{-ick\tau}$. Since $a=-1/(H\tau)$, its scalar-field mode function has the stated form $f_k=\mathcal N\tau e^{-ick\tau}$. The [canonical momentum](../../../classical-mechanics.md#canonical-momentum) in conformal time is $\pi=a^2\varphi'$, so the [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation) requires the [Wronskian normalization](../../../quantum-field-theory.md#wronskian-normalization)

$$
a^2(f_kf_k^{*\prime}-f_k^*f_k')=i.
$$

Substitution gives $2ick\,a^2|\mathcal N|^2\tau^2=i$. Hence, up to an irrelevant constant phase,

$$
\boxed{\mathcal N=\frac{H}{\sqrt{2ck}}},
\qquad
f_k(\tau)=\frac{H\tau}{\sqrt{2ck}}e^{-ick\tau}.
$$

The choice $e^{-ick\tau}$ is the [Bunch-Davies vacuum](../../../cosmic-inflation.md#bunch-davies-vacuum) condition at early conformal time.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Expanding the free field as

$$
\varphi_{\mathbf k}(\tau)=f_k(\tau)a_{\mathbf k}
+f_k^*(\tau)a_{-\mathbf k}^\dagger
$$

and using the vacuum [creation and annihilation operators](../../../quantum-mechanics.md#creation-and-annihilation-operators) algebra gives

$$
\boxed{
\langle\varphi_{\mathbf k}(\tau)\varphi_{\mathbf k'}(\tau)\rangle
=(2\pi)^3\delta^{(3)}(\mathbf k+\mathbf k')
\frac{H^2\tau^2}{2ck}}.
$$

**Thus the dimensional [power spectrum](../../../probability-and-statistics.md#power-spectrum) is $P_\varphi(k,\tau)=H^2\tau^2/(2ck)$. Unlike a minimally coupled massless inflationary fluctuation, this conformally coupled field decays as $a^{-1}$ and does not freeze at late time.**

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

In conformal time the interaction Hamiltonian is

$$
H_I(\eta)=-\frac{\lambda}{4!}\int d^3x\,a^4(\eta)\varphi^4(\eta,\mathbf x).
$$

The first-order [in-in formalism](../../../quantum-field-theory.md#keldysh-formalism) formula and [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) give the connected [primordial trispectrum](../../../cosmology.md#primordial-trispectrum)

$$
\begin{aligned}
\langle\varphi_{\mathbf k_1}\varphi_{\mathbf k_2}
\varphi_{\mathbf k_3}\varphi_{\mathbf k_4}\rangle_c
={}&2\lambda(2\pi)^3\delta^{(3)}\!\left(\sum_a\mathbf k_a\right)\\
&\times\operatorname{Im}\left[
\prod_{a=1}^4f_{k_a}^*(\tau)
\int_{-\infty(1-i\epsilon)}^\tau d\eta\,
a^4(\eta)\prod_{a=1}^4f_{k_a}(\eta)
\right].
\end{aligned}
$$

The factor $4!$ from the [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction) cancels the vertex factor. Writing $K=k_1+k_2+k_3+k_4$, the powers of $\eta$ cancel because $a^4\prod_af_{k_a}$ is constant apart from its phase, and the [i-epsilon prescription](../../../quantum-field-theory.md#feynman-i-epsilon-prescription) gives

$$
\int_{-\infty(1-i\epsilon)}^\tau e^{-icK\eta}\,d\eta
=\frac{i}{cK}e^{-icK\tau}.
$$

Consequently

$$
\boxed{
\langle\varphi_{\mathbf k_1}\varphi_{\mathbf k_2}
\varphi_{\mathbf k_3}\varphi_{\mathbf k_4}\rangle_c
=(2\pi)^3\delta^{(3)}\!\left(\sum_a\mathbf k_a\right)
\frac{\lambda H^4\tau^4}{8c^5K\,k_1k_2k_3k_4}}.
$$

The full four-point function also contains the three disconnected products of the free two-point function found in part c.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Constant $c$ and $\lambda$ preserve the six spatial Euclidean isometries, namely three [spatial translations](../../../general-relativity.md#spatial-translation) and three [spatial rotations](../../../general-relativity.md#spatial-rotation). They also preserve the [de Sitter dilation](../../../general-relativity.md#de-sitter-dilation) $(\tau,\mathbf x)\mapsto(s\tau,s\mathbf x)$, under which an equal-time correlator transforms covariantly together with its observation time. For generic $c\ne1$, the preferred propagation speed breaks the three [special conformal transformations](../../../general-relativity.md#special-conformal-transformation). The correlators therefore obey seven of the ten [de Sitter isometries](../../../general-relativity.md#de-sitter-isometry). When $c=1$, the action is fully de Sitter invariant and all ten are restored.

## 2

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the spatial [transverse-longitudinal decomposition](../../../quantum-field-theory.md#transverse-longitudinal-decomposition)

$$
A_0=\phi,
\qquad
A_i=A_i^V+\partial_i\chi,
\qquad
\partial_iA_i^V=0.
$$

Under the [U(1) gauge symmetry](../../../relativistic-quantum-field.md#u-1-gauge-symmetry) $A_\mu\mapsto A_\mu+\partial_\mu\epsilon$,

$$
\phi\mapsto\phi+\dot\epsilon,
\qquad
\chi\mapsto\chi+\epsilon,
\qquad
A_i^V\mapsto A_i^V.
$$

The assumption $\nabla^2\epsilon\ne0$ makes the longitudinal split unambiguous. The scalar

$$
\boxed{\Phi_A=\phi-\dot\chi}
$$

is therefore [gauge-invariant](../../../relativistic-quantum-field.md#gauge-invariance).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The electric components of the [electromagnetic field tensor](../../../electromagnetism.md#electromagnetic-field-tensor) are

$$
F_{0i}=\dot A_i^V-\partial_i\Phi_A,
$$

while $F_{ij}$ depends only on the transverse vector. The scalar-vector cross term integrates to zero because $\partial_iA_i^V=0$, so the scalar action is

$$
S_{\rm scalar}=\frac12\int dt\,d^3x\,a(\partial_i\Phi_A)^2.
$$

Varying the nondynamical scalar gives the [constraint equation in field theory](../../../quantum-field-theory.md#constraint-equation-in-field-theory)

$$
\boxed{\nabla^2\Phi_A=0}.
$$

For every nonzero Fourier momentum this fixes $\Phi_A=0$, confirming that a source-free massless vector has no propagating scalar polarization.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Applying $\epsilon=b_i(t)x^i$ to $A_\mu=0$ gives

$$
A_0=\dot b_i(t)x^i,
\qquad
A_i=b_i(t).
$$

Its field strength vanishes, so it is a [large gauge transformation](../../../relativistic-quantum-field.md#large-gauge-transformation) of the background. To arise as the zero-momentum limit of a physical transverse perturbation, $b_i(t)$ must obey the zero-momentum vector equation of motion. In the variables used in the question this is

$$
\boxed{\partial_t(a^3\dot b_i)=0},
$$

with a constant growing solution and a decaying solution proportional to $\int^t dt'/a^3(t')$. This condition makes the large gauge mode an [adiabatic mode](../../../linear-cosmological-perturbation-theory.md#adiabatic-mode) that can be continued to small nonzero momentum.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For constant $b_i$, the transformation is $\delta A_i^V=b_i$. Its [Noether charge](../../../quantum-field-theory.md#noether-charge) is therefore

$$
\boxed{Q=\int d^3x\,b_i\Pi^i
=\lim_{\mathbf q\to0}b_i\Pi^i(\mathbf q)}
$$

up to the Fourier-sign convention. Expand a transverse polarization as

$$
A_i^V(\mathbf q)=f_q a_i(\mathbf q)+f_q^*a_i^\dagger(-\mathbf q),
\qquad
\Pi_i(\mathbf q)=a^3\bigl(\dot f_q a_i(\mathbf q)
+\dot f_q^*a_i^\dagger(-\mathbf q)\bigr).
$$

Only the creation term survives on the vacuum, while $A_i^V(\mathbf q)|0\rangle=f_q^*a_i^\dagger(-\mathbf q)|0\rangle$. Hence

$$
\boxed{Q|0\rangle=\lim_{\mathbf q\to0}
\left[\frac{a^3\dot f_q^*}{f_q^*}
b^iA_i^V(\mathbf q)|0\rangle\right]}.
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Hermitian conjugation of part d gives the corresponding charge insertion on the bra. The [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity) $i\langle[Q,\mathcal O]\rangle=\langle\delta_b\mathcal O\rangle$ therefore becomes

$$
\boxed{
\lim_{\mathbf q\to0}a^3b^i\left[
\frac{\dot f_q}{f_q}\langle A_i^V(-\mathbf q)\mathcal O\rangle
-\frac{\dot f_q^*}{f_q^*}\langle\mathcal O A_i^V(\mathbf q)\rangle
\right]
=-i\langle\delta_b\mathcal O\rangle}.
$$

For a neutral operator, $\delta_b\mathcal O=0$, so the two soft limits, multiplied by their respective wavefunctional coefficients, are equal. If $\mathcal O$ is charged, the right side is nonzero. For a product of fields of charges $e_a$ at positions $\mathbf x_a$, it is proportional to $\sum_ae_a b_i x_a^i\langle\mathcal O\rangle$; in momentum space this becomes the corresponding momentum derivative. This is a soft-vector [Ward-Takahashi identity](../../../perturbative-quantum-field-theory.md#ward-identity).

## 3

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For nonzero momentum, the Fourier transform of the local [bias expansion](../../../large-scale-structure-of-the-universe.md#bias-expansion) is

$$
\delta_g(\mathbf k)=b_1\delta(\mathbf k)
+\frac{b_2}{2}\int\frac{d^3q}{(2\pi)^3}
\delta(\mathbf q)\delta(\mathbf k-\mathbf q).
$$

The subtracted variance contributes only at $\mathbf k=0$. Because $\delta$ is a [Gaussian random field](../../../stochastic-process.md#gaussian-random-field), its three-point function vanishes and its four-point function factorizes by [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem). At leading order one of the three galaxy fields supplies the quadratic term and the other two supply linear terms. The two cross-contractions cancel the factor $1/2$, giving

$$
\boxed{
\langle\delta_g(\mathbf k_1)\delta_g(\mathbf k_2)
\delta_g(\mathbf k_3)\rangle
=b_1^2b_2(2\pi)^3\delta^{(3)}\!\left(\sum_a\mathbf k_a\right)
\left[P(k_1)P(k_2)+P(k_2)P(k_3)+P(k_3)P(k_1)\right]}.
$$

**Thus even Gaussian matter fluctuations acquire a nonzero [galaxy bispectrum](../../../large-scale-structure-of-the-universe.md#galaxy-bispectrum) through [local quadratic galaxy bias](../../../large-scale-structure-of-the-universe.md#local-quadratic-galaxy-bias).**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Along the unperturbed photon path, combine the temperature and gravitational-redshift terms and use $\mathcal T'=-\Gamma$:

$$
\frac d{d\tau}(\Theta+\Psi)+\Gamma(\Theta+\Psi)
=\Phi'+\Psi'+\Gamma(\Theta_0+\Psi-\widehat{\mathbf n}\mathbin\cdot\mathbf v_e).
$$

The [integrating factor](../../../differential-equation.md#integrating-factor) is $e^{-\mathcal T}$, and $g=\Gamma e^{-\mathcal T}$. Neglecting the exponentially hidden initial boundary term gives the [Cosmic microwave background line-of-sight solution](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-line-of-sight-solution)

$$
(\Theta+\Psi)_0
=\int^{\tau_0}d\tau\,e^{-\mathcal T}(\Phi'+\Psi')
+\int^{\tau_0}d\tau\,g(\Theta_0+\Psi-\widehat{\mathbf n}\mathbin\cdot\mathbf v_e).
$$

For instantaneous recombination, $g(\tau)=\delta(\tau-\tau_{\rm dec})$, and the observer potential contributes only an unobservable monopole. Therefore

$$
\boxed{
\Theta(\tau_0,\mathbf0,\widehat{\mathbf n})
=\Theta_{0,{\rm dec}}+\Psi_{\rm dec}
-\widehat{\mathbf n}\mathbin\cdot\mathbf v_{e,{\rm dec}}
+\int_{\tau_{\rm dec}}^{\tau_0}d\tau\,(\Phi'+\Psi')}.
$$

The first two terms form the ordinary [Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-effect), the velocity term is the [Doppler CMB anisotropy](../../../cosmic-microwave-background-anisotropy.md#doppler-cmb-anisotropy) at last scattering, and the integral is the [Integrated Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#integrated-sachs-wolfe-effect) produced by evolving potentials.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Insert the [photon temperature multipole](../../../cosmic-microwave-background-anisotropy.md#photon-temperature-multipole) expansion into the Fourier-space transport equation. The [Legendre polynomial recurrence relation](../../../differential-equation.md#legendre-polynomial-recurrence-relation) turns multiplication by $\mu$ into nearest-neighbour multipole couplings, while [Orthogonality of Legendre polynomials](../../../differential-equation.md#orthogonality-of-legendre-polynomials) projects onto a fixed $\ell$. The monopole projection has no collision term because Thomson scattering conserves photon number:

$$
\boxed{\Theta_0'+k\Theta_1=\Phi'}.
$$

The dipole projection receives the electron-velocity source,

$$
\boxed{3\Theta_1'+k(\Theta_2-\Theta_0)
=k\Psi-\Gamma(3\Theta_1+v_e)}.
$$

For every $\ell\geq2$, the collision term damps the anisotropic multipole and the [photon Boltzmann hierarchy](../../../cosmic-microwave-background-anisotropy.md#photon-boltzmann-hierarchy) is

$$
\boxed{
\Theta_\ell'+\frac{k}{2\ell+1}
\left[(\ell+1)\Theta_{\ell+1}-\ell\Theta_{\ell-1}\right]
=-\Gamma\Theta_\ell}.
$$

**Thus the [Free-streaming photon Boltzmann equation](../../../cosmic-microwave-background-anisotropy.md#free-streaming-photon-boltzmann-equation) moves angular structure between neighbouring multipoles, whereas [Thomson scattering](../../../cosmic-microwave-background-anisotropy.md#thomson-scattering) suppresses all multipoles above the dipole in the [tight-coupling approximation](../../../cosmic-microwave-background-anisotropy.md#tight-coupling-approximation).**

## 4

↑ **Parent:** [Paper 312](paper-312.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The displayed kernel is the growing-mode result of [standard perturbation theory in cosmology](../../../large-scale-structure-of-the-universe.md#standard-perturbation-theory-in-cosmology). Its assumptions are a Newtonian, weak-field, subhorizon treatment of pressureless cold matter; a single-stream, irrotational velocity field; and negligible [velocity-dispersion tensor of collisionless matter](../../../large-scale-structure-of-the-universe.md#velocity-dispersion-tensor-of-collisionless-matter), so $\sigma_{ij}=0$. The background is the [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe), which makes the growing mode proportional to $a$ and permits the separated powers $a^nF_n$. The density contrast is assumed perturbatively small and the decaying solutions are discarded. [Gaussian initial conditions](../../../large-scale-structure-of-the-universe.md#gaussian-initial-conditions) are not needed to derive $F_2$, but they are needed for the loop contractions in the later parts.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For symmetrized [standard perturbation theory density kernels](../../../large-scale-structure-of-the-universe.md#standard-perturbation-theory-density-kernel), the two one-loop contractions are

$$
\boxed{P_{22}(k)=2\int\frac{d^3q}{(2\pi)^3}
\left[F_2(\mathbf q,\mathbf k-\mathbf q)\right]^2
P(q)P(|\mathbf k-\mathbf q|)},
$$

and

$$
\boxed{P_{13}(k)=3P(k)\int\frac{d^3q}{(2\pi)^3}
F_3(\mathbf k,\mathbf q,-\mathbf q)P(q)}.
$$

The factors $2$ and $3$ count the relevant [Wick contractions](../../../perturbative-quantum-field-theory.md#wick-contraction). Since the cross-correlation occurs in both orders, the [one-loop matter power spectrum](../../../large-scale-structure-of-the-universe.md#one-loop-matter-power-spectrum) is

$$
\boxed{P_{\rm 1-loop}(k)=a^2P(k)+a^4[P_{22}(k)+2P_{13}(k)].}
$$

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Put $\mathbf p=\mathbf k-\mathbf q$, $p^2=k^2-2kq\mu+q^2$, and $\mu=\widehat{\mathbf k}\mathbin\cdot\widehat{\mathbf q}$. Direct substitution into $F_2$ gives

$$
F_2(\mathbf q,\mathbf p)
=\frac{k^2[7k\mu+q(3-10\mu^2)]}{14q\,p^2}.
$$

Using $d^3q=2\pi q^2dq\,d\mu$ in part ii therefore yields

$$
\boxed{
P_{22}(k)=\int_0^\infty\frac{dq}{4\pi^2}
\int_{-1}^1d\mu\,
\frac{k^4[7k\mu+q(3-10\mu^2)]^2}
{98(k^2-2kq\mu+q^2)^2}
P(q)P\!\left(\sqrt{k^2-2kq\mu+q^2}\right)}.
$$

For $q\ll k$, $F_2(\mathbf q,\mathbf k-\mathbf q)\sim k\mu/(2q)$. Including the equal soft region $|\mathbf k-\mathbf q|\to0$ and using $\int_{-1}^1\mu^2d\mu=2/3$ gives

$$
\boxed{P_{22,{\rm IR}}(k)\longrightarrow
\frac13k^2P(k)\int\frac{dq}{2\pi^2}P(q)}.
$$

For $q\gg k$, the constant and linear hard-momentum terms cancel, displaying the [ultraviolet softness of the second-order density kernel](../../../large-scale-structure-of-the-universe.md#ultraviolet-softness-of-the-second-order-density-kernel). Since $p\sim q$,

$$
F_2\sim\frac{k^2}{14q^2}(3-10\mu^2).
$$

The angular integral $\int_{-1}^1(3-10\mu^2)^2d\mu=18$ then gives

$$
\boxed{P_{22,{\rm UV}}(k)\longrightarrow
\frac9{98}k^4\int\frac{dq}{2\pi^2}\frac{P(q)^2}{q^2}}.
$$

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

The leading infrared terms cancel in the observable sum:

$$
P_{22,{\rm IR}}+2P_{13,{\rm IR}}
=\left(\frac13-2\frac16\right)k^2P(k)
\int\frac{dq}{2\pi^2}P(q)=0.
$$

This [infrared cancellation in large-scale structure](../../../large-scale-structure-of-the-universe.md#infrared-cancellation-in-large-scale-structure) follows from the [Equivalence principle](../../../general-relativity.md#equivalence-principle): a sufficiently long-wavelength displacement translates short-scale structure without changing an equal-time power spectrum.

The ultraviolet part of $2P_{13}$ is proportional to $k^2P(k)$ and depends on the cutoff $\Lambda$. The leading deterministic [effective field theory of large-scale structure](../../../large-scale-structure-of-the-universe.md#effective-field-theory-of-large-scale-structure) counterterm has exactly this shape,

$$
\boxed{P_{\rm ct}(k)=-2a^4c_{\rm eff}^2(\Lambda)k^2P(k)}.
$$

Its cutoff-dependent part can be chosen as

$$
c_{\rm eff}^2(\Lambda)\big|_{\rm cutoff}
=-\frac{61}{630}\int^{\Lambda}\frac{dq}{2\pi^2}P(q),
$$

which cancels the stated $2P_{13,{\rm UV}}$. The $P_{22}$ ultraviolet contribution begins at $k^4$ and, when cutoff sensitive, is absorbed by higher-derivative or stochastic counterterms.

Physically, coarse graining the matter equations does not justify setting the short-scale stress $\sigma_{ij}$ to zero. Unresolved multistreaming and nonlinear motion generate an effective pressure and viscosity. Their leading derivative contribution to the Euler equation is proportional to $-c_{\rm eff}^2\nabla_i\delta$, producing the required $k^2\delta$ correction and making long-distance predictions independent of the arbitrary cutoff.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
