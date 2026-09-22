<h1 id="5j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**This is not a valid ordinary R glm family specification.** A [multinomial distribution](../../../../../../multinomial-distribution.md) is natural for the three damage counts conditional on the row total, but base R's [generalized linear model](../../../../../../generalized-linear-model.md) interface does not supply a family named multinomial. Furthermore, the written response is one cell count, not a three-category response or grouped multinomial vector. A properly specified [multinomial logistic regression](../../../../../../multinomial-logistic-regression.md) could model category probabilities by group, but it is not the model fit by this command. The independent-count [log-linear model](../../../../../../log-linear-model.md) in part (a), conditional on the margins, is the appropriate supplied alternative.

## ↑ Ancestors (11)

1. [B](../b.md)
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
