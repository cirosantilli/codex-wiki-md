<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the strict-order convention appropriate to the membership relation. A bounded [logical formula](../../../../../logical-formula.md) is

$$
\begin{aligned}
TO(x)\ \equiv\;&(\forall u\in x)\,\neg(u\in u)\\
&\wedge(\forall u\in x)(\forall v\in x)(\forall w\in x)
\bigl((u\in v\wedge v\in w)\to u\in w\bigr)\\
&\wedge(\forall u\in x)(\forall v\in x)
\bigl(u=v\vee u\in v\vee v\in u\bigr).
\end{aligned}
$$

The first clause is irreflexivity, the second transitivity, and the third comparability of distinct elements. Irreflexivity and transitivity exclude $u\in v\in u$, so distinct elements cannot be ordered in both directions. These are exactly the axioms of a [strict total order](../../../../../strict-total-order.md) on the [set](../../../../../set-split.md) $x$, with $\in$ as its order relation.

Every displayed [quantifier](../../../../../quantifier.md) is bounded by $x$, so **$TO(x)$ is $\Sigma_0$**. The [logical formula](../../../../../logical-formula.md) does not assert that $x$ is transitive as a [set](../../../../../set-split.md), and no such additional assertion is needed to say that the restriction of membership to $x$ is a [total order](../../../../../total-order.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
