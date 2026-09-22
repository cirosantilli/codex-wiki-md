<h1 id="a/1/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

First eliminate implication and biconditional using the [logical equivalences](../../../../../../logical-equivalence.md)

$$
A\to B\equiv\neg A\lor B,\qquad A\leftrightarrow B\equiv(\neg A\lor B)\land(\neg B\lor A).
$$

Push negations inwards using [De Morgan's laws](../../../../../../de-morgan-s-laws.md) and eliminate double negations. [Structural induction](../../../../../../structural-induction.md) leaves only literals joined by conjunction and disjunction.

Now induct on that remaining expression. A literal is already in [conjunctive normal form](../../../../../../conjunctive-normal-form.md). A conjunction of two [conjunctive normal forms](../../../../../../conjunctive-normal-form.md) is again one after associating its clauses. For a disjunction, write the two inductively obtained forms as $\bigwedge_i C_i$ and $\bigwedge_j D_j$ and use distributivity:

$$
\boxed{\left(\bigwedge_i C_i\right)\lor\left(\bigwedge_j D_j\right)\equiv\bigwedge_{i,j}(C_i\lor D_j).}
$$

Each $C_i\lor D_j$ is a clause. All operations preserve [logical equivalence](../../../../../../logical-equivalence.md), proving the required form exists.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the logic and set theory course of the University of Oxford](../../../../../split.md)
7. [Logic and set theory course of the University of Oxford](../../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
