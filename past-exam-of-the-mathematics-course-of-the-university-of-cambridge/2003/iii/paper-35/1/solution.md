<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Pauli group](../../../../../pauli-group.md) includes scalar phases $\mathcal Z=\{\pm I,\pm iI\}$. For a nonzero [stabilizer code](../../../../../stabilizer-code.md), its Abelian subgroup must satisfy $-I\notin S$. Otherwise a common positive [eigenvector](../../../../../eigenvector.md) would satisfy $-|\psi\rangle=|\psi\rangle$ and vanish; for example $S=\{I,-I\}$ is Abelian but yields no nonzero [stabilizer code](../../../../../stabilizer-code.md). We impose this standard admissibility condition.

Every element of such a [stabilizer group](../../../../../stabilizer-group.md) is Hermitian and squares to $I$: an imaginary-phase Pauli with square $-I$ is excluded. The associated [stabilizer code](../../../../../stabilizer-code.md) and its [orthogonal projector](../../../../../orthogonal-projection.md) are

$$
\mathcal C_S=\{|\psi\rangle:s|\psi\rangle=|\psi\rangle\text{ for every }s\in S\},\qquad
P=\frac1{|S|}\sum_{s\in S}s.
$$

The group multiplication proves $P^2=P$, Hermiticity gives $P^\dagger=P$, and its range is exactly the common positive eigenspace. If $S$ has $r$ independent generators, $|S|=2^r$. Every nonidentity element has trace zero, while $\operatorname{tr}I=2^n$, so

$$
\boxed{\dim\mathcal C_S=\operatorname{tr}P=2^{n-r}.}
$$

Thus it encodes $k=n-r$ [logical qubits](../../../../../logical-qubit.md).

For the [symplectic representation of a stabilizer code](../../../../../symplectic-representation-of-a-stabilizer-code.md), label $i^tX^aZ^b$ by $(a,b)\in\mathbb F_2^{2n}$, ignoring scalar phase. Products add labels, and

$$
(X^aZ^b)(X^{a'}Z^{b'})=(-1)^{a\cdot b'+b\cdot a'}(X^{a'}Z^{b'})(X^aZ^b).
$$

This is the nondegenerate alternating form $\omega((a,b),(a',b'))=a\cdot b'+b\cdot a'$ on the [binary symplectic space of Pauli labels](../../../../../binary-symplectic-space-of-pauli-labels.md). The image $L$ of $S$ is an r-dimensional [isotropic subspace of a binary symplectic space](../../../../../isotropic-subspace-of-a-binary-symplectic-space.md), since the generators commute and no nontrivial scalar lies in $S$. Consequently $L\subseteq L^\perp$ and $r\le n$. A binary generator [matrix](../../../../../matrix.md) $(A\mid B)$ satisfies $AB^T+BA^T=0$. Conversely an isotropic subspace can be lifted by choosing commuting Hermitian generators with independent labels; their products cannot equal $-I$, and the [orthogonal projector](../../../../../orthogonal-projection.md) formula supplies the [stabilizer code](../../../../../stabilizer-code.md). The labels of the [centralizer of a stabilizer group](../../../../../centralizer-of-a-stabilizer-group.md) are $L^\perp$, with nontrivial logical actions represented by $L^\perp\setminus L$.

For an example, the three-[qubit](../../../../../qubit.md) [bit-flip repetition code](../../../../../bit-flip-repetition-code.md) has $S=\langle Z_1Z_2,Z_2Z_3\rangle$ and $\mathcal C_S=\operatorname{span}\{|000\rangle,|111\rangle\}$. Its two binary rows have zero X part and Z parts $110,011$. The errors $I,X_1,X_2,X_3$ have respective [error syndromes](../../../../../error-syndrome.md) $00,10,11,01$, so all single bit flips can be corrected. This is not a [stabilizer code](../../../../../stabilizer-code.md) correcting every single-[qubit](../../../../../qubit.md) error: $Z_1$ acts as a nontrivial logical phase error.

Let $C(S)$ denote the Pauli centralizer. The exact [Pauli error criterion for a stabilizer code](../../../../../pauli-error-criterion-for-a-stabilizer-code.md) is

$$
\boxed{\text{For all }E_a,E_b\in\mathbb E,\quad E_a^\dagger E_b\in\mathcal ZS\ \text{or}\ E_a^\dagger E_b\notin C(S).}
$$

Equivalently, no difference of error labels lies in $L^\perp\setminus L$. The scalar phases in $\mathcal ZS$ are essential: an error product $-I$ is harmless even though it is not in $S$.

We prove the criterion. For $T=E_a^\dagger E_b$ outside $C(S)$, some $s\in S$ anticommutes with $T$. Since $sP=Ps=P$, we have $PTP=PsTsP=-PTP$, hence $PTP=0$. If $T=\lambda s\in\mathcal ZS$, then $PTP=\lambda P$. If $T\in C(S)\setminus\mathcal ZS$, it restricts to a [unitary operator](../../../../../unitary-operator.md) on the [stabilizer code](../../../../../stabilizer-code.md), but

$$
\operatorname{tr}(PT)=|S|^{-1}\sum_{s\in S}\operatorname{tr}(sT)=0:
$$

no $sT$ is scalar. A scalar restriction would have scalar coefficient zero by this trace equation, contradicting unitarity. Thus this third case is not scalar.

To justify why scalar compressions are exactly what correction requires, suppose one recovery corrects every $E_a$. Dilate that recovery to an isometry $W$ including its auxiliary system. Correct recovery of every pure [stabilizer code](../../../../../stabilizer-code.md) state gives $WE_a|\psi\rangle=|\psi\rangle\otimes|\eta_a\rangle$. The auxiliary state is independent of $\psi$: linearity on basis states and their superpositions forces their auxiliary vectors to coincide. Preservation of inner products then gives

$$
\langle\phi|E_a^\dagger E_b|\psi\rangle
=\langle\phi|\psi\rangle\langle\eta_a|\eta_b\rangle,
$$

which is the [Knill--Laflamme condition](../../../../../knill-laflamme-condition.md) $PE_a^\dagger E_bP=c_{ab}P$. The three cases above prove necessity of the boxed criterion.

For sufficiency, put errors in the same class when $E_a^\dagger E_b\in\mathcal ZS$. They act identically on the [stabilizer code](../../../../../stabilizer-code.md) up to scalar phase, so give the same error-image subspace. Under the criterion, different classes give mutually orthogonal subspaces $E_a\mathcal C_S$, because their cross-compressions vanish. Measure which of these subspaces is occupied and apply the inverse of a representative error. This returns every [stabilizer code](../../../../../stabilizer-code.md) state unchanged; extend the recovery on the orthogonal complement by preparing any fixed [stabilizer code](../../../../../stabilizer-code.md) state. Linearity also corrects any valid noise channel whose [Kraus operators](../../../../../kraus-operator.md) are linear combinations of the specified errors: within each syndrome all amplitudes multiply the same logical state, and trace preservation normalizes the recovered state. This proves sufficiency, including degenerate error classes.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
