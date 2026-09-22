# Universal lossless shortening is impossible

↑ **Parent:** [Data compression](data-compression-split.md)

Fix $n\geq1$. There is no [injective function](injective-function.md) from all length-$n$ [binary strings](binary-string.md) to [binary strings](binary-string.md) of length strictly less than $n$. There are $2^n$ possible [inputs](input-computer-science.md), but even allowing the empty string gives only

$$
\sum_{k=0}^{n-1}2^k=2^n-1
$$

possible shorter [outputs](output-computing.md). The [finite geometric series](finite-geometric-series.md) and [pigeonhole principle](pigeonhole-principle.md) leave at least two [inputs](input-computer-science.md) sharing an [output](output-computing.md), which prevents exact decoding. For $n=3$, eight [inputs](input-computer-science.md) compete for the empty string and the six strings `0`, `1`, `00`, `01`, `10`, `11`.

This counting argument includes any [file header](file-header.md) or other information sent to the decoder. An [algorithm](algorithm-split.md) chosen separately for each [input](input-computer-science.md) must also be identified to the receiver; its description is not free. A useful compressor saves space on some [inputs](input-computer-science.md) while leaving others unchanged or making them longer. [Lossy compression](lossy-compression.md) avoids the exact-recovery requirement by deliberately allowing several [inputs](input-computer-science.md) to share an [output](output-computing.md).

## ↑ Ancestors (3)

1. [Data compression](data-compression-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Deflate compression overhead](deflate-compression-overhead.md)
