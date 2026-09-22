# Method of conditional probabilities

↑ **Parent:** [Derandomization](derandomization.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Method_of_conditional_probabilities)

The method of conditional probabilities turns an [expected value](expected-value-split.md) guarantee into a deterministic construction. For a maximization [objective function](objective-function.md), fix one choice at a time, always keeping the [conditional expectation](conditional-expectation.md) of the final value at least as large as before. Once every choice is fixed, that [conditional expectation](conditional-expectation.md) is the actual value. The useful ingredient is a way to evaluate the [conditional expectations](conditional-expectation.md) efficiently.

No actual random choices are needed during this construction. The [probability distribution](probability-distribution-split.md) describes hypothetical completions used in the analysis; the algorithm compares their [conditional expectations](conditional-expectation.md) and commits deterministically. For [maximum cut](maximum-cut.md), this converts the [random cut lower bound](random-cut-lower-bound.md) into a [cut of a graph](cut-graph-theory.md) containing at least half the [edges](edge-of-a-graph.md). A [maximum cut](maximum-cut.md) can still be larger, as the [conditional expectations cut example](conditional-expectations-cut-example.md) shows.

**Table of contents**

- [Conditional expectation choice invariant](conditional-expectation-choice-invariant.md)
- [Conditional expectations for maximum cut](conditional-expectations-for-maximum-cut.md)
  - [Conditional expectation cut formula](conditional-expectation-cut-formula.md)
  - [Conditional expectations cut example](conditional-expectations-cut-example.md)
  - [Conditional expectations algorithm cost](conditional-expectations-algorithm-cost.md)

## ↑ Ancestors (5)

1. [Derandomization](derandomization.md)
2. [Randomized algorithm](randomized-algorithm.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Derandomization](derandomization.md)
- [Golden ratio approximation for MAX-2SAT](golden-ratio-approximation-for-max-2sat.md)
- [Maximum 2-satisfiability](maximum-2-satisfiability.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-37/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-37/6/d/solution.md)
- [Polynomial-time algorithm](polynomial-time-algorithm.md)
