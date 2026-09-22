<h1 id="37d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Lower the free index of $K$. The [Killing equation](../../../../../../killing-equation.md) makes the last two indices of $\nabla_\nu\nabla_\mu K_\alpha$ antisymmetric after the appropriate derivative is moved. Combining the three resulting [Ricci identities](../../../../../../curvature-commutator-on-a-covariant-tensor.md) cyclically gives

$$
\nabla_\nu\nabla_\mu K_\alpha
=\frac12\left(
[\nabla_\nu,\nabla_\mu]K_\alpha
-[\nabla_\mu,\nabla_\alpha]K_\nu
+[\nabla_\alpha,\nabla_\nu]K_\mu
\right).
$$

Applying the covector form of the Ricci identity and then the [first Bianchi identity](../../../../../../first-bianchi-identity.md) reduces this to

$$
\nabla_\nu\nabla_\mu K_\alpha
=R_{\alpha\mu\nu\beta}K^\beta.
$$

Raising $\alpha$ proves the [second covariant derivative of a Killing vector](../../../../../../second-covariant-derivative-of-a-killing-vector.md) identity

$$
\boxed{\nabla_\nu\nabla_\mu K^\alpha
=R^\alpha{}_{\mu\nu\beta}K^\beta.}
$$

Contracting $\mu$ and $\nu$ and using the definition and symmetries of the [Ricci tensor](../../../../../../ricci-tensor.md) gives

$$
\boxed{\nabla_\mu\nabla^\mu K^\alpha
=-R^\alpha{}_{\beta}K^\beta.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [37D](../../37d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
