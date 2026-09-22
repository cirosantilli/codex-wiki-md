<h1 id="7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Assume the [logical conjunction](../../../../../logical-conjunction.md) temporarily, then eliminate the premise's [logical disjunction](../../../../../logical-disjunction.md) by cases. A [natural deduction](../../../../../natural-deduction.md) proof, with each indented assumption delimiting its own subproof, is:

```
1.  not P or not Q                    premise
2.  | P and Q                        temporary assumption
3.  | P                              and-elim-L, 2
4.  | Q                              and-elim-R, 2
5.  | | not P                        first disjunction case
6.  | | false                        not-elim, 3,5
7.  | | not Q                        second disjunction case
8.  | | false                        not-elim, 4,7
9.  | false                          or-elim, 1, cases 5-6 and 7-8
10. not (P and Q)                     not-intro, discharge 2-9
```

Lines 5–6 and 7–8 are separate sibling subproofs, not one nested inside the other. Both derive the same contradiction under the common assumption on line 2. [Logical disjunction](../../../../../logical-disjunction.md) elimination discharges the two case assumptions, and [negation](../../../../../negation.md) introduction then discharges the [logical conjunction](../../../../../logical-conjunction.md) assumption. The sole undischarged premise is the required one. This proof uses only the supplied [logical conjunction](../../../../../logical-conjunction.md), [logical disjunction](../../../../../logical-disjunction.md) and [negation](../../../../../negation.md) rules; no converse form of [De Morgan's laws](../../../../../de-morgan-s-laws.md) is being assumed as an extra rule.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
