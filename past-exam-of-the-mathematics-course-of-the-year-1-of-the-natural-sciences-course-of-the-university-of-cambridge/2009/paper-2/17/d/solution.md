<h1 id="17/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under a uniform shuffle, every unordered five-card hand is equally likely, giving $\binom{52}{5}$ possible hands. Choose the triple's rank in 13 ways and its suits in $\binom43$ ways; then choose a different pair rank in 12 ways and its suits in $\binom42$ ways. Each full house determines these choices uniquely, so there is no further ordering factor. Therefore

$$
\boxed{N=13\binom43\,12\binom42=3744,\qquad P=\frac{3744}{\binom{52}{5}}.}
$$

The count uses [binomial coefficients](../../../../../binomial-coefficient-split.md) because the order of cards within a hand is irrelevant.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [17](../../17.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
