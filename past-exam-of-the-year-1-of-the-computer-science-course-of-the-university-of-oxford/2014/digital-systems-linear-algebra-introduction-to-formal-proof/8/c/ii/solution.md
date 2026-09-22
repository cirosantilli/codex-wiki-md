<h1 id="8/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Eliminate the existential premise with fresh witness $a$. Its first conjunct gives $Q(a)$ and its second gives $\forall y\,(Q(y)\to y=a)$. For a fresh arbitrary $b$, one direction of the desired [logical biconditional](../../../../../../logical-biconditional.md) follows by [universal elimination](../../../../../../universal-quantifier-elimination-rule.md). For the other, $b=a$ must be reversed before transporting $Q(a)$ to $Q(b)$ using the supplied oriented [equality elimination rule](../../../../../../equality-elimination-rule.md).

| Line | Context | Formula | Justification |
| --- | --- | --- | --- |
| 1 | $\{1\}$ | $\exists x\,(Q(x)\land\forall y\,(Q(y)\to y=x))$ | Premise |
| 2 | $\{1,2\}$ | $Q(a)\land\forall y\,(Q(y)\to y=a)$ | Temporary assumption |
| 3 | $\{1,2\}$ | $Q(a)$ | [conjunction elimination rule](../../../../../../conjunction-elimination-rule.md) $\land\text{-elim-L}$ on 2 |
| 4 | $\{1,2\}$ | $\forall y\,(Q(y)\to y=a)$ | [conjunction elimination rule](../../../../../../conjunction-elimination-rule.md) $\land\text{-elim-R}$ on 2 |
| 5 | $\{1,2\}$ | $Q(b)\to b=a$ | [universal elimination](../../../../../../universal-quantifier-elimination-rule.md) $\forall\text{-elim}$ on 4; instantiate at $b$ |
| 6 | $\{1,2,6\}$ | $b=a$ | Temporary assumption |
| 7 | $\{1,2,6\}$ | $b=b$ | [equality introduction rule](../../../../../../equality-introduction-rule.md) $=\text{-intro}$ |
| 8 | $\{1,2,6\}$ | $a=b$ | [equality elimination rule](../../../../../../equality-elimination-rule.md) $=\text{-elim}$ on 6, 7 |
| 9 | $\{1,2,6\}$ | $Q(b)$ | [equality elimination rule](../../../../../../equality-elimination-rule.md) $=\text{-elim}$ on 8, 3 |
| 10 | $\{1,2\}$ | $b=a\to Q(b)$ | [implication introduction rule](../../../../../../implication-introduction-rule.md) $\to\text{-intro}$ on 9; discharge 6 |
| 11 | $\{1,2\}$ | $Q(b)\leftrightarrow b=a$ | [biconditional introduction rule](../../../../../../biconditional-introduction-rule.md) $\leftrightarrow\text{-intro}$ on 5, 10 |
| 12 | $\{1,2\}$ | $\forall y\,(Q(y)\leftrightarrow y=a)$ | [universal introduction](../../../../../../universal-quantifier-introduction-rule.md) $\forall\text{-intro}$ on 11; $b$ fresh |
| 13 | $\{1,2\}$ | $\exists x\,\forall y\,(Q(y)\leftrightarrow y=x)$ | [existential quantifier introduction rule](../../../../../../existential-quantifier-introduction-rule.md) $\exists\text{-intro}$ on 12; witness $a$ |
| 14 | $\{1\}$ | $\exists x\,\forall y\,(Q(y)\leftrightarrow y=x)$ | [existential quantifier elimination rule](../../../../../../existential-quantifier-elimination-rule.md) $\exists\text{-elim}$ on 1, 13; discharge 2; $a$ fresh |

Here $b$ is absent from every open assumption when line 12 uses [universal introduction](../../../../../../universal-quantifier-introduction-rule.md). In line 13 the [existential quantifier](../../../../../../existential-quantification.md) binds the witness position occupied by $a$; the conclusion then has no free $a$, allowing line 14 to close its witness subproof. Hence

$$
\boxed{\exists x\,(Q(x)\land\forall y\,(Q(y)\to y=x))\vdash\exists x\,\forall y\,(Q(y)\leftrightarrow y=x).}
$$

The premise says an object satisfying $Q$ exists and every object satisfying $Q$ equals it. The [logical biconditional](../../../../../../logical-biconditional.md) adds the converse explicitly: every object equal to that witness also satisfies $Q$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
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
