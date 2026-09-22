# Randomized algorithm

↑ **Parent:** [Algorithm](algorithm-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Randomized_algorithm)

A randomized algorithm makes some choices using random bits.

For a fixed [input](input-computer-science.md), the random [bits](bit.md) can change the path taken by a [randomized algorithm](randomized-algorithm.md), its [output](output-computing.md), or its running time. Specify the distribution of those choices and which guarantee is required: [one-sided error](one-sided-error.md) permits mistakes of only one kind, whereas [ZPP](zpp.md) requires a correct answer and bounds the expected running time. [Polynomial identity testing](polynomial-identity-testing.md) makes this distinction concrete: choosing different [field](field.md) elements changes whether a nonidentity is detected.

A [uniform distribution on a finite set](discrete-uniform-distribution.md) must be implemented faithfully. To choose uniformly from $\{0,1,2,3,4\}$ using fair [independent](independent-random-variables.md) [bits](bit.md), read three [bits](bit.md) as a number from zero to seven, discard five through seven, and repeat until a permitted value appears. Each retained value has the same chance. Taking the three-bit number modulo five instead would give zero, one and two twice as many preimages as three and four, invalidating a calculation that assumes equal chances.

**Table of contents**

- [Derandomization](derandomization.md)
  - [Method of conditional probabilities](method-of-conditional-probabilities.md)
    - [Conditional expectation choice invariant](conditional-expectation-choice-invariant.md)
    - [Conditional expectations for maximum cut](conditional-expectations-for-maximum-cut.md)
      - [Conditional expectation cut formula](conditional-expectation-cut-formula.md)
      - [Conditional expectations cut example](conditional-expectations-cut-example.md)
      - [Conditional expectations algorithm cost](conditional-expectations-algorithm-cost.md)
- [Probabilistic Turing machine](probabilistic-turing-machine.md)
- [One-sided error](one-sided-error.md)
  - [RP (complexity)](rp-complexity.md)
  - [co-RP](co-rp.md)
- [ZPP](zpp.md)
- [Error reduction for a randomized algorithm](error-reduction-for-a-randomized-algorithm.md)
- [Polynomial identity testing](polynomial-identity-testing.md)
  - [Polynomial identity testing over a finite field](polynomial-identity-testing-over-a-finite-field.md)
  - [Random evaluation test for a polynomial identity](random-evaluation-test-for-a-polynomial-identity.md)
  - [Independent repetition of a polynomial identity test](independent-repetition-of-a-polynomial-identity-test.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Amortized analysis](amortized-analysis.md)
- [Conditional expectations algorithm cost](conditional-expectations-algorithm-cost.md)
- [Fully polynomial randomized approximation scheme](fully-polynomial-randomized-approximation-scheme.md)
- [One-sided error](one-sided-error.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-124/4/i/solution.md)
- [Randomized algorithm](randomized-algorithm.md)
- [Semicoloring](semicoloring.md)
- [Universal hash family](universal-hash-family.md)
- [Wald's equation](wald-s-equation.md)
