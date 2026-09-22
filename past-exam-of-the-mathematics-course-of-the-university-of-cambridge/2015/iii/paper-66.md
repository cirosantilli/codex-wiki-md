# Paper 66

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_66.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_66.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
  - [vi](#1/vi)
    - [Solution](#1/vi/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
    - [a](#4/ii/a)
      - [Solution](#4/ii/a/solution)
    - [b](#4/ii/b)
      - [Solution](#4/ii/b/solution)
    - [c](#4/ii/c)
      - [Solution](#4/ii/c/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)

## 1

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

In the state-picture convention, a [Stinespring representation of a completely positive map](../../../quantum-information-theory.md#stinespring-representation-of-a-completely-positive-map) $\mathcal N:\mathcal L(\mathcal H_Q)\to\mathcal L(\mathcal H_{Q'})$ consists of an auxiliary [Hilbert space](../../../hilbert-space.md) $\mathcal H_E$ and a linear map $V:\mathcal H_Q\to\mathcal H_{Q'}\otimes\mathcal H_E$ such that

$$
\boxed{\mathcal N(X)=\operatorname{Tr}_E(VXV^\dagger)\quad\text{for all }X.}
$$

The [partial trace](../../../quantum-theory.md#partial-trace) discards the environment. For example, from a [Kraus representation](../../../quantum-information-theory.md#kraus-representation) $\mathcal N(X)=\sum_jK_jXK_j^\dagger$, take $V=\sum_jK_j\otimes|j\rangle_E$. The adjoint, or observable-picture, form is $\mathcal N^\dagger(Y)=V^\dagger(Y\otimes I_E)V$.

A general [completely positive map](../../../quantum-information-theory.md#completely-positive-map) does not require $V$ to be an [linear isometry of Hilbert spaces](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces). If $\mathcal N$ is trace preserving, then $V^\dagger V=\sum_jK_j^\dagger K_j=I$, so $V$ is an [linear isometry of Hilbert spaces](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces). This is the [Stinespring dilation](../../../quantum-information-theory.md#stinespring-dilation) of a [quantum channel](../../../quantum-information-theory.md#quantum-channel), which will be used in the data-processing proof.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

By [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition), the [Von Neumann entropy](../../../von-neumann-entropy.md) is the [Shannon entropy](../../../information-theory.md#information-entropy) of the [eigenvalues](../../../linear-operator-theory.md#eigenvalue):

$$
\boxed{S(\rho_Q)=-\operatorname{Tr}(\rho_Q\log_2\rho_Q)=-\sum_{i=0}^{d-1}\lambda_i\log_2\lambda_i.}
$$

Throughout, logarithms have base two, so the [Von Neumann entropy](../../../von-neumann-entropy.md) and [Shannon entropy](../../../information-theory.md#information-entropy) are measured in bits. The continuous convention $0\log_2 0=0$ includes zero [eigenvalues](../../../linear-operator-theory.md#eigenvalue).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

For a bipartite [density operator](../../../quantum-theory.md#density-matrix) $\rho_{AB}$, let $S(A)_\rho=S(\rho_A)$, with $\rho_A=\operatorname{Tr}_B\rho_{AB}$, and similarly for other systems. The [quantum conditional entropy](../../../von-neumann-entropy.md#quantum-conditional-entropy) and [coherent information](../../../quantum-information-theory.md#coherent-information) are

$$
\boxed{H(A|B)_\rho=S(AB)_\rho-S(B)_\rho,\qquad I(A\rangle B)_\rho=S(B)_\rho-S(AB)_\rho=-H(A|B)_\rho.}
$$

Unlike classical [conditional entropy](../../../information-theory.md#conditional-entropy), [quantum conditional entropy](../../../von-neumann-entropy.md#quantum-conditional-entropy) can be negative. For a [Bell state](../../../bell-state.md), $S(AB)=0$ and $S(B)=1$, giving $H(A|B)=-1$ and [coherent information](../../../quantum-information-theory.md#coherent-information) equal to one bit.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Use the [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition) of the bipartite [pure state](../../../quantum-theory.md#pure-state):

$$
|\psi\rangle_{QR}=\sum_{j=1}^r\sqrt{p_j}\,|u_j\rangle_Q|v_j\rangle_R,\qquad p_j>0,\quad\sum_jp_j=1.
$$

The two [reduced density matrices](../../../bell-state.md#reduced-density-matrix), obtained by [partial trace](../../../quantum-theory.md#partial-trace), are

$$
\rho_Q=\sum_jp_j|u_j\rangle\langle u_j|,\qquad\rho_R=\sum_jp_j|v_j\rangle\langle v_j|.
$$

Their nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are identical, even if the two ambient dimensions differ. Zero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) contribute no [Von Neumann entropy](../../../von-neumann-entropy.md), so

$$
\boxed{H(Q)_\psi=H(R)_\psi=-\sum_jp_j\log_2p_j.}
$$

This common [Von Neumann entropy](../../../von-neumann-entropy.md) is the [entanglement entropy](../../../von-neumann-entropy.md#entanglement-entropy) of the bipartite [pure state](../../../quantum-theory.md#pure-state).

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

Use two results: the isometric [Stinespring dilation](../../../quantum-information-theory.md#stinespring-dilation) of a [quantum channel](../../../quantum-information-theory.md#quantum-channel), and [Strong subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy). Let $V:B\to B'E$ dilate the given operation, and define

$$
\omega_{AB'E}=(I_A\otimes V)\rho_{AB}(I_A\otimes V^\dagger),\qquad\sigma_{AB'}=\operatorname{Tr}_E\omega.
$$

An [linear isometry of Hilbert spaces](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces) preserves the nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue), so $S(B'E)_\omega=S(B)_\rho$ and $S(AB'E)_\omega=S(AB)_\rho$. Subtracting the two [coherent information](../../../quantum-information-theory.md#coherent-information) expressions gives

$$
\begin{aligned}
I(A\rangle B)_\rho-I(A\rangle B')_\sigma
&=S(B'E)_\omega-S(AB'E)_\omega-S(B')_\omega+S(AB')_\omega\\
&=I(A:E|B')_\omega\geq0.
\end{aligned}
$$

The last inequality is [Strong subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy), in the form $S(AB')+S(B'E)\geq S(B')+S(AB'E)$. Thus the [data-processing inequality for coherent information](../../../quantum-information-theory.md#data-processing-inequality-for-coherent-information) is

$$
\boxed{I(A\rangle B)_\rho\geq I(A\rangle B')_\sigma.}
$$

The lost [coherent information](../../../quantum-information-theory.md#coherent-information) is precisely the [quantum conditional mutual information](../../../von-neumann-entropy.md#quantum-conditional-mutual-information) between the reference $A$ and discarded environment $E$, conditional on the retained output $B'$.

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#1/vi)

Take a [purification of a density operator](../../../quantum-theory.md#purification-of-a-density-operator) $|\Psi\rangle_{ABCD}$ of $\rho_{ABC}$. Apply [Strong subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy) to the reduced state on $ACD$, with $A$ the conditioning system:

$$
S(AC)+S(AD)\geq S(A)+S(ACD).
$$

Complementary subsystems of a [pure state](../../../quantum-theory.md#pure-state) have the same [Von Neumann entropy](../../../von-neumann-entropy.md), by the [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition). Therefore $S(AD)=S(BC)$ and $S(ACD)=S(B)$. Substitution gives

$$
\boxed{S(A)+S(B)\leq S(AC)+S(BC).}
$$

This is [weak monotonicity of quantum entropy](../../../von-neumann-entropy.md#weak-monotonicity-of-quantum-entropy). The [purification of a density operator](../../../quantum-theory.md#purification-of-a-density-operator) is only a proof device; no purity assumption is imposed on $\rho_{ABC}$.

## 2

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use [superdense coding](../../../bell-state.md#superdense-coding). For the two-bit message $(a,b)\in\{0,1\}^2$, Alice applies $Z^aX^b$ to her half of the shared [Bell state](../../../bell-state.md), where $X,Z$ are the [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) and [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate). The encoded states are

$$
\begin{array}{c|c}
(a,b)&(Z^aX^b\otimes I)|\Phi^+\rangle\\\hline
(0,0)&(|00\rangle+|11\rangle)/\sqrt2\\
(0,1)&(|01\rangle+|10\rangle)/\sqrt2\\
(1,0)&(|00\rangle-|11\rangle)/\sqrt2\\
(1,1)&(|01\rangle-|10\rangle)/\sqrt2.
\end{array}
$$

These four [Bell states](../../../bell-state.md) are orthonormal. Alice then transmits her one [qubit](../../../quantum-mechanics.md#qubit) to Bob, who now holds both [qubits](../../../quantum-mechanics.md#qubit). A [Bell-basis measurement](../../../bell-state.md#bell-basis-measurement) identifies the message with probability one.

More explicitly, Bob can apply a [CNOT gate](../../../quantum-theory.md#controlled-not-gate) with the received [qubit](../../../quantum-mechanics.md#qubit) as control and his original [qubit](../../../quantum-mechanics.md#qubit) as target, followed by a [Hadamard gate](../../../quantum-theory.md#hadamard-gate) on the control. The [CNOT gate](../../../quantum-theory.md#controlled-not-gate) sends the encoded state to

$$
\frac{|0\rangle+(-1)^a|1\rangle}{\sqrt2}\otimes|b\rangle,
$$

and the [Hadamard gate](../../../quantum-theory.md#hadamard-gate) sends this to $|a\rangle\otimes|b\rangle$. Computational-basis [projective measurements](../../../quantum-measurement.md#projective-measurement) therefore read out $a,b$ exactly. **One transmitted qubit, assisted by one previously shared Bell pair, communicates two classical bits.**

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Use [one-bit remote preparation of real qubit states](../../../quantum-information-theory.md#one-bit-remote-preparation-of-real-qubit-states). Alice measures her [qubit](../../../quantum-mechanics.md#qubit) in the [orthonormal basis](../../../linear-algebra.md#orthonormal-basis)

$$
|\alpha_\theta\rangle=\cos\theta|0\rangle+\sin\theta|1\rangle,\qquad|\beta_\theta\rangle=-\sin\theta|0\rangle+\cos\theta|1\rangle.
$$

Because this change of basis is real and orthogonal, the shared [Bell state](../../../bell-state.md) has the expansion

$$
|\Phi^+\rangle=\frac{|\alpha_\theta\rangle_A|\alpha_\theta\rangle_B+|\beta_\theta\rangle_A|\beta_\theta\rangle_B}{\sqrt2}.
$$

Her [projective measurement](../../../quantum-measurement.md#projective-measurement) gives each outcome with probability one half. She sends $m=0$ for the first outcome and $m=1$ for the second. Bob's conditional [pure state](../../../quantum-theory.md#pure-state) is respectively $|\alpha_\theta\rangle$ or $|\beta_\theta\rangle$.

For $m=0$ Bob does nothing. For $m=1$ he applies the fixed [unitary operator](../../../vector-space.md#unitary-operator)

$$
U=iY=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\qquad U|\beta_\theta\rangle=|\alpha_\theta\rangle,
$$

where $Y$ is the [Pauli Y gate](../../../quantum-theory.md#pauli-y-gate). Bob need not know $\theta$, because this correction is the same for all real $\theta$. **Both outcomes produce the exact density operator $|\alpha_\theta\rangle\langle\alpha_\theta|$, using one classical bit and only local operations.**

This [remote state preparation](../../../quantum-information-theory.md#remote-state-preparation) consumes the shared [entangled state](../../../bell-state.md#entangled-state). Before receiving the bit, Bob has the mixture $(|\alpha_\theta\rangle\langle\alpha_\theta|+|\beta_\theta\rangle\langle\beta_\theta|)/2=I/2$, independent of $\theta$, as required by [quantum no-signalling](../../../quantum-theory.md#quantum-no-signalling). The real-state restriction is what permits a fixed unitary correction of the orthogonal outcome.

## 3

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [positive part of a Hermitian operator](../../../hilbert-space.md#positive-part-of-a-hermitian-operator) and [negative part of a Hermitian operator](../../../hilbert-space.md#negative-part-of-a-hermitian-operator) are the positive operators

$$
\boxed{X_+=\sum_i\max(\lambda_i,0)|\alpha_i\rangle\langle\alpha_i|,\qquad X_-=\sum_i\max(-\lambda_i,0)|\alpha_i\rangle\langle\alpha_i|.}
$$

Thus $X=X_+-X_-$ and $X_+X_-=0$. In this convention the negative part itself is nonnegative. This is the [positive-negative decomposition](../../../hilbert-space.md#positive-negative-decomposition-of-a-hermitian-operator) of the [Hermitian operator](../../../hilbert-space.md#hermitian-operator).

The [operator absolute value](../../../banach-algebra.md#absolute-value-of-an-operator) is defined by the unique [positive operator](../../../hilbert-space.md#positive-operator) square root

$$
|X|=\sqrt{X^\dagger X}=\sqrt{X^2}=\sum_i|\lambda_i|\,|\alpha_i\rangle\langle\alpha_i|.
$$

The scalar identity $|\lambda|=\max(\lambda,0)+\max(-\lambda,0)$ applied in the [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition) proves

$$
\boxed{|X|=X_++X_-.}
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For any linear operator, the [trace norm](../../../functional-analysis.md#trace-norm) is $\|X\|_1=\operatorname{Tr}\sqrt{X^\dagger X}$, the sum of its [singular values](../../../linear-algebra.md#singular-value). For a [Hermitian operator](../../../hilbert-space.md#hermitian-operator),

$$
\boxed{\|X\|_1=\operatorname{Tr}|X|=\sum_i|\lambda_i|.}
$$

The [Holevo–Helstrom theorem](../../../quantum-information-theory.md#holevo-helstrom-theorem) concerns minimum-error discrimination of two [density operators](../../../quantum-theory.md#density-matrix) $\rho,\sigma$. If their prior probabilities are $p$ and $1-p$, the maximum success probability over all [measurement in quantum measurements](../../../quantum-measurement.md) is

$$
\boxed{P_{\mathrm{succ}}^*=\frac12\left(1+\|p\rho-(1-p)\sigma\|_1\right).}
$$

An optimal binary [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) declares $\rho$ on the positive spectral subspace of $p\rho-(1-p)\sigma$ and declares $\sigma$ on its negative spectral subspace; zero-eigenvalue vectors can be assigned either way. For equal priors the formula becomes $P_{\mathrm{succ}}^*=\tfrac12+\tfrac14\|\rho-\sigma\|_1$.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The constraints $-I\leq T\leq I$ are in the order of [Hermitian operators](../../../hilbert-space.md#hermitian-operator). They imply $-1\leq\langle\alpha_i|T|\alpha_i\rangle\leq1$. Using the [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition) of $X$,

$$
\operatorname{Tr}(XT)=\sum_i\lambda_i\langle\alpha_i|T|\alpha_i\rangle\leq\sum_i|\lambda_i|=\|X\|_1.
$$

Choose $T=\operatorname{sgn}(X)$, with eigenvalues $+1$ on the positive spectral subspace, $-1$ on the negative spectral subspace, and zero on the kernel. It satisfies the constraints and attains equality. The [trace-norm variational principle for Hermitian operators](../../../functional-analysis.md#trace-norm-variational-principle-for-hermitian-operators) is therefore

$$
\boxed{\|X\|_1=\max_{-I\leq T\leq I}\operatorname{Tr}(XT).}
$$

To prove the [Holevo–Helstrom theorem](../../../quantum-information-theory.md#holevo-helstrom-theorem), write a binary [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) as $\{E,I-E\}$, where $0\leq E\leq I$, and associate the first outcome with $\rho$. Any larger outcome set followed by a binary decision can be grouped into this form. Put $\Delta=p\rho-(1-p)\sigma$. Its success probability is

$$
P_{\mathrm{succ}}=p\operatorname{Tr}(\rho E)+(1-p)\operatorname{Tr}(\sigma(I-E))=(1-p)+\operatorname{Tr}(\Delta E).
$$

The substitution $T=2E-I$ bijects the allowed effects with the interval $-I\leq T\leq I$. Since $\operatorname{Tr}\Delta=2p-1$,

$$
P_{\mathrm{succ}}=\frac12+\frac12\operatorname{Tr}(\Delta T)\leq\frac12(1+\|\Delta\|_1).
$$

Choosing $E$ as the positive spectral projection of $\Delta$ attains this value, with an arbitrary decision on its kernel. **This proves the optimal success probability and constructs an optimal measurement.**

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

For two [density operators](../../../quantum-theory.md#density-matrix), the [trace distance](../../../quantum-theory.md#trace-distance) and the unsquared [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states) are

$$
\boxed{D(\rho,\sigma)=\frac12\|\rho-\sigma\|_1,\qquad F(\rho,\sigma)=\operatorname{Tr}\sqrt{\sqrt\rho\,\sigma\sqrt\rho}=\|\sqrt\rho\sqrt\sigma\|_1.}
$$

The unsquared convention matters: if $P=|\psi\rangle\langle\psi|$ is a [pure state](../../../quantum-theory.md#pure-state), then $\sqrt\rho P\sqrt\rho$ is a rank-one [positive operator](../../../hilbert-space.md#positive-operator) with its sole nonzero [eigenvalue](../../../linear-operator-theory.md#eigenvalue) equal to $\langle\psi|\rho|\psi\rangle$. Hence

$$
\boxed{F(\rho,P)^2=\langle\psi|\rho|\psi\rangle.}
$$

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

Write $x_i=\langle\psi_i|X|\psi_i\rangle$, which is real because $X$ is a [Hermitian operator](../../../hilbert-space.md#hermitian-operator). Set

$$
T=\sum_i\operatorname{sgn}(x_i)|\psi_i\rangle\langle\psi_i|,
$$

with $\operatorname{sgn}(0)=0$. This [Hermitian operator](../../../hilbert-space.md#hermitian-operator) satisfies $-I\leq T\leq I$. The [trace-norm variational principle for Hermitian operators](../../../functional-analysis.md#trace-norm-variational-principle-for-hermitian-operators) gives the [diagonal absolute-sum bound for the trace norm](../../../functional-analysis.md#diagonal-absolute-sum-bound-for-the-trace-norm):

$$
\boxed{\|X\|_1\geq\operatorname{Tr}(XT)=\sum_i|\langle\psi_i|X|\psi_i\rangle|.}
$$

For $X=\rho-P$, with $P=|\psi\rangle\langle\psi|$, extend $|\psi\rangle$ to an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $|\psi_1\rangle=|\psi\rangle,|\psi_2\rangle,\ldots$. Put $r=\langle\psi|\rho|\psi\rangle$. The first diagonal entry is $r-1\leq0$, and all the others are nonnegative. Their sum is $1-r$, because $\operatorname{Tr}\rho=1$. The bound therefore yields $\|\rho-P\|_1\geq2(1-r)$. Using the definitions of [trace distance](../../../quantum-theory.md#trace-distance) and [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states),

$$
\boxed{D(\rho,P)\geq1-r=1-F(\rho,P)^2.}
$$

This [pure-target lower bound on trace distance](../../../quantum-theory.md#pure-target-lower-bound-on-trace-distance) is attained whenever $\rho$ has no coherence between $|\psi\rangle$ and its orthogonal complement. The proof used the [trace-norm variational principle for Hermitian operators](../../../functional-analysis.md#trace-norm-variational-principle-for-hermitian-operators), together with positivity and normalization of a [density operator](../../../quantum-theory.md#density-matrix).

## 4

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The [Shannon entropy](../../../information-theory.md#information-entropy) of a finite-valued [random variable](../../../random-variable.md) is

$$
\boxed{H(X)=-\sum_{x\in\mathcal A_X}P_X(x)\log_2P_X(x),\qquad0\log_2 0=0.}
$$

An [epsilon-sufficient set](../../../information-theory.md#epsilon-sufficient-set) is a subset $S\subseteq\mathcal A_X$ retaining all but at most $\epsilon$ of the probability:

$$
\boxed{\Pr(X\in S)=\sum_{x\in S}P_X(x)\geq1-\epsilon.}
$$

Usually $0\leq\epsilon\leq1$. Sufficiency here concerns retained probability mass, rather than a [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Use the weak notion of a [typical set](../../../information-theory.md#typical-set). For a word $z^n=(z_1,\ldots,z_n)$ write $P_Z^n(z^n)=\prod_{i=1}^nP_Z(z_i)$. The definition is

$$
\boxed{T_\delta^n(P_Z)=\left\{z^n:P_Z^n(z^n)>0,\ \left|-\frac1n\log_2P_Z^n(z^n)-H(Z)\right|\leq\delta\right\}.}
$$

A [weakly typical sequence](../../../information-theory.md#weakly-typical-sequence) therefore has probability between $2^{-n(H(Z)+\delta)}$ and $2^{-n(H(Z)-\delta)}$. Words containing zero-probability symbols are excluded. These two bounds and the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) provide the three conclusions below.

<h4 id="4/ii/a">a</h4>

↑ **Parent:** [Ii](#4/ii)

<h5 id="4/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#4/ii/a)

Let $Y_i=-\log_2P_Z(Z_i)$. Since the alphabet is finite, these [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) are finite almost surely, have mean $H(Z)$, and have finite variance $v$. Also

$$
-\frac1n\log_2P_Z^n(Z^{(n)})=\frac1n\sum_{i=1}^nY_i.
$$

The [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) says that this average converges in probability to $H(Z)$. Thus

$$
\boxed{\lim_{n\to\infty}\Pr\bigl(Z^{(n)}\in T_\delta^n(P_Z)\bigr)=1\quad(\delta>0).}
$$

One can also state the quantitative [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) bound $\Pr(Z^{(n)}\notin T_\delta^n)\leq v/(n\delta^2)$. If $v=0$, every word of positive probability is in the [typical set](../../../information-theory.md#typical-set). This is the finite-alphabet [asymptotic equipartition property](../../../information-theory.md#asymptotic-equipartition-property).

<h4 id="4/ii/b">b</h4>

↑ **Parent:** [Ii](#4/ii)

<h5 id="4/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#4/ii/b)

Every word in the [typical set](../../../information-theory.md#typical-set) has probability at least $2^{-n(H(Z)+\delta)}$. Consequently

$$
1\geq\sum_{z^n\in T_\delta^n}P_Z^n(z^n)\geq|T_\delta^n|\,2^{-n(H(Z)+\delta)}.
$$

Rearranging proves the upper estimate in the [typical-set cardinality bounds](../../../information-theory.md#typical-set-cardinality-bounds):

$$
\boxed{|T_\delta^n(P_Z)|\leq2^{n(H(Z)+\delta)}.}
$$

<h4 id="4/ii/c">c</h4>

↑ **Parent:** [Ii](#4/ii)

<h5 id="4/ii/c/solution">Solution</h5>

↑ **Parent:** [C](#4/ii/c)

Fix $0\leq\epsilon<1$ and $\delta>0$. By the [asymptotic equipartition property](../../../information-theory.md#asymptotic-equipartition-property), all sufficiently large $n$ satisfy $\Pr(Z^{(n)}\notin T_\delta^n)\leq(1-\epsilon)/2$. For any [epsilon-sufficient set](../../../information-theory.md#epsilon-sufficient-set) $S_n$,

$$
\Pr(Z^{(n)}\in S_n\cap T_\delta^n)\geq\Pr(Z^{(n)}\in S_n)-\Pr(Z^{(n)}\notin T_\delta^n)\geq\frac{1-\epsilon}{2}.
$$

Each word in this intersection has probability at most $2^{-n(H(Z)-\delta)}$. Hence

$$
\frac{1-\epsilon}{2}\leq|S_n\cap T_\delta^n|\,2^{-n(H(Z)-\delta)}\leq|S_n|\,2^{-n(H(Z)-\delta)},
$$

which gives the [minimum size of a sufficient set for an IID source](../../../information-theory.md#minimum-size-of-a-sufficient-set-for-an-iid-source):

$$
\boxed{|S_n|\geq\frac{1-\epsilon}{2}\,2^{n(H(Z)-\delta)}.}
$$

The [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) used above supplies the sufficient quantitative condition $n\geq2v/[\delta^2(1-\epsilon)]$. No assumption that $S_n$ itself is a [typical set](../../../information-theory.md#typical-set) is needed; its intersection with one provides the bound.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Use the [Shannon second coding theorem](../../../coding-theory.md#noisy-channel-coding-theorem) in its [channel capacity](../../../information-theory.md#channel-capacity) form $C=\max_{P_X}I(X;Y)$. The [finite-alphabet erasure channel](../../../coding-theory.md#finite-alphabet-erasure-channel) erases independently of the input. On an unerased output Bob knows $X$ exactly; on the erasure output his posterior distribution is still $P_X$. Its classical [conditional entropy](../../../information-theory.md#conditional-entropy) is therefore

$$
H(X|Y)=fH(X),\qquad I(X;Y)=H(X)-H(X|Y)=(1-f)H(X).
$$

Equivalently, $H(Y)=h(f)+(1-f)H(X)$ and $H(Y|X)=h(f)$, so the [binary entropy](../../../information-theory.md#binary-entropy) terms cancel in the [mutual information](../../../information-theory.md#mutual-information).

For an alphabet of size $k$, [Shannon entropy](../../../information-theory.md#information-entropy) is at most $\log_2k$, with equality for the uniform distribution. Maximizing the displayed [mutual information](../../../information-theory.md#mutual-information) proves the [capacity of a finite-alphabet erasure channel](../../../coding-theory.md#capacity-of-a-finite-alphabet-erasure-channel):

$$
\boxed{C=(1-f)\log_2k\quad\text{bits per channel use}.}
$$

This includes $f=0$, which transmits the whole symbol, and $f=1$, which transmits no information.

## 5

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

For $t<1$, normalize the remaining probabilities by $q_j=P_X(j)/(1-t)$, $j=2,\ldots,k$. Directly splitting the [Shannon entropy](../../../information-theory.md#information-entropy) sum gives

$$
H(X)=-t\log_2t-(1-t)\log_2(1-t)+(1-t)H(q)=h(t)+(1-t)H(q).
$$

Here $h$ is the [binary entropy](../../../information-theory.md#binary-entropy). The [Shannon entropy](../../../information-theory.md#information-entropy) of a distribution on $k-1$ points is at most $\log_2(k-1)$. For example, nonnegativity of its [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence) from the uniform distribution gives $\log_2(k-1)-H(q)\geq0$. Thus the [entropy bound with one prescribed probability](../../../information-theory.md#entropy-bound-with-one-prescribed-probability) is

$$
\boxed{H(X)\leq h(t)+(1-t)\log_2(k-1).}
$$

For $t<1$, equality holds precisely when the remaining probabilities are all $(1-t)/(k-1)$. For $t=1$, the distribution is deterministic and both sides are zero. The displayed formula is for $k\geq2$; a one-point alphabet simply has zero [Shannon entropy](../../../information-theory.md#information-entropy).

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Put $p_i=\langle\psi_i|\rho|\psi_i\rangle$. The [rank-one dephasing](../../../quantum-measurement.md#rank-one-dephasing) is $\rho'=\sum_ip_i|\psi_i\rangle\langle\psi_i|$. If $p_i=0$, positivity gives

$$
0=p_i=\|\sqrt\rho\,|\psi_i\rangle\|^2,
$$

so $\rho|\psi_i\rangle=0$. The kernel of $\rho'$ is exactly the span of these zero-probability basis vectors and is therefore contained in the kernel of $\rho$. Taking orthogonal complements proves [support inclusion under rank-one dephasing](../../../quantum-measurement.md#support-inclusion-under-rank-one-dephasing):

$$
\boxed{\operatorname{supp}\rho\subseteq\operatorname{supp}\rho'.}
$$

Here the [support of a positive operator](../../../hilbert-space.md#support-of-a-positive-operator) is the orthogonal complement of its kernel.

On that support, $\log_2\rho'$ is diagonal in the measurement basis, giving

$$
\operatorname{Tr}(\rho\log_2\rho')=\sum_{i:p_i>0}p_i\log_2p_i=\operatorname{Tr}(\rho'\log_2\rho').
$$

Consequently the [relative-entropy identity for rank-one dephasing](../../../quantum-measurement.md#relative-entropy-identity-for-rank-one-dephasing) is

$$
D_{\mathrm{rel}}(\rho\|\rho')=\operatorname{Tr}\bigl[\rho(\log_2\rho-\log_2\rho')\bigr]=S(\rho')-S(\rho).
$$

[Klein's inequality](../../../vector-space.md#klein-s-inequality) gives $D_{\mathrm{rel}}(\rho\|\rho')\geq0$, since both [density operators](../../../quantum-theory.md#density-matrix) have trace one. For singular $\rho$, first restrict to $\operatorname{supp}\rho'$ where $\rho'$ is positive definite, replace $\rho$ by $(\rho+\eta I)/(1+\eta\dim\operatorname{supp}\rho')$, and let $\eta\downarrow0$. The support inclusion ensures that the limit is finite. Thus

$$
\boxed{S(\rho')\geq S(\rho).}
$$

This proves [entropy increase under nonselective projective measurement](../../../von-neumann-entropy.md#entropy-increase-under-nonselective-projective-measurement) using [Klein's inequality](../../../vector-space.md#klein-s-inequality). Equality holds exactly when $\rho=\rho'$, so the original [density operator](../../../quantum-theory.md#density-matrix) was already diagonal in the chosen basis.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Choose an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of the joint $d^2$-dimensional [Hilbert space](../../../hilbert-space.md) whose first vector is the given [purification of a density operator](../../../quantum-theory.md#purification-of-a-density-operator) $|\rho\rangle_{QR}$. Apply [rank-one dephasing](../../../quantum-measurement.md#rank-one-dephasing) to $\sigma_{QR}$ in this basis, and denote the resulting diagonal probabilities by $p_1,\ldots,p_{d^2}$. Their first entry is

$$
p_1=\langle\rho|\sigma_{QR}|\rho\rangle=f^2.
$$

The preceding [entropy increase under nonselective projective measurement](../../../von-neumann-entropy.md#entropy-increase-under-nonselective-projective-measurement) and [entropy bound with one prescribed probability](../../../information-theory.md#entropy-bound-with-one-prescribed-probability) yield

$$
S(\sigma_{QR})\leq H(p)\leq h(f^2)+(1-f^2)\log_2(d^2-1).
$$

Therefore the [quantum Fano inequality](../../../quantum-information-theory.md#quantum-fano-inequality) is

$$
\boxed{S(\sigma_{QR})\leq h(f^2)+(1-f^2)\log_2(d^2-1).}
$$

The quantity $f^2$ is the [entanglement fidelity](../../../quantum-information-theory.md#entanglement-fidelity) of $\mathcal N$ on $\rho_Q$; it is already a squared overlap, so it is $f^2$, rather than $f$, that enters the [binary entropy](../../../information-theory.md#binary-entropy). The argument is an instance of the [entropy bound from overlap with a pure state](../../../von-neumann-entropy.md#entropy-bound-from-overlap-with-a-pure-state) in dimension $d^2$. At $f^2=1$ the output is the original [pure state](../../../quantum-theory.md#pure-state) and its [Von Neumann entropy](../../../von-neumann-entropy.md) is zero. For $d=1$ the system is trivial and the same zero-entropy conclusion holds without evaluating $\log_2(d^2-1)$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
