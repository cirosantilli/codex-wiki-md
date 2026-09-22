<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose for each $j\in\mathcal J$ a [categorical limit](../../../../../../categorical-limit.md) $L_j$ of $F(-,j)$, with projections $\lambda_{i,j}:L_j\to F(i,j)$. For $v:j\to k$, the [morphisms](../../../../../../morphism.md) $F(1_i,v)\lambda_{i,j}$ form a [categorical cone](../../../../../../cone-over-a-diagram.md) over $F(-,k)$, since the two actions of the product [functor](../../../../../../functor.md) $F$ commute. Define $L(v):L_j\to L_k$ by the equations

$$
\lambda_{i,k}L(v)=F(1_i,v)\lambda_{i,j}\qquad(i\in\mathcal I).
$$

Existence and uniqueness follow from the [universal property](../../../../../../universal-property.md). The [identity morphism](../../../../../../identity-morphism.md) of $L_j$ satisfies the equations for $v=1_j$, and $L(w)L(v)$ satisfies those for $wv$, so uniqueness gives $L(1_j)=1_{L_j}$ and $L(wv)=L(w)L(v)$. Hence $L:\mathcal J\to\mathcal D$ is a [functor](../../../../../../functor.md).

If $L'_j$ with projections $\lambda'_{i,j}$ are other choices, there is a unique [isomorphism](../../../../../../isomorphism.md) $u_j:L_j\to L'_j$ carrying every projection to the corresponding projection. The same equations show $u_kL(v)=L'(v)u_j$, because their composites with all $\lambda'_{i,k}$ agree. Thus the choices give **a unique [natural isomorphism](../../../../../../natural-isomorphism.md) compatible with the chosen [categorical limit](../../../../../../categorical-limit.md) [categorical cones](../../../../../../cone-over-a-diagram.md)**. Without the compatibility condition, uniqueness of an arbitrary [natural isomorphism](../../../../../../natural-isomorphism.md) is not asserted.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
