<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose distinct fresh variables $a,b$. Instantiate the outer [universal quantifier](../../../../../universal-quantification.md) first, then the inner one; generalize them in the opposite order.
```
1. ∀x ∀y P(x,y)         premise
2. ∀y P(a,y)            ∀E, 1
3. P(a,b)               ∀E, 2
4. ∀x P(x,b)            ∀I, 3, generalizing a
5. ∀y ∀x P(x,y)         ∀I, 4, generalizing b
```
Neither $a$ nor $b$ occurs free in the sole undischarged premise. Thus both [universal introduction](../../../../../universal-quantifier-introduction-rule.md) steps satisfy the [eigenvariable condition](../../../../../eigenvariable-condition.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
