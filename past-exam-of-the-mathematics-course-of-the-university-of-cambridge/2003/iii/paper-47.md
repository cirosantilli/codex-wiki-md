# Paper 47

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper47.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper47.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Take the [Hadamard gate](../../../quantum-theory.md#hadamard-gate) to be $H=2^{-1/2}\begin{pmatrix}1&1\\1&-1\end{pmatrix}$ and the [phase gate](../../../quantum-theory.md#phase-gate) to be $P(\phi)=\operatorname{diag}(1,e^{i\phi})$. This fixes the sign convention for the interference phase.

For the coherent [quantum circuit](../../../quantum-circuit.md), the successive [quantum states](../../../quantum-mechanics.md#quantum-state) are

$$
|0\rangle\longmapsto\frac{|0\rangle+|1\rangle}{\sqrt2}
\longmapsto\frac{|0\rangle+e^{i\phi}|1\rangle}{\sqrt2}
\longmapsto\frac{(1+e^{i\phi})|0\rangle+(1-e^{i\phi})|1\rangle}{2}.
$$

The [Born rule](../../../quantum-mechanics.md#born-rule) therefore gives the concise answer

$$
\boxed{P_0(\phi)=\frac{|1+e^{i\phi}|^2}{4}=\frac{1+\cos\phi}{2}=\cos^2(\phi/2).}
$$

With the stated [quantum decoherence](../../../quantum-theory.md#quantum-decoherence) after the [phase gate](../../../quantum-theory.md#phase-gate), the joint [pure state](../../../quantum-theory.md#pure-state) before the last [Hadamard gate](../../../quantum-theory.md#hadamard-gate) is

$$
\frac{|0\rangle|e_0\rangle+e^{i\phi}|1\rangle|e_1\rangle}{\sqrt2}.
$$

After that [Hadamard gate](../../../quantum-theory.md#hadamard-gate), its environment coefficient at output zero is $(|e_0\rangle+e^{i\phi}|e_1\rangle)/2$. Squaring its [norm](../../../functional-analysis.md#norm) sums over every unobserved environment outcome, so

$$
P_0=\frac14\left(2+e^{i\phi}\langle e_0|e_1\rangle+e^{-i\phi}\langle e_1|e_0\rangle\right),\qquad
\boxed{P_0(\phi,v,\alpha)=\frac{1+v\cos(\phi+\alpha)}2.}
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $0\le v\le1$. In this [single-qubit interference with conditional environment states](../../../quantum-theory.md#single-qubit-interference-with-conditional-environment-states), $v$ is the [interference visibility](../../../optics.md#interferometric-visibility): orthogonal environment states erase the fringe, while a unit-modulus overlap shifts its phase without reducing visibility. The plus sign in $\phi+\alpha$ follows from the specified overlap $\langle e_0|e_1\rangle$, rather than its complex conjugate.

If the same [quantum decoherence](../../../quantum-theory.md#quantum-decoherence) occurs before the [phase gate](../../../quantum-theory.md#phase-gate), the joint [pure state](../../../quantum-theory.md#pure-state) is first $(|0\rangle|e_0\rangle+|1\rangle|e_1\rangle)/\sqrt2$. The [phase gate](../../../quantum-theory.md#phase-gate) then produces exactly the same state used above. Equivalently, the controlled environment interaction commutes with the diagonal [phase gate](../../../quantum-theory.md#phase-gate). **The probability is unchanged.**

For the [Deutsch algorithm](../../../quantum-theory.md#deutsch-algorithm), use the reversible [Boolean quantum oracle](../../../quantum-theory.md#boolean-quantum-oracle)

$$
U_f|x\rangle|y\rangle=|x\rangle|y\oplus f(x)\rangle.
$$

The algebraic oracle map printed in the source has its arguments misplaced: taken literally, it sends two distinct answer inputs to the same output for constant $f$, so it cannot be a [unitary operator](../../../vector-space.md#unitary-operator). The corrected map above agrees with the diagram's input-control, answer-target arrangement. Put the answer [qubit](../../../quantum-mechanics.md#qubit) in $|-\rangle=(|0\rangle-|1\rangle)/\sqrt2$. Since the [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) satisfies $X|-\rangle=-|-\rangle$, [quantum phase kickback](../../../quantum-theory.md#phase-kickback) gives

$$
U_f|x\rangle|-\rangle=(-1)^{f(x)}|x\rangle|-\rangle.
$$

Write $b=f(0)\oplus f(1)$. Up to the irrelevant [global phase](../../../quantum-mechanics.md#global-phase) $(-1)^{f(0)}$, the input [qubit](../../../quantum-mechanics.md#qubit) acquires relative phase $(-1)^b$, so its ideal final [computational-basis measurement](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis) returns $b$: zero for a constant function and one for a balanced function.

Let the specified [quantum decoherence](../../../quantum-theory.md#quantum-decoherence) occur in the interference portion between the two [Hadamard gates](../../../quantum-theory.md#hadamard-gate). It commutes with the oracle's effective diagonal phase on the input, so the same analysis applies whether it occurs just before or just after the query. The two likelihoods are

$$
\Pr(0\mid b)=\frac{1+(-1)^b v\cos\alpha}{2},\qquad
\Pr(1\mid b)=\frac{1-(-1)^b v\cos\alpha}{2}.
$$

Thus the diagram's usual zero-for-constant decision rule has

$$
\boxed{P_{\mathrm{correct}}=\frac{1+v\cos\alpha}{2}.}
$$

This is the reliability for either promised class separately, with no prior needed. For equally likely classes, if $v\cos\alpha$ is known to be negative, reversing the interpretation gives $(1+|v\cos\alpha|)/2$. A known environment phase can instead be compensated by the [phase gate](../../../quantum-theory.md#phase-gate) $P(-\alpha)$ before the final [Hadamard gate](../../../quantum-theory.md#hadamard-gate), giving **success probability $(1+v)/2$**. In particular, $v=0$ gives no information and $v=1$ permits certainty after phase compensation. These refinements distinguish a shifted fringe from lost [quantum coherence](../../../quantum-theory.md#quantum-coherence-in-a-specified-basis); with the unmodified diagram a phase shift alone can reverse the apparent answer. [Quantum decoherence](../../../quantum-theory.md#quantum-decoherence) after the final [Hadamard gate](../../../quantum-theory.md#hadamard-gate) leaves its computational populations unchanged, so that different placement would not spoil the measured answer.

## 2

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Walsh-Hadamard transform](../../../quantum-theory.md#walsh-hadamard-transform) is the [tensor product](../../../linear-algebra.md#tensor-product) of one [Hadamard gate](../../../quantum-theory.md#hadamard-gate) on each [qubit](../../../quantum-mechanics.md#qubit). Indeed,

$$
H^{\otimes n}|x_1\cdots x_n\rangle
=\bigotimes_{j=1}^n\frac{|0\rangle+(-1)^{x_j}|1\rangle}{\sqrt2}
=2^{-n/2}\sum_{y\in\{0,1\}^n}(-1)^{\sum_jx_jy_j}|y\rangle.
$$

The network therefore consists of $n$ parallel [Hadamard gates](../../../quantum-theory.md#hadamard-gate), with no interaction between wires. Applied to an all-zero [quantum register](../../../quantum-circuit.md#quantum-register), it produces the [uniform quantum superposition](../../../quantum-theory.md#uniform-quantum-superposition) of all $2^n$ input strings. This lets a [Boolean quantum oracle](../../../quantum-theory.md#boolean-quantum-oracle) act coherently on all those inputs; a subsequent operation can turn their relative phases into useful interference. It does not permit reading all oracle values from a single [measurement in quantum mechanics](../../../quantum-measurement.md).

<a id="2/image-parallel-hadamard-gates-and-the-one-query-bernstein-vazirani-network"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47-hadamard-networks.png)

**[Figure 1](#2/image-parallel-hadamard-gates-and-the-one-query-bernstein-vazirani-network). Parallel Hadamard gates and the one-query Bernstein-Vazirani network**.

For the supplied linear-phase input, the amplitude on output $y$ is

$$
2^{-n}\sum_{x\in\{0,1\}^n}(-1)^{a\cdot x+x\cdot y}
=\prod_{j=1}^n\frac{1+(-1)^{a_j\oplus y_j}}2
=\begin{cases}1,&y=a,\\0,&y\ne a.\end{cases}
$$

Each factor is obtained by summing over the independent bit $x_j$. This directly proves the relevant [orthogonality](../../../linear-algebra.md#orthogonal-vectors) of the binary Fourier phases, and yields **the output state $|a\rangle$ exactly**.

For exact classical identification, query the [Boolean function](../../../combinatorics.md#boolean-function) at the $n$ standard unit vectors: $f(e_j)=a_j$. Hence $n$ oracle calls suffice. They are also necessary in the worst case, even with adaptive queries: every answer supplies one binary linear equation in the unknown string. With fewer than $n$ queries, their coefficient [matrix](../../../vector-space.md#matrix) has [matrix rank](../../../vector-space.md#matrix-rank) at most the number of queries, so its [null space](../../../linear-algebra.md#kernel-of-a-linear-map) contains a nonzero string $h$. The strings $a$ and $a\oplus h$ give identical answers along that adaptive transcript and cannot both be identified correctly. Equivalently, a depth-$t$ binary decision tree has at most $2^t$ leaves and must distinguish $2^n$ possibilities. Thus **the exact classical query count is $n$**. This concerns exact recovery, rather than allowing an arbitrary error probability.

The quantum network in the lower panel starts its data [quantum register](../../../quantum-circuit.md#quantum-register) in $|0\rangle^{\otimes n}$ and its answer [ancilla qubit](../../../quantum-information-theory.md#ancilla-qubit) in $|-\rangle$, which can be prepared as $H|1\rangle$. Apply [Hadamard gates](../../../quantum-theory.md#hadamard-gate) to the data wires, make one [Boolean quantum oracle](../../../quantum-theory.md#boolean-quantum-oracle) call, then apply [Hadamard gates](../../../quantum-theory.md#hadamard-gate) again to all data wires. [Quantum phase kickback](../../../quantum-theory.md#phase-kickback) produces

$$
|0^n\rangle|-\rangle
\longmapsto 2^{-n/2}\sum_x|x\rangle|-\rangle
\longmapsto 2^{-n/2}\sum_x(-1)^{a\cdot x}|x\rangle|-\rangle
\longmapsto |a\rangle|-\rangle.
$$

A [computational-basis measurement](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis) of the data wires gives all bits of $a$ with certainty. This is [Bernstein-Vazirani phase kickback](../../../quantum-theory.md#bernstein-vazirani-phase-kickback): **one quantum query**, $2n$ data [Hadamard gates](../../../quantum-theory.md#hadamard-gate), and one answer-state preparation suffice. The answer [ancilla qubit](../../../quantum-information-theory.md#ancilla-qubit) stays separate from the data at the output.

## 3

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use the [Hilbert-Schmidt inner product](../../../compact-operator.md#hilbert-schmidt-inner-product) normalized by the dimension: $(A,B)=\tfrac12\operatorname{Tr}(A^\dagger B)$. The identity and the three [Pauli matrices](../../../algebra.md#pauli-matrices) are Hermitian, each has square $I$, and each nonidentity [Pauli matrix](../../../algebra.md#pauli-matrices) has zero [trace](../../../linear-algebra.md#matrix-trace). For distinct nonidentity indices, the [Pauli matrix multiplication law](../../../algebra.md#pauli-matrix-multiplication-law) gives $\sigma_j\sigma_k=i\sum_l\varepsilon_{jkl}\sigma_l$, which is traceless. Therefore

$$
\frac12\operatorname{Tr}(\sigma_j^\dagger\sigma_k)=\delta_{jk}\qquad(0\le j,k\le3).
$$

There are four such [orthonormal](../../../linear-algebra.md#orthonormal-set) operators, and the complex [vector space](../../../vector-space.md) of two-by-two [matrices](../../../vector-space.md#matrix) has [dimension](../../../vector-space.md#dimension-vector-space) four. Hence they form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis). Taking the [inner product](../../../linear-algebra.md#inner-product) of any $E$ with each basis element proves, for arbitrary complex $E$ and not just Hermitian ones,

$$
\boxed{E=\frac12\sum_{k=0}^3\operatorname{Tr}(\sigma_kE)\sigma_k.}
$$

For example, if $E=\begin{pmatrix}a&b\\c&d\end{pmatrix}$, its four coefficients are $(a+d)/2$, $(b+c)/2$, $i(b-c)/2$, and $(a-d)/2$, respectively.

For the joint error, regard the two prescribed basis outputs as the columns of an environment-valued [linear map](../../../vector-space.md#linear-map). Its coefficient array in the usual output-row, input-column convention is

$$
M=\begin{pmatrix}|e_{00}\rangle&|e_{10}\rangle\\|e_{01}\rangle&|e_{11}\rangle\end{pmatrix}.
$$

The source's other array is arranged as a column of the images of basis kets; it must not be mistaken for this coefficient array acting on an amplitude column. Applying the just-proved [Pauli matrix](../../../algebra.md#pauli-matrices) expansion componentwise in any environment [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) gives the [Pauli decomposition of a qubit-environment isometry](../../../quantum-circuit.md#pauli-decomposition-of-a-qubit-environment-isometry):

$$
\boxed{\begin{aligned}
|e_0\rangle&=\tfrac12(|e_{00}\rangle+|e_{11}\rangle),&
|e_1\rangle&=\tfrac12(|e_{01}\rangle+|e_{10}\rangle),\\
|e_2\rangle&=\tfrac{i}{2}(|e_{10}\rangle-|e_{01}\rangle),&
|e_3\rangle&=\tfrac12(|e_{00}\rangle-|e_{11}\rangle).
\end{aligned}}
$$

To check the potentially delicate sign of the [Pauli Y gate](../../../quantum-theory.md#pauli-y-gate) coefficient, use $Y|0\rangle=i|1\rangle$ and $Y|1\rangle=-i|0\rangle$. The four terms then give

$$
\begin{aligned}
\sum_k\sigma_k|0\rangle|e_k\rangle
&=|0\rangle(|e_0\rangle+|e_3\rangle)+|1\rangle(|e_1\rangle+i|e_2\rangle)
=|0\rangle|e_{00}\rangle+|1\rangle|e_{01}\rangle,\\
\sum_k\sigma_k|1\rangle|e_k\rangle
&=|0\rangle(|e_1\rangle-i|e_2\rangle)+|1\rangle(|e_0\rangle-|e_3\rangle)
=|0\rangle|e_{10}\rangle+|1\rangle|e_{11}\rangle.
\end{aligned}
$$

[Linearity](../../../vector-space.md#linearity) proves the expansion for every input [pure state](../../../quantum-theory.md#pure-state). The environment coefficient vectors need not be normalized or mutually orthogonal. Consequently this expansion includes coherent combinations of [Pauli errors](../../../quantum-circuit.md#pauli-operator), rather than asserting that every [quantum channel](../../../quantum-information-theory.md#quantum-channel) is a probabilistic [Pauli channel](../../../quantum-information-theory.md#pauli-channel).

For the recovery probability, use the usual independent-use interpretation of the given [phase-flip channel](../../../quantum-information-theory.md#phase-flip-channel): each of the three transmitted [qubits](../../../quantum-mechanics.md#qubit) has a [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) error independently with probability $q$. The [phase-flip repetition code](../../../quantum-error-correction.md#phase-flip-repetition-code) uses logical codewords $|+++\rangle$ and $|---\rangle$. The decoding [Hadamard gates](../../../quantum-theory.md#hadamard-gate) convert physical phase flips to bit flips because $HZH=X$. We can then analyze the two decoding [controlled-NOT gates](../../../quantum-theory.md#controlled-not-gate) and the final [Toffoli gate](../../../quantum-theory.md#toffoli-gate) directly, rather than assuming a recovery rule.

Let $b_1,b_2,b_3$ be the error bits after this basis conversion. For a logical basis input $t\in\{0,1\}$, the three data bits before inverse encoding are $t\oplus b_1,t\oplus b_2,t\oplus b_3$. The two [controlled-NOT gates](../../../quantum-theory.md#controlled-not-gate) produce

$$
|t\oplus b_1\rangle\,|b_1\oplus b_2\rangle\,|b_1\oplus b_3\rangle.
$$

The [Toffoli gate](../../../quantum-theory.md#toffoli-gate) flips the first wire when both of the last two bits are one. Its residual error is

$$
r(b)=b_1\oplus\bigl[(b_1\oplus b_2)(b_1\oplus b_3)\bigr]
=\begin{cases}0,&b_1+b_2+b_3\le1,\\1,&b_1+b_2+b_3\ge2.\end{cases}
$$

The last two wires carry an [error syndrome](../../../quantum-error-correction.md#error-syndrome) independent of $t$. Thus this transformation preserves the amplitudes of an arbitrary superposition: zero or one phase error returns the original unknown [qubit](../../../quantum-mechanics.md#qubit), while two or three phase errors leave the logical [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) applied to it. The probability of universally successful recovery is therefore

$$
\boxed{P_{\mathrm{success}}=(1-q)^3+3q(1-q)^2=1-3q^2+2q^3.}
$$

Equivalently, the decoded [quantum channel](../../../quantum-information-theory.md#quantum-channel) is $\rho\mapsto(1-p_L)\rho+p_LX\rho X$, with [logical failure of the three-qubit phase-flip repetition code](../../../quantum-error-correction.md#logical-failure-of-the-three-qubit-phase-flip-repetition-code) $p_L=3q^2-2q^3$. For $0<q<1/2$, the failure probability is below $q$, since $q-p_L=q(1-q)(1-2q)>0$. A special input that is a [Pauli X eigenstate](../../../quantum-mechanics.md#pauli-x-eigenstate) is unchanged even by the residual logical error; this does not make the code correct that error on an unknown input. Its squared [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states) with a particular pure input is $1-p_L+p_L|\langle\chi|X|\chi\rangle|^2$. If the errors on different channel uses are correlated, the marginal probability $q$ alone is insufficient: the general universal success probability is the probability of at most one error.

## 4

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write both the input and output integer labels in most-significant-bit-first order, $x=\sum_{j=1}^n x_j2^{n-j}$ and $y=\sum_{j=1}^n y_j2^{n-j}$. Factoring the Fourier phase over the bits of $y$ gives the [product decomposition of a Fourier phase state](../../../quantum-theory.md#product-decomposition-of-a-fourier-phase-state):

$$
\operatorname{QFT}_{2^n}|x\rangle
=\bigotimes_{j=1}^n\frac{|0\rangle+e^{2\pi ix/2^j}|1\rangle}{\sqrt2}
=\bigotimes_{j=1}^n\frac{|0\rangle+e^{2\pi i\,0.x_{n-j+1}\cdots x_n}|1\rangle}{\sqrt2}.
$$

Here $0.x_l\cdots x_n$ denotes the binary fraction $\sum_{r=l}^n x_r/2^{r-l+1}$; the integer part of $x/2^j$ does not affect the phase.

Build a [dyadic quantum Fourier transform circuit](../../../quantum-theory.md#dyadic-quantum-fourier-transform-circuit) as follows. Process wires $j=1,\ldots,n$ in that order. First apply a [Hadamard gate](../../../quantum-theory.md#hadamard-gate) to wire $j$. Then, for each $l=j+1,\ldots,n$, apply the [controlled phase gate](../../../quantum-theory.md#controlled-phase-gate) $R_{l-j+1}$ with control wire $l$ and target wire $j$. On a [computational-basis state](../../../quantum-theory.md#computational-basis-state), every unprocessed control is still the bit $x_l$, so wire $j$ becomes

$$
\frac{|0\rangle+(-1)^{x_j}\prod_{l=j+1}^n e^{2\pi ix_l/2^{l-j+1}}|1\rangle}{\sqrt2}
=\frac{|0\rangle+e^{2\pi i\,0.x_j\cdots x_n}|1\rangle}{\sqrt2}.
$$

Once a wire has been processed it is not touched by later stages. Reversing the order of the output wires gives exactly the Fourier product above. Agreement on every [computational-basis state](../../../quantum-theory.md#computational-basis-state) proves agreement as [linear operators](../../../vector-space.md#linear-operator) on all superpositions, even though the intermediate operation on a general input can create [entanglement](../../../bell-state.md#entangled-state).

There are $n$ [Hadamard gates](../../../quantum-theory.md#hadamard-gate) and $n(n-1)/2$ [controlled phase gates](../../../quantum-theory.md#controlled-phase-gate). Output reversal may be treated as wire relabelling. If it must instead be implemented physically while using only the requested gate family, use $\lfloor n/2\rfloor$ [swap operators](../../../quantum-information-theory.md#swap-operator). Each swap is three [controlled-NOT gates](../../../quantum-theory.md#controlled-not-gate), and

$$
\operatorname{CNOT}_{a\to b}=H_b\,\operatorname{controlled}\!R_1(a,b)\,H_b,
\qquad R_1=Z.
$$

Thus the swaps use only [Hadamard gates](../../../quantum-theory.md#hadamard-gate) and [Controlled-Z gates](../../../quantum-theory.md#controlled-z-gate), which are controlled $R_1$ gates. An exact physical network has

$$
g_n=\frac{n(n+1)}2+9\lfloor n/2\rfloor=O(n^2)
$$

elementary gates from the stated family. **This implements the positive-exponent Fourier transform with the correct output order in quadratic size.** Omitting the output reversal without relabelling the wires would produce the reversed-order transform instead.

For the perturbation bound, the [operator norm](../../../continuous-dual-space.md#operator-norm) in the source is equivalently $\|A\|=\sup_{\|\psi\|=1}\|A\psi\|$. It satisfies the [triangle inequality](../../../topological-analysis.md#triangle-inequality), is unchanged by left or right multiplication by a [unitary operator](../../../vector-space.md#unitary-operator), and a [unitary operator](../../../vector-space.md#unitary-operator) has norm one. The exact telescoping identity is

$$
U_1\cdots U_m-V_1\cdots V_m
=\sum_{j=1}^m U_1\cdots U_{j-1}(U_j-V_j)V_{j+1}\cdots V_m.
$$

It follows by replacing one factor at a time; alternatively all intermediate products cancel in the sum. Taking the [operator norm](../../../continuous-dual-space.md#operator-norm) and using unitary invariance gives the [quantum circuit gate-error telescoping bound](../../../quantum-circuit.md#quantum-circuit-gate-error-telescoping-bound)

$$
\|U_1\cdots U_m-V_1\cdots V_m\|
\le\sum_{j=1}^m\|U_j-V_j\|<m\epsilon.
$$

The original PDF assumes strict $\|U_j-V_j\|<\epsilon$, so its strict conclusion is justified. If the hypothesis were weakened to a non-strict inequality, the conclusion would likewise be $\le m\epsilon$. The TeX aid misreads this hypothesis; the PDF resolves it.

Apply the non-strict version to each approximate unitary gate in the Fourier network. Extending a gate by the identity on other wires leaves its [operator norm](../../../continuous-dual-space.md#operator-norm) error unchanged. Including the physical swap decompositions, all gates are of the required type and can obey the stated accuracy. Hence

$$
\boxed{\|U_n-\operatorname{QFT}_{2^n}\|\le\frac{g_n}{n^4}
=\frac{n(n+1)/2+9\lfloor n/2\rfloor}{n^4}
=O(n^{-2}).}
$$

With exact output relabelling rather than physical swaps the numerator is just $n(n+1)/2$. The proof retains gate phases and makes no assumption of cancellation between coherent errors.

For every normalized input the output-state [norm](../../../functional-analysis.md#norm) error is at most this same bound. If $M$ is any [positive operator](../../../hilbert-space.md#positive-operator) satisfying $0\le M\le I$, the change in its [measurement in quantum mechanics](../../../quantum-measurement.md) outcome probability is at most $2\delta$, where $\delta=\|U_n-\operatorname{QFT}_{2^n}\|$: expand the difference of the two expectations into two terms, each bounded by $\delta$ using the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Thus **inverse-polynomial gate accuracy gives an inverse-polynomial total error**, rather than requiring exponential precision in the number of qubits. For the [phase gates](../../../quantum-theory.md#phase-gate) this corresponds to specifying angles with $O(\log n)$ bits of precision, since $|e^{i\theta}-e^{i\theta'}|\le|\theta-\theta'|$. This is a robustness statement for unitary gate approximations; it does not by itself correct [quantum decoherence](../../../quantum-theory.md#quantum-decoherence), correlated stochastic faults, or limitations of hardware connectivity.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
