<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Extract the universally quantified [logical implication](../../../../../../logical-implication.md) and the existentially quantified [logical conjunction](../../../../../../logical-conjunction.md) from the premise. Use one fresh witness $a$ for both conjuncts of the latter, so that the resulting $R(a)$ and $\neg S(a)$ concern the same object:

| Line | Context | Formula | Justification |
| --- | --- | --- | --- |
| 1 | $\{1\}$ | $(\forall x\,(Q(x)\to R(x)))\land(\exists x\,(Q(x)\land\neg S(x)))$ | Premise |
| 2 | $\{1\}$ | $\forall x\,(Q(x)\to R(x))$ | [conjunction elimination rule](../../../../../../conjunction-elimination-rule.md) $\land\text{-elim-L}$ on 1 |
| 3 | $\{1\}$ | $\exists x\,(Q(x)\land\neg S(x))$ | [conjunction elimination rule](../../../../../../conjunction-elimination-rule.md) $\land\text{-elim-R}$ on 1 |
| 4 | $\{1,4\}$ | $Q(a)\land\neg S(a)$ | Temporary assumption |
| 5 | $\{1,4\}$ | $Q(a)$ | [conjunction elimination rule](../../../../../../conjunction-elimination-rule.md) $\land\text{-elim-L}$ on 4 |
| 6 | $\{1,4\}$ | $\neg S(a)$ | [conjunction elimination rule](../../../../../../conjunction-elimination-rule.md) $\land\text{-elim-R}$ on 4 |
| 7 | $\{1,4\}$ | $Q(a)\to R(a)$ | [universal elimination](../../../../../../universal-quantifier-elimination-rule.md) $\forall\text{-elim}$ on 2; instantiate at $a$ |
| 8 | $\{1,4\}$ | $R(a)$ | [implication elimination rule](../../../../../../implication-elimination-rule.md) $\to\text{-elim}$ on 7, 5 |
| 9 | $\{1,4\}$ | $R(a)\land\neg S(a)$ | [conjunction introduction rule](../../../../../../conjunction-introduction-rule.md) $\land\text{-intro}$ on 8, 6 |
| 10 | $\{1,4\}$ | $\exists x\,(R(x)\land\neg S(x))$ | [existential quantifier introduction rule](../../../../../../existential-quantifier-introduction-rule.md) $\exists\text{-intro}$ on 9; witness $a$ |
| 11 | $\{1\}$ | $\exists x\,(R(x)\land\neg S(x))$ | [existential quantifier elimination rule](../../../../../../existential-quantifier-elimination-rule.md) $\exists\text{-elim}$ on 3, 10; discharge 4; $a$ fresh |

The witness $a$ occurs in no undischarged premise or final conclusion. Therefore the [existential quantifier elimination rule](../../../../../../existential-quantifier-elimination-rule.md) is valid and gives

$$
\boxed{(\forall x\,(Q(x)\to R(x)))\land(\exists x\,(Q(x)\land\neg S(x)))\vdash\exists x\,(R(x)\land\neg S(x)).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
