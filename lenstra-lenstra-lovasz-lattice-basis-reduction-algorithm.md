<h1 id="lenstra-lenstra-lovasz-lattice-basis-reduction-algorithm">Lenstra-Lenstra-Lovász lattice basis reduction algorithm</h1>

↑ **Parent:** [Euclidean lattice](euclidean-lattice.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lenstra–Lenstra–Lovász_lattice_basis_reduction_algorithm)

For an integer basis of a [Euclidean lattice](euclidean-lattice.md), the algorithm uses integer column operations and swaps to obtain a size-reduced basis with Gram-Schmidt coefficients $|\mu_{ij}|\le1/2$ and the condition $\delta\|b_i^*\|^2\le\|b_{i+1}^*\|^2+\mu_{i+1,i}^2\|b_i^*\|^2$. It preserves the lattice and exposes short vectors and near-relations. It is useful for improving proven Diophantine bounds by encoding scaled logarithms in integer coordinates. A certified lower bound for every nonzero lattice vector is $\min_i\|b_i^*\|$: in a nonzero integer linear combination, project onto the last nonzero Gram-Schmidt direction. Better-reduced bases improve this lower bound. Rounding and logarithm errors must still be bounded before turning it into a certified lower bound for a [logarithmic form](linear-form-in-logarithms-of-algebraic-numbers.md).

## ↑ Ancestors (6)

1. [Euclidean lattice](euclidean-lattice.md)
2. [Fourier analysis](fourier-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
