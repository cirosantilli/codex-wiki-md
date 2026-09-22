# One-sided error

↑ **Parent:** [Randomized algorithm](randomized-algorithm.md)

A randomized decision algorithm has one-sided error when one answer is always correct and only the other answer can be mistaken.

The guarantee concerns each fixed [input](input-computer-science.md), with [probability](probability.md) taken over the choices of the [randomized algorithm](randomized-algorithm.md). Always state which answer is protected. In [polynomial identity testing](polynomial-identity-testing.md), call an [input](input-computer-science.md) positive when its [polynomial](polynomial-split.md) is identically zero, and let acceptance mean claiming an identity. Then the possibilities are:

| Actual [polynomial](polynomial-split.md) | Accept: claim identity | Reject: claim nonidentity |
| --- | --- | --- |
| Identically zero | Always correct; every trial accepts. | Impossible with exact [polynomial evaluation](polynomial-evaluation.md). |
| Nonzero | Possible mistake if the chosen point is a zero. | Always correct; the point is a witness. |

Thus a zero [polynomial evaluation](polynomial-evaluation.md) can leave uncertainty, but a nonzero [polynomial evaluation](polynomial-evaluation.md) settles the question. An error bound for a fixed nonzero [polynomial](polynomial-split.md) is not the [conditional probability](conditional-probability.md) that a particular accepted [input](input-computer-science.md) is an identity; that latter question would need a distribution on the [inputs](input-computer-science.md) as well.

In [computational complexity theory](computational-complexity-theory.md), a [polynomial-time algorithm](polynomial-time-algorithm.md) with this orientation and false acceptance [probability](probability.md) at most $1/2$ establishes membership in [co-RP](co-rp.md). Reversing the question to ask whether the [polynomial](polynomial-split.md) is nonzero gives the [RP](rp-complexity.md) orientation: negative instances are always rejected. The [random evaluation test for a polynomial identity](random-evaluation-test-for-a-polynomial-identity.md) explains the required [field](field.md), [total degree](total-degree-of-a-polynomial.md), sampling and evaluation assumptions.

**Table of contents**

- [RP (complexity)](rp-complexity.md)
- [co-RP](co-rp.md)

## ↑ Ancestors (4)

1. [Randomized algorithm](randomized-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Error reduction for a randomized algorithm](error-reduction-for-a-randomized-algorithm.md)
- [Independent repetition of a polynomial identity test](independent-repetition-of-a-polynomial-identity-test.md)
- [Randomized algorithm](randomized-algorithm.md)
