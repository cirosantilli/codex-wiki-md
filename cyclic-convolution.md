# Cyclic convolution

↑ **Parent:** [Discrete convolution](discrete-convolution.md)

For arrays $a,b$ indexed by [integers](integer-split.md) modulo $k$, their cyclic convolution is

$$
(a*_k b)_r=\sum_{i=0}^{k-1}a_i b_{(r-i)\bmod k}.
$$

When $a_i$ and $b_j$ count choices with respective [residue classes](residue-class.md) $i$ and $j$, the cyclic convolution counts pairs whose sum has [residue class](residue-class.md) $r$. Repeated cyclic convolution therefore counts sums of longer sequences. The [discrete Fourier transform](discrete-fourier-transform-split.md) converts cyclic convolution into pointwise multiplication.

## ↑ Ancestors (7)

1. [Discrete convolution](discrete-convolution.md)
2. [Convolution](convolution.md)
3. [Fourier analysis](fourier-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
