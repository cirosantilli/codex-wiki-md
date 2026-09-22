# Repeat-until-success coding over an erasure channel

↑ **Parent:** [Binary erasure channel](binary-erasure-channel.md)

With [channel feedback](channel-feedback.md), resend each message [bit](bit.md) through a [binary erasure channel](binary-erasure-channel.md) until a non-erased copy arrives, then move to the next [bit](bit.md). The [channel decoder](channel-decoder.md) deletes erasure symbols, giving the message without error whenever transmission completes. For $q<1$, the waiting times have an [independent and identically distributed](independent-and-identically-distributed-random-variables.md) [geometric distribution](geometric-distribution.md) with [expectation](expected-value-split.md) $1/(1-q)$, so every finite message completes [almost surely](almost-sure-convergence.md). The [strong law of large numbers](strong-law-of-large-numbers.md) gives forward [code rate](code-rate.md) $n/\sum_{j=1}^nM_j\to1-q$, matching [channel capacity](channel-capacity.md). At $q=1$, transmission never completes. Independent erasure indicators, rather than independent message [bits](bit.md), are the essential hypothesis.

## ↑ Ancestors (7)

1. [Binary erasure channel](binary-erasure-channel.md)
2. [Discrete memoryless channel](discrete-memoryless-channel.md)
3. [Coding theory](coding-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Channel feedback](channel-feedback.md)
- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2023/3/c/i/solution.md)
