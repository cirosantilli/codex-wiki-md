<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\mathcal Q$ be the full subcategory of [quotients of decidable objects](../../../../../../quotients-of-decidable-objects.md). It is closed under quotients, by composition of [epimorphisms](../../../../../../epimorphism.md), and under small [coproducts](../../../../../../coproduct.md), by part (ii). It is also closed under [subobjects](../../../../../../subobject.md): pull back a decidable cover $D\twoheadrightarrow B$ along $B'\hookrightarrow B$. The resulting cover of $B'$ has domain a [subobject](../../../../../../subobject.md) of $D$, hence a decidable object.

The [terminal object](../../../../../../terminal-object.md) lies in $\mathcal Q$. If $D\twoheadrightarrow B$ and $D'\twoheadrightarrow C$ are decidable covers, their product is an [epimorphism](../../../../../../epimorphism.md) $D\times D'\twoheadrightarrow B\times C$. Part (ii) makes its domain decidable. Thus products, and then [equalizers](../../../../../../equaliser.md) as [subobjects](../../../../../../subobject.md) of products, remain in $\mathcal Q$. The inclusion $I:\mathcal Q\hookrightarrow\mathcal E$ preserves [finite limits](../../../../../../finite-limit.md).

We construct a [coreflective subcategory](../../../../../../coreflective-subcategory.md) rather than claim that every object has a decidable cover. For $X\in\mathcal E$, let $qX\hookrightarrow X$ be the union of all [subobjects](../../../../../../subobject.md) of $X$ which lie in $\mathcal Q$. The [Grothendieck topos](../../../../../../grothendieck-topos.md) is well-powered, so these [subobjects](../../../../../../subobject.md) form a set. Choose a decidable cover of each and take their [coproduct](../../../../../../coproduct.md). Its map to $X$ has image $qX$, so $qX$ is itself a quotient of a decidable object. Any map from an object of $\mathcal Q$ to $X$ has image in $\mathcal Q$, and therefore factors uniquely through $qX$. This gives

$$
I\dashv q,\qquad \mathcal E(IB,X)\cong\mathcal Q(B,qX).
$$

The induced [idempotent comonad](../../../../../../idempotent-comonad.md) $G=Iq$ on $\mathcal E$ preserves [finite limits](../../../../../../finite-limit.md): $q$ is a [right adjoint](../../../../../../adjoint-functors.md) and $I$ preserves those limits. Its counit is the inclusion $qX\hookrightarrow X$, and $q(qX)=qX$.

The coalgebras of this comonad are exactly the objects of $\mathcal Q$. A coalgebra structure is a section $X\to qX$ of the monic counit, forcing the counit to be an isomorphism; conversely an object already in $\mathcal Q$ has the unique such structure. Thus $\mathcal Q\simeq\mathcal E^G$. Part (i) now gives

$$
\boxed{\mathcal E_{qd}\text{ is a topos}.}
$$

This argument proves the required elementary-topos conclusion without presuming a small family of decidable generators for $\mathcal E$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Section A](../../section-a.md)
4. [Paper 20](../../../paper-20-split.md)
5. [Iii](../../../split.md)
6. [2014](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
