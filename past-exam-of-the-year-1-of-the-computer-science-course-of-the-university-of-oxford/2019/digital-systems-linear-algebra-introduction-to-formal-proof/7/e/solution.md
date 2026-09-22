<h1 id="7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the two [derived inference rules](../../../../../derived-inference-rule.md) whose complete [proofs](../../../../../mathematical-proof.md) were supplied in (d). The following [logical derivation](../../../../../logical-derivation.md) has **no nested hypothetical subproofs**:

```
1  P → Q                           premise
2  Q → R                           premise
3  P → (Q → R)                     → creation from 2
4  (P → Q) → (P → R)               → distribution from 3
5  P → R                           →-elim, 1 and 4
```

The creation instance takes $\phi=P$ and $\psi=(Q\to R)$. The distribution instance takes $(\phi,\psi,\rho)=(P,Q,R)$. The metarules are justified in (d); this requested flat use does not secretly invoke [implication introduction rule](../../../../../implication-introduction-rule.md) in one of its own lines.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
