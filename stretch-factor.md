# Stretch factor

↑ **Parent:** [Bi-Lipschitz distortion](bi-lipschitz-distortion.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stretch_factor)

For an [injective function](injective-function.md) that does not increase distances, one stretch-factor convention measures the largest compression that must be undone:

$$
t(f)=\sup_{x\ne y}\frac{d_X(x,y)}{d_Y(f(x),f(y))}
=\operatorname{Lip}(f^{-1}).
$$

If the sharp [Lipschitz constant](lipschitz-constant.md) of $f$ is one, this equals [bi-Lipschitz distortion](bi-lipschitz-distortion.md). Fixing the scale matters: uniform compression $f(x)=x/2$ has stretch factor two in this convention, but [bi-Lipschitz distortion](bi-lipschitz-distortion.md) one. In a [geometric spanner](geometric-spanner.md), the corresponding stretch factor is the largest graph-route distance divided by direct [Euclidean distance](euclidean-distance.md); the graph-to-Euclidean identification does not increase distances. [Gudmundsson, Narasimhan and Smid, Geometric Spanners, §1: the stretch-factor convention](https://people.scs.carleton.ca/~michiel/encyc_geometric_spanners.pdf).

## ↑ Ancestors (7)

1. [Bi-Lipschitz distortion](bi-lipschitz-distortion.md)
2. [Metric embedding](metric-embedding.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Bi-Lipschitz distortion](bi-lipschitz-distortion.md)
- [Geometric spanner](geometric-spanner.md)
