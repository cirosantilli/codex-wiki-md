<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Introduce an orthonormal classical label register $X$ and the [classical-quantum state](../../../../../../classical-quantum-state.md)

$$
\omega_{XQ}=\sum_i p_i|i\rangle\langle i|_X\otimes\rho_i.
$$

The blocks have orthogonal supports because their label vectors are orthogonal, regardless of whether the original $\rho_i$ have orthogonal supports. Part (a) gives $S(XQ)=H(p)+\sum_i p_iS(\rho_i)$. The marginals are $\omega_X=\sum_i p_i|i\rangle\langle i|$ and $\omega_Q=\sum_i p_i\rho_i$, so $S(X)=H(p)$. Apply the [Subadditivity of Von Neumann entropy](../../../../../../subadditivity-of-von-neumann-entropy.md) and cancel $H(p)$:

$$
H(p)+\sum_i p_iS(\rho_i)\leq H(p)+S\!\left(\sum_i p_i\rho_i\right).
$$

Thus **$S(\sum_i p_i\rho_i)\geq\sum_i p_iS(\rho_i)$**. This is the [Concavity of Von Neumann entropy](../../../../../../concavity-of-von-neumann-entropy.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
