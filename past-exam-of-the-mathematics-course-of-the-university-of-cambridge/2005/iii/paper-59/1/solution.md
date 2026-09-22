<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Apply the [Schmidt decomposition](../../../../../schmidt-decomposition.md) to the bipartite [pure state](../../../../../pure-state.md). Local [unitary operators](../../../../../unitary-operator.md) put it in the form $|\psi_\theta\rangle=\cos\theta|00\rangle+\sin\theta|11\rangle$, with $0<\theta\leq\pi/4$ after interchanging basis vectors. Both [Schmidt coefficients](../../../../../schmidt-coefficient.md) are nonzero because the state is [entangled](../../../../../entangled-state.md). Put $s=\sin2\theta>0$.

For this state, direct application of the [Pauli operators](../../../../../pauli-operator.md) gives

$$
\langle\sigma_z\otimes\sigma_z\rangle=1,\qquad
\langle\sigma_x\otimes\sigma_x\rangle=s,\qquad
\langle\sigma_z\otimes\sigma_x\rangle=\langle\sigma_x\otimes\sigma_z\rangle=0.
$$

For example $\sigma_x\otimes\sigma_x$ interchanges $|00\rangle$ and $|11\rangle$, giving $2\cos\theta\sin\theta$; the crossed products take these two kets into their [orthogonal complement](../../../../../orthogonal-complement.md).

Choose the [CHSH axes for an entangled pure two-qubit state](../../../../../chsh-axes-for-an-entangled-pure-two-qubit-state.md):

$$
A_0=\sigma_z,\qquad A_1=\sigma_x,\qquad
B_0=\frac{\sigma_z+s\sigma_x}{\sqrt{1+s^2}},\qquad
B_1=\frac{\sigma_z-s\sigma_x}{\sqrt{1+s^2}}.
$$

Their associated [Bloch vectors](../../../../../bloch-vector.md) have unit length, so each is a valid two-outcome [projective measurement](../../../../../projective-measurement.md) with projectors $(I\pm A_i)/2$ or $(I\pm B_j)/2$. The correlation combination is

$$
\begin{aligned}
\mathcal S&=\langle A_0\otimes(B_0+B_1)+A_1\otimes(B_0-B_1)\rangle\\
&=\frac{2\langle\sigma_z\otimes\sigma_z\rangle+2s\langle\sigma_x\otimes\sigma_x\rangle}{\sqrt{1+s^2}}
=2\sqrt{1+s^2}.
\end{aligned}
$$

A local hidden-variable assignment with outcomes $\pm1$ gives absolute value at most two: exactly one of $b_0+b_1$ and $b_0-b_1$ vanishes, while the other is $\pm2$. Averaging these assignments preserves that bound, which is the [CHSH inequality](../../../../../chsh-inequality.md).

Therefore **$\boxed{\mathcal S=2\sqrt{1+\sin^22\theta}>2}$**. For the original state $(U\otimes V)|\psi_\theta\rangle$, conjugate Alice's observables by $U$ and Bob's by $V$. These conjugations rotate their measurement axes and preserve all the displayed correlations. Thus every [entangled](../../../../../entangled-state.md) pure two-qubit state has the requested violating axes. The maximally [entangled](../../../../../entangled-state.md) case gives $2\sqrt2$, while the unentangled limit merely saturates two.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
