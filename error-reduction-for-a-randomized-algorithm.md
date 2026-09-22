# Error reduction for a randomized algorithm

↑ **Parent:** [Randomized algorithm](randomized-algorithm.md)

Independent repetitions reduce a randomized algorithm's error probability while preserving polynomial running time.

The combining rule depends on the error orientation. For [one-sided error](one-sided-error.md) with false acceptance [probability](probability.md) at most $p<1$, reject as soon as any trial rejects and accept only if every trial accepts. For $k$ [independent](independent-random-variables.md) trials on the same fixed negative [input](input-computer-science.md), false acceptance has [probability](probability.md) at most $p^k$. The protected positive [inputs](input-computer-science.md) still always accept. If false rejection is the possible mistake instead, accept as soon as any trial accepts. This uses the decisive answer rather than a majority vote.

For constant $p<1$, $k$ grows only logarithmically in $1/\varepsilon$ to achieve error at most $\varepsilon$. A polynomial number of trials preserves a [polynomial-time algorithm](polynomial-time-algorithm.md)'s running-time bound. Independence matters: repeating one answer, or evaluating at the same random point each time, supplies no new evidence. The [independent repetition of a polynomial identity test](independent-repetition-of-a-polynomial-identity-test.md) gives an exact $25$-outcome example.

## ↑ Ancestors (4)

1. [Randomized algorithm](randomized-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
