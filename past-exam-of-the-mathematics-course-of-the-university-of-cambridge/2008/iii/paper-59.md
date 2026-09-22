# Paper 59

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper59.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper59.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
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
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
  - [iv](#5/iv)
    - [Solution](#5/iv/solution)
  - [v](#5/v)
    - [Solution](#5/v/solution)

## 1

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A limiting argument starts with a family of microscopic models $T_N$, a specified macroscopic quantity $M_N$ and a topology or operational criterion for convergence as $N\to\infty$. It is not enough to say that a large system has many constituents: one must identify what is held fixed, what [observables](../../../quantum-mechanics.md#observable) are compared and whether predictions converge uniformly. A [thermodynamic limit](../../../statistical-physics.md#thermodynamic-limit), for example, normally holds density and intensive parameters fixed while size increases. Other limits remove a resolution cutoff or enlarge an [observable](../../../quantum-mechanics.md#observable) algebra.

**A limiting theory can be both deduced from microscopic models and qualitatively novel.** The compatibility depends on distinguishing an exact property at the mathematical limit from the approximate collective behaviour of actual finite systems. The conceptual distinction is developed below, followed by three complementary examples rather than a claim that every form of [emergence](../../../physics.md#emergence) has the same mechanism.

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

[Theoretical reduction](../../../physics.md#theoretical-reduction) requires a relation between the quantities and domains of two theories, not just an assertion that their objects are made of the same material. A microscopic model may imply a macroscopic law after identifying temperature, magnetization or another collective variable, fixing admissible states and controlling an approximation. The bridge between descriptions can involve averaging or coarse-graining, and its adequacy must be established for the [observables](../../../quantum-mechanics.md#observable) of interest. A reduction of a particular class of predictions is weaker than deriving every explanatory claim of an entire theory.

[Emergence](../../../physics.md#emergence) can mean that a collective description displays behaviour novel relative to individual constituents, robust under changes in microscopic details and naturally explained with new macroscopic concepts. In this sense it does not contradict [theoretical reduction](../../../physics.md#theoretical-reduction): a derivation can explain why a new pattern appears. A stronger assertion of irreducible causal powers is a different thesis. The existence of a singular mathematical limit does not on its own prove that stronger thesis.

A crucial distinction is between $T_\infty$ and any finite $T_N$. A limit of analytic functions need not be analytic, and a limiting state representation need not retain the structures of each finite representation. Therefore a claim about $T_\infty$ need not be literally true of $T_N$ even when the approximations are excellent for accessible measurements. Deduction of the limiting theory uses the whole family of finite theories together with a limit theorem; it does not deduce a false exact singularity in one finite system. Approximate [theoretical reduction](../../../physics.md#theoretical-reduction) then explains the observed rounded or scale-limited counterpart.

The role of explanatory autonomy is also important. [Universality](../../../critical-phenomenon.md#universality-of-critical-phenomena) at a [phase transition](../../../critical-phenomenon.md#phase-transition) can make a macroscopic description insensitive to many microscopic parameters. That robustness supports using the emergent description without tracking every particle. It does not establish that the microscopic laws have ceased to apply. The [renormalization group](../../../critical-phenomenon.md#renormalization-group) helps explain such insensitivity by distinguishing perturbations which persist at large scales from those which become negligible.

**The defensible conclusion is that novelty and derivability can coexist; the limiting idealization and its finite-system accuracy must be stated separately.** Whether one calls the resulting behaviour emergent depends partly on which lower-level description and explanatory expectations form the comparison, rather than solely on the size of $N$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For [fractal geometry](../../../geometry-and-topology.md#fractal-geometry), let $C_n$ be the $n$th middle-third construction of the [Cantor set](../../../geometry-and-topology.md#cantor-set). It contains $2^n$ intervals of length $3^{-n}$, with total length $(2/3)^n$. Each finite $C_n$ contains intervals, so its [Hausdorff dimension](../../../measure-theory.md#hausdorff-dimension) is one. The limiting set $C=\bigcap_nC_n$ has zero length and

$$
\boxed{\dim_H C=\frac{\log2}{\log3}.}
$$

Indeed, $2^n$ intervals of scale $3^{-n}$ cover it, giving the upper dimension bound from $2^n3^{-ns}\to0$ whenever $s>\log2/\log3$. For the lower bound, assign mass $2^{-n}$ to each level-$n$ interval. Any sufficiently small interval of length $r$ meets only a bounded number of construction intervals at the comparable scale, giving a bound $\mu(I)\le Kr^{\log2/\log3}$. Covering $C$ by such intervals then forces their dimension-weighted sizes to sum to at least $1/K$, yielding the matching lower bound. The noninteger dimension is deducible from a simple iterative rule even though it is absent from every finite-stage set at arbitrarily fine resolution. A finite construction nevertheless exhibits the same scaling over intermediate resolutions. Thus the order of idealization and probing ever smaller scales matters: an actual finite-resolution pattern can have useful fractal behaviour without possessing the exact limiting dimension at all scales.

For a [phase transition](../../../critical-phenomenon.md#phase-transition), finite-spin [partition functions](../../../statistical-physics.md#canonical-partition-function) are finite sums of positive exponentials at real finite temperature and field. Their [free energies](../../../thermodynamics.md#thermodynamic-free-energy) are therefore analytic there. Genuine thermodynamic nonanalyticity can appear only after a suitable infinite-system limit. The [Curie–Weiss model](../../../statistical-physics.md#curie-weiss-model) gives an explicit demonstration. With $s_i=\pm1$, take

$$
H_N=-\frac{J}{2N}\left(\sum_i s_i\right)^2-h\sum_i s_i,\qquad J>0,\qquad\beta=(k_BT)^{-1}.
$$

Grouping configurations by $m=N^{-1}\sum_i s_i$ and using their binomial multiplicities gives the limiting [free energy](../../../thermodynamics.md#thermodynamic-free-energy) as the minimum of

$$
f(m)=-\frac J2m^2-hm-\beta^{-1}s(m),\qquad s(m)=-\frac{1+m}{2}\log\frac{1+m}{2}-\frac{1-m}{2}\log\frac{1-m}{2}.
$$

The number of possible magnetizations grows only linearly with $N$, so their largest exponential contribution determines the limiting [free energy](../../../thermodynamics.md#thermodynamic-free-energy). Differentiating the variational expression gives

$$
m=\tanh\{\beta(Jm+h)\}.
$$

At $h=0$ and $\beta J>1$, its two stable minima have magnetizations $\pm m_*\ne0$. Every finite zero-field system instead has exactly zero mean magnetization by spin-inversion [symmetry](../../../physics.md#symmetry-physics). Consequently

$$
\boxed{\lim_{h\downarrow0}\lim_{N\to\infty}\langle m\rangle_{N,h}=m_*,\qquad\lim_{N\to\infty}\lim_{h\downarrow0}\langle m\rangle_{N,h}=0.}
$$

This noncommutation of limits explains how [spontaneous symmetry breaking](../../../quantum-field-theory.md#spontaneous-symmetry-breaking) emerges. Below the critical temperature, the limiting [free energy](../../../thermodynamics.md#thermodynamic-free-energy) has a cusp in $h$ at zero, while finite systems have a sharp but smooth crossover. Away from the critical point, the relative weights of the two phases behave approximately as $e^{2\beta Nhm_*}$; the rounded magnetization is correspondingly about $m_*\tanh(\beta Nhm_*)$. Exact singularity belongs to the idealized limit, whereas the narrow crossover and long-lived phases can be physically useful at finite size. The [theoretical reduction](../../../physics.md#theoretical-reduction) is the derivation and its approximation control, not a claim that a finite analytic [partition function](../../../statistical-physics.md#canonical-partition-function) is already nonanalytic.

For [superselection](../../../quantum-theory.md#superselection-rule), consider an infinite spin lattice with [quasi-local observable algebra](../../../functional-analysis.md#quasi-local-observable-algebra) $\mathcal A$. These are zero-temperature equilibrium phases of a ferromagnetic Ising spin Hamiltonian with nearest-neighbour interactions $-J\sigma_z^{(i)}\sigma_z^{(j)}$. At finite $N$, the all-up and all-down vectors belong to one Hilbert space, and the coherent state

$$
|\Psi_N\rangle=\frac{|\uparrow\cdots\uparrow\rangle+e^{i\theta}|\downarrow\cdots\downarrow\rangle}{\sqrt2}
$$

is distinguishable from the corresponding mixture by a suitably chosen global [observable](../../../quantum-mechanics.md#observable). But if $A_R$ acts on only $R<N$ spins, its off-diagonal matrix element between these vectors vanishes: the untouched spins contribute $\langle\uparrow|\downarrow\rangle=0$. Hence its expectations already equal those of the equal-weight mixture, independent of $\theta$. Increasingly global [observables](../../../quantum-mechanics.md#observable) can recover the phase at finite $N$, but the infinite product of spin flips is not a norm limit of finite-support [observables](../../../quantum-mechanics.md#observable) and is absent from $\mathcal A$.

In the infinite-volume limit the up and down phases have disjoint state representations. The averaged magnetization $M_N=N^{-1}\sum_i\sigma_z^{(i)}$ commutes asymptotically with any fixed local [observable](../../../quantum-mechanics.md#observable): $\|[M_N,A_R]\|\le2R\|A_R\|/N$. In the phase representations its limiting values are $+1$ and $-1$, distinguishing sectors. Finite spin-flip vectors form a dense set on which these averages tend to their respective scalar values, so boundedness extends the strong limits to the phase Hilbert spaces. An intertwiner between the representations would obey $(-I)T=T(+I)$ and must therefore vanish, explaining their disjointness. In the combined representation the [observable](../../../quantum-mechanics.md#observable) algebra is block-diagonal between them, so no quasilocal measurement detects their relative phase. This yields an emergent [superselection rule](../../../quantum-theory.md#superselection-rule) relative to the chosen [observable](../../../quantum-mechanics.md#observable) algebra. It is not a derivation of physical wave-function collapse. **Fractal dimension, a thermodynamic singularity and sector separation each exhibit new limiting structure while retaining an explicit microscopic construction.**

## 2

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Consider two spacelike-separated measurement regions $R_A$ and $R_B$, with locally chosen settings $a,b\in\{0,1\}$ and recorded outcomes $A,B\in\{-1,1\}$. A relevant past region supplies a sufficient specification $\lambda$ of the common preparation and other hidden physical information needed to screen the outcomes. This is not necessarily just a [quantum state](../../../quantum-mechanics.md#quantum-state) written at the source, nor a conditioning on arbitrary records which already contain the future choices. The spacetime shielding and sufficiency requirements are substantive causal assumptions.

Use [Bell local causality](../../../quantum-theory.md#bell-local-causality): once the relevant past is sufficiently specified, learning facts in the remote measurement region changes no local outcome probability. In particular, require

$$
P(A\mid a,b,B,\lambda)=P(A\mid a,\lambda),\qquad P(B\mid a,b,\lambda)=P(B\mid b,\lambda),
$$

where conditional probabilities are defined. The probability chain rule gives

$$
P(A,B\mid a,b,\lambda)=P(A\mid a,\lambda)P(B\mid b,\lambda).
$$

This factorization combines [parameter independence](../../../quantum-theory.md#parameter-independence) with [outcome independence](../../../quantum-theory.md#outcome-independence). Neither probability is required to be zero or one: the argument includes stochastic [local hidden-variable theories](../../../quantum-theory.md#local-hidden-variable-theory).

Also assume [measurement independence](../../../quantum-theory.md#measurement-independence), $\rho(\lambda\mid a,b)=\rho(\lambda)$, so all four setting pairs average over one normalized nonnegative past-variable distribution. This is a statistical condition on the setting procedure and relevant hidden information, not a proof of a metaphysical doctrine of free will. Finally the recorded outcomes must represent the same ensemble of trials. One can include nondetections in a specified bounded-outcome rule; if instead one discards events depending on setting or outcome, a further sampling assumption is required. Setting-dependent postselection is not covered silently by the argument.

Let $\alpha_a(\lambda)=\sum_A AP(A\mid a,\lambda)$ and $\beta_b(\lambda)=\sum_B BP(B\mid b,\lambda)$. They lie in $[-1,1]$, and the factorization gives

$$
E_{ab}=\int\rho(\lambda)\alpha_a(\lambda)\beta_b(\lambda)\,d\lambda.
$$

For each $\lambda$,

$$
|\alpha_0(\beta_0+\beta_1)+\alpha_1(\beta_0-\beta_1)|\le|\beta_0+\beta_1|+|\beta_0-\beta_1|=2\max(|\beta_0|,|\beta_1|)\le2.
$$

Averaging with the same $\rho$ proves the [CHSH inequality](../../../quantum-theory.md#chsh-inequality)

$$
\boxed{|E_{00}+E_{01}+E_{10}-E_{11}|\le2.}
$$

No separate assumption of simultaneous predetermined values for incompatible quantum [observables](../../../quantum-mechanics.md#observable) was needed. The common probability model and its screening relations did the work.

A [Reichenbach common cause principle](../../../physics.md#reichenbach-common-cause-principle) can motivate the same calculation: a complete classical common cause in the past screens the two outcomes, while each setting affects only its own wing. Together with setting-independent sampling this gives the displayed factorization. It is not enough to provide a different screening variable for each pair of settings: those constructions need not form one compatible common-cause model for the four correlations.

A [stochastic Einstein locality](../../../physics.md#stochastic-einstein-locality) formulation instead constrains objective chances by facts in the appropriate causal past. To use it as a sufficient premise here, specify both local dependence on settings and a joint screening condition for the two outcomes. Merely requiring local marginal chances not to depend on a remote setting gives [parameter independence](../../../quantum-theory.md#parameter-independence), which is weaker than factorization. Thus the precise stochastic locality version matters; one should not infer a [Bell inequality](../../../quantum-theory.md#bell-inequality) from every condition loosely described as no superluminal influence.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For a [spin singlet state](../../../bell-state.md#spin-singlet-state), quantum spin measurements along unit vectors $\mathbf a,\mathbf b$ predict $E(\mathbf a,\mathbf b)=-\mathbf a\cdot\mathbf b$. Take $\mathbf a_0=\mathbf z$, $\mathbf a_1=\mathbf x$, $\mathbf b_0=(\mathbf z+\mathbf x)/\sqrt2$ and $\mathbf b_1=(\mathbf z-\mathbf x)/\sqrt2$. These give

$$
\boxed{|E_{00}+E_{01}+E_{10}-E_{11}|=2\sqrt2>2.}
$$

The violation therefore excludes the whole conjunction of the sufficient assumptions, for any model reproducing these correlations. It does not identify which premise fails without further commitments about causal explanation, state completeness and measurement setting generation.

A defensible verdict is to retain ordinary independent setting preparation and reject [Bell local causality](../../../quantum-theory.md#bell-local-causality), specifically its classical screening-off factorization. In standard [quantum theory](../../../quantum-theory.md), taking the pure entangled state as the complete state preserves [parameter independence](../../../quantum-theory.md#parameter-independence): each local marginal is $1/2$, regardless of the distant setting. Yet [outcome independence](../../../quantum-theory.md#outcome-independence) fails. For equal spin axes, $P(A=+,B=-)=1/2$, whereas $P(A=+)P(B=-)=1/4$. The distant outcome changes the conditional prediction even after the [quantum state](../../../quantum-mechanics.md#quantum-state) is specified. This failure is compatible with [quantum no-signalling](../../../quantum-theory.md#quantum-no-signalling), since conditioning on that outcome requires learning a result which cannot itself be controlled.

Adding further past variables does not restore the entire Bell conjunction while retaining the violating correlations; the [CHSH inequality](../../../quantum-theory.md#chsh-inequality) already allowed arbitrary such $\lambda$. Alternatively, one may reject [measurement independence](../../../quantum-theory.md#measurement-independence), permit retrocausal setting dependence in the relevant past state, or adopt another non-Bell-local description. Those are logically possible responses, but each must explain its replacement probability and causal model rather than treating the inequality as a failed algebraic theorem. A deterministic theory is not exempt from this requirement.

The assumption of [measurement independence](../../../quantum-theory.md#measurement-independence) is supported by the purpose and design of independently varied settings, but cannot be proved for every conceivable hidden variable merely by inspecting observed setting frequencies. Conversely, a rejection of [Bell factorization](../../../quantum-theory.md#bell-local-causality) does not alone establish a controllable superluminal signal or select a unique ontology. **The reasoned verdict is against Bell's screening-off locality, conditional on the other stated premises; the unconditional conclusion concerns their conjunction.**

## 3

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a finite-dimensional mechanical system let $Q$ be its [configuration space](../../../classical-mechanics.md#mechanical-configuration-space), a smooth manifold incorporating the holonomic constraints. [Lagrangian mechanics](../../../classical-mechanics.md#lagrangian-mechanics) starts with $L:TQ\to\mathbb R$; a curve $q(t)$ makes the action stationary under fixed-endpoint variations. The resulting equations are

$$
\frac{d}{dt}\frac{\partial L}{\partial v^i}-\frac{\partial L}{\partial q^i}=0.
$$

This equation is coordinate-independent even though generalized coordinates give its familiar expression.

The fibre derivative $\mathbb FL(q,v)=(q,p)$, with $p_i=L_{v^i}$, defines the [Legendre transform in mechanics](../../../classical-mechanics.md#legendre-transform-in-mechanics). The [Cartan form of a regular mechanical Lagrangian](../../../classical-mechanics.md#cartan-form-of-a-regular-mechanical-lagrangian) is

$$
\theta_L=p_i\,dq^i,\qquad\omega_L=-d\theta_L,\qquad E_L=p_iv^i-L.
$$

For a [regular Lagrangian](../../../classical-mechanics.md#regular-lagrangian), the velocity Hessian is invertible, $\omega_L$ is symplectic, and $\iota_{\Gamma_L}\omega_L=dE_L$ determines a second-order vector field on $TQ$. In coordinates this recovers the displayed Euler–Lagrange equations: the velocity components of the vector field are $v^i$, and its acceleration components are fixed by the invertible Hessian.

[Hamiltonian mechanics](../../../classical-mechanics.md#hamiltonian-mechanics) takes place on $T^*Q$. Its [tautological one-form](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle) is $\theta=p_i\,dq^i$, and its canonical [symplectic form](../../../symplectic-geometry.md#symplectic-form) is $\omega=-d\theta=dq^i\wedge dp_i$. With $\iota_{X_H}\omega=dH$,

$$
\boxed{\dot q^i=H_{p_i},\qquad\dot p_i=-H_{q^i}.}
$$

The associated [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) is $\{f,g\}=f_{q^i}g_{p_i}-f_{p_i}g_{q^i}$, so $X_Hf=\{f,H\}$. For a [hyperregular Lagrangian](../../../classical-mechanics.md#hyperregular-lagrangian), $\mathbb FL$ is a global diffeomorphism, $H=E_L\circ(\mathbb FL)^{-1}$ and $(\mathbb FL)^*\omega=\omega_L$. The two formulations then describe the same trajectories. Regularity gives only local equivalence; degenerate Lagrangians require constraint analysis instead. These geometric structures distinguish equations of motion from arbitrary coordinate formulae and make [symmetry](../../../physics.md#symmetry-physics) reduction precise.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

In [Lagrangian mechanics](../../../classical-mechanics.md#lagrangian-mechanics), let a one-parameter group on $Q$ have generator $\xi_Q=\xi^i(q)\partial_{q^i}$. Its tangent lift acts on $TQ$ as

$$
\xi_{TQ}=\xi^i\partial_{q^i}+v^j\partial_j\xi^i\partial_{v^i}.
$$

If $L$ is invariant, $\xi_{TQ}L=0$. Along an Euler–Lagrange trajectory, the [Noether conserved quantity for a mechanical point symmetry](../../../calculus-of-variations.md#noether-conserved-quantity-for-a-mechanical-point-symmetry) is

$$
J^L_\xi=\theta_L(\xi_{TQ})=\frac{\partial L}{\partial v^i}\xi^i,
$$

because

$$
\frac{dJ^L_\xi}{dt}=\dot p_i\xi^i+p_i\partial_j\xi^i v^j=L_{q^i}\xi^i+L_{v^i}\partial_j\xi^iv^j=\xi_{TQ}L=0.
$$

Thus the [conserved quantity](../../../classical-mechanics.md#conserved-quantity) is explicitly derived, not merely attached to the name of a [symmetry](../../../physics.md#symmetry-physics). If the change of $L$ is the total derivative $dB/dt$, then $p_i\xi^i-B$ is conserved. For a general point transformation with time component $\tau$, the conserved expression is $p_i\xi^i-E_L\tau-B$, provided the variation of $L\,dt$ is $dB$. Time-translation invariance of an autonomous Lagrangian therefore yields conservation of energy.

In [Hamiltonian mechanics](../../../classical-mechanics.md#hamiltonian-mechanics), a cotangent-lifted action preserves $\theta$ and hence $\omega$. For its infinitesimal generator $\xi_{T^*Q}$, [Cartan's magic formula](../../../differential-form.md#cartan-s-magic-formula) gives

$$
0=\mathcal L_{\xi_{T^*Q}}\theta=\iota_{\xi_{T^*Q}}d\theta+d(\theta(\xi_{T^*Q})),\qquad\iota_{\xi_{T^*Q}}\omega=dJ_\xi,
$$

where $J_\xi=p_i\xi^i$. These components define the canonical [moment map](../../../symplectic-geometry.md#moment-map) $J:T^*Q\to\mathfrak g^*$, with $\langle J,\xi\rangle=J_\xi$. If $H$ is invariant, $\{H,J_\xi\}=0$, so $\dot J_\xi=\{J_\xi,H\}=0$. This is the Hamiltonian form of [Noether's theorem](../../../calculus-of-variations.md#noether-conserved-quantity-for-a-mechanical-point-symmetry), and the [Legendre transform in mechanics](../../../classical-mechanics.md#legendre-transform-in-mechanics) identifies its charges with the Lagrangian ones.

More generally, a [Hamiltonian group action](../../../symplectic-geometry.md#hamiltonian-group-action) is an action whose infinitesimal symplectic generators have globally defined Hamiltonian functions. The existence of those functions is an assumption, not a consequence of every symplectic action. For example, translation on a symplectic two-torus preserves $dq\wedge dp$ but contraction with $\partial_q$ gives $dp$, which is closed and not globally exact. Such a [symmetry](../../../physics.md#symmetry-physics) need not have a globally single-valued moment-map component. On $T^*Q$, the cotangent lift does have the canonical components just derived. **A Hamiltonian [symmetry](../../../physics.md#symmetry-physics) preserving $H$ gives a conserved generator; the global momentum-map hypotheses must be stated.**

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For $N$ labelled particles with collisions excluded, [Newtonian gravity](../../../classical-mechanics.md#gravitational-acceleration) has

$$
L=\frac12\sum_i m_i|\dot{\mathbf q}_i|^2+G\sum_{i<j}\frac{m_im_j}{|\mathbf q_i-\mathbf q_j|}.
$$

Simultaneously translating every position or applying the same time-independent spatial rotation preserves both [kinetic energy](../../../classical-mechanics.md#kinetic-energy) and the distance-dependent potential. The conserved [momentum](../../../classical-mechanics.md#momentum) and [angular momentum](../../../classical-mechanics.md#angular-momentum) obtained from [Noether's theorem](../../../calculus-of-variations.md#noether-conserved-quantity-for-a-mechanical-point-symmetry) are

$$
\boxed{\mathbf P=\sum_i\mathbf p_i,\qquad\mathbf L=\sum_i\mathbf q_i\times\mathbf p_i.}
$$

Time translations give the conserved Hamiltonian. Galilean boosts change the Lagrangian by a total derivative, rather than leaving it strictly unchanged; they give the conserved centre-of-mass quantity $M\mathbf R-t\mathbf P$, where $M=\sum_i m_i$ and $\mathbf R=M^{-1}\sum_i m_i\mathbf q_i$. Thus absolute uniform velocity is not singled out by the isolated dynamics.

Translations can be separated explicitly. Put $\mathbf r_i=\mathbf q_i-\mathbf R$, so $\sum_i m_i\mathbf r_i=0$. Then

$$
\frac12\sum_i m_i|\dot{\mathbf q}_i|^2=\frac12M|\dot{\mathbf R}|^2+\frac12\sum_i m_i|\dot{\mathbf r}_i|^2,
$$

with the cross-term vanishing. The potential depends only on $\mathbf r_i-\mathbf r_j$. The centre-of-mass motion is therefore a decoupled free motion; at fixed $\mathbf P$ its energy is $\mathbf P^2/(2M)$ and it can be eliminated from the internal equations. Choosing a centre-of-mass rest frame sets $\mathbf P=0$.

One can then quotient internal configurations by simultaneous rotations. On generic noncollinear configurations with $N\ge3$ the resulting [relational shape space](../../../classical-mechanics.md#relational-shape-space) has dimension $3N-6$; collinear configurations have stabilizers and belong to singular strata. For two particles only the separation remains, so that generic dimension formula is inapplicable. This configuration quotient identifies absolute placement and orientation, but it does not by itself specify all the reduced dynamics.

At the phase-space level, [symplectic reduction](../../../symplectic-geometry.md#symplectic-reduction) is performed at a fixed moment-map value: $J^{-1}(\mu)/G_\mu$, where $G_\mu$ is the coadjoint [stabilizer](../../../group-theory.md#stabilizer-subgroup). In particular, at fixed nonzero [angular momentum](../../../classical-mechanics.md#angular-momentum) one does not simply divide the [momentum](../../../classical-mechanics.md#momentum) level by every rotation. The reduction retains the appropriate angular-momentum data and centrifugal effects. Even for two gravitating particles, specifying $r$ and $\dot r$ alone is insufficient unless the angular-momentum parameter is supplied:

$$
\ddot r=\frac{\ell^2}{\mu_r^2r^3}-\frac{G(m_1+m_2)}{r^2},\qquad\mu_r=\frac{m_1m_2}{m_1+m_2}.
$$

Systems with identical instantaneous separation and radial velocity but different $\ell$ have different radial futures. Eliminating orientation while discarding this parameter would not be a faithful reduction.

These results support a relational treatment of overall position and orientation: isolated configurations differing only by one fixed translation or rotation have the same internal predictions. However, a [symmetry](../../../physics.md#symmetry-physics) and a declared gauge equivalence are conceptually different, and the quotient alone does not settle the ontology of space. Arbitrary time-dependent rotations are not [symmetries](../../../physics.md#symmetry-physics) of the original inertial equations; a rotating coordinate description brings Coriolis and centrifugal terms. Newtonian inertial structure and absolute acceleration therefore cannot be eliminated merely by citing rotational invariance. A relational theory may encode that structure through additional dynamical or connection data, but it must reproduce these effects rather than erase them.

**The [symmetries](../../../physics.md#symmetry-physics) license mathematically controlled elimination of collective variables, with [momentum](../../../classical-mechanics.md#momentum) and regularity qualifications; they do not alone prove either absolute space or complete relationalism.** This distinguishes redundant descriptions of a solution from genuinely different possible motions.

## 4

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [Poisson manifold](../../../symplectic-geometry.md#poisson-manifold) is a smooth manifold $M$ with a bilinear bracket on smooth functions that is antisymmetric, obeys the Leibniz rule and satisfies the [Jacobi identity](../../../lie-algebra.md#jacobi-identity). Equivalently, a [Poisson tensor](../../../symplectic-geometry.md#poisson-tensor) $\pi$ gives $\{f,g\}=\pi(df,dg)$. Its rank need not be constant or maximal. Here define Hamiltonian evolution by $X_Hf=\{f,H\}$, agreeing with the canonical bracket $\{q^i,p_j\}=\delta^i_j$.

A smooth [Lie group action](../../../lie-theory.md#lie-group-action) sends each $x$ along its orbit $Gx$, with [stabilizer](../../../group-theory.md#stabilizer-subgroup) $G_x$. If the action is free and proper, the orbit space is a smooth quotient manifold and the projection is a submersion. Without these hypotheses the quotient can have singular orbit-type strata, or even fail to be Hausdorff. For an action preserving the [Poisson bracket](../../../classical-mechanics.md#poisson-bracket), invariant functions form a Poisson subalgebra. On a smooth quotient $M/G$, their identification with smooth quotient functions defines

$$
\{\bar f,\bar g\}_{M/G}\circ r=\{\bar f\circ r,\bar g\circ r\}_M.
$$

Thus $r$ is a [Poisson map](../../../symplectic-geometry.md#poisson-map). The quotient is generally Poisson, not necessarily symplectic: different reduced [momentum](../../../classical-mechanics.md#momentum) sectors can be different leaves. An arbitrary smooth [group action](../../../group-theory.md#group-action) alone does not guarantee this bracket descent.

For a [Lie group](../../../lie-theory.md#lie-group) $G$, conjugation $h\mapsto ghg^{-1}$ differentiates at the identity to the [Adjoint representation of a Lie group](../../../lie-theory.md#adjoint-representation-of-a-lie-group), $\operatorname{Ad}_g:\mathfrak g\to\mathfrak g$. Its infinitesimal version is $\operatorname{ad}_\xi\eta=[\xi,\eta]$. The [coadjoint representation](../../../lie-theory.md#coadjoint-representation) on the dual space is defined by

$$
\langle\operatorname{Ad}^*_g\ell,\xi\rangle=\langle\ell,\operatorname{Ad}_{g^{-1}}\xi\rangle,\qquad\langle\operatorname{ad}^*_\xi\ell,\eta\rangle=-\langle\ell,[\xi,\eta]\rangle.
$$

The inverse in the first formula makes this a left action. These definitions distinguish the representation on infinitesimal generators from its dual action on momenta.

There is a natural positive [Lie-Poisson bracket](../../../symplectic-geometry.md#lie-poisson-bracket) on $\mathfrak g^*$:

$$
\boxed{\{F,G\}_+(\ell)=\langle\ell,[dF_\ell,dG_\ell]\rangle.}
$$

The differentials lie in $(\mathfrak g^*)^*\simeq\mathfrak g$. In a basis with $[e_a,e_b]=c_{ab}{}^ce_c$, linear coordinates satisfy $\{\ell_a,\ell_b\}_+=c_{ab}{}^c\ell_c$. The bracket extends by the chain rule and Leibniz rule to smooth functions. Its coordinate Jacobi condition reduces precisely to the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) for $c_{ab}{}^c$, proving that it is Poisson. Reversing its overall sign also gives a [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) and is useful for body-frame conventions below.

On a general [Poisson manifold](../../../symplectic-geometry.md#poisson-manifold), the vectors $X_f$ span a distribution. The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) closes this family under commutators, and its orbits under Hamiltonian flows form the [symplectic foliation](../../../symplectic-geometry.md#symplectic-foliation). On each leaf the induced two-form satisfies

$$
\omega(X_f,X_g)=\{f,g\}.
$$

It is well-defined after quotienting out differential covectors giving zero [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field), is nondegenerate on the leaf, and is closed by the [Jacobi identity](../../../lie-algebra.md#jacobi-identity). Leaf dimensions can vary, so ordinary constant-rank foliation terminology must be qualified. A Hamiltonian trajectory remains in one leaf; a [Casimir function of a Poisson manifold](../../../symplectic-geometry.md#casimir-function-of-a-poisson-manifold) is constant along all such trajectories, but its level set can contain more than one leaf.

For $\mathfrak g^*$, $X_F(\ell)=\operatorname{ad}^*_{dF_\ell}\ell$ under the convention above. Hence the connected [coadjoint orbits](../../../lie-theory.md#coadjoint-orbit) are exactly its [symplectic leaves](../../../symplectic-geometry.md#symplectic-leaf) for connected $G$; for disconnected $G$, take connected orbit components. The orbit two-form is the [Kirillov–Kostant–Souriau symplectic form](../../../lie-theory.md#kirillov-kostant-souriau-symplectic-form):

$$
\boxed{\omega_\ell(\operatorname{ad}^*_\xi\ell,\operatorname{ad}^*_\eta\ell)=\langle\ell,[\xi,\eta]\rangle.}
$$

If a generator is in the [stabilizer](../../../group-theory.md#stabilizer-subgroup), its pairing with every bracket vanishes, proving independence of the choice of tangent generator. Conversely, vanishing pairing with all tangent generators puts it in that [stabilizer](../../../group-theory.md#stabilizer-subgroup), proving nondegeneracy. The cyclic derivative relation giving $d\omega=0$ is the [Lie algebra](../../../lie-algebra.md) [Jacobi identity](../../../lie-algebra.md#jacobi-identity). This explains the symplectic structure of the orbit rather than just naming it.

Identify the [SO(3) Lie algebra](../../../semisimple-lie-algebra.md#so-3-lie-algebra) with $\mathbb R^3$ by the hat map $\widehat{\boldsymbol\xi}\mathbf v=\boldsymbol\xi\times\mathbf v$. Its Lie bracket becomes the vector cross product, and the invariant Euclidean pairing identifies the dual with angular-momentum vectors $\mathbf M$. The [coadjoint action](../../../lie-theory.md#coadjoint-representation) is ordinary rotation, with infinitesimal action $\boldsymbol\xi\times\mathbf M$. Therefore its nonzero orbits are spheres $|\mathbf M|=r$; the origin is a zero-dimensional leaf. In these coordinates,

$$
\{F,G\}_+=\mathbf M\cdot(\nabla F\times\nabla G),\qquad C(\mathbf M)=|\mathbf M|^2
$$

is a [Casimir function of a Poisson manifold](../../../symplectic-geometry.md#casimir-function-of-a-poisson-manifold), since its gradient is parallel to $\mathbf M$. For tangent vectors $\mathbf v,\mathbf w$ to a nonzero sphere, the positive orbit form is

$$
\omega_{\mathbf M}(\mathbf v,\mathbf w)=\frac{\mathbf M\cdot(\mathbf v\times\mathbf w)}{r^2}.
$$

Its area integral with the corresponding orientation is $4\pi r$, and it reverses sign with the negative bracket.

For a torque-free [rigid body](../../../classical-mechanics.md#rigid-body-dynamics), choose body [angular momentum](../../../classical-mechanics.md#angular-momentum) $\mathbf M$ and principal moments $I_1,I_2,I_3>0$. Reduction of $T^*SO(3)$ by spatial rotations gives the body-frame negative [Lie-Poisson bracket](../../../symplectic-geometry.md#lie-poisson-bracket) and Hamiltonian

$$
\{F,G\}_{\mathrm{body}}=-\mathbf M\cdot(\nabla F\times\nabla G),\qquad H=\frac12\sum_{i=1}^3\frac{M_i^2}{I_i}.
$$

Keeping the sign convention explicit is essential: using the positive bracket with the same body identification would reverse the Euler evolution. The negative bracket gives

$$
\boxed{\dot{\mathbf M}=\mathbf M\times\boldsymbol\Omega,\qquad\Omega_i=M_i/I_i,\qquad\dot M_1=(I_3^{-1}-I_2^{-1})M_2M_3,}
$$

with cyclic expressions for the other two components. These are the [Euler equations for a torque-free rigid body](../../../classical-mechanics.md#euler-equations-for-a-torque-free-rigid-body). The Hamiltonian and $C$ are conserved because $\boldsymbol\Omega\cdot(\mathbf M\times\boldsymbol\Omega)=0$ and $\mathbf M\cdot(\mathbf M\times\boldsymbol\Omega)=0$. Trajectories therefore lie on intersections of energy ellipsoids with [momentum](../../../classical-mechanics.md#momentum) spheres, the latter being the [symplectic leaves](../../../symplectic-geometry.md#symplectic-leaf).

The body's orientation is reconstructed from $\dot R=R\widehat{\boldsymbol\Omega}$. Its spatial [momentum](../../../classical-mechanics.md#momentum) $\mathbf J=R\mathbf M$ is constant, since $\dot{\mathbf J}=R(\boldsymbol\Omega\times\mathbf M+\mathbf M\times\boldsymbol\Omega)=0$. Thus the body [momentum](../../../classical-mechanics.md#momentum) need not be constant even though the spatial conserved [momentum](../../../classical-mechanics.md#momentum) is. **Poisson reduction retains the dynamics and its [momentum](../../../classical-mechanics.md#momentum) leaves while eliminating orientation variables; the unreduced motion is recovered by reconstruction.**

## 5

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Locality in [quantum theory](../../../quantum-theory.md) is not one interchangeable condition. Spatial concentration of a [wave packet](../../../wave-equation.md#wave-packet) concerns a state description. [Quantum no-signalling](../../../quantum-theory.md#quantum-no-signalling) restricts operational changes of remote statistics. [Microcausality](../../../relativistic-quantum-field.md#microcausality) concerns commutation of spacelike [observable](../../../quantum-mechanics.md#observable) algebras. The [spectrum condition](../../../quantum-field-theory.md#spectrum-condition) constrains energy-momentum and stability, while [primitive causality](../../../quantum-field-theory.md#primitive-causality) concerns determination of future-domain expectations by initial-region data. The distinctions are clearest when all five are discussed; none should be replaced silently by the [Bell factorization](../../../quantum-theory.md#bell-local-causality) examined elsewhere.

**Wave-function tails and entangled correlations are not by themselves controllable signals.** Conversely, absence of signals does not by itself supply a local initial-value dynamics or positive-energy spectrum. Each claim must specify the [observable](../../../quantum-mechanics.md#observable) algebras, allowed operations and relevant causal regions.

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

A free nonrelativistic [Gaussian wave packet](../../../quantum-mechanics.md#gaussian-wave-packet) with initial position variance $\sigma_0^2$ has [wave function](../../../quantum-mechanics.md#wave-function)

$$
\psi(x,0)=(2\pi\sigma_0^2)^{-1/4}e^{-x^2/(4\sigma_0^2)}.
$$

The free dispersion relation $E=p^2/(2m)$ makes its different [momentum](../../../classical-mechanics.md#momentum) components acquire different phases. Fourier evolution gives a position variance

$$
\boxed{\sigma(t)^2=\sigma_0^2\left[1+\left(\frac{\hbar t}{2m\sigma_0^2}\right)^2\right].}
$$

This spreading is ordinary unitary dynamics. A Gaussian already has nonzero tails initially, so its width increase alone is not an example of information suddenly appearing outside an initially compact support.

For genuinely compactly supported nonzero initial data, the nonrelativistic free kernel yields

$$
\psi(x,t)=\sqrt{\frac{m}{2\pi i\hbar t}}e^{imx^2/(2\hbar t)}\int e^{-imxy/(\hbar t)}e^{imy^2/(2\hbar t)}\psi(y,0)\,dy.
$$

At $t\ne0$, the integral is an entire Fourier transform of a compactly supported function. It cannot vanish on an open exterior interval unless the whole transform, and hence the initial state, vanishes. Thus this theory has no strict finite propagation cone for nonzero compact initial [wave functions](../../../quantum-mechanics.md#wave-function). It is a nonrelativistic theory, so that result is not a contradiction in a fundamental relativistic field theory.

Positive-energy relativistic particle descriptions raise a subtler issue. The [Hegerfeldt theorem](../../../quantum-mechanics.md#hegerfeldt-theorem) concerns a Hamiltonian bounded below and a positive localization effect $A$. The function $p_A(t)=\|A^{1/2}e^{-iHt}\psi\|^2$ either vanishes identically or is nonzero for almost every time. Vanishing for an open interval makes the analytic continuation of the vector matrix elements vanish identically. A sharp exterior localization probability which remains zero for a nonzero time interval but becomes positive later is therefore incompatible with those assumptions.

The conclusion restricts simultaneous assumptions about positive energy and sharp particle localization. It does not establish an admissible procedure for controllable superluminal messaging. A particle-position projection need not belong to the algebra of a physically local relativistic measurement, and strictly localized one-particle preparation can fail the required assumptions. In field theory the appropriate locality test concerns [local operations](../../../quantum-measurement.md#local-quantum-operation) and [observables](../../../quantum-mechanics.md#observable), not merely pointwise values of a one-particle [wave function](../../../quantum-mechanics.md#wave-function). **Localization, propagation of field disturbances and transmission of information must be distinguished.**

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

For a bipartite state $\rho_{AB}$, let a [local operation](../../../quantum-measurement.md#local-quantum-operation) on A have [Kraus operators](../../../quantum-information-theory.md#kraus-operator) $M_\alpha$ satisfying $\sum_\alpha M_\alpha^\dagger M_\alpha=I$. Without selecting its outcome, the state becomes

$$
\rho'_{AB}=\sum_\alpha(M_\alpha\otimes I)\rho_{AB}(M_\alpha^\dagger\otimes I).
$$

For every remote [observable](../../../quantum-mechanics.md#observable) $B$, cyclicity of the trace gives

$$
\operatorname{tr}[\rho'_{AB}(I\otimes B)]=\operatorname{tr}\left[\rho_{AB}\left(\sum_\alpha M_\alpha^\dagger M_\alpha\otimes B\right)\right]=\operatorname{tr}[\rho_{AB}(I\otimes B)].
$$

Therefore the remote [partial trace](../../../quantum-theory.md#partial-trace) is unchanged:

$$
\boxed{\rho'_B=\rho_B.}
$$

This proves [quantum no-signalling](../../../quantum-theory.md#quantum-no-signalling) for local trace-preserving [quantum channels](../../../quantum-information-theory.md#quantum-channel), including choices between different such operations. It makes no assumption that $\rho_{AB}$ is separable.

Conditioning on one outcome instead uses an unnormalized state with only that outcome's [Kraus operators](../../../quantum-information-theory.md#kraus-operator) and then divides by its probability. Its remote conditional state can change, yielding quantum steering. However, the outcome cannot be selected deterministically by choosing the measurement setting, and the remote observer needs an ordinary message identifying the selected ensemble. Ignoring the outcome restores the unchanged marginal. [No-signalling](../../../quantum-theory.md#quantum-no-signalling) thus concerns operationally accessible unconditional statistics, not equality of every conditional probability.

The proof presupposes that the intervention is genuinely confined to A and is trace-preserving when outcomes are ignored. A nonlocal operation or setting-dependent postselection does not meet those premises. In field theory local algebras need not come with a simple finite-dimensional tensor factorization; the corresponding statement is expressed using commuting local algebras and [local operations](../../../quantum-measurement.md#local-quantum-operation), as below.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

In [algebraic quantum field theory](../../../quantum-field-theory.md#algebraic-quantum-field-theory), regions carry [observable](../../../quantum-mechanics.md#observable) algebras $\mathcal A(O)$. [Microcausality](../../../relativistic-quantum-field.md#microcausality) requires

$$
\boxed{[A,B]=0\quad\text{if }A\in\mathcal A(O_1),\ B\in\mathcal A(O_2),\ O_1\text{ and }O_2\text{ are spacelike separated}.}
$$

Field operators are usually distributions, so the corresponding formula uses fields smeared with test functions of spacelike-separated support. Fermionic fields obey graded locality, while their physical even [observables](../../../quantum-mechanics.md#observable) commute. This separates the physical [observable](../../../quantum-mechanics.md#observable) condition from an unqualified demand that all fields commute.

For a free Klein–Gordon field, the commutator is proportional to the difference of retarded and advanced fundamental solutions. Their causal support makes this commutator vanish outside the [light cone](../../../special-relativity.md#light-cone). Vacuum two-point correlations can nevertheless be nonzero at spacelike separation: the condition concerns the commutator, not the expectation of a product or statistical independence of outcomes.

To see its operational relevance, take local [Kraus operators](../../../quantum-information-theory.md#kraus-operator) $M_\alpha\in\mathcal A(O_1)$ with $\sum_\alpha M_\alpha^\dagger M_\alpha=I$. For a remote $B\in\mathcal A(O_2)$ the dual operation satisfies

$$
\sum_\alpha M_\alpha^\dagger B M_\alpha=B\sum_\alpha M_\alpha^\dagger M_\alpha=B.
$$

Thus such a local unselected operation changes no remote expectation in any state, proving an algebraic [no-signalling](../../../quantum-theory.md#quantum-no-signalling) result without assuming a tensor-product decomposition of the local algebras. The allowed measurement operations must actually be local; calling an arbitrary ideal projector a measurement is not enough.

**Spacelike commutation allows [entanglement](../../../bell-state.md#entangled-state) and Bell-inequality violation while preventing signalling by these [local operations](../../../quantum-measurement.md#local-quantum-operation).** It is a kinematic algebraic condition. An additional dynamical condition is needed to say that initial-region data determine fields in the [domain of dependence](../../../partial-differential-equation.md#domain-of-dependence).

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

For translations represented by $U(a)=e^{ia_\mu P^\mu}$, the energy-momentum generators have a joint spectral measure. The [spectrum condition](../../../quantum-field-theory.md#spectrum-condition) is

$$
\boxed{\operatorname{Sp}(P)\subseteq\overline V_+=\{p:p^0\ge0,\ p_\mu p^\mu\ge0\},}
$$

using signature $(+,-,-,-)$. It excludes negative-energy and spacelike [momentum](../../../classical-mechanics.md#momentum) states in the vacuum representation, apart from the allowed zero [momentum](../../../classical-mechanics.md#momentum) of the vacuum. It is stronger than bounding the Hamiltonian below in just one chosen frame: energy is nonnegative in every future-directed inertial frame. Thermal infinite-system representations need not satisfy the same vacuum [spectrum condition](../../../quantum-field-theory.md#spectrum-condition), so the representation matters.

The condition supports stability and controls analyticity. For a translation-invariant vacuum, insertion of the spectral measure into a two-point function gives a form

$$
W(x)=\langle\Omega|\phi(x)\phi(0)|\Omega\rangle=\int_{\overline V_+}e^{-ip\cdot x}\,d\mu(p).
$$

Replacing $x$ by $x-iy$, with $y$ in the future timelike cone, inserts the decaying factor $e^{-p\cdot y}$ and gives analytic continuation into the appropriate tube, subject to the usual distributional bounds. This is a consequence of spectral support, not an assertion of compact spatial support of $W$.

Positive energy is not a commutator condition or a guarantee of finite-speed particle-position propagation. It supplies none of the region-algebra inclusions used in [primitive causality](../../../quantum-field-theory.md#primitive-causality) by itself. Its tension with sharp localization is precisely why the particle-localization discussion needs separate hypotheses. **Spectrum, spacelike commutation and operational [no-signalling](../../../quantum-theory.md#quantum-no-signalling) constrain different structures and cannot simply substitute for one another.**

<h3 id="5/v">v</h3>

↑ **Parent:** [5](#5)

<h4 id="5/v/solution">Solution</h4>

↑ **Parent:** [V](#5/v)

[Primitive causality](../../../quantum-field-theory.md#primitive-causality) is an initial-region completeness requirement. A state's full restriction to a suitable region $O$ determines expectations of [observables](../../../quantum-mechanics.md#observable) in its future [domain of dependence](../../../partial-differential-equation.md#domain-of-dependence). The [domain of dependence](../../../partial-differential-equation.md#domain-of-dependence) is not the whole causal future: it contains points whose past-inextendible causal curves all meet the specified initial data region. Merely being reachable by one causal curve from $O$ is not enough.

A standard local [time-slice axiom](../../../quantum-field-theory.md#time-slice-axiom) makes this precise when $O$ contains a neighbourhood of a [Cauchy slice](../../../general-relativity.md#cauchy-surface) of its causal development:

$$
\boxed{\mathcal A(O)=\mathcal A(D(O)),\qquad\mathcal A(D^+(O))\subseteq\mathcal A(O),}
$$

with the regions and algebra identifications understood in the specified local net. Definitions applying [primitive causality](../../../quantum-field-theory.md#primitive-causality) to all bounded open regions can be stronger than a time-slice property stated only for suitable causally convex Cauchy neighbourhoods; these formulations should not be conflated without extra hypotheses.

For a local hyperbolic Klein–Gordon equation, a later field is determined by the field and its normal derivative, or [canonical momentum](../../../classical-mechanics.md#canonical-momentum), on a [Cauchy slice](../../../general-relativity.md#cauchy-surface). Its value can be written using the causal fundamental solution, with integration supported where the past [light cone](../../../special-relativity.md#light-cone) meets the initial slice. If that support lies in the initial patch, the later smeared field is generated by the patch's initial field and [momentum](../../../classical-mechanics.md#momentum) operators. Their algebra therefore generates the [observables](../../../quantum-mechanics.md#observable) of the patch's [domain of dependence](../../../partial-differential-equation.md#domain-of-dependence). This is the local differential-equation mechanism behind the time-slice property.

The required information is the entire restricted [quantum state](../../../quantum-mechanics.md#quantum-state): it assigns expectations to every [observable](../../../quantum-mechanics.md#observable) and product in the initial algebra. Mean values of the initial field and [momentum](../../../classical-mechanics.md#momentum) alone do not determine their fluctuations or higher correlations and thus are insufficient. Knowledge of the restricted state fixes later [probability distributions](../../../probability-theory.md#probability-distribution) and correlations; it does not fix which individual outcome a future measurement will produce.

Finally, [primitive causality](../../../quantum-field-theory.md#primitive-causality) concerns propagation of information already encoded in initial data, while [microcausality](../../../relativistic-quantum-field.md#microcausality) controls compatibility of spacelike measurements and [quantum no-signalling](../../../quantum-theory.md#quantum-no-signalling) controls possible interventions. The [spectrum condition](../../../quantum-field-theory.md#spectrum-condition) adds a separate positivity restriction. **A causal initial-value evolution, positive energy and [no-signalling](../../../quantum-theory.md#quantum-no-signalling) are complementary requirements, not equivalent definitions of quantum locality.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
