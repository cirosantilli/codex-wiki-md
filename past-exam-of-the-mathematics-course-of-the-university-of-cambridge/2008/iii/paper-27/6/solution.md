<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use a relative consistency construction: a model of [ZF](../../../../../zermelo-fraenkel-set-theory.md) gives one of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) through $L$, and we construct a model of [New Foundations with urelements](../../../../../new-foundations-with-urelements.md) from it. In the language with membership and a unary predicate $S$, [NFU](../../../../../new-foundations-with-urelements.md) requires that atoms have no members, extensionality holds between [sets](../../../../../set-split.md), and every [stratified formula](../../../../../stratified-formula.md) has a [set](../../../../../set-split.md) extension. A type assignment gives equal variables equal types and raises type by one across membership. We prove the actual comprehension scheme, rather than invoke its consistency by name.

Start with a model $M\models\mathsf{ZFC}$ and Skolemize it. Apply the Ramsey construction from Question 1 to obtain increasing ordinal indiscernibles $(c_i)_{i\in\mathbb Z}$, all greater than $\omega+\omega$. The finite satisfiability step uses the infinite increasing list $\omega\cdot3,\omega\cdot4,\ldots$ in the original model. Include the ordinal and ordering requirements in the finite truth colorings. Ramsey and compactness produce the indiscernibles; their [Skolem hull](../../../../../skolem-hull.md) $N$ still models [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md). The index shift gives an external structure automorphism $j$ of $N$ with $j(c_i)=c_{i+1}$. Such a model is necessarily externally ill-founded: $(c_0,c_{-1},c_{-2},\ldots)$ is an external descending ordinal sequence. No well-founded-model hypothesis is being smuggled in.

For every integer $i$, let $D_i$ be the external domain consisting of the objects of $N$ belonging internally to $V_{c_i}^N$. At type $i+1$, declare $S_{i+1}(y)$ iff $N$ says $y\subseteq V_{c_i}$. Use membership of $N$ only for flagged targets; an unflagged object has no typed members. A flagged object is a [set](../../../../../set-split.md) of the preceding type. Set-extensionality holds since all members of a flagged [set](../../../../../set-split.md) lie in $D_i$.

Every typed comprehension instance holds. Translate its finitely many typed quantifiers into quantifiers bounded by the appropriate [sets](../../../../../set-split.md) $V_{c_r}^N$. Separation in $N$ gives its extension $A\subseteq V_{c_i}^N$ for the distinguished free variable of type $i$. Since $c_i+1\le c_{i+1}$, this subset is an object of $D_{i+1}$ and satisfies its [set](../../../../../set-split.md) predicate. Also $j:D_i\to D_{i+1}$ is bijective and preserves the typed relations and flags. This is the required [type-shifting automorphism](../../../../../type-shifting-automorphism.md).

Collapse to the single domain $D_0$ by defining

$$
S(y)\quad\Longleftrightarrow\quad N\models y\subseteq V_{c_{-1}},
\qquad
\boxed{x\mathrel E y\quad\Longleftrightarrow\quad S(y)\ \text{and}\ N\models x\in j(y).}
$$

If $S(y)$, its image $j(y)$ is a subset of $V_{c_0}$, so its entire extension is visible in $D_0$. The flag is necessary: an unflagged object might otherwise have a partial visible extension. Flagged coextensive objects have equal images under $j$, by extensionality in $N$, and hence are equal; atoms have no $E$-members.

Now take a stratified untyped formula $\varphi(x,\bar a)$. Shift its type assignment so that $x$ has type zero, allowing negative integer types for other variables. Send a variable of assigned type $r$ to $j^r$ of its untyped value. Equality is preserved, and membership $uEv$ translates to flagged ordinary membership from type $r$ to type $r+1$. A [set](../../../../../set-split.md) predicate translates to its flag at that type. Quantifiers correspond bijectively under $j^r:D_0\to D_r$. Thus induction on the formula gives exact agreement between its untyped truth and this typed translation.

Typed comprehension supplies an object $A\in D_1$, flagged at type one, containing exactly the type-zero solutions. Let $b=j^{-1}(A)\in D_0$. It is flagged at type zero, and for every $x\in D_0$, $xEb$ iff $x\in A$ iff $\varphi(x,\bar a)$. This proves all stratified comprehension, including an empty [set](../../../../../set-split.md) and the universal [set](../../../../../set-split.md). We have constructed

$$
\boxed{(D_0,E,S)\models\mathsf{NFU}.}
$$

If infinity is included in the convention for [NFU](../../../../../new-foundations-with-urelements.md), the same construction supports it: $\omega$ and its successor graph lie far below $c_{-1}$ and are fixed by $j$, since they are definable without parameters in $N$. The domain of the new [set](../../../../../set-split.md) $\omega$ is the old $\omega$, since $j(\omega)=\omega$. An ordered pair in the new membership relation is $j^{-2}$ of the old Kuratowski pair. The old successor graph is fixed as a whole by $j$, so its elements are exactly these recoded pairs $(n,n+1)$ as $n$ ranges over $\omega$. It therefore supplies an actual new successor injection with proper range. This does not assume that $j$ fixes each nonstandard [natural number](../../../../../natural-number.md). This is the [rank-shifting automorphism construction of NFU](../../../../../rank-shifting-automorphism-construction-of-nfu.md); its logical ingredients are precisely the proved indiscernible-model construction and ordinary [set](../../../../../set-split.md) separation in the typed domains.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
