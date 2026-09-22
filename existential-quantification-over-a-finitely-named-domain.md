# Existential quantification over a finitely named domain

↑ **Parent:** [Existential quantification](existential-quantification.md)

Assume $\forall x\,(x=c_1\lor\cdots\lor x=c_n)$ with $n\ge1$. For the forward implication, open a fresh existential witness, instantiate domain exhaustiveness at it, and split into the equality cases. The [equality elimination rule](equality-elimination-rule.md) transfers its predicate to the corresponding constant, which supplies the required disjunct. Closing the witness scope is legal because the result contains only the named constants. Conversely each named instance gives the existential by the [existential quantifier introduction rule](existential-quantifier-introduction-rule.md), and cases combine those derivations. The constants need not denote distinct objects. A negated named instance can eliminate one case through contradiction and [logical falsity elimination rule](logical-falsity-elimination-rule.md).

## ↑ Ancestors (8)

1. [Existential quantification](existential-quantification.md)
2. [First-order formula](first-order-formula.md)
3. [First-order logic](first-order-logic.md)
4. [Mathematical logic](mathematical-logic-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof-resit/8/d/solution.md)
