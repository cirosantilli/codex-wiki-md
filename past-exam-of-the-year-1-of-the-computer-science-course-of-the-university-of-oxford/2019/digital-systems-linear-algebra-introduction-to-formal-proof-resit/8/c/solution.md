<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For readability write $R(s,t)$ for the uninterpreted relation $s\ni t$. In the first [proof](../../../../../mathematical-proof.md), introduce the universal quantifier _inside_ the existential witness scope:

| Line | Formula | Justification |
| --- | --- | --- |
| 1 | $\exists y\,\forall x\,R(x,y)$ | Premise |
| 2 | $\forall x\,R(x,w)$ | Assume with fresh witness name $w$ |
| 3 | $R(u,w)$ | [Universal quantifier elimination rule](../../../../../universal-quantifier-elimination-rule.md), 2; choose fresh arbitrary $u$ |
| 4 | $\exists y\,R(u,y)$ | [Existential quantifier introduction rule](../../../../../existential-quantifier-introduction-rule.md), 3 |
| 5 | $\forall x\,\exists y\,R(x,y)$ | [Universal quantifier introduction rule](../../../../../universal-quantifier-introduction-rule.md), 4; $u$ is absent from open assumptions |
| 6 | $\forall x\,\exists y\,R(x,y)$ | [Existential quantifier elimination rule](../../../../../existential-quantifier-elimination-rule.md), 1 and 2–5 |

In the second [proof](../../../../../mathematical-proof.md), first close the witness scope and _then_ generalize the arbitrary object:

| Line | Formula | Justification |
| --- | --- | --- |
| 1 | $\exists y\,\forall x\,R(x,y)$ | Premise; choose $u$ arbitrary and fresh for this premise |
| 2 | $\forall x\,R(x,w)$ | Assume with fresh $w$, also different from $u$ |
| 3 | $R(u,w)$ | [Universal quantifier elimination rule](../../../../../universal-quantifier-elimination-rule.md), 2 |
| 4 | $\exists y\,R(u,y)$ | [Existential quantifier introduction rule](../../../../../existential-quantifier-introduction-rule.md), 3 |
| 5 | $\exists y\,R(u,y)$ | [Existential quantifier elimination rule](../../../../../existential-quantifier-elimination-rule.md), 1 and 2–4 |
| 6 | $\forall x\,\exists y\,R(x,y)$ | [Universal quantifier introduction rule](../../../../../universal-quantifier-introduction-rule.md), 5 |

These are distinct [proof](../../../../../mathematical-proof.md) trees: the final two rule applications are interchanged, and their freshness conditions have been checked in their respective contexts. They express the [quantifier order and uniform witness](../../../../../quantifier-order-and-uniform-witness.md) principle: a single witness working for every object also supplies a witness for each object individually.

**The converse is not valid.** In a domain $\{0,1\}$ interpret $R(s,t)$ as equality of its arguments. Every object has a witness, namely itself, but no one object equals both 0 and 1. The premise of the converse is true and its conclusion false. The symbol $\ni$ is an arbitrary binary relation here; no set-membership axioms may be imposed on it without an additional premise.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
