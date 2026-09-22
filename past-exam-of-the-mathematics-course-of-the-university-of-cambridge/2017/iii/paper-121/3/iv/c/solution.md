<h1 id="3/iv/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We prove [mutual genericity for product forcing](../../../../../../../mutual-genericity-for-product-forcing.md). Let $D\in M[G_0]$ be a dense [subset](../../../../../../../subset.md) of $\mathbb Q$, and take a [forcing name](../../../../../../../forcing-name.md) $\dot D\in M$ evaluating to $D$. By the [forcing theorem](../../../../../../../forcing-theorem.md), some $p_0\in G_0$ forces that $\dot D$ is a dense [subset](../../../../../../../subset.md) of the [canonical forcing name](../../../../../../../canonical-forcing-name.md) for $\mathbb Q$.

In $M$ define

$$
E=\{(p,q):p\perp p_0\}\ \cup\ \{(p,q):p\leq p_0\text{ and }p\Vdash\check q\in\dot D\}.
$$

This [set](../../../../../../../set-split.md) is dense in the [product forcing](../../../../../../../product-forcing.md) order. Given $(p,q)$, the incompatible case is immediate. Otherwise first strengthen $p$ below $p_0$. The forced density assertion and the [existential clause of syntactic forcing](../../../../../../../existential-clause-of-syntactic-forcing.md) supply a further $r\leq p,p_0$ and a ground-model $q'\leq q$ with $r\Vdash\check q'\in\dot D$. To justify choosing a ground-model $q'$, a name forced to lie in $\check{\mathbb Q}$ can densely be made equal to some $\check q'$ by the atomic membership clause; strengthen to that equality and use the forced order comparison. Thus $(r,q')\in E$ lies below $(p,q)$.

The [generic filter](../../../../../../../generic-filter.md) $H$ meets $E$. It cannot meet the first part, because its first projection contains $p_0$ and is directed. Hence there is $(p,q)\in H$ with $p\in G_0$ and $p\Vdash\check q\in\dot D$. Soundness of the [forcing theorem](../../../../../../../forcing-theorem.md) gives $q\in D$, and the projection gives $q\in G_1$. Since every such $D$ is met,

$$
\boxed{G_1\text{ is }\mathbb Q\text{-generic over }M[G_0].}
$$

This establishes the stronger property, rather than merely meeting dense ground-model [subsets](../../../../../../../subset.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [Iv](../../iv.md)
3. [3](../../../3.md)
4. [Paper 121](../../../../paper-121-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
