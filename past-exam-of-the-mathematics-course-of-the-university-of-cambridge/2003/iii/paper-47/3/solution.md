<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [Hilbert-Schmidt inner product](../../../../../hilbert-schmidt-inner-product.md) normalized by the dimension: $(A,B)=\tfrac12\operatorname{Tr}(A^\dagger B)$. The identity and the three [Pauli matrices](../../../../../pauli-matrices.md) are Hermitian, each has square $I$, and each nonidentity [Pauli matrix](../../../../../pauli-matrices.md) has zero [trace](../../../../../matrix-trace.md). For distinct nonidentity indices, the [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) gives $\sigma_j\sigma_k=i\sum_l\varepsilon_{jkl}\sigma_l$, which is traceless. Therefore

$$
\frac12\operatorname{Tr}(\sigma_j^\dagger\sigma_k)=\delta_{jk}\qquad(0\le j,k\le3).
$$

There are four such [orthonormal](../../../../../orthonormal-set.md) operators, and the complex [vector space](../../../../../vector-space-split.md) of two-by-two [matrices](../../../../../matrix.md) has [dimension](../../../../../dimension-vector-space.md) four. Hence they form an [orthonormal basis](../../../../../orthonormal-basis.md). Taking the [inner product](../../../../../inner-product.md) of any $E$ with each basis element proves, for arbitrary complex $E$ and not just Hermitian ones,

$$
\boxed{E=\frac12\sum_{k=0}^3\operatorname{Tr}(\sigma_kE)\sigma_k.}
$$

For example, if $E=\begin{pmatrix}a&b\\c&d\end{pmatrix}$, its four coefficients are $(a+d)/2$, $(b+c)/2$, $i(b-c)/2$, and $(a-d)/2$, respectively.

For the joint error, regard the two prescribed basis outputs as the columns of an environment-valued [linear map](../../../../../linear-map.md). Its coefficient array in the usual output-row, input-column convention is

$$
M=\begin{pmatrix}|e_{00}\rangle&|e_{10}\rangle\\|e_{01}\rangle&|e_{11}\rangle\end{pmatrix}.
$$

The source's other array is arranged as a column of the images of basis kets; it must not be mistaken for this coefficient array acting on an amplitude column. Applying the just-proved [Pauli matrix](../../../../../pauli-matrices.md) expansion componentwise in any environment [orthonormal basis](../../../../../orthonormal-basis.md) gives the [Pauli decomposition of a qubit-environment isometry](../../../../../pauli-decomposition-of-a-qubit-environment-isometry.md):

$$
\boxed{\begin{aligned}
|e_0\rangle&=\tfrac12(|e_{00}\rangle+|e_{11}\rangle),&
|e_1\rangle&=\tfrac12(|e_{01}\rangle+|e_{10}\rangle),\\
|e_2\rangle&=\tfrac{i}{2}(|e_{10}\rangle-|e_{01}\rangle),&
|e_3\rangle&=\tfrac12(|e_{00}\rangle-|e_{11}\rangle).
\end{aligned}}
$$

To check the potentially delicate sign of the [Pauli Y gate](../../../../../pauli-y-gate.md) coefficient, use $Y|0\rangle=i|1\rangle$ and $Y|1\rangle=-i|0\rangle$. The four terms then give

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

[Linearity](../../../../../linearity.md) proves the expansion for every input [pure state](../../../../../pure-state.md). The environment coefficient vectors need not be normalized or mutually orthogonal. Consequently this expansion includes coherent combinations of [Pauli errors](../../../../../pauli-operator.md), rather than asserting that every [quantum channel](../../../../../quantum-channel.md) is a probabilistic [Pauli channel](../../../../../pauli-channel.md).

For the recovery probability, use the usual independent-use interpretation of the given [phase-flip channel](../../../../../phase-flip-channel.md): each of the three transmitted [qubits](../../../../../qubit.md) has a [Pauli Z gate](../../../../../pauli-z-gate.md) error independently with probability $q$. The [phase-flip repetition code](../../../../../phase-flip-repetition-code.md) uses logical codewords $|+++\rangle$ and $|---\rangle$. The decoding [Hadamard gates](../../../../../hadamard-gate.md) convert physical phase flips to bit flips because $HZH=X$. We can then analyze the two decoding [controlled-NOT gates](../../../../../controlled-not-gate.md) and the final [Toffoli gate](../../../../../toffoli-gate.md) directly, rather than assuming a recovery rule.

Let $b_1,b_2,b_3$ be the error bits after this basis conversion. For a logical basis input $t\in\{0,1\}$, the three data bits before inverse encoding are $t\oplus b_1,t\oplus b_2,t\oplus b_3$. The two [controlled-NOT gates](../../../../../controlled-not-gate.md) produce

$$
|t\oplus b_1\rangle\,|b_1\oplus b_2\rangle\,|b_1\oplus b_3\rangle.
$$

The [Toffoli gate](../../../../../toffoli-gate.md) flips the first wire when both of the last two bits are one. Its residual error is

$$
r(b)=b_1\oplus\bigl[(b_1\oplus b_2)(b_1\oplus b_3)\bigr]
=\begin{cases}0,&b_1+b_2+b_3\le1,\\1,&b_1+b_2+b_3\ge2.\end{cases}
$$

The last two wires carry an [error syndrome](../../../../../error-syndrome.md) independent of $t$. Thus this transformation preserves the amplitudes of an arbitrary superposition: zero or one phase error returns the original unknown [qubit](../../../../../qubit.md), while two or three phase errors leave the logical [Pauli X gate](../../../../../pauli-x-gate.md) applied to it. The probability of universally successful recovery is therefore

$$
\boxed{P_{\mathrm{success}}=(1-q)^3+3q(1-q)^2=1-3q^2+2q^3.}
$$

Equivalently, the decoded [quantum channel](../../../../../quantum-channel.md) is $\rho\mapsto(1-p_L)\rho+p_LX\rho X$, with [logical failure of the three-qubit phase-flip repetition code](../../../../../logical-failure-of-the-three-qubit-phase-flip-repetition-code.md) $p_L=3q^2-2q^3$. For $0<q<1/2$, the failure probability is below $q$, since $q-p_L=q(1-q)(1-2q)>0$. A special input that is a [Pauli X eigenstate](../../../../../pauli-x-eigenstate.md) is unchanged even by the residual logical error; this does not make the code correct that error on an unknown input. Its squared [quantum fidelity](../../../../../fidelity-of-quantum-states.md) with a particular pure input is $1-p_L+p_L|\langle\chi|X|\chi\rangle|^2$. If the errors on different channel uses are correlated, the marginal probability $q$ alone is insufficient: the general universal success probability is the probability of at most one error.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
