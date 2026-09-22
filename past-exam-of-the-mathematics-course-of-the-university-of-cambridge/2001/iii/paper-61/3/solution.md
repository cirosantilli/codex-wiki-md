<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The resource here is one copy of a [two-qubit Werner state](../../../../../two-qubit-werner-state.md), with the physical range $1/2<F\leq1$. The impossibility must include successful conditional branches of [local operations and classical communication](../../../../../local-operations-and-classical-communication.md); average monotonicity alone would not exclude probabilistic enhancement.

For a normalized two-[qubit](../../../../../qubit.md) [pure state](../../../../../pure-state.md) $|\chi\rangle=\sum_{i,j}M_{ij}|ij\rangle$, define its [concurrence](../../../../../concurrence.md) as $C(\chi)=2|\det M|$. Its [mixed-state concurrence of two qubits](../../../../../mixed-state-concurrence-of-two-qubits.md) is the [convex roof extension](../../../../../convex-roof-extension.md)

$$
C(\rho)=\inf_{\rho=\sum_j r_j|\chi_j\rangle\langle\chi_j|}
\sum_jr_jC(\chi_j).
$$

Combining near-optimal decompositions proves convexity. A [separable quantum state](../../../../../separable-quantum-state.md) has zero [concurrence](../../../../../concurrence.md), because it has a decomposition into product vectors with zero coefficient determinant.

First establish the [concurrence of a two-qubit Werner state](../../../../../concurrence-of-a-two-qubit-werner-state.md). A [pure state](../../../../../pure-state.md) with squared [Schmidt coefficients](../../../../../schmidt-coefficient.md) $\lambda,1-\lambda$ has $C=2\sqrt{\lambda(1-\lambda)}$. In this Schmidt basis a [maximally entangled state](../../../../../maximally-entangled-state.md) has coefficient matrix $V/\sqrt2$ with $V$ unitary. Its overlap magnitude is at most $(\sqrt\lambda+\sqrt{1-\lambda})/\sqrt2$, because $|V_{ii}|\leq1$. Thus the singlet overlap satisfies

$$
|\langle\Psi_-|\chi\rangle|^2\leq\frac{1+C(\chi)}2.
$$

Averaging any decomposition of $W_F$ gives $C(W_F)\geq2F-1$.

For the reverse bound use the orthonormal triplet vectors

$$
t_1=\Psi_+,\qquad t_2=\Phi_-,\qquad t_3=i\Phi_+,
\qquad
|\chi_{j,\pm}\rangle=\sqrt F\,|\Psi_-\rangle
\pm\sqrt{1-F}\,|t_j\rangle.
$$

Each is normalized, and direct evaluation of its two-by-two coefficient determinant gives $C(\chi_{j,\pm})=2F-1$. Their equally weighted six-state mixture has cancelled singlet–triplet coherences and triplet weight $(1-F)/3$, so it is exactly $W_F$. Hence

$$
\boxed{C(W_F)=2F-1.}
$$

Every fully specified record of an [LOCC](../../../../../local-operations-and-classical-communication.md) protocol gives a product [Kraus operator](../../../../../kraus-operator.md) $A\otimes B$ on the original pair. Local ancillas and discarded local outcomes can be included by refining the record. Write its success probability and normalized output as

$$
p=\operatorname{Tr}[(A\otimes B)W_F(A^\dagger\otimes B^\dagger)],
\qquad
\rho'=\frac{(A\otimes B)W_F(A^\dagger\otimes B^\dagger)}p.
$$

For invertible $A,B$, the [concurrence scaling under invertible local filters](../../../../../concurrence-scaling-under-invertible-local-filters.md) is

$$
C(\rho')=\frac{|\det A\det B|}{p}C(W_F).
$$

Here is a derivation of that scaling. Each pure coefficient matrix transforms to $AMB^{\mathsf T}$, so its unnormalized determinant is multiplied by $\det A\det B$. If that pure component has success probability $p_j$, its normalized [concurrence](../../../../../concurrence.md) is multiplied by $|\det A\det B|/p_j$, while its mixture weight becomes $r_jp_j/p$. Every ensemble average therefore scales by $|\det A\det B|/p$. Invertibility provides the reverse correspondence for every decomposition of $\rho'$, so taking both infima proves equality. If either local filter has rank one, the output is a [separable quantum state](../../../../../separable-quantum-state.md) and the desired bound is immediate.

It remains to show that the filter normalization cannot make this ratio exceed one. Use the [Pauli matrices](../../../../../pauli-matrices.md) representation

$$
W_F=\frac14\left(I\otimes I-w\sum_{j=1}^3\sigma_j\otimes\sigma_j\right),
\qquad w=\frac{4F-1}{3}\in(1/3,1].
$$

Write the positive matrices $X=A^\dagger A=a_0I+a\cdot\sigma$ and $Y=B^\dagger B=b_0I+b\cdot\sigma$, so $a_0\geq|a|$, $b_0\geq|b|$. Taking traces gives

$$
p=a_0b_0-w\,a\cdot b
\geq a_0b_0-|a||b|
\geq\sqrt{(a_0^2-|a|^2)(b_0^2-|b|^2)}
=|\det A\det B|.
$$

For completeness, squaring the middle comparison leaves $(a_0|b|-b_0|a|)^2\geq0$, and both sides are nonnegative. This proves the [single-copy Werner filtering normalization bound](../../../../../single-copy-werner-filtering-normalization-bound.md), and hence

$$
\boxed{C(\rho')\leq C(W_F)\quad\text{for every nonzero-probability branch}.}
$$

Forgetting some record information or grouping several successful records mixes these branch outputs; convexity preserves the same bound. Any alleged final $W_{F'}$ would therefore obey $2F'-1\leq2F-1$, contradicting $F'>F$. Thus **even heralded single-copy [LOCC](../../../../../local-operations-and-classical-communication.md) cannot produce the specified improved [Werner state](../../../../../werner-state.md)**. This proves that [single-copy Werner filtering cannot increase concurrence](../../../../../single-copy-werner-filtering-cannot-increase-concurrence.md). It does not forbid collective [entanglement distillation](../../../../../entanglement-distillation.md) from several noisy pairs; allowing additional shared entangled input copies would change the resource assumption.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
