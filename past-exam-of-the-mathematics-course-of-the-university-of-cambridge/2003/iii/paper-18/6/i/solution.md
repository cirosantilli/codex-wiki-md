<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A presheaf on $0\to1$ is an arrow $r:B=X(1)\to A=X(0)$ in sets. A morphism of presheaves is a commuting square. Define

$$
\Pi(r)=A,\qquad\Gamma(r)=B,\qquad\Delta(S)=(S\xrightarrow1S),\qquad\nabla(S)=(S\to1).
$$

A commuting square from $r$ to $\Delta S$ is determined by its map $A\to S$, while a square from $\Delta S$ to $r$ is determined by its map $S\to B$. A square from $r$ to $\nabla S$ is also determined by its map $B\to S$, because the other component is the unique map $A\to1$. Therefore these Hom-set bijections establish the [adjoint chain for evaluation in an arrow category](../../../../../../adjoint-chain-for-evaluation-in-an-arrow-category.md):

$$
\boxed{\Pi\dashv\Delta\dashv\Gamma\dashv\nabla.}
$$

There is a further left adjoint to $\Pi$: $\Lambda(S)=(\varnothing\to S)$. A square $\Lambda S\to r$ is exactly a map $S\to A$, proving $\Lambda\dashv\Pi$.

There is no right adjoint to $\nabla$. If there were, $\nabla$ would be a left adjoint and preserve the [initial object](../../../../../../initial-object.md). But it sends the empty set to $(\varnothing\to1)$, whereas the [initial object](../../../../../../initial-object.md) of this arrow category is $(\varnothing\to\varnothing)$. They are not isomorphic. Hence **$\Pi$ does have a left adjoint, while $\nabla$ has no right adjoint**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
