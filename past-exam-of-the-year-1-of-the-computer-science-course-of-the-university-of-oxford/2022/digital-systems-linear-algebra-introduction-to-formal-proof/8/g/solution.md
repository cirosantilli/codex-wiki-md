<h1 id="8/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The printed expression has one unmatched closing parenthesis. Remove that final surplus parenthesis and read the first disjunct as $\exists x\,P(x)$; the other disjunct has outer [universal quantification](../../../../../universal-quantification.md) over the displayed implication. To distinguish the two independent bound uses of $x$, rename the first to $u$.

Push the outer [negation](../../../../../negation.md) through the [logical disjunction](../../../../../logical-disjunction.md) and through the [quantifiers](../../../../../quantifier.md). Negating the implication preserves its existential antecedent and negates its consequent. Applying [De Morgan's laws](../../../../../de-morgan-s-laws.md) and the [quantifier](../../../../../quantifier.md) negation rules gives the [negation normal form](../../../../../negation-normal-form.md)

$$
\boxed{\bigl(\forall u\,\neg P(u)\bigr)\land\exists x\left[\bigl(\exists y\,Q(x,y)\bigr)\land\bigl(\forall z\,\neg R(z)\bigr)\land\bigl(\exists t\,\neg T(x,t)\bigr)\right].}
$$

Each [negation](../../../../../negation.md) is now directly before an [atomic formula](../../../../../atomic-formula.md). No [bound variable](../../../../../bound-variable.md) has been captured, and no original [existential quantification](../../../../../existential-quantification.md) in the antecedent has accidentally been negated twice.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
