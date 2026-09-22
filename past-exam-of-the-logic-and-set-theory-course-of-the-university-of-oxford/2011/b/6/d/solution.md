<h1 id="b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\mathcal O$ be the set of strict total orders on $\kappa$. Each is a subset of $\kappa\times\kappa$, so the [square of an infinite cardinal](../../../../../square-of-an-infinite-cardinal.md) gives

$$
|\mathcal O|\leq2^{|\kappa\times\kappa|}=2^\kappa.
$$

For the lower bound, use the set $\kappa\times\{0,1\}$ and order the two-element blocks by their first coordinates, using the [well-order](../../../../../well-order.md) of $\kappa$. For every $A\subseteq\kappa$, put $(\alpha,0)$ before $(\alpha,1)$ exactly when $\alpha\in A$, reversing them otherwise. This defines a strict total order for each $A$, and different subsets give different orders. Transport these orders to $\kappa$ along a fixed [bijection](../../../../../bijection.md) $\kappa\times\{0,1\}\cong\kappa$. Thus $2^\kappa\leq|\mathcal O|$, and the [Cantor-Schröder-Bernstein theorem](../../../../../cantor-schroder-bernstein-theorem.md) gives

$$
\boxed{|\mathcal O|=2^\kappa.}
$$

If using the customary [axiom of choice](../../../../../axiom-of-choice.md) development of [infinite cardinal arithmetic](../../../../../infinite-cardinal-arithmetic.md), its use here is precisely to supply $\kappa\times\kappa\cong\kappa$ and $\kappa\times2\cong\kappa$. The ordering construction makes no further choices. It proves the [cardinality of the family of strict total orders](../../../../../cardinality-of-the-family-of-strict-total-orders.md). For $\kappa$ itself an [initial ordinal](../../../../../initial-ordinal.md), these particular product identities can also be proved in [ZF](../../../../../zermelo-fraenkel-set-theory.md) by well-ordering pairs according to their maximum coordinate, so full [axiom of choice](../../../../../axiom-of-choice.md) is stronger than this instance intrinsically requires.

## ↑ Ancestors (13)

1. [D](../d.md)
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
