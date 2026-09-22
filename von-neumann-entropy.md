# Von Neumann entropy

↑ **Parent:** [Density matrix](quantum-theory.md#density-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Von_Neumann_entropy)

The Von Neumann entropy of a density operator is

$$
S(\rho)=-\operatorname{Tr}(\rho\log\rho).
$$

It vanishes for a pure state and measures mixedness and quantum entanglement in reduced states.

**Table of contents**

- [Entropy continuity from Jordan decomposition](#entropy-continuity-from-jordan-decomposition)
- [Entropy of an orthogonal quantum mixture](#entropy-of-an-orthogonal-quantum-mixture)
- [Entropy of a binary diagonal qubit mixture](#entropy-of-a-binary-diagonal-qubit-mixture)
- [Entropy bound from overlap with a pure state](#entropy-bound-from-overlap-with-a-pure-state)
- [Maximum entropy of a quantum state](#maximum-entropy-of-a-quantum-state)
- [Entropy increase under nonselective projective measurement](#entropy-increase-under-nonselective-projective-measurement)
  - [Relative entropy of a pinched state](#relative-entropy-of-a-pinched-state)
- [Entanglement entropy](#entanglement-entropy)
  - [Average monotonicity of pure-state entanglement entropy](#average-monotonicity-of-pure-state-entanglement-entropy)
  - [Schmidt decomposition](#schmidt-decomposition)
    - [Operator Schmidt rank](#operator-schmidt-rank)
      - [Local Kraus rank bound from an entangled resource](#local-kraus-rank-bound-from-an-entangled-resource)
    - [Schmidt-basis Pauli correlation tensor](#schmidt-basis-pauli-correlation-tensor)
    - [Schmidt coefficient](#schmidt-coefficient)
    - [Schmidt rank](#schmidt-rank)
      - [Schmidt-rank contraction under product operators](#schmidt-rank-contraction-under-product-operators)
      - [Monotonicity of Schmidt rank under LOCC](#monotonicity-of-schmidt-rank-under-locc)
      - [Maximally entangled overlap bound from Schmidt rank](#maximally-entangled-overlap-bound-from-schmidt-rank)
  - [Schmidt number](#schmidt-number)
- [Subadditivity of Von Neumann entropy](#subadditivity-of-von-neumann-entropy)
  - [Araki–Lieb inequality](#araki-lieb-inequality)
  - [Strong subadditivity of quantum entropy](#strong-subadditivity-of-quantum-entropy)
    - [Strong subadditivity from relative-entropy monotonicity](#strong-subadditivity-from-relative-entropy-monotonicity)
    - [Weak monotonicity of quantum entropy](#weak-monotonicity-of-quantum-entropy)
- [Concavity of Von Neumann entropy](#concavity-of-von-neumann-entropy)
  - [Strict concavity of Von Neumann entropy](#strict-concavity-of-von-neumann-entropy)
  - [Entropy bounds for a quantum mixture](#entropy-bounds-for-a-quantum-mixture)
  - [Entropy bound for a binary mixture](#entropy-bound-for-a-binary-mixture)
- [Quantum conditional entropy](#quantum-conditional-entropy)
  - [Pure-state negative conditional entropy criterion](#pure-state-negative-conditional-entropy-criterion)
  - [Concavity of quantum conditional entropy](#concavity-of-quantum-conditional-entropy)
  - [Continuity bound for quantum conditional entropy](#continuity-bound-for-quantum-conditional-entropy)
  - [Dimension bound for quantum conditional entropy](#dimension-bound-for-quantum-conditional-entropy)
- [Quantum relative entropy](#quantum-relative-entropy)
  - [Relative entropy of classically flagged states](#relative-entropy-of-classically-flagged-states)
  - [Nonnegativity of quantum relative entropy](#nonnegativity-of-quantum-relative-entropy)
    - [Eigenbasis proof of quantum relative entropy nonnegativity](#eigenbasis-proof-of-quantum-relative-entropy-nonnegativity)
  - [Quantum Pinsker inequality](#quantum-pinsker-inequality)
  - [Donald's identity](#donald-s-identity)
    - [Relative-entropy barycenter of a quantum ensemble](#relative-entropy-barycenter-of-a-quantum-ensemble)
  - [Data-processing inequality for quantum relative entropy](#data-processing-inequality-for-quantum-relative-entropy)
  - [Additivity of quantum relative entropy](#additivity-of-quantum-relative-entropy)
  - [Superadditivity of quantum relative entropy](#superadditivity-of-quantum-relative-entropy)
    - [Multipartite superadditivity of quantum relative entropy](#multipartite-superadditivity-of-quantum-relative-entropy)
      - [Lower asymptotic semicontinuity of quantum relative entropy](#lower-asymptotic-semicontinuity-of-quantum-relative-entropy)
  - [Quantum mutual information](#quantum-mutual-information)
    - [Quantum conditional mutual information](#quantum-conditional-mutual-information)
    - [Data processing for quantum mutual information](#data-processing-for-quantum-mutual-information)
      - [Postselection can increase conditional quantum mutual information](#postselection-can-increase-conditional-quantum-mutual-information)
      - [Mutual-information loss as conditional mutual information](#mutual-information-loss-as-conditional-mutual-information)
    - [Quantum mutual information balance identity](#quantum-mutual-information-balance-identity)
  - [Variational characterization of quantum conditional entropy](#variational-characterization-of-quantum-conditional-entropy)

## Entropy continuity from Jordan decomposition

↑ **Parent:** [Von Neumann entropy](von-neumann-entropy.md)

For [density operators](quantum-theory.md#density-matrix) in dimension $d$, let $\delta=\tfrac12\|\rho-\sigma\|_1$. The positive and negative parts of their difference have the same trace $\delta$. Normalize them as $\tau_+,\tau_-$ and write $(\rho+\delta\tau_-)/(1+\delta)=(\sigma+\delta\tau_+)/(1+\delta)$. Applying the two [entropy bounds for a quantum mixture](#entropy-bounds-for-a-quantum-mixture) to this common state proves the displayed bound. The function $g(\delta)=(1+\delta)h_2(\delta/(1+\delta))$ is increasing and concave, with $g(0)=0$, which also controls average entropy errors in pure-source compression.

## Entropy of an orthogonal quantum mixture

↑ **Parent:** [Von Neumann entropy](von-neumann-entropy.md)

For [density operators](quantum-theory.md#density-matrix) supported on mutually orthogonal subspaces, the eigenvalues of their mixture are $p_i\lambda_{ij}$, where $\lambda_{ij}$ are the eigenvalues of $\rho_i$. Substitution into the definition of [Von Neumann entropy](von-neumann-entropy.md) gives the displayed decomposition into [Shannon entropy](information-theory.md#information-entropy) of the label and the mean entropy within each block. Zero eigenvalues use $0\log0=0$.

## Entropy of a binary diagonal qubit mixture

↑ **Parent:** [Von Neumann entropy](von-neumann-entropy.md)

A mixture of two orthogonal pure qubit states has [Von Neumann entropy](von-neumann-entropy.md) equal to the [binary entropy](information-theory.md#binary-entropy) of its weights. Its entropy difference from the first [pure state](quantum-theory.md#pure-state) is exactly $h_2(u)$ and its [trace distance](quantum-theory.md#trace-distance) from that state is $u$. The elementary bound $-(1-u)\ln(1-u)\leq u$ gives $h_2(u)\leq u\log_2(e/u)$; entropy also never exceeds one bit. For small $u$, the leading term is $u\log_2(1/u)$.

## Entropy bound from overlap with a pure state

↑ **Parent:** [Von Neumann entropy](von-neumann-entropy.md)

If a [density operator](quantum-theory.md#density-matrix) $\sigma$ on an $m\geq2$ dimensional [Hilbert space](hilbert-space.md) has overlap $t=\langle\psi|\sigma|\psi\rangle$ with a fixed [pure state](quantum-theory.md#pure-state), then $S(\sigma)\leq h(t)+(1-t)\log_2(m-1)$. Dephase in a basis containing $|\psi\rangle$ and apply the [entropy bound with one prescribed probability](information-theory.md#entropy-bound-with-one-prescribed-probability). The abstract state bound is attained by $\sigma=t|\psi\rangle\langle\psi|+(1-t)(I-|\psi\rangle\langle\psi|)/(m-1)$.

## Maximum entropy of a quantum state

↑ **Parent:** [Von Neumann entropy](von-neumann-entropy.md)

On a $d$-dimensional [Hilbert space](hilbert-space.md), the [Von Neumann entropy](von-neumann-entropy.md) is maximized uniquely by $I/d$. Indeed, [nonnegativity of quantum relative entropy](#nonnegativity-of-quantum-relative-entropy) gives

$$
0\leq D(\rho\|I/d)=\log_2d-S(\rho),
$$

with equality exactly when $\rho=I/d$.

## Entropy increase under nonselective projective measurement

↑ **Parent:** [Von Neumann entropy](von-neumann-entropy.md)

If $\sigma=\sum_iP_i\rho P_i$ is a [nonselective projective measurement](quantum-measurement.md#nonselective-projective-measurement), then $S(\sigma)\geq S(\rho)$. Equality holds exactly when $\rho$ is already block diagonal in the measurement decomposition, equivalently $[\rho,P_i]=0$ for every $i$.

### Relative entropy of a pinched state

↑ **Parent:** [Entropy increase under nonselective projective measurement](#entropy-increase-under-nonselective-projective-measurement)

The [pinching map](quantum-measurement.md#pinching-map) is self-adjoint for the trace pairing, and $\log\mathcal P(\rho)$ is block diagonal. Thus $\operatorname{Tr}\rho\log\mathcal P(\rho)=\operatorname{Tr}\mathcal P(\rho)\log\mathcal P(\rho)$. The kernel of $\mathcal P(\rho)$ is contained in that of $\rho$, so the relative entropy is finite on its support. Expanding the [quantum relative entropy](#quantum-relative-entropy) gives the displayed identity. Its nonnegativity proves entropy increase, with equality exactly when the original state is already block diagonal.

## Entanglement entropy

↑ **Parent:** [Von Neumann entropy](von-neumann-entropy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entanglement_entropy)

For a bipartite pure state, the entanglement entropy is the Von Neumann entropy of either [reduced density matrix](bell-state.md#reduced-density-matrix). The two reduced states have the same nonzero eigenvalues, so their entropies agree.

### Average monotonicity of pure-state entanglement entropy

↑ **Parent:** [Entanglement entropy](#entanglement-entropy)

For a bipartite [pure state](quantum-theory.md#pure-state), [entanglement entropy](#entanglement-entropy) is the [Von Neumann entropy](von-neumann-entropy.md) of either [reduced density matrix](bell-state.md#reduced-density-matrix). When Alice makes a local measurement with pure conditional branches, Bob's reductions average to his original reduction. [Concavity of Von Neumann entropy](#concavity-of-von-neumann-entropy) therefore gives $\sum_r p_rS(\rho_{B,r})\leq S(\rho_B)$. When Bob measures, apply concavity to Alice's reductions. In each pure branch the two reduced entropies coincide by the [Schmidt decomposition](#schmidt-decomposition). Refining measurement outcomes to individual [Kraus operators](quantum-information-theory.md#kraus-operator) and iterating proves the inequality for arbitrary finite-round [LOCC](bell-state.md#local-operations-and-classical-communication). Discarded local systems can be measured and their outcomes refined as well, so discarding does not evade the bound.

### Schmidt decomposition

↑ **Parent:** [Entanglement entropy](#entanglement-entropy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schmidt_decomposition)

Every finite-dimensional bipartite pure state has a decomposition $|\psi\rangle=\sum_{j=1}^r s_j|a_j\rangle|b_j\rangle$ with positive Schmidt coefficients $s_j$ and orthonormal families on each subsystem.

#### Operator Schmidt rank

↑ **Parent:** [Schmidt decomposition](#schmidt-decomposition)

The operator Schmidt rank of a bipartite [linear operator](vector-space.md#linear-operator) is its shortest expansion as a sum of product [linear operators](vector-space.md#linear-operator). Expanding in local orthonormal operator bases gives a coefficient [matrix](vector-space.md#matrix); its [matrix rank](vector-space.md#matrix-rank) is the [operator Schmidt rank](#operator-schmidt-rank), by a [singular value decomposition](linear-algebra.md#singular-value-decomposition). It is unchanged by invertible local operator-basis changes. A rank-one projector onto a bipartite [pure state](quantum-theory.md#pure-state) of [Schmidt rank](#schmidt-rank) $d$ has [operator Schmidt rank](#operator-schmidt-rank) $d^2$: its expansion contains all $d^2$ independent products of local matrix units.

##### Local Kraus rank bound from an entangled resource

↑ **Parent:** [Operator Schmidt rank](#operator-schmidt-rank)

If two parties share a pure resource of [Schmidt rank](#schmidt-rank) $R$, a fully refined branch of their local operations has [Kraus operator](quantum-information-theory.md#kraus-operator) $K_{\mu\nu}=\sum_{j=1}^R\sqrt{p_j}A_{\mu j}\otimes B_{\nu j}$. Hence its [operator Schmidt rank](#operator-schmidt-rank) is at most $R$. Local ancillas, locally adaptive readouts and refined discarded environments are included in the branch operators. Shared classical randomness only mixes such branches. Classical comparison of records does not increase their [operator Schmidt rank](#operator-schmidt-rank).

#### Schmidt-basis Pauli correlation tensor

↑ **Parent:** [Schmidt decomposition](#schmidt-decomposition)

For the [pure state](quantum-theory.md#pure-state) $\lambda_0|00\rangle+\lambda_1|11\rangle$ with real normalized [Schmidt coefficients](#schmidt-coefficient), the two-body [Pauli correlators](quantum-circuit.md#pauli-correlator) form $T=\operatorname{diag}(s,-s,1)$, $s=2\lambda_0\lambda_1$. Thus arbitrary local axes give $\langle(\mathbf a\cdot\sigma)\otimes(\mathbf b\cdot\sigma)\rangle=s(a_xb_x-a_yb_y)+a_zb_z$. The negative $yy$ component follows from the phases in the [Pauli operators](quantum-circuit.md#pauli-operator).

#### Schmidt coefficient

↑ **Parent:** [Schmidt decomposition](#schmidt-decomposition)

The Schmidt coefficients of a normalized bipartite pure state are the nonnegative numbers $s_j$ in its [Schmidt decomposition](#schmidt-decomposition); they satisfy $\sum_js_j^2=1$ and their squares are the nonzero eigenvalues of either [reduced density matrix](bell-state.md#reduced-density-matrix).

#### Schmidt rank

↑ **Parent:** [Schmidt decomposition](#schmidt-decomposition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schmidt_rank)

The Schmidt rank is the number of nonzero terms in a [Schmidt decomposition](#schmidt-decomposition), equivalently the rank of either [reduced density matrix](bell-state.md#reduced-density-matrix) of a bipartite pure state.

##### Schmidt-rank contraction under product operators

↑ **Parent:** [Schmidt rank](#schmidt-rank)

The coefficient matrix of a bipartite [pure state](quantum-theory.md#pure-state) has rank equal to its [Schmidt rank](#schmidt-rank), by [singular value decomposition](linear-algebra.md#singular-value-decomposition). A local product operation $A\otimes B$ sends it to $AMB^{\mathsf T}$, whose rank cannot increase. A complete classical transcript of an [LOCC](bell-state.md#local-operations-and-classical-communication) protocol still selects one product [Kraus operator](quantum-information-theory.md#kraus-operator), so every nonzero branch obeys the bound. Discarding the transcript gives a mixed output with [Schmidt number](#schmidt-number) at most the initial rank.

##### Monotonicity of Schmidt rank under LOCC

↑ **Parent:** [Schmidt rank](#schmidt-rank)

The [Schmidt rank](#schmidt-rank) of a bipartite pure state cannot increase under local operations, even in a nonzero selected branch. A coefficient matrix $C$ changes under a local product operator to $ACB^T$, whose rank is at most that of $C$. For deterministic exact conversions the same conclusion follows from [Nielsen's pure-state conversion theorem](bell-state.md#nielsen-s-pure-state-conversion-theorem): at the input rank $r$, the majorization inequality forces all output coefficients after $r$ to vanish.

##### Maximally entangled overlap bound from Schmidt rank

↑ **Parent:** [Schmidt rank](#schmidt-rank)

A normalized bipartite [pure state](quantum-theory.md#pure-state) of [Schmidt rank](#schmidt-rank) $r$ has [quantum fidelity](quantum-information-theory.md#fidelity-of-quantum-states) at most $\sqrt{r/d}$ with a fixed [maximally entangled state](quantum-theory.md#maximally-entangled-state) on $d\otimes d$. Its coefficient [matrix](vector-space.md#matrix) has [matrix rank](vector-space.md#matrix-rank) $r$ and [Hilbert-Schmidt norm](compact-operator.md#hilbert-schmidt-norm) one. Its overlap is the [trace](linear-algebra.md#matrix-trace) of that [matrix](vector-space.md#matrix) divided by $\sqrt d$; [trace duality](compact-operator.md#trace-duality) and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bound this by $\sqrt{r/d}$. Uniform [Schmidt coefficients](#schmidt-coefficient) on $r$ matching basis pairs attain equality.

### Schmidt number

↑ **Parent:** [Entanglement entropy](#entanglement-entropy)

The Schmidt number of a mixed bipartite state is the smallest $k$ for which it has a pure-state ensemble whose members all have Schmidt rank at most $k$. Schmidt number one is equivalent to separability.

## Subadditivity of Von Neumann entropy

↑ **Parent:** [Von Neumann entropy](von-neumann-entropy.md)

For a bipartite [density operator](quantum-theory.md#density-matrix) $\rho_{AB}$,

$$
S(\rho_{AB})\leq S(\rho_A)+S(\rho_B).
$$

Equality holds exactly when $\rho_{AB}=\rho_A\otimes\rho_B$.

<h3 id="araki-lieb-inequality">Araki–Lieb inequality</h3>

↑ **Parent:** [Subadditivity of Von Neumann entropy](#subadditivity-of-von-neumann-entropy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Araki–Lieb_inequality)

For a bipartite [density operator](quantum-theory.md#density-matrix) $\rho_{AB}$,

$$
|S(\rho_A)-S(\rho_B)|\leq S(\rho_{AB}).
$$

### Strong subadditivity of quantum entropy

↑ **Parent:** [Subadditivity of Von Neumann entropy](#subadditivity-of-von-neumann-entropy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strong_subadditivity_of_quantum_entropy)

For a tripartite [density operator](quantum-theory.md#density-matrix) $\rho_{ABC}$,

$$
S(\rho_{ABC})+S(\rho_B)\leq S(\rho_{AB})+S(\rho_{BC}).
$$

Equivalently, conditioning on an additional quantum system cannot increase [quantum conditional entropy](#quantum-conditional-entropy).

#### Strong subadditivity from relative-entropy monotonicity

↑ **Parent:** [Strong subadditivity of quantum entropy](#strong-subadditivity-of-quantum-entropy)

Apply [data-processing inequality for quantum relative entropy](#data-processing-inequality-for-quantum-relative-entropy) to $\rho_{ABC}$ and $\rho_A\otimes\rho_{BC}$, tracing out $C$. The resulting comparison is $D(\rho_{ABC}\|\rho_A\otimes\rho_{BC})\geq D(\rho_{AB}\|\rho_A\otimes\rho_B)$. Expand the logarithms of the product marginals to obtain $S(AB)+S(BC)-S(B)-S(ABC)\geq0$, exactly [Strong subadditivity of Von Neumann entropy](#strong-subadditivity-of-quantum-entropy).

#### Weak monotonicity of quantum entropy

↑ **Parent:** [Strong subadditivity of quantum entropy](#strong-subadditivity-of-quantum-entropy)

Every tripartite [density operator](quantum-theory.md#density-matrix) satisfies $S(AC)+S(BC)\geq S(A)+S(B)$. Purify to $ABCD$ and apply [Strong subadditivity of Von Neumann entropy](#strong-subadditivity-of-quantum-entropy) to $ACD$, conditioned on $A$. The [Schmidt decomposition](#schmidt-decomposition) gives $S(AD)=S(BC)$ and $S(ACD)=S(B)$, proving the inequality. The original tripartite state need not be pure.

## Concavity of Von Neumann entropy

↑ **Parent:** [Von Neumann entropy](von-neumann-entropy.md)

For [density operators](quantum-theory.md#density-matrix) $\rho_1,\rho_2$ and $0\leq p\leq1$, [Von Neumann entropy](von-neumann-entropy.md) is [concave](real-analysis.md#concave-function):

$$
S(p\rho_1+(1-p)\rho_2)\geq pS(\rho_1)+(1-p)S(\rho_2).
$$

### Strict concavity of Von Neumann entropy

↑ **Parent:** [Concavity of Von Neumann entropy](#concavity-of-von-neumann-entropy)

For $0<b<1$ and distinct [density operators](quantum-theory.md#density-matrix), the [Von Neumann entropy](von-neumann-entropy.md) of $\rho=b\rho_1+(1-b)\rho_2$ is strictly larger than the corresponding average. The difference is $bD(\rho_1\|\rho)+(1-b)D(\rho_2\|\rho)$, positive by [nonnegativity of quantum relative entropy](#nonnegativity-of-quantum-relative-entropy) unless both states coincide. On the closed interval $0\le b\le1$, equality holds exactly when $b=0$, $b=1$, or $\rho_1=\rho_2$.

### Entropy bounds for a quantum mixture

↑ **Parent:** [Concavity of Von Neumann entropy](#concavity-of-von-neumann-entropy)

For a mixture of [density operators](quantum-theory.md#density-matrix), the lower bound follows from $S(\bar\rho)-\sum_ip_iS(\rho_i)=\sum_ip_iD(\rho_i\|\bar\rho)\geq0$, with equality precisely when all positive-weight states coincide. For the upper bound, resolve each state into pure eigenvectors and form the Gram matrix of the resulting weighted vectors. Its nonzero eigenvalues are those of $\bar\rho$, while its diagonal has probabilities $p_i\lambda_{ia}$. Averaging diagonal unitary conjugations deletes its off-diagonal entries; [Concavity of Von Neumann entropy](#concavity-of-von-neumann-entropy) therefore gives the bound. Equality holds exactly when positive-weight component supports are mutually orthogonal.

### Entropy bound for a binary mixture

↑ **Parent:** [Concavity of Von Neumann entropy](#concavity-of-von-neumann-entropy)

The entropy of a binary mixture also satisfies

$$
S(p\rho_1+(1-p)\rho_2)\leq pS(\rho_1)+(1-p)S(\rho_2)+H(p),
$$

where $H$ is [binary entropy](information-theory.md#binary-entropy). This follows by applying the [operator monotonicity of logarithm](calculus.md#operator-monotonicity-of-logarithm) to $p\rho_1\leq p\rho_1+(1-p)\rho_2$ and its counterpart for $\rho_2$.

## Quantum conditional entropy

↑ **Parent:** [Von Neumann entropy](von-neumann-entropy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_conditional_entropy)

The quantum conditional entropy is $H(A|B)_\rho=S(\rho_{AB})-S(\rho_B)$. Unlike its classical counterpart, it may be negative.

### Pure-state negative conditional entropy criterion

↑ **Parent:** [Quantum conditional entropy](#quantum-conditional-entropy)

For a bipartite [pure state](quantum-theory.md#pure-state) with finite [Von Neumann entropy](von-neumann-entropy.md), the joint [Von Neumann entropy](von-neumann-entropy.md) is zero, so its [quantum conditional entropy](#quantum-conditional-entropy) is $-S(\rho_A)$. The [Schmidt decomposition](#schmidt-decomposition) makes the nonzero [eigenvalues](linear-operator-theory.md#eigenvalue) of $\rho_A$ the squared [Schmidt coefficients](#schmidt-coefficient). Their [Shannon entropy](information-theory.md#information-entropy) vanishes exactly when there is one coefficient, equivalently the joint [pure state](quantum-theory.md#pure-state) is a [product state](bell-state.md#product-state). Thus negative [quantum conditional entropy](#quantum-conditional-entropy) detects exactly the [entangled](bell-state.md#entangled-state) bipartite [pure states](quantum-theory.md#pure-state); it is only a sufficient criterion for [entanglement](bell-state.md#entangled-state) of general mixed [density operators](quantum-theory.md#density-matrix).

### Concavity of quantum conditional entropy

↑ **Parent:** [Quantum conditional entropy](#quantum-conditional-entropy)

For bipartite [density operators](quantum-theory.md#density-matrix),

$$
H(A|B)_{p\rho+(1-p)\sigma}\geq pH(A|B)_\rho+(1-p)H(A|B)_\sigma.
$$

This is a consequence of [Strong subadditivity of Von Neumann entropy](#strong-subadditivity-of-quantum-entropy).

### Continuity bound for quantum conditional entropy

↑ **Parent:** [Quantum conditional entropy](#quantum-conditional-entropy)

If $\varepsilon=\lVert\rho_{AB}-\sigma_{AB}\rVert_1/2$ and $d_A=\dim\mathcal H_A$, then

$$
|H(A|B)_\rho-H(A|B)_\sigma|
\leq2\varepsilon\log d_A+(1+\varepsilon)H\!\left(\frac{\varepsilon}{1+\varepsilon}\right).
$$

The proof couples the two states through their positive and negative differences, then combines [concavity of quantum conditional entropy](#concavity-of-quantum-conditional-entropy) with the [entropy bound for a binary mixture](#entropy-bound-for-a-binary-mixture).

### Dimension bound for quantum conditional entropy

↑ **Parent:** [Quantum conditional entropy](#quantum-conditional-entropy)

For every state on $\mathcal H_A\otimes\mathcal H_B$,

$$
-\log d_A\leq H(A|B)\leq\log d_A.
$$

The upper bound follows from [Subadditivity of Von Neumann entropy](#subadditivity-of-von-neumann-entropy) and the lower bound from the [Araki–Lieb inequality](#araki-lieb-inequality).

## Quantum relative entropy

↑ **Parent:** [Von Neumann entropy](von-neumann-entropy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_relative_entropy)

The quantum relative entropy is $D(\rho\|\sigma)=\operatorname{Tr}[\rho(\log\rho-\log\sigma)]$ when the support of $\rho$ lies in that of $\sigma$.

### Relative entropy of classically flagged states

↑ **Parent:** [Quantum relative entropy](#quantum-relative-entropy)

For common classical weights, the [matrix logarithm](vector-space.md#matrix-logarithm) on each positive-weight block is $\log(p_i\rho_i)=(\log p_i)I+\log\rho_i$ on its support. The two logarithms of $p_i$ cancel in the [quantum relative entropy](#quantum-relative-entropy), giving the displayed identity. Zero-weight blocks are omitted, including if their unweighted relative entropy is infinite. If a positive-weight block violates support inclusion, both sides are infinite. Applying the [data-processing inequality for quantum relative entropy](#data-processing-inequality-for-quantum-relative-entropy) to the [partial trace](quantum-theory.md#partial-trace) over the flag gives [joint convexity of quantum relative entropy](quantum-information-theory.md#joint-convexity-of-quantum-relative-entropy).

### Nonnegativity of quantum relative entropy

↑ **Parent:** [Quantum relative entropy](#quantum-relative-entropy)

For [density operators](quantum-theory.md#density-matrix), [Klein's inequality](vector-space.md#klein-s-inequality) gives $D(\rho\|\sigma)\geq0$, with equality exactly when $\rho=\sigma$. If the [support of a positive operator](hilbert-space.md#support-of-a-positive-operator) $\rho$ is not contained in that of $\sigma$, the [quantum relative entropy](#quantum-relative-entropy) is $+\infty$.

#### Eigenbasis proof of quantum relative entropy nonnegativity

↑ **Parent:** [Nonnegativity of quantum relative entropy](#nonnegativity-of-quantum-relative-entropy)

Diagonalize two [density operators](quantum-theory.md#density-matrix) with eigenvalues $r_i,s_j$, and put $q_{ij}=|\langle i|j\rangle|^2$. This overlap matrix has row and column sums one. The scalar inequality $u\ln(u/v)\ge u-v$ yields $D(\rho\|\sigma)\ge\sum_{ij}q_{ij}(r_i-s_j)=0$ in natural units; division by $\ln2$ gives bits. Equality forces $r_i=s_j$ whenever $q_{ij}>0$, so $\sigma|i\rangle=r_i|i\rangle$ and $\rho=\sigma$. Zero eigenvalues use limits, and failure of support inclusion gives infinite [quantum relative entropy](#quantum-relative-entropy).

### Quantum Pinsker inequality

↑ **Parent:** [Quantum relative entropy](#quantum-relative-entropy)

In bits, the quantum Pinsker inequality is

$$
D(\rho\|\sigma)\geq\frac{2}{\ln2}D(\rho,\sigma)^2.
$$

The [trace-distance-preserving binary measurement](quantum-theory.md#trace-distance-preserving-binary-measurement) converts the [trace distance](quantum-theory.md#trace-distance) into classical [total variation distance](probability-and-statistics.md#total-variation-distance) without loss. Apply the [data-processing inequality for quantum relative entropy](#data-processing-inequality-for-quantum-relative-entropy) to that measurement, then classical [Pinsker's inequality](probability-and-statistics.md#pinsker-s-inequality). The factor $\ln2$ is omitted when relative entropy uses natural [logarithms](calculus.md#logarithm).

<h3 id="donald-s-identity">Donald's identity</h3>

↑ **Parent:** [Quantum relative entropy](#quantum-relative-entropy)

For an ensemble of [density operators](quantum-theory.md#density-matrix) with average $\overline\omega=\sum_jp_j\omega_j$,

$$
\sum_jp_jD(\omega_j\|\rho)
=\sum_jp_jD(\omega_j\|\overline\omega)+D(\overline\omega\|\rho).
$$

Expanding the trace definitions cancels the $\log\omega_j$ terms, and the remaining sum combines to a trace against $\overline\omega$. Positive-weight ensemble states have their support contained in that of the average, so the first sum on the right is finite in finite dimension. If the reference-state support condition fails, both sides are $+\infty$. The identity is associated with [Donald's work on relative entropy](https://www.mjdquantum.uk/otrea.html).

#### Relative-entropy barycenter of a quantum ensemble

↑ **Parent:** [Donald's identity](#donald-s-identity)

The ensemble average $\overline\omega$ uniquely minimizes $\sum_jp_jD(\omega_j\|\rho)$ over [density operators](quantum-theory.md#density-matrix) $\rho$. [Donald's identity](#donald-s-identity) separates this objective into a constant plus $D(\overline\omega\|\rho)$, and [nonnegativity of quantum relative entropy](#nonnegativity-of-quantum-relative-entropy) proves the claim. The minimum is the [Holevo quantity](quantum-information-theory.md#holevo-quantity) $S(\overline\omega)-\sum_jp_jS(\omega_j)$, equivalently the [quantum mutual information](#quantum-mutual-information) of the associated [classical-quantum state](quantum-information-theory.md#classical-quantum-state).

### Data-processing inequality for quantum relative entropy

↑ **Parent:** [Quantum relative entropy](#quantum-relative-entropy)

For every [quantum channel](quantum-information-theory.md#quantum-channel) $T$,

$$
D(T(\rho)\|T(\sigma))\leq D(\rho\|\sigma).
$$

For a [partial trace](quantum-theory.md#partial-trace), this says that discarding a subsystem cannot make two [density operators](quantum-theory.md#density-matrix) more distinguishable in [quantum relative entropy](#quantum-relative-entropy).

### Additivity of quantum relative entropy

↑ **Parent:** [Quantum relative entropy](#quantum-relative-entropy)

The [quantum relative entropy](#quantum-relative-entropy) is additive on [tensor products](linear-algebra.md#tensor-product):

$$
D(\rho_A\otimes\rho_B\|\sigma_A\otimes\sigma_B)
=D(\rho_A\|\sigma_A)+D(\rho_B\|\sigma_B).
$$

This follows by expanding $\log(\sigma_A\otimes\sigma_B)=\log\sigma_A\otimes I+I\otimes\log\sigma_B$ and its counterpart for $\rho$.

### Superadditivity of quantum relative entropy

↑ **Parent:** [Quantum relative entropy](#quantum-relative-entropy)

For a bipartite [density operator](quantum-theory.md#density-matrix) $\rho_{AB}$ and a product reference state,

$$
D(\rho_{AB}\|\sigma_A\otimes\sigma_B)
\geq D(\rho_A\|\sigma_A)+D(\rho_B\|\sigma_B).
$$

The difference between the two sides is the nonnegative [quantum mutual information](#quantum-mutual-information) of $\rho_{AB}$.

#### Multipartite superadditivity of quantum relative entropy

↑ **Parent:** [Superadditivity of quantum relative entropy](#superadditivity-of-quantum-relative-entropy)

Repeated application of [superadditivity of quantum relative entropy](#superadditivity-of-quantum-relative-entropy) gives

$$
D(\rho_{1\ldots n}\|\sigma_1\otimes\cdots\otimes\sigma_n)
\geq\sum_{j=1}^nD(\rho_j\|\sigma_j).
$$

##### Lower asymptotic semicontinuity of quantum relative entropy

↑ **Parent:** [Multipartite superadditivity of quantum relative entropy](#multipartite-superadditivity-of-quantum-relative-entropy)

If $\lVert\rho'_n-\rho^{\otimes n}\rVert_1\to0$, then

$$
\liminf_{n\to\infty}\frac1n
\left(D(\rho'_n\|\sigma^{\otimes n})-D(\rho^{\otimes n}\|\sigma^{\otimes n})\right)\geq0.
$$

In finite dimension this follows from [multipartite superadditivity of quantum relative entropy](#multipartite-superadditivity-of-quantum-relative-entropy), [additivity of quantum relative entropy](#additivity-of-quantum-relative-entropy), contraction of [trace distance](quantum-theory.md#trace-distance) under [partial trace](quantum-theory.md#partial-trace), and [uniform continuity](topological-analysis.md#uniform-continuity) on the compact state space.

### Quantum mutual information

↑ **Parent:** [Quantum relative entropy](#quantum-relative-entropy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_mutual_information)

The quantum mutual information of a bipartite state is

$$
I(A:B)_\rho
=D(\rho_{AB}\|\rho_A\otimes\rho_B)
=S(\rho_A)+S(\rho_B)-S(\rho_{AB}).
$$

Its nonnegativity is equivalent to [Subadditivity of Von Neumann entropy](#subadditivity-of-von-neumann-entropy).

#### Quantum conditional mutual information

↑ **Parent:** [Quantum mutual information](#quantum-mutual-information)

For a tripartite [density operator](quantum-theory.md#density-matrix), the quantum conditional mutual information is $I(A:C|B)=S(AB)+S(BC)-S(B)-S(ABC)$. It is nonnegative by [Strong subadditivity of Von Neumann entropy](#strong-subadditivity-of-quantum-entropy). It measures the [coherent information](quantum-information-theory.md#coherent-information) lost when a channel environment is discarded after an isometric dilation.

#### Data processing for quantum mutual information

↑ **Parent:** [Quantum mutual information](#quantum-mutual-information)

A local [quantum channel](quantum-information-theory.md#quantum-channel) on either subsystem cannot increase [quantum mutual information](#quantum-mutual-information). Indeed, apply the [data-processing inequality for quantum relative entropy](#data-processing-inequality-for-quantum-relative-entropy) to $D(\rho_{AB}\|\rho_A\otimes\rho_B)$; the channel maps the product of marginals to the product of the new marginals.

##### Postselection can increase conditional quantum mutual information

↑ **Parent:** [Data processing for quantum mutual information](#data-processing-for-quantum-mutual-information)

Let a uniformly random bit $A$ be copied into a three-state classical register $B$ with probability $\varepsilon$, and otherwise replaced in $B$ by a flagged erasure independent of $A$. Then $I(A:B)=\varepsilon$ bits. Projecting $B$ onto its two nonerased states and conditioning on success gives a perfectly correlated bit pair with mutual information one. The [postselection](quantum-measurement.md#postselection) branch is completely positive and trace decreasing, but renormalization after conditioning is not a deterministic [quantum channel](quantum-information-theory.md#quantum-channel). This does not contradict [data processing for quantum mutual information](#data-processing-for-quantum-mutual-information), which applies to trace-preserving operations or an unconditioned instrument including its outcome flag.

##### Mutual-information loss as conditional mutual information

↑ **Parent:** [Data processing for quantum mutual information](#data-processing-for-quantum-mutual-information)

For a channel on $B$, use a [Stinespring dilation](quantum-information-theory.md#stinespring-dilation) $B\to B'E$. Isometry invariance gives $I(A:B)=I(A:B'E)$, so the loss on discarding $E$ is $I(A:B)-I(A:B')=I(A:E\mid B')$. This [quantum conditional mutual information](#quantum-conditional-mutual-information) is nonnegative by [Strong subadditivity of Von Neumann entropy](#strong-subadditivity-of-quantum-entropy). The identity holds for arbitrary mixed inputs and identifies the correlations lost to the discarded environment.

#### Quantum mutual information balance identity

↑ **Parent:** [Quantum mutual information](#quantum-mutual-information)

For any tripartite [density operator](quantum-theory.md#density-matrix), expanding the three [quantum mutual information](#quantum-mutual-information) terms in [Von Neumann entropy](von-neumann-entropy.md) gives $I(X:BD)=I(X:B)+I(XB:D)-I(B:D)$. This algebraic identity allows separate bounds on two information contributions, while [nonnegativity of quantum relative entropy](#nonnegativity-of-quantum-relative-entropy) allows the last term to be dropped in an upper bound.

### Variational characterization of quantum conditional entropy

↑ **Parent:** [Quantum relative entropy](#quantum-relative-entropy)

The [quantum conditional entropy](#quantum-conditional-entropy) has the relative-entropy representation

$$
-H(A|B)_\rho=\min_{\xi_B}D(\rho_{AB}\|I_A\otimes\xi_B),
$$

where the minimum ranges over [density operators](quantum-theory.md#density-matrix) on $B$.

## ↑ Ancestors (5)

1. [Density matrix](quantum-theory.md#density-matrix)
2. [Quantum theory](quantum-theory.md)
3. [Branches of physics](physics.md#branches-of-physics)
4. [Physics](physics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (60)

- [Average monotonicity of pure-state entanglement entropy](#average-monotonicity-of-pure-state-entanglement-entropy)
- [Concavity of Von Neumann entropy](#concavity-of-von-neumann-entropy)
- [Entropy of a binary diagonal qubit mixture](#entropy-of-a-binary-diagonal-qubit-mixture)
- [Entropy of a classical-quantum state](quantum-information-theory.md#entropy-of-a-classical-quantum-state)
- [Entropy of an orthogonal quantum mixture](#entropy-of-an-orthogonal-quantum-mixture)
- [Holevo capacity of a qubit depolarizing channel](quantum-information-theory.md#holevo-capacity-of-a-qubit-depolarizing-channel)
- [Linear isometry of Hilbert spaces](hilbert-space.md#linear-isometry-of-hilbert-spaces)
- [Maximum entropy of a quantum state](#maximum-entropy-of-a-quantum-state)
- [Memoryless quantum information source](quantum-information-theory.md#memoryless-quantum-information-source)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-25.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-33.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-33.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-33.md#5/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-33.md#5/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-34.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-34.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-50.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-50.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-50.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-50.md#5/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-65.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#1/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323.md#5/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323.md#2/ii/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#33b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-354.md#2/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-323.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-2.md#35a/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-323.md#4/a/solution)
- [Product-input block bound for a qubit depolarizing channel](quantum-information-theory.md#product-input-block-bound-for-a-qubit-depolarizing-channel)
- [Product state](bell-state.md#product-state)
- [Pure-state negative conditional entropy criterion](#pure-state-negative-conditional-entropy-criterion)
- [Quantum mutual information balance identity](#quantum-mutual-information-balance-identity)
- [Rank-one dephasing](quantum-measurement.md#rank-one-dephasing)
- [Schumacher compression](quantum-information-theory.md#schumacher-compression)
- [Strict concavity of Von Neumann entropy](#strict-concavity-of-von-neumann-entropy)
- [Superadditivity of Holevo capacity](quantum-information-theory.md#superadditivity-of-holevo-capacity)
