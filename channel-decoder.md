# Channel decoder

↑ **Parent:** [Discrete memoryless channel](discrete-memoryless-channel.md)

A deterministic [channel decoder](channel-decoder.md) maps a received length-$n$ word over the output [alphabet](alphabet.md) $\mathcal Y$ to an estimated message label. Given message $m$, successful decoding means $g(Y^n)=m$, where $Y^n$ is the random received word after the [communication channel](communication-channel.md) acts on the [channel encoder](channel-encoder.md)'s word $f(m)$. The [channel decoder](channel-decoder.md) can recover a message despite changed symbols because it uses the relationships among complete [codewords](codeword.md). The [Shannon second coding theorem](noisy-channel-coding-theorem.md) concerns choosing both maps so that the decoding-error [probability](probability.md) becomes small at a specified rate.

## ↑ Ancestors (6)

1. [Discrete memoryless channel](discrete-memoryless-channel.md)
2. [Coding theory](coding-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Channel decoder](channel-decoder.md)
