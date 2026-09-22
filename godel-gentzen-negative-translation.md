<h1 id="godel-gentzen-negative-translation">Gödel-Gentzen negative translation</h1>

↑ **Parent:** [Intuitionistic first-order logic](intuitionistic-first-order-logic.md)

For an [atomic formula](atomic-formula.md) $P$ (including [logical equality](logical-equality.md)), put $P^N=\neg\neg P$, and put $\bot^N=\bot$. Preserve [logical conjunction](logical-conjunction.md), [logical implication](logical-implication.md) and [universal quantification](universal-quantification.md) recursively, while setting

$$
(A\lor B)^N=\neg\neg(A^N\lor B^N),\qquad (\exists x\,A)^N=\neg\neg\exists x\,A^N.
$$

[Logical negation](negation.md) is [logical implication](logical-implication.md) to [logical falsity](logical-falsity.md), so $(\neg A)^N=\neg A^N$. The displayed [logical disjunction](logical-disjunction.md) and existence clauses are intuitionistically equivalent to the usual negative forms $\neg(\neg A^N\land\neg B^N)$ and $\neg\forall x\,\neg A^N$. Every translated [first-order formula](first-order-formula.md) is stable by [stability of a formula under double negation](stability-of-a-formula-under-double-negation.md). In classical logic the translation is equivalent to the original [first-order formula](first-order-formula.md) by [mathematical induction](mathematical-induction.md) and [double-negation elimination](double-negation-elimination.md).

**Table of contents**

- [Negative translation of a classical proof](negative-translation-of-a-classical-proof.md)

## ↑ Ancestors (7)

1. [Intuitionistic first-order logic](intuitionistic-first-order-logic.md)
2. [First-order logic](first-order-logic.md)
3. [Mathematical logic](mathematical-logic-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Logical equality](logical-equality.md)
- [Negative translation of a classical proof](negative-translation-of-a-classical-proof.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135/5/solution.md)
