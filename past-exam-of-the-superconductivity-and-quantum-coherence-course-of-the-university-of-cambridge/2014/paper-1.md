# Paper 1

↑ **Parent:** [2014](../2014.md)

Original public paper: [Physical PDF pages 687–688](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=687). All five optional notes and both longer questions are covered. The density plot uses the prescribed fixed-coupling model, with its low-density limitations stated.

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
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A neutral [superfluid](../../statistical-physics.md#superfluid) can select a phase of its complex [order parameter](../../critical-phenomenon.md#order-parameter), breaking a global $U(1)$ symmetry. A spatially uniform change of that phase costs no [energy](../../energy.md). Slowly varying changes therefore produce a gapless [Goldstone mode](../../critical-phenomenon.md#goldstone-boson). For a dilute weakly repulsive [Bose gas](../../quantum-ideal-gas-statistics.md#bose-gas), the [Bogoliubov quasiparticle dispersion](../../quantum-ideal-gas-statistics.md#bogoliubov-quasiparticle-dispersion) is

$$
E_k=\sqrt{\epsilon_k(\epsilon_k+2g_Bn_0)},\qquad
\epsilon_k=\frac{\hbar^2k^2}{2m_B},
$$

so $E_k\simeq\hbar c_sk$ at long wavelengths, with $c_s=\sqrt{g_Bn_0/m_B}$. Density and phase fluctuations are canonically coupled components of this sound branch, rather than two independent positive-frequency modes. Superfluid helium and dilute atomic condensates supply neutral examples, although the dilute-gas formula is not quantitatively valid for strongly interacting liquid helium.

In a [superconductor](../../superconductivity.md#superconductor), the pair field is charged and its phase couples to the electromagnetic [gauge field](../../relativistic-quantum-field.md#gauge-field). Only combinations such as $\nabla\theta-q\mathbf A/\hbar$ are physically meaningful. The [Anderson-Higgs mechanism in a superconductor](../../superconductivity.md#anderson-higgs-mechanism-in-a-superconductor) produces electromagnetic screening and removes the neutral sound mode as an independent gapless charged-density oscillation. In a homogeneous three-dimensional continuum, long-range Coulomb [forces](../../force.md) give a longitudinal plasma gap, approximately $\omega^2=\omega_p^2+c_s^2k^2$ at small $k$. The static transverse response gives the [Meissner effect](../../magnetic-field.md#meissner-effect) and

$$
\lambda_L^{-2}=\mu_0\frac{n_se^2}{m},
$$

when $n_s$ counts superconducting [electrons](../../physics.md#electron) of effective [mass](../../classical-mechanics.md#mass) $m$. Counting pairs instead uses density $n_s/2$, charge $-2e$ and [mass](../../classical-mechanics.md#mass) $2m$, giving the same stiffness. The condensate amplitude may also have a gapped [Higgs mode](../../quantum-field-theory.md#higgs-mode), but that amplitude oscillation is distinct from the electromagnetic Higgs mechanism. Local gauge transformations remain a redundancy; this is not spontaneous breaking of an observable local symmetry in the same sense as the neutral global phase symmetry.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A bosonic [coherent state](../../quantum-theory.md#coherent-state) is an annihilation-operator eigenstate,

$$
|\alpha\rangle=e^{-|\alpha|^2/2}\sum_{N=0}^{\infty}\frac{\alpha^N}{\sqrt{N!}}|N\rangle,
\qquad a|\alpha\rangle=\alpha|\alpha\rangle.
$$

It has $\langle N\rangle=\operatorname{Var}N=|\alpha|^2$, a selected complex amplitude, and Poisson-distributed particle number. A [coherent-field condensate variational state](../../quantum-theory.md#coherent-field-condensate-variational-state) extends this construction to a spatial field with $\langle\widehat\psi(\mathbf r)\rangle=\Psi(\mathbf r)$. Evaluating a normal-ordered interacting Bose Hamiltonian in that state gives a classical-field [energy](../../energy.md) functional; its variational equation is the [Gross–Pitaevskii equation](../../quantum-ideal-gas-statistics.md#gross-pitaevskii-equation). This connects a macroscopic phase to [interference](../../physical-optics.md#interference-wave-propagation), [quantized circulation](../../critical-phenomenon.md#quantized-circulation) and neutral [Josephson effects](../../superconductivity.md#josephson-effect). A fixed-number condensate instead has vanishing one-point field expectation; [off-diagonal long-range order](../../critical-phenomenon.md#off-diagonal-long-range-order) identifies the condensate without requiring exact number fluctuations.

The [BCS ground state](../../fermi-liquid.md#bcs-ground-state) has the pair-coherent form

$$
|\mathrm{BCS}\rangle=\prod_{\mathbf k}
\left(u_{\mathbf k}+v_{\mathbf k}c_{\mathbf k\uparrow}^\dagger c_{-\mathbf k\downarrow}^\dagger\right)|0\rangle.
$$

It is a product of [Cooper-pair pseudospin coherent states](../../fermi-liquid.md#cooper-pair-pseudospin-coherent-state): each paired [momentum](../../momentum.md) sector mixes its empty and doubly occupied configurations. The anomalous pair expectation is $\langle c_{-\mathbf k\downarrow}c_{\mathbf k\uparrow}\rangle=u_{\mathbf k}^*v_{\mathbf k}$, while an ordinary single-electron expectation vanishes by [fermion](../../tensor-product-of-quantum-systems.md#fermion) parity. Pair operators are not unrestricted canonical [boson](../../tensor-product-of-quantum-systems.md#boson) operators, so this state must not be identified with a naive oscillator coherent state of individual [electrons](../../physics.md#electron). Number projection gives a fixed-even-number description with pair correlations. Phase differences between condensates enter the [Josephson effect](../../superconductivity.md#josephson-effect); in a charged condensate that phase difference must be gauge invariant.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For a one-component superfluid with nonzero order-parameter magnitude on a closed loop, the phase defines a map from the loop into the circle. Its [winding number](../../complex-analysis.md#winding-number) is

$$
\boxed{n=\frac1{2\pi}\oint\nabla\theta\cdot d\mathbf l\in\mathbb Z.}
$$

The [fundamental group](../../algebraic-topology.md#fundamental-group) $\pi_1(S^1)=\mathbb Z$ means that smooth deformations preserving nonzero amplitude cannot change this integer. With [superfluid velocity](../../statistical-physics.md#superfluid-velocity) $\mathbf v_s=\hbar\nabla\theta/m_B$, it gives [quantized circulation](../../critical-phenomenon.md#quantized-circulation) $\oint\mathbf v_s\cdot d\mathbf l=nh/m_B$. A vortex core permits the [order parameter](../../critical-phenomenon.md#order-parameter) to vanish and carries the winding; a [superfluid phase slip](../../critical-phenomenon.md#superfluid-phase-slip) changes a loop's winding when a core crosses it. For paired neutral [fermions](../../tensor-product-of-quantum-systems.md#fermion), the relevant condensed-object [mass](../../classical-mechanics.md#mass) is the pair [mass](../../classical-mechanics.md#mass).

For charged pairs, gauge-covariant phase rigidity gives [fluxoid and flux quantization in a superconductor](../../quantum-theory.md#fluxoid-and-flux-quantization-in-a-superconductor):

$$
\boxed{\Phi+\frac{m_*}{q}\oint\mathbf v_s\cdot d\mathbf l=\frac{nh}{q}.}
$$

The magnitude of the pair flux quantum is $h/(2e)$. [Magnetic flux](../../magnetic-field.md#magnetic-flux) alone approaches an integer multiple of this value when the circulating-velocity term on a bulk contour is negligible. The topological condition is not a claim that an arbitrary finite loop has exactly quantized [magnetic flux](../../magnetic-field.md#magnetic-flux) independent of its screening current.

There are also momentum-space invariants, distinct from real-space vortex winding. A fully gapped two-dimensional [Bogoliubov--de Gennes Hamiltonian](../../topological-quantum-matter.md#bogoliubov-de-gennes-hamiltonian) can have a [Chern number](../../algebraic-geometry.md#chern-number) obtained from its occupied [quasiparticle](../../quantum-mechanics.md#quasiparticle) bands' [Berry curvature](../../quantum-mechanics.md#berry-curvature). In a chiral paired model it can protect edge modes while the bulk gap and relevant symmetry class are maintained. Such an invariant can change only when those assumptions fail, for example through a bulk gap closing. A nodal d-wave state requires a different analysis; it is not automatically a fully gapped Chern superconductor.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [t-J model](../../statistical-physics.md#t-j-model) approximates the low-energy sector of a repulsive [Hubbard model](../../statistical-physics.md#hubbard-model) with $U\gg t$ near one [electron](../../physics.md#electron) per site. Large on-site repulsion suppresses double occupancy. Virtual hopping out of and back into that low-energy sector produces antiferromagnetic [superexchange](../../electromagnetism.md#superexchange) with $J=4t^2/U$. One conventional effective Hamiltonian is

$$
H=-t\sum_{\langle ij\rangle,\sigma}
\left(\widetilde c_{i\sigma}^\dagger\widetilde c_{j\sigma}+\mathrm{h.c.}\right)
+J\sum_{\langle ij\rangle}\left(\mathbf S_i\cdot\mathbf S_j-\frac14n_in_j\right),
$$

with [projected electron operator](../../statistical-physics.md#projected-electron-operator) $\widetilde c_{i\sigma}=c_{i\sigma}(1-n_{i\bar\sigma})$. At half filling, nearest-neighbor hopping cannot move an [electron](../../physics.md#electron) without entering a forbidden doubly occupied state, leaving the leading spin-exchange model. Doped holes can move and couple the charge dynamics to these spin correlations. Additional terms, including three-site processes at order $t^2/U$, are omitted in this simplified Hamiltonian.

The exchange term energetically favors a nearest-neighbor spin singlet. With $b_{ij}^\dagger=(c_{i\uparrow}^\dagger c_{j\downarrow}^\dagger-c_{i\downarrow}^\dagger c_{j\uparrow}^\dagger)/\sqrt2$ in the no-double-occupancy subspace, $\mathbf S_i\cdot\mathbf S_j-n_in_j/4=-b_{ij}^\dagger b_{ij}$. A square-lattice pairing ansatz can therefore use bond singlets with opposite signs along the two axes. This [d-wave bond order](../../superconductivity.md#d-wave-bond-order) has

$$
\boxed{\Delta_{\mathbf k}\propto\cos(k_xa)-\cos(k_ya),\qquad\Delta_x=-\Delta_y.}
$$

It changes sign under a quarter-turn and vanishes along the zone diagonals. It is an even-parity, spin-singlet pairing pattern, not a statement of triplet pairing or necessarily broken time reversal. Phase-sensitive [interference](../../physical-optics.md#interference-wave-propagation) experiments distinguish this sign structure from a merely anisotropic nonnegative gap in [cuprate superconductors](../../superconductivity.md#cuprate-superconductor).[1994 phase-sensitive tricrystal test](../../physics-bibliography.md#pairing-symmetry-and-flux-quantization-in-a-tricrystal-superconducting-ring-by-c-c-tsuei-and-others)

The model captures strong local repulsion, antiferromagnetism and mobile doped carriers. Its interacting phase diagram is not solved by writing down the Hamiltonian: a mean-field d-wave ansatz is a proposed approximation, not a proof that every parameter choice has that exact [ground state](../../quantum-mechanics.md#ground-state) or a complete microscopic explanation of every high-temperature superconductor.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

A [SQUID](../../superconductivity.md#squid) converts [magnetic flux](../../magnetic-field.md#magnetic-flux) into a periodic [interference](../../physical-optics.md#interference-wave-propagation) response of superconducting weak links. A [DC SQUID](../../superconductivity.md#dc-squid) has two [Josephson junctions](../../superconductivity.md#josephson-junction) in a loop. For equal junction critical currents $I_0$ and negligible loop self-inductance, their [Gauge-invariant Josephson phases](../../superconductivity.md#gauge-invariant-josephson-phase) differ by $2\pi\Phi/\Phi_0$, with $\Phi_0=h/(2e)$. Adding $I_0\sin\delta_1+I_0\sin\delta_2$ and maximizing over the common phase gives

$$
\boxed{I_c(\Phi)=2I_0\left|\cos\frac{\pi\Phi}{\Phi_0}\right|.}
$$

Thus the critical current repeats for every added flux quantum. A suitable current bias and dissipative junction dynamics convert the changing critical current into an observable voltage modulation. Junction asymmetry prevents exact zero minima, and appreciable self-inductance makes the flux include the circulating current's contribution; these require a modified response model. The [Jaklevic Josephson interference experiment](../../superconductivity.md#jaklevic-josephson-interference-experiment) supplies an early experimental realization of the [interference](../../physical-optics.md#interference-wave-propagation) principle.

An [RF SQUID](../../superconductivity.md#rf-squid) instead uses one junction in a loop inductively coupled to a radio-frequency resonator. In either design, a pickup coil and flux transformer can couple a small external field into the sensor, and flux feedback can keep it near a sensitive operating point over a larger measurement range. Applications include weak-field magnetometry, measurements of magnetic susceptibility and persistent currents, geophysical surveys and precision low-current detection. Gradiometers suppress common external fields, while thermal, junction and environmental noise set practical sensitivity. The instrument measures a flux-dependent electrical response; sensitivity is not established solely by the small size of $\Phi_0$.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [electron-phonon interaction](../../quantum-ideal-gas-statistics.md#electron-phonon-interaction) lets one [electron](../../physics.md#electron) polarize the ionic lattice and another interact with that delayed deformation. [Phonon-mediated electron attraction](../../quantum-ideal-gas-statistics.md#phonon-mediated-electron-attraction) acts over [energy](../../energy.md) transfers below a characteristic phonon scale. Pairing additionally requires a net attractive interaction in some allowed pairing channel after screened Coulomb repulsion is included. In the conventional weak-coupling situation, retardation separates the low phonon scale from the much larger electronic scale, reducing the effective repulsion. The [Cooper instability](../../fermi-liquid.md#cooper-instability) then makes a [Fermi surface](../../fermi-liquid.md#fermi-surface) unstable to an arbitrarily weak net attraction in the idealized channel; finite [temperature](../../temperature.md) cuts off its logarithmic enhancement.

In [BCS theory](../../fermi-liquid.md#bcs-theory), a momentum-independent pairing amplitude within the cutoff obeys a self-consistency equation containing $\tanh(E/2k_BT)/(2E)$, with [quasiparticle](../../quantum-mechanics.md#quasiparticle) [energy](../../energy.md) $E=\sqrt{\xi^2+|\Delta|^2}$. At a continuous transition, take $\Delta\to0$. A constant effective [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) and coupling combine into $\lambda$, while the band bottom truncates the negative-energy side at $-\sigma$, with $\sigma=\min(\mu,\theta)$. This gives the supplied linearized gap equation. Its integrand is even, so with

$$
I(a,T)=\int_0^a\frac{d\xi}{\xi}\tanh\frac{\xi}{2k_BT},
$$

it becomes $1/\lambda=[I(\theta,T_c)+I(\sigma,T_c)]/2$. If both cutoffs are much larger than $k_BT_c$, the given large-cutoff integral gives $I(a,T_c)\simeq\ln(1.13a/(k_BT_c))$. Consequently the [asymmetric-cutoff BCS transition temperature](../../fermi-liquid.md#asymmetric-cutoff-bcs-transition-temperature) is

$$
\frac1\lambda\simeq\ln\frac{1.13\sqrt{\theta\sigma}}{k_BT_c},\qquad
\boxed{k_BT_c\simeq1.13\sqrt{\theta\sigma}\,e^{-1/\lambda}.}
$$

For $\mu>\theta$, this reduces to $1.13\theta e^{-1/\lambda}$; for $0<\mu<\theta$, it is $1.13\sqrt{\theta\mu}\,e^{-1/\lambda}$. The second limit requires $k_BT_c\ll\mu$ as well as $k_BT_c\ll\theta$. Weak $\lambda$ at fixed nonzero $\mu/\theta$ supplies that limit, but taking $\mu\to0$ afterward need not preserve it.

For a three-dimensional spin-degenerate parabolic [electron](../../physics.md#electron) band in the degenerate regime,

$$
\mu\simeq E_F=\frac{\hbar^2}{2m}(3\pi^2n)^{2/3}.
$$

Define

$$
n_\theta=\frac1{3\pi^2}\left(\frac{2m\theta}{\hbar^2}\right)^{3/2},\qquad
T_0=\frac{1.13\theta}{k_B}e^{-1/\lambda},\qquad u=\frac n{n_\theta}.
$$

Holding the other model parameters fixed gives

$$
\boxed{T_c(n)\simeq
\begin{cases}
T_0u^{1/3},&0<u<1,\\
T_0,&u\ge1.
\end{cases}}
$$

Thus the log-log slope is $1/3$ below the cutoff-density scale and zero above it. For the specified parameters,

$$
\boxed{n_\theta\simeq1.15\times10^{26}\,\mathrm{m^{-3}},\qquad T_0\simeq40.3\,\mathrm K.}
$$

This [density crossover of a fixed-coupling BCS cutoff model](../../fermi-liquid.md#density-crossover-of-a-fixed-coupling-bcs-cutoff-model) is the requested prescribed model. A real three-dimensional parabolic band also has a changing [density of states](../../quantum-ideal-gas-statistics.md#density-of-states), so keeping $\lambda$ constant as density varies is an additional imposed assumption, not a consequence of that dispersion.

For noninteracting spinless bosonic pairs, [mass](../../classical-mechanics.md#mass) $m_B=2m$ and density $n_B=n/2$, [homogeneous ideal Bose gas condensation](../../quantum-ideal-gas-statistics.md#homogeneous-ideal-bose-gas-condensation) gives

$$
T_B=\frac{2\pi\hbar^2}{2mk_B}
\left[\frac{n/2}{\zeta(3/2)}\right]^{2/3}
=C_BT_F,\qquad T_F=E_F/k_B.
$$

Using the supplied integral $I_B=\int_0^\infty x^{1/2}/(e^x-1)\,dx\simeq2.3$ gives $C_B=\frac12[2/(3I_B)]^{2/3}\simeq0.219$. Its slight difference from the more precise $0.218$ is consistent with the rounded integral. Write $a=T_0/(\theta/k_B)=1.13e^{-1/\lambda}\simeq0.0403$. On the low-density branch,

$$
\frac{T_c}{T_B}=\frac{a}{C_B}u^{-1/3}.
$$

Since $a/C_B<1$, no part of the high-density plateau exceeds $T_B$. The formal crossing condition is

$$
\boxed{u<\left(\frac{a}{C_B}\right)^3\simeq0.00624,
\qquad n\lesssim7.2\times10^{23}\,\mathrm{m^{-3}}.}
$$

The crossing occurs near $T_c\simeq7.4\,\mathrm K$ and $T_F\simeq34\,\mathrm K$.

<a id="2/image-fixed-coupling-bcs-cutoff-prediction-compared-with-ideal-condensation-of-bosonic-pairs"></a>
![](../../past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge/2014/paper-1-transition-density.png)

**[Figure 1](#2/image-fixed-coupling-bcs-cutoff-prediction-compared-with-ideal-condensation-of-bosonic-pairs). Fixed-coupling BCS cutoff prediction compared with ideal condensation of bosonic pairs**.

The apparent low-density excess should not be read as a reliable transition above the ideal condensation scale of preformed pairs. On this extrapolation $k_BT_c/\mu=a u^{-1/3}$ grows without bound, violating the degenerate-gas and large-lower-cutoff approximations. It reaches one already near $7.5\times10^{21}\,\mathrm{m^{-3}}$; well before using an arbitrarily small density, the [chemical potential](../../chemical-potential.md), pairing, [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) and pair fluctuations need a self-consistent treatment. The asymptotic formula and ideal-boson curve compare two stipulated models, rather than solving the full [BCS-BEC crossover](../../fermi-liquid.md#bcs-bec-crossover).

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A complex [order parameter](../../critical-phenomenon.md#order-parameter) captures both the amplitude and phase rigidity of a [superfluid](../../statistical-physics.md#superfluid). A local isotropic [Ginzburg-Landau theory](../../critical-phenomenon.md#ginzburg-landau-theory) writes its free-energy functional, to fourth order in amplitude and second order in gradients, as

$$
\mathcal F[\Psi]=\int d^3r\left[\alpha|\Psi|^2+\frac\beta2|\Psi|^4+K|\nabla\Psi|^2\right],\qquad \beta,K>0.
$$

The uniform minimum has $\Psi=0$ for $\alpha>0$ and $|\Psi_0|^2=-\alpha/\beta$ for $\alpha<0$. Its phase remains arbitrary under a global $U(1)$ transformation. Minimizing with respect to $\Psi^*$ gives $-K\nabla^2\Psi+\alpha\Psi+\beta|\Psi|^2\Psi=0$. The phenomenological description specifies the allowed structures and coefficients; microscopic input is needed to identify the normalization of $\Psi$ and calculate those coefficients. A static functional by itself does not fix the dynamical equation or mode frequencies.

For a dilute three-dimensional Bose gas with short-range repulsion and particle [mass](../../classical-mechanics.md#mass) $m_B$, the microscopic low-energy Hamiltonian is

$$
\widehat H=\int d^3r\left[
\frac{\hbar^2}{2m_B}\nabla\widehat\psi^\dagger\cdot\nabla\widehat\psi
+V_{\rm ext}\widehat\psi^\dagger\widehat\psi
+\frac{g_B}{2}\widehat\psi^\dagger\widehat\psi^\dagger\widehat\psi\widehat\psi\right],
\qquad g_B=\frac{4\pi\hbar^2a_s}{m_B}>0.
$$

The interaction parameter is expressed through the low-energy [s-wave scattering length](../../quantum-scattering.md#s-wave-scattering-length) $a_s$, rather than an unrenormalized bare delta potential. In a symmetry-selected description, $\Psi=\langle\widehat\psi\rangle$ and $|\Psi|^2=n_0$ is condensate density. Equivalently, fixed-number [off-diagonal long-range order](../../critical-phenomenon.md#off-diagonal-long-range-order) identifies the macroscopically occupied natural orbital and its amplitude without a nonzero one-point expectation.

Evaluating $\widehat H-\mu\widehat N$ in a [coherent-field condensate variational state](../../quantum-theory.md#coherent-field-condensate-variational-state) gives the [Ginzburg-Landau functional of a dilute Bose gas](../../critical-phenomenon.md#ginzburg-landau-functional-of-a-dilute-bose-gas), with the mean-field microscopic identifications

$$
\boxed{K=\frac{\hbar^2}{2m_B},\qquad
\alpha=V_{\rm ext}-\mu,\qquad\beta=g_B.}
$$

Its stationary variational equation is the [Gross–Pitaevskii equation](../../quantum-ideal-gas-statistics.md#gross-pitaevskii-equation). The time-dependent variational action additionally contains $i\hbar\Psi^*\partial_t\Psi$, giving

$$
i\hbar\partial_t\Psi=\left[-\frac{\hbar^2\nabla^2}{2m_B}+V_{\rm ext}+g_B|\Psi|^2\right]\Psi.
$$

This term expresses [density-phase conjugacy](../../statistical-physics.md#density-phase-conjugacy). It is the missing microscopic dynamical input; a purely dissipative relaxation law would describe a different approximation.

[Bogoliubov theory](../../quantum-ideal-gas-statistics.md#bogoliubov-theory) writes $\widehat\psi=\Psi+\delta\widehat\psi$ and retains quadratic fluctuations. In a uniform condensate, $\mu=g_Bn_0$ and the fluctuation matrix is

$$
\begin{pmatrix}
\epsilon_k+g_Bn_0&g_Bn_0\\
-g_Bn_0&-\epsilon_k-g_Bn_0
\end{pmatrix}.
$$

Its eigenvalues are $\pm\sqrt{\epsilon_k(\epsilon_k+2g_Bn_0)}$. The positive branch is the gapless sound mode, continuously crossing over to particle-like excitations at larger $k$. The same result follows by linearizing the time-dependent [Gross–Pitaevskii equation](../../quantum-ideal-gas-statistics.md#gross-pitaevskii-equation) about its uniform solution. Thus the microscopic condensate amplitude, scattering interaction and [mass](../../classical-mechanics.md#mass) determine the mean-field static coefficients and the collective mode. Quadratic quantum fluctuations also produce [quantum depletion of a Bose condensate](../../quantum-ideal-gas-statistics.md#quantum-depletion-of-a-bose-condensate), which a pure coherent-state product omits.

These identifications are controlled for a dilute weakly interacting gas away from a fluctuation-dominated critical region. They are not a universal statement that the exact finite-temperature GL coefficient is always $-\mu$ or that its quartic coefficient never receives corrections. Integrating out noncondensed and short-wavelength modes produces effective temperature-dependent coefficients and can change their near-critical behavior. The phase rigidity described by $K$ and the thermodynamic order-parameter expansion remain the shared organizing structure.

For [BCS theory](../../fermi-liquid.md#bcs-theory), the microscopic [order parameter](../../critical-phenomenon.md#order-parameter) is instead an anomalous pair amplitude, commonly normalized as an [energy](../../energy.md) gap $\Delta\propto\langle\widehat\psi_\downarrow\widehat\psi_\uparrow\rangle$. It is not an ordinary single-electron field expectation or automatically the square root of a pair number density. Integrating out [fermions](../../tensor-product-of-quantum-systems.md#fermion) and expanding in small $\Delta$ and slow gradients near $T_c$ gives the [microscopic derivation of Ginzburg-Landau theory](../../superconductivity.md#microscopic-derivation-of-ginzburg-landau-theory). The [BCS pairing-field effective action](../../fermi-liquid.md#bcs-pairing-field-effective-action) supplies its coefficients through normal-state pair-response functions and thermal [fermion](../../tensor-product-of-quantum-systems.md#fermion) sums.

For example, a clean isotropic three-dimensional weak-coupling s-wave model, with $N(0)$ the [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) per spin at the [Fermi energy](../../quantum-ideal-gas-statistics.md#fermi-energy) and $\Delta$ measured in [energy](../../energy.md) units, gives

$$
\mathcal F_s-\mathcal F_n=\int d^3r
\left[\alpha_\Delta|\Delta|^2+\frac{\beta_\Delta}{2}|\Delta|^4
+K_\Delta\left|\left(\nabla-\frac{iq\mathbf A}{\hbar}\right)\Delta\right|^2
+\frac{|\mathbf B|^2}{2\mu_0}\right],\qquad q=-2e,
$$

with [microscopic Ginzburg-Landau coefficients from BCS theory](../../superconductivity.md#microscopic-ginzburg-landau-coefficients-from-bcs-theory)

$$
\boxed{\alpha_\Delta\simeq N(0)\frac{T-T_c}{T_c},\qquad
\beta_\Delta=\frac{7\zeta(3)N(0)}{8\pi^2(k_BT_c)^2},\qquad
K_\Delta=\frac{7\zeta(3)N(0)\hbar^2v_F^2}{48\pi^2(k_BT_c)^2}.}
$$

The numerical factors arise from fermionic [Matsubara sums](../../quantum-field-theory.md#bosonic-matsubara-sum) and the isotropic velocity average; they depend on the stated gap and density-of-states conventions. Rescaling the [order parameter](../../critical-phenomenon.md#order-parameter) rescales all three coefficients. The expansion applies near the transition with sufficiently slow spatial variation; disorder, anisotropic pairing and strong coupling alter the coefficients or require additional components. Microscopic derivation also fixes the pair charge in the covariant gradient, producing the superconducting screening current and the [Meissner effect](../../magnetic-field.md#meissner-effect).[1959, near-transition gap expansion and twice-electron charge](../../physics-bibliography.md#microscopic-derivation-of-the-ginzburg-landau-equations-in-the-theory-of-superconductivity-by-lev-gor-kov)

The neutral Bose and charged Fermi theories therefore share a complex [order parameter](../../critical-phenomenon.md#order-parameter) and a phase-stiffness functional, while deriving that field from different microscopic objects. The [Bogoliubov transformation](../../quantum-field-theory.md#bogoliubov-transformation) mixes particle and hole fluctuations of the bosonic condensate in one case and paired fermionic excitations in the other. The static GL limit organizes long-distance behavior; the full microscopic theories retain excitation spectra and [temperature](../../temperature.md) dependence beyond that local near-transition expansion.

## ↑ Ancestors (11)

1. [2014](../2014.md)
2. [Past exam of the superconductivity and Quantum Coherence course of the University of Cambridge](../../past-exam-of-the-superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge.md)
3. [Superconductivity and Quantum Coherence course of the University of Cambridge](../../university-of-cambridge.md#superconductivity-and-quantum-coherence-course-of-the-university-of-cambridge)
4. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
