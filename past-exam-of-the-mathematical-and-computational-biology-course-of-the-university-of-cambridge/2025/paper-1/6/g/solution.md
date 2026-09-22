<h1 id="6/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

**Direct independent sampling is preferable.** The [posterior distribution](../../../../../bayesian-posterior.md) is the standard [beta distribution](../../../../../beta-distribution.md) $\operatorname{Beta}(9,38)$, for which exact [posterior moments](../../../../../posterior-moment.md) and standard random-number generators are available. For example, draw independent $U\sim\operatorname{Gamma}(9,1)$ and $V\sim\operatorname{Gamma}(38,1)$ with the same rate, and return $U/(U+V)$. This has the required [beta distribution](../../../../../beta-distribution.md) and avoids [Markov chain Monte Carlo](../../../../../markov-chain-monte-carlo.md) convergence problems. A correct, converged MCMC method could sample this target, but it is unnecessarily complicated here.

## ↑ Ancestors (13)

1. [G](../g.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
