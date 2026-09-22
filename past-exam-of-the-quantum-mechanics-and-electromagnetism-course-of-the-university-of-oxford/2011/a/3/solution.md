<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a nonzero [quantum state](../../../../quantum-state.md) $\psi$ and a [self-adjoint operator](../../../../self-adjoint-operator.md) $A$, the [expectation value](../../../../expectation-value.md) and [standard deviation](../../../../standard-deviation.md) of its measurement are

$$
\boxed{a=\mathbb E_\psi(A)=\frac{\langle\psi,A\psi\rangle}{\langle\psi,\psi\rangle},\qquad
\Delta_\psi(A)=\frac{\|(A-aI)\psi\|}{\|\psi\|}=\sqrt{\mathbb E_\psi(A^2)-a^2}.}
$$

The squared deviation is also called the [variance](../../../../variance-split.md) of the [observable](../../../../observable.md). All displayed products are understood on [quantum states](../../../../quantum-state.md) for which the relevant moments exist. Self-adjointness gives $\overline{\langle\psi,A\psi\rangle}=\langle A\psi,\psi\rangle=\langle\psi,A\psi\rangle$, so $a$ is real. Expanding the squared [norm](../../../../norm.md) gives the [variance](../../../../variance-split.md) expression. A [norm](../../../../norm.md) is nonnegative and is zero exactly for the zero [vector](../../../../vector.md), hence $\Delta_\psi(A)=0$ precisely when $A\psi=a\psi$. Thus **zero dispersion is equivalent to being an [eigenstate](../../../../eigenstate.md)**.

For bounded $H$, the [operator exponential](../../../../operator-exponential.md) is the [norm](../../../../norm.md)-convergent power series

$$
U_t=\sum_{n=0}^\infty\frac{(-itH/\hbar)^n}{n!}.
$$

For a general unbounded [self-adjoint](../../../../self-adjoint-operator.md) [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md), the [spectral theorem](../../../../spectral-theorem.md) defines the same notation by

$$
U_t=\int_{\mathbb R}e^{-itE/\hbar}\,dP_H(E).
$$

This definition does not require the power series to converge on every [quantum state](../../../../quantum-state.md). [complex conjugation](../../../../complex-conjugation.md) of the spectral multiplier gives $U_t^*=U_{-t}$, and multiplication of the phases gives $U_{-t}U_t=I$. Thus **$U_t$ is [unitary](../../../../unitary-connection.md)**, preserves the [quantum state](../../../../quantum-state.md) [norm](../../../../norm.md), and has $U_0=I$.

For initial data in the domain of $H$, differentiating the spectral expression yields $\partial_tU_t\psi_0=-(i/\hbar)HU_t\psi_0$. Consequently

$$
\boxed{\psi_t=U_t\psi_0}
$$

solves the [Schrödinger equation](../../../../schrodinger-equation.md) with the prescribed initial [quantum state](../../../../quantum-state.md). Uniqueness follows by differentiating $U_{-t}\psi_t$: the two terms cancel, leaving the constant $\psi_0$.

In the two-dimensional energy [basis](../../../../basis.md), expand the initial [quantum state](../../../../quantum-state.md) as $\psi_0=c_1\Psi_1+c_2\Psi_2$. Each energy [eigenvector](../../../../eigenvector.md) receives its own phase under the [operator exponential](../../../../operator-exponential.md), giving

$$
\boxed{\psi_t=c_1e^{-itE_1/\hbar}\Psi_1+c_2e^{-itE_2/\hbar}\Psi_2.}
$$

This is the general solution because every initial [vector](../../../../vector.md) has a unique [basis](../../../../basis.md) expansion.

In that [orthonormal basis](../../../../orthonormal-basis.md) the other [observable](../../../../observable.md) has the real symmetric [matrix](../../../../matrix.md)

$$
[A]=\begin{pmatrix}\cos2\alpha&\sin2\alpha\\\sin2\alpha&-\cos2\alpha\end{pmatrix}.
$$

Its conjugate transpose equals itself, so it is [self-adjoint](../../../../self-adjoint-operator.md). Also $A^2=I$ and $\operatorname{tr}A=0$, giving [eigenvalues](../../../../eigenvalue.md) $+1$ and $-1$. Direct substitution gives the normalized [orthogonal](../../../../orthogonal-vectors.md) [eigenvectors](../../../../eigenvector.md)

$$
\boxed{v_+=\cos\alpha\,\Psi_1+\sin\alpha\,\Psi_2,\qquad
v_-=-\sin\alpha\,\Psi_1+\cos\alpha\,\Psi_2.}
$$

An irrelevant global phase may multiply either [vector](../../../../vector.md). With the chosen lower [eigenstate](../../../../eigenstate.md) initially,

$$
\boxed{\psi_t=-\sin\alpha\,e^{-itE_1/\hbar}\Psi_1+\cos\alpha\,e^{-itE_2/\hbar}\Psi_2.}
$$

The [Born rule](../../../../born-rule.md) says that the [probability](../../../../probability.md) for the higher [eigenstate](../../../../eigenstate.md) is $|\langle v_+,\psi_t\rangle|^2$. Its amplitude is $\sin\alpha\cos\alpha(e^{-itE_2/\hbar}-e^{-itE_1/\hbar})$. Using $|e^{-iu}-e^{-iv}|^2=4\sin^2((u-v)/2)$ gives

$$
\boxed{P_+(t)=\sin^2(2\alpha)\sin^2\left(\frac{(E_2-E_1)t}{2\hbar}\right).}
$$

This is the [transition probability for a rotated two-level observable](../../../../transition-probability-for-a-rotated-two-level-observable.md). Its time dependence comes from the relative phase between two energy [eigenstates](../../../../eigenstate.md). If their energies coincide, or if the measured [observable](../../../../observable.md) has the energy [eigenvectors](../../../../eigenvector.md) as its [eigenvectors](../../../../eigenvector.md), this transition [probability](../../../../probability.md) is zero at all times.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the quantum mechanics and electromagnetism course of the University of Oxford](../../../split.md)
5. [Quantum mechanics and electromagnetism course of the University of Oxford](../../../../quantum-mechanics-and-electromagnetism-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
