<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the known bit string $y$, define the [Pauli gate](../../../../../../pauli-gate.md) product $T_y=\bigotimes_{j=0}^{N-1}Z_j^{y_j}$. Its diagonal action is $T_y|x\rangle=(-1)^{x\cdot y}|x\rangle$, where the [binary inner product](../../../../../../binary-inner-product.md) is taken modulo two. The [Hadamard transform](../../../../../../hadamard-transform.md) produces $|\phi_y\rangle=H^{\otimes N}|y\rangle=T_y|\phi\rangle$. Thus the required [vectors](../../../../../../vector.md) for [Grover search with a nonzero reflection label](../../../../../../grover-search-with-a-nonzero-reflection-label.md) are

$$
\boxed{|\widetilde\Psi_g\rangle=\frac1{\sqrt M}\sum_{f(x)=1}(-1)^{x\cdot y}|x\rangle,\qquad |\widetilde\Psi_b\rangle=\frac1{\sqrt{2^N-M}}\sum_{f(x)=0}(-1)^{x\cdot y}|x\rangle.}
$$

They remain [orthonormal](../../../../../../orthonormal-set.md) and $|\phi_y\rangle=\sin\theta|\widetilde\Psi_g\rangle+\cos\theta|\widetilde\Psi_b\rangle$. The new iterate is $G_y=(2|\phi_y\rangle\langle\phi_y|-I)U_f$. Since $T_y$ commutes with the diagonal [marked-state phase oracle](../../../../../../marked-state-phase-oracle.md) and $T_y^2=I$,

$$
G_y=T_yGT_y.
$$

Consequently its [matrix](../../../../../../matrix.md) on the signed [basis](../../../../../../basis.md) is exactly the [rotation matrix](../../../../../../rotation-matrix.md) in part (a), proving the claimed equivalence of the two evolutions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
