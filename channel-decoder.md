# Channel decoder

↑ **Parent:** [Discrete memoryless channel](discrete-memoryless-channel.md)

A deterministic [channel decoder](channel-decoder.md) maps a received length-$n$ word over the output [alphabet](alphabet.md) $\mathcal Y$ to an estimated message label. Given message $m$, successful decoding means $g(Y^n)=m$, where $Y^n$ is the random received word after the [communication channel](communication-channel.md) acts on the [channel encoder](channel-encoder.md)'s word $f(m)$. The [channel decoder](channel-decoder.md) can recover a message despite changed symbols because it uses the relationships among complete [codewords](codeword.md). The [Shannon second coding theorem](noisy-channel-coding-theorem.md) concerns choosing both maps so that the decoding-error [probability](probability.md) becomes small at a specified rate.

**Table of contents**

- [Maximal decoding error probability](maximal-decoding-error-probability.md)

## ↑ Ancestors (6)

1. [Discrete memoryless channel](discrete-memoryless-channel.md)
2. [Coding theory](coding-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Channel code](channel-code.md)
- [Channel decoder](channel-decoder.md)
- [Erasure-pattern counting bound for maximal decoding error](erasure-pattern-counting-bound-for-maximal-decoding-error.md)
- [Maximal decoding error probability](maximal-decoding-error-probability.md)
- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2023/3/b/solution.md)
- [Repeat-until-success coding over an erasure channel](repeat-until-success-coding-over-an-erasure-channel.md)
