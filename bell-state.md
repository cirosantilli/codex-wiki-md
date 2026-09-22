# Bell state

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bell_state)

The four Bell states form an orthonormal maximally entangled basis for two qubits.

**Table of contents**

- [Local flag correction of a Bell-state phase mixture](#local-flag-correction-of-a-bell-state-phase-mixture)
- [Bell pair](#bell-pair)
- [Dephased Bell-state mixture](#dephased-bell-state-mixture)
- [Bell-basis measurement](#bell-basis-measurement)
  - [Bell-state nondemolition measurement](#bell-state-nondemolition-measurement)
- [Superdense coding](#superdense-coding)
- [Spin singlet state](#spin-singlet-state)
  - [Collective-unitary covariance of the two-qubit singlet](#collective-unitary-covariance-of-the-two-qubit-singlet)
- [Reduced density matrix](#reduced-density-matrix)
  - [No-communication theorem](#no-communication-theorem)
    - [Remote state invariance under a local trace-preserving operation](#remote-state-invariance-under-a-local-trace-preserving-operation)
  - [Product state](#product-state)
    - [Two-qubit product-state determinant criterion](#two-qubit-product-state-determinant-criterion)
  - [Entangled state](#entangled-state)
    - [Entanglement distillation](#entanglement-distillation)
    - [Entanglement dilution](#entanglement-dilution)
      - [Exact dilution obstruction from Schmidt rank](#exact-dilution-obstruction-from-schmidt-rank)
      - [Deterministic two-qubit entanglement dilution](#deterministic-two-qubit-entanglement-dilution)
    - [Entanglement monotone](#entanglement-monotone)
      - [Relative entropy of entanglement](#relative-entropy-of-entanglement)
      - [Schmidt-tail entanglement monotone](#schmidt-tail-entanglement-monotone)
    - [Concurrence](#concurrence)
      - [Mixed-state concurrence of two qubits](#mixed-state-concurrence-of-two-qubits)
        - [Concurrence scaling under invertible local filters](#concurrence-scaling-under-invertible-local-filters)
    - [Entanglement criterion for a two-term correlated state](#entanglement-criterion-for-a-two-term-correlated-state)
    - [Entanglement concentration](#entanglement-concentration)
      - [Schmidt projection entanglement concentration](#schmidt-projection-entanglement-concentration)
        - [Tripartite Schmidt projection entanglement concentration](#tripartite-schmidt-projection-entanglement-concentration)
  - [Local indistinguishability of Bell-state phase](#local-indistinguishability-of-bell-state-phase)
- [Local operations and classical communication](#local-operations-and-classical-communication)
  - [Two-outcome LOCC dilution of a Bell pair](#two-outcome-locc-dilution-of-a-bell-pair)
  - [Deterministic reduction of maximally entangled Schmidt rank](#deterministic-reduction-of-maximally-entangled-schmidt-rank)
  - [Asymptotic pure-state entanglement conversion rate](#asymptotic-pure-state-entanglement-conversion-rate)
    - [Collective advantage over independent two-qubit filtering](#collective-advantage-over-independent-two-qubit-filtering)
  - [Optimal stochastic conversion of a two-qubit pure state](#optimal-stochastic-conversion-of-a-two-qubit-pure-state)
  - [Local unitary operation](#local-unitary-operation)
    - [Local-unitary invariance of reduced-state spectra](#local-unitary-invariance-of-reduced-state-spectra)
  - [Nielsen's pure-state conversion theorem](#nielsen-s-pure-state-conversion-theorem)
  - [LOCC discrimination of two Bell states](#locc-discrimination-of-two-bell-states)
  - [Quantum teleportation](#quantum-teleportation)
    - [Dicke-resource telecloning](#dicke-resource-telecloning)
    - [Exact teleportation resource criterion](#exact-teleportation-resource-criterion)
    - [Entanglement swapping](#entanglement-swapping)
    - [Qudit teleportation](#qudit-teleportation)
    - [Teleportation as an identity channel on a reference](#teleportation-as-an-identity-channel-on-a-reference)
    - [One-bit teleportation](#one-bit-teleportation)
      - [Pauli-frame propagation along a measurement wire](#pauli-frame-propagation-along-a-measurement-wire)
      - [Graph-state preparation of a computational-basis input](#graph-state-preparation-of-a-computational-basis-input)
      - [Heralded Pauli X correction using controlled-Z and measurements](#heralded-pauli-x-correction-using-controlled-z-and-measurements)
      - [J gate in measurement-based quantum computation](#j-gate-in-measurement-based-quantum-computation)
        - [J-gate phase-error operator norm](#j-gate-phase-error-operator-norm)
    - [Bell-basis teleportation identity](#bell-basis-teleportation-identity)
    - [No-programming theorem](#no-programming-theorem)
    - [Teleportation with the psi-plus Bell state](#teleportation-with-the-psi-plus-bell-state)
- [Quantum dense coding](#quantum-dense-coding)

## Local flag correction of a Bell-state phase mixture

↑ **Parent:** [Bell state](bell-state.md)

Suppose Alice holds a classical orthogonal flag $F$ for the phase of a [Bell state](bell-state.md):

$$
\rho_{ABF}=p|\Phi^+\rangle\langle\Phi^+|_{AB}\otimes|0\rangle\langle0|_F+(1-p)|\Phi^-\rangle\langle\Phi^-|_{AB}\otimes|1\rangle\langle1|_F.
$$

Her local controlled phase correction $U=I_{AB}\otimes|0\rangle\langle0|_F+(Z_A\otimes I_B)\otimes|1\rangle\langle1|_F$ maps this to $|\Phi^+\rangle\langle\Phi^+|_{AB}\otimes[p|0\rangle\langle0|+(1-p)|1\rangle\langle1|]_F$. Thus Alice and Bob recover an exact [Bell pair](#bell-pair) without revealing its bit value. Even if Eve knows the flag, [purity decouples a subsystem from its purification](quantum-theory.md#purity-decouples-a-subsystem-from-its-purification), so the corrected pair can supply a private bit. Discarding the flag first can instead yield a [separable quantum state](quantum-information-theory.md#separable-quantum-state), as happens at $p=1/2$.

## Bell pair

↑ **Parent:** [Bell state](bell-state.md)

A Bell pair consists of two [qubits](quantum-mechanics.md#qubit) prepared jointly in a [Bell state](bell-state.md). It is a maximally entangled two-qubit resource with [Schmidt rank](von-neumann-entropy.md#schmidt-rank) two. Two independent [Bell pairs](#bell-pair) have resource [Schmidt rank](von-neumann-entropy.md#schmidt-rank) four across the same party partition.

## Dephased Bell-state mixture

↑ **Parent:** [Bell state](bell-state.md)

For real $-1\leq\alpha\leq1$, this two-[qubit](quantum-mechanics.md#qubit) [density operator](quantum-theory.md#density-matrix) has equal $00$ and $11$ populations and off-diagonal coherences $\alpha/2$. It is a [pure state](quantum-theory.md#pure-state) exactly when $\alpha=\pm1$, and a [separable quantum state](quantum-information-theory.md#separable-quantum-state) exactly when $\alpha=0$. Its [partial transpose](quantum-information-theory.md#partial-transpose) has [eigenvalues](linear-operator-theory.md#eigenvalue) $1/2,1/2,\alpha/2,-\alpha/2$, directly witnessing entanglement for every nonzero admissible coherence.

## Bell-basis measurement

↑ **Parent:** [Bell state](bell-state.md)

A Bell-basis measurement is the four-outcome projective measurement whose projectors are onto the four [Bell states](bell-state.md). It jointly measures two qubits and is the sender's measurement in [quantum teleportation](#quantum-teleportation).

### Bell-state nondemolition measurement

↑ **Parent:** [Bell-basis measurement](#bell-basis-measurement)

The [Bell states](bell-state.md) are joint [eigenstates](quantum-mechanics.md#eigenstate) of commuting $Z_AZ_B$ and $X_AX_B$. Two shared [Bell state](bell-state.md) meter pairs realize their two [entanglement-assisted nondemolition parity measurements](quantum-measurement.md#entanglement-assisted-nondemolition-parity-measurement) using spacelike local circuits. Their projector products give the four rank-one [Bell state](bell-state.md) outcomes and preserve each input [Bell state](bell-state.md). The globally identified outcome requires later [local operations and classical communication](#local-operations-and-classical-communication).

## Superdense coding

↑ **Parent:** [Bell state](bell-state.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Superdense_coding)

Superdense coding uses a shared [Bell state](bell-state.md) to communicate two classical bits by transmitting one qubit. The sender selects one of the four Bell states with a local [Pauli operation](algebra.md#pauli-matrices), and the receiver performs a Bell-basis measurement.

## Spin singlet state

↑ **Parent:** [Bell state](bell-state.md)

The two-spin singlet is

$$
|\Psi^-\rangle=\frac{|01\rangle-|10\rangle}{\sqrt2}.
$$

Spin measurements along axes $\mathbf a$ and $\mathbf b$ have correlation $E(\mathbf a,\mathbf b)=-\mathbf a\cdot\mathbf b$, and equal axes give perfect anticorrelation.

This is the [spin-one-half singlet state](quantum-mechanics.md#spin-one-half-singlet-state), an example of an [angular momentum singlet state](quantum-mechanics.md#singlet-state). The general singlet condition is zero total angular momentum, not the choice of a particular two-qubit Bell basis.

### Collective-unitary covariance of the two-qubit singlet

↑ **Parent:** [Spin singlet state](#spin-singlet-state)

For $|s\rangle=(|01\rangle-|10\rangle)/\sqrt2$ and any two-by-two [unitary matrix](linear-operator-theory.md#unitary-matrix), expand the two columns of $U$. The equal-index coefficients cancel, and the coefficient of $|01\rangle-|10\rangle$ is the determinant. Its modulus is one, so a common change of qubit basis preserves the [spin singlet state](#spin-singlet-state) up to a [global phase](quantum-mechanics.md#global-phase). The density projector is exactly invariant.

## Reduced density matrix

↑ **Parent:** [Bell state](bell-state.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduced_density_matrix)

For a bipartite density operator $\rho_{AB}$, the reduced state of subsystem $A$ is the partial trace $\rho_A=\operatorname{Tr}_B\rho_{AB}$. Every measurement performed only on $A$ has outcome probabilities determined entirely by $\rho_A$.

### No-communication theorem

↑ **Parent:** [Reduced density matrix](#reduced-density-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/No-communication_theorem)

A trace-preserving operation on subsystem $B$ cannot change the [reduced density matrix](#reduced-density-matrix) of a disjoint subsystem $A$ when its unobserved outcomes are averaged. Local measurements on $A$ therefore cannot reveal which operation was chosen on $B$.

#### Remote state invariance under a local trace-preserving operation

↑ **Parent:** [No-communication theorem](#no-communication-theorem)

For local [Kraus operators](quantum-information-theory.md#kraus-operator) $A_i$ with $\sum_iA_i^\dagger A_i=I$, let $\rho'_{AB}=\sum_i(A_i\otimes I)\rho_{AB}(A_i^\dagger\otimes I)$. For every remote operator $B$, cyclicity of the [trace](linear-algebra.md#matrix-trace) gives $\operatorname{Tr}[(I\otimes B)\rho'_{AB}]=\sum_i\operatorname{Tr}[(A_i^\dagger A_i\otimes B)\rho_{AB}]=\operatorname{Tr}[(I\otimes B)\rho_{AB}]$. Hence the remote [reduced density matrix](#reduced-density-matrix) is unchanged. In particular every remote [POVM](quantum-measurement.md#positive-operator-valued-measure) has the same outcome probabilities, proving the [no-communication theorem](#no-communication-theorem) from the measurement rule rather than assuming it as a physical postulate.

### Product state

↑ **Parent:** [Reduced density matrix](#reduced-density-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Product_state)

A bipartite [density operator](quantum-theory.md#density-matrix) is a product state when it factors as $\rho_A\otimes\rho_B$. A pure product state factors as $|\psi_A\rangle\otimes|\psi_B\rangle$; its [reduced density matrices](#reduced-density-matrix) have rank one and zero [entanglement entropy](von-neumann-entropy.md#entanglement-entropy). Mixed product states can have nonzero marginal [Von Neumann entropy](von-neumann-entropy.md).

#### Two-qubit product-state determinant criterion

↑ **Parent:** [Product state](#product-state)

Write a two-qubit pure state as $\sum_{i,j=0}^1c_{ij}|ij\rangle$ and form its coefficient matrix $C=(c_{ij})$. The state is a [product state](#product-state) exactly when $C$ has rank one, equivalently when

$$
c_{00}c_{11}=c_{01}c_{10}.
$$

### Entangled state

↑ **Parent:** [Reduced density matrix](#reduced-density-matrix)

A bipartite [density operator](quantum-theory.md#density-matrix) is entangled when it is not a [separable quantum state](quantum-information-theory.md#separable-quantum-state). For a pure state, this is equivalent to not being a [product state](#product-state), or to either [reduced density matrix](#reduced-density-matrix) having rank greater than one.

#### Entanglement distillation

↑ **Parent:** [Entangled state](#entangled-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entanglement_distillation)

Entanglement distillation uses [local operations and classical communication](#local-operations-and-classical-communication) on many noisy [entangled states](#entangled-state) to produce fewer high-fidelity [Bell pairs](#bell-pair). It is also called entanglement purification. The protocol may fail or abort; naming a purification step does not guarantee successful output for arbitrary inputs. If the output is an exact [pure state](quantum-theory.md#pure-state) of [Bell pairs](#bell-pair), every [purification of a density operator](quantum-theory.md#purification-of-a-density-operator) factors between those pairs and the environment, so measuring each pair in the [computational basis](quantum-theory.md#computational-basis) gives a shared uniform bit independent of an eavesdropper. Approximate privacy follows when the entire retained output is sufficiently close to that pure target. A [separable quantum state](quantum-information-theory.md#separable-quantum-state) cannot be distilled into a [Bell pair](#bell-pair) by [LOCC](#local-operations-and-classical-communication), because each local branch preserves separability.

#### Entanglement dilution

↑ **Parent:** [Entangled state](#entangled-state)

Entanglement dilution uses [local operations and classical communication](#local-operations-and-classical-communication) to prepare partially entangled states from [maximally entangled states](quantum-theory.md#maximally-entangled-state), such as [Bell pairs](#bell-pair). For many identical bipartite pure targets, the asymptotic cost in Bell pairs per target, allowing a vanishing approximation error, is their [entanglement entropy](von-neumann-entropy.md#entanglement-entropy) in bits. The [quantum typical subspace](quantum-information-theory.md#quantum-typical-subspace) of the target's [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) has almost all its weight and dimension at most $2^{m(S+\delta)}$. A maximally entangled state of this dimension can be converted to the normalized truncated target by [Nielsen's pure-state conversion theorem](#nielsen-s-pure-state-conversion-theorem). The resulting state approaches the full target as the retained weight tends to one. [Average monotonicity of pure-state entanglement entropy](von-neumann-entropy.md#average-monotonicity-of-pure-state-entanglement-entropy) and entropy continuity give the converse lower bound. This is the reverse asymptotic task to [entanglement concentration](#entanglement-concentration).

##### Exact dilution obstruction from Schmidt rank

↑ **Parent:** [Entanglement dilution](#entanglement-dilution)

For $0<p<1$, every bipartition of $\Psi_p^{\otimes n}$ has [Schmidt rank](von-neumann-entropy.md#schmidt-rank) $2^n$, while $m$ copies of a [GHZ state](quantum-theory.md#greenberger-horne-zeilinger-state) have [Schmidt rank](von-neumann-entropy.md#schmidt-rank) $2^m$. [Schmidt-rank contraction under product operators](von-neumann-entropy.md#schmidt-rank-contraction-under-product-operators) therefore forbids any exact successful [LOCC](#local-operations-and-classical-communication) branch when $m<n$. Approximate [entanglement dilution](#entanglement-dilution) avoids this obstruction by retaining only a high-weight [quantum typical subspace](quantum-information-theory.md#quantum-typical-subspace), whose dimension has logarithm $nh_2(p)+o(n)$. Exact finite-block conversion and asymptotically faithful conversion are different tasks.

##### Deterministic two-qubit entanglement dilution

↑ **Parent:** [Entanglement dilution](#entanglement-dilution)

For nonnegative $u,v$ with $u^2+v^2=1$, Alice applies [Kraus operators](quantum-information-theory.md#kraus-operator) $M_0=\operatorname{diag}(u,v)$ and $M_1=\operatorname{diag}(v,u)$ to one half of a [Bell state](bell-state.md). Their squared effects sum to the identity, and both outcomes have probability one half. The first branch is the target; the second becomes the target after both parties apply [Pauli X gates](quantum-theory.md#pauli-x-gate). Sending the outcome by [classical communication](quantum-information-theory.md#classical-communication) makes this exact deterministic [entanglement dilution](#entanglement-dilution), rather than a postselected conversion.

#### Entanglement monotone

↑ **Parent:** [Entangled state](#entangled-state)

An entanglement monotone quantifies [entanglement](#entangled-state) without increasing on average under [local operations and classical communication](#local-operations-and-classical-communication). The average is over recorded [measurement in quantum mechanics](quantum-measurement.md) outcomes: individual successful branches can have more entanglement, provided their probabilities compensate for that increase. This distinction makes an entanglement monotone useful for bounding probabilistic state conversion. A pure-state entanglement monotone need only satisfy this inequality on pure input states and pure conditional branches, with local measurement outcomes refined to individual [Kraus operators](quantum-information-theory.md#kraus-operator).

##### Relative entropy of entanglement

↑ **Parent:** [Entanglement monotone](#entanglement-monotone)

The relative entropy of entanglement is the smallest [quantum relative entropy](von-neumann-entropy.md#quantum-relative-entropy) from a [density operator](quantum-theory.md#density-matrix) to a [separable quantum state](quantum-information-theory.md#separable-quantum-state), with the separable set specified for the relevant division into parties. [Nonnegativity of quantum relative entropy](von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy) implies $E_R\geq0$. For a [separable quantum state](quantum-information-theory.md#separable-quantum-state), choosing $\sigma=\rho$ gives $E_R=0$. For finite-dimensional bipartite states, compactness of the separable set and lower semicontinuity of the relative entropy give the converse. The support convention is $D(\rho\|\sigma)=+\infty$ unless $\operatorname{supp}\rho\subseteq\operatorname{supp}\sigma$.

##### Schmidt-tail entanglement monotone

↑ **Parent:** [Entanglement monotone](#entanglement-monotone)

For a bipartite [pure state](quantum-theory.md#pure-state), the squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) are the nonzero [eigenvalues](linear-operator-theory.md#eigenvalue) of either [reduced density matrix](#reduced-density-matrix). Their sum except the largest defines $E_2=1-\lambda_{\max}(\rho_A)$. The largest eigenvalue is a convex function, since $\lambda_{\max}(\rho)=\max_{\|v\|=1}\langle v|\rho|v\rangle$; consequently $E_2$ is concave. If Alice measures locally and records outcome $r$, Bob's conditional reductions satisfy $\sum_r p_r\rho_{B,r}=\rho_B$. Concavity gives $\sum_r p_rE_2(\chi_r)\leq E_2(\chi)$. For Bob's measurements use Alice's unchanged average reduction instead. Iteration proves average monotonicity under [LOCC](#local-operations-and-classical-communication). For [Schmidt rank](von-neumann-entropy.md#schmidt-rank) at most two, $E_2$ is the smaller squared Schmidt coefficient. A conversion succeeding with probability $p$ therefore obeys $pE_2(\phi)\leq E_2(\psi)$, since failure branches contribute nonnegative amounts.

#### Concurrence

↑ **Parent:** [Entangled state](#entangled-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Concurrence)

For a normalized pure state of two qubits with coefficient matrix $C$, the concurrence is $2|\det C|$. It ranges from zero for a [product state](#product-state) to one for a [maximally entangled state](quantum-theory.md#maximally-entangled-state).

##### Mixed-state concurrence of two qubits

↑ **Parent:** [Concurrence](#concurrence)

For a normalized two-[qubit](quantum-mechanics.md#qubit) [pure state](quantum-theory.md#pure-state) with coefficient matrix $M$, [concurrence](#concurrence) is $2|\det M|$. The displayed [convex roof extension](quantum-theory.md#convex-roof-extension) defines its mixed-state version. Combining decompositions proves convexity: $C(\sum_jr_j\rho_j)\leq\sum_jr_jC(\rho_j)$. Every [separable quantum state](quantum-information-theory.md#separable-quantum-state) has a decomposition into product vectors, each with zero determinant, so its concurrence is zero.

###### Concurrence scaling under invertible local filters

↑ **Parent:** [Mixed-state concurrence of two qubits](#mixed-state-concurrence-of-two-qubits)

For $\rho'=(A\otimes B)\rho(A^\dagger\otimes B^\dagger)/p$, with invertible $A,B$, a pure coefficient matrix transforms as $M\mapsto AMB^{\mathsf T}$. Its unnormalized determinant is multiplied by $\det A\det B$. The invertible filter bijects pure decompositions before and after conditioning, with branch weights rescaled by their success probabilities. Taking both infima in the [convex roof extension](quantum-theory.md#convex-roof-extension) gives the displayed exact scaling. If either filter has rank one, the retained state is separable across that party.

#### Entanglement criterion for a two-term correlated state

↑ **Parent:** [Entangled state](#entangled-state)

The state $a|00\rangle+b|11\rangle$ is entangled exactly when $ab\ne0$. Its reduced density matrix has nonzero eigenvalues $|a|^2$ and $|b|^2$.

#### Entanglement concentration

↑ **Parent:** [Entangled state](#entangled-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entanglement_concentration)

Entanglement concentration probabilistically converts partially entangled pure states into fewer maximally entangled states by local operations and classical communication.

##### Schmidt projection entanglement concentration

↑ **Parent:** [Entanglement concentration](#entanglement-concentration)

For $n$ copies of a normalized [pure state](quantum-theory.md#pure-state) $\alpha|00\rangle+\beta|11\rangle$, regroup Alice's and Bob's tensor factors. Alice performs a [projective measurement](quantum-measurement.md#projective-measurement) of the total number $k$ of zeroes, preserving all coherence among strings with that count. The outcome has [binomial distribution](discrete-probability-distribution.md#binomial-distribution)

$$
p_k=\binom nk|\alpha|^{2k}|\beta|^{2(n-k)}.
$$

Each retained string has the same complex amplitude $\alpha^k\beta^{n-k}$, so, up to a common phase, the conditional [quantum state](quantum-mechanics.md#quantum-state) is

$$
|T_k\rangle=\binom nk^{-1/2}\sum_{z(x)=k}|x\rangle_A|x\rangle_B.
$$

Its equal [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) make it a [maximally entangled state](quantum-theory.md#maximally-entangled-state) of [Schmidt rank](von-neumann-entropy.md#schmidt-rank) $\binom nk$. Alice sends the count to Bob. They can relabel the corresponding local [computational basis](quantum-theory.md#computational-basis) strings with local unitary operations, and convert the resulting resource to [Bell pairs](#bell-pair). Measuring the individual bits instead would reveal the entire string and leave a [product state](#product-state).

###### Tripartite Schmidt projection entanglement concentration

↑ **Parent:** [Schmidt projection entanglement concentration](#schmidt-projection-entanglement-concentration)

For $\sqrt p\,|000\rangle+\sqrt{1-p}\,|111\rangle$, a [projective measurement](quantum-measurement.md#projective-measurement) of the number of ones in one party's $n$ local [qubits](quantum-mechanics.md#qubit) gives a common type class of size $d_k=\binom nk$. The conditional [pure state](quantum-theory.md#pure-state) is $d_k^{-1/2}\sum_{|x|=k}|x,x,x\rangle$. It can be converted exactly and deterministically to a uniform common-label state of any dimension $m\leq d_k$: one party measures an $m$-element subset $S$ with [Kraus operator](quantum-information-theory.md#kraus-operator) $\Pi_S/\sqrt{\binom{d_k-1}{m-1}}$, and all parties relabel their common retained labels after receiving $S$. Choosing $m=2^f$ gives $f$ independent [GHZ states](quantum-theory.md#greenberger-horne-zeilinger-state). [Stirling's formula](real-analysis.md#stirling-formula) and the [weak law of large numbers](convergence-of-random-variables.md#weak-law-of-large-numbers) give $f/n\to h_2(p)$ in probability. Measuring every local bit separately would instead destroy the coherence and leave a [product state](#product-state).

### Local indistinguishability of Bell-state phase

↑ **Parent:** [Reduced density matrix](#reduced-density-matrix)

The Bell states $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$ and $|\Phi^-\rangle=(|00\rangle-|11\rangle)/\sqrt2$ both have reduced state $I/2$ on either qubit. No measurement on one qubit alone can distinguish their relative sign.

## Local operations and classical communication

↑ **Parent:** [Bell state](bell-state.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_operations_and_classical_communication)

Local operations and classical communication allow separated parties to measure or transform their own subsystems and exchange ordinary classical messages.

### Two-outcome LOCC dilution of a Bell pair

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

Let $c,s\geq0$ and $c^2+s^2=1$. Starting from the [Bell state](bell-state.md) $(|00\rangle+|11\rangle)/\sqrt2$, Alice applies the [measurement in quantum mechanics](quantum-measurement.md) with [Kraus operators](quantum-information-theory.md#kraus-operator) $M_0,M_1$ displayed above. Completeness follows from $M_0^\dagger M_0+M_1^\dagger M_1=I$. Each outcome has [probability](probability-theory.md#probability) $1/2$. The normalized outputs are $c|00\rangle+s|11\rangle$ and $s|00\rangle+c|11\rangle$. Communicating the outcome allows both parties to apply a [Pauli X gate](quantum-theory.md#pauli-x-gate) in the second branch, making both outputs equal to the first. Thus this [LOCC](#local-operations-and-classical-communication) protocol deterministically converts one [Bell pair](#bell-pair) into any two-[qubit](quantum-mechanics.md#qubit) [pure state](quantum-theory.md#pure-state) with these [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient), after appropriate [local unitary operations](#local-unitary-operation). It includes the [product state](#product-state) endpoint without [postselection](quantum-measurement.md#postselection).

### Deterministic reduction of maximally entangled Schmidt rank

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

Let $|\Phi_d\rangle=d^{-1/2}\sum_{j=0}^{d-1}|j,j\rangle$ and $1\leq m\leq d$. It can be converted deterministically by [LOCC](#local-operations-and-classical-communication) to $|\Phi_m\rangle$. For each $m$-element subset $S$ of the local basis labels, let $\Pi_S$ be its projector and let Alice's [Kraus operator](quantum-information-theory.md#kraus-operator) be $K_S=\Pi_S/\sqrt{\binom{d-1}{m-1}}$. Every label occurs in $\binom{d-1}{m-1}$ subsets, so $\sum_SK_S^\dagger K_S=I$. Each outcome has [probability](probability-theory.md#probability) $m/[d\binom{d-1}{m-1}]=1/\binom dm$ and leaves the [maximally entangled state](quantum-theory.md#maximally-entangled-state) $m^{-1/2}\sum_{j\in S}|j,j\rangle$. Alice reports $S$, and both parties relabel these $m$ basis states to $0,\ldots,m-1$ by [local unitary operations](#local-unitary-operation).

For $d=6$, $m=4$, only three outcomes are needed: partition the six labels into disjoint pairs $T_0,T_1,T_2$ and use $K_r=(I-\Pi_{T_r})/\sqrt2$. Each label is retained twice, proving completeness, and each outcome has [probability](probability-theory.md#probability) $1/3$. Every branch leaves four equal [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient), hence two independent [Bell pairs](#bell-pair) after binary relabelling.

### Asymptotic pure-state entanglement conversion rate

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

For bipartite pure source and target states with positive target [entanglement entropy](von-neumann-entropy.md#entanglement-entropy), the optimal rate of [LOCC](#local-operations-and-classical-communication) conversion with vanishing output error is the ratio of their entanglement entropies. Here vanishing error means that the [trace distance](quantum-theory.md#trace-distance) between the output and $|\phi\rangle\langle\phi|^{\otimes m}$ tends to zero; a recorded failure probability must also tend to zero. [Entanglement concentration](#entanglement-concentration) first provides $nS(\rho_A^\psi)-o(n)$ [Bell pairs](#bell-pair), and [entanglement dilution](#entanglement-dilution) needs $mS(\rho_A^\phi)+o(m)$ such pairs. This achieves the ratio. Conversely, refine the output into pure branches. [Average monotonicity of pure-state entanglement entropy](von-neumann-entropy.md#average-monotonicity-of-pure-state-entanglement-entropy) bounds their average entropy by the input entropy; [continuity bound for quantum conditional entropy](von-neumann-entropy.md#continuity-bound-for-quantum-conditional-entropy), with trivial conditioning, makes the output entropy loss per target tend to zero. This forbids a larger rate. The convention permits approximations for finite blocks: exact deterministic conversion of every finite block can obey stricter [majorization](vector-space.md#majorization) constraints. The reversible concentration construction is given in the [original concentration paper](https://arxiv.org/abs/quant-ph/9511030).

#### Collective advantage over independent two-qubit filtering

↑ **Parent:** [Asymptotic pure-state entanglement conversion rate](#asymptotic-pure-state-entanglement-conversion-rate)

For two-qubit pure states with smaller squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) $s<t$, [optimal stochastic conversion of a two-qubit pure state](#optimal-stochastic-conversion-of-a-two-qubit-pure-state) succeeds independently with probability $s/t$. The [asymptotic pure-state entanglement conversion rate](#asymptotic-pure-state-entanglement-conversion-rate) of collective [LOCC](#local-operations-and-classical-communication) is instead $h_2(s)/h_2(t)$, where $h_2$ is [binary entropy](information-theory.md#binary-entropy). The difference is strict: differentiating gives $\frac{d}{dx}[h_2(x)/x]=\log_2(1-x)/x^2<0$. Hence $h_2(s)/s>h_2(t)/t$. Independent filtering loses entanglement in its product-state failure branches, whereas collective concentration and dilution preserve entanglement asymptotically.

### Optimal stochastic conversion of a two-qubit pure state

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

Write a source and target in [Schmidt decomposition](von-neumann-entropy.md#schmidt-decomposition) with squared coefficients $(1-s,s)$ and $(1-t,t)$, where $0<s,t\leq1/2$. If $s\geq t$, [Nielsen's pure-state conversion theorem](#nielsen-s-pure-state-conversion-theorem) allows deterministic conversion. If $s<t$, the [Schmidt-tail entanglement monotone](#schmidt-tail-entanglement-monotone) gives $p\leq s/t$. Alice attains this bound with a local two-outcome [measurement in quantum mechanics](quantum-measurement.md) whose success [Kraus operator](quantum-information-theory.md#kraus-operator) is $K_s=\operatorname{diag}(\sqrt{s(1-t)/(t(1-s))},1)$ and whose failure operator is $K_f=\operatorname{diag}(\sqrt{1-s(1-t)/(t(1-s))},0)$. They obey $K_s^\dagger K_s+K_f^\dagger K_f=I$. The successful unnormalized state is $\sqrt{s/t}$ times the target, and failure leaves a [product state](#product-state). A classical message tells Bob which branch occurred. Known local changes of Schmidt bases allow the same protocol for arbitrary two-qubit pure states with these coefficients.

### Local unitary operation

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

An operation that applies a [unitary operator](vector-space.md#unitary-operator) to one party's subsystem and the identity to the other is a local unitary operation. Several separated parties may each apply a known unitary, resulting in a product of their local unitaries. Such operations preserve the squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) across the relevant bipartition.

#### Local-unitary invariance of reduced-state spectra

↑ **Parent:** [Local unitary operation](#local-unitary-operation)

Under a product [unitary operator](vector-space.md#unitary-operator) $U_A\otimes U_B$, the [reduced density matrix](#reduced-density-matrix) of $A$ becomes $U_A\rho_AU_A^\dagger$. The unitary on $B$ cancels under the [partial trace](quantum-theory.md#partial-trace). Unitary conjugation preserves [eigenvalues](linear-operator-theory.md#eigenvalue), so the squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) of a bipartite [pure state](quantum-theory.md#pure-state) are unchanged. Conversely, two normalized bipartite pure states with the same squared Schmidt coefficients, including multiplicities and zero padding, have [Schmidt decompositions](von-neumann-entropy.md#schmidt-decomposition) carried into each other by local unitaries mapping their Schmidt bases. Thus reduced-state spectra completely classify bipartite pure states up to local unitary operations.

<h3 id="nielsen-s-pure-state-conversion-theorem">Nielsen's pure-state conversion theorem</h3>

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

An exact deterministic [LOCC](#local-operations-and-classical-communication) conversion of a bipartite pure state to another is possible exactly when the input vector of squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) is majorized by the output vector. Sort the two probability vectors decreasingly and pad with zeros to a common length before applying [majorization](vector-space.md#majorization). A maximally entangled state may therefore be converted to a product state, while the reverse conversion is forbidden. The criterion does not assert conversion by postselection or with a catalyst.

### LOCC discrimination of two Bell states

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

Two parties can distinguish $|\Phi^+\rangle$ from $|\Phi^-\rangle$ by both measuring in the Hadamard basis and comparing outcomes: equal outcomes identify $|\Phi^+\rangle$, while unequal outcomes identify $|\Phi^-\rangle$.

### Quantum teleportation

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_teleportation)

Quantum teleportation transfers an unknown qubit using one shared Bell pair, a Bell-basis measurement by the sender, two classical bits, and a Pauli correction by the receiver.

#### Dicke-resource telecloning

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

For odd $n=2k+1$, a symmetric [quantum teleportation](#quantum-teleportation) resource can encode an unknown [qubit](quantum-mechanics.md#qubit) into $E(\alpha|0\rangle+\beta|1\rangle)=\alpha|D_k^n\rangle+\beta|D_{k+1}^n\rangle$. Begin with $|D_{k+1}^{n+1}\rangle$, apply a [controlled-NOT gate](quantum-theory.md#controlled-not-gate) from the input to the sender's resource qubit, apply a [Pauli X gate](quantum-theory.md#pauli-x-gate) to that resource qubit and a [Hadamard gate](quantum-theory.md#hadamard-gate) to the input, and measure those two qubits. The four unnormalized remaining vectors are $E|\psi\rangle/2$, $EX|\psi\rangle/2$, $EZ|\psi\rangle/2$ and $EXZ|\psi\rangle/2$. Each outcome has probability $1/4$. Since $X^{\otimes n}$ interchanges $|D_k^n\rangle$ and $|D_{k+1}^n\rangle$, and $Z^{\otimes n}$ acts as logical $Z$ up to the common phase $(-1)^k$, local Pauli corrections make the output independent of the result. The [one-qubit reduction of Dicke-state superpositions](quantum-mechanics.md#one-qubit-reduction-of-dicke-state-superpositions) gives

$$
\rho=\frac1n\begin{pmatrix}k+|\alpha|^2&(k+1)\alpha\beta^*\\(k+1)\alpha^*\beta&k+|\beta|^2\end{pmatrix},\qquad \langle\psi|\rho|\psi\rangle=\frac{k+1+2k|\alpha|^2|\beta|^2}{n}.
$$

For $n>1$ this distributes imperfect copies, as required by the [no-cloning theorem](quantum-theory.md#no-cloning-theorem). For $n=1$ it reduces to exact [quantum teleportation](#quantum-teleportation).

#### Exact teleportation resource criterion

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

A shared resource enables deterministic exact transmission of an arbitrary unknown [qubit](quantum-mechanics.md#qubit) using only [local operations and classical communication](#local-operations-and-classical-communication) if and only if it can produce a shared [Bell pair](#bell-pair) deterministically by such operations. Sufficiency follows from [quantum teleportation](#quantum-teleportation). For necessity, prepare a Bell pair locally at the sender and apply the purported transmission protocol to one half: exact identity-channel action leaves a shared Bell pair between the retained reference and the receiver. A separable shared resource cannot satisfy this condition because local operations and classical communication preserve separability.

#### Entanglement swapping

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entanglement_swapping)

Two initial maximally entangled pairs $AB_1$ and $B_2C$ can be turned into an entangled pair $AC$ by a [generalized Bell basis](quantum-theory.md#generalized-bell-basis) measurement on $B_1B_2$, followed by a local correction at an endpoint using its classical label. This is [qudit teleportation](#qudit-teleportation) of $B_1$, including its correlations with $A$, to $C$. The initial two pairs are consumed. Without the classical label, averaging the conditional endpoint states need not leave entanglement.

#### Qudit teleportation

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

A sender and receiver share $n^{-1/2}\sum_j|j j\rangle$. The sender measures the input and their resource half in the [generalized Bell basis](quantum-theory.md#generalized-bell-basis). Outcome $(r,s)$ gives the receiver $X^sZ^{-r}|\chi\rangle/n$, with probability $1/n^2$. After [classical communication](quantum-information-theory.md#classical-communication) of the outcome, the correction $Z^rX^{-s}$ restores the unknown [quantum state](quantum-mechanics.md#quantum-state). The same calculation preserves correlations with a reference, as in [teleportation as an identity channel on a reference](#teleportation-as-an-identity-channel-on-a-reference).

#### Teleportation as an identity channel on a reference

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

Ideal corrected [quantum teleportation](#quantum-teleportation) transfers an input system to the receiver while preserving its entire joint [density operator](quantum-theory.md#density-matrix) with an arbitrary reference. Expand a joint [pure state](quantum-theory.md#pure-state) as $\sum_j|j\rangle|r_j\rangle$. Every teleportation branch acts with the same known correction on each system basis vector and does nothing to the reference vectors; undoing that correction restores the complete sum. Linearity extends the result to mixed states. The sender's measured carrier no longer retains the original reference correlations.

#### One-bit teleportation

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

Apply a [Controlled-Z gate](quantum-theory.md#controlled-z-gate) to input $a|0\rangle+b|1\rangle$ and a fresh $|+\rangle$ [quantum ancilla](quantum-information-theory.md#quantum-ancilla). Measuring the input in the [equatorial qubit measurement](quantum-measurement.md#equatorial-qubit-measurement) basis at angle $\alpha$, with outcome $s$, leaves the unnormalized output

$$
\frac1{\sqrt2}\left(a|+\rangle+(-1)^se^{i\alpha}b|-\rangle\right)=\frac1{\sqrt2}X^sJ(\alpha)|\psi\rangle.
$$

Each branch has [probability](probability-theory.md#probability) $1/2$, independently of the input. The logical output is $J(\alpha)|\psi\rangle$ with known [Pauli frame](quantum-circuit.md#pauli-frame) $X^s$; the input [qubit](quantum-mechanics.md#qubit) has been measured, so this does not clone it.

##### Pauli-frame propagation along a measurement wire

↑ **Parent:** [One-bit teleportation](#one-bit-teleportation)

With [equatorial qubit measurement](quantum-measurement.md#equatorial-qubit-measurement) vectors $(|0\rangle+(-1)^s e^{i\eta}|1\rangle)/\sqrt2$, the gate in [one-bit teleportation](#one-bit-teleportation) is $U(\eta)=H\operatorname{diag}(1,e^{-i\eta})=J(-\eta)$. Direct multiplication gives $U(\eta)Z=XU(\eta)$ and $U(\eta)X=e^{-i\eta}ZU(-\eta)$. Moving a [Pauli frame](quantum-circuit.md#pauli-frame) through this gate therefore exchanges its $X$ and $Z$ exponents and reverses the angle if the old $X$ exponent is one, as displayed up to [global phase](quantum-mechanics.md#global-phase). A measurement outcome $s$ adds a further $X^s$ factor. This calculation supplies adaptive angle choices and the final classical output-bit correction of a linear [cluster state](topological-quantum-matter.md#cluster-state) computation.

##### Graph-state preparation of a computational-basis input

↑ **Parent:** [One-bit teleportation](#one-bit-teleportation)

A two-vertex [graph state](quantum-circuit.md#graph-state) starts with two $|+\rangle$ states joined by a [Controlled-Z gate](quantum-theory.md#controlled-z-gate). Measuring the first vertex in the $X$ basis leaves the second in $X^sH|+\rangle=X^s|0\rangle$, where $s$ is the measurement outcome. Thus a known zero input can be supplied to a measurement wire using only a graph-state resource and a known [Pauli frame](quantum-circuit.md#pauli-frame). This preparation link precedes the links implementing the desired logical [J gate](#j-gate-in-measurement-based-quantum-computation); later measurement angles and output-bit corrections absorb its byproduct.

##### Heralded Pauli X correction using controlled-Z and measurements

↑ **Parent:** [One-bit teleportation](#one-bit-teleportation)

Two angle-zero [one-bit teleportations](#one-bit-teleportation) with outcomes $p,q$ implement $X^qH X^pH=X^qZ^p$ on an arbitrary input, up to [global phase](quantum-mechanics.md#global-phase). A [Controlled-Z gate](quantum-theory.md#controlled-z-gate) with a fixed $|1\rangle$ [quantum ancilla](quantum-information-theory.md#quantum-ancilla) implements $Z$, so $Z^p$ removes the known $Z$ factor. The result is $X^q$ up to phase. With probability one half the desired [Pauli X gate](quantum-theory.md#pauli-x-gate) is applied; otherwise the input is unchanged. Repeating until $q=1$ gives an exact heralded correction with two attempts on average and almost-sure termination. It has no finite worst-case measurement count. A [Pauli frame](quantum-circuit.md#pauli-frame) avoids this repeat-until-success procedure when only logical action or classical output statistics are required.

##### J gate in measurement-based quantum computation

↑ **Parent:** [One-bit teleportation](#one-bit-teleportation)

For the printed equatorial-basis convention,

$$
J(\alpha)=\frac1{\sqrt2}\begin{pmatrix}1&e^{i\alpha}\\1&-e^{i\alpha}\end{pmatrix}=H\operatorname{diag}(1,e^{i\alpha}).
$$

It is the [Hadamard gate](quantum-theory.md#hadamard-gate) after a [phase gate](quantum-theory.md#phase-gate). The identities $J(\alpha)Z=XJ(\alpha)$ and $J(\alpha)X=e^{i\alpha}ZJ(-\alpha)$ follow by multiplying their matrices. For $\alpha=0,\pi/2$ these are [Clifford gates](quantum-circuit.md#clifford-gate). In particular $J(-\pi/2)=XJ(\pi/2)$, permitting a sign change of the measurement angle to be absorbed into a [Pauli frame](quantum-circuit.md#pauli-frame).

###### J-gate phase-error operator norm

↑ **Parent:** [J gate in measurement-based quantum computation](#j-gate-in-measurement-based-quantum-computation)

The [J gate](#j-gate-in-measurement-based-quantum-computation) is $J(\alpha)=HP(\alpha)$, where $P(\alpha)=\operatorname{diag}(1,e^{i\alpha})$: the [phase gate](quantum-theory.md#phase-gate) acts first and the [Hadamard gate](quantum-theory.md#hadamard-gate) acts second. Unitary invariance of the [operator norm](continuous-dual-space.md#operator-norm) reduces its angle error to the single nonzero diagonal difference of the [phase gate](quantum-theory.md#phase-gate). Its norm is $|e^{i\delta}-1|=2|\sin(\delta/2)|\leq|\delta|$. The [quantum circuit gate-error telescoping bound](quantum-circuit.md#quantum-circuit-gate-error-telescoping-bound) then makes an angle tolerance of $\epsilon/k$ sufficient for $k$ such imperfect gates and exact other gates.

#### Bell-basis teleportation identity

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

For $|\beta_{xz}\rangle=(Z^zX^x\otimes I)|\beta_{00}\rangle$, an arbitrary qubit obeys

$$
|\alpha\rangle_C|\beta_{00}\rangle_{AB}
=\frac12\sum_{x,z\in\{0,1\}}
|\beta_{xz}\rangle_{CA}X^xZ^z|\alpha\rangle_B.
$$

A Bell-basis measurement reveals $(x,z)$, after which the receiver applies the inverse Pauli correction.

#### No-programming theorem

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

A deterministic finite-dimensional universal programmable quantum gate cannot implement every unitary exactly: programs for physically distinct unitaries would have to be mutually orthogonal, but a finite-dimensional program register contains only finitely many mutually orthogonal states.

This is a restriction on programmable [quantum circuits](quantum-circuit.md) and their [unitary operators](vector-space.md#unitary-operator), rather than a statement about the existence of classical program descriptions.

#### Teleportation with the psi-plus Bell state

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

When the shared resource is $|\Psi^+\rangle$, Bell outcomes $\Phi^+,\Phi^-,\Psi^+,\Psi^-$ leave the receiver with $X|\alpha\rangle,XZ|\alpha\rangle,|\alpha\rangle,Z|\alpha\rangle$, respectively, up to global phases.

## Quantum dense coding

↑ **Parent:** [Bell state](bell-state.md)

Quantum dense coding uses one shared Bell pair and one transmitted qubit to communicate two classical bits. Alice applies one of four Pauli operators to her qubit, producing four orthogonal Bell states that Bob can distinguish jointly. The transmitted qubit alone is maximally mixed for every message and reveals no information to an interceptor.

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (71)

- [Bell basis](quantum-theory.md#bell-basis)
- [Bell-basis conversion circuit](quantum-theory.md#bell-basis-conversion-circuit)
- [Bell-basis measurement](#bell-basis-measurement)
- [Bell pair](#bell-pair)
- [Bell-state nondemolition measurement](#bell-state-nondemolition-measurement)
- [Bell twirling followed by triplet symmetrization](quantum-theory.md#bell-twirling-followed-by-triplet-symmetrization)
- [Coplanar qubit realization of the chained Bell inequality](quantum-theory.md#coplanar-qubit-realization-of-the-chained-bell-inequality)
- [Deterministic two-qubit entanglement dilution](#deterministic-two-qubit-entanglement-dilution)
- [Entanglement-assisted nondemolition parity measurement](quantum-measurement.md#entanglement-assisted-nondemolition-parity-measurement)
- [Generalized Bell state](quantum-theory.md#generalized-bell-state)
- [Local flag correction of a Bell-state phase mixture](#local-flag-correction-of-a-bell-state-phase-mixture)
- [Localizing a Bell pair from a GHZ state](quantum-theory.md#localizing-a-bell-pair-from-a-ghz-state)
- [LOCC discrimination of four Bell states using two copies](quantum-theory.md#locc-discrimination-of-four-bell-states-using-two-copies)
- [One-bit remote preparation of real qubit states](quantum-information-theory.md#one-bit-remote-preparation-of-real-qubit-states)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-33.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-59.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-59.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-59.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-58.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-50.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53.md#4/a/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53.md#4/a/4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-57.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-57.md#3/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323.md#3/iii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1.md#10d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2.md#15d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#10d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2.md#10c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2.md#10c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2.md#15d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-323.md#1/b/i/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-323.md#4/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1.md#10d/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#10d/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#15d/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-325.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2.md#10d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#15d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#10d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#10d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#10e/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#10e/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-2.md#35a/e/solution)
- [Perfect two-basis discrimination would allow superluminal signalling](quantum-theory.md#perfect-two-basis-discrimination-would-allow-superluminal-signalling)
- [Remote preparation in conjugate bases](quantum-theory.md#remote-preparation-in-conjugate-bases)
- [Superdense coding](#superdense-coding)
- [Two-outcome LOCC dilution of a Bell pair](#two-outcome-locc-dilution-of-a-bell-pair)
- [Two-qubit Werner state](quantum-theory.md#two-qubit-werner-state)
