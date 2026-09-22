<h1 id="b/6/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [cumulative hierarchy](../../../../../../cumulative-hierarchy.md) is defined by [transfinite recursion](../../../../../../transfinite-recursion.md):

$$
\boxed{V_0=\varnothing,\qquad V_{\alpha+1}=\mathcal P(V_\alpha),\qquad
V_\lambda=\bigcup_{\alpha<\lambda}V_\alpha\quad(\lambda\text{ a limit ordinal}).}
$$

This recursion on [ordinals](../../../../../../ordinal-split.md) is available without assuming the [Axiom of foundation](../../../../../../axiom-of-regularity.md) for all sets. The stages are increasing and transitive, by [transfinite induction](../../../../../../transfinite-induction.md) using their definitions.

Work internally in the specified model of ZF without the [Axiom of foundation](../../../../../../axiom-of-regularity.md), and assume the [membership induction theorem](../../../../../../membership-induction-theorem.md). Apply it to

$$
\varphi(x)\equiv\exists\alpha\in\mathrm{On}\ (x\in V_\alpha).
$$

Suppose every member $y$ of $x$ lies in some stage. Assign to each such $y$ the least [ordinal](../../../../../../ordinal-split.md) $\alpha_y$ for which $y\in V_{\alpha_y}$. The [Axiom schema of replacement](../../../../../../axiom-schema-of-replacement.md) gives a set of these [ordinals](../../../../../../ordinal-split.md), and let $\beta$ be their supremum, taking $\beta=0$ for the empty collection. Monotonicity gives $x\subseteq V_\beta$, and therefore $x\in V_{\beta+1}$.

This proves progressivity of $\varphi$, so membership induction gives it for every set of the model. Every stage already consists of sets in that model. Consequently

$$
\boxed{V^*=\bigcup_{\alpha\in\mathrm{On}}V_\alpha.}
$$

The equality is internal to the given model; its [ordinals](../../../../../../ordinal-split.md) and power sets are computed there.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [D](../../d.md)
3. [6](../../../6.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../../split.md)
7. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
