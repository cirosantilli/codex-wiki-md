<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Being constant on the two-element orbits is equivalent to $f(-x,-y)=f(x,y)$. In characteristic zero, comparing [monomial](../../../../../monomial.md) coefficients shows that precisely the terms of even total degree survive. Thus a [vector space](../../../../../vector-space-split.md) [basis](../../../../../basis.md) is

$$
\boxed{\{x^{2a}y^{2b},\ x^{2a+1}y^{2b+1}:a,b\ge0\}.}
$$

Set $u=x^2$, $v=xy$, $w=y^2$. The two basis types are $u^aw^b$ and $vu^aw^b$, so they prove $R=k[u,v,w]$. Hence $R$ is a [finitely generated algebra](../../../../../finitely-generated-algebra.md). It is an [integral domain](../../../../../integral-domain.md) as a subring of the [integral domain](../../../../../integral-domain.md) $k[x,y]$.

The generators satisfy $uw-v^2=0$. To prove this is the whole relation ideal, reduce any polynomial in $U,V,W$ modulo the monic relation $V^2-UW$ to

$$
A(U,W)+VB(U,W).
$$

Its image in $k[x,y]$ is $A(x^2,y^2)+xyB(x^2,y^2)$. The first summand has both exponents even and the second both odd; their distinct [monomials](../../../../../monomial.md) are linearly independent. Thus the image vanishes only when both $A,B$ are zero. Consequently

$$
\boxed{R\cong k[U,V,W]/(UW-V^2),\qquad Y=V(UW-V^2)\subseteq\mathbb A^3.}
$$

This gives the requested closed embedding and the [quadratic cone invariant ring](../../../../../quadratic-cone-invariant-ring.md) presentation.

The associated [morphism of algebraic varieties](../../../../../morphism-of-algebraic-varieties.md) is explicitly

$$
f:\mathbb A^2\longrightarrow Y,\qquad (x,y)\longmapsto(x^2,xy,y^2).
$$

It is surjective. For $(u,v,w)\in Y$, if $u\ne0$, choose $x$ with $x^2=u$ using algebraic closedness and put $y=v/x$. Then $y^2=v^2/u=w$. If $u=0$, the relation forces $v=0$; take $x=0$ and choose $y^2=w$. This covers every point of $Y$. Except over the origin, the two preimages differ by the simultaneous sign change, consistent with the orbit description.

Finally the gradient of $UW-V^2$ is $(W,-2V,U)$, so the [Jacobian criterion](../../../../../jacobian-criterion.md) makes every nonzero point smooth. At the origin, the maximal ideal modulo its square has the three independent classes of $U,V,W$, since the defining relation is quadratic. The tangent space there has dimension three, while $Y$ has dimension two. Therefore

$$
\boxed{\operatorname{Sing}Y=\{(0,0,0)\}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
