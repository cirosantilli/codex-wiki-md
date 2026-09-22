<h1 id="16b/solution">Solution</h1>

↑ **Parent:** [16B](../16b.md)

Expand the initial [wavefunction](../../../../../wave-function.md) in the complete orthonormal [energy eigenstates](../../../../../energy-eigenstate.md), with $c_n=\langle\psi_n,\Psi(0)\rangle$. The [unitary time evolution](../../../../../unitary-time-evolution.md) is

$$
\boxed{\Psi(x,t)=\sum_{n=1}^\infty c_ne^{-iE_nt/\hbar}\psi_n(x),\qquad\sum_{n=1}^\infty|c_n|^2=1.}
$$

On the two-dimensional subspace spanned by $\psi_1,\psi_2$, the [observable](../../../../../observable.md) has [matrix](../../../../../matrix.md) $\begin{pmatrix}2&-1\\-1&2\end{pmatrix}$. Its normalized [eigenvectors](../../../../../eigenvector.md) are the symmetric and antisymmetric combinations. A complete orthonormal [eigenbasis](../../../../../eigenbasis.md) is therefore

$$
\boxed{\phi_1=\frac{\psi_1+\psi_2}{\sqrt2},\quad A\phi_1=\phi_1;\qquad
\phi_2=\frac{\psi_1-\psi_2}{\sqrt2},\quad A\phi_2=3\phi_2;\qquad
\phi_n=\psi_n,\quad A\phi_n=0\ (n\geq3).}
$$

The [eigenvalues](../../../../../eigenvalue.md) are $1,3,0$, with $0$ infinitely degenerate. The first two are nondegenerate, regardless of the distinct energies $E_n$.

The first [measurement in quantum mechanics](../../../../../quantum-measurement-split.md), with outcome $3$, leaves the state $\phi_2$ up to an irrelevant phase. At time $t$ it has become

$$
\Psi(t)=\frac{e^{-iE_1t/\hbar}\psi_1-e^{-iE_2t/\hbar}\psi_2}{\sqrt2}.
$$

Its [probability amplitude](../../../../../probability-amplitude.md) for outcome $1$ is

$$
\langle\phi_1,\Psi(t)\rangle=\frac12\left(e^{-iE_1t/\hbar}-e^{-iE_2t/\hbar}\right).
$$

The [Born rule](../../../../../born-rule.md) gives the [two-level observable transition probability](../../../../../two-level-observable-transition-probability.md)

$$
\boxed{\mathbb P(A(t)=1\mid A(0)=3)=\sin^2\left(\frac{(E_2-E_1)t}{2\hbar}\right).}
$$

## ↑ Ancestors (10)

1. [16B](../16b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
