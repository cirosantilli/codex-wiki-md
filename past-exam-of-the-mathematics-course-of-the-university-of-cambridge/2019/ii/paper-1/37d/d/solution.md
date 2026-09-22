<h1 id="37d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Killing equation](../../../../../../killing-equation.md) gives $\nabla_\mu K^\mu=0$ and $\nabla_{[\mu}K_{\lambda]}=\nabla_\mu K_\lambda$. Commuting derivatives once and contracting the [Ricci identity](../../../../../../curvature-commutator-on-a-covariant-tensor.md) gives

$$
\nabla^\lambda\nabla_\mu K_\lambda=R_{\mu\beta}K^\beta.
$$

Therefore, using the [contracted Bianchi identity](../../../../../../contracted-bianchi-identity.md) and symmetry of $R_{\mu\beta}$,

$$
\begin{aligned}
2\nabla^\mu\nabla^\lambda\nabla_{[\mu}K_{\lambda]}
&=2\nabla^\mu(R_{\mu\beta}K^\beta)\\
&=K^\beta\nabla_\beta R
+2R_{\mu\beta}\nabla^\mu K^\beta\\
&=K^\beta\nabla_\beta R.
\end{aligned}
$$

Since $\nabla_{[\mu}K_{\lambda]}$ is antisymmetric, swapping the two contracted index names shows that the left side equals its derivative-antisymmetrized form:

$$
\boxed{K^\alpha\nabla_\alpha R
=2\nabla^{[\mu}\nabla^{\lambda]}\nabla_{[\mu}K_{\lambda]}.}
$$

Now set $A_{\mu\lambda}=\nabla_{[\mu}K_{\lambda]}$. The right side is the contracted commutator $[\nabla^\mu,\nabla^\lambda]A_{\mu\lambda}$. By the [curvature commutator on a covariant tensor](../../../../../../curvature-commutator-on-a-covariant-tensor.md), it is a sum of contractions of the symmetric [Ricci tensor](../../../../../../ricci-tensor.md) with the antisymmetric tensor $A$, and hence vanishes. Thus

$$
\boxed{K^\alpha\nabla_\alpha R=0,}
$$

so the [Killing vector preserves scalar curvature](../../../../../../killing-vector-preserves-scalar-curvature.md).

## ↑ Ancestors (11)

1. [D](../d.md)
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
