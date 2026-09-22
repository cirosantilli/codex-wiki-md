<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use a sequential [SATPlan](../../../../../satplan.md) encoding with times $t=0,\ldots,T$. The fluent universe is

$$
\mathcal P=\{\operatorname{On}(b,x):b\in\{A,B,C\},\ x\in\{A,B,C,\tau\}\setminus\{b\}\}\cup\{\operatorname{Clear}(A),\operatorname{Clear}(B),\operatorname{Clear}(C)\}.
$$

There are nine support [Boolean variables](../../../../../boolean-variable.md) and three clearance [Boolean variables](../../../../../boolean-variable.md) per time layer. Static block types, parameter inequalities and permanent table availability are handled during [action grounding](../../../../../action-grounding.md). For each well-typed [ground action](../../../../../ground-action.md) $a$ from parts (b)–(c), introduce an occurrence [Boolean variable](../../../../../boolean-variable.md) $a_t$ for $0\leq t<T$. Allow **at most one action per layer**, including no action, so that a horizon of $T$ encodes at most $T$ physical actions.

The complete initial-state formula is

$$
\begin{aligned}
I_0={}&\operatorname{On}(A,\tau)_0\land\operatorname{On}(B,\tau)_0\land\operatorname{On}(C,A)_0\\
&\land\operatorname{Clear}(B)_0\land\operatorname{Clear}(C)_0\land\neg\operatorname{Clear}(A)_0\\
&\land\neg\operatorname{On}(A,B)_0\land\neg\operatorname{On}(A,C)_0\\
&\land\neg\operatorname{On}(B,A)_0\land\neg\operatorname{On}(B,C)_0\\
&\land\neg\operatorname{On}(C,B)_0\land\neg\operatorname{On}(C,\tau)_0.
\end{aligned}
$$

Every well-typed fluent not initially true is explicitly false. The final goal formula is simply **$G_T=\operatorname{On}(A,B)_T\land\operatorname{On}(B,C)_T$**. Leaving unrelated final facts unconstrained is appropriate; leaving unrelated initial facts unconstrained would introduce imaginary starting states.

For each $t<T$, include all [action precondition axioms](../../../../../action-precondition-axiom.md) $a_t\to\bigwedge_{p\in\operatorname{Pre}(a)}p_t$, after removing static true conditions. For example,

$$
\operatorname{Move}(A,\tau,B)_t\to\operatorname{On}(A,\tau)_t\land\operatorname{Clear}(A)_t\land\operatorname{Clear}(B)_t.
$$

The [precondition](../../../../../precondition.md) axiom for $\operatorname{MoveToTable}(C,A)_t$ similarly requires $\operatorname{On}(C,A)_t\land\operatorname{Clear}(C)_t$.

For every fluent $p\in\mathcal P$, let $\operatorname{Add}_p(t)$ be the [logical disjunction](../../../../../logical-disjunction.md) of actions at $t$ adding $p$, and $\operatorname{Del}_p(t)$ the [logical disjunction](../../../../../logical-disjunction.md) deleting it. Include the [successor-state axiom](../../../../../successor-state-axiom.md)

$$
p_{t+1}\leftrightarrow\operatorname{Add}_p(t)\lor\bigl(p_t\land\neg\operatorname{Del}_p(t)\bigr).
$$

It combines action effects with the [frame axiom](../../../../../frame-axiom.md), preventing unsupported changes. A fully grounded example is

$$
\begin{aligned}
\operatorname{On}(A,B)_{t+1}\leftrightarrow{}&\operatorname{Move}(A,\tau,B)_t\lor\operatorname{Move}(A,C,B)_t\\
&\lor\bigl(\operatorname{On}(A,B)_t\land\neg\operatorname{Move}(A,B,C)_t\land\neg\operatorname{MoveToTable}(A,B)_t\bigr).
\end{aligned}
$$

Apply the same construction to every support and clearance fluent, using the exact add/delete lists. If no action occurs, both effect [logical disjunctions](../../../../../logical-disjunction.md) are false, so all fluents persist.

The sequential [action exclusion axioms](../../../../../action-exclusion-axiom.md) are $\neg a_t\lor\neg b_t$ for every pair of distinct grounded actions $a,b$. For example,

$$
\neg\operatorname{Move}(A,\tau,B)_t\lor\neg\operatorname{Move}(C,A,B)_t
$$

forbids selecting those two occurrences together. Do not add a requirement that some action occur in every layer: that would remove idle padding and change “at most $T$” into an exact-length requirement. One may additionally include true [planning state invariants](../../../../../planning-state-invariant.md), such as a block having at most one support and a block support carrying at most one block; the unlimited table must be exempt from the latter restriction.

Finally, conjoin $I_0$, $G_T$, and all precondition, successor and exclusion formulas over the layers to obtain $\varphi_T$. It is a [propositional formula](../../../../../propositional-formula.md); if a solver requires [conjunctive normal form](../../../../../conjunctive-normal-form.md), use a satisfiability-preserving [Tseitin transformation](../../../../../tseytin-transformation.md) with auxiliary [Boolean variables](../../../../../boolean-variable.md). The equivalence between this encoding and real action [sequences](../../../../../sequence.md) follows from [sequential SATPlan correctness](../../../../../sequential-satplan-correctness.md): a satisfying assignment induces exactly the stated [STRIPS](../../../../../strips.md) trajectory, and every sufficiently short valid [plan](../../../../../plan.md) supplies such an assignment.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
