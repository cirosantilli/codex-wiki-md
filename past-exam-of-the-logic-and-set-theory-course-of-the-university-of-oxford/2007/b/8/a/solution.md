<h1 id="b/8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Zorn's lemma](../../../../../zorn-s-lemma.md) states that a nonempty [partially ordered set](../../../../../partially-ordered-set.md) in which every [chain](../../../../../chain-in-a-partial-order.md) has an [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) contains a [maximal element](../../../../../maximal-element-of-a-partially-ordered-set.md). Here a [chain](../../../../../chain-in-a-partial-order.md) means a [subset](../../../../../subset.md) totally ordered by the inherited order; it need not have a greatest member.

View every [partial function](../../../../../partial-function.md) as its graph, a [subset](../../../../../subset.md) of $\mathbb R\times\mathbb R$. The family $\mathcal F$ is a [set](../../../../../set-split.md) by [axiom of separation](../../../../../axiom-schema-of-specification.md) from the [power set](../../../../../power-set.md) of this product. Let $\mathcal C\subseteq\mathcal F$ be a [chain](../../../../../chain-in-a-partial-order.md) and put $h=\bigcup\mathcal C$. If two members of the [union](../../../../../set-union.md) assign values to the same input, the [chain](../../../../../chain-in-a-partial-order.md) property makes one graph contain the other, so those values agree. Thus $h$ is a [partial function](../../../../../partial-function.md).

If $x\in\operatorname{dom}h$ and $q\in\mathbb Q$, choose a [chain](../../../../../chain-in-a-partial-order.md) member containing $x$ in its domain. Its rational-scalar closure gives $qx\in\operatorname{dom}h$. If $x,y\in\operatorname{dom}h$, choose two [chain](../../../../../chain-in-a-partial-order.md) members containing them; the larger one contains both, and therefore contains $x+y$ with value $h(x)+h(y)$. Hence $h$ satisfies the required additive identity and domain closure. Consequently

$$
\boxed{\bigcup\mathcal C\in\mathcal F,}
$$

and it is an [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) for the [chain](../../../../../chain-in-a-partial-order.md). For the empty [chain](../../../../../chain-in-a-partial-order.md) its [union](../../../../../set-union.md) is the [empty function](../../../../../empty-function.md), which satisfies the defining [logical implications](../../../../../logical-implication.md) vacuously, so this case is covered too.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
