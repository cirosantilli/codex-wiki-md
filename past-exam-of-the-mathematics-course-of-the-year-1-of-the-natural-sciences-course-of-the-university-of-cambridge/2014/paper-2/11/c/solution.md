<h1 id="11/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the usual model of independent games, each with Sheila-win [probability](../../../../../probability.md) $\theta$. After $m+n$ games, an outcome with $m$ wins and $n$ losses has $\binom{m+n}{m}$ possible orders. Since both totals are below eleven, none of those sequences has already ended the match. Thus

$$
\boxed{P(m\text{ wins},n\text{ losses})=\binom{m+n}{m}\theta^m(1-\theta)^n}.
$$

For a completed Sheila win with $n$ losses, the last game must be her eleventh win. The preceding $10+n$ games contain ten wins and $n$ losses, so their [probability](../../../../../probability.md) is $\binom{10+n}{10}\theta^{10}(1-\theta)^n$, followed by one further factor $\theta$. The allowed loss counts are $0\leq n\leq10$, and these terminal events are disjoint. Hence

$$
\boxed{P(\text{Sheila wins match})=
\sum_{n=0}^{10}\binom{10+n}{10}\theta^{11}(1-\theta)^n}.
$$

This is the [match win probability with a fixed winning score](../../../../../match-win-probability-with-a-fixed-winning-score.md), obtained by the [negative binomial stopping argument](../../../../../negative-binomial-stopping-argument.md). Constant marginal game-win [probabilities](../../../../../probability.md) alone would not justify the product without the usual independence assumption.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [11](../../11.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
