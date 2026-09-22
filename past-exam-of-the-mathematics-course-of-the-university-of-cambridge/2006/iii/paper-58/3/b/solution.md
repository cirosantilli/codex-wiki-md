<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Represent the pure states by [density matrices](../../../../../../density-matrix.md) $\rho_u=(I+u\cdot\sigma)/2$ and $\rho_v=(I+v\cdot\sigma)/2$. The [Pauli matrices](../../../../../../pauli-matrices.md) obey $\operatorname{Tr}\sigma_i=0$ and $\operatorname{Tr}(\sigma_i\sigma_j)=2\delta_{ij}$. Consequently

$$
\operatorname{Tr}(\rho_u\rho_v)=\frac14\operatorname{Tr}\left[I+(u+v)\cdot\sigma+
\sum_{i,j}u_iv_j\sigma_i\sigma_j\right]
=\frac12(1+u\cdot v).
$$

On the other hand, $\rho_u=|u\rangle\langle u|$ and $\rho_v=|v\rangle\langle v|$ make that [trace](../../../../../../matrix-trace.md) equal to $\langle u|v\rangle\langle v|u\rangle$. Thus the [pure-qubit overlap identity](../../../../../../pure-qubit-overlap-identity.md) is

$$
\boxed{|\langle u|v\rangle|^2=\tfrac12(1+u\cdot v).}
$$

For mixed states the [trace](../../../../../../matrix-trace.md) formula still holds, but its left side is then a Hilbert–Schmidt overlap rather than this squared pure-state overlap.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
