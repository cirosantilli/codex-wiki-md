<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Apply the assumed [data-processing inequality for quantum relative entropy](../../../../../../data-processing-inequality-for-quantum-relative-entropy.md) to the normalized [partial trace](../../../../../../partial-trace.md) over $C$, with the two input states

$$
\rho_{ABC},
\qquad
\frac{I_A}{d_A}\otimes\rho_{BC}.
$$

The channel sends them to $\rho_{AB}\otimes I_C/d_C$ and $I_A/d_A\otimes\rho_B\otimes I_C/d_C$. Additivity over the common maximally mixed factor reduces data processing to

$$
D\left(\rho_{ABC}\middle\|\frac{I_A}{d_A}\otimes\rho_{BC}\right)
\geq
D\left(\rho_{AB}\middle\|\frac{I_A}{d_A}\otimes\rho_B\right).
$$

Expanding the [Umegaki relative entropy](../../../../../../quantum-relative-entropy.md) in terms of [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) gives

$$
-S(\rho_{ABC})+\log d_A+S(\rho_{BC})
\geq
-S(\rho_{AB})+\log d_A+S(\rho_B).
$$

After cancelling $\log d_A$, this is precisely the [Strong subadditivity of Von Neumann entropy](../../../../../../strong-subadditivity-of-quantum-entropy.md)

$$
\boxed{S(\rho_B)+S(\rho_{ABC})
\leq S(\rho_{AB})+S(\rho_{BC})}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
