<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Both output states have the same reference marginal, and $S(R)=S(\rho)$. Expand [quantum mutual information](../../../../../../quantum-mutual-information.md) to obtain the [mutual information and coherent information identity](../../../../../../mutual-information-and-coherent-information-identity.md)

$$
I(R:B_1)_\sigma=S(\rho)+I_c(\Lambda_1,\rho),\qquad
I(R:B_2)_\omega=S(\rho)+I_c(\Lambda_2\circ\Lambda_1,\rho).
$$

The input-entropy term is identical in the two expressions. Subtract them and use the preceding [data-processing inequality for coherent information](../../../../../../data-processing-inequality-for-coherent-information.md):

$$
\boxed{I(R:B_1)_\sigma-I(R:B_2)_\omega
=I_c(\Lambda_1,\rho)-I_c(\Lambda_2\circ\Lambda_1,\rho)\geq0.}
$$

Thus the final [quantum channel](../../../../../../quantum-channel.md) cannot increase the reference-output [quantum mutual information](../../../../../../quantum-mutual-information.md), as required by [data processing for quantum mutual information](../../../../../../data-processing-for-quantum-mutual-information.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
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
