<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Dilate the second [quantum channel](../../../../../../quantum-channel.md) by an isometry $W:B_1\longrightarrow B_2E_2$, and set $\tau_{RB_2E_2}=(I_R\otimes W)\sigma_{RB_1}(I_R\otimes W^\dagger)$. Its $RB_2$ marginal is the final output. Isometry invariance of [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) gives $S(B_1)_\sigma=S(B_2E_2)_\tau$ and $S(RB_1)_\sigma=S(RB_2E_2)_\tau$. The difference between the two values of [coherent information](../../../../../../coherent-information.md) is therefore

$$
\begin{aligned}
I_c(\Lambda_1,\rho)-I_c(\Lambda_2\circ\Lambda_1,\rho)
&=S(B_2E_2)-S(RB_2E_2)-S(B_2)+S(RB_2)\\
&=I(R:E_2\mid B_2)_\tau\geq0.
\end{aligned}
$$

Nonnegativity follows from [Strong subadditivity of Von Neumann entropy](../../../../../../strong-subadditivity-of-quantum-entropy.md). This proves the [data-processing inequality for coherent information](../../../../../../data-processing-inequality-for-coherent-information.md):

$$
\boxed{I_c(\Lambda_2\circ\Lambda_1,\rho)\leq I_c(\Lambda_1,\rho).}
$$

The dilated state here need not be pure. The proof uses only isometry invariance and strong subadditivity, so it applies even when the first channel has already entangled the input with its own discarded environment.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
