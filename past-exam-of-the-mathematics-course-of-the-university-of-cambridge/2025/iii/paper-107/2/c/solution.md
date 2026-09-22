<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The boundary data are encoded by the [Affine Sobolev space](../../../../../../affine-sobolev-space.md)

$$
\mathcal A_\varphi=\varphi+W_0^{1,p}(\Omega)
=\{u\in W^{1,p}(\Omega):\operatorname{Tr}u=\operatorname{Tr}\varphi\}.
$$

A function $u\in\mathcal A_\varphi$ is a weak solution of the homogeneous [p-Laplacian equation](../../../../../../p-laplacian.md) when

$$
\int_\Omega|Du|^{p-2}Du\mathbin\cdot D\psi=0
\qquad\text{for every }\psi\in W_0^{1,p}(\Omega).
$$

For existence, take a minimizing sequence for the [p-energy](../../../../../../p-energy.md) on $\mathcal A_\varphi$. The [Poincaré inequality](../../../../../../poincare-inequality.md) bounds $u-\varphi$ in $W^{1,p}$ by its gradient, so the sequence is bounded in the [reflexive Banach space](../../../../../../reflexive-banach-space.md) $W^{1,p}$. A weakly convergent subsequence remains in the weakly closed affine space, and convexity of $|\eta|^p$ gives [weak lower semicontinuity](../../../../../../weak-lower-semicontinuity.md). The [direct method in the calculus of variations](../../../../../../direct-method-in-the-calculus-of-variations.md) therefore produces a minimizer, whose first variation is precisely the displayed weak equation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
