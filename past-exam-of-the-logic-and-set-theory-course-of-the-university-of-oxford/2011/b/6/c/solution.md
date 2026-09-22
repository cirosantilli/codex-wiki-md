<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the standard definition of [algebraic independence](../../../../../algebraic-independence.md), finite tuples are required to have distinct entries. Let $\mathcal P$ be the set of all subsets of $L$ with [algebraic independence](../../../../../algebraic-independence.md) over $K$, ordered by inclusion. It is nonempty because $\varnothing\in\mathcal P$.

If $\mathcal C$ is a chain in $\mathcal P$, put $U=\bigcup\mathcal C$. A finite tuple of distinct elements of $U$ lies in one member of $\mathcal C$: choose a member containing each element and take the largest of those finitely many members. A polynomial relation on that tuple would then be a polynomial relation in that member, contradicting its [algebraic independence](../../../../../algebraic-independence.md). Thus $U\in\mathcal P$ and is an upper bound. For the empty chain, $\varnothing$ is an upper bound. The [Zorn's lemma](../../../../../zorn-s-lemma.md) now gives a maximal member $B$, which is a [transcendence basis](../../../../../transcendence-basis.md) by the specified maximality criterion. To also recover the usual field-theoretic definition, if $a\in L$ were transcendental over $K(B)$, clearing denominators in a polynomial relation would show that $B\cup\{a\}$ still has [algebraic independence](../../../../../algebraic-independence.md) over $K$, contradicting maximality. Thus $L$ is algebraic over $K(B)$. Hence **every field extension has a [transcendence basis](../../../../../transcendence-basis.md)**.

There is a literal issue in the printed definition: it does not require the tuple entries to be distinct. With that wording, any nonempty $X$ fails the test: for $a\in X$, the nonzero polynomial $X_1-X_2$ vanishes on $(a,a)$, in every characteristic. Thus under the literal printed test the family is exactly $\{\varnothing\}$, and $\varnothing$ is its maximal member. The same chain-and-[Zorn's lemma](../../../../../zorn-s-lemma.md) argument still proves existence for that literal notion, but it is not the usual [transcendence basis](../../../../../transcendence-basis.md) notion. **The conventional result above uses distinct tuple entries.**

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
