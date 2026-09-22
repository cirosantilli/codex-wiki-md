<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $V=k_0^2(n^2-1)$ be the [scattering potential](../../../../../../scattering-potential.md) supported in $D$. The background [Helmholtz equation](../../../../../../helmholtz-equation.md) and its outgoing kernel give the scalar [Lippmann-Schwinger equation](../../../../../../lippmann-schwinger-equation.md)

$$
\psi(\mathbf r)=\psi_i(\mathbf r)+\int_DG_{k_0}(\mathbf r,\mathbf r')V(\mathbf r')\psi(\mathbf r')\,d\mathbf r'.
$$

Replacing the unknown field in the integral by the incident field gives the [Born approximation for scalar wave scattering](../../../../../../born-approximation-for-scalar-wave-scattering.md):

$$
\boxed{\psi_B=\psi_i+\psi_{s,B},\qquad \psi_{s,B}(\mathbf r)=\int_DG_{k_0}(\mathbf r,\mathbf r')V(\mathbf r')\psi_i(\mathbf r')\,d\mathbf r'.}
$$

For the [Rytov approximation](../../../../../../rytov-approximation.md), work where $\psi_i\ne0$ and set $\psi=\psi_i e^\phi$. Dividing the wave equation by the total field and subtracting the incident equation gives

$$
\Delta\phi+2\nabla\log\psi_i\cdot\nabla\phi+(\nabla\phi)^2=-V.
$$

Neglect the quadratic gradient term. If $\phi_1=\psi_{s,B}/\psi_i$, direct differentiation shows $\Delta\phi_1+2\nabla\log\psi_i\cdot\nabla\phi_1=-V$, so

$$
\boxed{\psi_R=\psi_i\exp\left(\frac{\psi_{s,B}}{\psi_i}\right).}
$$

Expanding the exponential in the potential gives $\psi_R=\psi_i+\psi_{s,B}+O(V^2)=\psi_B+O(V^2)$. Thus both approximations have the same first-order field, although exponentiation retains a particular family of higher powers.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
