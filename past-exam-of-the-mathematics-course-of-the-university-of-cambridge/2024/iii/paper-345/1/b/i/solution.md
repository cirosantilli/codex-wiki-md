<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Local [mass conservation](../../../../../../../mass-conservation.md) of each particle species gives the [system of conservation laws](../../../../../../../system-of-conservation-laws.md)

$$
\partial_t\phi_i+\partial_z(\phi_iW_i)=0,
\qquad i=1,2.
$$

For $\boldsymbol\phi=(\phi_1,\phi_2)^T$ and flux $F_i=\phi_iW_i$, the [flux Jacobian](../../../../../../../flux-jacobian.md) is

$$
A(\boldsymbol\phi)=
\begin{pmatrix}
(1-2\phi_1)\widehat W_1-\phi_2\widehat W_2&-\phi_1\widehat W_2\\
-\phi_2\widehat W_1&(1-2\phi_2)\widehat W_2-\phi_1\widehat W_1
\end{pmatrix}.
$$

Writing its entries as $A_{ij}$, the two [characteristic speeds](../../../../../../../characteristic-speed.md) are its [eigenvalues](../../../../../../../eigenvalue.md)

$$
\lambda_\pm
=\frac{A_{11}+A_{22}}2
\pm\frac12\sqrt{(A_{11}-A_{22})^2+4A_{12}A_{21}}.
$$

The discriminant is nonnegative because $A_{12}A_{21}=\phi_1\phi_2\widehat W_1\widehat W_2\geq0$, so positive concentrations of two settling species give real characteristics.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 345](../../../../paper-345-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
