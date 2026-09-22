<h1 id="s/s2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**A fixed proposal-count budget does not [bias](../../../../../bias-of-an-estimator.md) the accepted values.** For each trial, acceptance has probability $a$, and conditional on acceptance its label has law $p$ independently of the other trials. Conditional on the full accept/reject pattern among the first $N^*$ proposals, the successful labels are [independent](../../../../../independent-random-variables.md) with common law $p$. Therefore $K\sim\operatorname{Binomial}(N^*,a)$, and conditional on $K=k$, the $k$ retained samples are [independent](../../../../../independent-random-variables.md) draws from $p$. When $K=0$ there is simply no sample. This concerns a budget fixed independently of the proposal values; it does not assert that an empirical average is defined on an empty output.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [S2](../../s2.md)
3. [S](../../../s.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
