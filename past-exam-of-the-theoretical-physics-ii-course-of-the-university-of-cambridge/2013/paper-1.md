# Paper 1

↑ **Parent:** [2013](../2013.md)

[Original public PDF, physical pages 280–286](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1)

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
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
  - [e](#5/e)
    - [Solution](#5/e/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $\Delta=\Omega_0-\omega$ and $R(t)=e^{-i\omega tS_z/\hbar}$. Differentiating $|\Psi\rangle=R|\Psi_R\rangle$ gives the rotating-frame [Hamiltonian operator](../../quantum-system.md#hamiltonian-quantum-mechanics) $R^\dagger HR-i\hbar R^\dagger\dot R$. The [angular momentum](../../momentum.md#angular-momentum) [commutator](../../lie-algebra.md#commutator) yields $R^\dagger S_\pm R=e^{\pm i\omega t}S_\pm$, while $-i\hbar R^\dagger\dot R=-\omega S_z$. Thus the [rotating-frame Rabi Hamiltonian](../../quantum-system.md#rotating-frame-rabi-hamiltonian) is

$$
\boxed{H_R=\Delta S_z+\Omega_RS_x
=\frac\hbar2\begin{pmatrix}\Delta&\Omega_R\\\Omega_R&-\Delta\end{pmatrix}},\qquad
i\hbar\partial_t|\Psi_R\rangle=H_R|\Psi_R\rangle.
$$

This transformation is exact for the circular drive; no [rotating-wave approximation](../../quantum-mechanics.md#rotating-wave-approximation) has been used.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Define $\Omega=\sqrt{\Delta^2+\Omega_R^2}$. Squaring the two-by-two matrix gives $H_R^2=\hbar^2\Omega^2 I/4$, so

$$
\boxed{E_\pm=\pm\frac{\hbar\Omega}{2},\qquad
|\Psi_\pm(t)\rangle=e^{\mp i\Omega t/2}e^{-i\omega tS_z/\hbar}|\pm\rangle_R}.
$$

Here $|\pm\rangle_R$ is the corresponding normalized [eigenstate](../../energy-eigenvalue.md#eigenstate) at $t=0$. In the rotating frame only its [quantum phase](../../quantum-system.md#quantum-phase) changes. In the laboratory frame its [spin](../../angular-momentum-operator.md#spin) direction also rotates about $z$ at [angular velocity](../../rigid-body-dynamics.md#angular-velocity) $\omega$: $\langle\mathbf S\rangle_\pm=\pm\hbar(\Omega_R\cos\omega t,\Omega_R\sin\omega t,\Delta)/(2\Omega)$. An arbitrary initial state is the same fixed linear combination of these two solutions. If $\Omega=0$, the rotating-frame [Hamiltonian operator](../../quantum-system.md#hamiltonian-quantum-mechanics) vanishes and the entire doublet is degenerate; evolution is just $R(t)$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Take $\omega>0$ and $T=2\pi/\omega$. A full [spin one-half](../../angular-momentum-operator.md#spin-one-half) rotation gives $R(T)=-I$, an essential sign. The [cyclic phase of a spin in a rotating field](../../quantum-mechanics.md#cyclic-phase-of-a-spin-in-a-rotating-field) has factors and total [quantum phases](../../quantum-system.md#quantum-phase)

$$
\boxed{e^{i\Phi_\pm}=-e^{\mp i\pi\Omega/\omega},\qquad
\Phi_\pm=\pi\mp\frac{\pi\Omega}{\omega}\pmod{2\pi}}.
$$

To separate the adiabatic [dynamical phase](../../quantum-system.md#dynamical-phase), set $B=\sqrt{\Omega_0^2+\Omega_R^2}>0$ and $\cos\theta=\Omega_0/B$. Then $\Omega=B-\omega\cos\theta+O(\omega^2/B)$. The instantaneous laboratory energies are $\pm\hbar B/2$, so the adiabatic [dynamical phases](../../quantum-system.md#dynamical-phase) are $\mp BT/2$. Subtracting them from $\Phi_\pm$ gives

$$
\boxed{\gamma_\pm=\mp\pi(1-\cos\theta)=\mp\frac{\mathcal A}{2}\pmod{2\pi},\qquad
\mathcal A=2\pi(1-\cos\theta)}.
$$

The oriented [solid angle](../../euclidean-geometry.md#solid-angle) $\mathcal A$ is swept out by the field direction. These are the [Berry phases](../../quantum-mechanics.md#berry-phase) for the [eigenstates](../../energy-eigenvalue.md#eigenstate) parallel and antiparallel to that direction. Retaining the [spinor](../../algebra-over-a-field.md#spinor) sign makes the [quantum phase](../../quantum-system.md#quantum-phase) vanish modulo $2\pi$ when the field does not trace a nontrivial loop. The assumption $\omega\ll B$ suffices for adiabatic following; near degeneracy it must not be silently dropped.[Section 4, spinning particles in slowly changing magnetic fields](../../physics-bibliography.md#quantal-phase-factors-accompanying-adiabatic-changes-by-michael-victor-berry)

<a id="1/c/image-original-rotating-field-cone-and-convergence-of-the-exact-cyclic-phase-to-the-spin-one-half-geometric-phase"></a>
![](../../past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2013/paper-1-rotating-spin-phase.png)

**[Figure 1](#1/c/image-original-rotating-field-cone-and-convergence-of-the-exact-cyclic-phase-to-the-spin-one-half-geometric-phase). Original rotating-field cone and convergence of the exact cyclic phase to the spin-one-half geometric phase**.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [angular momentum](../../momentum.md#angular-momentum) [commutators](../../lie-algebra.md#commutator) used in the frame transformation are representation-independent. Therefore $H_R=\Delta S_z+\Omega_RS_x$ still holds. Rotating its axis onto $z$ gives $2s+1$ [eigenvalues](../../linear-operator-theory.md#eigenvalue) and exact laboratory solutions

$$
\boxed{E_\mu=\hbar\mu\Omega,\quad
|\Psi_\mu(t)\rangle=e^{-i\mu\Omega t}R(t)|\mu\rangle_R,\quad
\mu=-s,-s+1,\ldots,s}.
$$

Now $R(T)=(-1)^{2s}I$, so $e^{i\Phi_\mu}=(-1)^{2s}e^{-i\mu\Omega T}$. In the adiabatic limit the [dynamical phase](../../quantum-system.md#dynamical-phase) is $-\mu BT$ and

$$
\boxed{\gamma_\mu=-\mu\mathcal A\pmod{2\pi}}.
$$

Indeed $2\pi s+2\pi\mu\cos\theta$ and $-2\pi\mu(1-\cos\theta)$ differ by $2\pi(s+\mu)$, an integer multiple of $2\pi$. Integer [spins](../../angular-momentum-operator.md#spin) return with a positive rotation sign and half-integer [spins](../../angular-momentum-operator.md#spin) with a negative one; the [geometric phase](../../quantum-system.md#geometric-phase) need not vanish for either.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Put $T=t-t'$. [momentum](../../momentum.md) [eigenstates](../../energy-eigenvalue.md#eigenstate) evolve with [energy](../../energy.md) $p^2/(2m)$, so the retarded [momentum](../../momentum.md) kernel is $\theta(T)\delta(p-p')e^{-ip^2T/(2m\hbar)}$. Its [Fourier transform](../../fourier-transform.md) reduces to

$$
K_0=\frac{\theta(T)}{2\pi\hbar}\int dp\,
\exp\left[\frac i\hbar\left(p(x-x')-\frac{p^2T}{2m}\right)\right].
$$

Completing the square and defining the oscillatory [Gaussian integral](../../integral.md#gaussian-integral) by a convergent limiting prescription gives

$$
\boxed{K_0=\theta(T)\sqrt{\frac{m}{2\pi i\hbar T}}
\exp\left[\frac{im(x-x')^2}{2\hbar T}\right]}.
$$

For $T>0$ the [square root](../../algebra.md#square-root) has [quantum phase](../../quantum-system.md#quantum-phase) $e^{-i\pi/4}$. As $T\downarrow0$, this kernel tends to $\delta(x-x')$ in the distributional sense. Differentiating the [Heaviside step function](../../integral-transform.md#heaviside-step-function) consequently supplies the required $i\hbar\delta(T)\delta(x-x')$ source; an extra $-i/\hbar$ factor would correspond to a different Green-function convention.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For the [momentum-space propagator in a uniform force](../../quantum-system.md#momentum-space-propagator-in-a-uniform-force), the stated Fourier convention makes $x$ act on [momentum](../../momentum.md) [wavefunctions](../../wave-function.md) as $i\hbar\partial_p$. Hence

$$
\boxed{\left[i\hbar\partial_t-\frac{p^2}{2m}-i\alpha\hbar\partial_p\right]K_p
=i\hbar\delta(T)\delta(p-p')}.
$$

For $T>0$, the characteristic has $p(s)=p'-\alpha(s-t')$. Along it the amplitude acquires [quantum phase](../../quantum-system.md#quantum-phase) $-\int_{t'}^t p(s)^2ds/(2m\hbar)$. [momentum](../../momentum.md) is translated without a Jacobian, giving

$$
\boxed{K_p=\theta(T)\delta(p-p'+\alpha T)
\exp\left[\frac{i(p^3-p'^3)}{6\alpha m\hbar}\right]}.
$$

The cubic expression is evaluated on the delta-function support. There it equals $-i[p'^2T-\alpha p'T^2+\alpha^2T^3/3]/(2m\hbar)$, making both its sign and its continuous $\alpha\to0$ limit clear. The jump at $T=0$ is the identity [momentum](../../momentum.md) kernel.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use the [Dirac delta function](../../distribution-theory.md#dirac-delta-function) to set $p'=p+\alpha T$, and write $X=x-x'$. The remaining momentum-dependent [quantum phase](../../quantum-system.md#quantum-phase) is

$$
pX-\alpha Tx'-\frac{T}{2m}\left(p+\frac{\alpha T}{2}\right)^2
-\frac{\alpha^2T^3}{24m}.
$$

Shifting the integration variable by $\alpha T/2$ reduces the integral to the free [Gaussian integral](../../integral.md#gaussian-integral). Therefore

$$
\boxed{K_\alpha=\theta(T)\sqrt{\frac{m}{2\pi i\hbar T}}
\exp\left\{\frac i\hbar\left[
\frac{mX^2}{2T}-\frac{\alpha T(x+x')}{2}-\frac{\alpha^2T^3}{24m}
\right]\right\}}.
$$

The [force](../../force.md) is $-\alpha$, not $+\alpha$. Both the linear endpoint term and the cubic-time term disappear in the zero-force limit. The prefactor remains the free one.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Measure intermediate time $u$ from $t'$. The [classical path](../../quantum-field-theory.md#classical-path) with the fixed endpoints is

$$
x_c(u)=x'+\frac{X}{T}u+\frac{\alpha}{2m}u(T-u),\qquad 0\leq u\leq T.
$$

It satisfies $m\ddot x_c=-\alpha$. Direct integration of $m\dot x_c^2/2-\alpha x_c$ gives

$$
\boxed{S_c=\frac{mX^2}{2T}-\frac{\alpha T(x+x')}{2}-\frac{\alpha^2T^3}{24m}}.
$$

For an arbitrary path write $x=x_c+\eta$ with $\eta(0)=\eta(T)=0$. Integrating the cross term by parts gives $-\int(m\ddot x_c+\alpha)\eta\,du=0$. Thus $S[x]=S_c+\int m\dot\eta^2du/2$ exactly. The fluctuation [path integral](../../quantum-field-theory.md#path-integral) is the free endpoint-fixed one, so its [determinant](../../multilinear-algebra.md#determinant) supplies $\sqrt{m/(2\pi i\hbar T)}$. Multiplication by $\theta(T)e^{iS_c/\hbar}$ reproduces the previous kernel. This exact [classical-path factorization of a quadratic path integral](../../quantum-field-theory.md#classical-path-factorization-of-a-quadratic-path-integral) is possible because a linear potential introduces no additional quadratic fluctuation term.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For [elastic scattering](../../quantum-scattering.md#elastic-scattering) by a real short-range scalar potential, write $C=m/(2\pi\hbar^2)$, $\mathbf k_i=\mathbf k$ and $|\mathbf k_f|=k$. In the far field, $|\mathbf r-\mathbf r'|=r-\widehat{\mathbf r}\cdot\mathbf r'+O(r^{-1})$ and $\mathbf k_f=k\widehat{\mathbf r}$. The outgoing spherical-wave coefficient is

$$
f(\mathbf k_f,\mathbf k_i)=-C\int d^3r'\,
e^{-i\mathbf k_f\cdot\mathbf r'}V(\mathbf r')\psi_{\mathbf k_i}(\mathbf r').
$$

Substitution of the incident [plane wave](../../wave-function.md#plane-wave) inside this integral gives

$$
\boxed{f^{(1)}=-C\widetilde V(\mathbf q),\qquad
\frac{d\sigma^{(1)}}{d\Omega}=C^2|\widetilde V(\mathbf q)|^2},\qquad
\widetilde V(\mathbf q)=\int e^{-i\mathbf q\cdot\mathbf r}V(\mathbf r)\,d^3r.
$$

The incoming and outgoing [flux](../../mathematical-physics.md#flux) factors cancel because their speeds agree. Here $\mathbf q=\mathbf k_f-\mathbf k_i$ is a [wavevector](../../elasticity-physics.md#wavevector) transfer; the actual [momentum transfer](../../quantum-scattering.md#momentum-transfer) is $\hbar\mathbf q$. This distinction preserves dimensions. The approximation requires the scattered correction to the interior wave to be small, and does not in general apply to an unscreened long-range potential.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Expanding the modulus squared yields an outgoing-angle factor $e^{-i\mathbf k_f\cdot\mathbf d}$ and an incoming factor $e^{i\mathbf k_i\cdot\mathbf d}$, where $\mathbf d=\mathbf r-\mathbf r'$. Choosing a polar axis along $\mathbf d$ gives

$$
\int d\Omega_f\,e^{-ik\widehat{\mathbf k}_f\cdot\mathbf d}
=2\pi\int_{-1}^1e^{-ikdu}\,du=4\pi\frac{\sin kd}{kd}.
$$

Consequently

$$
\boxed{\sigma^{(1)}_{\rm total}=\frac{m^2}{\pi\hbar^4}
\int d^3r\,d^3r'\,V(\mathbf r)V(\mathbf r')
\frac{\sin kd}{kd}\,e^{i\mathbf k_i\cdot\mathbf d}}.
$$

The apparent $d=0$ singularity is removable: $\sin(kd)/(kd)\to1$. Exchanging $\mathbf r$ and $\mathbf r'$ cancels the imaginary part, while nonnegativity follows directly from its origin as an integral of $|f^{(1)}|^2$. A complex absorbing potential would require $V(\mathbf r')^*$ instead; the lossless [optical theorem](../../quantum-scattering.md#optical-theorem) comparison below uses real $V$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The first scattered correction to the incident wave is

$$
\psi^{(1)}(\mathbf r)=-C\int d^3r'\,
\frac{e^{ik|\mathbf r-\mathbf r'|}}{|\mathbf r-\mathbf r'|}
V(\mathbf r')e^{i\mathbf k_i\cdot\mathbf r'}.
$$

Inserting it into the amplitude gives a second, positive contribution because the two minus signs multiply:

$$
\boxed{f^{(2)}=C^2\int d^3r\,d^3r'\,
e^{-i\mathbf k_f\cdot\mathbf r}V(\mathbf r)
\frac{e^{ikd}}dV(\mathbf r')e^{i\mathbf k_i\cdot\mathbf r'}}.
$$

Thus the amplitude through second Born order is $f^{(1)}+f^{(2)}+O(V^3)$. The intervening [outgoing Green function for the three-dimensional Helmholtz equation](../../partial-differential-equation.md#outgoing-green-function-for-the-three-dimensional-helmholtz-equation) describes propagation between the two interactions; replacing it by a real standing-wave kernel would discard the imaginary part needed for [unitarity](../../vector-space.md#unitary-operator).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

In the forward direction $\mathbf k_f=\mathbf k_i$, the first Born amplitude $-C\int V$ is real. Symmetrize the second-order double integral under $\mathbf r\leftrightarrow\mathbf r'$ before taking its imaginary part. This replaces $e^{-i\mathbf k_i\cdot\mathbf d}$ by $\cos(\mathbf k_i\cdot\mathbf d)$, and gives

$$
\operatorname{Im}f^{(2)}(0)=C^2\int d^3r\,d^3r'\,
V(\mathbf r)V(\mathbf r')\frac{\sin kd}{d}
\cos(\mathbf k_i\cdot\mathbf d).
$$

The preceding total-cross-section integral equals the same real integral multiplied by $4\pi/k$. Therefore

$$
\boxed{\operatorname{Im}[f^{(1)}(0)+f^{(2)}(0)]
=\frac{k\sigma^{(1)}_{\rm total}}{4\pi}+O(V^3)}.
$$

This is the [optical theorem at second Born order](../../quantum-scattering.md#optical-theorem-at-second-born-order). Comparing only the real first-order forward amplitude with a nonzero second-order [scattering cross-section](../../quantum-scattering.md#scattering-cross-section) would mix perturbative orders. Terms of order $V^3$ require both the next amplitude order and interference in the [scattering cross-section](../../quantum-scattering.md#scattering-cross-section).

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

There is a state-assumption issue. For a [number-conserving Gaussian quantum state](../../quantum-system.md#number-conserving-gaussian-quantum-state) with no anomalous contractions, put $\psi_i=\psi(\mathbf r_i)$, $n_i=\langle\psi_i^\dagger\psi_i\rangle$ and the [one-body density matrix](../../density-matrix.md#one-body-density-matrix) $g_{ij}=\langle\psi_i^\dagger\psi_j\rangle$. [Wick's theorem](../../perturbative-quantum-field-theory.md#wick-s-theorem) pairs each creation operator with an annihilation operator. The direct pairing gives $n_1n_2$; the exchanged pairing gives $\epsilon g_{12}g_{21}$, with $\epsilon=+1$ for [bosons](../../tensor-product-of-quantum-systems.md#boson) and $-1$ for [fermions](../../tensor-product-of-quantum-systems.md#fermion). Hence

$$
\boxed{C_{12}=n_1n_2+\epsilon|g_{12}|^2}.
$$

[normal ordering](../../perturbative-quantum-field-theory.md#normal-ordering) removes the equal-position delta-function self-counting term. Fermionic occupation-number product states are [Slater determinants](../../tensor-product-of-quantum-systems.md#slater-determinant) and obey this [Wick theorem](../../perturbative-quantum-field-theory.md#wick-s-theorem). Independent thermal bosonic modes also obey it, with $N_\alpha$ understood as mean occupations.

**A bosonic Fock product state does not generally obey the asserted identity.** The [bosonic number-state corrections to Gaussian density correlations](../../perturbative-quantum-field-theory.md#bosonic-number-state-corrections-to-gaussian-density-correlations) follow from $\langle a_\alpha^{\dagger2}a_\alpha^2\rangle=N_\alpha(N_\alpha-1)$ and give

$$
\boxed{C_{12}^{\rm Fock}=n_1n_2+|g_{12}|^2
-\sum_\alpha N_\alpha(N_\alpha+1)|\varphi_\alpha(\mathbf r_1)|^2
|\varphi_\alpha(\mathbf r_2)|^2}.
$$

For one occupied mode this is $N(N-1)|\varphi_1|^2|\varphi_2|^2$, whereas the uncorrected Gaussian expression gives $2N^2|\varphi_1|^2|\varphi_2|^2$. **This counterexample disproves the asserted identity for arbitrary bosonic number-product states.** The formulas below give both the Gaussian result, with its additional state assumption, and the exact bosonic number-state alternative. The ensemble distinction is also explicit in a later primary treatment of ideal-gas correlations.[Abstract: canonical reduced density matrices versus grand-canonical Wick factorization; 2016](../../physics-bibliography.md#quantum-correlations-of-ideal-bose-and-fermi-gases-in-the-canonical-ensemble-by-kazumasa-tsutsui-and-takafumi-kita)

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Under the Gaussian assumption, $g(\mathbf r,\mathbf r)=n(\mathbf r)$, so the coincident [normally ordered density correlation](../../perturbative-quantum-field-theory.md#normally-ordered-density-correlation) is $(1+\epsilon)n(\mathbf r)^2$. For a homogeneous nonzero density $n$, the large-separation limit is $n^2$, giving

$$
\boxed{\text{bosons: }2,\qquad\text{fermions: }0}.
$$

These [coincident-point bunching factors](../../perturbative-quantum-field-theory.md#coincident-point-bunching-factors) describe enhanced bosonic coincidence and excluded same-component fermionic coincidence. More generally the density-normalized ratio $C_{12}/(n_1n_2)$ tends to one at large separation. **The unnormalized ratio printed in the paper additionally needs matching nonzero local and remote densities**; $g_{12}\to0$ alone does not ensure this. For a bosonic Fock product state, the local normalized value instead is $2-\sum_\alpha N_\alpha(N_\alpha+1)|\varphi_\alpha(\mathbf r)|^4/n(\mathbf r)^2$, and even a large-separation factorization must be checked separately.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [three-point density correlation of an ideal quantum gas](../../perturbative-quantum-field-theory.md#three-point-density-correlation-of-an-ideal-quantum-gas) follows first for a [number-conserving Gaussian quantum state](../../quantum-system.md#number-conserving-gaussian-quantum-state). There are six pairings, one for each [permutation](../../combinatorics.md#permutation) of three annihilation operators. The identity gives the product of densities; each [transposition](../../combinatorics.md#transposition-permutation) has sign $\epsilon$; both three-cycles have positive sign. Thus

$$
\boxed{\begin{aligned}
C^{(3)}_{123}={}&n_1n_2n_3
+\epsilon\left[n_1|g_{23}|^2+n_2|g_{13}|^2+n_3|g_{12}|^2\right]\\
&+g_{12}g_{23}g_{31}+g_{13}g_{32}g_{21}.
\end{aligned}}
$$

The last two terms are [complex conjugates](../../complex-analysis.md#complex-conjugate). They equal $2\operatorname{Re}(g_{12}g_{23}g_{31})$, not an additional signed pair term. This is the [permanent of a matrix](../../linear-algebra.md#permanent-mathematics) $(g_{ij})$ for [bosons](../../tensor-product-of-quantum-systems.md#boson) and its [determinant](../../multilinear-algebra.md#determinant) for [fermions](../../tensor-product-of-quantum-systems.md#fermion). [Wick's theorem](../../perturbative-quantum-field-theory.md#wick-s-theorem) supplies the six terms only with the state assumption stated in part (a).

For completeness an exact bosonic Fock-state alternative can be given without that assumption. Let $\boldsymbol\ell$ be a mode-occupation decrement with $\sum_\alpha\ell_\alpha=3$. Define $A_{\boldsymbol\ell}(1,2,3)$ as the sum of $\prod_{j=1}^3\varphi_{\alpha_j}(\mathbf r_j)$ over all distinct ordered triples having these mode multiplicities. Acting three annihilation fields on the [number state](../../quantum-harmonic-oscillator.md#number-state) leaves mutually orthogonal states for different $\boldsymbol\ell$. Therefore

$$
\boxed{C^{(3),\rm Fock}_{123}=\sum_{\boldsymbol\ell:\,\sum\ell_\alpha=3}
\left[\prod_\alpha N_\alpha^{\underline{\ell_\alpha}}\right]
|A_{\boldsymbol\ell}(1,2,3)|^2}.
$$

Here $N^{\underline\ell}=N!/(N-\ell)!$, with zero when $\ell>N$. This expression includes repeated-mode occupation corrections absent from the Gaussian permanent; for a single mode it reduces to $N(N-1)(N-2)\prod_j|\varphi(\mathbf r_j)|^2$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

At coincident points the Gaussian expression has $g_{ij}=n$. Its six contributions give

$$
C^{(3)}(\mathbf r,\mathbf r,\mathbf r)
=(1+3\epsilon+2)n^3.
$$

When all mutual separations become large and the density stays the same nonzero $n$, only $n_1n_2n_3=n^3$ remains. Consequently

$$
\boxed{\text{bosons: }6,\qquad\text{fermions: }0}.
$$

The bosonic value is $3!$ from Gaussian exchange pairings; the fermionic [determinant](../../multilinear-algebra.md#determinant) vanishes when its rows coincide. Density-normalized correlations avoid the additional homogeneity assumption. For a specified bosonic number product, part (c)'s occupation sum must replace the six-pairing formula, so neither the universal factor six nor a universal printed ratio follows from that specification alone.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Use $[a_i,a_j^\dagger]=\delta_{ij}$ and define $E_{ij}=a_i^\dagger a_j$. A direct multiplication gives

$$
[E_{ij},E_{kl}]=\delta_{jk}E_{il}-\delta_{il}E_{kj}.
$$

With $S_+=\hbar a_\uparrow^\dagger a_\downarrow$, $S_-=\hbar a_\downarrow^\dagger a_\uparrow$, this implies $[S_+,S_-]=2\hbar S_z$ and $[S_z,S_\pm]=\pm\hbar S_\pm$. Resolving the raising and lowering combinations gives

$$
\boxed{[S_i,S_j]=i\hbar\varepsilon_{ijk}S_k}.
$$

These operators realize the [Schwinger boson representation](../../quantum-mechanics.md#schwinger-boson-representation) of [angular momentum](../../momentum.md#angular-momentum). Each commutes with $\widehat N=n_\uparrow+n_\downarrow$, so fixed total occupation is an invariant subspace.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The bosonic [commutator](../../lie-algebra.md#commutator) is important in $S_+S_-=\hbar^2n_\uparrow(n_\downarrow+1)$ and $S_-S_+=\hbar^2n_\downarrow(n_\uparrow+1)$. Therefore

$$
S^2=S_z^2+\frac{S_+S_-+S_-S_+}{2}
=\frac{\hbar^2}{4}\left[(n_\uparrow+n_\downarrow)^2+2(n_\uparrow+n_\downarrow)\right].
$$

On the $N$-particle sector,

$$
\boxed{S^2=\hbar^2\frac N2\left(\frac N2+1\right),\qquad s=\frac N2}.
$$

For example $N=0,1,2$ gives [spin](../../angular-momentum-operator.md#spin) $0,\tfrac12,1$. The total [number operator](../../quantum-harmonic-oscillator.md#number-operator) can be retained in the same identity before restricting to a sector.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Total symmetry makes a component depend only on its number $n_\uparrow$ of up indices. The possible values are $0,1,\ldots,N$, giving

$$
\boxed{\dim\operatorname{Sym}^N(\mathbb C^2)=N+1=2s+1}.
$$

A normalized basis is $|n_\uparrow,N-n_\uparrow\rangle$, with $S_z$ [eigenvalue](../../linear-operator-theory.md#eigenvalue) $\hbar(n_\uparrow-N/2)$. It is precisely one spin-$N/2$ multiplet. These are independent complex amplitudes before normalization and removal of a common [quantum phase](../../quantum-system.md#quantum-phase), rather than $N+1$ independent real physical parameters.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

The defining matrix conditions are

$$
\boxed{SU(2)=\{U\in M_2(\mathbb C):U^\dagger U=I,\ \det U=1\}}.
$$

The group operation is matrix multiplication. Equivalently $U=a_0I-i\mathbf a\cdot\boldsymbol\sigma$ with real $a_0,\mathbf a$ and $a_0^2+|\mathbf a|^2=1$, so it has three real parameters and is a compact connected simply connected [Lie group](../../lie-theory.md#lie-group). Its Hermitian [spin](../../angular-momentum-operator.md#spin) generators obey the [commutator](../../lie-algebra.md#commutator) from part (a); the corresponding Lie-algebra matrices themselves are traceless and anti-Hermitian.

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

**The literal printed difference is zero**, because the same spin-index product appears twice, and zero is invariant under every transformation. The intended [SU(2)-invariant antisymmetric spinor contraction](../../topological-group.md#su-2-invariant-antisymmetric-spinor-contraction) uses opposite indices in the second term. With $\varepsilon=\begin{pmatrix}0&1\\-1&0\end{pmatrix}$, define $I=\phi^T\varepsilon\chi$. For any two-by-two matrix,

$$
U^T\varepsilon U=(\det U)\varepsilon.
$$

Thus for $U\in SU(2)$,

$$
\boxed{I'=(U\phi)^T\varepsilon(U\chi)=I}.
$$

Expanding the [determinant](../../multilinear-algebra.md#determinant) identity proves the result without complex conjugating either [spinor](../../algebra-over-a-field.md#spinor). This is the invariant alternating tensor behind the [spin singlet state](../../bell-state.md#spin-singlet-state). If the two [spinors](../../algebra-over-a-field.md#spinor) are identical, the contraction vanishes. An antisymmetric internal two-boson state also needs an antisymmetric additional degree of freedom for overall bosonic symmetry; it does not lie in the fully symmetric fixed-two-mode sector discussed above.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A constant electrostatic [energy](../../energy.md) offset is removed locally by the [quantum phase](../../quantum-system.md#quantum-phase) substitution $\psi=e^{-iV_0t/\hbar}\psi_0$, since $(i\hbar\partial_t-V_0)\psi=e^{-iV_0t/\hbar}i\hbar\partial_t\psi_0$. Therefore the two [frequency](../../wave.md#frequency) branches become

$$
\boxed{\psi=\sum_k\frac1{\sqrt{2\omega_k}}\left[
a_ke^{ikx-i(\omega_k+V_0/\hbar)t}
+b_k^\dagger e^{-ikx+i(\omega_k-V_0/\hbar)t}\right]}.
$$

The normalization uses the kinetic [frequency](../../wave.md#frequency) $\omega_k$, while the canonical [energy](../../energy.md) [eigenvalues](../../linear-operator-theory.md#eigenvalue) are $E=V_0\pm\hbar\omega_k$. The opposite-frequency branch is not obtained by replacing $\omega_k$ by the same shifted positive [frequency](../../wave.md#frequency) in both terms. A globally constant offset produces no [electric field](../../electric-field.md), whereas different offsets on opposite sides of a step cannot be removed by a single smooth [global phase](../../quantum-system.md#global-phase).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Assume a positive-energy incoming particle, $E>mc^2$, and a nonzero upward step $V_0>0$. Set $M=mc^2$ and $k=\sqrt{E^2-M^2}/(\hbar c)>0$. With the common time factor $e^{-iEt/\hbar}$ removed, take $\phi_<(x)=e^{ikx}+r e^{-ikx}$ and $\phi_>(x)=t e^{iqx}$. The right-hand wavenumber satisfies $q^2=[(E-V_0)^2-M^2]/(\hbar c)^2$; its physical branch is specified in part (c). Integrating the stationary equation across the finite step requires continuity of $\phi$ and $\phi'$, giving $1+r=t$ and $k(1-r)=qt$. Thus

$$
\boxed{r=\frac{k-q}{k+q},\qquad t=\frac{2k}{k+q}}.
$$

These are wave amplitudes, not [flux](../../mathematical-physics.md#flux) probabilities. The [Noether current of scalar electrodynamics](../../relativistic-quantum-field.md#noether-current-of-scalar-electrodynamics), in a convenient common normalization for a stationary mode, is $\rho_Q=(E-V)|\phi|^2/(mc^2)$ and $j_Q=(\hbar/m)\operatorname{Im}(\phi^*\partial_x\phi)$. For a real $q$, its charge-current ratios are $\mathcal R=|r|^2$ and $\mathcal T=(q/k)|t|^2$, with $\mathcal R+\mathcal T=1$. The same statement uses $\operatorname{Re}q$ for a decaying solution. The [electrostatic potential](../../electric-field.md#electric-potential) couples through the time derivative; it is not a Lorentz-scalar [mass](../../classical-mechanics.md#mass) shift. A zero step is recovered separately with $q=k$, $r=0$ and $t=1$.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Let $z=E-V_0+i0$. The [outgoing analytic branch of Klein-Gordon step momentum](../../wave-equation.md#outgoing-analytic-branch-of-klein-gordon-step-momentum) is

$$
\boxed{q(z)=\frac{\sqrt{z-M}\sqrt{z+M}}{\hbar c}},
$$

where each [square root](../../algebra.md#square-root) is continued from the [upper half-plane](../../complex-analysis.md#upper-half-plane-complex-analysis). It behaves as $z/(\hbar c)$ at large positive or negative real $z$. The [branch points](../../complex-analysis.md#branch-point) are $E=V_0\pm M$; replacing this product by a principal [square root](../../algebra.md#square-root) of $z^2-M^2$ can choose the wrong sign below the lower threshold.

**I.** For $E-V_0>M$, $q>0$ and both transmitted [kinetic energy](../../energy.md#kinetic-energy) and [group velocity](../../dispersion-relation.md#group-velocity) are positive. Thus $0\leq\mathcal R<1$ and $\mathcal T=4kq/(k+q)^2>0$; the transmission decreases to zero on approaching the upper threshold from above.

**II.** For $|E-V_0|<M$, write $q=i\kappa$ with $\kappa=\sqrt{M^2-(E-V_0)^2}/(\hbar c)>0$. The right wave decays, $r=(k-i\kappa)/(k+i\kappa)$ has modulus one, and $\mathcal T=0$. There is an evanescent tail but no [flux](../../mathematical-physics.md#flux) transmitted to infinity. Its reflection [quantum phase](../../quantum-system.md#quantum-phase) changes continuously between the two thresholds.

**III.** For $E-V_0<-M$, the [analytic continuation](../../holomorphic-function.md#analytic-continuation) gives $q=-Q$, where $Q=\sqrt{(E-V_0)^2-M^2}/(\hbar c)>0$. The [group velocity](../../dispersion-relation.md#group-velocity) $c^2\hbar q/(E-V_0)$ is again rightward, while the charge density and transmitted charge current are negative. Therefore

$$
\boxed{\mathcal R=\frac{(k+Q)^2}{(k-Q)^2}>1,\qquad
\mathcal T=-\frac{4kQ}{(k-Q)^2}<0,\qquad
\mathcal R+\mathcal T=1}.
$$

Choosing $q=+Q$ would describe a wavepacket arriving from the right, inconsistent with the chosen incoming channel. As the lower threshold is approached, $q\to0^-$ and $\mathcal R\to1$ from above. This [Klein-Gordon step amplification](../../wave-equation.md#klein-gordon-step-amplification) has a real denominator zero at $E=V_0/2$ when $V_0>2M$: there $Q=k$, and no finite stationary solution with unit incoming amplitude satisfies both matching equations. The resulting formal pole must not be described as an infinite single-particle [probability](../../probability-theory.md#probability). Finite switching, wavepackets and the treatment of the external source require a multiparticle analysis.[Equations 4.142–4.155: outgoing negative-momentum branch, boundary matching and charge currents](../../physics-bibliography.md#klein-paradox-for-spin-0-particles-by-douglas-m-gingrich)

<a id="6/c/image-original-outgoing-klein-gordon-momentum-branches-and-charge-current-reflection-for-a-supercritical-sharp-step"></a>
![](../../past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2013/paper-1-klein-step-branches.png)

**[Figure 2](#6/c/image-original-outgoing-klein-gordon-momentum-branches-and-charge-current-reflection-for-a-supercritical-sharp-step). Original outgoing Klein-Gordon momentum branches and charge-current reflection for a supercritical sharp step**.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

The negative-kinetic-energy branch is interpreted as an [antiparticle](../../relativistic-quantum-field.md#antiparticle) channel. In the overlap $mc^2<E<V_0-mc^2$, particles can escape to the left and oppositely charged [antiparticles](../../relativistic-quantum-field.md#antiparticle) to the right. This interval exists only when $V_0>2mc^2$. The external electrostatic source supplies the [energy](../../energy.md) for pair creation; the reflected particle [flux](../../mathematical-physics.md#flux) can exceed the incident one because the outgoing state need not contain only the incident particle.

**The conserved quantity is signed charge current, not a positive one-particle [probability](../../probability-theory.md#probability) in both regions.** Negative $\mathcal T$ denotes rightward transport of opposite charge, so it is consistent with $\mathcal R>1$ and $\mathcal R+\mathcal T=1$. A quantized charged field with particle and [antiparticle](../../relativistic-quantum-field.md#antiparticle) creation operators gives the appropriate interpretation of this [Klein paradox](../../wave-equation.md#klein-paradox). This bosonic result must not be replaced by a fermionic reflection law or interpreted as a failure of charge conservation.[Discussion after equation 4.155: pair creation and the oppositely signed transmitted current](../../physics-bibliography.md#klein-paradox-for-spin-0-particles-by-douglas-m-gingrich)

## ↑ Ancestors (12)

1. [2013](../2013.md)
2. [Past exam of the theoretical physics II course of the University of Cambridge](../../past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge.md)
3. [Theoretical Physics II course of the University of Cambridge](../../university-of-cambridge.md#theoretical-physics-ii-course-of-the-university-of-cambridge)
4. [Theoretical Physics course of the University of Cambridge](../../university-of-cambridge.md#theoretical-physics-course-of-the-university-of-cambridge)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
8. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
9. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
10. [University of Cambridge](../../university-of-cambridge.md)
11. [List of universities](../../README.md#list-of-universities)
12. [Codex Wiki](../../README.md)
