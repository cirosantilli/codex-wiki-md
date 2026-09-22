<h1 id="9/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First prove the exact lifting statement for the [forgetful functor](../../../../../../forgetful-functor.md) $U^T:\mathcal C^T\to\mathcal C$. Take any [diagram in a category](../../../../../../diagram-category-theory.md) of [algebras for a monad](../../../../../../algebra-for-a-monad.md) $(A_j,a_j)$ whose underlying diagram has a chosen [categorical limit](../../../../../../categorical-limit.md) $p_j:L\to A_j$. The arrows $a_jT(p_j):TL\to A_j$ form a [categorical cone](../../../../../../cone-over-a-diagram.md), since every diagram arrow is a [morphism of algebras for a monad](../../../../../../morphism-of-algebras-for-a-monad.md). Thus the [universal property](../../../../../../universal-property.md) gives a unique arrow $a:TL\to L$ satisfying

$$
\boxed{p_ja=a_jT(p_j)\quad\text{for every }j.}
$$

The projections are jointly monic: two arrows into $L$ with the same composites with every $p_j$ are equal. Therefore the algebra identities can be checked after these projections. For the unit,

$$
p_ja\eta_L=a_jT(p_j)\eta_L=a_j\eta_{A_j}p_j=p_j.
$$

For multiplication,

$$
\begin{aligned}
p_jaT(a)&=a_jT(p_ja)=a_jT(a_j)T^2(p_j),\\
p_ja\mu_L&=a_jT(p_j)\mu_L=a_j\mu_{A_j}T^2(p_j).
\end{aligned}
$$

The algebra law for $a_j$ makes the right-hand sides equal. Thus $(L,a)$ is an [algebra for a monad](../../../../../../algebra-for-a-monad.md), and each $p_j$ is a [morphism of algebras for a monad](../../../../../../morphism-of-algebras-for-a-monad.md). Its action is unique with this property.

Given an algebra cone $q_j:(B,b)\to(A_j,a_j)$, let $q:B\to L$ be its unique underlying mediating map. Then

$$
p_jqb=q_jb=a_jT(q_j)=p_jaT(q),
$$

so $qb=aT(q)$ by joint monicity. Hence $q$ is an algebra map, proving the lifted cone is limiting. This establishes that the [monad algebra forgetful functor creates limits](../../../../../../monad-algebra-forgetful-functor-creates-limits.md), **without any assumption that $T$ preserves limits**.

For a [monadic adjunction](../../../../../../monadic-adjunction.md), the comparison satisfies $U=U^TK$. If $K$ is an [isomorphism of categories](../../../../../../isomorphism-of-categories.md) over the base, the preceding unique lift transports back literally, so $U$ is a [limit-creating functor](../../../../../../limit-creating-functor.md). If monadic means that $K$ is only an [equivalence of categories](../../../../../../equivalence-of-categories.md), the precise conclusion is [creation of limits up to isomorphism](../../../../../../creation-of-limits-up-to-isomorphism.md): the lifted algebra is isomorphic to an object $K(D)$, and its limiting cone transports along that isomorphism. Full faithfulness supplies the arrows and their uniqueness.

This distinction concerns prescribed underlying objects, not existence of limits. Literal creation does not follow from an arbitrary equivalence alone. For example, the inclusion of the one-object category into the two-object [indiscrete category](../../../../../../indiscrete-category.md), choosing one of its objects, is an [equivalence of categories](../../../../../../equivalence-of-categories.md) and is monadic under the equivalence convention. Either object of the target is terminal, but the other chosen [terminal object](../../../../../../terminal-object.md) has no literal object preimage. Thus the strict reading of the requested assertion needs the strict comparison convention; the equivalence-invariant statement is proved above.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [9](../../9.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
