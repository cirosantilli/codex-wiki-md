# Universal hash family

↑ **Parent:** [Hash function](hash-function.md)

A [universal hash family](universal-hash-family.md) is a finite collection $\mathcal H$ of [hash functions](hash-function.md) into an [output](output-computing.md) [set](set-split.md) of size $q$ such that, for any fixed distinct [inputs](input-computer-science.md) $x,y$,

$$
\Pr_{h\in\mathcal H}[h(x)=h(y)]\leq\frac1q.
$$

The choice of $h$ uses the [uniform distribution on a finite set](discrete-uniform-distribution.md). The keys are fixed before that choice: the randomness belongs to the [hash function](hash-function.md), so the guarantee does not assume naturally random keys. Choose one member and keep it while using the table; changing it requires redistributing the stored records. The bound holds separately for every distinct pair, without requiring uniform individual [outputs](output-computing.md) or [independent random variables](independent-random-variables.md). A [strongly universal hash family](strongly-universal-hash-family.md) supplies those stronger properties.

The practical payoff follows from [linearity of expectation](linearity-of-expectation.md). If $n$ stored keys are distinct from a fixed query, let $C$ count how many share its bucket. Then $\mathbb E[C]\leq n/q$: each key contributes at most $1/q$ to the [expected value](expected-value.md). With $100$ stored keys and $100$ buckets, an unsuccessful search encounters at most one record on average over the random choice of [hash function](hash-function.md). This is an [expected value](expected-value.md), not a limit on every search; one unlucky choice can still create a long chain.

This calculation needs no [independence](independent-random-variables.md) between the collision events: [linearity of expectation](linearity-of-expectation.md) adds their individual [probabilities](probability.md). The fixed-query condition matters, since deliberately choosing keys after inspecting the selected [hash function](hash-function.md) can target a crowded bucket.

Carter and Wegman introduced this way of analyzing storage and retrieval in their 1977 paper: average over a chosen class of [hash functions](hash-function.md) while allowing any fixed sequence of [inputs](input-computer-science.md). Their 1979 journal version develops the same universal-pair collision condition and constructions. The insight is useful because a [randomized algorithm](randomized-algorithm.md) can obtain a performance guarantee through its own choices, even when its [inputs](input-computer-science.md) have inconvenient patterns.[Carter and Wegman, Universal classes of hash functions, STOC 1977](https://dl.acm.org/doi/10.1145/800105.803400)[Carter and Wegman, Universal Classes of Hash Functions, 1979](https://www.cs.princeton.edu/courses/archive/fall09/cos521/Handouts/universalclasses.pdf)

**Table of contents**

- [Strongly universal hash family](strongly-universal-hash-family.md)

## ↑ Ancestors (3)

1. [Hash function](hash-function.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Almost strongly universal hash family](almost-strongly-universal-hash-family.md)
- [Birthday probability for hash outputs](birthday-probability-for-hash-outputs.md)
- [Hash function](hash-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-54/3/solution.md)
- [Separate chaining](separate-chaining.md)
- [Strongly universal hash family](strongly-universal-hash-family.md)
- [Universal hash family](universal-hash-family.md)
