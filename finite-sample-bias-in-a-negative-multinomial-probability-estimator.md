# Finite-sample bias in a negative multinomial probability estimator

↑ **Parent:** [Negative multinomial distribution](negative-multinomial-distribution.md)

For $n$ independent one-stop [negative multinomial distribution](negative-multinomial-distribution.md) observations, the natural estimates are $\widehat\alpha=S_X/(n+S_X+S_Y)$ and $\widehat\beta=S_Y/(n+S_X+S_Y)$. Their sum is $g((S_X+S_Y)/n)$ with strictly concave $g(z)=z/(1+z)$, so [Jensen's inequality](jensen-s-inequality.md) makes its expectation strictly below $\alpha+\beta$. Conditional category proportions split this bias between both estimates. With zero observed counts of a category, that estimate lies at zero; in a parameter space requiring strict positivity the likelihood supremum is not attained.

## ↑ Ancestors (9)

1. [Negative multinomial distribution](negative-multinomial-distribution.md)
2. [Multinomial distribution](multinomial-distribution.md)
3. [Discrete probability distribution](discrete-probability-distribution-split.md)
4. [Probability distribution](probability-distribution.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-2/19h/solution.md)
