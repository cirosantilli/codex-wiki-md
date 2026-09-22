<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write a qubit [density operator](../../../../../../density-matrix.md) in [Bloch vector](../../../../../../bloch-vector.md) form, $\rho=(I+\mathbf r\mathbin\cdot\boldsymbol\sigma)/2$, with $|\mathbf r|\leq1$. The [quantum depolarizing channel](../../../../../../quantum-depolarizing-channel.md) maps $\mathbf r$ to $p\mathbf r$, so its output eigenvalues are $(1\pm p|\mathbf r|)/2$. The output [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is minimized on pure inputs, where it equals $h_2((1+p)/2)$.

For any input ensemble, its output [Holevo quantity](../../../../../../holevo-quantity.md) is at most the maximum qubit entropy minus this minimum output entropy:

$$
\chi\leq1-h_2\left(\frac{1+p}2\right).
$$

Equality is attained by two equiprobable orthogonal pure inputs: their average output is $I/2$, while each output has the minimum entropy. Thus

$$
\boxed{\chi^*(\Lambda_{\rm dep})=1-h_2\left(\frac{1+p}2\right)}.
$$

This uses the question's retention parameter $p$; in the usual convex-mixture range, $0\leq p\leq1$. The expression also holds throughout the full completely positive qubit range $-1/3\leq p\leq1$, since $h_2((1+p)/2)=h_2((1+|p|)/2)$.

The supplied [additivity of Holevo capacity](../../../../../../additivity-of-holevo-capacity.md) gives $\chi^*(\Lambda_{\rm dep}^{\otimes n})=n\chi^*(\Lambda_{\rm dep})$. The [Holevo-Schumacher-Westmoreland theorem](../../../../../../holevo-schumacher-westmoreland-theorem.md) expresses the unassisted [classical capacity of a quantum channel](../../../../../../classical-capacity-of-a-quantum-channel.md) as the regularized [Holevo capacity](../../../../../../holevo-capacity.md), so

$$
\boxed{C(\Lambda_{\rm dep})=\chi^*(\Lambda_{\rm dep})}.
$$

Therefore entangled inputs across channel uses cannot increase this classical capacity.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
