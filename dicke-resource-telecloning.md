# Dicke-resource telecloning

↑ **Parent:** [Quantum teleportation](quantum-teleportation.md)

For odd $n=2k+1$, a symmetric [quantum teleportation](quantum-teleportation.md) resource can encode an unknown [qubit](qubit.md) into $E(\alpha|0\rangle+\beta|1\rangle)=\alpha|D_k^n\rangle+\beta|D_{k+1}^n\rangle$. Begin with $|D_{k+1}^{n+1}\rangle$, apply a [controlled-NOT gate](controlled-not-gate.md) from the input to the sender's resource qubit, apply a [Pauli X gate](pauli-x-gate.md) to that resource qubit and a [Hadamard gate](hadamard-gate.md) to the input, and measure those two qubits. The four unnormalized remaining vectors are $E|\psi\rangle/2$, $EX|\psi\rangle/2$, $EZ|\psi\rangle/2$ and $EXZ|\psi\rangle/2$. Each outcome has probability $1/4$. Since $X^{\otimes n}$ interchanges $|D_k^n\rangle$ and $|D_{k+1}^n\rangle$, and $Z^{\otimes n}$ acts as logical $Z$ up to the common phase $(-1)^k$, local Pauli corrections make the output independent of the result. The [one-qubit reduction of Dicke-state superpositions](one-qubit-reduction-of-dicke-state-superpositions.md) gives

$$
\rho=\frac1n\begin{pmatrix}k+|\alpha|^2&(k+1)\alpha\beta^*\\(k+1)\alpha^*\beta&k+|\beta|^2\end{pmatrix},\qquad \langle\psi|\rho|\psi\rangle=\frac{k+1+2k|\alpha|^2|\beta|^2}{n}.
$$

For $n>1$ this distributes imperfect copies, as required by the [no-cloning theorem](no-cloning-theorem.md). For $n=1$ it reduces to exact [quantum teleportation](quantum-teleportation.md).

## ↑ Ancestors (7)

1. [Quantum teleportation](quantum-teleportation.md)
2. [Local operations and classical communication](local-operations-and-classical-communication.md)
3. [Bell state](bell-state-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/1/b/solution.md)
