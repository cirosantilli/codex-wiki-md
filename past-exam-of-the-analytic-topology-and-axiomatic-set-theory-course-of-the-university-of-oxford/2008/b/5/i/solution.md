<h1 id="b/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In first-order [set](../../../../../set-split.md) theory a [class in set theory](../../../../../class-set-theory.md) is a definable collection, written schematically $\{x:\theta(x,\vec p)\}$ using a [logical formula](../../../../../logical-formula.md) and [set](../../../../../set-split.md) parameters. A [class term](../../../../../class-term.md) is an abbreviation for such a defining condition; it does not add a new kind of object to the [quantifiers](../../../../../quantifier.md) of [ZF](../../../../../zermelo-fraenkel-set-theory.md). A [class in set theory](../../../../../class-set-theory.md) is proper if it is not the collection of elements of any [set](../../../../../set-split.md).

Define the [cumulative hierarchy](../../../../../cumulative-hierarchy.md) by [transfinite recursion](../../../../../transfinite-recursion.md):

$$
V_0=\varnothing,\qquad V_{\alpha+1}=\mathcal P(V_\alpha),\qquad
V_\lambda=\bigcup_{\alpha<\lambda}V_\alpha\quad(\lambda\text{ a nonzero limit ordinal}),
$$

and let $V=\{x:\exists\alpha\text{ ordinal }(x\in V_\alpha)\}$. Without [foundation](../../../../../axiom-of-regularity.md) this denotes the well-founded part produced by the hierarchy; it must not simply be assumed to contain every ambient [set](../../../../../set-split.md). [Transfinite recursion](../../../../../transfinite-recursion.md) on [ordinals](../../../../../ordinal-split.md) and the relevant [set](../../../../../set-split.md) constructions remain available in [ZF without foundation](../../../../../zf-without-foundation.md).

Prove transitivity by [transfinite induction](../../../../../transfinite-induction.md). The empty stage is transitive. Suppose $T=V_\alpha$ is transitive. Then each member of $T$ is a [subset](../../../../../subset.md) of $T$, so $T\subseteq\mathcal P(T)$. Also $\mathcal P(T)$ is transitive: if $u\in v\in\mathcal P(T)$, then $u\in T$ and, by transitivity of $T$, $u\subseteq T$, so $u\in\mathcal P(T)$. At a limit stage, a [union](../../../../../set-union.md) of [transitive sets](../../../../../transitive-set.md) is transitive. This proves transitivity at every stage.

Finally transitivity of $V_\alpha$ itself implies that every member is a [subset](../../../../../subset.md) of $V_\alpha$, giving

$$
\boxed{V_\alpha\subseteq\mathcal P(V_\alpha)=V_{\alpha+1}.}
$$

These successive inclusions and the limit definition also imply $V_\alpha\subseteq V_\beta$ whenever $\alpha\le\beta$. The argument has not used [foundation](../../../../../axiom-of-regularity.md). This leaf includes the unnumbered definitions preceding the source's three claims.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
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
