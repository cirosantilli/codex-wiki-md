<h1 id="8/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The existential premise is $\exists x\,(Q(x)\to R(x))$, with the [logical implication](../../../../../../logical-implication.md) inside the [existential quantifier](../../../../../../existential-quantification.md). Eliminate it using a fresh witness $a$, specialize $\forall x\,Q(x)$ to that same witness, and introduce the required [existential quantifier](../../../../../../existential-quantification.md) before closing the witness subproof:

| Line | Context | Formula | Justification |
| --- | --- | --- | --- |
| 1 | $\{1\}$ | $\exists x\,(Q(x)\to R(x))$ | Premise |
| 2 | $\{1,2\}$ | $\forall x\,Q(x)$ | Premise |
| 3 | $\{1,2,3\}$ | $Q(a)\to R(a)$ | Temporary assumption |
| 4 | $\{1,2,3\}$ | $Q(a)$ | [universal elimination](../../../../../../universal-quantifier-elimination-rule.md) $\forall\text{-elim}$ on 2; instantiate at $a$ |
| 5 | $\{1,2,3\}$ | $R(a)$ | [implication elimination rule](../../../../../../implication-elimination-rule.md) $\to\text{-elim}$ on 3, 4 |
| 6 | $\{1,2,3\}$ | $\exists x\,R(x)$ | [existential quantifier introduction rule](../../../../../../existential-quantifier-introduction-rule.md) $\exists\text{-intro}$ on 5; witness $a$ |
| 7 | $\{1,2\}$ | $\exists x\,R(x)$ | [existential quantifier elimination rule](../../../../../../existential-quantifier-elimination-rule.md) $\exists\text{-elim}$ on 1, 6; discharge 3; $a$ fresh |

The [eigenvariable](../../../../../../eigenvariable.md) $a$ is absent from the premises and from $\exists x\,R(x)$. Consequently,

$$
\boxed{\exists x\,(Q(x)\to R(x)),\ \forall x\,Q(x)\vdash\exists x\,R(x).}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
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
