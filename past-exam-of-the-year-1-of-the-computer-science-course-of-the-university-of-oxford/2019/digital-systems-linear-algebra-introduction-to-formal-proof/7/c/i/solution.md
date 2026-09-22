<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Retain the two given [logical implications](../../../../../../logical-implication.md) and temporarily assume their common starting [proposition](../../../../../../proposition.md).

```
1  P → Q                    premise
2  Q → R                    premise
3  | P                      assume
4  | Q                      →-elim, 3 and 1
5  | R                      →-elim, 4 and 2
6  P → R                    →-intro, discharge 3–5
```

Only the original premises remain undischarged, giving the required composition of [logical implications](../../../../../../logical-implication.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
