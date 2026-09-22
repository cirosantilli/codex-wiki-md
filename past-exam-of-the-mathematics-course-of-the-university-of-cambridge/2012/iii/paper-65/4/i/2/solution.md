<h1 id="4/i/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Encode the ensemble label in an orthogonal classical register:

$$
\omega_{XB}=\sum_xp_x|x\rangle\langle x|\otimes\rho_x.
$$

The [classical-quantum state](../../../../../../../classical-quantum-state.md) has $S(XB)=H(p)+\sum_xp_xS(\rho_x)$, $S(X)=H(p)$ and $S(B)=S(\bar\rho)$, where $\bar\rho=\sum_xp_x\rho_x$. Hence

$$
I(X:B)_\omega=S(\bar\rho)-\sum_xp_xS(\rho_x)=\chi(\mathcal E).
$$

Applying $\operatorname{id}_X\otimes\Lambda$ changes the conditional states to the output ensemble. The same identity gives $I(X:B')=\chi(\mathcal E')$. [Data processing for quantum mutual information](../../../../../../../data-processing-for-quantum-mutual-information.md), proved in Question 3, therefore yields the [Holevo quantity under a quantum channel](../../../../../../../holevo-quantity-under-a-quantum-channel.md):

$$
\boxed{\chi(\mathcal E')\leq\chi(\mathcal E).}
$$

This concerns the information available in the whole ensemble, not the change in the entropy of each individual state.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [I](../../i.md)
3. [4](../../../4.md)
4. [Paper 65](../../../../paper-65-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
