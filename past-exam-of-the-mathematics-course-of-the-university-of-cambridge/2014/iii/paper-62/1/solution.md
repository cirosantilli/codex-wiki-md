<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Schmidt decomposition theorem](../../../../../schmidt-decomposition.md) states that a normalized vector in a finite-dimensional [tensor product](../../../../../tensor-product.md) $\mathcal H_A\otimes\mathcal H_B$ has the form $\sum_{j=1}^r s_j|u_j\rangle|v_j\rangle$, where the two families are orthonormal, $s_j>0$, $\sum_js_j^2=1$, and $r\leq\min(\dim\mathcal H_A,\dim\mathcal H_B)$. Extending each family to an [orthonormal basis](../../../../../orthonormal-basis.md) for two [qubits](../../../../../qubit.md) gives

$$
|\psi\rangle=\lambda_0|00\rangle+\lambda_1|11\rangle,\qquad
\lambda_i\geq0,\quad\lambda_0^2+\lambda_1^2=1.
$$

The nonzero [Schmidt coefficients](../../../../../schmidt-coefficient.md) can be made positive by absorbing phases into the basis vectors. Both are positive exactly when the [pure state](../../../../../pure-state.md) is entangled. A [product state](../../../../../product-state.md) has [Schmidt rank](../../../../../schmidt-rank.md) one, so one coefficient is zero; the source's assertion of two positive coefficients for every pure state needs this exception.

Choose each local [orthonormal basis](../../../../../orthonormal-basis.md) independently as the computational basis. In that basis $\sigma_z=|0\rangle\langle0|-|1\rangle\langle1|$. This is a local change of coordinates, implemented by separate [unitary matrices](../../../../../unitary-matrix.md), rather than a physical restriction on the original [quantum state](../../../../../quantum-state.md). The associated [Pauli operators](../../../../../pauli-operator.md) supply the other two local axes. Up to an irrelevant common phase, each unitary change of [qubit](../../../../../qubit.md) basis corresponds to a rotation of its [Bloch sphere](../../../../../bloch-sphere.md).

Put $s=2\lambda_0\lambda_1$. The [Schmidt-basis Pauli correlation tensor](../../../../../schmidt-basis-pauli-correlation-tensor.md) is diagonal. The [Pauli operators](../../../../../pauli-operator.md) $\sigma_x\otimes\sigma_x$ exchange $|00\rangle$ and $|11\rangle$, while $\sigma_y\otimes\sigma_y$ do so with minus signs, and $\sigma_z\otimes\sigma_z$ leaves both fixed. Hence

$$
\langle\sigma_x\otimes\sigma_x\rangle=s,\qquad
\langle\sigma_y\otimes\sigma_y\rangle=-s,\qquad
\langle\sigma_z\otimes\sigma_z\rangle=1.
$$

Mixed components vanish: those containing one $z$ and one transverse [Pauli operator](../../../../../pauli-operator.md) map the occupied basis vectors outside their span, while the $xy$ and $yx$ matrix elements are purely imaginary and cancel for real [Schmidt coefficients](../../../../../schmidt-coefficient.md). By bilinearity, for arbitrary real vectors,

$$
\boxed{P(\mathbf a,\mathbf b)=s(a_xb_x-a_yb_y)+a_zb_z.}
$$

For a [CHSH inequality](../../../../../chsh-inequality.md) test take unit [measurement in quantum mechanics](../../../../../quantum-measurement-split.md) axes

$$
\mathbf a=\mathbf e_z,\quad\mathbf a'=\mathbf e_x,\qquad
\mathbf b=\frac{\mathbf e_z+s\mathbf e_x}{\sqrt{1+s^2}},\quad
\mathbf b'=\frac{\mathbf e_z-s\mathbf e_x}{\sqrt{1+s^2}}.
$$

These [CHSH axes for an entangled pure two-qubit state](../../../../../chsh-axes-for-an-entangled-pure-two-qubit-state.md) give

$$
\boxed{S=P(\mathbf a,\mathbf b)+P(\mathbf a,\mathbf b')+P(\mathbf a',\mathbf b)-P(\mathbf a',\mathbf b')
=2\sqrt{1+s^2}>2\quad(s>0).}
$$

The local bound is two: for each hidden state, $A(B+B')+A'(B-B')$ is $\pm2$ when all four outcomes are $\pm1$, and averaging cannot increase its absolute value. Thus **every entangled pure two-qubit state violates a CHSH inequality**, the content of [Gisin's theorem](../../../../../gisin-s-theorem.md). A [product state](../../../../../product-state.md) has $s=0$ and does not violate it, so the unqualified final claim in the question is false for that case. The maximum $2\sqrt2$ occurs for equal [Schmidt coefficients](../../../../../schmidt-coefficient.md). This excludes [local hidden-variable theories](../../../../../local-hidden-variable-theory.md) satisfying [measurement independence](../../../../../measurement-independence.md), but does not permit faster-than-light signalling: the local [reduced density matrix](../../../../../reduced-density-matrix.md) and its [measurement in quantum mechanics](../../../../../quantum-measurement-split.md) probabilities are unchanged by the remote choice of axis.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
