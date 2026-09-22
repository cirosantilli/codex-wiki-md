# Lossy compression

↑ **Parent:** [Data compression](data-compression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lossy_compression)

[Lossy compression](lossy-compression.md) reduces a representation while permitting irreversible changes to the original. The encoder can map distinct [inputs](input-computer-science.md) to the same [output](output-computing.md), so its decoder cannot recover both originals exactly. The useful question becomes how much storage is saved for an acceptable amount of distortion: [mean squared error](mean-squared-error.md) is one numerical criterion, but it does not by itself measure how noticeable a visual change is.

For example, storing the [arithmetic mean](arithmetic-mean.md) of four [grayscale](grayscale.md) [pixels](pixel.md) retains their average shade while discarding their arrangement. Blocks $\left(\begin{smallmatrix}0&100\\100&0\end{smallmatrix}\right)$ and $\left(\begin{smallmatrix}50&50\\50&50\end{smallmatrix}\right)$ both produce 50. The former has detail and the latter is uniform, yet the decoder receives the same value. [Lossy block averaging](lossy-block-averaging.md) makes this ambiguity, its [bit](bit.md) saving and its [mean squared error](mean-squared-error.md) exact.

**Table of contents**

- [Lossy block averaging](lossy-block-averaging.md)

## ↑ Ancestors (3)

1. [Data compression](data-compression.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Data compression](data-compression.md)
- [Image compression](image-compression.md)
- [Lossy compression](lossy-compression.md)
- [Rate-distortion theory](rate-distortion-theory.md)
- [Three-bit lossy Hamming code](three-bit-lossy-hamming-code.md)
- [Universal lossless shortening is impossible](universal-lossless-shortening-is-impossible.md)
