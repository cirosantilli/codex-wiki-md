<h1 id="3/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the reverse implication, suppose $p\in G$ and $M\models p\Vdash^*\exists x\,\varphi(x)$. By the [existential clause of syntactic forcing](../../../../../../../existential-clause-of-syntactic-forcing.md), the set

$$
D=\{q\leq p:M\models\exists\sigma\;(q\Vdash^*\varphi(\sigma))\}
$$

is dense below $p$; the existential quantifier ranges over [forcing names](../../../../../../../forcing-name.md) of $M$. Definability of the [syntactic forcing relation](../../../../../../../syntactic-forcing-relation.md) and [axiom schema of separation](../../../../../../../axiom-schema-of-specification.md) put $D$ in $M$.

To apply genericity, augment it to the globally dense set

$$
D'=D\cup\{q\in\mathbb P:q\perp p\}.
$$

A condition compatible with $p$ has an extension below $p$, then one in $D$, and an incompatible condition already lies in $D'$. Thus $D'$ is a [dense subset of a forcing order](../../../../../../../dense-subset-of-a-forcing-order.md) in $M$. The [generic filter](../../../../../../../generic-filter.md) meets it. Since $p\in G$, directedness prevents $G$ from containing a condition incompatible with $p$, so some $q\in G\cap D$ exists.

There is consequently a name $\sigma\in M$ with $M\models q\Vdash^*\varphi(\sigma)$. The assumed truth lemma gives $M[G]\models\varphi(\operatorname{val}(\sigma,G))$, and hence

$$
\boxed{\exists p\in G\;M\models p\Vdash^*\exists x\,\varphi(x)\quad\Longrightarrow\quad M[G]\models\exists x\,\varphi(x).}
$$

Together with part (a), this completes the existential step of the [forcing theorem](../../../../../../../forcing-theorem.md) without assuming the desired existential truth lemma in advance.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [3](../../../3.md)
4. [Paper 121](../../../../paper-121-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
