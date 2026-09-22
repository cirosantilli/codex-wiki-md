<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With vanishing [extrinsic curvature](../../../../../../extrinsic-curvature.md), the [momentum constraint](../../../../../../momentum-constraint.md) is identically satisfied and the vacuum [Hamiltonian constraint](../../../../../../hamiltonian-constraint.md) reduces to $\mathcal R=0$. To evaluate that [Ricci scalar](../../../../../../ricci-scalar.md), write $\psi_i=\partial_i\psi$, raise these intermediate indices with $\delta^{ij}$, and use $\gamma^{ij}=\psi^{-4}\delta^{ij}$. The [Levi-Civita connection](../../../../../../levi-civita-connection.md) is

$$
\Gamma^k{}_{ij}=\frac2\psi\left(\delta^k{}_i\psi_j+\delta^k{}_j\psi_i-\delta_{ij}\psi^k\right).
$$

Substitution into the stated curvature convention gives

$$
\mathcal R_{ij}
=-\frac2\psi\partial_i\partial_j\psi
-\frac2\psi\delta_{ij}\Delta\psi
+\frac6{\psi^2}\psi_i\psi_j
-\frac2{\psi^2}\delta_{ij}|\nabla\psi|^2.
$$

Tracing with $\gamma^{ij}$ cancels the gradient-square terms:

$$
\boxed{\mathcal R=-8\psi^{-5}\Delta\psi.}
$$

Here the [Laplacian](../../../../../../laplacian.md) and norm on the right are those of the flat Euclidean metric. Thus the [time-symmetric conformally flat vacuum initial data](../../../../../../time-symmetric-conformally-flat-vacuum-initial-data.md) constraints become

$$
\boxed{\Delta\psi=0.}
$$

The equivalence uses $\psi\ne0$. This identity is also the three-dimensional specialization of [scalar curvature under conformal rescaling](../../../../../../scalar-curvature-under-conformal-rescaling.md); locally the conformal exponent is $2\log|\psi|$, so either fixed nonzero sign of $\psi$ gives the same metric.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
