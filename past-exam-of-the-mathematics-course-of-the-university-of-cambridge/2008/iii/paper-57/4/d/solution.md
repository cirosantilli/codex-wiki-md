<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With access to the uncontrolled physical gate, use [single-qubit process tomography](../../../../../../single-qubit-process-tomography.md). Prepare the positive [eigenstate](../../../../../../eigenstate.md) of each of $X,Y,Z$, apply $V$, and on independent copies measure each of $X,Y,Z$. Arbitrary single-qubit [rotation gates](../../../../../../rotation-gate.md) let one prepare these inputs and rotate each measurement into the [computational basis](../../../../../../computational-basis.md). The nine measured means are

$$
R_{ij}=\operatorname{Tr}\left[\sigma_iV\frac{I+\sigma_j}{2}V^\dagger\right]=\frac12\operatorname{Tr}(\sigma_iV\sigma_jV^\dagger),\qquad i,j\in\{x,y,z\}.
$$

They determine the real [rotation matrix](../../../../../../rotation-matrix.md) $R$ of the [Bloch vector](../../../../../../bloch-vector.md), and hence the action of $V$ on every [qubit](../../../../../../qubit.md) state. To see precisely what this identifies, suppose another unitary $U$ has the same action. Then $V^\dagger U$ commutes with every [Pauli matrix](../../../../../../pauli-matrices.md). Commuting with $Z$ makes it diagonal; commuting with $X$ makes its diagonal entries equal. Therefore $U=e^{i\gamma}V$.

Consequently **tomography determines $V$, and its [eigenvalues](../../../../../../eigenvalue.md), up to a common phase**. More explicitly, write a representative as $V=e^{i\gamma}(\cos a\,I-i\sin a\,\boldsymbol n\cdot\boldsymbol\sigma)$. Its [eigenvalues](../../../../../../eigenvalue.md) are $e^{i(\gamma-a)}$ and $e^{i(\gamma+a)}$, and its [Bloch vector](../../../../../../bloch-vector.md) action is [rotation](../../../../../../rotation-mathematics.md) through $2a$ about $\boldsymbol n$. The measured [rotation](../../../../../../rotation-mathematics.md) identifies the unordered relative [eigenphase](../../../../../../eigenphase.md) information; for example $\operatorname{Tr}R=1+2\cos(2a)$. Once a representative with a specified overall phase is supplied, diagonalizing that representative gives the corresponding two [eigenvalues](../../../../../../eigenvalue.md).

The common phase itself cannot be recovered with the stated uncontrolled access. Indeed, $(e^{i\gamma}V)\rho(e^{i\gamma}V)^\dagger=V\rho V^\dagger$ for every input, including inputs entangled with ancillas. Replacing $V$ by $e^{i\gamma}V$ therefore leaves every such preparation-and-measurement experiment unchanged, whereas it multiplies both [eigenvalues](../../../../../../eigenvalue.md) by $e^{i\gamma}$. For example, $I$ and $e^{i\gamma}I$ are indistinguishable physical gates under these operations. This proves that the request for absolute [eigenvalue](../../../../../../eigenvalue.md) phases needs an additional phase reference or controlled-gate assumption: the [global phase of an uncontrolled quantum gate is unobservable](../../../../../../global-phase-of-an-uncontrolled-quantum-gate-is-unobservable.md). The controlled powers in the earlier parts supply that extra resource, since $\operatorname{diag}(I,e^{i\gamma}V)$ changes a relative phase between the two control branches.

The practical advantages are that no unknown [eigenstate](../../../../../../eigenstate.md) preparation, controlled powers, entangling gates or inverse [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) are needed: a fixed set of single-qubit preparations and measurements suffices. The disadvantages are [statistical estimation](../../../../../../statistical-estimation.md) and the phase ambiguity just proved. Estimating the bounded [Pauli measurement](../../../../../../measurement-of-a-pauli-observable.md) means to additive accuracy $\epsilon$ at fixed confidence requires order $\epsilon^{-2}$ independent repetitions, giving the usual sampling cost for this direct procedure. The earlier [quantum phase estimation](../../../../../../quantum-phase-estimation.md) circuit uses $N$ phase [qubits](../../../../../../qubit.md) and high controlled powers to resolve scale $2^{-N}$ in one coherent experiment with a constant success bound; constructing those powers from controlled uses of $V$ costs $2^N-1$ gate calls, so its exponential-looking precision is not obtained with only $N$ uses of $V$. Repetitions can raise confidence. Finally, full process tomography grows exponentially with the number of system [qubits](../../../../../../qubit.md), whereas the eigenstate-based phase procedure can estimate a selected [eigenphase](../../../../../../eigenphase.md) without reconstructing the entire operator.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
