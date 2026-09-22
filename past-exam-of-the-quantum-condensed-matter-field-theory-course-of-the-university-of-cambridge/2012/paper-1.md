# Paper 1

↑ **Parent:** [2012](../2012.md)

[Original examination PDF, physical pages455–457](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=455)

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
    - [i](#1/d/i)
      - [Solution](#1/d/i/solution)
    - [ii](#1/d/ii)
      - [Solution](#1/d/ii/solution)
    - [iii](#1/d/iii)
      - [Solution](#1/d/iii/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
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
  - [e](#3/e)
    - [Solution](#3/e/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For the [Transverse-field Ising model](../../spin-model.md#transverse-field-ising-model), use dimensionless [spin one-half](../../angular-momentum-operator.md#spin-one-half) operators, so $S^x$ has eigenvalues $\pm1/2$. At zero transverse field every aligned bond contributes $-J$. The two [ground states](../../quantum-mechanics.md#ground-state) are

$$
\boxed{|X_\pm\rangle=\bigotimes_{n=1}^N|\!\pm x\rangle_n,\qquad E_0=-JN.}
$$

They span an exactly two-dimensional ground space on the finite periodic ferromagnetic chain. Any linear combination is also a ground state; parity eigenstates are the symmetric and antisymmetric combinations. Choosing one ordered product state in the thermodynamic limit is [spontaneous symmetry breaking](../../quantum-field-theory.md#spontaneous-symmetry-breaking).

For large positive field the leading term is $-2Jg\sum_nS_n^z$. Its unique minimizing state is

$$
\boxed{|Z\rangle=\bigotimes_n|\!+z\rangle_n,\qquad E_0\sim-JgN\quad(g\to\infty).}
$$

The exchange has zero first-order expectation in this state and produces virtual spin-pair fluctuations at finite g. Thus the polarized product is the limiting wavefunction, not an exact finite-field ground state. Bulk perturbation theory gives $E_0/N=-Jg-J/(4g)+O(J/g^3)$. The field-polarized phase has no twofold ordered-state degeneracy.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $n_n=c_n^\dagger c_n$ and $P_n=\prod_{m<n}(1-2n_m)$. The [Jordan–Wigner transformation](../../angular-momentum-operator.md#jordan-wigner-transformation) gives $2S_n^x=P_n(c_n+c_n^\dagger)$ and $P_{n+1}=P_n(1-2n_n)$. The [canonical anticommutation relations](../../supersymmetric-quantum-mechanics.md#canonical-anticommutation-relations) imply

$$
(c_n+c_n^\dagger)(1-2n_n)=c_n^\dagger-c_n.
$$

Consequently the [bondwise cancellation of a Jordan-Wigner string](../../angular-momentum-operator.md#bondwise-cancellation-of-a-jordan-wigner-string) yields

$$
4S_n^xS_{n+1}^x=(c_n^\dagger-c_n)(c_{n+1}^\dagger+c_{n+1}),\qquad
2S_n^z=1-2n_n.
$$

Substitution therefore gives

$$
\boxed{H=-J\sum_n\left[(c_n^\dagger-c_n)(c_{n+1}^\dagger+c_{n+1})+g(1-2n_n)\right].}
$$

The [finite-ring parity qualification of an Ising quasiparticle gap](../../spin-model.md#finite-ring-parity-qualification-of-an-ising-quasiparticle-gap) matters here. For an exact periodic spin chain, the closing bond retains total [fermion parity](../../topological-quantum-matter.md#fermion-parity). The [parity-dependent boundary condition of the Jordan-Wigner chain](../../angular-momentum-operator.md#parity-dependent-boundary-condition-of-the-jordan-wigner-chain) is $c_{N+1}=-Pc_1$, with $P=(-1)^{N_f}$. Fixing that parity determines the allowed Fourier grid, and the resulting many-body states must still have the chosen parity. Dropping this boundary issue preserves the thermodynamic energy density, but can lose a degeneracy or the correct finite-ring excitation gap. [§5.1, spin-chain fermionization and boundary sectors](../../physics-bibliography.md#physics-215c-quantum-field-theory-part-3-by-john-mcgreevy)

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

With the specified [Fourier transform](../../fourier-transform.md) convention, [normal ordering](../../perturbative-quantum-field-theory.md#normal-ordering) gives

$$
\sum_n(c_n^\dagger c_{n+1}-c_nc_{n+1}^\dagger)=2\sum_k\cos k\,c_k^\dagger c_k,
$$

where the possible constant $\sum_ke^{ik}$ vanishes on the complete lattice momentum grid. Antisymmetry of opposite-momentum pairs similarly gives

$$
\sum_nc_n^\dagger c_{n+1}^\dagger=-i\sum_k\sin k\,c_k^\dagger c_{-k}^\dagger,\qquad
\sum_nc_nc_{n+1}=i\sum_k\sin k\,c_kc_{-k}.
$$

Hence

$$
H=-JgN+2J\sum_k(g-\cos k)c_k^\dagger c_k
+iJ\sum_k\sin k\,(c_k^\dagger c_{-k}^\dagger+c_kc_{-k}).
$$

Use the [Ising-chain Nambu spinor](../../quantum-field-theory.md#ising-chain-nambu-spinor) $\Psi_k=(c_k,-ic_{-k}^\dagger)^T$. Expanding its two diagonal terms uses $c_{-k}c_{-k}^\dagger=1-c_{-k}^\dagger c_{-k}$, retaining the constant. The result is

$$
\boxed{H=J\sum_k\Psi_k^\dagger\left[(g-\cos k)\sigma_z-\sin k\,\sigma_x\right]\Psi_k.}
$$

This is a full-zone sum. Its opposite-momentum components are redundant; treating each matrix eigenvalue as an independent physical excitation would miss the factor of two in the quasiparticle energy. Self-paired momenta have zero anomalous term and are ordinary number levels.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Put $d_k=\sqrt{(g-\cos k)^2+\sin^2k}$. The matrix in the [Ising-chain Nambu spinor](../../quantum-field-theory.md#ising-chain-nambu-spinor) has eigenvalues $\pm d_k$. A canonical [Bogoliubov transformation](../../quantum-field-theory.md#bogoliubov-transformation), with paired angles satisfying $\cos\vartheta_k=(g-\cos k)/d_k$ and $\sin\vartheta_k=-\sin k/d_k$, diagonalizes it. Accounting for [full-zone fermionic Nambu energy counting](../../quantum-field-theory.md#full-zone-fermionic-nambu-energy-counting) gives

$$
\boxed{H=\sum_k\epsilon_k\left(\gamma_k^\dagger\gamma_k-\frac12\right),\qquad
\epsilon_k=2Jd_k.}
$$

Thus the bulk [Ising-chain ground-state energy](../../spin-model.md#ising-chain-ground-state-energy) is

$$
\boxed{E_0=-\frac12\sum_k\epsilon_k,\qquad
\frac{E_0}{N}\longrightarrow-\frac{J}{2\pi}\int_{-\pi}^{\pi}\sqrt{1+g^2-2g\cos k}\,dk.}
$$

Exact finite-chain states additionally obey their [fermion parity](../../topological-quantum-matter.md#fermion-parity) sector.

The [Ising-chain quasiparticle dispersion](../../spin-model.md#ising-chain-quasiparticle-dispersion) has bulk gap $2J|1-g|$, closing at the [Ising-chain quantum critical point](../../spin-model.md#ising-chain-quantum-critical-point). Finite-system parity splittings and the bulk gap are distinct scales. The three requested limits are illustrated below.

<a id="1/d/image-ising-quasiparticle-bands"></a>
![](../../past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2012/paper-1-qcm2012-ising-bands.png)

**[Figure 1](#1/d/image-ising-quasiparticle-bands). Ising quasiparticle bands**. [Source](paper-1-qcm2012-ising-bands.py).

<h4 id="1/d/i">i</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/i/solution">Solution</h5>

↑ **Parent:** [I](#1/d/i)

At g=0, $\epsilon_k=2J$ is flat. A domain wall costs 2J, but walls occur in pairs on a periodic spin ring. A single bulk quasiparticle is therefore not automatically the first physical finite-ring spin excitation.

<h4 id="1/d/ii">ii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/d/ii)

At large positive g, $\epsilon_k=2Jg-2J\cos k+O(J/g)$. The gap grows as $2J(g-1)$ while the leading bandwidth remains 4J. The field-polarized vacuum is unique.

<h4 id="1/d/iii">iii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/d/iii)

At g=1, $\epsilon_k=4J|\sin(k/2)|\sim2J|k|$. The gap closes at zero momentum and $E_0/N=-4J/\pi$. With unit lattice spacing the critical velocity is $2J/\hbar$.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The [Hellmann–Feynman theorem](../../quantum-mechanics.md#hellmann-feynman-theorem) applied to the source field normalization gives

$$
\frac{\partial E_0}{\partial g}=\left\langle\frac{\partial H}{\partial g}\right\rangle
=-2J\sum_n\langle S_n^z\rangle.
$$

Differentiating the [Ising-chain ground-state energy](../../spin-model.md#ising-chain-ground-state-energy), using $\partial_g\epsilon_k=4J^2(g-\cos k)/\epsilon_k$, therefore proves

$$
\boxed{\sum_n\langle S_n^z\rangle=\sum_k\frac{J(g-\cos k)}{\epsilon_k}.}
$$

This is the [Ising-chain field derivative and transverse polarization](../../spin-model.md#ising-chain-field-derivative-and-transverse-polarization), not its spontaneous x-order parameter. It tends to zero at g=0 and to N/2 at large positive field. The [critical transverse polarization of an Ising chain](../../spin-model.md#critical-transverse-polarization-of-an-ising-chain) is finite: in the thermodynamic critical limit this gives $\langle S^z\rangle=1/\pi$. A zero-energy isolated momentum is treated by the appropriate limiting state, rather than by assigning a value to a literal 0/0 summand.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use dimensionless [spin](../../angular-momentum-operator.md#spin) operators and nearest-neighbour exchange $J_H>0$ on a regular [bipartite graph](../../bipartite-graph.md) with N sites and [coordination number of a lattice](../../statistical-physics.md#coordination-number-of-a-lattice) z. Count each bond once and define $\gamma_{\mathbf k}=z^{-1}\sum_\delta e^{i\mathbf k\cdot\delta}$, real for the inversion-symmetric examples considered here.

For the ferromagnetic [Heisenberg model](../../angular-momentum-operator.md#heisenberg-model), $H_F=-J_H\sum_{\langle ij\rangle}\mathbf S_i\cdot\mathbf S_j$. Expanding the [Holstein–Primakoff transformation](../../angular-momentum-operator.md#holstein-primakoff-transformation) about all spins along +z gives

$$
S_i^z=S-a_i^\dagger a_i,\qquad S_i^+\simeq\sqrt{2S}\,a_i,\qquad
H_F=E_{\rm cl}+J_HS\sum_{\langle ij\rangle}(a_i^\dagger-a_j^\dagger)(a_i-a_j),
$$

up to interactions of higher order in boson density, with $E_{\rm cl}=-NzJ_HS^2/2$. The [isotropic spin-wave vacuum energy comparison](../../critical-phenomenon.md#isotropic-spin-wave-vacuum-energy-comparison) starts with this normal ordering. The [linear spin-wave approximation](../../critical-phenomenon.md#linear-spin-wave-approximation) then gives

$$
\boxed{E_F(\mathbf k)=zJ_HS(1-\gamma_{\mathbf k}),\qquad
H_F=E_{\rm cl}+\sum_{\mathbf k}E_F(\mathbf k)a_{\mathbf k}^\dagger a_{\mathbf k}.}
$$

Each [ferromagnetic magnon](../../statistical-physics.md#ferromagnetic-magnon) lowers total $S^z$ by one. The fully aligned state is an exact eigenstate and ground state; there is no harmonic vacuum depletion or added zero-point energy in this normal-ordered Hamiltonian. The global spin-rotation multiplet remains degenerate. On a hypercubic lattice of spacing a, $z=2d$ and $\gamma_{\mathbf k}=d^{-1}\sum_j\cos k_ja$, so $E_F\simeq J_HSa^2k^2$. The exact one-magnon sector agrees with this result even at finite S; interactions enter for multiple magnons.

For the [Heisenberg antiferromagnet](../../angular-momentum-operator.md#heisenberg-antiferromagnet), take $H_A=+J_H\sum_{\langle ij\rangle}\mathbf S_i\cdot\mathbf S_j$ and expand around a [Néel state](../../statistical-physics.md#neel-state). On A, $S^z=S-a^\dagger a$ and $S^+\simeq\sqrt{2S}a$; on B, $S^z=-S+b^\dagger b$ and $S^+\simeq\sqrt{2S}b^\dagger$. A bond becomes

$$
\mathbf S_i\cdot\mathbf S_j\simeq-S^2+S(a_i^\dagger a_i+b_j^\dagger b_j+a_ib_j+a_i^\dagger b_j^\dagger).
$$

With N/2 momenta in the magnetic [Brillouin zone](../../bloch-s-theorem.md#brillouin-zone),

$$
H_A=E_{\rm cl}+zJ_HS\sum_{\mathbf k\in{\rm MBZ}}\left[a_{\mathbf k}^\dagger a_{\mathbf k}+b_{\mathbf k}^\dagger b_{\mathbf k}+\gamma_{\mathbf k}(a_{\mathbf k}b_{-\mathbf k}+a_{\mathbf k}^\dagger b_{-\mathbf k}^\dagger)\right].
$$

The bosonic [Bogoliubov transformation](../../quantum-field-theory.md#bogoliubov-transformation) has $u_k^2-v_k^2=1$ and $\tanh2\theta_k=\gamma_k$. For example $a_k=u_k\alpha_k-v_k\beta_{-k}^\dagger$ and $b_{-k}=u_k\beta_{-k}-v_k\alpha_k^\dagger$. It gives two branches in this reduced zone,

$$
\boxed{E_A(\mathbf k)=zJ_HS\sqrt{1-\gamma_{\mathbf k}^2},\quad
E_{A,0}=E_{\rm cl}+\sum_{{\rm MBZ}}[E_A(\mathbf k)-zJ_HS],\quad
v_k^2=\frac12\left[\frac1{\sqrt{1-\gamma_k^2}}-1\right].}
$$

The [reduced-zone counting of bipartite spin waves](../../statistical-physics.md#reduced-zone-counting-of-bipartite-spin-waves) gives N oscillators in total, not 2N. The negative vacuum correction and [quantum depletion of Néel order](../../statistical-physics.md#quantum-depletion-of-neel-order), $\delta S=(2/N)\sum_{{\rm MBZ}}v_k^2$, distinguish the antiferromagnet from the ferromagnet. At nonzero temperature replace $v_k^2$ by $v_k^2+(u_k^2+v_k^2)n_B(E_k)$. Hypercubic small-momentum modes have $E_A\simeq2J_HSa\sqrt d\,|k|$, hence linear physical frequency $E_A/\hbar$.

Self-consistency requires depletion much smaller than S and respects the [Holstein–Primakoff occupation constraint](../../angular-momentum-operator.md#holstein-primakoff-occupation-constraint). In one dimension the antiferromagnetic vacuum depletion diverges logarithmically, invalidating ordered spin-wave theory; it does not alone prove an exact gap or its absence. At positive temperature, isotropic short-range models in d≤2 cannot sustain such magnetic order by the [Mermin-Wagner theorem](../../critical-phenomenon.md#mermin-wagner-theorem). In three dimensions the quadratic ferromagnetic modes give the low-temperature magnetization reduction proportional to $T^{3/2}$, whereas the antiferromagnetic thermal reduction scales as $T^2$. Anisotropy, fields, frustration and magnon interactions alter these conclusions. [§4.1, contrasting ferromagnetic and antiferromagnetic low-energy dynamics](../../physics-bibliography.md#physics-215c-quantum-field-theory-part-3-by-john-mcgreevy)

<a id="2/a/image-spin-wave-comparison"></a>
![](../../past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2012/paper-1-qcm2012-spin-waves.png)

**[Figure 2](#2/a/image-spin-wave-comparison). Spin-wave comparison**. [Source](paper-1-qcm2012-spin-waves.py).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Insert position resolutions between short-time evolution factors for $H=p^2/(2M)+V(q)$. Integrating the momenta gives the [path integral](../../quantum-field-theory.md#path-integral), with real-time slice factor $[M/(2\pi i\hbar\Delta t)]^{1/2}$ and weight $e^{iS[q]/\hbar}$. A real classical trajectory cannot pass through a barrier with insufficient energy, but the path integral includes nonclassical paths.

Continue $t=-is$, with s physical [imaginary time](../../perturbative-quantum-field-theory.md#imaginary-time). The damped kernel is

$$
K_E(q_f,q_i;\mathcal T)=\langle q_f|e^{-H\mathcal T/\hbar}|q_i\rangle
=\int\mathcal Dq\,e^{-S_E[q]/\hbar},\qquad
S_E=\int_0^{\mathcal T}ds\left[\frac M2\dot q^2+V(q)\right].
$$

The [Euclidean action](../../perturbative-quantum-field-theory.md#euclidean-action) saddle obeys $M\ddot q=V'(q)$: motion in the inverted potential. For degenerate minima at $\pm a$, subtract their common potential energy. A trajectory joining them with zero Euclidean energy satisfies

$$
\frac M2\dot q^2=V(q),\qquad
\boxed{S_I=\int_{-a}^{a}dq\,\sqrt{2MV(q)}.}
$$

It is an [instanton](../../quantum-field-theory.md#instanton); reversing its direction gives an [anti-instanton](../../quantum-field-theory.md#anti-instanton). Thus a crossing amplitude is nonperturbative, proportional to $e^{-S_I/\hbar}$. For the representative quartic well $V=M\omega_0^2(q^2-a^2)^2/(8a^2)$, direct integration gives

$$
q_I(s)=a\tanh\frac{\omega_0(s-s_0)}2,\qquad S_I=\frac23M\omega_0a^2.
$$

The arbitrary center $s_0$ is an [instanton translation zero mode](../../quantum-field-theory.md#instanton-translation-zero-mode). Expanding $q=q_I+\eta$ gives a [Gaussian path integral](../../quantum-field-theory.md#gaussian-path-integral) involving $L_I=-\partial_s^2+V''(q_I)/M$. Treating the zero mode as a collective coordinate rather than a zero Gaussian denominator produces the [instanton fluctuation prefactor](../../quantum-field-theory.md#instanton-fluctuation-prefactor)

$$
K=\sqrt{\frac{S_I}{2\pi\hbar}}\left[\frac{\det L_0}{\det' L_I}\right]^{1/2},\qquad
L_0=-\partial_s^2+\omega_0^2,\qquad \kappa=K e^{-S_I/\hbar}.
$$

Common endpoint regularization defines the [functional determinant](../../quantum-field-theory.md#functional-determinant) ratio; K and kappa have inverse-time units. The prime removes only the zero eigenvalue, while integrating the center supplies the total available time. Large $S_I/\hbar$ and $\kappa\ll\omega_0$ justify a [dilute instanton gas](../../quantum-field-theory.md#dilute-instanton-gas).

Multiple crossings alternate direction. Integrating n ordered centers gives $\mathcal T^n/n!$. Return paths contain even n, and transfer paths contain odd n, so their common local-well factor multiplies $\cosh(\kappa\mathcal T)$ and $\sinh(\kappa\mathcal T)$ respectively. The two lowest levels are consequently

$$
\boxed{E_\pm=E_{\rm well}\mp\hbar\kappa,\qquad
\Delta E=2\hbar K e^{-S_I/\hbar}.}
$$

The lower state is the even combination of the two localized states. Local anharmonic corrections modify $E_{\rm well}\simeq\hbar\omega_0/2$ and higher semiclassical corrections modify K. The [thermal trace as a closed Euclidean path integral](../../quantum-field-theory.md#thermal-trace-as-a-closed-euclidean-path-integral) gives $Z\simeq2e^{-\beta E_{\rm well}}\cosh(\beta\hbar\kappa)$ when higher local levels are negligible. This describes coherent level splitting in a stable well, not irreversible decay.

For a scattering barrier at energy E, the leading [WKB tunnelling exponent](../../analysis.md#wkb-tunnelling-exponent) gives an amplitude $\exp[-\int_{q_1}^{q_2}\sqrt{2M(V-E)}\,dq/\hbar]$ and a transmission probability with twice that exponent. Endpoint matching fixes prefactors. Metastable escape instead uses a [Euclidean bounce](../../quantum-field-theory.md#euclidean-bounce), with a negative fluctuation mode and a decay rate. Neither its negative mode nor the probability/amplitude factor should be transplanted into the stable double-well splitting. [Chapter2, §§2.3.2–2.3.3, printedpp.56–60: quantum-mechanical tunnelling, fluctuation determinants and repeated instanton events](../../physics-bibliography.md#gauge-theory-by-david-tong)

<a id="2/b/image-double-well-instanton"></a>
![](../../past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2012/paper-1-qcm2012-instanton.png)

**[Figure 3](#2/b/image-double-well-instanton). Double-well instanton**. [Source](paper-1-qcm2012-instanton.py).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use the reduced attractive [reduced BCS pairing Hamiltonian](../../fermi-liquid.md#reduced-bcs-pairing-hamiltonian) with volume V, $\xi_k=\varepsilon_k-\mu$ and attraction $\lambda>0$:

$$
\mathcal H=\sum_{k\sigma}\xi_kc_{k\sigma}^\dagger c_{k\sigma}-\frac\lambda V B^\dagger B,\qquad
B=\sum_kc_{-k\downarrow}c_{k\uparrow}.
$$

A specified pairing shell or an ultraviolet renormalization is part of the model. The trace is grand canonical. Insert [fermionic coherent states](../../quantum-theory.md#fermionic-coherent-state) into its time-sliced trace. The resulting [Grassmann variables](../../multilinear-algebra.md#grassmann-variable) are antiperiodic, and with inverse-energy [imaginary time](../../perturbative-quantum-field-theory.md#imaginary-time) $0\le\tau\le\beta$ the dimensionless action is

$$
\mathcal S=\int_0^\beta d\tau\left[\sum_{k\sigma}\bar\psi_{k\sigma}(\partial_\tau+\xi_k)\psi_{k\sigma}-\frac\lambda V\bar P P\right],\qquad
P=\sum_k\psi_{-k\downarrow}\psi_{k\uparrow}.
$$

This boundary condition is essential for [Fermi-Dirac statistics](../../tensor-product-of-quantum-systems.md#fermi-dirac-statistics); replacing it by a bosonic periodic trace changes the answer. A complex [Hubbard–Stratonovich transformation](../../quantum-field-theory.md#hubbard-stratonovich-transformation) uses the local identity

$$
e^{(\lambda/V)\bar P P}\propto\int d\Delta\,d\Delta^*\,
e^{-V|\Delta|^2/\lambda+\Delta\bar P+\Delta^*P},
$$

with time-slice factors understood. The pairing field renders the fermion action quadratic. For a uniform static field the independent [Nambu spinor](../../quantum-field-theory.md#nambu-spinor) block $(\psi_{k\uparrow},\bar\psi_{-k\downarrow})^T$ has

$$
\mathcal G^{-1}(k,i\omega_n)=
\begin{pmatrix}-i\omega_n+\xi_k&-\Delta\\-\Delta^*&-i\omega_n-\xi_k\end{pmatrix},\qquad
\omega_n=(2n+1)\pi/\beta,\qquad E_k=\sqrt{\xi_k^2+|\Delta|^2}.
$$

Its determinant is $-(\omega_n^2+E_k^2)$. The phase-independent determinant sign cancels under consistent reference normalization. Integrating the fermions gives the [BCS pairing-field effective action](../../fermi-liquid.md#bcs-pairing-field-effective-action), $\mathcal S_{\rm eff}=\int_0^\beta V|\Delta|^2/\lambda\,d\tau-\operatorname{Tr}\ln\mathcal G^{-1}$, with the normal-ordering/reference term retained. The [fermionic pairing-block determinant normalization](../../fermi-liquid.md#fermionic-pairing-block-determinant-normalization) uses one independent pairing block for every k; a fully doubled spin-particle-hole trace instead needs one half. The [subtracted grand potential of the reduced BCS model](../../fermi-liquid.md#subtracted-grand-potential-of-the-reduced-bcs-model) is particularly unambiguous:

$$
\Omega(\Delta)-\Omega(0)=\frac{V|\Delta|^2}{\lambda}
-\frac1\beta\sum_{kn}\ln\frac{\omega_n^2+E_k^2}{\omega_n^2+\xi_k^2}.
$$

Performing the [Matsubara frequency](../../quantum-field-theory.md#matsubara-frequency) sum yields

$$
\Omega(\Delta)=\frac{V|\Delta|^2}{\lambda}
+\sum_k(\xi_k-E_k)-\frac2\beta\sum_k\ln(1+e^{-\beta E_k}),
$$

up to a common constant. At zero gap this reduces exactly to the two-spin free-gas result. The [Matsubara derivation of the BCS saddle](../../fermi-liquid.md#matsubara-derivation-of-the-bcs-saddle) follows by differentiating with respect to $\Delta^*$ and using $\beta^{-1}\sum_n(\omega_n^2+E^2)^{-1}=\tanh(\beta E/2)/(2E)$ gives

$$
\boxed{1=\frac\lambda V\sum_k\frac{\tanh(\beta E_k/2)}{2E_k},\qquad
N=\sum_k\left[1-\frac{\xi_k}{E_k}\tanh\frac{\beta E_k}2\right].}
$$

The second equation fixes the [chemical potential](../../chemical-potential.md) at specified number. This stationary action is BCS [mean-field theory](../../statistical-physics.md#mean-field-theory), not an exact integration of pairing-field fluctuations. With constant single-spin [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) $\nu_F$ per volume and a symmetric energy cutoff $\Lambda$, weak coupling gives $\Delta(0)\simeq2\Lambda e^{-1/(\lambda\nu_F)}$ and $k_BT_c\simeq(2e^{\gamma_E}/\pi)\Lambda e^{-1/(\lambda\nu_F)}$. The zero-temperature condensation grand-potential density is $-\nu_F\Delta^2/2$ to leading weak-coupling order; using a spin-summed density would change these displayed factors. The [BCS coherence factors](../../fermi-liquid.md#bcs-coherence-factors) are $u_k^2=(1+\xi_k/E_k)/2$ and $v_k^2=(1-\xi_k/E_k)/2$, and the associated [BCS ground state](../../fermi-liquid.md#bcs-ground-state) is the normalized product of empty and occupied pair states. [Chapter11, BCS variational state, coherence factors, gap and thermal occupations](../../physics-bibliography.md#lecture-notes-for-quantum-matter-by-steven-h-simon)

Allowing a slowly varying complex pairing field generates phase stiffness and, near the transition, the [Ginzburg-Landau theory of superconductivity](../../superconductivity.md#ginzburg-landau-theory-of-superconductivity). A neutral paired system has a gapless phase sound mode; in a charged bulk superconductor electromagnetic coupling produces the [Anderson-Higgs mechanism in a superconductor](../../superconductivity.md#anderson-higgs-mechanism-in-a-superconductor) and the [Meissner effect](../../magnetic-field.md#meissner-effect). These collective fluctuations are distinct from the gapped fermionic excitations. A microscopic dynamical calculation is needed to fix collective-mode dispersion and damping; the static saddle alone does not determine them. [§§3.1–3.2, coherent-state construction; §2.3, pair-field integration and charged phase dynamics](../../physics-bibliography.md#physics-215c-quantum-field-theory-part-3-by-john-mcgreevy)

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For the untwisted [quantum rotor](../../quantum-mechanics.md#quantum-rotor), periodicity on the angle circle requires $\psi(\phi+2\pi)=\psi(\phi)$. The normalized [energy eigenstates](../../energy-eigenvalue.md#energy-eigenstate) and their [angular momentum](../../momentum.md#angular-momentum) are

$$
u_n(\phi)=\frac{e^{in\phi}}{\sqrt{2\pi}},\qquad
\ell_n=\hbar n,\qquad E_n=\frac{\hbar^2n^2}{2I},\qquad n\in\mathbb Z.
$$

Taking the [trace](../../linear-algebra.md#matrix-trace) in this orthonormal basis therefore gives

$$
\boxed{Z=\sum_{n\in\mathbb Z}\exp\left[-\frac{\beta\hbar^2n^2}{2I}\right].}
$$

The n=0 state is nondegenerate and each nonzero $|n|$ has two opposite-angular-momentum states. No flux or twisted angular boundary condition is present.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

First lift the angle to the real line. The [time-sliced configuration-space path integral](../../quantum-field-theory.md#time-sliced-configuration-space-path-integral) for a free coordinate with inertia I has kinetic action $\int dt\,I\dot\phi^2/2$. The rotor kernel sums lifted endpoints separated by $\phi_F-\phi_I+2\pi m$, because all such endpoints represent the same final angle on the circle.

Continue real time as $t=-i\hbar\tau$. Then $e^{-iHt/\hbar}=e^{-H\tau}$ and the end of the thermal interval is $\tau=\beta$, in inverse-energy units. Thus

$$
\frac{S_E}{\hbar}=\frac{I}{2\hbar^2}\int_0^\beta d\tau\,\dot\phi^2.
$$

The [trace](../../linear-algebra.md#matrix-trace) integrates the initial angle over one copy of the circle, not the whole lifted line. It yields the [rotor winding-sector path integral](../../quantum-mechanics.md#rotor-winding-sector-path-integral)

$$
\boxed{Z=\int_0^{2\pi}d\phi\sum_{m\in\mathbb Z}
\int_{\phi(0)=\phi}^{\phi(\beta)=\phi+2\pi m}\mathcal D\phi\,
\exp\left[-\frac{I}{2\hbar^2}\int_0^\beta d\tau\,\dot\phi^2\right].}
$$

The integer m is temporal [winding number](../../complex-analysis.md#winding-number), not the angular-momentum label n. Locally the measure has the free-kernel normalization $[I/(2\pi\hbar^2\Delta\tau)]^{1/2}$ per time slice. Summing topological sectors and retaining this normalization are necessary for the correct thermal trace.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

In winding sector m write the lifted path as

$$
\phi(\tau)=\phi_0+\frac{2\pi m\tau}{\beta}+\eta(\tau),\qquad \eta(0)=\eta(\beta)=0.
$$

The cross term vanishes since $\int_0^\beta\dot\eta\,d\tau=0$. The action separates into $I(2\pi m)^2/(2\hbar^2\beta)$ and the same fixed-endpoint [Gaussian path integral](../../quantum-field-theory.md#gaussian-path-integral) for every m. Neither term depends on the initial angle, so its integral supplies $2\pi$:

$$
\boxed{Z=2\pi Z_0\sum_m e^{-I(2\pi m)^2/(2\hbar^2\beta)},\qquad
Z_0=\int_{\eta(0)=\eta(\beta)=0}\mathcal D\eta\,
e^{-I\int_0^\beta\dot\eta^2d\tau/(2\hbar^2)}.}
$$

The [fixed-endpoint rotor fluctuation normalization](../../quantum-mechanics.md#fixed-endpoint-rotor-fluctuation-normalization) is

$$
\boxed{Z_0=\sqrt{\frac{I}{2\pi\hbar^2\beta}}.}
$$

It is the diagonal free-particle thermal kernel on the lifted line, or the amplitude density for a zero-displacement fluctuation bridge. It is not by itself the circle partition function or a separately countable angular zero mode. The integration over $\phi_0$ has already counted that mode. Quadraticity makes the saddle-plus-fluctuation evaluation exact.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Analytically continue the supplied free propagator using $M=I$ and $t=-i\hbar\beta$. This gives $Z_0=\sqrt{I/(2\pi\hbar^2\beta)}$ without an arbitrary measure constant.

Apply the [Poisson summation formula](../../fourier-analysis.md#poisson-summation-formula) to $h(x)=e^{-Ax^2}$, with $A=2\pi^2I/(\hbar^2\beta)$. Its [Gaussian integral](../../integral.md#gaussian-integral) is

$$
\int_{-\infty}^\infty dx\,e^{-Ax^2+2\pi inx}=\sqrt{\frac\pi A}\,e^{-\pi^2n^2/A}.
$$

The prefactors cancel exactly because $2\pi Z_0\sqrt{\pi/A}=1$. Therefore the [momentum-winding duality of the quantum rotor](../../quantum-mechanics.md#momentum-winding-duality-of-the-quantum-rotor) gives

$$
\boxed{2\pi Z_0\sum_me^{-Am^2}=\sum_ne^{-\beta\hbar^2n^2/(2I)},}
$$

in agreement with the spectrum. The [thermal winding dominance of a free rotor](../../quantum-mechanics.md#thermal-winding-dominance-of-a-free-rotor) interchanges between the two representations. At low temperature the momentum sum is dominated by n=0 and $Z\to1$. At high temperature the winding sum is dominated by m=0 and $Z\sim\sqrt{2\pi I/(\beta\hbar^2)}$, the classical angular phase-space integral. Winding and momentum labels are dual descriptions; keeping only m=0 at low temperature would be incorrect.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The [coupled quantum rotor chain](../../quantum-mechanics.md#coupled-quantum-rotor-chain) has a compact phase and conjugate integer number $n_j=\ell_j/\hbar$. Expanding the cosine gives

$$
H\simeq-NJ+\sum_j\left[\frac{\ell_j^2}{2I}+\frac J2(\phi_{j+1}-\phi_j)^2\right].
$$

In the phase-space [Euclidean path integral](../../quantum-field-theory.md#euclidean-path-integral), using inverse-energy time, each rotor has the action term $\ell_j^2/(2I)-i\ell_j\dot\phi_j/\hbar$. Completing its Gaussian square produces $I\dot\phi_j^2/(2\hbar^2)$. Equivalently, apply the short-time free-rotor kernel locally and retain winding sectors. The smooth-sector continuum limit at unit spacing is consequently

$$
\boxed{Z\simeq e^{\beta NJ}\int\mathcal D\phi\,e^{-\mathcal S},\qquad
\mathcal S=\int_0^\beta d\tau\int dx\left[\frac{I}{2\hbar^2}(\partial_\tau\phi)^2+\frac J2(\partial_x\phi)^2\right].}
$$

The overall constant is omitted when the reference bond energy is subtracted. **With the same physical J as the Hamiltonian, the printed spatial coefficient has an extra factor $1/\hbar^2$.** The [imaginary-time normalization for a coupled rotor chain](../../quantum-mechanics.md#imaginary-time-normalization-for-a-coupled-rotor-chain) requires $\hbar^2J/2$ inside a bracket with common prefactor $1/\hbar^2$. Setting $\hbar=1$ hides the discrepancy; it cannot establish the printed formula with explicit physical units.

Returning to physical time gives $I\partial_t^2\phi=J\partial_x^2\phi$. The [harmonic phase mode of a quantum rotor chain](../../quantum-mechanics.md#harmonic-phase-mode-of-a-quantum-rotor-chain) therefore has

$$
\boxed{\omega(k)=2\sqrt{J/I}\,|\sin(k/2)|\simeq c|k|,\qquad
c=\sqrt{J/I},\qquad E_k=\hbar\omega(k).}
$$

This is a gapless sound-like collective phase mode, analogous to neutral [superfluid](../../statistical-physics.md#superfluid) sound. In [rotor-chain phase-number hydrodynamics](../../quantum-mechanics.md#rotor-chain-phase-number-hydrodynamics), number fluctuations supply the compressibility and the intersite coupling supplies [phase stiffness](../../critical-phenomenon.md#phase-stiffness). The mode is a phase-density oscillation, not a free single-rotor transition. The [global phase zero mode of a finite rotor chain](../../quantum-mechanics.md#global-phase-zero-mode-of-a-finite-rotor-chain) is a compact rotor with inertia NI, which should not be counted as an independent zero-frequency oscillator.

The [compactness qualification of a harmonic rotor chain](../../quantum-mechanics.md#compactness-qualification-of-a-harmonic-rotor-chain) matters here. The smooth harmonic theory requires small neighbouring phase differences and cannot settle the entire strong-fluctuation phase diagram. In one dimension its zero-temperature phase variance grows logarithmically, so the gapless regime has algebraic phase correlations rather than a true condensate. Thermal fluctuations and compact [phase slips](../../dynamical-systems.md#phase-slip) require additional care; phase-slip proliferation can produce a gapped phase outside the Gaussian regime. [§5.2, rotor phase/number variables and limits of smooth superfluid theory](../../physics-bibliography.md#physics-215c-quantum-field-theory-part-3-by-john-mcgreevy)

## ↑ Ancestors (11)

1. [2012](../2012.md)
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
