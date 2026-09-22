# Paper 1

↑ **Parent:** [2015](../2015.md)

Original solutions covering every option, including all three essay alternatives. [Original public PDF, physical pages 724–727; dated 14 January 2015](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=724)

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
  - [f](#1/f)
    - [Solution](#1/f/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
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

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use $\hbar=1$ and $S_n^\pm=S_n^x\pm iS_n^y$. Operators on different sites commute, and expanding the two products gives $S_n^+S_{n+1}^-+S_n^-S_{n+1}^+=2(S_n^xS_{n+1}^x+S_n^yS_{n+1}^y)$. Therefore the [quantum XX chain](../../statistical-physics.md#quantum-xx-chain) has

$$
\boxed{H=-\frac J2\sum_{n=1}^N(S_n^+S_{n+1}^-+S_n^-S_{n+1}^+)-h\sum_{n=1}^NS_n^z.}
$$

Each exchange moves a reversed [spin](../../angular-momentum-operator.md#spin) between neighbours, conserving the total number of reversed [spins](../../angular-momentum-operator.md#spin). The factor of one half follows from defining $S^\pm$ without a normalizing square root.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [spin commutation relations](../../angular-momentum-operator.md#spin-commutation-relations) give $[S_{\rm tot}^z,S_n^\pm]=\pm S_n^\pm$. Using the product rule for a [commutator](../../lie-algebra.md#commutator),

$$
[S_{\rm tot}^z,S_n^+S_{n+1}^-]
=S_n^+S_{n+1}^--S_n^+S_{n+1}^-=0,
$$

and the conjugate term also vanishes. The longitudinal field commutes with every $S_n^z$, so **$[H,S_{\rm tot}^z]=0$**. The [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) is invariant under the global [spin rotation](../../angular-momentum-operator.md#spin-rotation) $U(\theta)=e^{-i\theta S_{\rm tot}^z}$: its [continuous symmetry](../../physics.md#continuous-symmetry) group is $U(1)$. Simultaneous [energy](../../energy.md) and total-magnetization [eigenstates](../../energy-eigenvalue.md#eigenstate) can be chosen, and evolution preserves each fixed-magnetization sector. Local [magnetization](../../electromagnetism.md#magnetization) can still flow between sites; generally $[H,S_n^z]\ne0$. In the [fermion](../../tensor-product-of-quantum-systems.md#fermion) [representation](../../representation-theory.md#group-representation) the conserved number will be $N_f=N/2-S_{\rm tot}^z$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use the [canonical anticommutation relations](../../supersymmetric-quantum-mechanics.md#canonical-anticommutation-relations) $\{c_n,c_m^\dagger\}=\delta_{nm}$ and $\{c_n,c_m\}=0$. In particular, $n_m=c_m^\dagger c_m$ is a [projector](../../vector-space.md#projection-linear-algebra), so $(1-2n_m)^2=1$. Define $K_n=\prod_{m<n}(1-2n_m)$. Then $K_n^\dagger=K_n$, $K_n^2=1$, and $K_n$ commutes with $c_n$ and $c_n^\dagger$. Taking the adjoint of the given raising operator gives $S_n^-=c_n^\dagger K_n$. Hence

$$
[S_n^+,S_n^-]
=K_nc_nc_n^\dagger K_n-c_n^\dagger K_n^2c_n
=c_nc_n^\dagger-c_n^\dagger c_n
=1-2n_n=2S_n^z.
$$

Also $[n_n,c_n]=-c_n$ and $[n_n,c_n^\dagger]=c_n^\dagger$ imply $[S_n^z,S_n^\pm]=\pm S_n^\pm$. For different sites, exchanging two [fermion](../../tensor-product-of-quantum-systems.md#fermion) operators contributes one minus sign and commuting an operator through the other site's parity string contributes another; their product is positive. Thus distinct [spin](../../angular-momentum-operator.md#spin) algebras commute. **The string supplies precisely the signs required for the [Jordan–Wigner transformation](../../angular-momentum-operator.md#jordan-wigner-transformation).** The [fermion](../../tensor-product-of-quantum-systems.md#fermion) vacuum corresponds to [spin](../../angular-momentum-operator.md#spin) up, while one occupied site corresponds to [spin](../../angular-momentum-operator.md#spin) down; this convention fixes subsequent signs.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For a bulk bond, $K_{n+1}=K_n(1-2n_n)$ and $c_n(1-2n_n)=-c_n$. Reordering the remaining different-site operators then gives

$$
S_n^+S_{n+1}^-=c_{n+1}^\dagger c_n,\qquad
S_n^-S_{n+1}^+=c_n^\dagger c_{n+1}\quad(n<N).
$$

The periodic [spin](../../angular-momentum-operator.md#spin) [boundary condition](../../differential-equation.md#boundary-condition) requires separate attention. Set $P=\prod_{n=1}^N(1-2n_n)=(-1)^{N_f}$. The end bond becomes $S_N^+S_1^-=-P c_1^\dagger c_N$, with the conjugate relation for its adjoint. Consequently the exact finite-ring [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) is

$$
\boxed{H=-\frac{hN}{2}+h\sum_{n=1}^Nn_n
-\frac J2\sum_{n=1}^{N-1}(c_n^\dagger c_{n+1}+c_{n+1}^\dagger c_n)
+\frac{JP}{2}(c_N^\dagger c_1+c_1^\dagger c_N).}
$$

[fermion parity](../../topological-quantum-matter.md#fermion-parity) is conserved, so diagonalize in a sector $P=\pm1$. There the end bond can be written like every other bond provided $c_{N+1}=-Pc_1$. This [parity-dependent boundary condition of the Jordan-Wigner chain](../../angular-momentum-operator.md#parity-dependent-boundary-condition-of-the-jordan-wigner-chain) is **antiperiodic for even [fermion](../../tensor-product-of-quantum-systems.md#fermion) number and periodic for odd [fermion](../../tensor-product-of-quantum-systems.md#fermion) number**. Simply assuming periodic [fermions](../../tensor-product-of-quantum-systems.md#fermion) in both sectors changes the finite-size spectrum.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

In a fixed fermion-parity sector use lattice spacing one and the unitary [discrete Fourier transform](../../discrete-fourier-transform.md)

$$
c_n=\frac1{\sqrt N}\sum_k e^{ikn}c_k,\qquad
c_k=\frac1{\sqrt N}\sum_n e^{-ikn}c_n.
$$

The allowed momenta satisfy $e^{ikN}=-P$: they are $k=2\pi(\ell+1/2)/N$ for $P=+1$ and $k=2\pi\ell/N$ for $P=-1$, with $N$ distinct values modulo $2\pi$. The hopping and number sums become $\sum_k2\cos k\,c_k^\dagger c_k$ and $\sum_kc_k^\dagger c_k$. Thus

$$
\boxed{H=E+\sum_k\epsilon_k c_k^\dagger c_k,\qquad
E=-hN/2,\qquad\epsilon_k=h-J\cos k.}
$$

Here $E$ is the [energy](../../energy.md) of the all-up [spin](../../angular-momentum-operator.md#spin) configuration, not generally the ground-state [energy](../../energy.md). The dispersion has minimum $h-J$ at $k=0$, maximum $h+J$ at $k=\pi$, and positive curvature at its minimum. Since the [fermions](../../tensor-product-of-quantum-systems.md#fermion) do not interact, each mode can be occupied zero or one [time](../../classical-mechanics.md#time-in-physics). A negative-energy occupation lowers the many-body [energy](../../energy.md), so in the [thermodynamic limit](../../statistical-physics.md#thermodynamic-limit)

$$
|\mathrm{gs}\rangle=\prod_{|k|<k_F}c_k^\dagger|0\rangle,
\qquad k_F=\arccos(h/J),\quad 0<h<J.
$$

This is a filled [Fermi sea](../../quantum-ideal-gas-statistics.md#fermi-sea) containing many [fermions](../../tensor-product-of-quantum-systems.md#fermion); it is not obtained by putting a single particle into the band minimum. For $h>J$ every mode has positive [energy](../../energy.md) and the vacuum is the [ground state](../../quantum-mechanics.md#ground-state). Its [spin](../../angular-momentum-operator.md#spin) interpretation is complete longitudinal [polarization](../../wave.md#polarization-waves). At $h=J$ the zero-momentum one-particle excitation first becomes gapless.

For an exact finite ring use [parity-consistent filling of a free-fermion band](../../topological-quantum-matter.md#parity-consistent-filling-of-a-free-fermion-band). In each [momentum](../../momentum.md) grid fill negative-energy levels, check that their particle number has the chosen parity, and if necessary toggle a mode with the smallest $|\epsilon_k|$. Compare the two sector energies. A zero-energy mode allows degenerate occupations. This restores the physical [spin](../../angular-momentum-operator.md#spin) [Hilbert space](../../hilbert-space.md) without changing the stated band.

<a id="1/e/image-original-xx-chain-dispersion-occupied-interval-and-thermodynamic-magnetization-illustrative-field-ratios"></a>
![](../../past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2015/paper-1-xx-band.png)

**[Figure 1](#1/e/image-original-xx-chain-dispersion-occupied-interval-and-thermodynamic-magnetization-illustrative-field-ratios). Original XX-chain dispersion, occupied interval and thermodynamic magnetization; illustrative field ratios**.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Because $S_{\rm tot}^z=N/2-N_f$, the exact finite-size answer is $m_N=1/2-N_f^{\rm gs}/N$, with $N_f^{\rm gs}$ determined by the parity-consistent filling above. For the thermodynamic [magnetization of the quantum XX chain](../../statistical-physics.md#magnetization-of-the-quantum-xx-chain), the occupied fraction is the [length](../../physics.md#length) of the negative-energy interval divided by the Brillouin-zone [length](../../physics.md#length):

$$
\frac{N_f}{N}\longrightarrow\frac1{2\pi}\int_{-k_F}^{k_F}dk
=\frac{k_F}{\pi}.
$$

Therefore

$$
\boxed{m_z(h)=\begin{cases}
\displaystyle\frac12-\frac1\pi\arccos(h/J)
=\frac1\pi\arcsin(h/J),&0\le h\le J,\\[3pt]
\displaystyle\frac12,&h\ge J,
\end{cases}\qquad h_c=J.}
$$

The zero-field limit has zero [magnetization](../../electromagnetism.md#magnetization) and the high-field limit has all [spins](../../angular-momentum-operator.md#spin) up. The finite-ring curve consists of [magnetization](../../electromagnetism.md#magnetization) steps approaching this continuous limit. Strictly above $h_c$ the fully polarized [ground state](../../quantum-mechanics.md#ground-state) is unique; exactly at $h_c$ a zero-energy spin-flip state can be degenerate with it. This finite-size qualification does not alter the saturation field or limiting [magnetization](../../electromagnetism.md#magnetization) density.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Holstein–Primakoff transformation](../../angular-momentum-operator.md#holstein-primakoff-transformation) converts a [spin](../../angular-momentum-operator.md#spin) algebra into bosonic operators while retaining the finite physical [spin](../../angular-momentum-operator.md#spin) [Hilbert space](../../hilbert-space.md). With $[a_n,a_m^\dagger]=\delta_{nm}$, write

$$
S_n^z=S-a_n^\dagger a_n,\qquad
S_n^+=\sqrt{2S-a_n^\dagger a_n}\,a_n,\qquad
S_n^-=a_n^\dagger\sqrt{2S-a_n^\dagger a_n}.
$$

The [Holstein–Primakoff occupation constraint](../../angular-momentum-operator.md#holstein-primakoff-occupation-constraint) is $0\le n_n\le2S$. Acting on $|n\rangle$, the raising [matrix](../../vector-space.md#matrix) element is $\sqrt{n(2S-n+1)}$ and the lowering element is $\sqrt{(n+1)(2S-n)}$. Their squared difference is $2(S-n)$, reproducing $[S^+,S^-]=2S^z$. Operator ordering inside the square roots is essential. For low [boson](../../tensor-product-of-quantum-systems.md#boson) occupation relative to $S$, expand them to obtain $S^+\simeq\sqrt{2S}\,a$ and $S^-\simeq\sqrt{2S}\,a^\dagger$. Keeping quadratic terms gives the [linear spin-wave approximation](../../critical-phenomenon.md#linear-spin-wave-approximation); higher terms describe [magnon](../../critical-phenomenon.md#magnon) interactions. Large $S$ helps control the expansion, but a low-dimensional [infrared divergence](../../quantum-field-theory.md#infrared-divergence) can invalidate it even at large finite $S$.

For the [ferromagnet](../../electromagnetism.md#ferromagnet) choose $H_F=-J\sum_n\mathbf S_n\cdot\mathbf S_{n+1}$, $J>0$, with unit lattice spacing and $\hbar=1$. Expand around the all-up state. A longitudinal bond contributes $-JS^2+JS(n_n+n_{n+1})$, and the transverse exchange contributes $-JS(a_n^\dagger a_{n+1}+a_{n+1}^\dagger a_n)$. After a [Fourier transform](../../fourier-transform.md),

$$
H_F^{(2)}=-JNS^2+\sum_k\omega_F(k)a_k^\dagger a_k,
\qquad\boxed{\omega_F(k)=2JS(1-\cos k)\simeq JS k^2.}
$$

These are [ferromagnetic magnons](../../statistical-physics.md#ferromagnetic-magnon). The polarized vacuum is an exact [ground state](../../quantum-mechanics.md#ground-state) of the full ferromagnetic [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian): every bond is in its maximum [total-spin sector](../../angular-momentum-operator.md#total-spin-sector), minimizing that bond [energy](../../energy.md). It therefore has no quantum zero-point reduction of its [magnetization](../../electromagnetism.md#magnetization). The one-magnon dispersion is also exact, although interacting many-magnon states need not be free [bosons](../../tensor-product-of-quantum-systems.md#boson). Rotating the [polarization](../../wave.md#polarization-waves) generates the maximum-total-spin ground-state multiplet. Selecting a definite direction in a thermodynamic symmetry-breaking description breaks $SU(2)$ to $U(1)$; the two transverse [spin](../../angular-momentum-operator.md#spin) components form a canonical pair, producing a single quadratic [type-B Goldstone boson](../../critical-phenomenon.md#type-b-goldstone-boson). A small aligning field gaps it by the Zeeman [energy](../../energy.md).

At nonzero [temperature](../../temperature.md) the one-dimensional [ferromagnet](../../electromagnetism.md#ferromagnet) is different: its thermal [magnon](../../critical-phenomenon.md#magnon) number contains $\int dk\,[e^{\beta JS k^2}-1]^{-1}$, with infrared behaviour $\int dk\,T/k^2$. The divergent [magnetization](../../electromagnetism.md#magnetization) reduction signals the absence of finite-temperature [long-range order](../../statistical-physics.md#long-range-order) in an infinite short-range isotropic chain, consistent with the [Mermin-Wagner theorem](../../critical-phenomenon.md#mermin-wagner-theorem). It does not disallow the polarized zero-temperature [ground states](../../quantum-mechanics.md#ground-state) just constructed.[abstract and finite-temperature theorem](../../physics-bibliography.md#absence-of-ferromagnetism-or-antiferromagnetism-in-one-or-two-dimensional-isotropic-heisenberg-models-by-n-d-mermin-and-h-wagner)

For the [antiferromagnet](../../electromagnetism.md#antiferromagnetism) use $H_{AF}=+J\sum_n\mathbf S_n\cdot\mathbf S_{n+1}$, still $J>0$, on an even bipartite chain. The classical reference state alternates up and down. Rotate one sublattice through $\pi$ so that both local quantization axes point along their reference [spins](../../angular-momentum-operator.md#spin). In unrotated physical components, to leading order $S_A^z=S-a^\dagger a$, $S_B^z=-S+b^\dagger b$, $S_A^+\simeq\sqrt{2S}\,a$ and $S_B^+\simeq\sqrt{2S}\,b^\dagger$. Choosing Fourier phases using the actual site [positions](../../classical-mechanics.md#position) gives

$$
H_{AF}^{(2)}=-JNS^2+2JS\sum_{k\in\mathrm{RBZ}}
\left[a_k^\dagger a_k+b_k^\dagger b_k+
\cos k\,(a_kb_{-k}+a_k^\dagger b_{-k}^\dagger)\right].
$$

The reduced [Brillouin zone](../../bloch-s-theorem.md#brillouin-zone) has $M=N/2$ momenta and [length](../../physics.md#length) $\pi$. The pair creation and annihilation terms express the fact that an antiparallel reference product state is not an [eigenstate](../../energy-eigenvalue.md#eigenstate). A bosonic [Bogoliubov transformation](../../quantum-field-theory.md#bogoliubov-transformation) with $u_k=\cosh\theta_k$, $v_k=\sinh\theta_k$, $\tanh2\theta_k=\cos k$ diagonalizes each two-mode block. With the sign convention $a_k=u_k\alpha_k-v_k\beta_{-k}^\dagger$ and $b_{-k}=u_k\beta_{-k}-v_k\alpha_k^\dagger$, the result is

$$
H_{AF}^{(2)}=E_{AF}^{(2)}+\sum_{k\in\mathrm{RBZ}}\omega_{AF}(k)
(\alpha_k^\dagger\alpha_k+\beta_k^\dagger\beta_k),
$$



$$
\boxed{\omega_{AF}(k)=2JS\sqrt{1-\cos^2 k}=2JS|\sin k|\simeq2JS|k|,}
\qquad E_{AF}^{(2)}=-JNS^2+\sum_{k\in\mathrm{RBZ}}[\omega_{AF}(k)-2JS].
$$

Thus the harmonic antiferromagnetic modes have linear, rather than quadratic, long-wave dispersion. In an unfolded Brillouin-zone description the same result is represented by zeros at both zero and the antiferromagnetic [wavevector](../../elasticity-physics.md#wavevector); these are not extra independent degrees of freedom beyond the two-sublattice accounting.

The Bogoliubov vacuum has no $\alpha$ or $\beta$ excitations but contains original [spin](../../angular-momentum-operator.md#spin) [bosons](../../tensor-product-of-quantum-systems.md#boson), with $v_k^2=\tfrac12(|\sin k|^{-1}-1)$. Its [staggered magnetization](../../statistical-physics.md#staggered-magnetization) is $m_s=S-M^{-1}\sum_{k\in\mathrm{RBZ}}v_k^2$. This [quantum depletion of Néel order](../../statistical-physics.md#quantum-depletion-of-neel-order) diverges logarithmically at small $k$ in one dimension. **Linear spin-wave theory therefore does not establish a stable ordered antiferromagnetic [ground state](../../quantum-mechanics.md#ground-state) for this chain.** Its nominal gapless dispersion is a result of expanding around an invalid ordered reference, not a general proof of the exact excitation spectrum. For the nearest-neighbour isotropic chain, integer-spin systems have a Haldane gap, whereas half-integer-spin systems are gapless; the spin-one-half chain in particular has fractional [spin](../../angular-momentum-operator.md#spin) excitations rather than a simple dilute gas of ordered-state [magnons](../../critical-phenomenon.md#magnon). This distinction requires physics beyond the harmonic expansion, including the topological term in the continuum theory.[pp.1153–1156, integer versus half-integer spin](../../physics-bibliography.md#nonlinear-field-theory-of-large-spin-heisenberg-antiferromagnets-semiclassically-quantized-solitons-of-the-one-dimensional-easy-axis-neel-state-by-f-duncan-m-haldane)

<a id="2/a/image-original-harmonic-chain-dispersions-the-antiferromagnetic-curve-is-a-spin-wave-approximation-not-the-exact-spectrum-for-every-spin"></a>
![](../../past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2015/paper-1-spin-wave.png)

**[Figure 2](#2/a/image-original-harmonic-chain-dispersions-the-antiferromagnetic-curve-is-a-spin-wave-approximation-not-the-exact-spectrum-for-every-spin). Original harmonic chain dispersions; the antiferromagnetic curve is a spin-wave approximation, not the exact spectrum for every spin**.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For one coordinate with [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) $H=\hat p^2/(2m)+V(\hat x)$, the propagator is $K(x_f,t_f;x_i,t_i)=\langle x_f|e^{-iHT/\hbar}|x_i\rangle$, where $T=t_f-t_i>0$. Divide $T$ into $M$ intervals $\delta t$, use the [Trotter product formula](../../numerical-analysis.md#lie-product-formula) to separate kinetic and potential evolution, and insert complete [position](../../classical-mechanics.md#position) and [momentum](../../momentum.md) bases at each slice. The [momentum](../../momentum.md) integral is Gaussian:

$$
\langle x_{j+1}|e^{-i\delta t\hat p^2/(2m\hbar)}|x_j\rangle
=\int\frac{dp_j}{2\pi\hbar}\exp\left[\frac i\hbar p_j(x_{j+1}-x_j)-\frac{i\delta t}{2m\hbar}p_j^2\right]
=\left(\frac m{2\pi i\hbar\delta t}\right)^{1/2}
 e^{im(x_{j+1}-x_j)^2/(2\hbar\delta t)}.
$$

Multiplying the short-time kernels gives the [time-sliced configuration-space path integral](../../quantum-field-theory.md#time-sliced-configuration-space-path-integral),

$$
K=\lim_{M\to\infty}\left(\frac m{2\pi i\hbar\delta t}\right)^{M/2}
\int\prod_{j=1}^{M-1}dx_j\,
\exp\left\{\frac i\hbar\sum_{j=0}^{M-1}
\left[\frac{m(x_{j+1}-x_j)^2}{2\delta t}-\delta t V(x_j)\right]\right\},
$$

with $x_0=x_i$, $x_M=x_f$. Continuum notation abbreviates this limit as $\int_{x_i}^{x_f}\mathcal D x\,e^{iS[x]/\hbar}$, where $S=\int dt\,[m\dot x^2/2-V(x)]$. The measure includes the displayed normalization; it is not an unweighted count of paths. A small damping or analytic-continuation prescription defines the oscillatory integrals. The paths contribute complex amplitudes, so alternative histories interfere before [probabilities](../../probability-theory.md#probability) are calculated. This is the central difference from a classical statistical mixture of trajectories.[pp.367–374, action phases and construction of the propagator](../../physics-bibliography.md#space-time-approach-to-non-relativistic-quantum-mechanics-by-richard-feynman)

When [actions](../../lagrangian-mechanics.md#action) vary rapidly relative to $\hbar$, [stationary phase](../../analysis.md#stationary-phase-method) selects [classical paths](../../quantum-field-theory.md#classical-path). Put $x=x_{\rm cl}+\eta$, with $\eta$ zero at the endpoints. Vanishing first variation gives $m\ddot x_{\rm cl}+V'(x_{\rm cl})=0$. The quadratic term is

$$
S[x]=S[x_{\rm cl}]+\frac12\int dt\,
\eta\left(-m\frac{d^2}{dt^2}-V''(x_{\rm cl})\right)\eta+O(\eta^3).
$$

The resulting Gaussian fluctuation [determinant](../../multilinear-algebra.md#determinant) is the [semiclassical propagator](../../quantum-system.md#semiclassical-propagator) prefactor. In one dimension, away from caustics,

$$
\boxed{K_{\rm sc}=\sum_{\rm cl}
\left(\frac{D_{\rm cl}}{2\pi i\hbar}\right)^{1/2}
\exp\left[\frac{iS_{\rm cl}}\hbar-\frac{i\pi\nu_{\rm cl}}2\right],\qquad
D_{\rm cl}=\left|-\frac{\partial^2S_{\rm cl}}{\partial x_f\partial x_i}\right|.}
$$

The branch convention makes $\nu=0$ for a direct free-particle path before any caustic. The [Maslov index](../../symplectic-geometry.md#maslov-index) tracks the phase changes as fluctuations pass through a focal singularity. In several dimensions replace the endpoint [derivative](../../calculus.md#derivative) by the [Van Vleck determinant](../../quantum-system.md#van-vleck-determinant). The approximation sums all relevant [classical paths](../../quantum-field-theory.md#classical-path); real-time [action](../../lagrangian-mechanics.md#action) need only be stationary, not a minimum. It fails in this simple form at a caustic or coalescing saddles, where a uniform approximation is needed. Quadratic [actions](../../lagrangian-mechanics.md#action) have no higher fluctuation terms, making their Gaussian evaluation exact. For example $S_{\rm cl}=m(x_f-x_i)^2/(2T)$ gives the exact free-particle kernel $\sqrt{m/(2\pi i\hbar T)}e^{iS_{\rm cl}/\hbar}$. Tunnelling involves classically forbidden regions and can be described by imaginary-time saddles rather than real classical trajectories.

Quantum [statistical mechanics](../../statistical-physics.md#statistical-mechanics) follows by [Wick rotation](../../perturbative-quantum-field-theory.md#wick-rotation) $t=-i\tau$. The imaginary-time evolution operator is $e^{-\tau H/\hbar}$, with [Euclidean action](../../perturbative-quantum-field-theory.md#euclidean-action)

$$
S_E[x]=\int_0^{\beta\hbar}d\tau\left[\frac m2(\partial_\tau x)^2+V(x)\right].
$$

Taking a [thermal trace](../../canonical-ensemble.md#thermal-trace) identifies and integrates the endpoint [positions](../../classical-mechanics.md#position):

$$
\boxed{Z=\operatorname{Tr}e^{-\beta H}
=\int dx\int_{x(0)=x}^{x(\beta\hbar)=x}\mathcal D x\,e^{-S_E[x]/\hbar}.}
$$

This [thermal trace as a closed Euclidean path integral](../../quantum-field-theory.md#thermal-trace-as-a-closed-euclidean-path-integral) explains the periodic imaginary-time direction. A density-matrix element instead retains open endpoints. For many identical particles the [trace](../../linear-algebra.md#matrix-trace) also sums over endpoint permutations, with a plus sign for [bosons](../../tensor-product-of-quantum-systems.md#boson) and permutation parity for [fermions](../../tensor-product-of-quantum-systems.md#fermion). In coherent-state language this becomes periodic bosonic fields and antiperiodic [Grassmann fields](../../quantum-field-theory.md#grassmann-field), with corresponding [Matsubara frequencies](../../quantum-field-theory.md#matsubara-frequency).

The Euclidean weight resembles a classical [Boltzmann weight](../../canonical-ensemble.md#boltzmann-factor). A time-sliced local [quantum field](../../quantum-field-theory.md#quantum-field) in $d$ spatial dimensions becomes a classical-looking field model in $d+1$ dimensions, with anisotropic couplings and extra extent $\beta\hbar$. Thus zero-temperature quantum criticality can be treated using an infinitely extended imaginary-time direction, while nonzero [temperature](../../temperature.md) imposes a finite thickness. The dynamical scaling of [time](../../classical-mechanics.md#time-in-physics) need not equal the spatial scaling: the [dynamical critical exponent](../../critical-phenomenon.md#dynamical-critical-exponent) specifies their relationship. This [quantum-to-classical imaginary-time mapping](../../quantum-field-theory.md#quantum-to-classical-imaginary-time-mapping) requires qualification when weights have signs or imaginary terms; such a [functional integral](../../quantum-field-theory.md#functional-measure) is not automatically an ordinary positive classical [probability](../../probability-theory.md#probability) [distribution](../../distribution-theory.md#distribution-mathematical-analysis). Even with a positive weight, the mapping concerns equilibrium statistics, not literal dissipative real-time trajectories. For a free particle the Euclidean kernel is a [diffusion](../../thermodynamics.md#diffusion) kernel with [diffusion](../../thermodynamics.md#diffusion) coefficient $\hbar/(2m)$, illustrating the mathematical correspondence.

The classical high-temperature limit is a further approximation, rather than simply another name for imaginary [time](../../classical-mechanics.md#time-in-physics). If quantum level spacings and exchange effects are negligible, a one-particle [partition function](../../canonical-ensemble.md#canonical-partition-function) in $d$ dimensions becomes

$$
Z_{\rm cl}\simeq\int\frac{d^dx\,d^dp}{(2\pi\hbar)^d}
 e^{-\beta[p^2/(2m)+V(x)]}.
$$

For [indistinguishable particles](../../tensor-product-of-quantum-systems.md#indistinguishable-particles) there is a factor $1/N!$ in the dilute classical gas, and exchange is negligible when the [number density](../../statistical-physics.md#number-density) [times](../../classical-mechanics.md#time-in-physics) the [thermal de Broglie wavelength](../../canonical-ensemble.md#thermal-de-broglie-wavelength) to power $d$ is small. For a [harmonic oscillator](../../classical-mechanics.md#simple-harmonic-motion), the exact quantum result $Z=[2\sinh(\beta\hbar\omega/2)]^{-1}$ tends to $1/(\beta\hbar\omega)$ as $\beta\hbar\omega\to0$, recovering the classical phase-space integral. **[stationary phase](../../analysis.md#stationary-phase-method) explains [classical mechanics](../../classical-mechanics.md); the short imaginary-time, weak-exchange limit explains classical [statistical mechanics](../../statistical-physics.md#statistical-mechanics).** These are related but distinct limits of the same quantum formulation.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Consider a conventional spin-singlet, weak-coupling, three-dimensional [superconductor](../../superconductivity.md#superconductor). Set $\hbar=k_B=1$ in the microscopic [action](../../lagrangian-mechanics.md#action) and restore electromagnetic units below. An attraction $\lambda>0$ in an [energy](../../energy.md) shell about the [Fermi surface](../../fermi-liquid.md#fermi-surface) gives a Grassmann [action](../../lagrangian-mechanics.md#action)

$$
S=\int d\tau\,d^3x\left[\sum_{\sigma=\uparrow,\downarrow}
\bar\psi_\sigma(\partial_\tau+\xi(-i\nabla))\psi_\sigma
-\lambda\bar\psi_\uparrow\bar\psi_\downarrow\psi_\downarrow\psi_\uparrow\right],
\qquad\xi_{\mathbf k}=\epsilon_{\mathbf k}-\mu.
$$

The attractive sign permits pairing even when the single-particle [Fermi gas](../../quantum-ideal-gas-statistics.md#fermi-gas) is otherwise stable. A complex [Hubbard–Stratonovich transformation](../../quantum-field-theory.md#hubbard-stratonovich-transformation) introduces a pair field $\Delta$ proportional at the saddle to $\lambda\langle\psi_\downarrow\psi_\uparrow\rangle$. The [action](../../lagrangian-mechanics.md#action) is then quadratic in [fermions](../../tensor-product-of-quantum-systems.md#fermion). Integrating them out gives the [BCS pairing-field effective action](../../fermi-liquid.md#bcs-pairing-field-effective-action)

$$
S_{\rm eff}[\Delta]=\int d\tau\,d^3x\,\frac{|\Delta|^2}{\lambda}
-\operatorname{Tr}\ln\mathcal G^{-1}[\Delta]+\text{constant}.
$$

Here the [trace](../../linear-algebra.md#matrix-trace) uses one independent [Nambu spinor](../../quantum-field-theory.md#nambu-spinor) pairing block; a fully doubled particle-hole [representation](../../representation-theory.md#group-representation) instead carries its corresponding one-half factor. At a uniform saddle the [Bogoliubov--de Gennes Hamiltonian](../../topological-quantum-matter.md#bogoliubov-de-gennes-hamiltonian) can be written as

$$
\mathcal H_{\rm BdG}(\mathbf k)=\begin{pmatrix}\xi_{\mathbf k}&\Delta\\
\Delta^*&-\xi_{\mathbf k}\end{pmatrix},\qquad
E_{\mathbf k}=\sqrt{\xi_{\mathbf k}^2+|\Delta|^2}.
$$

The negative branch describes the paired vacuum; excitations are [Bogoliubov quasiparticles](../../quantum-mechanics.md#bogoliubov-quasiparticle) mixing particles and holes. Extremizing the [effective action](../../perturbative-quantum-field-theory.md#effective-action) gives

$$
\boxed{\frac1\lambda=\int_{\rm shell}\frac{d^3k}{(2\pi)^3}
\frac{\tanh(E_{\mathbf k}/2T)}{2E_{\mathbf k}}.}
$$

The physical cutoff or a renormalized interaction is part of the microscopic model; an unregulated contact integral must not be used indiscriminately. With constant [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) $N(0)$ per [spin](../../angular-momentum-operator.md#spin) and shell half-width $\Omega_c$, the zero-temperature weak-coupling solution is $\Delta_0\simeq2\Omega_c e^{-1/[N(0)\lambda]}$. The exponentially small scale follows from the logarithmic pairing susceptibility of states near the [Fermi surface](../../fermi-liquid.md#fermi-surface). For this ideal weak-coupling model, $2\Delta_0/(k_BT_c)\simeq3.53$. The microscopic theory relates the gap, pairing and thermodynamic transition.[pp.1175–1177 and the energy-gap and finite-temperature developments](../../physics-bibliography.md#theory-of-superconductivity-by-john-bardeen-and-others)

Close to a continuous transition, for fields varying slowly compared with microscopic scales, expand the [effective action](../../perturbative-quantum-field-theory.md#effective-action) in powers and [gradients](../../multivariable-calculus.md#gradient) of $\Delta$. Its static part is the [Ginzburg-Landau theory of superconductivity](../../superconductivity.md#ginzburg-landau-theory-of-superconductivity):

$$
F=\int d^3x\left[a(T)|\Delta|^2+\frac b2|\Delta|^4+
K\left|\left(-i\nabla-\frac q\hbar\mathbf A\right)\Delta\right|^2
+\frac{|\mathbf B|^2}{2\mu_0}\right],
\qquad q=-2e,\quad b,K>0.
$$

The normalization of $\Delta$ fixes the coefficients; here $a(T)$ changes sign at $T_c$. The uniform minimum has $|\Delta_0|^2=-a/b$ for $a<0$, condensation [free-energy density](../../statistical-physics.md#free-energy-density) $-a^2/(2b)$, and characteristic coherence-length scale $\xi=\sqrt{K/|a|}$. Above the transition the minimum is at zero. The quartic stabilization and [gradient](../../multivariable-calculus.md#gradient) cost are precisely the ingredients of [Landau theory](../../critical-phenomenon.md#landau-theory) for a complex [order parameter](../../critical-phenomenon.md#order-parameter). This controlled near-transition expansion supplies a bridge between microscopic [BCS theory](../../fermi-liquid.md#bcs-theory) and macroscopic magnetic response; its coefficients and validity depend on the material and fluctuation regime.[pp.1364–1367, microscopic expansion near the transition](../../physics-bibliography.md#microscopic-derivation-of-the-ginzburg-landau-equations-in-the-theory-of-superconductivity-by-lev-gor-kov)

Write $\Delta=(|\Delta_0|+\eta)e^{i\phi}$. The radial fluctuation has positive local restoring curvature, whereas the phase has no local potential in a neutral theory with global $U(1)$ [symmetry](../../physics.md#symmetry-physics). Freezing the amplitude gives

$$
F_\phi=\frac{\rho_s}{2}\int d^3x
\left(\nabla\phi-\frac q\hbar\mathbf A\right)^2,
\qquad\rho_s=2K|\Delta_0|^2.
$$

The neutral case supports a gapless collective phase mode. In the charged case the [electromagnetic field](../../electromagnetism.md#electromagnetic-field) couples to this phase rigidity. Under $\mathbf A\mapsto\mathbf A+\nabla\chi$ and $\phi\mapsto\phi+q\chi/\hbar$, the displayed combination is invariant. Locally choosing a gauge with constant phase leaves a quadratic term in $\mathbf A$. Varying the [free energy](../../thermodynamic-potential.md#thermodynamic-free-energy) gives the transverse London current and magnetic screening scale,

$$
\mathbf j=-\frac{q^2\rho_s}{\hbar^2}\mathbf A,
\qquad\boxed{\lambda_L^{-2}=\frac{\mu_0q^2\rho_s}{\hbar^2}.}
$$

Combining this relation with static [Maxwell equations](../../maxwell-equations.md) gives exponential field penetration, the [Meissner effect](../../magnetic-field.md#meissner-effect). Single-valuedness of the pair field around a loop with negligible current gives flux in units $\Phi_0=2\pi\hbar/|q|=\pi\hbar/e$. These are gauge-invariant physical consequences of the condensate stiffness.

For the dynamics, the neutral phase and density mode is reorganized by the Coulomb interaction and the dynamical [electromagnetic field](../../electromagnetism.md#electromagnetic-field). In a bulk three-dimensional system the long-wave longitudinal mode has a plasma gap, rather than remaining the neutral sound mode. This is the [Anderson-Higgs mechanism in a superconductor](../../superconductivity.md#anderson-higgs-mechanism-in-a-superconductor): a phase coordinate becomes part of the electromagnetic collective response instead of surviving as an independent massless physical particle. Local [gauge transformations](../../electromagnetism.md#gauge-transformation) are redundancies of the description, so a literal breaking of a local redundancy is not an observable. Phase coherence, current response and magnetic screening provide the physical statements.[pp.439–442, plasma oscillations and the charged versus neutral matter spectrum](../../physics-bibliography.md#plasmons-gauge-invariance-and-mass-by-philip-warren-anderson)

A static Landau functional alone cannot determine that full dynamical spectrum. A two-dimensional film, for example, need not have the same long-wave plasma dispersion as a bulk charged system. Nor does a positive radial curvature automatically guarantee a sharp Higgs amplitude [resonance](../../dynamical-systems.md#resonance): coupling to quasiparticles and other modes can damp it. The chosen mean-field phase is also a thermodynamic symmetry-breaking description; an isolated finite system can be formulated with definite particle number. **The microscopic pairing saddle, the near-transition Landau expansion and the electromagnetic Anderson-Higgs response describe successive scales of the same superconducting state, with distinct assumptions at each step.**

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a normal-ordered bosonic [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian), insert coherent-state resolutions between short imaginary-time evolution factors. The overlaps generate $\bar\psi\partial_\tau\psi$ and the [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) symbol is obtained by replacing creation and [annihilation operators](../../quantum-harmonic-oscillator.md#annihilation-operator) by $\bar\psi$ and $\psi$. Including the [chemical potential](../../chemical-potential.md) gives, in the stated $\hbar=1$ convention,

$$
\boxed{S=\int_0^\beta d\tau\int_Vd^dr\left[
\bar\psi\left(\partial_\tau-\frac{\nabla^2}{2m}-\mu\right)\psi
+\frac g2(\bar\psi\psi)^2\right].}
$$

The [trace](../../linear-algebra.md#matrix-trace) imposes **periodic imaginary-time [boundary conditions](../../differential-equation.md#boundary-condition)**,

$$
\psi(\mathbf r,\beta)=\psi(\mathbf r,0),\qquad
\bar\psi(\mathbf r,\beta)=\bar\psi(\mathbf r,0),
$$

so bosonic [Matsubara frequencies](../../quantum-field-theory.md#matsubara-frequency) are $\omega_n=2\pi n/\beta$. The two complex coherent-state integration variables are treated independently before imposing the physical saddle contour. There is no extra zero-point ordering term: the supplied interaction is already normal ordered.

The spatial confinement is not specified beyond the volume. The uniform bulk results below use a homogeneous box with periodic spatial boundaries, or the interior of a large vessel where boundary effects can be neglected. A hard wall instead requires a vanishing field at that wall and an inhomogeneous saddle near it. Temporal periodicity follows from the [thermal trace](../../canonical-ensemble.md#thermal-trace) and does not by itself impose periodic spatial boundaries.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a uniform time-independent saddle, extremizing the [action](../../lagrangian-mechanics.md#action) gives $(-\mu+g|\psi_0|^2)\psi_0=0$. Its grand-potential density is $f(\rho)=-\mu\rho+g\rho^2/2$, with $\rho=|\psi_0|^2\ge0$. Since $g>0$, the minimum at positive density for $\mu>0$ is

$$
\boxed{\rho_0=\mu/g,\qquad
\psi_0=\sqrt{\rho_0}\,e^{i\phi_0},\qquad
f_{\min}=-\mu^2/(2g).}
$$

For $\mu\le0$ the uniform mean-field minimum is the vacuum, rather than a positive-density condensate. At fixed nonzero density in the weakly interacting condensed regime, the saddle relation sets $\mu\simeq g\rho_0$. The mean-field one-body [density matrix](../../density-matrix.md) factorizes as $\langle a^\dagger(\mathbf r)a(\mathbf r')\rangle\simeq\rho_0$, giving macroscopic occupation of the uniform mode. Depletion corrections are omitted at this stage.

The [action](../../lagrangian-mechanics.md#action) has the global particle-number [symmetry](../../physics.md#symmetry-physics) $\psi\mapsto e^{i\alpha}\psi$, $\bar\psi\mapsto e^{-i\alpha}\bar\psi$. Choosing one saddle phase breaks this $U(1)$ [symmetry](../../physics.md#symmetry-physics); the degenerate mean-field minima form the circle **$U(1)\simeq S^1$**. There is no energetic preference for a uniform value of $\phi_0$, but spatially varying phase costs [gradient energy](../../critical-phenomenon.md#gradient-energy). Consequently a neutral condensate has a gapless [Goldstone mode](../../critical-phenomenon.md#goldstone-boson) and a nonzero [phase stiffness](../../critical-phenomenon.md#phase-stiffness). The mode becomes sound once density dynamics is included. With $\hbar=1$ the [superfluid velocity](../../statistical-physics.md#superfluid-velocity) is $\nabla\phi/m$, so a single-valued field allows circulation in units $2\pi/m$ around a closed loop that avoids zeros of the amplitude. This phase coherence and rigidity are the physical content of the broken-symmetry description.

The claim is a mean-field saddle statement, not an assertion that every $d$ and [temperature](../../temperature.md) in the question supports true [long-range order](../../statistical-physics.md#long-range-order). In a finite number-conserving system $\langle a\rangle=0$; the symmetry-breaking [order parameter](../../critical-phenomenon.md#order-parameter) is defined with the [thermodynamic limit](../../statistical-physics.md#thermodynamic-limit) taken before an infinitesimal source is removed. In a homogeneous infinite short-range gas at nonzero [temperature](../../temperature.md), infrared phase fluctuations prohibit true condensation in $d\le2$. In one dimension they also destroy true condensate [long-range order](../../statistical-physics.md#long-range-order) at zero [temperature](../../temperature.md). A two-dimensional gas can nevertheless have [superfluidity](../../statistical-physics.md#superfluidity) and algebraically decaying correlations below a [Berezinskii–Kosterlitz–Thouless transition](../../critical-phenomenon.md#berezinskii-kosterlitz-thouless-transition). A finite trap can have substantial coherence without contradicting these thermodynamic statements.[abstract and pp.383–386; finite-temperature restriction](../../physics-bibliography.md#existence-of-long-range-order-in-one-and-two-dimensions-by-pierre-hohenberg)

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

On the physical density-phase contour put $\bar\psi=\sqrt\rho\,e^{-i\phi}$. Direct differentiation gives

$$
\bar\psi\partial_\tau\psi=\frac12\partial_\tau\rho+i\rho\partial_\tau\phi,
\qquad
|\nabla\psi|^2=\frac{|\nabla\rho|^2}{4\rho}+\rho|\nabla\phi|^2.
$$

Integrating the [Laplacian](../../multivariable-calculus.md#laplacian) by parts with the stated bulk boundary convention, and dropping the periodic total [derivative](../../calculus.md#derivative) of $\rho$, produces the [density-phase action of a Bose gas](../../quantum-ideal-gas-statistics.md#density-phase-action-of-a-bose-gas),

$$
S=\int d\tau\,d^dr\left[i\rho\partial_\tau\phi
+\frac{|\nabla\rho|^2}{8m\rho}+\frac\rho{2m}|\nabla\phi|^2
+\frac g2(\rho-\rho_0)^2-\frac{\mu^2}{2g}\right].
$$

Write $\rho=\rho_0+\delta\rho$ and $\phi=\phi_0+\varphi$, where $\phi_0$ is constant. To quadratic order,

$$
\boxed{S_2=\int d\tau\,d^dr\left[
\frac g2(\delta\rho)^2+i\delta\rho\partial_\tau\varphi
+\frac{|\nabla\delta\rho|^2}{8m\rho_0}
+\frac{\rho_0}{2m}|\nabla\varphi|^2\right].}
$$

The uniform static density fluctuation has positive curvature $g$. Its inverse static susceptibility at [wavevector](../../elasticity-physics.md#wavevector) $q$ is $A_q=g+q^2/(4m\rho_0)$, which remains nonzero at $q=0$. This is the sense in which the amplitude or density fluctuation is massive. The phase has no term proportional to $\varphi^2$ without [derivatives](../../calculus.md#derivative); a uniform phase [rotation](../../riemannian-geometry.md#rotation-mathematics) costs no [action](../../lagrangian-mechanics.md#action). It is the massless direction required by global $U(1)$ [symmetry](../../physics.md#symmetry-physics).

The term $i\delta\rho\partial_\tau\varphi$ shows [density-phase conjugacy](../../statistical-physics.md#density-phase-conjugacy). It is important to distinguish [static density stiffness versus an excitation gap](../../quantum-ideal-gas-statistics.md#static-density-stiffness-versus-an-excitation-gap): the density and phase do not form two independent normal-mode branches with one gapped and one gapless particle. In this nonrelativistic first-order theory they supply the conjugate variables of one positive Bogoliubov branch, derived below. The omitted cubic terms include $\delta\rho|\nabla\varphi|^2/(2m)$ and corrections from the density-gradient denominator.

There is also a background term $i\rho_0\int d\tau\,d^dr\,\partial_\tau\varphi$. It vanishes for smooth fluctuations with zero temporal winding. Periodicity of $\psi$, however, permits $\varphi(\beta)-\varphi(0)=2\pi w$. The [compact phase winding term](../../quantum-ideal-gas-statistics.md#compact-phase-winding-term) must be retained when such sectors are included; it is not generally the same constant in all sectors. The local Gaussian [phonon](../../quantum-ideal-gas-statistics.md#phonon) calculation concerns the smooth zero-winding sector and does not describe vortices or points where the density vanishes.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

At wavelengths with $q^2/(4m\rho_0)\ll g$, neglect the density-gradient term in the [quadratic density-phase action](../../quantum-ideal-gas-statistics.md#quadratic-density-phase-action). Complete the square in its remaining density terms:

$$
\frac g2(\delta\rho)^2+i\delta\rho\partial_\tau\varphi
=\frac g2\left(\delta\rho+\frac i g\partial_\tau\varphi\right)^2
+\frac1{2g}(\partial_\tau\varphi)^2.
$$

The convergent [Gaussian integral](../../integral.md#gaussian-integral) can be performed by a contour shift or by its Fourier-transform identity. Its [determinant](../../multilinear-algebra.md#determinant) is independent of $\varphi$ at this order. Combining that normalization with the saddle [action](../../lagrangian-mechanics.md#action) into a constant $S_0$ gives

$$
\boxed{Z=e^{-S_0}\int\mathcal D\varphi\,e^{-S_{\rm eff}[\varphi]},\qquad
S_{\rm eff}=\frac12\int_0^\beta d\tau\int_Vd^dr
\left[\frac{(\partial_\tau\varphi)^2}{g}+\frac{\rho_0}{m}|\nabla\varphi|^2\right].}
$$

The saddle contribution to $S_0$ is $-\beta V\mu^2/(2g)$; the additional measure-dependent constant need not be assigned an invented numerical value. The density Gaussian extends the fluctuation integration beyond its exact positivity domain, which is justified only while fluctuations around $\rho_0>0$ are small. The smooth zero-winding assumption is also required as discussed above. A constant [global phase](../../quantum-system.md#global-phase) zero mode gives a finite compact-group volume, handled separately from nonzero [phonon](../../quantum-ideal-gas-statistics.md#phonon) modes.

Fourier transforming the [Bose-gas phase-only action](../../quantum-ideal-gas-statistics.md#bose-gas-phase-only-action) gives a kernel $\omega_n^2/g+(\rho_0/m)q^2$. Analytically continuing $\omega_n\mapsto-i(\omega+i0^+)$ gives its real-frequency poles,

$$
\boxed{\omega(q)=c|q|,\qquad c=\sqrt{g\rho_0/m}.}
$$

In the present units the excitation [energy](../../energy.md) equals $\omega$. Each real Fourier coordinate is a [harmonic oscillator](../../classical-mechanics.md#simple-harmonic-motion) with inertia coefficient $1/g$ and spring coefficient $\rho_0q^2/m$, hence [frequency](../../wave.md#frequency) equal to the square root of their ratio. This is the direct relation to a quantum [harmonic chain](../../classical-mechanics.md#harmonic-chain). The mode is a gapless sound [phonon](../../quantum-ideal-gas-statistics.md#phonon); its finite speed reflects both the [compressibility](../../thermodynamics.md#compressibility) $\partial\rho/\partial\mu=1/g$ and the [phase stiffness](../../critical-phenomenon.md#phase-stiffness) $\rho_0/m$.

Retaining the density-gradient term provides a useful check. Its integration instead gives a temporal coefficient $1/A_q$, so

$$
\omega^2(q)=\frac{\rho_0 q^2}{m}\left(g+\frac{q^2}{4m\rho_0}\right)
=c^2q^2+\frac{q^4}{4m^2},
\qquad\omega(q)=\sqrt{\epsilon_q(\epsilon_q+2g\rho_0)},\quad\epsilon_q=\frac{q^2}{2m}.
$$

This is the [Bogoliubov spectrum](../../quantum-ideal-gas-statistics.md#bogoliubov-quasiparticle-dispersion). Its small-$q$ limit is the derived sound branch; at large $q$ within the contact model it crosses towards particle-like behaviour. The crossover in the squared dispersion is $q\sim2\sqrt{mg\rho_0}$, precisely the scale beyond which the discarded density [gradient](../../multivariable-calculus.md#gradient) is not small.

The same [action](../../lagrangian-mechanics.md#action) checks the dimensional restriction in the saddle analysis. At nonzero [temperature](../../temperature.md) its zero Matsubara mode gives phase fluctuations proportional to $\int d^dq/q^2$; at zero [temperature](../../temperature.md) integrating the [frequency](../../wave.md#frequency) gives $\int d^dq/|q|$. Their [infrared divergences](../../quantum-field-theory.md#infrared-divergence) invalidate uniform true [long-range order](../../statistical-physics.md#long-range-order) for $d\le2$ at nonzero [temperature](../../temperature.md) and for $d=1$ at zero [temperature](../../temperature.md). The long-wave collective description can remain useful for correlations even where a global condensate saddle is not a literal symmetry-broken state. The contact coupling here is an effective low-energy parameter; this calculation does not determine ultraviolet [renormalization](../../perturbative-quantum-field-theory.md#renormalization) or trap-specific surface modes.

<a id="3/d/image-original-dimensionless-bogoliubov-dispersion-and-its-sound-and-particle-limits"></a>
![](../../past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2015/paper-1-bose-spectrum.png)

**[Figure 3](#3/d/image-original-dimensionless-bogoliubov-dispersion-and-its-sound-and-particle-limits). Original dimensionless Bogoliubov dispersion and its sound and particle limits**.

## ↑ Ancestors (11)

1. [2015](../2015.md)
2. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
3. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../university-of-cambridge.md#quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge)
4. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
