<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the PDF's [Bell state](../../../../../../bell-state-split.md) labels throughout this question: its $\Phi_-$ is the antisymmetric [spin singlet state](../../../../../../spin-singlet-state.md), whereas $\Psi_\pm$ are the even-parity states. Write

$$
|a\rangle=a_0|0\rangle+a_1|1\rangle,\qquad
|b\rangle=b_0|0\rangle+b_1|1\rangle.
$$

Expanding the antisymmetric combination cancels its $00$ and $11$ components and gives

$$
\frac{|a\rangle|b\rangle-|b\rangle|a\rangle}{\sqrt2}
=(a_0b_1-a_1b_0)\frac{|01\rangle-|10\rangle}{\sqrt2}.
$$

The two normalized orthogonal vectors are the columns of a [unitary matrix](../../../../../../unitary-matrix.md) $U$. Its determinant $a_0b_1-a_1b_0$ has modulus one because $\det(U^\dagger U)=|\det U|^2=1$. Therefore

$$
\boxed{\frac{|a\rangle|b\rangle-|b\rangle|a\rangle}{\sqrt2}
=(\det U)|\Phi_-\rangle=e^{i\alpha}|\Phi_-\rangle.}
$$

This proves [collective-unitary covariance of the two-qubit singlet](../../../../../../collective-unitary-covariance-of-the-two-qubit-singlet.md): a common basis change alters only its [global phase](../../../../../../global-phase.md), and leaves its density projector unchanged.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
