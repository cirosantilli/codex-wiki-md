# Negative binomial stopping argument

↑ **Parent:** [Negative binomial distribution](negative-binomial-distribution.md)

For the [negative binomial distribution](negative-binomial-distribution.md) with positive [integer](integer-split.md) target $r$ and success [probability](probability.md) $0<p<1$, the $r$th success occurs after exactly $x$ failures only if the final trial is a success, while the preceding $x+r-1$ trials contain $x$ failures and $r-1$ successes. Choosing the failure locations gives the [binomial coefficient](binomial-coefficient-split.md) $\binom{x+r-1}{x}$. Each such stopped sequence has [probability](probability.md) $(1-p)^xp^r$ by [independence](independent-random-variables.md), and the sequences describe mutually exclusive [events](event.md), so their [probabilities](probability.md) add. This proves the [probability mass function](probability-mass-function.md). Counting arrangements among all $x+r$ positions would wrongly include sequences that already reached the target earlier. The same argument is used for three heads in [MIT 18.05, spring 2022, problem set 9 solutions, problem 2(b)](https://ocw.mit.edu/courses/18-05-introduction-to-probability-and-statistics-spring-2022/mit18_05_s22_pset09_sol.pdf).

A short route to normalization and moments is to split the failures count into successive waiting blocks:

$$
X=F_1+\cdots+F_r,
$$

where $F_i$ counts failures after success $i-1$ and before success $i$, with $F_1$ starting at the first trial. Fresh [independent](independent-random-variables.md) [Bernoulli trials](bernoulli-trial.md) make the blocks [independent](independent-random-variables.md), each with the failures-count [geometric distribution](geometric-distribution.md). Each block has total mass $p\sum_{j=0}^{\infty}(1-p)^j=1$ by the [geometric series](geometric-series.md), so their sum also defines a normalized [probability distribution](probability-distribution-split.md). The [linearity of expectation](linearity-of-expectation.md) and [variance additivity for independent random variables](variance-additivity-for-independent-random-variables.md) give $\mathbb E X=r(1-p)/p$ and $\operatorname{Var}(X)=r(1-p)/p^2$. This makes the moments transparent without a long calculation of sums. For $p=1$, every block is zero.

**Table of contents**

- [Success-count and waiting-time duality](success-count-and-waiting-time-duality.md)
- [Success-failure stopping identity](success-failure-stopping-identity.md)
- [Match win probability with a fixed winning score](match-win-probability-with-a-fixed-winning-score.md)

## ↑ Ancestors (8)

1. [Negative binomial distribution](negative-binomial-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Negative binomial distribution](negative-binomial-distribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-2/12f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/5j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-1/12/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-1/12/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/11/c/solution.md)
- [Success-failure stopping identity](success-failure-stopping-identity.md)
