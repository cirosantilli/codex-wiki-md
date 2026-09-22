# Geometric continuation after an initial tie

↑ **Parent:** [Geometric distribution](geometric-distribution.md)

Suppose a contest uses $N_0$ trials initially and ends there with probability $1-\alpha$. Conditional on an initial tie, independent further rounds each use $\ell$ trials and resolve the contest with a fixed probability $0<r\leq1$. The number $J$ of further rounds, conditional on that tie, has a [geometric distribution](geometric-distribution.md): $\Pr(J=j\mid\text{tie})=(1-r)^{j-1}r$ for $j\geq1$. Thus the total number $N$ of trials has an atom $1-\alpha$ at $N_0$ and the displayed probabilities thereafter. The geometric series sums to $\alpha$, so termination has probability one, and the [expected value](expected-value-split.md) is $\mathbb E[N]=N_0+\ell\alpha/r$. The displayed distribution requires independence of the future rounds from the initial tie.

## ↑ Ancestors (8)

1. [Geometric distribution](geometric-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-2/5/ii/solution.md)
