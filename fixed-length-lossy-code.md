# Fixed-length lossy code

↑ **Parent:** [Rate-distortion function](rate-distortion-function.md)

A [fixed-length lossy code](fixed-length-lossy-code.md) maps a block of $n$ source symbols to one of $M_n$ messages, then maps that message to a reconstruction block. The [encoder](channel-encoder.md) and [decoder](channel-decoder.md) together define the reconstruction. Its rate is $\log_2 M_n/n$ [bits](bit.md) per source symbol; an implementation using a fixed binary message needs $\lceil\log_2 M_n\rceil$ transmitted [bits](bit.md) per block. Its performance also depends on [expected distortion](expected-distortion.md), block length, and the chosen [distortion measure](distortion-measure-information-theory.md).

## ↑ Ancestors (7)

1. [Rate-distortion function](rate-distortion-function.md)
2. [Rate-distortion theory](rate-distortion-theory.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Fixed-length lossy code](fixed-length-lossy-code.md)
- [Shannon's rate-distortion theorem](shannon-s-rate-distortion-theorem.md)
