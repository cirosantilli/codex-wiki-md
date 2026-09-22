<h1 id="b/6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Zorn's lemma](../../../../../zorn-s-lemma.md) states that a nonempty [partially ordered set](../../../../../partially-ordered-set.md) in which every chain has an [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) has a [maximal element](../../../../../maximal-element-of-a-partially-ordered-set.md). Order the partial [group](../../../../../group-split.md) operations by inclusion of their graphs. The collection is a [set](../../../../../set-split.md), since its members are [subsets](../../../../../subset.md) of $X\times X\times X$. It is nonempty: choose $x_0\in X$ and put the one-element [group operation](../../../../../group-operation.md) on $\{x_0\}$.

To construct a [chain union of partial group operations](../../../../../chain-union-of-partial-group-operations.md), for the given nonempty chain, let $m=\bigcup_{n\in\mathcal C}n$ and let $A$ be the union of the corresponding [group](../../../../../group-split.md) carriers. Comparability guarantees agreement wherever two operations are both defined, so $m$ is a function. Its domain is $A\times A$: any two elements of $A$ lie together in one carrier, by taking the larger of the two chain members containing them. Their product then lies in that carrier and hence in $A$.

Any three elements similarly lie together in one chain member, where [associativity](../../../../../associative-property.md) holds; therefore [associativity](../../../../../associative-property.md) holds for $m$. The identities of nested nonempty [groups](../../../../../group-split.md) agree: the smaller identity remains an [idempotent](../../../../../idempotent.md) under the larger [group operation](../../../../../group-operation.md), whose only [idempotent](../../../../../idempotent.md) is its identity. Hence the whole chain has a common identity. Each element's inverse in a carrier remains its inverse in every larger carrier, so it is an inverse in the union as well. Thus $(A,m)$ satisfies all [group axioms](../../../../../group-axioms.md) and

$$
\boxed{\bigcup\mathcal C\in\mathcal G.}
$$

It is an [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) for the chain. The empty chain also has an [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) because $\mathcal G$ is nonempty, completing the hypothesis needed for [Zorn's lemma](../../../../../zorn-s-lemma.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
