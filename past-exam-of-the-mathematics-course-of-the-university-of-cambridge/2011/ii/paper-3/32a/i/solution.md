<h1 id="32a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Differentiating the two equations for a fundamental matrix of solutions gives

$$
\psi_{\rho\tau}=(U_\tau+UV)\psi,\qquad\psi_{\tau\rho}=(V_\rho+VU)\psi.
$$

Equality for all independent initial vectors is equivalent to the [zero-curvature condition](../../../../../../zero-curvature-condition.md)

$$
\boxed{U_\tau-V_\rho+[U,V]=0.}
$$

A single possibly zero solution vector alone would not imply a matrix identity; compatibility is understood for the complete linear system.

Write $q=\phi_\rho$, $s=\sin\phi$, $c=\cos\phi$ and use [Pauli matrices](../../../../../../pauli-matrices.md):

$$
U=i\lambda\sigma_3+\frac{iq}{2}\sigma_1,\qquad V=\frac1{4i\lambda}(c\sigma_3+s\sigma_2),\quad\lambda\ne0.
$$

The matrix products give

$$
[U,V]=-\frac{i s}{2}\sigma_1-\frac{i q c}{4\lambda}\sigma_2+\frac{i q s}{4\lambda}\sigma_3,
$$

whereas $V_\rho=-(iqc/(4\lambda))\sigma_2+(iqs/(4\lambda))\sigma_3$. Thus these last two components cancel, and the remaining curvature is $(i/2)(\phi_{\rho\tau}-\sin\phi)\sigma_1$. Therefore

$$
\boxed{\phi_{\rho\tau}=\sin\phi,}
$$

the [Sine-Gordon equation](../../../../../../sine-gordon-equation.md) in light-cone coordinates.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [32A](../../32a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
