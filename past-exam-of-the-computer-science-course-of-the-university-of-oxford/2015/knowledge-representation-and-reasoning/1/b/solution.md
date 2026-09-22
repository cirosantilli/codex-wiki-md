<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $S,T,U,M,F,Q,J$ for the [atomic formulas](../../../../../atomic-formula.md) $\mathit{Student}(x)$, $\mathit{Takes}(x,\mathit{KRR},2015)$, $\mathit{Undergrad}(x)$, $\mathit{Masters}(x)$, $\mathit{FacultyMember}(x)$, $\mathit{GreaterOrEqual}(\mathit{CountSupervise}(x),2)$, and $\mathit{Teach}(x,y)$, respectively. These are abbreviations for formulas, not new symbols in the vocabulary. In [clausal normal form](../../../../../clausal-form.md), with all remaining variables implicitly universally quantified, the three translations become:

$$
\begin{array}{ll}
\text{(i)}&\neg S\lor\neg T\lor U\lor M,\\
&\neg S\lor\neg T\lor\neg U\lor\neg M;\\[2pt]
\text{(ii)}&\neg U\lor\mathit{SupervisedBy}(x,f(x)),\\
&\neg M\lor\mathit{SupervisedBy}(x,f(x));\\[2pt]
\text{(iii)}&\neg F\lor\neg Q\lor\neg J\lor\mathit{Busy}(x).
\end{array}
$$

For (ii), [Skolemization](../../../../../skolemization.md) introduces the fresh [Skolem function](../../../../../skolem-function.md) $f$. One supervisor suffices even when both categories hold, so the same $f$ can be used in both [first-order clauses](../../../../../first-order-clause.md). For (iii), moving the existentially quantified course out of an antecedent produces a universally quantified variable in the resulting [first-order clause](../../../../../first-order-clause.md):

$$
((F(x)\land Q(x)\land\exists y\,\mathit{Teach}(x,y))\to\mathit{Busy}(x))
\equiv\forall y\,((F(x)\land Q(x)\land\mathit{Teach}(x,y))\to\mathit{Busy}(x)).
$$

The [resolution with free selection](../../../../../resolution-with-free-selection.md) calculus for [first-order Horn clauses](../../../../../first-order-horn-clause.md) is sound and refutationally complete for the clause sets from $\boxed{\text{(ii) and (iii)}}$. For example, select the unique positive [first-order literal](../../../../../first-order-literal.md) in every definite [first-order Horn clause](../../../../../first-order-horn-clause.md), and select one negative [first-order literal](../../../../../first-order-literal.md) in every nonempty clause without a positive one. On the displayed definite [first-order Horn clauses](../../../../../first-order-horn-clause.md), this selects $\mathit{SupervisedBy}(x,f(x))$ or $\mathit{Busy}(x)$. A fair saturation must still consider all permitted inferences. Functions do not invalidate this completeness theorem, although they can prevent termination. [Section 2, “Resolution with Free Selection”: the selection condition and Horn resolution calculus](../../../../../rewriting-conjunctive-queries-under-description-logic-constraints.md)

The first [first-order clause](../../../../../first-order-clause.md) of (i) has two positive [first-order literals](../../../../../first-order-literal.md), so the Horn [resolution with free selection](../../../../../resolution-with-free-selection.md) theorem does not apply to that sentence. General [first-order resolution](../../../../../first-order-resolution.md), with its usual completeness requirements, can handle it. Soundness of an individual resolution inference is not the issue; the issue is applicability and completeness of this particular restricted calculus.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Knowledge representation and reasoning](../../../knowledge-representation-and-reasoning-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
