<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $A=S^2\times S^2$ and let $i:A\to X$ be its inclusion after the attachment. The [cohomology ring of a product of two spheres](../../../../../../cohomology-ring-of-a-product-of-two-spheres.md) is

$$
H^*(A;\mathbb Z)=\mathbb Z[a,b]/(a^2,b^2),\qquad |a|=|b|=2,
$$

where $a,b$ come from the first and second factors and $ab$ is the chosen orientation class. The diagonal pulls both $a$ and $b$ back to the same generator of $H^2(S^2;\mathbb Z)$.

There is one new three-cell. In the [cellular chain complex](../../../../../../cellular-chain-complex.md), its boundary has coordinates $(1,1)$ in the two-dimensional cells. Thus the relevant differential is

$$
\mathbb Z\xrightarrow{\binom11}\mathbb Z^2,
$$

and the original four-cell still has zero boundary. This gives $H_2(X;\mathbb Z)=\mathbb Z$, $H_3(X;\mathbb Z)=0$, $H_4(X;\mathbb Z)=\mathbb Z$, and no other positive [homology groups](../../../../../../homology-group.md). Equivalently, the [relative cohomology](../../../../../../relative-cohomology.md) sequence of $(X,A)$ gives an injective restriction in degree two with image $\mathbb Z(a-b)$, and an [isomorphism](../../../../../../isomorphism.md) in degree four.

Choose $u\in H^2(X;\mathbb Z)$ and $v\in H^4(X;\mathbb Z)$ by $i^*u=a-b$, $i^*v=ab$. Naturality of the [cup product](../../../../../../cup-product.md) gives

$$
i^*(u^2)=(a-b)^2=-2ab.
$$

Since restriction is injective in degree four, $u^2=-2v$. All further positive-degree [cup products](../../../../../../cup-product.md) vanish by dimension. Therefore

$$
\boxed{H^*(X;\mathbb Z)\cong\mathbb Z[u,v]/(u^2+2v,uv,v^2),\qquad |u|=2,\quad |v|=4.}
$$

Changing the sign of $v$ would instead give $u^2=2v$; the displayed sign uses the product orientation $ab$. The factor $2$ is the characteristic feature of a [cup square after a diagonal sphere attachment](../../../../../../cup-square-after-a-diagonal-sphere-attachment.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
