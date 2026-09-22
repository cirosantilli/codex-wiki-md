<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

After the first [quantum channel](../../../../../../quantum-channel.md), denote the joint reference-output state by $\omega_{RB_1}$. Dilate the second [CPTP map](../../../../../../quantum-channel.md) as an [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md) $B_1\to B_2E_2$, with the resulting state denoted $\tau$. [Linear isometries](../../../../../../linear-isometry-of-hilbert-spaces.md) preserve nonzero eigenvalues, both globally and on the transformed output, giving

$$
I_c(\Phi_1,\rho)=S(B_2E_2)_\tau-S(RB_2E_2)_\tau.
$$

Tracing out $E_2$ implements the second channel, so

$$
I_c(\Phi_2\circ\Phi_1,\rho)=S(B_2)_\tau-S(RB_2)_\tau.
$$

The [Strong subadditivity of Von Neumann entropy](../../../../../../strong-subadditivity-of-quantum-entropy.md) for $R,B_2,E_2$ gives $S(RB_2)+S(B_2E_2)\geq S(B_2)+S(RB_2E_2)$. Rearranging proves the [data-processing inequality for coherent information](../../../../../../data-processing-inequality-for-coherent-information.md):

$$
\boxed{I_c(\Phi_1,\rho)\geq I_c(\Phi_2\circ\Phi_1,\rho)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
