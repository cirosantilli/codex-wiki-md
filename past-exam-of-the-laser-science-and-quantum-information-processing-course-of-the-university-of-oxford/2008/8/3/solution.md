<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the ordered [computational basis](../../../../computational-basis.md) $(|00\rangle,|01\rangle,|10\rangle,|11\rangle)$, with qubit 1 written first. **The half-time gate requires a branch convention.** Even stationary [Hamiltonian](../../../../hamiltonian.md) evolution with $W(2\tau)=\mathrm{SWAP}$ does not uniquely specify $W(\tau)$: different accumulated [eigenstate](../../../../eigenstate.md) phases can agree at $2\tau$ and differ at $\tau$. In particular, both $S$ and $S^\dagger$ below square to [SWAP gate](../../../../swap-gate.md) and leave $|00\rangle,|11\rangle$ unchanged. Adopt the conventional continuous isotropic [exchange interaction](../../../../exchange-interaction.md) branch, with a relative singlet phase increasing from $0$ to $\pi$ during the full pulse. This is the [exchange square-root branch convention](../../../../exchange-square-root-branch-convention.md).

The symmetric and antisymmetric [eigenstates](../../../../eigenstate.md)

$$
|\psi_+\rangle=\frac{|01\rangle+|10\rangle}{\sqrt2},\qquad
|\psi_-\rangle=\frac{|01\rangle-|10\rangle}{\sqrt2}
$$

have [SWAP gate](../../../../swap-gate.md) [eigenvalues](../../../../eigenvalue.md) $+1,-1$. Let $P_-=|\psi_-\rangle\langle\psi_-|$ and $P_+=I_4-P_-$ be their antisymmetric and symmetric [orthogonal projectors](../../../../orthogonal-projection.md). The adopted exchange evolution is

$$
W(t)=P_++e^{i\pi t/(2\tau)}P_-,\qquad
H_{\mathrm{ex}}=-\frac{\pi\hbar}{2\tau}P_-.
$$

For effective spin-one-half [qubits](../../../../qubit.md), $H_{\mathrm{ex}}=\pi\hbar(X_1X_2+Y_1Y_2+Z_1Z_2-I_4)/(8\tau)$, an isotropic [exchange interaction](../../../../exchange-interaction.md) plus an energy offset that fixes the common phase. At half time choose $+1$ on the symmetric sector and $+i$ on the antisymmetric sector, the conventional principal square-root value of $-1$. Hence the [square root of the SWAP gate](../../../../square-root-of-the-swap-gate.md) is

$$
\boxed{S=\sqrt{\mathrm{SWAP}}=P_++iP_-
=\begin{pmatrix}
1&0&0&0\\
0&(1+i)/2&(1-i)/2&0\\
0&(1-i)/2&(1+i)/2&0\\
0&0&0&1
\end{pmatrix}.}
$$

Thus $S|00\rangle=|00\rangle$, $S|11\rangle=|11\rangle$, $S|01\rangle=a|01\rangle+b|10\rangle$ and $S|10\rangle=b|01\rangle+a|10\rangle$, where $a=(1+i)/2$ and $b=(1-i)/2$. The identities $a^2+b^2=0$ and $2ab=1$ verify $S^2=\mathrm{SWAP}$, and the projector form proves [unitarity](../../../../unitary-operator.md). The endpoint truth table alone would allow other [matrix square roots](../../../../square-root-of-a-matrix.md); the stated exchange branch supplies the additional physical assumption.

For the network, fix the [Pauli Z gate](../../../../pauli-z-gate.md), [Hadamard gate](../../../../hadamard-gate.md) and [S gate](../../../../s-gate.md) conventions

$$
Z=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad
H=\frac1{\sqrt2}\begin{pmatrix}1&1\\1&-1\end{pmatrix},\qquad
P=\sqrt Z=\begin{pmatrix}1&0\\0&i\end{pmatrix}.
$$

The letter $P$ distinguishes this local [S gate](../../../../s-gate.md) from the two-[qubit](../../../../qubit.md) exchange gate $S$. In particular $P^2=Z$; replacing $P$ by $P^\dagger$ changes the network. Subscripts specify the acted-on [qubit](../../../../qubit.md): $Z_1=Z\otimes I_2$, $P_2=I_2\otimes P$ and $H_2=I_2\otimes H$. Operators act **rightmost first**, so the printed [quantum circuit](../../../../quantum-circuit-split.md) is

$$
U=H_2SZ_1SP_2H_2.
$$

First multiply the central two exchange pulses. Since $a^2-b^2=i$, their off-diagonal terms cancel:

$$
K=SZ_1S=\operatorname{diag}(1,i,-i,-1),\qquad
D=KP_2=\operatorname{diag}(1,-1,-i,-i).
$$

This reduces the entire network to $U=H_2DH_2$. Its action on all four [computational basis](../../../../computational-basis.md) states, retaining every relative [quantum phase](../../../../quantum-phase.md), is

$$
\begin{array}{c|c|c|c}
\text{input}&\text{after rightmost }H_2&\text{after }D&\text{after leftmost }H_2\\\hline
|00\rangle&(|00\rangle+|01\rangle)/\sqrt2&(|00\rangle-|01\rangle)/\sqrt2&|01\rangle\\
|01\rangle&(|00\rangle-|01\rangle)/\sqrt2&(|00\rangle+|01\rangle)/\sqrt2&|00\rangle\\
|10\rangle&(|10\rangle+|11\rangle)/\sqrt2&-i(|10\rangle+|11\rangle)/\sqrt2&-i|10\rangle\\
|11\rangle&(|10\rangle-|11\rangle)/\sqrt2&-i(|10\rangle-|11\rangle)/\sqrt2&-i|11\rangle
\end{array}
$$

Equivalently,

$$
\boxed{U=\begin{pmatrix}0&1&0&0\\1&0&0&0\\0&0&-i&0\\0&0&0&-i\end{pmatrix}
=|0\rangle\langle0|\otimes X-i|1\rangle\langle1|\otimes I_2.}
$$

It flips the second [qubit](../../../../qubit.md) when the first is zero and contributes $-i$ when the first is one. That conditional phase cannot be discarded as a [global phase](../../../../global-phase.md).

To obtain the standard [CNOT gate](../../../../controlled-not-gate.md) controlled by qubit 1, append an $X$ gate to qubit 2 and $P$ to qubit 1. They commute, and

$$
\boxed{\mathrm{CNOT}_{1\to2}=P_1X_2U
=P_1X_2H_2SZ_1SP_2H_2
=\begin{pmatrix}1&0&0&0\\0&1&0&0\\0&0&0&1\\0&0&1&0\end{pmatrix}.}
$$

For control zero, $X_2$ undoes the original flip. For control one, it supplies the desired flip and $P_1$ cancels the phase because $i(-i)=1$. This [phase-corrected exchange network for a CNOT gate](../../../../phase-corrected-exchange-network-for-a-cnot-gate.md) realizes the standard gate exactly with the declared conventions.

Finally, $S|01\rangle=(e^{i\pi/4}|01\rangle+e^{-i\pi/4}|10\rangle)/\sqrt2$ has equal [Schmidt coefficients](../../../../schmidt-coefficient.md) and is maximally entangled: a half exchange creates [quantum entanglement](../../../../entangled-state.md) although a full [SWAP gate](../../../../swap-gate.md) does not. More constructively, the network above produces a [CNOT gate](../../../../controlled-not-gate.md) from two half exchanges and local gates. Since [CNOT gates](../../../../controlled-not-gate.md) and arbitrary single-[qubit](../../../../qubit.md) [unitary operators](../../../../unitary-operator.md) form a [universal quantum gate set](../../../../universal-quantum-gate-set.md), **the [square root of the SWAP gate](../../../../square-root-of-the-swap-gate.md) and arbitrary single-[qubit](../../../../qubit.md) gates are universal**. The alternative inverse exchange branch remains entangling and universal, but its phases and local correction must be recomputed consistently.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [8](../../8-split.md)
3. [2008](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
