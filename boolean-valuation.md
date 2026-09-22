# Boolean valuation

↑ **Parent:** [Propositional logic](propositional-logic.md)

A [Boolean valuation](boolean-valuation.md) $v$ assigns each primitive [proposition](proposition.md) a value in $\{\mathrm F,\mathrm T\}$, equivalently $\{0,1\}$, and extends recursively to every [propositional formula](propositional-formula.md) using the classical [logical connectives](logical-connective.md). The same primitive [proposition](proposition.md) always receives the same value within one [Boolean valuation](boolean-valuation.md). For compound [propositional formulas](propositional-formula.md) $A$ and $B$,

$$
\begin{aligned}
v(\neg A)=\mathrm T&\iff v(A)=\mathrm F,\\
v(A\land B)=\mathrm T&\iff v(A)=\mathrm T\text{ and }v(B)=\mathrm T,\\
v(A\lor B)=\mathrm T&\iff v(A)=\mathrm T\text{ or }v(B)=\mathrm T,\\
v(A\to B)=\mathrm F&\iff v(A)=\mathrm T\text{ and }v(B)=\mathrm F.
\end{aligned}
$$

Every other case receives the opposite value. Thus $v(p)=\mathrm T,v(q)=\mathrm F$ gives $v((p\to q)\land p)=\mathrm F$. A [truth table](truth-table.md) varies the assignment; recursive evaluation computes one row. The truth-functional restriction means that changing what the primitive [propositions](proposition.md) describe, while retaining their values, cannot change the value of the compound [propositional formula](propositional-formula.md). See [forall x: Calgary, chapter 9](https://forallx.openlogicproject.org/html/Ch9.html) and [section 10.1](https://forallx.openlogicproject.org/html/Ch10.html).

**Table of contents**

- [Truth table](truth-table.md)

## ↑ Ancestors (6)

1. [Propositional logic](propositional-logic.md)
2. [Mathematical logic](mathematical-logic-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (70)

- [3-SAT reduction to vertex cover](3-sat-reduction-to-vertex-cover.md)
- [Boolean formula](boolean-formula.md)
- [Boolean game](boolean-game.md)
- [Boolean literal](boolean-literal.md)
- [Boolean operation](boolean-operation.md)
- [Boolean satisfiability problem](boolean-satisfiability-problem.md)
- [Boolean valuation](boolean-valuation.md)
- [Boolean variable](boolean-variable.md)
- [Clause of a Boolean formula](clause-of-a-boolean-formula.md)
- [Conjunctive normal form](conjunctive-normal-form.md)
- [De Morgan's laws](de-morgan-s-laws.md)
- [Endpoint-false disjunctive normal form](endpoint-false-disjunctive-normal-form.md)
- [Equivalence of weighted formula utility representations](equivalence-of-weighted-formula-utility-representations.md)
- [Existential equilibrium checking in a Boolean game](existential-equilibrium-checking-in-a-boolean-game.md)
- [Extended omitting types theorem for propositional logic](extended-omitting-types-theorem-for-propositional-logic.md)
- [Finite-variable dependence of a propositional rule base](finite-variable-dependence-of-a-propositional-rule-base.md)
- [Implicant](implicant.md)
- [Logical equivalence](logical-equivalence.md)
- [Logical validity](logical-validity.md)
- [Logical variable](logical-variable.md)
- [Minterm](minterm.md)
- [One-preserving Boolean function](one-preserving-boolean-function.md)
- [Partial Boolean assignment](partial-boolean-assignment.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computational-complexity/2/d/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computational-complexity/2/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/knowledge-representation-and-reasoning/3/f/ii/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/logic-and-proof/1/c/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/logic-and-proof/1/d/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/logic-and-proof/1/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/logic-and-proof/1/f/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/2/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/1/f/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/1/g/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/1/i/solution.md)
- [Solution](past-exam-of-the-logic-and-set-theory-course-of-the-university-of-oxford/2007/a/1/i/solution.md)
- [Solution](past-exam-of-the-logic-and-set-theory-course-of-the-university-of-oxford/2007/a/1/ii/solution.md)
- [Solution](past-exam-of-the-logic-and-set-theory-course-of-the-university-of-oxford/2007/a/1/iii/solution.md)
- [Solution](past-exam-of-the-logic-and-set-theory-course-of-the-university-of-oxford/2008/a/1/g/solution.md)
- [Solution](past-exam-of-the-logic-and-set-theory-course-of-the-university-of-oxford/2008/a/2/a/solution.md)
- [Solution](past-exam-of-the-logic-and-set-theory-course-of-the-university-of-oxford/2008/a/2/b/solution.md)
- [Solution](past-exam-of-the-logic-and-set-theory-course-of-the-university-of-oxford/2008/a/2/c/solution.md)
- [Solution](past-exam-of-the-logic-and-set-theory-course-of-the-university-of-oxford/2008/a/4/a/solution.md)
- [Solution](past-exam-of-the-logic-and-set-theory-course-of-the-university-of-oxford/2011/a/1/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-20/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-38/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/16i/solution.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2022/computational-game-theory/2/c/solution.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2023/computational-game-theory/1/c/solution.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2023/computational-game-theory/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/7/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/7/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/7/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/7/d/solution.md)
- [Propositional formula](propositional-formula.md)
- [Propositional logic](propositional-logic.md)
- [Propositional theory](propositional-theory.md)
- [Propositional type](propositional-type.md)
- [Propositional variable](propositional-variable.md)
- [Quadratic-size formula with prescribed model count](quadratic-size-formula-with-prescribed-model-count.md)
- [Replacement theorem for logical equivalence](replacement-theorem-for-logical-equivalence.md)
- [Satisfying assignment](satisfying-assignment.md)
- [Satisfying-assignment count for nested implications](satisfying-assignment-count-for-nested-implications.md)
- [Semantic entailment](semantic-entailment.md)
- [Tautology](tautology.md)
- [Truth table](truth-table.md)
- [Truth value](truth-value.md)
- [Unit propagation](unit-propagation.md)
- [Unsatisfiable Boolean formula](unsatisfiable-boolean-formula.md)
- [Verifying a satisfying assignment](verifying-a-satisfying-assignment.md)
- [Weighted formula utility representation](weighted-formula-utility-representation.md)
