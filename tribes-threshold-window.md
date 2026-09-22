# Tribes threshold window

↑ **Parent:** [Tribes function](tribes-function.md)

For $m$ tribes of size $w$ with $m\sim(\log2)2^w$ and $n=mw$, the success probability under the [p-biased product measure](p-biased-product-measure.md) is $1-(1-p^w)^m$. Its $x$-quantile is $p_x=[1-(1-x)^{1/m}]^{1/w}$. For fixed $0<x<1$,

$$
p_x=\frac12+\frac1{2w}\log\frac{-\log(1-x)}{\log2}+O_x(w^{-2}).
$$

Thus the fixed-error window has order $1/\log n$. For small fixed error the leading coefficient grows with $\log(1/\varepsilon)$, so the general [Friedgut-Kalai sharp threshold theorem](friedgut-kalai-sharp-threshold-theorem.md) also has the correct error dependence up to absolute constants.

## ↑ Ancestors (8)

1. [Tribes function](tribes-function.md)
2. [Boolean function](boolean-function.md)
3. [Boolean hypercube](boolean-hypercube.md)
4. [Analysis of Boolean functions](analysis-of-boolean-functions.md)
5. [Combinatorics](combinatorics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
