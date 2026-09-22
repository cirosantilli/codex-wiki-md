# Posterior coin count after exactly one head

↑ **Parent:** [Bayes' theorem](bayes-theorem.md)

Let $N$ have the positive-integer [geometric distribution](geometric-distribution.md) with success parameter $p\in(0,1)$, and conditionally toss $N$ independent coins with head [probability](probability.md) $\theta\in(0,1)$. Exactly one head has conditional [probability](probability.md) $n\theta(1-\theta)^{n-1}$. Combining this with the prior by [Bayes' theorem](bayes-theorem.md) gives the displayed posterior with $r=(1-p)(1-\theta)$; its normalization uses $\sum_{n\geq1}nr^{n-1}=(1-r)^{-2}$. For $p=\theta=1/2$, the posterior is $9n/4^{n+1}$. It is also a shifted [negative binomial distribution](negative-binomial-distribution.md), with $N-1$ equal in law to the number of failures before two successes of [probability](probability.md) $1-r$.

## ↑ Ancestors (7)

1. [Bayes' theorem](bayes-theorem.md)
2. [Conditional probability](conditional-probability.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-2/3f/solution.md)
