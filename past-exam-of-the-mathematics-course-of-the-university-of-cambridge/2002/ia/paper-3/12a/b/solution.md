<h1 id="12a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [product rule](../../../../../../product-rule.md) for the [divergence](../../../../../../divergence.md) of the [vector field](../../../../../../vector-field.md) $F=\phi\nabla\psi-\psi\nabla\phi$:

$$
\begin{aligned}
\nabla\cdot F
&=\nabla\phi\cdot\nabla\psi+\phi\nabla^2\psi
-\nabla\psi\cdot\nabla\phi-\psi\nabla^2\phi\\
&=\phi\nabla^2\psi-\psi\nabla^2\phi.
\end{aligned}
$$

The two [dot products](../../../../../../dot-product.md) cancel. Apply the [divergence theorem](../../../../../../divergence-theorem.md) with outward unit [normal vector](../../../../../../normal-vector.md) $n$ to obtain [Green's second identity](../../../../../../green-second-identity.md):

$$
\boxed{\int_V(\phi\nabla^2\psi-\psi\nabla^2\phi)\,dV
=\int_S(\phi\nabla\psi-\psi\nabla\phi)\cdot n\,dS.}
$$

Smoothness of the functions and boundary supplies the regularity needed for the [divergence theorem](../../../../../../divergence-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12A](../../12a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
