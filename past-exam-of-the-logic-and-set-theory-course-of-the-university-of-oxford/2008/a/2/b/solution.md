<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Translate [logical formulas](../../../../../logical-formula.md) recursively, leaving [propositional variables](../../../../../propositional-variable.md) unchanged and translating [negation](../../../../../negation.md) by applying [negation](../../../../../negation.md) to the translation. For the other two [logical connectives](../../../../../logical-connective.md) [set](../../../../../set-split.md)

$$
T(\psi\lor\chi)=(\neg T(\psi)\to T(\chi)),\qquad
T(\psi\land\chi)=\neg(T(\psi)\to\neg T(\chi)).
$$

The first [logical implication](../../../../../logical-implication.md) is false exactly when both original inputs are false; the second displayed [logical formula](../../../../../logical-formula.md) is true exactly when both inputs are true. Hence each clause preserves [truth values](../../../../../truth-value.md). [Structural induction](../../../../../structural-induction.md) gives $v(T(\theta))=v(\theta)$ for every [Boolean valuation](../../../../../boolean-valuation.md) and every [logical formula](../../../../../logical-formula.md) $\theta$ in the larger language.

By the assumed [functional completeness](../../../../../functional-completeness.md) of [negation](../../../../../negation.md), [logical conjunction](../../../../../logical-conjunction.md) and [logical disjunction](../../../../../logical-disjunction.md), any finite [Boolean function](../../../../../boolean-function.md) has such a [logical formula](../../../../../logical-formula.md) $\theta$. Its translation $T(\theta)$ uses only [negation](../../../../../negation.md) and [logical implication](../../../../../logical-implication.md) and represents the same [function](../../../../../function-split.md). **Thus $\{\neg,\to\}$ is adequate.**

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
