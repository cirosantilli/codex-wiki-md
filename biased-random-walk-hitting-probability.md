# Biased random walk hitting probability

↑ **Parent:** [Biased random walk](biased-random-walk.md)

For a [biased random walk](biased-random-walk.md) on the [nonnegative integers](natural-number.md) with upward [probability](probability.md) $p>q=1-p>0$, the [hitting probability](hitting-probability.md) of zero from $i$ is $(q/p)^i$. Indeed, [first-step analysis](first-step-analysis.md) gives $h_i=ph_{i+1}+qh_{i-1}$ for $i\geq1$, with $h_0=1$. Its characteristic roots are $1$ and $\beta=q/p$, so any solution is $A+(1-A)\beta^i$. Nonnegativity as $i\to\infty$ forces $A\geq0$ and hence a value at least $\beta^i$. This candidate itself satisfies the recurrence. The theorem on the [minimal nonnegative solution for hitting probabilities](hitting-probability-is-the-minimal-nonnegative-harmonic-extension.md) therefore identifies it with $h_i$. A walk on all of $\mathbb Z$ has the same probability until it first reaches zero.

## ↑ Ancestors (11)

1. [Biased random walk](biased-random-walk.md)
2. [Simple random walk on the integer line](simple-random-walk-on-the-integer-line.md)
3. [Random walk on a graph](random-walk-on-a-graph.md)
4. [Random walk](random-walk-split.md)
5. [Markov chain](markov-chain-split.md)
6. [Markov process](markov-process-split.md)
7. [Probability theory](probability-theory-split.md)
8. [Probability and statistics](probability-and-statistics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Minimum of an upward-biased random walk](minimum-of-an-upward-biased-random-walk.md)
- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2015/3/b/iii/solution.md)
