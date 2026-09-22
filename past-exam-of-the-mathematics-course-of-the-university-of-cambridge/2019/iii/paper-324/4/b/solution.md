<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a [reversible circuit](../../../../../../reversible-circuit.md) $T$ to compute an $L=O(n)$-bit representation of the angle into a workspace register, with all additional work bits retained:

$$
|x\rangle|0^L\rangle|0\rangle\xrightarrow{T}
|x\rangle|\theta_x\rangle|0\rangle.
$$

Write that representation as $\theta_x=\sum_{l=1}^L b_l(x)\alpha_l$, with known binary place values $\alpha_l$ (including the fixed scale and any integer bit). On the target, apply a [controlled unitary gate](../../../../../../controlled-unitary-gate.md) $R_y(2\alpha_l)$ controlled by each angle bit $b_l$. Rotations about the same axis add their angles, so their product is

$$
\prod_{l=1}^LR_y(2b_l\alpha_l)=R_y(2\theta_x),\qquad
R_y(2\theta_x)|0\rangle=\cos\theta_x|0\rangle+\sin\theta_x|1\rangle.
$$

Finally apply $T^\dagger$ to perform [uncomputation](../../../../../../uncomputation.md). The workspace returns to zero while the control register and rotated target remain unchanged; the construction works coherently on every superposition of $x$.

A [polynomial time](../../../../../../polynomial-time.md) classical calculation has a polynomial-size [reversible circuit](../../../../../../reversible-circuit.md) with [Toffoli gates](../../../../../../toffoli-gate.md), and each Toffoli gate has a constant-size decomposition into one-qubit and two-qubit gates. The $L$ controlled rotations are themselves two-qubit gates. Thus the total [quantum circuit](../../../../../../quantum-circuit-split.md) size is **$\operatorname{poly}(n)$**. This is the [binary-angle implementation of a quantum variable rotation](../../../../../../binary-angle-implementation-of-a-quantum-variable-rotation.md); the stipulated angle precision is understood.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
