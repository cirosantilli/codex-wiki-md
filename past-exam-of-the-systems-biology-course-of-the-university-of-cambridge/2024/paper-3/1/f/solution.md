<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Include both main effects and their [interaction term](../../../../../interaction-term.md):

```
fit_interaction <- lm(testosterone ~ weight * sex, data = mice)
```

Here `mice` denotes the data frame containing the named variables. In this R formula, `weight * sex` expands to `weight + sex + weight:sex`; it does not omit the main effects.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the systems biology course of the University of Cambridge](../../../../split.md)
6. [Systems Biology course of the University of Cambridge](../../../../../systems-biology-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
