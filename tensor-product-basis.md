# Tensor-product basis

↑ **Parent:** [Tensor product](tensor-product.md)

If $(e_1,\ldots,e_m)$ and $(f_1,\ldots,f_n)$ are [bases](basis.md) of [finite-dimensional vector spaces](finite-dimensional-vector-space.md) $V,W$ over $F$, then the $mn$ products $e_i\otimes f_j$ form a [basis](basis.md) of $V\otimes_F W$. There is one independent [coordinate](coordinate-linear-algebra.md) for every pair of indices.[§9D, Theorems 9.72 and 9.74, printed pp. 372–373: dimension and tensor-product basis](linear-algebra-done-right-by-sheldon-axler-4th-edition.md)

For a proof outline, [bilinearity](bilinearity.md) expands each [pure tensor](pure-tensor.md) as

$$
\left(\sum_i v_ie_i\right)\otimes\left(\sum_j w_jf_j\right)=\sum_{i,j}v_iw_j(e_i\otimes f_j),
$$

so these products form a [spanning set](spanning-set.md). For [linear independence](linear-independence.md), take the [coordinate functionals](coordinate-functional.md) $e^k,f^\ell$ from the two [dual bases](dual-basis.md). The [bilinear map](bilinear-map.md) $(v,w)\mapsto e^k(v)f^\ell(w)$ induces a [linear functional](linear-functional.md) $\lambda_{k\ell}$ on the [tensor product](tensor-product.md), satisfying $\lambda_{k\ell}(e_i\otimes f_j)=\delta_{ki}\delta_{\ell j}$. Applying it to a proposed zero [linear combination](linear-combination.md) selects just $c_{k\ell}$, forcing every coefficient to vanish. Thus [dimensions](dimension-vector-space.md) multiply, rather than add. This finite-dimensional count includes a zero factor, whose [tensor product](tensor-product.md) has [dimension](dimension-vector-space.md) zero.

**Table of contents**

- [Tensor-product coefficient matrix](tensor-product-coefficient-matrix.md)

## ↑ Ancestors (7)

1. [Tensor product](tensor-product.md)
2. [Multilinear algebra](multilinear-algebra-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323/5/i/solution.md)
- [Tensor product](tensor-product.md)
- [Tensor-product coefficient matrix](tensor-product-coefficient-matrix.md)
- [Tensor-product operator](tensor-product-operator.md)
- [Universal property of a tensor product](universal-property-of-a-tensor-product.md)
