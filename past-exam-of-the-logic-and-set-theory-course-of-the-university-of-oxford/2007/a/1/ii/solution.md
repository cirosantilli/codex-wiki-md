<h1 id="a/1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Two [propositional formulas](../../../../../propositional-formula.md) are [logically equivalent](../../../../../logical-equivalence.md) if every [Boolean valuation](../../../../../boolean-valuation.md) gives them the same [truth value](../../../../../truth-value.md). A [disjunctive normal form](../../../../../disjunctive-normal-form.md) is a [logical disjunction](../../../../../logical-disjunction.md) of [logical conjunctions](../../../../../logical-conjunction.md) of [literals](../../../../../boolean-literal.md), with a [literal](../../../../../boolean-literal.md) being a [propositional variable](../../../../../propositional-variable.md) or its [negation](../../../../../negation.md).

Let $p_1,\ldots,p_n$ include all [propositional variables](../../../../../propositional-variable.md) appearing in $\phi$. For each [Boolean valuation](../../../../../boolean-valuation.md) $s\in\{T,F\}^n$, put

$$
M_s=\bigwedge_{j=1}^n L_{s,j},\qquad
L_{s,j}=\begin{cases}p_j&s_j=T,\\\neg p_j&s_j=F.\end{cases}
$$

The [minterm](../../../../../minterm.md) $M_s$ is true exactly for [Boolean valuations](../../../../../boolean-valuation.md) whose restrictions to these [propositional variables](../../../../../propositional-variable.md) are $s$. Consequently

$$
\boxed{\phi\equiv\bigvee_{s:\,\widetilde s(\phi)=T}M_s.}
$$

Indeed, an [Boolean valuation](../../../../../boolean-valuation.md) making $\phi$ true makes its own [minterm](../../../../../minterm.md) true, while a true [minterm](../../../../../minterm.md) in the displayed [logical disjunction](../../../../../logical-disjunction.md) certifies the truth of $\phi$. There are only finitely many [Boolean valuations](../../../../../boolean-valuation.md), so this is a finite [disjunctive normal form](../../../../../disjunctive-normal-form.md). If there are no satisfying [Boolean valuations](../../../../../boolean-valuation.md), use $p\wedge\neg p$ for any [propositional variable](../../../../../propositional-variable.md) $p$; this is a [disjunctive normal form](../../../../../disjunctive-normal-form.md) for falsity without needing an empty [logical disjunction](../../../../../logical-disjunction.md) convention.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [A](../../../a.md)
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
