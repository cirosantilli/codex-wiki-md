# Embedded Markov chain at level exits

↑ **Parent:** [Markov chain](markov-chain-split.md)

Suppose motion within each level ends on hitting one of two boundaries, and each boundary transition resets the process to a fixed entry state of an adjacent level. Observe only the successive level exits. The resulting level process is a [Markov chain](markov-chain-split.md), with transition [probabilities](probability.md) equal to the within-level boundary-hitting [probabilities](probability.md). The fixed-entry condition matters: without it, retaining only the level may discard information needed for the next transition law.

For a [simple symmetric random walk](simple-symmetric-random-walk.md) on local rooms $0,\ldots,r$, starting each excursion at room $1$, the [gambler's ruin](gambler-s-ruin.md) [probability](probability.md) of reaching $r$ first is $1/r$. Thus the level chain moves up with [probability](probability.md) $1/r$ and down with [probability](probability.md) $(r-1)/r$. Independent future decisions, or more generally the [Strong Markov property](strong-markov-property.md), justify restarting this calculation after each exit.

For two active levels between absorbing levels $0$ and $3$, starting on level $1$, put $p=1/r$ and $q=1-p$. The success [probabilities](probability.md) satisfy $u=pv$ and $v=p+qu$, hence

$$
u=\frac{p^2}{1-pq}.
$$

For $r=4$, the result is $1/13$. This compression illustrates how unbiased microscopic choices can produce a biased coarse [random walk](random-walk-split.md) when entry points are close to one boundary.

## ↑ Ancestors (7)

1. [Markov chain](markov-chain-split.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/9/c/solution.md)
