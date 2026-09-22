# Syndrome decoding

↑ **Parent:** [Syndrome](syndrome.md)

For a [linear code](linear-code.md) with [parity-check matrix](parity-check-matrix.md) $H$, write the received word as $y=c+e$, where $c$ is a [codeword](codeword.md) and $e$ an error pattern. Its [syndrome](syndrome.md) depends only on the error because $Hc^T=0$. A syndrome decoder chooses a representative error $\widehat e$ with that syndrome and returns $y-\widehat e$. Choosing a minimum-[Hamming weight](hamming-weight.md) representative gives [minimum-distance decoding](minimum-distance-decoding.md); within the guaranteed correction radius it recovers the unique transmitted [codeword](codeword.md). Several representatives may tie outside that radius.

## ↑ Ancestors (8)

1. [Syndrome](syndrome.md)
2. [Parity-check matrix](parity-check-matrix.md)
3. [Linear code](linear-code.md)
4. [Coding theory](coding-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Error-correcting code](error-correcting-code.md)
