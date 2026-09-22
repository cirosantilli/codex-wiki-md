<h1 id="5j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**This does not model the full three-category response.** A [binomial distribution](../../../../../../binomial-distribution.md) has two outcome classes, whereas the observed damage factor has three. In base R, a factor response to a binomial [generalized linear model](../../../../../../generalized-linear-model.md) is coded as first level versus all other levels; this would silently collapse the categories. It would also treat the nine table rows as nine individual observations, ignoring the frequencies. A deliberate binary analysis would require specifying the collapse and retaining the counts, but cannot recover the full damage distribution.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5J](../../5j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
