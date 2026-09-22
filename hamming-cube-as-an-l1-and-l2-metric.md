# Hamming cube as an L1 and L2 metric

↑ **Parent:** [Metric embedding](metric-embedding.md)

Use the $\{0,1\}^n$ convention for the [Hamming cube](hamming-cube.md) $H_n$. Its elements are length-$n$ [binary strings](binary-string.md), and their [Hamming distance](hamming-distance.md) counts the differing coordinates:

$$
k=d_H(x,y)=\sum_{j=1}^n|x_j-y_j|.
$$

Send each [binary string](binary-string.md) to the [vector](vector.md) with the same coordinates, by $\iota_n:H_n\to\mathbb R^n$. Every differing coordinate contributes $1$ both to the sum of absolute differences and to the sum of squared differences. Therefore the [L1 norm](l1-norm.md) and [L2 norm](l2-norm.md) give, respectively,

$$
d_1(\iota_nx,\iota_ny)=k,\qquad
d_2(\iota_nx,\iota_ny)=\sqrt{k}.
$$

This short coordinate calculation proves that the [L1 norm](l1-norm.md) gives an [isometric embedding](isometric-embedding.md), while [Euclidean distance](euclidean-distance.md) grows like the [square root](square-root.md) of the number of changed [binary digits](binary-digit.md). For example, $000$ and $101$ differ twice: their [Hamming distance](hamming-distance.md) and [Manhattan distance](manhattan-distance.md) are $2$, but their [Euclidean distance](euclidean-distance.md) is $\sqrt2$. Comparing [binary strings](binary-string.md) in these two geometric representations answers different questions even though the points have the same coordinates.

For distinct pairs $k$ ranges over every integer from $1$ to $n$. The [metric embedding](metric-embedding.md) into the [L2 norm](l2-norm.md) thus has sharp ratios

$$
\frac{d_2(\iota_nx,\iota_ny)}{d_H(x,y)}=\frac1{\sqrt{k}},\qquad
a=\frac1{\sqrt n},\quad b=1,\quad
\operatorname{dist}(\iota_n)=\sqrt n.
$$

Neighbors attain $b$ and opposite corners attain $a$. This computes the [bi-Lipschitz distortion](bi-lipschitz-distortion.md) of this coordinate map; it does not prove that every [metric embedding](metric-embedding.md) into an [L2 space](l2-space-is-a-hilbert-space.md) has at least this [bi-Lipschitz distortion](bi-lipschitz-distortion.md). Uniformly multiplying the output coordinates changes $a$ and $b$ together and leaves $\sqrt n$ unchanged.

<a id="image-hamming-distances-become-k-in-l1-and-square-root-of-k-in-l2-with-controls-independent-of-dimension"></a>
![](hamming-cube-distance-scaling.png)

**[Figure 2](#image-hamming-distances-become-k-in-l1-and-square-root-of-k-in-l2-with-controls-independent-of-dimension). Hamming distances become k in L1 and square root of k in L2, with controls independent of dimension**.

The important family distinction is that these coordinate maps have no dimension-independent bound on their [bi-Lipschitz distortion](bi-lipschitz-distortion.md) into the [L2 norm](l2-norm.md), yet they do give a [uniform coarse embedding of a family of metric spaces](uniform-coarse-embedding-of-a-family-of-metric-spaces.md). Pad each output [vector](vector.md) with zero coordinates to view all maps in the single [l2 sequence space](l2-sequence-space.md), an [L2 space](l2-space-is-a-hilbert-space.md) for [counting measure](counting-measure.md). Then the same functions

$$
\rho_-(t)=\rho_+(t)=\sqrt t\qquad(t\geq0)
$$

work for every $n$, and $\rho_-(t)\to\infty$. Similarly, padding into the [l1 sequence space](absolutely-summable-sequence-space.md) gives common controls $\rho_-(t)=\rho_+(t)=t$ and exact preservation of [Hamming distance](hamming-distance.md). These claims use unnormalized [Hamming distance](hamming-distance.md); replacing it by [normalized Hamming distance](normalized-hamming-distance.md) changes the family of source [metrics](metric.md).

The geometry has a practical origin: Hamming's 1950 paper uses the number of differing positions between [binary strings](binary-string.md) to study [error-correcting codes](error-correcting-code.md). Changing one [binary digit](binary-digit.md) moves to a neighboring corner, so a question about corrupted messages becomes a question about separation in the [Hamming cube](hamming-cube.md). [R. W. Hamming, Error Detecting and Error Correcting Codes, 1950, Section 5](https://ineffectivetheory.com/edu/papers/hamming-codes-1950.pdf)

## ↑ Ancestors (6)

1. [Metric embedding](metric-embedding.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Metric embedding](metric-embedding.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-155/1/solution.md)
- [Uniform coarse embedding of a family of metric spaces](uniform-coarse-embedding-of-a-family-of-metric-spaces.md)
