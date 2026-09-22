<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the [Gödel-Gentzen negative translation](../../../../../godel-gentzen-negative-translation.md), writing $A^N$ for the translated [first-order formula](../../../../../first-order-formula.md). On [atomic formulas](../../../../../atomic-formula.md) $P$, including [logical equality](../../../../../logical-equality.md), put $P^N=\neg\neg P$, and put $\bot^N=\bot$. Extend recursively by

$$
\begin{aligned}
(A\land B)^N&=A^N\land B^N,&(A\to B)^N&=A^N\to B^N,\\
(\forall x\,A)^N&=\forall x\,A^N,&(A\lor B)^N&=\neg\neg(A^N\lor B^N),\\
(\exists x\,A)^N&=\neg\neg\exists x\,A^N.&
\end{aligned}
$$

[Logical negation](../../../../../negation.md) abbreviates [logical implication](../../../../../logical-implication.md) to [logical falsity](../../../../../logical-falsity.md), so $(\neg A)^N=\neg A^N$. The displayed [logical disjunction](../../../../../logical-disjunction.md) and existential clauses are intuitionistically equivalent to the usual negative clauses $\neg(\neg A^N\land\neg B^N)$ and $\neg\forall x\,\neg A^N$, respectively. Thus these clauses specify the same [negative interpretation](../../../../../godel-gentzen-negative-translation.md). Translation commutes with [capture-avoiding substitution](../../../../../capture-avoiding-substitution.md) of terms for [free variables](../../../../../free-variable.md).

First prove by [structural induction](../../../../../structural-induction.md) the [stability of a formula under double negation](../../../../../stability-of-a-formula-under-double-negation.md):

$$
\mathrm{IL}\vdash\neg\neg A^N\to A^N.
$$

Every double [logical negation](../../../../../negation.md) is stable, since [intuitionistic first-order logic](../../../../../intuitionistic-first-order-logic.md) proves $\neg\neg\neg\neg C\to\neg\neg C$; [logical falsity](../../../../../logical-falsity.md) is stable as well. Stability passes to [logical conjunction](../../../../../logical-conjunction.md) by obtaining double [logical negation](../../../../../negation.md) of each component. For a [logical implication](../../../../../logical-implication.md) $C\to D$ with stable $D$, assume $\neg\neg(C\to D)$ and $C$. An assumption $\neg D$ would give $\neg(C\to D)$, a contradiction, so $\neg\neg D$ and then $D$. For a universal [first-order formula](../../../../../first-order-formula.md), $\neg\neg\forall x\,C(x)$ implies $\neg\neg C(y)$ for arbitrary fresh $y$; use stability pointwise and generalize. [Logical disjunction](../../../../../logical-disjunction.md) and existential translations are already double negations. This proves all cases.

Now regard classical first-order [natural deduction](../../../../../natural-deduction.md) as intuitionistic [natural deduction](../../../../../natural-deduction.md) plus unrestricted [double-negation elimination](../../../../../double-negation-elimination.md), and induct on a classical derivation. The rules for [logical conjunction](../../../../../logical-conjunction.md), [logical implication](../../../../../logical-implication.md), [universal quantification](../../../../../universal-quantification.md) and [logical falsity](../../../../../logical-falsity.md) translate directly. [Logical disjunction](../../../../../logical-disjunction.md) introduction gives $A^N\lor B^N$ and then its double [logical negation](../../../../../negation.md). For [logical disjunction](../../../../../logical-disjunction.md) elimination, the translated premise is $\neg\neg(A^N\lor B^N)$ and the two translated branches yield the stable conclusion $C^N$. Assuming $\neg C^N$ makes each branch contradictory, giving $\neg A^N$ and $\neg B^N$, hence $\neg(A^N\lor B^N)$, which contradicts the premise. We have $\neg\neg C^N$ and remove it by stability.

Existential introduction likewise adds a double [logical negation](../../../../../negation.md) to the ordinary witness introduction. In existential elimination, the witness branch $A^N(y)\vdash C^N$ has the original fresh-variable condition. Assuming $\neg C^N$ makes that branch give $\neg A^N(y)$; generalization gives $\forall y\,\neg A^N(y)$ and therefore $\neg\exists y\,A^N(y)$, contradicting the translated premise. Again stability supplies $C^N$. The universal-rule side conditions are preserved because the translation introduces no new [free variables](../../../../../free-variable.md).

For [logical equality](../../../../../logical-equality.md), reflexivity gives $t=t$ and then its double [logical negation](../../../../../negation.md). For substitution, from $\neg\neg(s=t)$ and $A^N(s)$, temporarily assume $\neg A^N(t)$. An assumption $s=t$ would transport $A^N(s)$ to $A^N(t)$ by intuitionistic [logical equality](../../../../../logical-equality.md) substitution, so it gives a contradiction and hence $\neg(s=t)$. The first premise contradicts this. Thus $\neg\neg A^N(t)$ holds and stability gives $A^N(t)$. Finally a classical [double-negation elimination](../../../../../double-negation-elimination.md) step translates precisely to $\neg\neg A^N\to A^N$, already proved. Every rule is therefore covered, giving [negative translation of a classical proof](../../../../../negative-translation-of-a-classical-proof.md):

$$
\boxed{\Gamma\vdash_{\mathrm{CL}}\varphi\quad\Longrightarrow\quad\Gamma^N\vdash_{\mathrm{IL}}\varphi^N.}
$$

In particular a classical thesis has an intuitionistic, constructive translated proof. If nonlogical assumptions are present, they must be translated too.

In classical logic, [double-negation elimination](../../../../../double-negation-elimination.md) gives $P^N\leftrightarrow P$ on atoms. [Structural induction](../../../../../structural-induction.md) propagates equivalence through [logical conjunction](../../../../../logical-conjunction.md), [logical implication](../../../../../logical-implication.md) and both quantifiers, and removes the added double negations on [logical disjunction](../../../../../logical-disjunction.md) and existence. Therefore

$$
\boxed{\mathrm{CL}\vdash\varphi^N\leftrightarrow\varphi,\qquad\mathrm{CL}\vdash\varphi\ \Longrightarrow\ \mathrm{IL}\vdash\varphi^N.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 135](../../paper-135-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
