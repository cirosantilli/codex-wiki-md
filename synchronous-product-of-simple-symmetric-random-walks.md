# Synchronous product of simple symmetric random walks

↑ **Parent:** [Product Markov chain](product-markov-chain.md)

Take $d$ [independent](independent-random-variables.md) copies of the [simple random walk on the integer line](simple-random-walk-on-the-integer-line.md), each stepping left or right with equal [probability](probability.md) at every integer time. Their [product Markov chain](product-markov-chain.md) moves all coordinates at once; each of its $2^d$ diagonal increments has [probability](probability.md) $2^{-d}$. At odd times a return to the origin is impossible. At time $2n$, [independence](independent-random-variables.md) gives the displayed return probability, whose [asymptotic equivalence](asymptotic-equivalence.md) follows from [Stirling's approximation](stirling-formula.md). The [recurrence criterion by return probabilities](recurrence-criterion-by-return-probabilities.md) and the [p-series](p-series.md) therefore imply [recurrence](recurrent-markov-chain.md) for $d=1,2$ and a [transient Markov chain](transient-markov-chain.md) for $d\geq3$.

For $d>1$ the chain from the origin visits only the [sublattice](sublattice-euclidean-geometry.md) whose coordinates all have the same parity. This is one [communicating class](communicating-class.md); restricting to it gives an [irreducible Markov chain](irreducible-markov-chain.md). The [period of a state in a Markov chain](period-of-a-state-in-a-markov-chain.md) is two here. The conclusion applies to that class, without incorrectly claiming [Markov chain irreducibility](irreducible-markov-chain.md) on all of $\mathbb Z^d$. This walk moves diagonally; the usual axis-step [simple random walk](simple-random-walk.md) has different transition probabilities, even though the same dimensional recurrence threshold holds.

## ↑ Ancestors (8)

1. [Product Markov chain](product-markov-chain.md)
2. [Markov chain](markov-chain-split.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2014/3/c/iii/solution.md)
