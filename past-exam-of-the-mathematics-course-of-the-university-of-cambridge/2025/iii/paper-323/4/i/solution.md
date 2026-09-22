<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Umegaki relative entropy](../../../../../../quantum-relative-entropy.md) is

$$
D(\rho\|\sigma)
=\operatorname{Tr}\rho(\log\rho-\log\sigma)
$$

when the support of $\rho$ is contained in that of $\sigma$, and $+\infty$ otherwise. Its [additivity of quantum relative entropy](../../../../../../additivity-of-quantum-relative-entropy.md) is

$$
D(\rho_A\otimes\rho_B\|\sigma_A\otimes\sigma_B)
=D(\rho_A\|\sigma_A)+D(\rho_B\|\sigma_B),
$$

its [superadditivity of quantum relative entropy](../../../../../../superadditivity-of-quantum-relative-entropy.md) is

$$
D(\rho_{AB}\|\sigma_A\otimes\sigma_B)
\geq D(\rho_A\|\sigma_A)+D(\rho_B\|\sigma_B),
$$

and its [data-processing inequality for quantum relative entropy](../../../../../../data-processing-inequality-for-quantum-relative-entropy.md) is $D(T(\rho)\|T(\sigma))\leq D(\rho\|\sigma)$ for every [quantum channel](../../../../../../quantum-channel.md) $T$.

Additivity follows from the logarithm of a [tensor product](../../../../../../tensor-product.md),

$$
\log(\rho_A\otimes\rho_B)
=\log\rho_A\otimes I+I\otimes\log\rho_B,
$$

and the analogous identity for $\sigma_A\otimes\sigma_B$. For superadditivity, subtract the two marginal relative entropies from the joint one. The reference-state terms cancel, leaving

$$
S(\rho_A)+S(\rho_B)-S(\rho_{AB})
=I(A:B)_\rho\geq0.
$$

This is the nonnegativity of [quantum mutual information](../../../../../../quantum-mutual-information.md), equivalently [Subadditivity of Von Neumann entropy](../../../../../../subadditivity-of-von-neumann-entropy.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
