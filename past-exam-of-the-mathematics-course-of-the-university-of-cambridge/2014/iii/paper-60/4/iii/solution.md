<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For any tripartite [density operator](../../../../../../density-matrix.md), [Strong subadditivity of Von Neumann entropy](../../../../../../strong-subadditivity-of-quantum-entropy.md) is

$$
\boxed{S(AB)+S(BC)\geq S(B)+S(ABC).}
$$

Use [quantum relative entropy](../../../../../../quantum-relative-entropy.md) $D(\rho\|\sigma)=\operatorname{Tr}\rho(\log_2\rho-\log_2\sigma)$, with the usual support condition. The equivalent relative-entropy comparison is

$$
D(\rho_{ABC}\|\rho_A\otimes\rho_{BC})\geq D(\rho_{AB}\|\rho_A\otimes\rho_B).
$$

Indeed the two sides expand respectively as $S(A)+S(BC)-S(ABC)$ and $S(A)+S(B)-S(AB)$. Subtracting cancels $S(A)$ and leaves exactly the strong-subadditivity gap. Marginal-product supports contain the support of the joint state, so these expressions are finite; singular marginals can also be handled by full-rank regularization and a limit.

Finally, tracing out $C$ sends the numerator and denominator of the first relative entropy to those of the second. The [data-processing inequality for quantum relative entropy](../../../../../../data-processing-inequality-for-quantum-relative-entropy.md) therefore proves the comparison. This is [strong subadditivity from relative-entropy monotonicity](../../../../../../strong-subadditivity-from-relative-entropy-monotonicity.md), rather than an assumption that classical entropy proofs automatically apply to quantum states.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
