# A function of a Markov chain need not be Markov

↑ **Parent:** [Lumped Markov chain](lumped-markov-chain.md)

A function of the current state of a [Markov chain](markov-chain-split.md) can discard information needed to predict its next value. A sufficient condition preserving the [Markov property](markov-property.md) is [strong lumpability](strong-lumpability.md): all original states with the same recorded value must give the same transition probabilities to every recorded class.

For the two-column model in [growth rate of two-column sticky deposition](growth-rate-of-two-column-sticky-deposition.md), the pair of column heights is Markov, but its maximum alone is not. Starting empty, the maximum-height histories $(1,1,2)$ and $(1,2,2)$ both end at height two. The former leaves unequal columns, so the next height increases with probability $1/2$; the latter leaves equal columns, so it increases with probability one. Each history has positive probability. Their different predictions at the same time and current value violate the [Markov property](markov-property.md). By contrast, the absolute height difference retains exactly the information needed for its own transitions.

## ↑ Ancestors (8)

1. [Lumped Markov chain](lumped-markov-chain.md)
2. [Markov chain](markov-chain-split.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2017/3/b/i/solution.md)
