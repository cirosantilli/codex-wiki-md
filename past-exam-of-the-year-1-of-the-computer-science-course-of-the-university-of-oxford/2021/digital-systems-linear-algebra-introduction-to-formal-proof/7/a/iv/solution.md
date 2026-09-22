<h1 id="7/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Assume $E\to G$ under label $a$, $F\to G$ under label $b$, and $E\lor F$ under label $c$. A temporary case assumption $E$ gives $G$ by the [modus ponens rule](../../../../../../implication-elimination-rule.md) using $a$. A temporary case assumption $F$ gives $G$ by the [modus ponens rule](../../../../../../implication-elimination-rule.md) using $b$. The [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md) discharges these case assumptions and concludes $G$ under $a,b,c$.

Apply the [implication introduction rule](../../../../../../implication-introduction-rule.md) three times, discharging $c$, then $b$, then $a$. The resulting theorem is

$$
(E\to G)\to((F\to G)\to((E\lor F)\to G)).
$$

The displayed parentheses make explicit the right association of the source formula.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
