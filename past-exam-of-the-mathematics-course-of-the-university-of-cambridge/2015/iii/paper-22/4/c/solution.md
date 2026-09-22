<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

It is enough to prove the [solution-set condition](../../../../../../solution-set-condition.md) and then apply the [general adjoint functor theorem](../../../../../../freyd-general-adjoint-functor-theorem.md). Fix $D\in\mathcal D$ and a [morphism](../../../../../../morphism.md) $d:D\to UC$. We will factor it through one object in a [set](../../../../../../set-split.md) depending only on $D$.

First construct a [minimal supported subobject](../../../../../../minimal-supported-subobject.md). Among the [subobjects](../../../../../../subobject.md) $m:M\hookrightarrow C$ for which $d=U(m)d_M$ for some $d_M:D\to UM$, include $1_C$ and take their intersection $m_0:C_0\hookrightarrow C$. This is a small intersection, by well-poweredness. It exists by completeness as the [categorical limit](../../../../../../categorical-limit.md) of the diagram consisting of these [monomorphisms](../../../../../../monomorphism.md) into $C$. Its map to $C$ is a [monomorphism](../../../../../../monomorphism.md): two maps with the same composite to $C$ have equal projections to every $M$, since each $m$ is monic, and are then equal by the [categorical limit](../../../../../../categorical-limit.md) property. One can equivalently construct these intersections by [pullbacks in a category](../../../../../../pullback-category-theory.md) and small [products in a category](../../../../../../product-category-theory.md), using stability of [monomorphisms](../../../../../../monomorphism.md) under [pullback in a category](../../../../../../pullback-category-theory.md).

Choose the factorizations $d_M$. They form a compatible [categorical cone](../../../../../../cone-over-a-diagram.md) into the image diagram under $U$, all with common composite $d$ to $UC$. Preservation of small [categorical limits](../../../../../../categorical-limit.md) yields $d_0:D\to UC_0$ with $U(m_0)d_0=d$. If $n:N\hookrightarrow C_0$ is another [subobject](../../../../../../subobject.md) through which $d_0$ factors after applying $U$, then $m_0n$ is among the original supported [subobjects](../../../../../../subobject.md). The intersection property gives $r:C_0\to N$ with $m_0nr=m_0$. Since $m_0$ is monic, $nr=1_{C_0}$; since $n$ is monic, also $rn=1_N$. Thus **every supported subobject of $C_0$ is invertible**.

For each member $Q_i$ of the [small cogenerating family](../../../../../../cogenerating-set.md), consider

$$
\theta_i:\mathcal C(C_0,Q_i)\longrightarrow\mathcal D(D,UQ_i),\qquad q\longmapsto U(q)d_0.
$$

This map is [injective](../../../../../../injective-function.md). If $U(q)d_0=U(q')d_0$, preservation of the [equalizer](../../../../../../equaliser.md) of $q,q'$ makes $d_0$ factor through the image of that [equalizer](../../../../../../equaliser.md). Minimality makes its inclusion an [isomorphism](../../../../../../isomorphism.md), so $q=q'$.

Write $R_i=\mathcal D(D,UQ_i)$; it is a [set](../../../../../../set-split.md) by local smallness of $\mathcal D$. Let $S_i\subseteq R_i$ be the image of $\theta_i$. For each $s\in S_i$, there is exactly one corresponding $q_{i,s}:C_0\to Q_i$. These maps define the [evaluation embedding into cogenerator products](../../../../../../evaluation-embedding-into-cogenerator-products.md)

$$
e:C_0\longrightarrow P_S:=\prod_{i\in I}\prod_{s\in S_i}Q_i.
$$

It is a [monomorphism](../../../../../../monomorphism.md): if $eg=eh$ and $g\ne h$, cogeneration supplies some $q:C_0\to Q_i$ distinguishing $g,h$; that $q$ is one of the projections of $e$, a contradiction. The product is small. It is important to use the subfamilies $S_i$, since some missing coordinate in $R_i$ need not correspond to a [morphism](../../../../../../morphism.md) out of $C_0$.

There are only a [set](../../../../../../set-split.md) of possible families $(S_i\subseteq R_i)_{i\in I}$. For each such family form $P_S$, choose a [set](../../../../../../set-split.md) of representatives $N\hookrightarrow P_S$ of its [subobjects](../../../../../../subobject.md), and take all pairs $(N,d_N:D\to UN)$. Local smallness of $\mathcal D$ and well-poweredness make their union a [set](../../../../../../set-split.md). In the case just constructed, $e$ identifies $C_0$ with one chosen representative $N$. Transporting $d_0$ to $UN$ and composing the inverse identification with $m_0$ gives a factorization of the original $d$ through that pair. Therefore these pairs form a [weakly initial set](../../../../../../weakly-initial-set.md) in $(D\downarrow U)$.

The [general adjoint functor theorem](../../../../../../freyd-general-adjoint-functor-theorem.md) now supplies a [left adjoint](../../../../../../adjoint-functors.md) to $U$. Conversely, a [right adjoint](../../../../../../adjoint-functors.md) preserves small [categorical limits](../../../../../../categorical-limit.md), either by the [adjunction](../../../../../../adjoint-functors.md) [hom-set](../../../../../../hom-set.md) bijections and the [hom-set detection of categorical limits](../../../../../../hom-set-detection-of-categorical-limits.md), or directly from their [universal properties](../../../../../../universal-property.md). Hence **the stated special theorem is proved in both directions**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
