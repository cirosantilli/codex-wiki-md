<h1 id="8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Push the outer [negation](../../../../../negation.md) inward using [De Morgan's laws](../../../../../de-morgan-s-laws.md) and the duality of universal and existential [quantifiers](../../../../../quantifier.md). Negating the outer universal [quantifier](../../../../../quantifier.md) first gives an existential $x$. Negating its conjunction produces either $\forall y\,\neg P(x,y)$ or a witness $z$ for failure of the other conjunct. The implication fails precisely when $\neg Q(z)$ holds but its consequent fails. Therefore a [negation normal form](../../../../../negation-normal-form.md) is

$$
\boxed{\exists x\left(
(\forall y\,\neg P(x,y))\lor
\exists z\left(\neg Q(z)\land
\left(\neg P(x,z)\lor\forall t\,\neg P(z,t)\right)\right)
\right).}
$$

All [negations](../../../../../negation.md) now apply directly to [atomic formulas](../../../../../atomic-formula.md). In particular, the $\neg Q(z)$ remains negative: failure of an implication requires its antecedent to be true.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [8](../../8.md)
3. [Introduction to formal proof](../../introduction-to-formal-proof.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
