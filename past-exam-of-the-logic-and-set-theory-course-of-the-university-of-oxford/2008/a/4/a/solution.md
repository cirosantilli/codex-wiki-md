<h1 id="a/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a standard classical propositional calculus, strong completeness states

$$
\boxed{\Gamma\models\phi\quad\Longrightarrow\quad\Gamma\vdash\phi.}
$$

Together with [soundness](../../../../../soundness.md), this identifies semantic consequence with [formal derivability](../../../../../formal-derivability.md). One proves the contrapositive by the [maximal consistent set in propositional logic](../../../../../maximal-consistent-set-in-propositional-logic.md) construction. If $\Gamma\nvdash\phi$, the [set](../../../../../set-split.md) $\Gamma\cup\{\neg\phi\}$ is [propositionally consistent](../../../../../propositional-consistency.md), by the [deduction theorem for propositional logic](../../../../../deduction-theorem-for-propositional-logic.md) and classical propositional reasoning. Extend it to a [maximal consistent set in propositional logic](../../../../../maximal-consistent-set-in-propositional-logic.md) $M$, deciding each [logical formula](../../../../../logical-formula.md) in turn. At each stage at least one selection of $\theta$ or $\neg\theta$ preserves [propositional consistency](../../../../../propositional-consistency.md); a contradiction in the [union](../../../../../set-union.md) would use only finitely many assumptions and hence already occur at a stage.

Define a [Boolean valuation](../../../../../boolean-valuation.md) by $v(p_i)=1$ exactly when $p_i\in M$. [Maximal consistency in propositional logic](../../../../../maximal-consistency-in-propositional-logic.md) gives $\neg\theta\in M$ exactly when $\theta\notin M$, and $(\theta\to\eta)\in M$ exactly when either $\theta\notin M$ or $\eta\in M$. [Structural induction](../../../../../structural-induction.md) on [logical formulas](../../../../../logical-formula.md) therefore proves the [maximal consistent set truth lemma](../../../../../maximal-consistent-set-truth-lemma.md) $v(\theta)=1\Longleftrightarrow\theta\in M$. Thus $v$ satisfies $\Gamma$ but falsifies $\phi$, contradicting [semantic entailment](../../../../../semantic-entailment.md). The countable language here permits an enumeration of [logical formulas](../../../../../logical-formula.md); the corresponding general-language argument uses a [well-ordering](../../../../../well-order.md) or a principle of [maximality in a partially ordered set](../../../../../maximality-in-a-partially-ordered-set.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
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
